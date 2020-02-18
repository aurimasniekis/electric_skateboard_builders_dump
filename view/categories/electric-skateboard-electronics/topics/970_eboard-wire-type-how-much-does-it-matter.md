# Eboard wire type- how much does it matter?

### Replies: 32 Views: 9282

## \#1 Posted by: EnertionSupport Posted at: 2016-01-09T21:37:25.520Z Reads: 346

```
@lox897 is right about the shrink wrap- only cut it if you need to access a covered port. 

as for the wires, you will want to strip the insulation enough for you to solder the bullet connectors without burning the rubber part of the wire. I'd suggest maybe 1/4inch to be taken off, but it depends on the bullet connectors as well. 

Also, it is fine to power the VESC with a Space Cell during detection. If you plan on doing it often though a power supply is always better.

**About editting the title**: just reply to my post with how you want it to be named, and I will change it for you. I think over time the title get's locked in, so it can only be changed by moderators... I'll handle it for you if you just tell me what you want it to say.

@lox897 had a good message about how titles should be formatted, so I'd take a look at his post for ideas on your new title.
```

---
## \#2 Posted by: chaka Posted at: 2016-01-09T22:23:42.065Z Reads: 340

```
[quote="EnertionSupport, post:50, topic:298"]
as for the wires, you will want to strip the insulation enough for you to solder the bullet connectors without burning the rubber part of the wire. I'd suggest maybe 1/4inch to be taken off, but it depends on the bullet connectors as well.
[/quote]


The insulation should not burn if the correct wire is used. If you are burning the insulation while soldering connectors to your cables you have incorrect cabling for our purposes and it should be replaced. You want to make sure you are using "high strand silicon wire".
```

---
## \#3 Posted by: EnertionSupport Posted at: 2016-01-09T23:27:53.967Z Reads: 335

```
sorry for not being clearer @chaka

I was referring to burning the insulation by touching it with the soldering iron. 

when @disastorm referred to the wires as:

[quote="disastorm, post:48, topic:298"]
should I strip the wires first, or is the surface area of the wires already good enough?
[/quote]  

I believe he was looking at unstripped wires. Trying to solder them when they are unstripped would burn the insulation (because the bullet connector and solder would touch the outside of the wire), so that is why I mentioned that he should strip the wire far enough as to not burn the rubber. 

Again, sorry for the miscommunication.
```

---
## \#4 Posted by: chaka Posted at: 2016-01-10T00:17:16.304Z Reads: 332

```
I will say again, the correct wires will not burn while soldering.

For reference, I completely submerged some silicon wire in my solder pot for 5 seconds and it slightly discolored the insulation. If you are burning insulation it means you are most likely using automotive electrical wire and it will not do well with the high currents we use on electric skateboards.

<img src="/uploads/db1493/original/2X/8/8ef53c7d5e56a3befa8e0739391ad41bc1062b41.jpg" width="618" height="500">
```

---
## \#5 Posted by: cmatson Posted at: 2016-01-10T01:37:01.099Z Reads: 327

```
High strand silicon wire insulation will still melt if you touch the tip of a soldering iron to it- not to mention it doesn't smell too good either!

but let's not all argue- can we agree that with normal soldering the wire insulation is not going to melt, but if you were to touch it with your soldering iron it would melt (i.e. if the wire wasn't stripped) .
```

---
## \#6 Posted by: chaka Posted at: 2016-01-10T06:47:13.543Z Reads: 333

```
Thats the thing @cmatson, I can take a soldering iron and rest it on some silicone wire insulation and it will not melt and if your insulation is melting from touching it with your iron it is not high strand silicone wire.

This is a big one too. All of the specs we build on require a very high current carrying capacity and automotive grade wire isn't really up to the task. The loads we carry can melt the insulation on common copper wire and potentially cause a fire. 

If you are using common copper wire you would need to use at least 8 awg to get the same carrying capacity as 10 awg high strand silicone. Likewise, if you are using 10 awg common wire it is the equivalent of 14 awg silicone wire.
```

---
## \#7 Posted by: trbt555 Posted at: 2016-01-11T13:03:14.998Z Reads: 315

```
@chaka I don't agree with your statements. Based on physics.

First let's get a few things straight before we start confusing people.

"High strand wire" just tells us the wire is composed of a high number of individual strands, which improves the flexibility of the wire, not the cross section, nor the current carrying capacity. If anything, a massive conductor would be better, however unpractical.

"Silicone" just tells us the insulation of the wire is made of a flexible and heat-resistant silicone polymer.

Copper is always copper and 10 AWG wire always has the same cross copper cross section, thus the same current carrying capacity in terms of heat dissipation.

I do not believe that the currents we are putting through these wires can melt the insulation.
Let's calculate the power dissipated by 25cm of copper 10AWG wire.

First we need to calculate the resistance of this piece of wire.
Resistivity ρ = R * (A/L) where R is the resistance (Ohm), L is the length (m) or the wire and A (m²) is the cross section.
Therefore R = ρ * (L/A)

The resistivity of copper is roughly 1.7 x 10^-8 Ohm.m
The length of our wire is 0.25m
The section of our wire is 5.2 x 10^-6 m²

Result R = 0.0008 Ohm

Let's now calculate the dissipated power over this length of wire at a current of 120A.

Dissipated power P = R * I² where R is resistance (Ohm) and I is current (A)

Result P = 0.0008 Ohm * (120 A)² = **11,5 W**

I seriously doubt that 11.5W spread over 25cm of wire during a brief period of time on a moving e-board will be capable of melting any insulation.

Yes, high strand count wire is more flexible and combined with silicone insulation it gives you an exceptionally flexible, durable and heat-resistant wire, which is good for our applications.

Now if vendor A was selling PCB's with plain automotive wire and vendor B was selling the same PCB's at the same price but with high strand count silicone insulated wire, you could safely say vendor B is offering better quality.
```

---
## \#8 Posted by: chaka Posted at: 2016-01-11T15:07:20.427Z Reads: 283

```
[quote="trbt555, post:58, topic:298"]
I don't agree with your statements. Based on physics.
[/quote]

This is well known in the RC world due to "real world" results. 

A high strand cable does indeed have more copper than a lower strand cable of the same gauge so it can carry more DC current.

 Now for the part you have overlooked. AC current and skin effect! We run AC current though our motor leads and the more surface area we have in our cables the more current we can carry in them. The higher the frequency of the AC current the higher the effect. Our current consumption peaks in tandem with the peak in frequency so it sets up a very good failure scenario for wire of insufficient capacity.
```

---
## \#9 Posted by: trbt555 Posted at: 2016-01-11T15:16:45.300Z Reads: 282

```
Have you ever seen *real word results* under normal use on an e-board where 10AWG wire got so hot it could melt insulation ?
I don't agree on high strand having more copper for the same gauge but I don't want to hijack @disastorm 's thread so I'll leave it at that.
```

---
## \#10 Posted by: longhairedboy Posted at: 2016-01-11T19:33:29.345Z Reads: 282

```
i've been using Super Worm high strand silicone insulated wire which is pretty common in the RC world. It comes in multiple gauges and works really well for everything in the box. I only use 10 awg on battery wiring and typically it seems like motors are coming with 12awg phase wiring, so i'll use that when i need to make phase leads. 

The only time i've ever seen the insulation melt or burn is in two edge cases: 1) when i screw up and throw sparks. But when that happens, entire bullet connectors can disintegrate and throw slag everywhere. 2) when i lay the soldering iron tip directly on the insulation, but even then it just sort of gets soft, it doesn't discolor and do that margarine separation thing that automotive wire does. 

In all three of the boards i've prototyped with inlaid wiring i've used 10awg stranded wiring with non-silicone insulation, basically automotive wire. The insulation on that wire does separate and get gross and oily with heat, so when filling the back of the bullets with solder i have to be careful. I use that wire in that particular case because its not springy and holds its shape when bent. 

long story short: super worm and other high strand count silicone insulated wire is the shit and its the best wire for inside the box for many reasons.
```

---
## \#11 Posted by: onloop Posted at: 2016-01-12T02:48:44.719Z Reads: 286

```
For those of you who want to count the strands here (wire at the bottom) is the wire that came on the last batch of VESC, its 12AWG high strand count copper wire with polyurethane insulation rated to around 100C.
The one at the top is "12AWG - high strand count - tinned copper wire - with silicone rubber insulation" 
<img src="/uploads/db1493/original/2X/e/ed22094a8bb51bf831bb8dab001a95f060c5dc4a.jpg" width="281" height="500">

If you have silicone rubber insulation the wire can heat to 200C without melting the insulation.. If you dont have it your wire insulation will melt at lower tempratures. 

If your wire temprature reaches 200C you have other issues that need to be addressed, such as why your system is pulling such a huge amount of amps.
```

---
## \#12 Posted by: MonsterCoatings Posted at: 2016-01-13T08:34:32.815Z Reads: 292

```
Found this on Quora, too late for me to type it out.

Either is fine.  While it is true that at very high frequencies, solid conductor wire shows increased impedance due to eddy current forcing the current to the outside, aka the skin effect, that is not the case at 60Hz and common wire sizes.  (Note:  a useful approximation for the wire diameter where the resistance increases by 10% is Dw = 200/sqrt(f), with f in Hz and Dw in mm.  So for 60 Hz, Dw is 25.8, or just over an inch.)  

The reason that we use stranded versus solid wire in our day to day lives is that solid wire is cheaper, but does not put up with the constant flexing of power cords.  So, we have solid core wire in our walls where it does not need to move, but cost matters, and stranded wire in our power cords where a solid wire would quickly work harden, embrittle and break.

Now, as to why the solid wire would work harden, embrittle and break, you need to understand that the strand diameter relative to the bend radius is what determines how much strain is imparted into the wire.  Solid wires have large strand diameters and see lots of strain.  Stranded wires have strands with small diameters and see much less.  

One last thing, the above statement about skin effect being of no consequence until relative high frequencies speaks to the actual sinusoidal components.  So if you have a square wave (or close to it) you would see quite a bit of impact on your edges if you used thick solid conductor wire.  Similarly, if the wire is in a magnetic field, say in a motor, eddy currents come into play at much lower frequencies.
```

---
## \#13 Posted by: chaka Posted at: 2016-01-13T16:06:22.584Z Reads: 295

```
I have learned long ago, when working with electricity it is best to stay within the specs of the materials and component used.

 I design for the worst possible scenario, 6s single motor pulling close to 80+ amps. The specs on 10 awg high strand silicone wire barely meet this demand. If you were to run conventional multi-strand 12 awg wire with a nylon insulator it would quickly heat up and possibly melt the insulator. 

Someone new to the sport will more, often than not, come to the plate with a 6s lipo and the capability to pull 80 amps becomes quite an easy task. It is irresponsible to use anything not built for the worst case scenario.

<img src='/uploads/db1493/original/2X/b/b041f15a19d7d5c9c0d478894688331a5e3d11e9.jpg'>
```

---
## \#14 Posted by: treenutter Posted at: 2016-01-13T16:50:29.388Z Reads: 283

```
Thanks for this @chaka; we had a thread a [few months ago abut wire guage][1] and I had concluded that for my 8s system with a single motor (max 70A), 12AWG silicone wire was sufficient. I've had no troubles with this set up so far. Do you think the that conclusion was correct?

Are the max motor amp ratings provided by manufacturers reliable, or are those figures exceeded in real-world use?

I based that on the image below that @lowGuido shared. 

http://www.electric-skateboard.builders/uploads/db1493/original/1X/7dd620e04f19d6750c05cf0b55bab78e0a0d5611.jpg

  [1]: http://www.electric-skateboard.builders/t/wire-gauge-in-esk8/213
```

---
## \#15 Posted by: chaka Posted at: 2016-01-13T17:12:57.774Z Reads: 266

```
In my honest opinion good 12 awg silicone wire will "get you by" but it is going to get hot frequently. DrBass did an actual real world test showing the actual temp measured through the insulation. You can imagine the conductor had a temp much greater than this.

[https://www.youtube.com/watch?v=0DhzWPoSYoQ][1]


  [1]: https://www.youtube.com/watch?v=0DhzWPoSYoQ
```

---
## \#16 Posted by: lowGuido Posted at: 2016-01-13T21:30:29.598Z Reads: 273

```
while I agree that bigger is most certainly better when it comes to wire gauge and current flow. well it is always better. heck just go as big as you can!

although sometimes we have to be a bit realistic with space and what not on our boards. its also important to remember that these are skateboards and not RC cars. I  have never pulled anywhere near as much current on my skateboards as I would on my RC car. my RC cars are regularly HOT to the touch. in fact I have actually burned my finger picking up my car before. my skateboard has never been that hot, ever.

to put this in some kind of scientific perspective for those who prefer that kind of thing.

I ride my skateboard for close an hour and I get about 15km out of the battery
so my average speed is 15km/h 
my battery is 5000 mAh, so you could say over my 15km hour long trip I have average current Draw of 5 Amps 

wait? what?
average of 5 Amps?
that doesn't sound like very much? but facts are facts on my average skate on any average day, my average current draw is 5 amps.
yeah sure i'll pull some 40Amps up a hill for a short time or something but these bursts are only short.
my average load is well within the specs of a good quality 12AWG cable.


UNLESS you are doing massive hill climbs for extended periods...  

everyone's situation will be slightly different, but 100A? I'm never gonna see it.
you guys have all the data of your own builds, you can do the simple maths and work out for yourselves if its worth the extra guage or not.
```

---
## \#17 Posted by: longhairedboy Posted at: 2016-01-14T18:55:08.559Z Reads: 261

```
trying to cram 10awg silicone wire into a low profile box with all the other stuff and having to route it all crazy because you have multiple ESCs and what not is already a challenge. 8awg would be a total troll, so i stick with 10awg.

since i've been testing this 10S build i've only found coolness. Cool motors, cool wires, cool ESCs, cool box. immediatley after a sprint i have warm (but not remotely hot) motors, cool wires, cool ESCs and a cool box and a set of warm (again, not remotely hot) belts. 

Hot? The only time i've seen hot is when my pulleys on my 6S worked their way into a rub with the older open source mounts i have on there and my 5060 270s were heating up as a result. That was the result of bad belt alignments and not using proper clips/keyways/notches while attempting to top out.
```

---
## \#18 Posted by: oriol360 Posted at: 2016-01-15T02:13:52.155Z Reads: 250

```
What do you guys suggest for a good flat cable that will hide well under grip tape?
```

---
## \#19 Posted by: longhairedboy Posted at: 2016-01-15T18:50:58.616Z Reads: 257

```
for power? or phase leads?
```

---
## \#20 Posted by: oriol360 Posted at: 2016-01-19T08:06:11.571Z Reads: 288

```
For power. I want to do my own kind of boosted clone without carving the deck to hide cables :/
```

---
## \#21 Posted by: longhairedboy Posted at: 2016-01-19T13:03:31.055Z Reads: 289

```
Something like this might work. 

http://www.ebay.com/itm/like/151895915285?ul_noapp=true&chn=ps&lpid=82

Is anyone else familiar with guaging requirments for the kinds of loads we would be putting on braided copper flat wire? 

I've often thought of doing something like this.
```

---
## \#22 Posted by: trbt555 Posted at: 2016-01-19T13:44:23.799Z Reads: 282

```
The net copper cross section is important but it's not stated in the ebay item description.
But let's say this braid is 1mm thick and 15mm wide, and contains 50% copper (estimate, the rest ia air between the individual strands), you have 15 x 1 x 50% = 7.5 square mm copper, which is a bit [less than AWG 8 but more than AWG 10][1].


  [1]: http://www.engineeringtoolbox.com/awg-wire-gauge-d_731.html
```

---
## \#23 Posted by: MonsterCoatings Posted at: 2016-02-09T15:22:05.675Z Reads: 265

```
I know under ceramic tiles we used to use flat copper wire when connecting floor heating systems, kind of like the old window security tape but heavier gauge. Wonder if that could also heat the deck for those chilly morning commutes???? LOL
```

---
## \#24 Posted by: laurnts Posted at: 2016-02-09T16:24:13.958Z Reads: 263

```
Interesting discussion, but I have a point to add here. I believe current (amps) only flows on the surface of a copper wire, hence high strand wire (more surface area) could deliver better current compared to same thickness of a single copper wire.
```

---
## \#25 Posted by: Blasto Posted at: 2016-02-09T16:45:04.504Z Reads: 253

```
You are referring to the skin effect, that happens at high frequency, not high current. Stranded and braided wires offer a mechanical advantage where the wire can be move around more than a single conductor with the same gauge
```

---
## \#26 Posted by: laurnts Posted at: 2016-02-09T16:54:08.019Z Reads: 253

```
Ohh well yes you're right. My mistake :)
```

---
## \#27 Posted by: longhairedboy Posted at: 2016-02-09T19:47:05.511Z Reads: 252

```
I'd like to point out that space cells apparently have 16awg mains. 16 GAUGE MAINS. 

which makes my 10 gauge mains policy pretty pointless as far as I can tell. I may as well just run 16 awg all the way up to the VESC.  

when i build my own packs they will have 10 gauge super worm mains. They'll also be 12S, but that's another topic for later.
```

---
## \#28 Posted by: laurnts Posted at: 2016-02-09T21:25:31.049Z Reads: 244

```
I've totally agree with 10 gauge by far is the most suitable wire I've ever used. It's not as rigid as 8 awg but does feel more sturdy than 8 awg. Lipo packs with 20 - 30c discharge uses this 10 awg - 12 awg wire, so it's also good reason to stick with it. 8 awg wire also doesn't fit into XT60, so it requires more expensive XT90 plugs. And again all of these wire sizes in the circuit does get affected by the weakest / thinnest cable, so thats the reason I also stick with all 10 awg.
```

---
## \#29 Posted by: chaka Posted at: 2016-02-09T23:31:57.179Z Reads: 243

```
[quote="longhairedboy, post:27, topic:970"]
I may as well just run 16 awg all the way up to the VESC.
[/quote]

 That would only exacerbate the weak link. Using 16 awg over a short distance will not have too much resistance but it would be bad news if you added more length at 16 awg.
```

---
## \#30 Posted by: Hummie Posted at: 2016-02-29T20:17:58.804Z Reads: 238

```
How about 18650 packs?  I see many different ways they're connected and they all look thin.  More so how about capacitance..will a typical 18650 pack need more capacitors?
```

---
## \#31 Posted by: Okami Posted at: 2017-01-27T21:46:22.863Z Reads: 179

```
Actually I think this was good topic.. 

It seems that for lower power setups, it is possible to use 14awg wire.. but since motors come with 12awg wire, that is also the size I sticked to..

14awg seems to be rated at something like 50-60Amps..

--

One thing why I started searching wire gauges / sizes.. with higher amps there seems to be quite high voltage drop.. this is especially a case for charger cables.. 

Sorry for bringing up this old topic.. just wanted to throw in what I use and what has been more important for me - the voltage drop because of the small wire diameter / its current capability

---
http://www.solar-wind.co.uk/cable-sizing-DC-cables.html

This site seems to give off some good estimate / info on what wire to choose.. based on distance / amps needed.
```

---
## \#32 Posted by: Schulerbible Posted at: 2017-01-27T23:50:53.999Z Reads: 160

```
The spacecell (Raptor battery) has 12 AWG leads and this is more than enough for the complete build. I am using the Raptor dual setup on a different board and I literally can not feel any temperature increase in the 12AWG HobbyKing wires.
```

---
