# Riding with focbox turned off?

### Replies: 65 Views: 1982

## \#1 Posted by: DK-Odense Posted at: 2017-10-18T21:46:02.104Z Reads: 267

```
Hi guys

Noob question: if i roll my board downhill with my focbox turned off by a antispark (PCB with button from esk8.de) will i then blow my vesc?

I mean, blown from the power generated from the rolling motor with no acces to allow regenerating the batteri, since the antispark is off.
```

---
## \#2 Posted by: ninja Posted at: 2017-10-18T21:52:39.407Z Reads: 264

```
I'm also interesting in this. Also I don't get it where goes generated energy when you just cruising with no throttle pushed? I mean after you get your desired speed by pushing throttle and then just letting go throttle. So when we brake with vesc we charge battery, but what happens on free rolling with antispark swiched on? Where goes generated energy- also charging battery?
```

---
## \#3 Posted by: RedEagle Posted at: 2017-10-18T21:59:53.904Z Reads: 256

```
If you exceed the erpm limit (60.000 erpm) while going downhill with a board that is on you will likely blow your vesc.

Regarding your question.. no I don't think you will blow anything when going downhill because you pulled out the antispark, therefore breaking the circuit.
```

---
## \#4 Posted by: chaka Posted at: 2017-10-18T22:04:26.212Z Reads: 250

```
The board will turn on, the reverse current will charge the MOSFET's in the switch and allow power to flow back into the pack.
```

---
## \#5 Posted by: Jinra Posted at: 2017-10-18T22:06:02.771Z Reads: 239

```
Wait really? So if even an antispark switch is turned off, a reverse charge will turn it on and let power through?
```

---
## \#6 Posted by: RedEagle Posted at: 2017-10-18T22:07:26.936Z Reads: 233

```
That's what I'm wondering about now...
```

---
## \#7 Posted by: ducktaperules Posted at: 2017-10-18T22:08:39.207Z Reads: 232

```
If your "free rolling" then there is no energy generated. if your not accelerating or decelerating then i would assume all of the FET's on the esc are off and the motor is basically disconnected so there is no energy to go anywhere. Also if you exceed the erpm limit but your not asking for any power then again it shouldn't matter cause the motor is not connected.
```

---
## \#8 Posted by: Martinsp Posted at: 2017-10-18T22:09:11.754Z Reads: 227

```
Theoretically that is the way (as @chaka said) it works, because of the body diodes in the mosfets. I have not tested it myself so "theoretically".
```

---
## \#9 Posted by: Jinra Posted at: 2017-10-18T22:10:09.321Z Reads: 224

```
There is at least some electricity generated. If you spin your wheels by hand you'll see the lights on the vesc light up.
```

---
## \#10 Posted by: ninja Posted at: 2017-10-18T22:11:13.692Z Reads: 217

```
1) So going down hill with no braking, no throttle applied, with turned on board- it still be charging battery?

2) going down hill with turned off antispark switch will not damage anything?
```

---
## \#11 Posted by: ducktaperules Posted at: 2017-10-18T22:12:16.185Z Reads: 207

```
interesting . . .
```

---
## \#12 Posted by: Martinsp Posted at: 2017-10-18T22:13:22.944Z Reads: 203

```
If you dont exceed the limit. there was a thread recently that was explaining this. People there were discussing going down hill and passing 60k ERPM. I am not sure about the name maybe someone remembers :/
```

---
## \#13 Posted by: HifuSk8 Posted at: 2017-10-18T22:15:33.240Z Reads: 197

```
So first Off, it seems correct to me that you risk to blow something if going downhill very fast, so I wouldn't do it.

Second: why would you wanna Turn Off your Board via Antispark when going downhill?  Because you cant break and therefore, you just end up with a heavy Board with no breaking.

To try to ansewer the other question, wich Ninja asked (as far as I understand, correct me of I'm wrong):

No where! Because when free-rolling ( No throttle, No Breaks) your Motor does not generate any current.
```

---
## \#14 Posted by: scepterr Posted at: 2017-10-18T22:16:19.597Z Reads: 190

```
If you take your board and disconnect from power and spin the motor you'll see the lights flicker on
Motor generates electricity whether breaking or not
Regen just channels that to battery
```

---
## \#15 Posted by: RedEagle Posted at: 2017-10-18T22:16:23.305Z Reads: 184

```
1) It'll charge the battery when you brake. Be careful not to exceed the erpm limit though.

2) Correct (theoretically)
```

---
## \#16 Posted by: ninja Posted at: 2017-10-18T22:22:38.560Z Reads: 182

```
I see antispark led switch(light) turning on when just turning drive wheel by hand when board is off. So energy generates. I don't want to go down hill with turned off board, i just want to understand what happens when cruising with no throttle, since i see that motor genarates energy just from spinning it.
```

---
## \#17 Posted by: scepterr Posted at: 2017-10-18T22:31:22.317Z Reads: 177

```
Well you just explained what happens 😉

I don't think it's healthy for the vesc
```

---
## \#18 Posted by: HifuSk8 Posted at: 2017-10-18T22:42:19.476Z Reads: 177

```
Yes there will be some Energy generated, since moving Magnets (Rotor) over a Coil (Stator) induces current.but Not a Lot. That ist what you see and that ist correct.

I am probably oversimplifing but when you apply throttle, your VESC will control the voltage like so, that the created magnetic field in the stator is ahead of the Position of the Magnets in the Rotor, thus you Draw current (a Lot) and the Motor moves.

If the Rotor moves because you're going downhill and you apply the Breaks, your VESC will control the voltage like so, that the created magnetic field in the stator is behind the Position of the Magnets in the Rotor, thus the Magnets try to slow down, they induce a negative Current .
```

---
## \#19 Posted by: jmasta Posted at: 2017-10-18T23:07:55.165Z Reads: 168

```
You need the VESC turned on, even if you're cruising with no throttle.  The motor acts as a generator and produces a small amount of electricity. If the VESC is off, that power has nowhere to go.  It can handle some until the caps are charged, but after that you can blow your speed controller.  There are some threads on it on the VESC forums if you are interested

One spin of my wheel by hand with the VESC "off" is enough to power on the receiver, voltmeter, and Bluetooth adapter for a second
```

---
## \#20 Posted by: DK-Odense Posted at: 2017-10-19T05:28:18.901Z Reads: 157

```
So, the real thing is that i have build a 4wd board, with a antispark in both ends. This will allow med to choose between fwd, rwd or 4wd by disconnecting the vescs. 

Works like a charm at slow in my test environment.... Then i thought - what happens at high speed with the disabled vescs. 

For information this is hub motors 70 KV.
```

---
## \#21 Posted by: scepterr Posted at: 2017-10-19T05:31:42.151Z Reads: 147

```
Seems like some kind of 3 phase disconnect switch on each motor would be required or physically disconnecting the motors.
```

---
## \#22 Posted by: Acido Posted at: 2017-10-19T05:42:12.615Z Reads: 146

```
If there is no connection between motor na vesc there will not be any problem
```

---
## \#23 Posted by: Jinra Posted at: 2017-10-19T05:56:15.693Z Reads: 143

```
i don't think that's what the question is though. Also dangling phase wires is a concern if you disconnect :p if they accidentally touch, it'll send you flying.
```

---
## \#24 Posted by: Hummie Posted at: 2017-10-19T05:56:46.525Z Reads: 141

```
someone mentioned it above and thought it worth mentioning and I wondered about it a lot:


you can go down hill as fast as you want as long as you don't go over the erpm limit it wont damage esc but if you go over your no-load speed, based on your kv and voltage, your throttle will turn into a brake.
```

---
## \#25 Posted by: ARetardedPillow Posted at: 2017-10-19T06:55:33.284Z Reads: 135

```
Hmm does that mean if I roll my board enough with the circuit not completed, Id blow out my vesc?
```

---
## \#26 Posted by: DK-Odense Posted at: 2017-10-19T07:37:01.800Z Reads: 131

```
Thank you for all your feedback guys, but I feel that a lot of untestet theories are being thrown in the air here 😁

Some says that nothing happens, and some says that it will blow up.

Is there any people here with actual experience what happens to the vesc, if the vesc loses battery connection at high speed (eg, if a plug/soldering disconnects )?

Or even better, a vesc electronics developer is present in here?
```

---
## \#27 Posted by: scepterr Posted at: 2017-10-19T07:58:27.386Z Reads: 127

```
I don't think anybody is saying it will blow up...just that you could degrade components if they're constantly charged and powered by the current from the motor. There are a lot of variables that come into play into how long you'de have to do this to cause damage
```

---
## \#28 Posted by: GrecoMan Posted at: 2017-10-19T10:59:05.427Z Reads: 115

```
lol @scepterr “makes” vesc’s...
```

---
## \#29 Posted by: scepterr Posted at: 2017-10-19T11:00:21.973Z Reads: 117

```
I assemble, repair, I don't think "makes" is a fitting term 😋
```

---
## \#30 Posted by: GrecoMan Posted at: 2017-10-19T11:00:51.576Z Reads: 113

```
there’s a reason I put “makes” in quotes 😉
```

---
## \#31 Posted by: longhairedboy Posted at: 2017-10-19T11:47:41.683Z Reads: 116

```
[quote="chaka, post:4, topic:35906, full:true"]
The board will turn on, the reverse current will charge the MOSFET's in the switch and allow power to flow back into the pack.
[/quote]

This is what i have seen too. And if everything is on, and you pass the ERPM limit, you'll either pop stuff or get "enforced with negative torque" if that's what's set up in your vesc. 

the idea that the motors only generate enough current "to matter" when the vesc is on is ridonkulous.
```

---
## \#32 Posted by: FredSaberhagen Posted at: 2017-10-19T13:21:21.163Z Reads: 114

```
What nobody is saying in this thread is that without power to the vesc you can't really turn those FETs off.

To pull the gate of an NFET low (turn it off) you need a current sink

Where is that gonna come from?  Thus the tiniest amount of charge floating around (maybe a faerie farts on your vesc and deposits 10 nano coulomb) can turn on a FET and allow current flow

ERPM limit is meaningless if your FETs are truly off and you're freewheeling.  You don't have to "keep up" with the changing polarities.  Ofc if you wanted to apply brakes you'd need to be under the eRPM 

If you can truly disconnect from the motor phase wires then you could run your motor downhill for days and never care

Just disconnecting power from your vesc is a bad idea since you just have an indeterminate state of phase FETs  - and with a solid state switch like in the antispark as Chaka said it will still allow backwards current. 

If you really want to tune in, turn off and drop out put a dual throw triple pole switch in shunt with your phase wires and flip that bitch off.  Now freeroll all you want
```

---
## \#33 Posted by: chaka Posted at: 2017-10-19T13:25:04.856Z Reads: 107

```
> I don't think anybody is saying it will blow up...just that you could degrade components if they're constantly charged and powered by the current from the motor. There are a lot of variables that come into play into how long you'de have to do this to cause damage

It wont hurt any components by allowing current to flow intermittently in either direction. You can corrupt the firmware from too low of voltage for an extended period but I have only seen this happen once. Might have been a fluke. 

One thing that surprises people is the motors will generate power whenever they are spinning. Even if we are on the throttle they are still generating power. During heavy braking they can generate more current than we use when on the throttle. This is a big reason why I build massive battery packs, they can take heavy regen without having the voltage spike too much.
```

---
## \#34 Posted by: longhairedboy Posted at: 2017-10-19T13:57:15.204Z Reads: 100

```
[quote="chaka, post:33, topic:35906"]
This is a big reason why I build massive battery packs, they can take heavy regen without having the voltage spike too much.
[/quote]

Word. I would go so far as to say that is the cake, while further mitigating voltage sag and providing more power and range in general, not to mention the robustness you can get from the additional cells, is the icing.
```

---
## \#35 Posted by: DK-Odense Posted at: 2017-10-19T15:33:04.558Z Reads: 103

```
Hmmmm - Thank you for the good answers. So what I hear is that it may not break my vescs, but then again it may still break them over time :smiley: What to do. 

My idea was that I could drive with rwd as a daily driver, and make it 4wd when it's going to be fun or at hill climping. Therefore, I made the opportunity to disconnect the motors with an anti spark unit.

I searched for a electrical relay, and a mechanical button to integrate in the enclosure, but haven't really found anything with three poles / contacts that fit into my build. Maybe i'm doomed to always be running in quattro-mode :open_mouth:

I guess that one day i will forget to turn on either fwd /rwd and then we will see what happens.
```

---
## \#36 Posted by: longhairedboy Posted at: 2017-10-19T17:27:10.700Z Reads: 102

```
you could run individual eswitches. but unless you disconnect the phase leads you're going to be throwing current at the entire system the entire time from whatever ESCs you cut power to.
```

---
## \#37 Posted by: psychotiller Posted at: 2017-10-19T17:33:13.202Z Reads: 99

```
This is wrong...The motor is a generator. I have personally melted motor wiring as well as burned out mosfets. The motor does generate power and it has to go somewhere. If the board doesn't turn back on to allow energy through, things will melt.
```

---
## \#38 Posted by: longhairedboy Posted at: 2017-10-19T17:41:53.967Z Reads: 98

```
[quote="psychotiller, post:37, topic:35906"]
If the board doesn't turn back on to allow energy through, things will melt.
[/quote]

Your mom's going to melt.
```

---
## \#39 Posted by: Blasto Posted at: 2017-10-19T18:05:59.518Z Reads: 98

```
If you have a mosfet switch, the current will run though the internal diode of the mosfet and back to the battery. Even if the fet is open (off)
```

---
## \#40 Posted by: DK-Odense Posted at: 2017-10-19T18:25:51.397Z Reads: 96

```
With this you are saying that it is okay to to leave the vesc off, because the current is just going through the vesc -> anti spark -> BMS -> Battery?

This is the antisparks: https://dqzrr9k4bjpzk.cloudfront.net/images/7570530/480656861.jpg
```

---
## \#41 Posted by: Blasto Posted at: 2017-10-19T18:44:52.444Z Reads: 97

```
[quote="DK-Odense, post:40, topic:35906"]
With this you are saying that it is okay to to leave the vesc off, because the current is just going through the vesc -&gt; anti spark -&gt; BMS -&gt; Battery?
[/quote]

yes, it will power up the esc, so if you have your remote on and accidentally hit the brakes, it will brake


<img src="/uploads/db1493/original/3X/7/c/7c5aa9c36b6d0c614b5e20a4c03f16cdceebc1ac.png" width="384" height="428">
```

---
## \#42 Posted by: DK-Odense Posted at: 2017-10-19T19:55:14.686Z Reads: 95

```
Thats actually nice, because i will never have det remote off - either 4wd or rwd, using the same remote. 
So if the only "downside" is that the vesc is still able to brake, it is not a downside at all :smiley: 

But you are sure that the vesc will be powered by the generated current from the free rolling motors?

I think I owe you a picture of the monster:
<img src="/uploads/db1493/original/3X/b/b/bb5358446477815fa4521cf6b8088fe09302d2ed.jpg" width="690" height="479">
```

---
## \#43 Posted by: FredSaberhagen Posted at: 2017-10-22T15:56:33.650Z Reads: 89

```
Not necessarily wrong but the motor only "generates power" when you have a full closed current loop.

If you are free wheeling a motor even at high speeds it is not a generator!  In order for it to "generate" power you have to trade kinetic energy for electrical.  If you are coasting,  "generating power without braking", then you win the Nobel prize for disproving basic laws of physics.  Free energy!!!  

Now with a powered off VESC you may or may not have a connection for the phases (FET gates are indeterminate states) and if at some point you are in a braking situation then yep Now it's a generator.
```

---
## \#44 Posted by: psychotiller Posted at: 2017-10-22T16:01:00.993Z Reads: 88

```
So...Explain to me then, @FredSaberhagen  How did my motor wires melt and phase out while riding downhill with the board off?

Second time, explain to me how my mosfets melted and phased out my motor while being towed with the board off?

I never said anything about creating free energy...Rolling downhill is the equivalent of the wind spinning a turbine. Something from something.

The motors do generate power from spinning. They are generators.
```

---
## \#45 Posted by: chaka Posted at: 2017-10-22T16:36:12.443Z Reads: 85

```
But the motor does generate energy while coasting. It generates power while on the throttle too.... just not as much as it consumes. Are you talking about a motor with the phase wires disconnected?
```

---
## \#46 Posted by: FredSaberhagen Posted at: 2017-10-22T16:59:18.135Z Reads: 81

```
It's because when your vesc was turned off (no current sink output from drv pulling their gates *low* - all fets are nfet in vesc) the gates probably floated (they call it shoot-thru) and connected two of your phase wires to each other.  Youll get the same result if you connect two phase wires and tow your board :slight_smile:
```

---
## \#47 Posted by: FredSaberhagen Posted at: 2017-10-22T17:00:51.206Z Reads: 81

```
Yes if youre driving it then a current loop exists and it does have a back emf (why we need 14S) to beat that.  If the vesc is on then it can effectively disconnect and float the phase wires and you dont pay a inertial momentum penalty.  Nothing generated (to generate you would have had to put in kinetic energy to trade for coulombs)

To test this - what would happen to a motor with dangling phase wires connected to nothing - if you spun it up really fast?  Would it explode from all the energy "generated" with no where to put it (it would have to dissipate it as heat?)
```

---
## \#48 Posted by: psychotiller Posted at: 2017-10-22T17:14:33.129Z Reads: 76

```
I've thought of this scenario too. Not sure. Heat builds up though to a point where things will melt. That is how my motor phased out . The power created had no where to go.

I'm not the only one this has happened to.
```

---
## \#49 Posted by: Deckoz Posted at: 2017-10-22T18:09:47.275Z Reads: 73

```
Fred is right. 

Motors don't make energy by just spinning. "Energy" aka "electrical energy" ie Watts requires voltage and current. When a motor is being used as a generator, with no load, it creates voltage based on its kV and rpm. Ie it makes voltage with no current as there is no load. 

Once you add load such as the vesc with nfets the load (even though small) is powering the vesc, the vesc boots up and keeps sync with the motor, when your towing you speed up and slow down, slowing down and the voltage drops below minimum input, vesc at low speed goes though what is called "electrical brown out" where the voltage is enough to keep the mechanism on, but to low of voltage to function properly. Possibly leaving the vesc out of sync with the motor, shorting braking and causing heat. 
 
Solutions
-disconnect the belt
-unplug or switch cut the phase wires
-ride with the board plugged 
-design an esc?
```

---
## \#50 Posted by: psychotiller Posted at: 2017-10-22T18:31:51.179Z Reads: 71

```
[quote="Deckoz, post:49, topic:35906"]
Solutions
-disconnect the belt
-unplug or switch cut the phase wires
-ride with the board plugged 
-design an esc?
[/quote]

Why would you need to do any of those things if no power/heat is created?

A bottleneck is a bottleneck.

And outrunners most definitely create energy by spinning.
```

---
## \#51 Posted by: Deckoz Posted at: 2017-10-22T18:34:22.015Z Reads: 67

```
If the vesc is connected refer to brown out section of post.

If the motors phases are disconnected no load is there just voltage at rpm

The only way you could have melted if the phases were disconnected is if there was already a short in the phases from the enamel melting off.
```

---
## \#52 Posted by: psychotiller Posted at: 2017-10-22T18:35:02.650Z Reads: 66

```
Nope! 10 characters  HEAT.
```

---
## \#53 Posted by: Deckoz Posted at: 2017-10-22T18:38:40.887Z Reads: 65

```
Lol heat doesn't appear from thin air. Magnetic flux of a no load motor(generator)...making that much heat I doubt too. 

So please explain where the heat is coming from.
```

---
## \#54 Posted by: chaka Posted at: 2017-10-22T18:38:54.576Z Reads: 70

```
I guess if we make a hypothetical argument we can say anything we want but the fact remains the motor will generate power and turn the vesc on if it is in circuit with a soft switch. That's why we can use our brakes if we are coasting with the board switched off.
```

---
## \#55 Posted by: psychotiller Posted at: 2017-10-22T18:44:56.207Z Reads: 70

```
Seriously? The heat comes from energy created by the motor spinning. That energy with no where to go creates heat. Heat melts copper and mosfets.

I've seen it happen 2 times.
```

---
## \#56 Posted by: FredSaberhagen Posted at: 2017-10-22T19:57:26.622Z Reads: 69

```
And @chaka this analogy will make more sense:

Imagine you are breathing though a big straw.  In, out, repeat, in the air.  Not that hard.

This is what happens in your motor as a magnet passes a pole.  Magnetic field in/out

Now, it's easy to do in the air.  But if you place the straw in a bucket of water it becomes very hard.   You still have to breathe in and out ... but now you're moving a mass of water up and down the straw.

That water sloshing back and forth has friction in the straw.  Friction = heat of course

So take away the pool of water/phase connection and no work no friction no heat :-)  

When you say " I have brakes when rolling  powered off" then you are not powered off ;-)  like compression starting a car I guess.   Only way to stop that would be to have a source actively sinking all 6 of your FETs at all times.

Psycho you are a little bit right in that those big outrunner magnets have a little bit of resistance to them ... flipping that mag field back and forth does induce eddy currents and lose a little energy to heat!

This mellow mitigated by stacking up loads of tiny tiny magnets insulated from each other so eddy current loops must be very small.  If you have a cheap motor with one big long magnet you will pay more % in eddy currents for sure (besides friction, this the only reason cogging isn't truly energy neutral)
```

---
## \#57 Posted by: chaka Posted at: 2017-10-22T20:08:26.076Z Reads: 68

```
I'm not sure you are understanding. This is a commonly observed behavior of a well designed board. If it is switched off and you roll down a hill it will turn on, simple as that. Thanks for the explanation though, I have a pretty good understanding of how motors work ;) But your analogy will definitely help others around here.

Maybe you are arguing what happens in a broken circuit, i.e. no soft switch. If that is the case you wont here me arguing anything.... I have my regular kick push boards for that!
```

---
## \#59 Posted by: Hummie Posted at: 2017-10-23T19:10:06.089Z Reads: 56

```
So ur saying even w batteries connected but board not turnrf on if going at slow speeds as the  vesc turns on and off that's a brownout and potential damage ?
```

---
## \#60 Posted by: DK-Odense Posted at: 2017-10-23T19:13:53.730Z Reads: 57

```
Thank you for all your in-depth  answers guys. It is interesting reading stuff.

I think, however, I found a completely different solution. I put a switch to disconnect the supply to the two front axle remote receivers, so that I can drive rwd with the two front controllers powered on.

They Will not react to the remote input since they dont receive a signal from the remote control, but the vescs are still on controlling the motors.

What do you think about solution?
Let me know if i have to explain it in another way (and no - english is not my first language) 😊
```

---
## \#61 Posted by: Deckoz Posted at: 2017-10-23T19:20:52.864Z Reads: 61

```
@Hummie If your batteries are DISCONNECTED, ie board not turned on, with or without a soft switch(loop key or antispark), if the power to the VESC is solely from the motor, your VESC will be going through waves of brownouts yes. 

If your board is turned on and the VESC's are receiving power from the battery, the components will be run at proper operating voltages, and not be going through waves of voltage brownouts


@DK-Odense that would probably be the best/easiest solution, leaving the esc's powered with a disconnect switch for the PPM signal - just make sure you have your failsafe setup properly and i'd probably suggest unchecking limit erpm with negative torque for the front wheels...
```

---
## \#62 Posted by: Hummie Posted at: 2017-10-23T19:28:55.572Z Reads: 59

```
I understood from others before that riding without batteries is quick doom and the motor will power on the vesc and get overburdened with current and get damaged. And braking especially will do it. I've experienced suden braking when I'd ridden e no batteries.  But ur saying even with batteries connected brownouts could happen if board is off and this could damage. Know were going in circles here but I need a couple loops
```

---
## \#63 Posted by: Deckoz Posted at: 2017-10-23T19:35:40.564Z Reads: 61

```
Hummie 

If your considering "Braking" while the board is powered off, chaka has covered this

-If you have a loop key, you have a incomplete circuit, with the board powered off, braking currents would have no where to go, burn up is inevitable

-if you have a soft switch(mosfet antispark), with the board powered off, the circuit to the battery is still technically "complete" and braking currents have some where to go.

with either of those scenarios with the board powered OFF if you take braking OUT of the picture. The voltage being supplied to the VESC coming from the motor, will not be a constant voltage that can keep the VESC within operating voltages. In other words, unless you never stop and never go below x rpm to maintain X volts, your VESC will be going through waves of brownouts when power is supplied by motor/generator.

Does that make sense?
```

---
## \#64 Posted by: Hummie Posted at: 2017-10-23T19:53:23.901Z Reads: 60

```
Thanks yes.  
A bit different related question:  you mentioned the fet switch being able to complete a circuit and braking being possible even if board is off.  Right?  As apposed to a true broken circuit.  
+++ I rode around w batteries disconnected without braking and didn't ruin the vesc but hear I could've. I did have brakes slam on. Won't do I again but are u saying if had a fet switch, and powered off, I'd be OK coasting  or even braking if batteries connected?
```

---
## \#65 Posted by: Deckoz Posted at: 2017-10-23T20:31:31.245Z Reads: 60

```
Yes you'd be "fine" with regards to somewhere for the current to go. Still would have low speed brownouts, better off just turning the board on and leaving the remote turned off in your pocket.
```

---
## \#66 Posted by: psychotiller Posted at: 2017-10-23T21:24:20.456Z Reads: 56

```
That's exactly what I was saying. Fashionable to disagree then agree I guess...
```

---
