# Inboard battery and braking: Fresh &lt;&gt; Full

### Replies: 42 Views: 4726

## \#1 Posted by: Calhoun Posted at: 2016-01-11T09:28:34.009Z Reads: 192

```
Hi all, I'm trying to cut through Inboard's marketing-speak to figure out the physics involved. They didn't really confirm that they will undercharge, but if they're not force-feeding a full battery and have no secondary rheostatic or friction-based braking, there's no other way for the BMS to instamagically make the regen current disappear, right? 

>  Inboard: However, when the battery is full, the current has nowhere to go and braking is disabled to avoid damaging the battery. With the M1, you'll still be able to engage the brakes with a battery that's fresh off the charger."

> Gongfu Xiongmao: My physics teacher is a hardcore e-skate builder. He said that if you can brake with a M1 "fresh off the charger" the board is converting the current to heat somewhere or putting back into the battery (electricity). Does this mean that the M1 will always be charged under capacity to leave room for braking regeneration current? Isn't this sacrificing distance for those few clients who happen to live atop large hills? Top speed would be lower, since a lower charge would also mean less top voltage/power too? 

> Inboard: Hey Gongfu. For us addressing this was more of a safety issue than anything else... not as much for the few clients who live on top of a large hill, but those who don't but may occasionally start on top of a large hill and expect the brakes to work on a fresh battery. Without this feature they're in for a dangerous surprise. I can only say we're using the BMS to manage this extra power, and so far this is not sacrificing advertised distance or advertised top speed.
```

---
## \#3 Posted by: trbt555 Posted at: 2016-01-11T10:37:48.536Z Reads: 184

```
Looks to me they're undercharging the battery to prevent customers living on top of a hill losing their braking function due to a full battery. But the braking current will be so small and of such short duration, I don't think they need to undercharge so much that it will affect range.
```

---
## \#4 Posted by: longhairedboy Posted at: 2016-01-11T12:30:13.228Z Reads: 181

```
how much current is actually generated during braking above and beyond the current used to actually **do** the braking? And is that even enough to worry about? it seems like the steeper the hill the more current it would take to keep you slowed down.
```

---
## \#5 Posted by: psychotiller Posted at: 2016-01-11T12:43:42.420Z Reads: 175

```
I believe they are trying to focus on those who don't brake down hill. Not sure it matters though.  That energy has to go somewhere.
```

---
## \#6 Posted by: longhairedboy Posted at: 2016-01-11T12:51:00.040Z Reads: 170

```
Ah, of course. I was too busy thinking about the braking instead of the not-braking. I suppose they don't want to just cut the current at the ESC and let the motors dissipate the heat via those cool fan-shaped wheel hub covers.
```

---
## \#7 Posted by: Calhoun Posted at: 2016-01-11T13:15:23.774Z Reads: 167

```
No current is used in regen (induction) braking; just the opposite. ("DC injection braking" on the other hand, is the use of a separate power source to create a static magnetic field which slows the motor.)

Cutting the current before the ESC would be bad. Or impossible. The more kinetic energy being converted into current, the stronger the braking. If 0 current is pulled from the motor, there is no braking. Like psychotiller said, the current has to go somewhere. Also, the first place where you really don't want excess heat is the motor...the battery can at least be replaced more easily.

Rheostatic/dynamic braking would give you what you are looking for longhairedboy. If the current or load is too high for the battery to take, the BMS will shunt it to a resistor, converting electricity to heat (and global warming!) and dissipating it. Mellow Drive is the only e-skate setup that I know of with this secondary braking ability.

Question to the forum: For rheostatic braking...why a resistor? Would it be possible to dissipate electricity with a big huge spark from a huge capacitor, like a Taser? Also, wouldn't that be bad-ass? The Max Max e-skate.
```

---
## \#8 Posted by: trbt555 Posted at: 2016-01-11T13:15:53.366Z Reads: 151

```
When you're going downhill and braking your motor management electronics are allowing the motors to generate a current which is then fed back to the battery. This current flowing through the motors creates an electromechanical force which tries to slow the motor down.

When you're going downhill without braking (neutral), your motor managment electronics are not allowing this current to flow, thus preventing the electromechanical force from slowing the motor down.

So basically if you start down a hill with a full battery and the electronics don't allow the current to go anywhere, you don't have brakes.
```

---
## \#9 Posted by: psychotiller Posted at: 2016-01-11T13:58:29.244Z Reads: 146

```
I have had a board stop on a hill I was coasting down. The batteries were dead so I was pushing my way home. In fact it got to the point that just trying to push on flats was impossible. The motors generate power even when coasting. And if the power has no where to go, things happen.
```

---
## \#10 Posted by: trbt555 Posted at: 2016-01-11T14:02:33.813Z Reads: 142

```
That's weird.
I can easily push my board with an empty battery (or even turned off).
May have something to do with individual controllers ESC/VESC whatever.
```

---
## \#11 Posted by: psychotiller Posted at: 2016-01-11T14:17:27.487Z Reads: 143

```
Yeah I never figured it out. It was a castle controller. One of many. It was the only build I had that did it. I accepted it as just that board's personality. Tore it down , rebuilt, same esc, different result. I know that it's possible now though, and it is always in the back of my mind.
```

---
## \#12 Posted by: Calhoun Posted at: 2016-01-11T15:05:33.688Z Reads: 133

```
Latest video from CES has a shot of Inboard's battery label: hello 12s1p!!!
http://www.digitaltrends.com/cool-tech/inboard-m1-electric-skateboard-hands-on-ces-2016/
```

---
## \#13 Posted by: chaka Posted at: 2016-01-11T15:16:39.518Z Reads: 137

```
[quote="trbt555, post:8, topic:964"]
echanical force which tries to slow the motor down.

When you're going downhill without braking (neutral), your motor managment electronics are not allowing this current to flow, thus preventing the electromechanical force from slowing the motor down.

So basically if you start down a hill with a full battery and the electronics don't allow the current to go anywhere, you don't have brakes.
[/quote]


I have been thinking, what if we introduced a chiller plate for excess regenerative current? I have not done any calculations yet but it would be a good use of the excess regen.
```

---
## \#14 Posted by: Calhoun Posted at: 2016-01-11T15:25:44.063Z Reads: 133

```
Awesome. Talk about conservation/conversion of energy: Electric (wall socket) to chemical (battery) to electric (current to motor) to kinetic (riding!) to electric (braking) to thermal (chilling) to chemical (cold beer) to biological (buuuurrrrp). 

Those poor electrons do so much work for us.
```

---
## \#15 Posted by: chaka Posted at: 2016-01-11T15:33:29.733Z Reads: 126

```
This is a 12v 5  amp module: [Peltier Thermo-Electric Cooler Module - 12V 5A][1]

It measures 40mm x 40mm so it would be perfect match for the VESC. Would only add 3.5mm to the height.


  [1]: https://www.adafruit.com/products/1330
```

---
## \#16 Posted by: trbt555 Posted at: 2016-01-11T15:49:07.871Z Reads: 120

```
I don't get your intentions here @chaka, you want to actively cool the VESC ?
```

---
## \#17 Posted by: longhairedboy Posted at: 2016-01-11T15:50:21.926Z Reads: 122

```
if it could be done only while braking or coasting it might make sense in extreme use cases like racing.
```

---
## \#18 Posted by: Calhoun Posted at: 2016-01-11T15:58:31.994Z Reads: 125

```
I seem to have misinterpreted what the chiller plate was for. Sorry. Hic.
```

---
## \#19 Posted by: chaka Posted at: 2016-01-11T16:04:00.800Z Reads: 128

```
I suppose you could use the excess energy for anything you like. Cooling the system just seems to be the most practical use. The esc would most likely be very hot if you have already been using the brakes heavily. You would need to develop a circuit of course but it can be done.

@Calhoun You can use these chiller plates for all kinds of projects. The specs state a max temperature differential of 66°C.
```

---
## \#20 Posted by: lowGuido Posted at: 2016-01-11T23:06:50.320Z Reads: 121

```
the problem with the peltier "chiller plate" is that in order to get cold it needs to get hot on the other side, so you will need to heat sink the hot side thus almost negating the relatively slim hight of the  plate.
```

---
## \#21 Posted by: chaka Posted at: 2016-01-11T23:24:36.159Z Reads: 120

```
You could pop it through the enclosure. I think that kind of thing looks nice when done right.
```

---
## \#22 Posted by: trbt555 Posted at: 2016-01-12T06:37:04.694Z Reads: 112

```
You could pop your vesc heatsink through the enclosure and save yourself the hassle.
```

---
## \#23 Posted by: lowGuido Posted at: 2016-01-12T07:43:07.363Z Reads: 113

```
oh by the way, to understand the OP's confusion you need to first understand that coasting or braking will both generate power. the harder you brake the more power you generate. generally this power is soaked up by the caps and eventually charges back into the battery.
the point in question is that if the battery is fully charged what happens to the power?? some ESC's will prevent braking from happening to eliminate the risk of over charging lipos and setting fire to your legs.
smarter designs will incorporate a BMS, which uses a series of resistors connected to each cell which will actually burn off (hahah bad choice of word) bleed off any excess voltage when compared to the other cells so that the cells always stay "balanced". 
One would then have to assume that a more sophisticated BMS would be able to also use a resistive circuit to bleed off any excess voltage gained by regenerative braking when the battery is hot of the charger full.
```

---
## \#24 Posted by: Calhoun Posted at: 2016-01-12T11:12:22.876Z Reads: 113

```
Thanks @lowGuido. What are "caps"? 

Are the registers used for balancing able to soak up a lot of current if the cells are all full? 

So to permit braking in a "fresh" battery, Inboard is either undercharging, or using the BMS balancing registers, or using a dedicated braking resistor?

Is DC injection a viable method for braking e-skates?
```

---
## \#25 Posted by: lowGuido Posted at: 2016-01-12T11:20:54.808Z Reads: 105

```
caps = Capacitors
Also I am not speculating on the design that any particular people use in their BMS, either employing the balance resistors or a separate over voltage resistive circuit. either way, a resistor will work regardless of the level of charge in the battery.

they do not need to under charge anything.
```

---
## \#26 Posted by: longhairedboy Posted at: 2016-01-12T14:28:58.550Z Reads: 103

```
This thread has been very informative. I realize now that i had no clue how regen brakes actually worked.
```

---
## \#27 Posted by: lowGuido Posted at: 2016-01-12T22:38:10.748Z Reads: 97

```
a cool thing to do is to hook up LED's to your motor and then spin the motor to light the LEDs 
doesn't really achieve anything but its kinda fun.
```

---
## \#28 Posted by: longhairedboy Posted at: 2016-01-12T23:09:34.080Z Reads: 94

```
yeah my volt meter lights up pretty bright when i spin my wheels on my 6S.
```

---
## \#29 Posted by: psychotiller Posted at: 2016-01-12T23:22:22.842Z Reads: 95

```
That's power son! Who knew?
```

---
## \#30 Posted by: longhairedboy Posted at: 2016-01-12T23:36:18.915Z Reads: 95

```
so hold up i need to get the image in my head a little clearer... so regen braking is basically allowing a load to be put on the motors (which are now generators, or alternators?) by having the power it generates fight against the current that's coming from the battery? 

my artist brain wants images.
```

---
## \#31 Posted by: psychotiller Posted at: 2016-01-12T23:56:39.650Z Reads: 93

```
Yup. Generators.  Maybe we could install plasma weapons on our boards to use up all of our downhill energy.
```

---
## \#32 Posted by: longhairedboy Posted at: 2016-01-12T23:59:27.044Z Reads: 95

```
phased plasma pulse rifles in the 60 megawatt range, like the ones that the terminator was looking for in the pawn shop.
```

---
## \#33 Posted by: psychotiller Posted at: 2016-01-13T00:14:50.968Z Reads: 96

```
Yup and we could shoot ankles and tiny dogs!
```

---
## \#34 Posted by: lowGuido Posted at: 2016-01-13T00:32:44.824Z Reads: 99

```
the best way I can put it is like this:

if you dump a load of current into a motor and try to hold it still with your hand, the more current flows the harder it is to stop the motor from turning.

generator is motor exactly in reverse.

if you Suck a load of current from a generator and try to turn the generator by hand, its going to become very hard for you to continue turning the generator.

in closing, brakes suck.
```

---
## \#35 Posted by: MonsterCoatings Posted at: 2016-01-13T08:51:38.126Z Reads: 100

```
I think we could all settle this very easily with a beginner lesson.
https://www.youtube.com/watch?v=_dFzOHyZSNk
```

---
## \#36 Posted by: trbt555 Posted at: 2016-01-13T11:11:57.212Z Reads: 101

```
Good point. Let's not forget we're on longboards and it's important to master the basic techniques too.

Something they forgot to mention in the video and something I know from first-hand experience: when footbraking avoid hitting your rear wheel with your foot or you'll street your face.
```

---
## \#37 Posted by: longhairedboy Posted at: 2016-01-13T13:19:07.369Z Reads: 100

```
that's also an excellent rule to follow when pushing. lol
```

---
## \#38 Posted by: Calhoun Posted at: 2016-01-13T16:20:36.845Z Reads: 102

```
A BLDC electric motor moves by running current through the windings to create electromagnets, timing it in such a way that the active ones will be attracted by the next permanent magnet, and repelled by the one it has just passed, moving the rotor and thus the load. 

In braking, your movement/inertia is the power source that turns the rotor, pushing electrons through the windings by induction and thus supplying current to the electromagnets. The logic controlling the current strength and signal timing (charging the right phases/electromagnets) is reversed. Instead of facilitating this "hand-off" from one magnet to another, the process is rendered more difficult be repelling where previously attracted, etc. The battery becomes the load that you are "pushing."

tldr: In forward movement, battery current pushes electrons through windings creating magnetic attraction/repulsion which turn the rotor and push you. Braking is your movement turning the rotor, using induction to push electrons through the windings towards the battery, creating magnetic friction that slows the rotor.
```

---
## \#39 Posted by: longhairedboy Posted at: 2016-01-13T18:18:27.590Z Reads: 99

```
Thank you for a clear and concise explanation that my artist brain can handle. This makes perfect sense to me now.
```

---
## \#40 Posted by: Calhoun Posted at: 2016-01-14T14:44:29.875Z Reads: 99

```
Awesome! Here's an even shorter version.

To braking, you push zillion electron. To moving, like in Soviet Russia, zillion electron push you.

(Could have made it shorter without the joke, but couldn't resist.)
```

---
## \#41 Posted by: Hillso Posted at: 2016-04-26T06:54:26.797Z Reads: 86

```
The solution seems very simple to me if its possible. Just use DC injection braking and switch to regen when the battery is 95% full. and than switch again when the battery is 100% full.
does the VESC have DC injection braking, and Is it possible to do this switch thing with the VESC?
```

---
## \#42 Posted by: trbt555 Posted at: 2016-04-26T09:58:05.384Z Reads: 81

```
Vesc has regen braking only.
```

---
## \#43 Posted by: Calhoun Posted at: 2016-05-04T12:33:51.489Z Reads: 73

```
DC injection braking apparently generates a lot of heat in the motor. You probably don't want that.
```

---
