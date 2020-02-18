# Open Source Precision Trucks and Hub Motors Project

### Replies: 53 Views: 2146

## \#1 Posted by: harrypzee Posted at: 2018-07-10T21:20:53.656Z Reads: 420

```
Hi All,

I am in the process of building my first ESK8, and I am very interested in fabricating my own precision trucks and hub motors much later down the road. I have built 3D printers, drones, and other projects in the past, and I recently taught myself how to use Fusion 360, so I have some amateur experience with engineering and fabricating. I am creating this topic to share my ideas, designs, and to take advice and inspiration from other ESK8ers who are perhaps more experienced than I am.

My goals for this project are:

* Create precision trucks that are designed with ESK8 in mind and hub motors to go with them
* Build upon and address issues with current truck and hub motor designs
* Share my designs with the public via thingiverse.com
* Design with the amateur hobbyist in mind, so that anyone with access to a metal CNC mill can make it themselves

My current ideas for this project are:

* Make precision trucks that use the same bushing and pivot cup dimensions as an existing precision truck (possibly Surf-Rodz RKP) so that instead of having to make custom bushings of dubious quality, people can buy bushings from a tried-and-true manufacturer like Riptide.

* Make Hummie style hub motors rather than Carvon style motors. I know this is a FIERCE topic of debate in the community, but I want to go with Hummie style hubs. Here's why:

  * Stress is more evenly distributed across the motor

  * They make use of space much more efficiently

  * It seems like just about everyone in the unpowered downhill scene uses much shorter width trucks. I think having shorter trucks might increase stability at high speeds, because it essentially makes the wheelbase longer relative to the truck width. Also, the longer your trucks are, the more your leaning is converted into turning, which can lead to instability. I think we can learn a lot from the guys going 50+ mph. How does this relate to hub motors, you might ask? Well, with Carvon style hubs, the trucks need to be SUPER wide to accommodate the motors in between the kingpin and the wheels. But with Hummie style hubs, since the motors are in the wheels, you have a lot more room to shorten the trucks.

  * Stealthy as fuck. Not nearly as important as the other things listed, but I know some people care a lot about looks.

  * As for the issue with thin urethane on in wheel hub motors, I think there is an easy fix. Bigger wheels! Why stop at 90, 97, 107mm? Since in wheel hubs require casting urethane, why not use that as an opportunity to cast some bigass wheels? I'm thinking 120, maybe even 130mm. That would allow the motor to be bigger as well, which would increase power and cooling.

* Make the truck a giant heatsink. The biggest issue with in wheel hub motors is that they have a hard time cooling down. Duh. You can't stick a motor capable of pushing a human being over long distances at speeds over 30 mph in a nice blanket of heat insulating urethane and expect it to be cool as a cucumber afterwards. So why not make the truck a giant heatsink? After reading @Minim's awesome post about his custom Raptor 2 hangers (link: https://www.electric-skateboard.builders/t/raptor-2-custom-hanger-for-better-cooling/61104) I had a eureka moment. USE THE TRUCK AS A HEATSINK! Minim had to design the hangar to be compatible with all of the Raptor 2 measurements, but if I am making trucks/motors from scratch, I can design it to be one large, incredibly effective heatsink. Perhaps I could use thermal paste where the motors attach to the hanger to augment the heat transfer even more.

Anyways, those are my ideas so far. If you have any suggestions or advice, please comment below.

Thanks,

Harry
```

---
## \#2 Posted by: FredrikHems Posted at: 2018-07-10T21:45:29.475Z Reads: 363

```
Seems like an interesting topic. Why not try to make something new, like a mix between Carvon style motors and regular hub motors? :grinning: 
That would have been very cool IMO
```

---
## \#3 Posted by: harrypzee Posted at: 2018-07-10T21:47:05.172Z Reads: 365

```
I believe Carvon actually did that a while ago with their V2s. Like half of the motor went into the wheel.
```

---
## \#4 Posted by: baxter Posted at: 2018-07-11T09:23:02.918Z Reads: 342

```
A suggestion for your design: A queen pin, like on Ronin trucks
```

---
## \#5 Posted by: baxter Posted at: 2018-07-11T09:26:30.727Z Reads: 335

```
FYI

https://www.electric-skateboard.builders/t/open-source-precision-trucks-looking-for-design-feedback/20231
```

---
## \#6 Posted by: Bor.inc Posted at: 2018-07-11T09:46:14.900Z Reads: 308

```
For the record, what are precision trucks? :slight_smile:

I am very interested in how your hubmotors will be designed because I am also interested in building my own but don't know where to find information about how to design them
```

---
## \#7 Posted by: Fraserrazor Posted at: 2018-07-11T11:37:04.255Z Reads: 291

```
Larger wheels do affect the acceleration curve (decrease in gradient). They also can reduce or even prevent the ability to push kick the board although I suppose the USP of the larger-urethane wheel hubs would be top speed.
```

---
## \#8 Posted by: harrypzee Posted at: 2018-07-11T18:08:57.039Z Reads: 282

```
Interesting. Can't the decrease in acceleration be counteracted by a lower-kv hub motor? Also, I know a lot of people use pneumatics which are even bigger than the wheels I want to make.
```

---
## \#9 Posted by: harrypzee Posted at: 2018-07-11T18:12:04.649Z Reads: 281

```
Yeah, designing trucks/hub motors is tough because there is hardly any information on the internet regarding dimensions, sizing etc. Probably because everyone wants to buy them :joy:. I'm getting a lot of info from Hummies thread about his hub motors.
```

---
## \#10 Posted by: harrypzee Posted at: 2018-07-11T18:12:44.616Z Reads: 267

```
Thanks for the link! That is super interesting.
```

---
## \#11 Posted by: harrypzee Posted at: 2018-07-11T19:06:13.227Z Reads: 277

```
UPDATE: I came up with a few more ideas I'd like to implement in my design.

* Built in split angles. For example, I can make the powered rear trucks 40 degrees and the unpowered front trucks 60 degrees. This way, no wedges will be required. I'm thinking of going with a 60/40 split because it is sort of a middle ground. Maybe I could design some baseplates with different angles for people who like to experiment, but for now I think 60/40 will satisfy 90% of everyone's requirements.
* A hexagonal hanger. I was thinking of doing a round hanger at first, because without the need to mount belt driven motors, a round hanger distributes load more evenly than a square one. However, making it round would drive up machining costs by a lot, so hexagonal seems like a good compromise.

That's it for now. One thing I am really struggling with is finding the right dimensions of pivot cups and bushing seats for precision trucks like Surf Rodz. If anyone has a Surf Rodz RKP truck and some calipers, I would really appreciate it if you could give me the diameter/depth of the pivot cup and bushing seat. @Alphamail, perhaps you could help me out?
```

---
## \#12 Posted by: Alphamail Posted at: 2018-07-11T19:10:51.840Z Reads: 278

```
I would not copy the SZ RKP bushing seat as it is substandard many levels! 
 Here are good basic seat cross sections in mm and Inches.
![basic%20bushing%20seat%20dimensioned%20mm|690x476](upload://7Qgu4KWTZx52vOdJNG57Da7kIwk.JPG)![basic%20bushing%20seat%20dimensioned|690x473](upload://aNo3ylRAAgRGtHhlbHLkbiCQHZ7.JPG)
```

---
## \#13 Posted by: Alphamail Posted at: 2018-07-11T19:14:20.550Z Reads: 252

```
The Pivot Axis should intersect the center of the bushing floor spacing
```

---
## \#14 Posted by: Alphamail Posted at: 2018-07-11T19:17:08.777Z Reads: 247

```
If you work in solidworks,2012 or older, i can look at the part file, otherwise send me a .step file and I can convert it to help you with the pivot cup placement and dimensions.  My email address is brad@riptidesports.com
```

---
## \#15 Posted by: Alphamail Posted at: 2018-07-11T19:27:15.773Z Reads: 255

```
One other thought is a 20 degree split is great but i think you are on the highside with the 60 degree front.  I think you will be happier with a 50/30 configuration
```

---
## \#16 Posted by: harrypzee Posted at: 2018-07-11T19:38:48.981Z Reads: 262

```
Thanks for all the data! It's interesting that the SZ RKP bushing seat is substandard. I've heard some people complain about SZ trucks being too tight or "sticky". Does that have to do with the bushing seat at all? Right now I'm trying to find the best pivot cup to use. I found this handy diagram about your different pivot cup dimensions here:![all-pivot-cup-specs-to-scale|690x151](upload://6FtJNYDD0BN7q6w6nN2FsPuowW3.png) I don't know if the above image is precise at all or just an approximation. I want to use existing pivot cup dimensions so that people can buy Riptide pivot cups for X truck that will work perfectly with my trucks instead of having to make custom sized pivot cups. Which would you recommend? Is bigger better? Also, what tolerance should I go for when designing the pivot cup and bushing seats? For example, if I decide to go with your Caliber II pivot cups, should the hole be 18.1mm? 18.2? 18.05?
```

---
## \#17 Posted by: Alphamail Posted at: 2018-07-11T19:43:53.668Z Reads: 255

```
These details should be discussed confidentially
```

---
## \#18 Posted by: skatardude10 Posted at: 2018-07-11T19:58:50.687Z Reads: 251

```
Do you design in Fusion 360? 

How about adjustable angle baseplates?

I'd love to help out with this project in some of my spare time... I have some experience designing longboard trucks, testing prototypes, and have had some of my designs manufactured in the past.
```

---
## \#19 Posted by: harrypzee Posted at: 2018-07-11T20:09:25.934Z Reads: 239

```
I do indeed use Fusion 360. That's super awesome! Once I get my first revision done, maybe you can take a look at it and tell me how I can improve. I've never heard of adjustable angle baseplates, but that is a very interesting idea. I'll look into it.
```

---
## \#20 Posted by: chuttney1 Posted at: 2018-07-11T21:21:36.059Z Reads: 246

```
[quote="harrypzee, post:1, topic:61480"]
Design with the amateur hobbyist in mind, so that anyone with access to a metal CNC mill can make it themselves
[/quote]

You should rewrite this so anyone with access to a knee mill or CNC can make these trucks. 

[quote="harrypzee, post:1, topic:61480"]
I think having shorter trucks might increase stability at high speeds
[/quote]
Do you mean hanger width? Becuase if it is, this concept is already proven in Motorsports with regards to vehicle track width as wider is more stable, but you run into problems to is a choice for a specific width in design.
```

---
## \#21 Posted by: harrypzee Posted at: 2018-07-11T21:31:23.082Z Reads: 228

```
Yeah I mean hanger width. I have to disagree with you, because a) longboard trucks are different than car axles, and b) check out what ronin (one of the best truck makers on the planet says about this) says regarding this topic:

"Despite popular belief, narrower is not less stable. What you get is a quicker turning truck that allows you to better apply your weight on the wheels. The cleaner you are through the turn, the faster you go, and narrower setups provide this."
```

---
## \#22 Posted by: harrypzee Posted at: 2018-07-16T21:56:21.418Z Reads: 221

```
Alright guys, I just wanted to give y'all an update on where I'm at. I decided to go with Caliber II pivot cup and bushing seats, because a) they are some of the most common and b) they take some of the biggest pivot cups, which gives me more confidence about the longevity and durability. I have designed the baseplate with the pivot cup seat, but I haven't designed the kingpin holder because I wanted to do the hanger first.

Now, the hanger is where things are getting really interesting. I used this website https://celsiainc.com/heat-sink-size-calculator/ to roughly estimate how much heat sink volume I need. I plugged in 1,512 Watts, or 50.4 Volts (a fully charged 12S battery) x 30 amps. Then I plugged in 60 degrees Celsius as the maximum temperature for the motors (obviously motors can get much hotter and still be okay but 60 degrees is about the temperature where they start to temporarily demagnetize, which quickly reduces efficiency) and 25 degrees as the maximum ambient temperature. I got 3456 cm3! And that's for one side (aka one motor)! For two sides it would be 3456 x 2 = 6912 cm3. So obviously I can't meet that number. But I can try. I've been designing the hanger with as much heat sink as possible. And the result is... 118.7 cm3 in volume! Lol. But some is better than none.

Here's a picture of my current design:
![Rear%20Truck%2035%20Degree%20v144|690x344](upload://nAYzKaVjuo79kJXq7sKXgzAsHN5.png)
```

---
## \#23 Posted by: harrypzee Posted at: 2018-07-21T19:18:36.614Z Reads: 208

```
Okay, a little update. I decided to go with Carvon style motors in the end. I think they just have so many advantages to Hummie style motors (not that Hummie style motors are at all bad). I am currently redesigning a lot of stuff, but I will post a picture once I have made some progress.
```

---
## \#24 Posted by: Hummie Posted at: 2018-07-21T19:58:41.359Z Reads: 212

```
[quote="harrypzee, post:22, topic:61480"]
I plugged in 1,512 Watts, or 50.4 Volts (a fully charged 12S battery) x 30 amps.
[/quote]

I think if the motor was totally inefficient and turned everything to heat that would be appropriate but much of that energy is turned to motion. maybe could assume 85% efficiency and cut 85% off that number

bigger and bigger hanger with lots of fins but how about a better conduit for the heat.  will the motor just be sitting against the hanger aluminum because even with thermal paste that area is sure to be the bottleneck.  it needs more contact either by being a continuous metal all the way under the stator or much more surface area in contact.   
maybe forget that approach of trying to transfer from the motor's metal case transfering to the hanger and instead have the phase wires or magnet wires going through the hanger.  they'd have to be electrically isolated somehow but if that can be done and still with a good thermal pathway then you could free the rest of the design up for other goals.    also those wires coming out could be made much more robust and that's where a lot of hubs break.
 to make the wires insulated electrically but with a good thermal pathway is a challenge.  the best i came up with was some thermally conductive silicone and was planning to make wires with it but it's not nearly as strong as typical silicone for wires and dont think it will work that way.  thermal and electrical conductivity seem to go hand in hand.
 

you can get magnets that have different much higher currie temp (demagnetize) and the lead up to that temp and subsequent temporary loss of magnetism is also moved to higher temps.
```

---
## \#25 Posted by: harrypzee Posted at: 2018-07-21T21:34:01.888Z Reads: 193

```
That's super interesting Hummie! Thanks for giving your input on this thread, I was hoping some of the big guys would chime in :slight_smile:
```

---
## \#26 Posted by: Hummie Posted at: 2018-07-21T21:47:36.738Z Reads: 194

```
no problem this is fun for me i like design challenges.  I only have big interest.  ...and hopefully you see things my way and further develop it.  gotta find that conductive insulator/ insulating conductor and figure a way to do it practically.
another option which would be easier would be flattening the motor leads or better yet the magnet wire as it comes out of the motor and epoxying it to the hanger outside.  could look really nice or could like like a kindergarten art project but a lot easier.   a thin coat of epoxy on the wires after banging them flat and then just glue them on, maybe route them up to some imbedded bullet plugs or something would be slick
```

---
## \#27 Posted by: harrypzee Posted at: 2018-07-22T04:23:22.507Z Reads: 181

```
Quick update. I'm super torn between Hummie style hubs and Carvon style hubs still. Earlier I said I was going to go with Carvon style, but now I'm not so sure. Deciding what to design is almost harder than designing!
```

---
## \#28 Posted by: Hummie Posted at: 2018-07-22T04:56:32.082Z Reads: 180

```
how bout you do an inrunner motor in the hanger.
```

---
## \#29 Posted by: harrypzee Posted at: 2018-07-22T05:08:08.809Z Reads: 184

```
Interesting. Can you elaborate?
```

---
## \#30 Posted by: pat.speed Posted at: 2018-07-22T05:22:27.073Z Reads: 185

```
I vouch for carvon, as you get a full amount of urethane to dampen the ride, with in-wheel hubs you will only get about 10-20mm of urethane
```

---
## \#31 Posted by: harrypzee Posted at: 2018-07-22T05:23:02.836Z Reads: 183

```
True, but with Hummie style hubs you have waaay more protection for the motor.
```

---
## \#32 Posted by: harrypzee Posted at: 2018-07-22T05:23:49.858Z Reads: 191

```
![Rear%20Truck%2035%20Degree%20v163|690x344](upload://bBd05og1N1LZ8mL15BlHaZUcX1T.png)

This is my latest design. I think it looks a lot better than the hexagonal one.
```

---
## \#33 Posted by: pat.speed Posted at: 2018-07-22T05:23:54.220Z Reads: 187

```
Just add a urethane sleeve...second wheel?
```

---
## \#34 Posted by: Schulerbible Posted at: 2018-07-22T06:37:06.794Z Reads: 183

```
I like the idea but it doesn't look to be a simple CNC job. Also, some of the shown geometries are nearly impossible to machine. Curious what the outcome is! A few people have tried making CNC trucks but never really marketed the thing. Making trucks is pretty expensive. My own set (just the hangers) cost me $270 per piece machined out of AL7075 and abut $240 out of AL6082. Adding things like a queenpin is a nice idea but is going to be expensive at the end of the day. Not sure if you find a lot of people who are willing to buy a CNC truck for their cheap Chinese hubs :)
```

---
## \#35 Posted by: harrypzee Posted at: 2018-07-22T06:52:52.943Z Reads: 182

```
Yeah, this is a passion project and I don't really give a fuck about whether or not it's too expensive to sell :stuck_out_tongue:
```

---
## \#36 Posted by: Minim Posted at: 2018-07-22T09:41:31.870Z Reads: 178

```
Good points. I would also suggest that once the design is finalized it’s a good idea to speak to the one that’s going to machine it and see if there is changes that can be made to simplify machining without sacrificing to much on the design. Small simple things can make a huuuuge difference in cost/time.
```

---
## \#37 Posted by: Schulerbible Posted at: 2018-07-22T10:02:52.811Z Reads: 191

```
There is always the possibility to upload the 3D file to xometry or 3D hubs to get an instant quote. They also show the price reduction for multiple copies. When tighter tolerances come into the game e.g. axle concentricity or pivot seat, the price changes pretty quick.
```

---
## \#38 Posted by: Vanarian Posted at: 2018-07-22T10:23:33.316Z Reads: 184

```
**Cough** A layer of Gelid Extreme or Shin Etsu compound trapped around your cables and hanger, then epoxy armor lacquered on top of it **Cough**

There goes your insulated thermal conductor for your wires :beers:
```

---
## \#39 Posted by: Luvafreeride Posted at: 2018-07-22T14:21:39.749Z Reads: 175

```
Yes with  planetary gears in the wheel!
```

---
## \#40 Posted by: Hummie Posted at: 2018-07-22T17:23:28.922Z Reads: 187

```
I dont know what shin etsu product you were thinking but the gelid extreme stuff looks awesome, but im still not sure what you meant to do with it.  If gluing flattened motor wires to the hanger id think it wouldnt be worth using a paste and just the thinnest insulator between the wire and hanger..a painting of epoxy.   But if you mean a hole in the hanger...then yea maybe just a thin painting of epoxy in the hole and insert the tight fitting wire with the gelid stuff to fill any gaps. seems risky though and fear the wire would be not secured and eventually if it rubs the epoxy off against the inside of the hanger.   just gluing the flattened motor wires to the outside of the hanger with a very thin heat resistant epoxy is seeming the more reliable and doable.  I dont think a conductive epoxy would be as good and instead a pure resin unfilled and the thinnest coat possible.    if the wire cant move it seems safe.  so i think.   or maybe the wires in the holes if they were the original motor leads with their insulation and then fill the hole with a harder resin like a highly filled epoxy so the wires were fully secured.
@Luvafreeride planetary gears maybe are an unnecessary complication if you can make the motor big and strong enough.  they make noise and need maintenance and will be the first to break.   try to make it all as simple as possible and more likely to actually make it to reality.
```

---
## \#41 Posted by: harrypzee Posted at: 2018-07-22T20:12:51.338Z Reads: 180

```
Agreed. I don't want to go with planetary. I want to go as simple as possible while still achieving my goals.
```

---
## \#42 Posted by: harrypzee Posted at: 2018-12-14T22:54:11.836Z Reads: 168

```
Hey guys! It's been a while since I've worked on this project, but I started back on it recently. I decided to go with a Caliber II compatible hanger, so that I won't have to design my own baseplate. I used @Alphamail's bushing seat dimensions he recommended earlier in the thread. I also took a different approach to cooling - instead of having a closed off motor, I designed it so that the end caps of the motor are actually fan blades that push air thru the motor, directly cooling the stator. I also designed the endcaps to fit into the rotor without any bolts, so that it only requires 1 centerlock nut for the 10mm axle to fit the whole thing together (other than the stator, which will be epoxied on). Who knows how well this will work, but hey! Why not try it? :) Anyways, here are some photos:

![Truck%20With%20Hub%20Motors%20v85%202|689x343](upload://tnuTUrSaDxoKyIW0xSSEO3BIm6r.png) ![Truck%20With%20Hub%20Motors%20v85|689x343](upload://xY1moAvCkKTmw05asHCRoydGdCl.png) ![Truck%20With%20Hub%20Motors%20v85%203|689x343](upload://4lpJcEklfVHmOTJu8Lc2wnkzdkT.png) ![Truck%20With%20Hub%20Motors%20v85%204|689x343](upload://4Jqr1qgXHr15kdj9ZcwIoTSxoKB.png) ![Truck%20With%20Hub%20Motors%20v85%205|689x343](upload://bNWixHNu2OU824XK4Rj96nKyRmB.png)
```

---
## \#43 Posted by: Minim Posted at: 2019-01-07T15:45:50.329Z Reads: 151

```
How will you solve the problem with dirt being blown into the engine?
```

---
## \#44 Posted by: harrypzee Posted at: 2019-01-07T17:54:35.349Z Reads: 141

```
I was thinking of somehow attaching a super fine mesh on the inside of the fan blades.
```

---
## \#45 Posted by: Luvafreeride Posted at: 2019-01-07T18:44:40.838Z Reads: 138

```
Something like stocking material might work.
```

---
## \#46 Posted by: Minim Posted at: 2019-01-07T20:50:53.596Z Reads: 137

```
That could work. @trampa made a thread about sealing the motors he's selling. Maybe some of that will work. 

Are you machining this yourself? If not have you gotten a quote on the machining?
```

---
## \#47 Posted by: harrypzee Posted at: 2019-04-16T19:13:47.002Z Reads: 107

```
Hey guys, I haven't changed my design much since I last posted. I got a bit discouraged, because I honestly have no idea how to machine this thing. I also know very little about how I would go about getting the stator made. One change I want to make to the model is simplify the design of the end caps and make the fan blades a separate 3D printed object. Milling fan blades out of metal seems really difficult and expensive.
```

---
## \#48 Posted by: Vanarian Posted at: 2019-04-16T19:34:26.701Z Reads: 107

```
I know your pain, here is an idea to cheer up a bit : you should try straight cut centrifugal blades, instead of sucking air in it will suck air *out* of your motor (you need holes on the other side). It is easier to machine and as efficient in airflow cooling, while stressing less airdrag.

Forced intake is more useful if you intend to *use* the air as a propelling force.

You can get custom stators from China but it's better to start off an existing model cause it's one less thing to build. Rotor is bound to be expensive, can't help out with that.
```

---
## \#49 Posted by: harrypzee Posted at: 2019-04-17T17:49:20.141Z Reads: 92

```
I really like the idea of using centrifugal blades to cool the motor, but I can't think of how I could fit it in there.
```

---
## \#50 Posted by: Vanarian Posted at: 2019-04-17T18:41:14.659Z Reads: 91

```
There seems to be spare room between the truck and the wheel ? If fins are thin enough it'll do the job
```

---
## \#51 Posted by: harrypzee Posted at: 2019-04-24T17:35:13.158Z Reads: 86

```
I have a new idea for a way to cool the motor. What if the endcaps have fins on them that act as a spinning heatsink? Here's a photo of a quadcopter motor that uses this method:![Brotherhobby-Tornado-T2-2206-2600KV-Motor-feature-1024x768|666x500](upload://tZBLs0Wmuo9p0ugLLAiSYOPdFH.jpeg) 
What do y'all think? Oh, and one more question: what axle diameter should I use? Right now the design uses 10mm axles. I remember reading that Enertion had to beef up the axles in the Raptor 2 hubs because 10mm was too weak.
```

---
## \#52 Posted by: pat.speed Posted at: 2019-04-24T21:30:27.403Z Reads: 77

```
12mm is the best, 10mm will work if it’s strong metal
```

---
## \#54 Posted by: harrypzee Posted at: 2019-04-26T19:19:12.291Z Reads: 55

```
Gotcha. I'm gonna redesign the axles to be 12mm then; above all else, I want these motors to be tough.
```

---
