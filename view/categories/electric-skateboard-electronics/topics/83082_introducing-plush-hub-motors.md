# Introducing&hellip; Plush Hub Motors

### Replies: 100 Views: 2872

## \#1 Posted by: evoheyax Posted at: 2019-02-03T23:58:45.080Z Reads: 521

```
I've been focusing a lot of time lately into two things. Finding permanent work: Check! So now I'm on to the next part: Developing a pneumatic hub motor based on my experience of working with hummie.

The goals of this project are simple:
- Supports 6-inch, 7-inch, or 8-inch tires
- At least 2000 watts con per motor
- Easy swapping of tires
- As compact in width as possible while still achieving the performance required (67mm in this case from tip to tip)

Currently, the design uses a 6430 stator which I have found a supplier of.

Speed wise, looking to hit around 40 kv. This would give the following top speeds roughly:
- 6-inch: 26 mph
- 7-inch: 31 mph
- 8-inch: 35 mph

![PNG|451x500](upload://2jTP3CvV5E9fCHfts8DzRfZP6mx.jpeg)

![PNG|461x500](upload://2Yu3CadmlxIEVare7azwzo2KqUe.jpeg) 

![PNG|404x500](upload://dSjJ9bEM7xF1wqL1I6qq2V9PewA.jpeg)

![PNG|577x500](upload://s5zaImu78rsmJihdsEL7yLvqD5V.jpeg)

**Where I need the communities help**

First off, I need experienced view points about trucks:
Which trucks do you like and why?
What is the best wheel case to you?
RKP/TKP/Spring truck like trampa?

Second piece is I'm wondering if there's any expert lathers that could assist in machining 2 or 4 prototypes? Getting the first couple to assure everything is correct is the most costly part as china charge an arm and a leg, plus they are not going to be doing much for the next month.

The hope is to bring these to market by no later than the end of this year. Hard to comment on pricing, but aiming around $700 for a 2wd with front wheels and both trucks. This might be hard though so we will see.

Thank you for checking it out!
```

---
## \#2 Posted by: Pedrodemio Posted at: 2019-02-04T00:17:56.676Z Reads: 485

```
What about doing something similar to carvon first iteration, motor partially inside the wheel, but far off back that the valve is not in the way and you can use a larger diameter stator?
```

---
## \#3 Posted by: evoheyax Posted at: 2019-02-04T02:27:56.493Z Reads: 476

```
This is a pretty decent size stator. I’m personally more attracted to hub motors than dd setups.
```

---
## \#4 Posted by: Friskies Posted at: 2019-02-04T02:38:39.357Z Reads: 477

```
Looks sick!!! If you are using something similar to hummies bearings I would make sure they are sealed - if you are thinking off road applications. Those huge inner bearings do not like dirt and sand haha.
```

---
## \#5 Posted by: mishrasubhransu Posted at: 2019-02-04T09:34:21.913Z Reads: 435

```
Looks Awesome! And congratulations on your new job. Is it an engineering job?

As for my thoughts on the hub motor, I would suggest that you only focus on the rear wheels and trucks to start with. I like wide trucks with pneumatics. Pretty happy with TB218. You can start with iterating with 3d printed parts even before you machine anything. Try to get better deals from the supplier. You know how cheap hub motors are these days (the skull board hubs with 105 tires and both trucks were selling for $180). You can probably use those prices to negotiate better. I think that's it.
```

---
## \#6 Posted by: Scooterskater Posted at: 2019-02-04T13:19:08.265Z Reads: 399

```
Nice! You could also try to bring that to the scooter industry.  Innovation is not keeping up with the laws . There are no 9in x 3.5-4 wheels that are electric for scooters (standard electric wheel chair mobility scooter) aka cheap . Make something that killed 2-3 birds ? I always felt the scooter, and skate board were a close industry.  Keep innovating.  It's like the dawning of the auto industry.  There were many "great ideas" but only few got to keep them.
```

---
## \#7 Posted by: evoheyax Posted at: 2019-02-04T15:56:30.757Z Reads: 366

```
No, unfortunately, it's not an engineering position, but when I get to full time, the pay is very good for a single person, lol.

The front truck will be easier this time around. Not having to produce wheels from the ground up is a big plus.

I'm not sure how much it'll cost to machine, but it's hard to compare these to anything else on the market. I will be focusing on quality parts. Hoping to use n52sh magnets for example. I'm planning on building these in house, like the hummie hubs.
```

---
## \#8 Posted by: mishrasubhransu Posted at: 2019-02-04T16:12:04.903Z Reads: 334

```
Yeah for sure you'll use quality bearings and magnets but machining cost makes sense to remain close. So just asking to bargain well citing those examples.
```

---
## \#9 Posted by: evoheyax Posted at: 2019-02-04T16:22:46.342Z Reads: 334

```
Oh I will look. It's a tough cookie to crumble. I remember with hummie, it took over a dozen places to get the prices he got today, which was pretty reasonable. The next best was many times higher. It's not an easy game, and in this case, the motor diameter is much larger, so we're talking about 4 times as much steel in the first place.

The issue is the magnets, magnet glue, and motor winding epoxy are not cheap. And stators, we'll see.
```

---
## \#10 Posted by: mishrasubhransu Posted at: 2019-02-04T16:24:36.104Z Reads: 319

```
[quote="evoheyax, post:9, topic:83082"]
so we’re talking about 4 times as much steel in the first place
[/quote]
:open_mouth: forgot about the squared law for a bit.
```

---
## \#11 Posted by: evoheyax Posted at: 2019-02-04T16:27:08.279Z Reads: 302

```
yea, I'm starting at 110mmx110mm Hummie hubs are starting at almost half of that. So almost 4 hummie hubs could be made from the same block. That will be the biggest issue imo of getting these affordable.
```

---
## \#12 Posted by: mishrasubhransu Posted at: 2019-02-04T16:35:39.448Z Reads: 299

```
Have you considered aluminum as the build material or at least the majority of it? All hub motors wheels are usually aluminum, like the ones used on scooter. The shock and fatigue from the vibration it's much less with pneumatics, so you should definitely consider it. There is no point in over engineering if it's not needed.
```

---
## \#13 Posted by: kuphjr Posted at: 2019-02-04T16:42:41.634Z Reads: 298

```
Would this be an open source project?  Would you post your parts list and any CAD files?  I am a computer science / engineering student and I have long wanted to do a project where I construct my own motor.  I have access to the machine shop at my university with a cnc, metal lathe and pretty much any tool I could ever need.

If you want to keep the IP behind this project private I totally understand, but I figured it is worth a shot asking for the designs as you finish them.
```

---
## \#14 Posted by: mishrasubhransu Posted at: 2019-02-04T18:07:03.216Z Reads: 278

```
There is a different different opensource hub motor design on this forum. Give it a search.
```

---
## \#15 Posted by: Minim Posted at: 2019-02-04T18:32:16.917Z Reads: 278

```
I dont have a cnc lathe and I haven’t used my manual lathe long enough to do real parts on it but if you need something CNC milled I can help  out. For prototypes I’m pretty sure a milled hub will do but you will ofc get better accuracy with a lathe ^^ Shoot me a PM if you don’t find another option.
```

---
## \#16 Posted by: treenutter Posted at: 2019-02-04T19:34:49.962Z Reads: 272

```
@evoheyax I'm really glad you're doing this, after our hangout at the renegade weekend I've been waiting to see what you'd do with all the knowledge and experience you've got. Congrats for getting to this point! I'm excited to see how this turns out.  

I'm also curious about how the heat generated by a hub motor might impact the integrity of a tire (vs a urethane sleeve like most hub motors).
```

---
## \#17 Posted by: Clintroberts Posted at: 2019-02-11T17:00:52.310Z Reads: 243

```
Okay what is the benefit of a hub driving pneumatics that are large in diameter. You can already do with direct drive and 6” wheels easily. Everybody is doing large pneumatics. Now let’s talk about a hub motor driving pneumatics that are wide and say 105mm in diameter like a skateboard wheel. I want to be low to the ground and have a super smooth ride without all the noise/weight of belt driven motors.
```

---
## \#18 Posted by: evoheyax Posted at: 2019-02-11T17:51:27.547Z Reads: 251

```
In terms of benefits vs direct drive, one big benefit is ease to switch tires and tubes.

**Direct drive:** Remove a nut, then pull the wheel off of an adapter, then unscrew the hub split it in half, and do the replacement

**Hub Motor:** 7 screws, plate comes off, and tire and tube come off.

It's also simpler in construction. There's no adapter, the wheel locking mechanism is built straight into the motor.

In terms of DD motors, I haven't see any 40 kv DD motors on the market. This is a problem as I stated before because the top speed will be too high, resulting in weaker torqure than a motor with a reasonable top speed (i.e. lower kv).

It's also way more compact than a DD motor. By adding adapters, motor 100% outside of the wheel, you lose space. In this design, 80% of the motor is actually inside of the wheel. There's a slight hangout for the turns on the ends of the stators and for bearings and the C-Clip.

So what do you get? Less parts (simpler design), easier to replace tires/tubes, correct kv (and thus, reasonable top speed), and more compact design that keeps almost the entire motor in the frame of the wheel, allowing for more stealth (this is the main reason many looked at hub motors over DD motors in the first place).
```

---
## \#19 Posted by: Clintroberts Posted at: 2019-02-11T18:11:19.718Z Reads: 231

```
I just meant why make a hub with a big tire. Everyone has large tires already whether belt or DD. I own belt pneumatic, DD with urethane and belt urethane. I have owned hubs too. I would only use hub with pneumatics as the thin urethane is no good for smooth riding or longevity of the hub motor imho. I’m interested in seeing a hub pneumatic being done. Just wish someone would make it small in diameter as I want some drop but not major drop and want to be closer to the ground (not to mention having a giant wheel).
```

---
## \#20 Posted by: FredrikHems Posted at: 2019-02-11T18:17:36.147Z Reads: 227

```
Have you though about doing a mix between hub motor and direct drive? Like a direct drive thats go inside the wheel hub aswell. Wondering why anyone havent done this yet, as it would result a lot more torque. :thinking:
```

---
## \#21 Posted by: evoheyax Posted at: 2019-02-11T18:30:25.148Z Reads: 222

```
I don't think I understand what you are trying to say. What do you mean by small in diameter? The goal of this is to create a motor similar to a trampa hub (without a motor). The ride height will be based on the diameter of the tire you use, so you can use a 6 inch tire and get lower to the ground or an 8 or 9 inch and get higher from the ground. The inner diameter of most penultimates is about 93.5mm, with walls around 110mm to keep the tire on. Then there is about 30mm inside of the walls (width of the tire). This is the constraint of pnuematic wheels, and making a motor with a smaller diameter would mean you need to make custom pneumatic tires and tubes and that even wouldn't necessarily get you closer to the ground, unless the diameter of the tire is less.
```

---
## \#22 Posted by: evoheyax Posted at: 2019-02-11T18:38:38.102Z Reads: 226

```
[quote="FredrikHems, post:20, topic:83082"]
as it would result a lot more torque.
[/quote]

I think your confused about torque. The torque between a hub and DD motor with the same sized stator and same winding pattern and same esc and battery will be the same. The location of the motor doesn't matter, since the gearing ratio stays the same (1:1).

Unless you mean by you can use a much larger diameter stator (since the stem doesn't get in the way). This would make sense, and is a reason I thought about it. It's a nice idea. But I believe I can still get good performance from this stator (it's much larger in diameter than most stators used in eboards).

Thus if it can be fit in wheel to have the performance needed, why not fit it in wheel?
```

---
## \#23 Posted by: FredrikHems Posted at: 2019-02-11T18:51:06.652Z Reads: 217

```
Nah, not like that. 
Imagine if you have a motor which both sits inside the wheel (like a hub motor), aswell as on the hangar (direct drive). Lest say you have a hub motor which is 40mm in length, and you have a direct drive motor which is 40mm in length. Now combine these, and you will have an 80mm long motor. 
Make sense now?
```

---
## \#24 Posted by: MoeStooge Posted at: 2019-02-11T18:54:23.265Z Reads: 225

```
Yea Buddy. At 50v looking at 9kw per wheel.  
![Screenshot_20190211-105117|281x500](upload://hoZaYPvENNWxsR8hFCmcwDVrR2H.png) 
https://rover.ebay.com/rover/0/0/0?mpre=https%3A%2F%2Fwww.ebay.com%2Fulk%2Fitm%2F183638309572
```

---
## \#25 Posted by: evoheyax Posted at: 2019-02-11T18:54:24.026Z Reads: 214

```
I understand what your saying and I understood it before.

Basically, you end up with a bigger stator. That won't give more torque still. It will just run cooler, unless the original stator is so small that the stator saturates and can't give the torque it's designed for.
```

---
## \#26 Posted by: evoheyax Posted at: 2019-02-11T18:59:12.568Z Reads: 204

```
At some point, all of the power is useless without
A) bigger contact patches
B) a way to hold on for dear life.

You know that 10kw across the board is insane, dangerous really, which is why you throttle back the watts.

So at some point, it comes down to what is practical. I'm aiming for 8kw total (2kw per motor x 4 if you want power) or 4kw total (2kw x 2 for sane people who still want crazy power).
```

---
## \#27 Posted by: evoheyax Posted at: 2019-02-11T19:03:12.283Z Reads: 189

```
I think that it's just not necessary to make it much longer. If I can not get the performance I'm looking for from this in wheel design, my next option would be to extend it outward until it is large enough.
```

---
## \#28 Posted by: Pedrodemio Posted at: 2019-02-11T19:23:50.505Z Reads: 185

```
The questions that you will hopefully answer once these are tested is: Is a stator narrow enough to fit just inside the tires capable of producing sufficient torque?

After that we can debate if a bigger stator is needed or not
```

---
## \#29 Posted by: Saturn_Corp Posted at: 2019-02-11T19:39:09.191Z Reads: 185

```
I might have missed this earlier in the thread, but will these have a wide enough range of torque/speed to run well with a range of 6-9 inch tires? Say it has great torque on 6 inchers, would it have enough to be acceptable running 9 inchers? Seems to me like you're asking a lot for it to be ideal with such a potential difference in wheel sizes but I don't know enough yet to make any assumptions.
```

---
## \#30 Posted by: evoheyax Posted at: 2019-02-11T19:41:35.248Z Reads: 182

```
That is the goal here. 2wd should be great on 6 and 7 inch tires, and 4wd should be great with 6, 7, 8, and 9 inch tires. I listed projected top speeds in the first post.
```

---
## \#32 Posted by: FredrikHems Posted at: 2019-02-11T19:58:44.254Z Reads: 186

```
[quote="evoheyax, post:22, topic:83082"]
larger diameter stator
[/quote]
Sorry, misunderstood. But I think you mean length, and not diameter here?^^ 

Anyway, wouldnt a 6374 produce more torque than a 6355? This is my experience atleast from riding both on same vesc settings.
```

---
## \#33 Posted by: evoheyax Posted at: 2019-02-11T20:28:59.499Z Reads: 198

```
In theory, no.

Torque (km) is proportional to kv and the watts you put into it. The issue is when a motor's stator is too small for the amount of watts you push into it, your stator saturates, and loses torque and efficiency.

If you take hummie v1 hub motors, you could the same torqure as the v4 motors (double the stator length than v1).

You can take a really tiny motor and get the same torque as a big motor. The difference is the little motor will get hotter than the bigger motor. Thus the bigger motor can take more current and provide a stronger acceleration. If you only change motor size and no amp limit settings, you should experience the same torque, unless you saturate the stator in the smaller stator.

Bigger stator = more copper in the motor = lower winding resistance (since you can fit more copper in each wind). Lower winding resistance = less copper losses = less heat generated from the resistance of the copper wire. It also means more steel in the stator (which is important for flipping the poles) and you also have more magnets.

Thus, bigger motor = bigger elector magnet and permanent magnet = can handle more watts without heat issues = more powerful acceleration. But do not confuse this for torque. Torque is a constant value. The actual rate of acceleration is a different story.

If you want to see this, take two different size motors on the same truck (different wheels). Put one into a vesc at a time, same settings (set them lower so you don't saturate the stator) and do an acceleration test. You should feel a similar acceleration. But the smaller motor (assuming they are the same motor kv's, same winding and winding pattern, same brand, just different stator size) will be hotter (easy to measure with cheap hobbyking laser thermometer). Now up the amp limits some more, and you'll see the heat difference between the motors more drastically.

On the hummie hubs, the one piece that made a difference is the wider wheel base, which gives more traction. At 30a per motor (50v), wheels would slip on the hummie v1. On the hummie v4, it takes over 50a per motor to get the wheel to slip. Thus I get better acceleration on the v4's than the v1's, even though the torque is the same.
```

---
## \#34 Posted by: Hummie Posted at: 2019-02-11T20:48:57.760Z Reads: 164

```
dont think wheelbase would determine if the wheel slips.   

the peak torque output of the v4 is much more than the v1 as its over twice the stator size. 

why the new wouldnt slip but the old would given the same esc amp settings is likely because the v4 use a bigger softer tire.   otherwise they should slip more as they're lower kv and more torque per amp.
```

---
## \#35 Posted by: rusins Posted at: 2019-02-11T20:56:16.413Z Reads: 171

```
The forum must have been hiding this topic from me, noticed it only today :thinking:

First of all: THIS SEEMS AWESOME!  Lowering the amount of parts for AT builds is much needed.
Secondly: Small pneumatic wheels like the Bergmeisters seem to be a hot trend right now. Assuming these hubs would fit sixshooter tires, they would also fit Bergmeister tires (same core/internal wheel size I believe). Only problem is that at 5" and just 40KV, top speed is significantly lacking. Seeing as a lot of people prefer the 30mph sweet spot, was just wondering if you'd be open to having a 55kv motor option as well.
```

---
## \#36 Posted by: FredrikHems Posted at: 2019-02-11T21:15:21.976Z Reads: 169

```
Thank you for the very detailed post! :yum: 

I guess I used the word torque wrong. so you should only experience better acceleration with a longer stator if the smaller gets hot enought to be become saturated, right?
```

---
## \#37 Posted by: evoheyax Posted at: 2019-02-11T21:44:53.503Z Reads: 180

```
[quote="Hummie, post:34, topic:83082"]
dont think wheelbase would determine if the wheel slips.
[/quote]

Never said wheel base, I said contact patch. Larger contact patch = more grip, that's just basic science. And I'm not just talking about the new wheels, but also the v3 motors too, which those crappy poured wheels.

[quote="Hummie, post:34, topic:83082"]
the peak torque output of the v4 is much more than the v1 as its over twice the stator size.
[/quote]

Formula?

Everything I've seen (online calculators and other topics on this forum and from what you've told me personally), is that the torque is a constant, called kt, which is propositional to kv, which is decided by the wind. https://calc.3dservisas.eu/ for example calculate torque without considering magnets or stator size.

[quote="Hummie, post:34, topic:83082"]
otherwise they should slip more as they’re lower kv and more torque per amp.
[/quote]

First v1 hummie hubs were all under 85 kv, most where just over 80 kv. My v4's are 80 kv, 85 kv, and 2 at 90 kv. So they are not a lower kv for me, actually, the opposite.
```

---
## \#38 Posted by: Hummie Posted at: 2019-02-11T22:26:29.081Z Reads: 162

```
Wheel base. [quote="evoheyax, post:33, topic:83082"]
On the hummie hubs, the one piece that made a difference is the wider wheel base
[/quote]
But a larger contact patch isn’t always better grip and you can get fast wearing soft sticky tires with better traction or hard n long lasting n bad traction  

I agree the kv/kt reveals what torque the motor will put out with general use but if you’re overloading the motor trying to get as much torque as possible the bigger stator won’t saturate and get extra hot, as you said.
```

---
## \#39 Posted by: evoheyax Posted at: 2019-02-11T22:28:10.242Z Reads: 167

```
[quote="Hummie, post:38, topic:83082"]
But a larger contact patch isn’t always better grip and you can get fast wearing soft sticky tires or hard.
[/quote]

I don't disagree with this either. It's totally possible this played a role in my experience also. But generally speaking, same wheel with a longer contact patch = more grip.
```

---
## \#40 Posted by: Dagad Posted at: 2019-02-19T12:36:02.889Z Reads: 168

```
Wow - thanks so much for this - really happy you are determined to create a proper hub motor for 6-8” pneumatics. 

I agree with your measurements 93.5mm or about 3.75” for tire rim plus the height of walls sticks up from that to hold the tire on.  I do think you could increase the width a little - perhaps 40-50mm rim width between walls.  

The trick/problem is that stem to inflate the tire takes up so much space below the 93.5mm rim so you might lose 10mm for that (though you could also use that space to attach tire rim to motor). You would probably end up with  a max motor diameter of about 80mm (at least that’s how I have it pictured in my head - wish I could think of a way to get a larger diameter motor) 

I have been trying to figure out pneumatic hub motors for my current project.   Was considering buying TRAMPA superstar rims (plastic) or more likely megastars (aluminum) without the hubs and stuffing your existing hummie hub in there and finding someone to mill out a simple interface between them.   Seems do-able - am I missing something - why hasn’t this been done before?
```

---
## \#41 Posted by: Dagad Posted at: 2019-02-19T13:09:19.620Z Reads: 165

```
A few other ideas:

if you’re machining your own rims, you could create/machine a rim profile that is similar to some automotive or bicycle rims.  The rim profiles sometimes incorporate a “hook” (small recess as well as a bump) that hold the tire bead on more securely. . . This in conjunction with a permenantly installed (and strategically placed valve stem) might save some space allowing increased diameter of motor and have the added benefit allowing tires to be run tubless.  Tubless tires save a lot of weight and have other benefits.   

Speaking of weight - please count every gram as you design this thing - a heavy weight will dissuade majority and really take the fun out of it. 

Regarding your decision of 40kv.  That is PERFECT for me - in fact could go even lower!
```

---
## \#42 Posted by: Goonman Posted at: 2019-02-20T11:04:31.810Z Reads: 165

```
Hub is direct drive.
```

---
## \#43 Posted by: Goonman Posted at: 2019-02-20T11:10:34.923Z Reads: 162

```
Already have hub motor off road. Lunyee make scooter motors. L faster make channel trucks for the motors. There are lots of little things to improve but they work well. I'm 105+/-3kg and my ghetto board v2 is approx 25kg. Goes off road like a champ. Maybe talk to lunyee.![20181125_185517|690x388](upload://18HCuOW5DFmOxYViPTeeHZHDFp9.jpeg)
```

---
## \#44 Posted by: Mich21050 Posted at: 2019-02-20T11:39:57.594Z Reads: 164

```
@b264 :joy:
```

---
## \#45 Posted by: janpom Posted at: 2019-02-20T12:27:31.643Z Reads: 162

```
You should send him the sticker. :laughing:
```

---
## \#46 Posted by: evoheyax Posted at: 2019-02-20T15:47:35.461Z Reads: 160

```
Thank you for posting that here. It's great to have a discussion about why these are not suitable for me.

Here's the issues: 
- These are 350w motors and I want 2000w+ per motor.
- I want hub motors with a through axle, not held to a plate that they call a truck with 4 screws.

This requires a design from the ground up. Because those are not scooter motors. Some scooter motors can actually do 1000w each. Those are hover board motors wound to a higher kv.

Why are these such low power? They use a tiny stator with little copper and weak magnets. n52sh's cost 10-20x the cost of a n42, which is a standard motor magnet with a fraction of the magnetism of a n52sh and much lower heat rating. They make something that works, but they don't engineer it to work great.

A 350w motor is very easy to build, just chose any magnet, any stator in a certain range, any copper fill, ect. a 2000w motor is not because you need to very strong magnets, as much copper as possible, as big of a stator as possible, and you need the flux to flow properly. Thus why you see 350w motors on the market, and not 2000w motors.
```

---
## \#47 Posted by: evoheyax Posted at: 2019-02-20T15:55:59.976Z Reads: 164

```
Weight will be a considered factor. Obviously, they won't be light. But I will do my best to keep weight down.

The reason no one has put a pneumatic on a hummie hub is simply because it requires a custom piece, wither to bridge the hub to wheel or a piece that has the grove for the wheel. Neither are easy. And neither maximize the stator size. Can fit a much bigger diameter stator in this that the hummie hubs 47mm stator.

An announcement for everyone. I wish I could of had more feedback from pneumatic riders on this forum about trucks, but they have been silent. I have decided to design this for the Trampa Vertigo truck. This seems like a great truck, compatible with a wide range of decks, and has a nice square profile to lock the motor in (instead of motor mounts as it was designed for).

![trampa|690x315](upload://a2FhqgknOetB4eYEdVAWsnPR28g.jpeg)
```

---
## \#48 Posted by: Sn4pz Posted at: 2019-02-20T17:13:17.017Z Reads: 151

```
When youre done designing these, do you think they will fit onto the mini vertigo trucks as well?
```

---
## \#49 Posted by: Vanarian Posted at: 2019-02-20T17:33:34.968Z Reads: 152

```
[quote="evoheyax, post:1, topic:83082"]
the design uses a 6430 stator which I have found a supplier of.
[/quote]

You sexy manizer 🍖 hitting you a PM for the stator supplier! Pretty sure I can squeeze that into my skates wheels later!
```

---
## \#50 Posted by: mutantbass Posted at: 2019-02-20T17:42:26.247Z Reads: 154

```
You know trampa came out with a vertigo electric hanger just for stuff like this

https://www.trampaboards.com/cnc-precision-made-vertigo-emtb-hanger--used-in-conjunction-with-all-pro-series-mountainboard-motor-mounts--16-inch-wide-p-26040.html

Have a look. Might be a better option
```

---
## \#51 Posted by: Goonman Posted at: 2019-02-20T19:01:16.847Z Reads: 144

```
Lunyee does custom windings
Did you check their options?
I measured these at about 1000w per each motor.
They really aren't what you think they are. With a big rolling diameter they go over rough terrain and can do 38kmh on the flat.
I'm sure they can find more power and trim some fat. But you know $$$$$
QS motor will make a hub with the a custom axle.
Weight and money will always be the issue..... for just about anything actually come to think about it.
```

---
## \#52 Posted by: Sn4pz Posted at: 2019-02-20T19:04:22.347Z Reads: 144

```
Hes stated before he wants to be able to hit 45mph, so unfortunately 38kms is out of the question. Also, dont forget that evo worked on hummies hubs with him, so im sure he has a very good idea of where to start :)
```

---
## \#53 Posted by: b264 Posted at: 2019-02-20T20:26:48.838Z Reads: 138

```
Still has to keep pushing the cheap china stuff or he won't earn his paycheck this week though.
```

---
## \#54 Posted by: Sn4pz Posted at: 2019-02-20T20:29:31.251Z Reads: 143

```
I must not know what youre talking about, care to enlighten me?
```

---
## \#55 Posted by: Bor.inc Posted at: 2019-02-20T20:36:50.551Z Reads: 141

```
Well there are some users that are just payed by chinese manufactures that try to endorse that brand
```

---
## \#56 Posted by: Sn4pz Posted at: 2019-02-20T20:38:21.337Z Reads: 139

```
So I shouldnt be excited about any of this? :cloud_with_rain: :( :cloud_with_rain:
```

---
## \#57 Posted by: Bor.inc Posted at: 2019-02-20T20:41:15.520Z Reads: 141

```
I have no idea, but I think that's what @b264 meant (correct me if im wrong)

But I would be excited for this at hubmotor @evoheyax is making if im you because it looks awesome
```

---
## \#58 Posted by: b264 Posted at: 2019-02-20T20:45:38.648Z Reads: 140

```
[quote="Bor.inc, post:55, topic:83082, full:true"]
Well there are some users that are just payed [sic] by chinese manufactures that try to endorse that brand
[/quote]


:arrow_up:  yes, this
```

---
## \#59 Posted by: evoheyax Posted at: 2019-02-21T03:12:54.794Z Reads: 136

```
Shit, that's the one I meant to order lol. I can't find that in a complete truck though...
```

---
## \#60 Posted by: mutantbass Posted at: 2019-02-21T03:16:00.768Z Reads: 139

```
hehe I imagine if you message @trampa , he will tell you a way. Makes no sense otherwise
```

---
## \#61 Posted by: evoheyax Posted at: 2019-02-21T03:17:12.585Z Reads: 143

```
I agree, anything I can do to switch tucks frank @trampa?
```

---
## \#62 Posted by: trampa Posted at: 2019-02-21T07:26:45.646Z Reads: 139

```
The complete trucks do not feature this hanger. We make it especially for our E-Boards and this is a spare part. If you want it, you have to get in touch with David Garlinge: david.garlinge at trampaboards dot com.
Good luck with pneumatics on hubs: 4 motors instead of 2, 4 heavy motors, negative gearing ratio, pneumatic tires don't like heat, so make it stay cool! It's still worth a try, but keep expectations low. 

Frank
```

---
## \#63 Posted by: evoheyax Posted at: 2019-02-21T13:56:25.893Z Reads: 131

```
Do you have any idea (maybe from experience) what temps these tubes can generally take?

I don’t think the motor will get hotter than 65c if done right.

In general, it’s not a new idea. The ride sharing scooters are chafing to tubeless tires now but they’ve been using tubes hub motors for over a year now @ 1000 watts.and they are not using the best of anything.
```

---
## \#64 Posted by: trampa Posted at: 2019-02-21T16:29:33.757Z Reads: 131

```
Scooters might have 1000W motors but thermal wattage is probably 250 to 350W on them. Anything beyond that makes them sweat.
Look at R2.1 temp settings for thermal throtteling 100deg cutoff start, 170 hard cutoff 
No motor will survive that for long and pneumatics will blow sooner than later. Stator to wheel diameter ratio will be very bad using pneumatics. You will have negative gearing because of that. In consequence you will face even more heat. Friction is 30% higher compared to PU on tarmac and that works against you in addition. So you will end up with 4 heavy motors and your board will likely feel like a tank and will have half of the performance of a properly geared twin setup with two tiny motors. 
Sorry for being so realistic.
```

---
## \#65 Posted by: evoheyax Posted at: 2019-02-21T17:12:22.769Z Reads: 133

```
First off, thank you for taking the time to respond and give your insight. I don't want to fight with you, just understand your point of view better.

[quote="trampa, post:64, topic:83082"]
Stator to wheel diameter ratio will be very bad using pneumatics.
[/quote]

So then your saying it's also a bad idea to put pneumatics on carvons or @torqueboards new DD? They are not any different in this respect.

[quote="trampa, post:64, topic:83082"]
No motor will survive that for long
[/quote]

From china, yes. I hit that with hummie hubs all of the time without issue, because everything except magnets is rated to 200 C. High heat windings, high heat epoxies, high heat magnets, ect. It's all available.

[quote="trampa, post:64, topic:83082"]
4 heavy motors
[/quote]

Why are they necessarily so much heavier? Unless of course your talking about using smaller motors with gearing to achieve the same efficiency. This eliminates the motor mount and gearing system. If made with aluminum, with machining to reduce extra material between the stator and the inner tube, I would imagine it would only be slightly heavier.

I love the feedback and the challenge! I might need to do a lot of modeling first, and I might have to ditch the fully in wheel and do a half in, wheel half out to maximize the stator diameter.
```

---
## \#66 Posted by: torqueboards Posted at: 2019-02-21T17:29:43.336Z Reads: 123

```
Gearing will always be better. I'm pretty sure everyone knows that. If you want a true pneumatic setup it won't be DD unless it's a DD built specifically for pneumatics. DD w/ pneumatics is a temporary solution and you aren't dogging the setup out. Street cruising would be fine but you aren't racing with a DD pneumatic setup designed for urethane. Still fun to have but it has it's limits.

Test it though doesn't hurt. I like the idea.
```

---
## \#67 Posted by: Hummie Posted at: 2019-02-21T17:32:55.493Z Reads: 114

```
@evoheyax Magnets go to 150c or 300f on what I’m selling. Not 200c.
```

---
## \#68 Posted by: Vanarian Posted at: 2019-02-21T17:36:15.806Z Reads: 120

```
That's already strong margin for neodymium magnets :fire:
```

---
## \#69 Posted by: Lionpuncher Posted at: 2019-02-21T18:10:48.583Z Reads: 127

```
[quote="FredrikHems, post:23, topic:83082"]
Imagine if you have a motor which both sits inside the wheel (like a hub motor), aswell as on the hangar (direct drive).
[/quote]

This has already been done. They’re called carvon V2’s.
```

---
## \#70 Posted by: Goonman Posted at: 2019-02-21T22:37:54.782Z Reads: 131

```
I assume you were referring to me. You are wrong. I wouldn't be trying to get sales from this niche market. I used them because they were all I could find that were decent size direct drive, well sealed and could deliver consistent power. 
Please send me some information about a similar or better motor not made in China. 
@trampa Not they are not thermally managed. I wanted a thermocouple but they won't fit one. I couldn't find any thermistor

Yes I know they aren't to spec but it sounded like he was after some help or suggestions starting point.
I was only trying to help out. 
They work they don't over heat.... As far I can tell and as much as I have tried. They can customise windings.

Carvelab does an adaptor for pneumatic Meepo with a custom DD motor
```

---
## \#71 Posted by: Martin Posted at: 2019-02-22T11:17:17.278Z Reads: 122

```
I am also worried about a hub motor for AT-Tire. Not heavy
So, I have had meaningful results in recent attempts.
I used a 5.5" HUB motor for the kickboard.
Not bad torque, not bad brake strength.

https://www.electric-skateboard.builders/t/my-3rd-hub-direct-drive-for-at-version-trampa-atb-skate-truck-5-5-inch-hub-motor-for-kick-board/80317



So, I try to make it a little thinner and mount it on a trampa spring truck.
I share some photos that I'm working on.
![NaverBlog_20190129_185039_00|374x500](upload://j0ckji59W0VIz2XGxV1geNtkvKW.jpeg) ![NaverBlog_20190129_185041_02|374x500](upload://ewoxbJIiT0yfTl7YfTs4VkplmU9.jpeg) ![NaverBlog_20190129_185040_01|374x500](upload://mETiM83ODgDY412QEfkKZvMFoRW.jpeg)
```

---
## \#72 Posted by: evoheyax Posted at: 2019-02-22T20:13:24.040Z Reads: 115

```
That is an interesting project your working on there! Thank you for sharing that.

After a long talk with John (i.e. hummie), I'm leaning towards an airless solution. This would allow me to maximize the stator size, since the annoying valve won't be in the way. I could fit as large as a 7535 stator completely inside of the hub, and also eliminate the risk of tubes getting too hot and blowing. This would help with that negative gearing that Frank brought up, as a larger stator will have better leverage. Would this would mean as for tires is gummies, or a solid rubber or pu tire in the shape of a normal pneumatic tire.
```

---
## \#73 Posted by: torqueboards Posted at: 2019-02-22T20:35:22.224Z Reads: 112

```
Sounds like a good idea actually. That's pretty much what escooters do anyways. Most of them aren't pneumatic and just rubber tires.
```

---
## \#74 Posted by: evoheyax Posted at: 2019-02-22T20:36:51.859Z Reads: 117

```
https://www.electric-skateboard.builders/t/has-anyone-used-foam-filled-pneumatics/85059

Interested if anyone has used these before. Seems like the best of all worlds. No flats, no tubes, still pretty light since it's filled with foam, and I imagine much better ride than a solid rubber tire.
```

---
## \#75 Posted by: Dagad Posted at: 2019-02-22T23:44:16.729Z Reads: 110

```
foam filled or solid tire vs pnematics - 

in terms of ride quality and performance (and even weight), I imagine pneumatic would win every time.  I'm not aware of any application in any industry that values ride quality and performance where non-pneumatic tires are used.  Yes air in tires is a pain and they go flat and require more maintenance, but it's seemed for years that smart people having been trying to come up with a  comfortable and well performing non-air solution to tires, but have not come up with anything close.  

Now that I think about it, under 10 or 15 mph and on smooth terrain I bet there are a number of interesting non-air solutions that could work. . . but as speed increases and terrain gets rougher, air filled tire advantages seem to increase.  

I recommend you stick with the pneumatic tire route - though if you do decide to go airless - it will still be a very unique product and it might sell because it will likely be the most powerful small hub motor ever :-) . . . . . . .I bet you personally wouldn't ride it as often or enjoyed it as much as if you made it pneumatic though.
```

---
## \#76 Posted by: Dagad Posted at: 2019-02-23T00:44:45.313Z Reads: 104

```
one possible solution to increased motor size and avoid hot/bursting tubes is design this with a custom valve stem and run the tires tubeless.  This is thinking quite a ways outside the box so bear with me. . .

If your doing this build 100% custom and mounting the tire directly on the motor (not they way @martin is doing it - which is extremely cool btw) then you could save precious millimeters by using a presta valve instead of a schrader valve (6mm vs 8mm).  You could also drill a hole and mount the valve wherever you could to maximize motor diameter.   You could mount it on outer rim or inner rim.  I'm picturing something where you mount it on the inner rim partially on the rim wall where the tire bead sits.  You can buy presta valves in many different lengths long or short depending on your design.  You could even design an elbow for the valve to install into if you needed to change the valve direction.
```

---
## \#77 Posted by: Dagad Posted at: 2019-02-23T00:52:10.409Z Reads: 105

```
![image|509x500](upload://r6zsNlkCSSm0lFynwdCMtWlpfNp.png) 

here's a rough idea for one of probably many possible solutions.

motor bumps in toward board and valve points in toward board.

rim diameter at inside 93mm
rim diameter at wall 112mm
motor diameter where it's exposed not hidden by tire) 90mm
valve stem diameter 6mm
```

---
## \#78 Posted by: evoheyax Posted at: 2019-02-23T01:23:46.706Z Reads: 99

```
I thought about that before. The goal originally was to fit standard tubes and tires. It's really impossible to tell how well a motor design will run without building it and actually running it. Simulations only tell so much. So as thus, I need to make the best effort on the first go at a well functional motor.

The custom tube and tire would be nice but it's also a complication. And it would be a significant new cost and introduce a lot of unknowns.
```

---
## \#79 Posted by: Hummie Posted at: 2019-02-23T01:30:33.156Z Reads: 106

```
And I guess in ur drawing the small tube coming out the side would be hollow for the tube?  Maybe if it was further higher on the rim I can imagine sticking a presta valve through, but that would be a crazy metal part to machine.  Maybe they would cast it and then machine it. 

As far as if air tires being the best and nothing else close I think Pu is just as good except when it gets to higher temps then it breaks down.  car tires need to be able to take high heat. There is a weight penalty with a solid tire.  There’s coming to the market Pu air car tires soon so they seem pretty close in everything other than weight n  heat thing is getting better.  
And then it seems most everyone riding air tires on a board has the psi low n I bet less efficient than if it had been a solid good Pu.  Or they pump them fully and get low rolling resistance and lose a lot of the grip and then seems like it’s Pu.  (I ride a bike with latex tubes and some of the lowest rolling resistance tires for sale, people test these things, but if I dropped 1/5 the psi it will have much more rolling resistance) 

I’d like to see a simple test instead.  Rolling resistance, grip, and feel, of the same shape Pu vs air tires on a mountain board.  I’ll cast one in 80duro Pu if someone has a mountain board around and tells me what rim they use.  Maybe it would need be a reinforced rim.  I’m sure such a thing is out there already.  I’ve seen Pu that looks the same diameter but skinnier than a mountain tire
```

---
## \#80 Posted by: Hummie Posted at: 2019-02-23T01:56:22.485Z Reads: 101

```
[quote="evoheyax, post:78, topic:83082"]
I need to make the best effort on the first go at a well functional motor.
[/quote]
But first grammar. Or how’s bout learnin one of them programs. Them computer motor programs.   @Pedrodemio where to get a good tutorial with the latest solver program I think it was you were saying good things about. How bad you think emetor is in comparison as I can run that but not thrilled.
I’ve got a bunch of comparisons I want to run n know @evoheyax is at least interested in some of the same.  Some classic comparisons of copper Percent to iron, long vs short teeth, many teeth n poles vs few. A bunch of other stuff too.  Itching to learn a program n design a stator if u want to help.  Make it.
```

---
## \#81 Posted by: Pedrodemio Posted at: 2019-02-23T02:02:55.695Z Reads: 97

```
Also agree with that, take a look at my feather build topic, there are some information there, also if you need any help you got it
```

---
## \#82 Posted by: Dagad Posted at: 2019-02-23T06:46:21.737Z Reads: 101

```
Glad you saw picture I drew - sorry wasn’t more clear.  I drew it very fast on the way out the door and made it a little too simple it seems.  

The two tiny cylinders were supposed to represent a presta valve stem - one of these: ![image|440x440](upload://xbyWC12XWzgMdepTE0cl6vt6aSK.png) https://i.stack.imgur.com/R19lp.png

All you would have to do is make the wall were the tire bead sits a bit taller than usual and put a hole in the wall.  The valve stem would just install in the hole.  

The rim wall would need to be shaped correctly for tubless but I suspect that would be straightforward.   This is just one simple idea - likely not the best idea - but one way to skin the cat.  

@evoheyax. Regarding your comment about custom tubes and tires and added expense - I would recommend running just the standard popular pneumatic skate tires and no tubes.  @psychotiller has those cool 2x6 tires that are rated to 50psi that would be great to try tubeless.  

In mountain biking many run both tube and tubeless tires interchangeably with and without tubes.  A tire specifically labeled tubeless has thicker sidewalls and allows lower pressures such as 15 psi (for higher traction and cushy ride).  Tubeless label is neither special nor necessary - it simply means a heavier duty tire.  Many, especially weight conscious bikers, run as light of a tire as possible tubeless.  

 My guess is most of the popular skate all terrain tires would fare very well Tubeless.  Run them at their rates psi and put in a little “notubes” sealant and you’re set.  

So - in short - no custome tubes and no custome tires.   You could do some fancy stuff with the rim machining and drilling if you wanted but I suspect there would be only a little added expense for that.
```

---
## \#83 Posted by: evoheyax Posted at: 2019-02-23T07:21:47.137Z Reads: 98

```
[quote="Dagad, post:82, topic:83082"]
The rim wall would need to be shaped correctly for tubless but I suspect that would be straightforward. This is just one simple idea - likely not the best idea - but one way to skin the cat.
[/quote]

So use a pressed fit basically with the tire and the valve in the hub... That might just be the solution actually. I ordered some of those tubeless valves so I can play with them and will start some new designs based on that and see. I have found an appropriate stator at an 80mm diameter. 8040. Just waiting on pricing. But should work.
```

---
## \#84 Posted by: Hummie Posted at: 2019-02-23T07:22:50.122Z Reads: 97

```
O I get u I thought it would be with a tube.  Never ran them but aren’t they sometimes hard to get pumped and need a compressor to get them to first seal?
```

---
## \#85 Posted by: deucesdown Posted at: 2019-02-23T18:31:13.332Z Reads: 89

```
https://youtu.be/63RAFk1Ae84
```

---
## \#86 Posted by: Hummie Posted at: 2019-02-23T19:09:37.122Z Reads: 88

```
Seems complicated and problematic w tubeless especially as you’d be using a split hub that would need to be sealed. 
I like solid Pu.  It’s shown good so far.
```

---
## \#87 Posted by: evoheyax Posted at: 2019-02-23T19:14:56.255Z Reads: 87

```
I don't think it would be that hard to seal. These use a sealant on bike tires. Some proper groves could also be helpful.

https://www.youtube.com/watch?v=6lKRYuaxLls
```

---
## \#88 Posted by: Dagad Posted at: 2019-02-23T21:17:18.928Z Reads: 83

```
Yea - I think tubless is not recommended with a split hub.   Not really sure it would work.   I was thinking about a one piece rim/hub.  

I don’t mean to say tubeless is the only solution.  I was merely brainstorming in an effort to get the largest possible diameter motor and still have air in tires.   

Certainly an airless tire is much much easier from a design perspective, which is probably why 99% of the small hub motors do it that way.    You guys are awesome with what you’ve built so far and  I’d be interested in what you come up with regardless of tire.
```

---
## \#89 Posted by: evoheyax Posted at: 2019-02-23T21:38:52.652Z Reads: 84

```
The issue with a one piece rim is getting the tire on. I'll post some pics in a little of what I'm thinking, but basically, 2 groves for the tire to sit in (93.5mm diameter) and 95mm diameter inside. This would give a  dip for the tire beads to sit in. And on the outside, you can use the plate to compress the tire in to create a seal. You'll see what I mean soon.
```

---
## \#90 Posted by: Pedrodemio Posted at: 2019-02-23T22:04:47.914Z Reads: 81

```
Just put an oring between each half and you can run tub less all day
```

---
## \#91 Posted by: evoheyax Posted at: 2019-02-24T00:38:30.515Z Reads: 85

```
Ok everyone,

Time for an update!

Based on the valve, the biggest stator I can fit now inside of the hub is a 7040. I have not yet found this stator, so I can not finish the design without this. Thus these designs are far form being finished. I can't choose bearings until I know the stators inner diameter. The idea here is to show the groves for the tire to sit in. The outer lip will be compressed by the plate, which I hope will help with the seal. I can use tubeless sealant also if the seal is not good enough. The idea for the valve is to screw it into the hub with locktite to prevent it from unscrewing and seal it.

Here's the latest idea for a tubeless pneumatic hub motor:

![PNG|535x499](upload://f4j2QrkjQkime0S8wZuXT4tviGz.jpeg)

![PNG|489x500](upload://Af9jw3AlHP9XLYAsDp30wjU45SN.jpeg) 

![PNG|522x500](upload://cbVv2vcSJaTIhRvH4b9bREMaH3N.jpeg)

Would love to hear opinions on this design or suggestions of how to make it better.
```

---
## \#92 Posted by: Dagad Posted at: 2019-02-24T01:30:24.337Z Reads: 81

```
that's cool.  I like it.  I see you went with a two piece design. . .   Very cool!  I'm not sure if you realize it - but you've just about created a beadlock wheel (commonly used in offroading).  Here's a pic:

<img src="http://atvconnection.com/Features/images/Beadlock_Cutaway_2.jpg" alt="Image result for beadlock rim profile"/>
```

---
## \#93 Posted by: Dagad Posted at: 2019-02-24T01:34:58.053Z Reads: 79

```
I also like your idea of screwing the stem directly into the hub with locktite.  

I can't quite tell - but it looks like you have the stem screwed into the space where magnets are typically placed?
```

---
## \#94 Posted by: Dagad Posted at: 2019-02-24T01:46:54.158Z Reads: 82

```
regarding the bead seat - here's a "rim profile" pic that shows how bikes typically do it: 

<img src="https://amclassic.com/media/catalog/product/cache/1/image/550x550/9df78eab33525d08d6e5fb8d27136e95/s/m/smokin_gun_rim.jpg" alt="Image result for rim profile"/>

They have a low space in the middle so you can actually stretch the tire on - though not needed in your case if you stick with two piece rim.   Then there's the bump, then there's the "hook" at  the top.  Not sure if any of that is needed if you use removable rim. . .


If you decide Schrader valve is better, here's a possible design using a schrader 90" elbow screwed into a 4mm pipe

![image|690x494](upload://wT1XPvzpdqRfSvCAEy9d1krm0TH.png) 

![image|690x436](upload://gzAbiDFj7Uo7PYIkiHjNvBwS9aD.png) 

![image|690x493](upload://m4NMYsGl8bqaLZsxIFoRGXHfOS1.png) 

I'm not that familiar with motor design - but I think this would require a small gap in magnets. . .
```

---
## \#95 Posted by: evoheyax Posted at: 2019-02-24T02:00:04.789Z Reads: 80

```
Theres 1.6mm of steel between the magnets and the valve. This may get a little thicker depending on actual stator size that I can find.
```

---
## \#96 Posted by: Dagad Posted at: 2019-02-24T03:16:54.190Z Reads: 79

```
What is the wall thickness of the motor?  I think it's called a "bell"?  The part that holds the magnets.  

I put in my drawing 3mm wall thickness but yours would have to be closer to 10mm to fit that presta valve. . .
```

---
## \#97 Posted by: evoheyax Posted at: 2019-02-24T03:26:37.465Z Reads: 79

```
The problem with your design is it eats into the magnets. You need magenets, thin wall, valve, thin wall, tire. So 9mm is the least you can get away with. I can drill out that to reduce weight also.
```

---
## \#98 Posted by: Dagad Posted at: 2019-02-24T03:41:55.658Z Reads: 78

```
Thanks for explaining.  That makes sense.    9mm wall thickness.
```

---
## \#99 Posted by: Pedrodemio Posted at: 2019-02-24T04:46:21.013Z Reads: 79

```
Love the solution, I think this and variations are the way to go for hubs of this kind

About the stator, there are lots of companies at Alibaba that does small quantity stators using EDM and laser cutters, also there are some some US based that does the same, including windings, don’t recall the names at the moment, but I imagine it will be way more expensive than the China ones
```

---
## \#100 Posted by: evoheyax Posted at: 2019-02-24T05:46:03.461Z Reads: 77

```
I've been talking with a few companies through alibaba. The prices are not as good as I was hoping though. John found a steal of a deal for the price he pays for his stator. Best I've found for an 8040 stator is $75 each, which is very high. Unless I can get better prices (more like $20 a stator), it will end up costing $500 a set of motors at cost + labor, easily $800-$1000 a set, without trucks or front wheels. That's too high of a price imo for most, so I have a lot of work to do, beyond actually making a functional prototype.
```

---
## \#101 Posted by: Goonman Posted at: 2019-03-02T11:58:07.957Z Reads: 60

```
Two piece rims are nothing new. Sealing should be done with an o-ring but I'm sure plenty of peeps are just using non corrosive silicone sealant. Generally tubeless tyres are sealed with liquid latex or similar proprietary ingredients.
```

---
