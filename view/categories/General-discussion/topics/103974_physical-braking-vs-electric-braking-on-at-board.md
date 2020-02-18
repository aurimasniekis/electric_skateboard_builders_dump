# Physical braking vs electric braking on AT board

### Replies: 14 Views: 277

## \#1 Posted by: mjaffee Posted at: 2019-11-18T05:32:27.617Z Reads: 88

```
Hi all, 

I'm going on my second build and thinking of building an AT board with both physical disk brakes and electronic braking. I live in San Francisco where electric braking on the steep hills can kill your range, or cause overheating / extra wear issues (larger tires to get over the potholes would also be nice).

For those riders that are running both, do the physical brakes significantly extend your range and/or reduce motor / component wear?  How often / what's your preferred method of braking? Thx
```

---
## \#2 Posted by: telnoi Posted at: 2019-11-18T05:35:30.544Z Reads: 86

```
Actually physical brakes kill range. No regen and it makes the board heavier.
```

---
## \#3 Posted by: Benjo Posted at: 2019-11-18T06:25:48.492Z Reads: 82

```
How does regen braking cause wear or kill the range? As the name suggests it regenerates energy, especially in areas with a lot of hills that can significantly increase your range. I am also not aware that this puts any strain on the motor whatsoever. All that wears over time in a brushless motor is the bearings and they shouldn't care about braking.

Also with physical brakes you need to hold an additional thingy in your hand and have an extra cable.

Edit: From a safety standpoint brakes are obviously a good idea. If something runs too hot, regen braking will be reduced, also if you say you live in a hilly area you need to make sure that you start with a battery that isn't fully charged or with a part of the trip that has a long incline. Otherwise your battery may be full once you try to brake and regen braking will shut off to prevent overcharging the batteries.
```

---
## \#4 Posted by: venom121212 Posted at: 2019-11-18T13:54:01.225Z Reads: 63

```
All of this with the caveat:

You can still electric brake on a full battery if you wire a rheostatic brake in parallel with your battery.
```

---
## \#5 Posted by: mjaffee Posted at: 2019-11-18T16:17:46.792Z Reads: 54

```
i guess that i should be clear that physical brakes would only be used when braking is absolutely necessary. My thought is that if it takes energy to e-brake, range could be extended. Regen and braking hard on these hills is pretty much a net zero range increase game. 

The vesc heats up as Its used and when it regens more energy than what you program it to recover. The motor heats up as its used. If heat reduces component lifetime and reduces efficiency physical brakes could help share the burden.
```

---
## \#6 Posted by: Balta_6 Posted at: 2019-11-18T17:03:07.360Z Reads: 49

```
[quote="mjaffee, post:5, topic:103974"]
is that if it takes energy to e-brake
[/quote]

but it doesn't

With the universal conservation of energy, because you are breaking, you're losing energy, but it need to be transformed somewhere

With regular brakes it's with heat, and with regenerative breaking, the motor acts like a dynamo and transfer the energy back to the battery
Obviously it's not a 100% efficiency, but it does make a significant differences for your range (more range)

I used to live on top of my city (in the swiss alp), I could ride 5km and arrive at the bottom with still a full battery (on a mellow drive : it has a resistor to dissipate excess energy)
```

---
## \#7 Posted by: Benjo Posted at: 2019-11-18T18:27:55.880Z Reads: 43

```
Me and Balta_6 already said it, but again: Regen braking (or e-braking if you want to) doesn't consume power from the battery, it puts power into the battery! That's why it is called regenerative braking! It regenerates energy by using the motor as a generator. And this really is not a problem at all for neither the motor nor the VESC.
```

---
## \#8 Posted by: venom121212 Posted at: 2019-11-18T23:03:53.404Z Reads: 40

```
Regenerative braking: Your motor working backwards as a generator to recharge or *regenerate* your battery.
```

---
## \#9 Posted by: mjaffee Posted at: 2019-11-20T19:16:18.667Z Reads: 32

```
I understand the principle of regenerative braking as you all are saying. I'm willing to bet that a lot of us don't understand exactly how it works tho. There's something called torque blending which implies that at low speeds, the motor doesn't generate enough braking torque to effectively brake...usually a friction brake is used to finish braking. I'm wondering if braking at slow speeds and/or at low speed warrants the need for a physical brake. This is done all the time in larger electric vehicles. I don't see why vesc wouldn't have the same issues. From a report online "At lower speeds, relatively little current is being produced by the generator to ensure desirable battery charge efficiencies. Therefore at these speeds, the friction brakes are applied to decrease electrical cycling through the generator and batteries. It has been implied in literature that the life of the electrical system, especially the batteries, is adversely effected by this micro-cycling process where the battery pack is subjected to short-term charge and discharge cycles, thereby reducing life and efficiency". Life and efficiency, in addition to battery wear might explain why I feel like i'm getting less range out of regen in the long run. 

All of this is just thinking tho. I don't have any data to back this stuff up...capturing telemetry from my board and long term range / batt condition info seems like something I should have done a long time ago.
```

---
## \#10 Posted by: Sn4pz Posted at: 2019-11-20T19:45:04.469Z Reads: 27

```
And I thought I had ordered everything for my vanguard :roll_eyes: :laughing:

Time to see if it'll even fit in my ESC enclosure 🤔
```

---
## \#11 Posted by: BluPenguin Posted at: 2019-11-20T20:12:07.893Z Reads: 23

```
As far as I understand, low speed braking in vesc is done by essentially shorting out the motors once regen voltage is too low to be effective, creating a strong low speed brake. Energy is dissipated as heat by the motors and esc. I would assume that if a lot of low speed, high torque braking is done on the board, a mechanical brake would drastically offset heat in the motor and esc, probably extending the life of the fets etc too.
```

---
## \#12 Posted by: mjaffee Posted at: 2019-11-20T20:38:12.227Z Reads: 21

```
Got it, that may also be why my DRV fried a few months ago while going down a steep hill at slow speed (probably put the nail in the coffin for an already worn component). Makes sense now that I know how it works.
```

---
## \#13 Posted by: Benjo Posted at: 2019-11-20T21:02:30.565Z Reads: 20

```
As far as I understood it till now the shorting of phase wires is only done to serve as an electronic handbrake at a standstill or near standstill, not at any speed you would normally travel at. So just a very brief moment in the end. Not much heat to be dissipated there.
But I could be mistaken.
```

---
## \#14 Posted by: boards Posted at: 2019-11-20T23:47:59.264Z Reads: 17

```
I live in SF. Dual motors will slow you down even the steepest hills in my experience.
```

---
