# Upgrading to Dual Drive Advice/Help

### Replies: 9 Views: 306

## \#1 Posted by: UKRider Posted at: 2018-09-02T14:33:02.646Z Reads: 134

```
I'm ready to make some upgrades but some advice is needed from all you experts.

**Existing build:**
90mm Clones, 6S Lipo (2 X Turnigy 3S 5000mah 30-40c), 5065 Motor 270KV, Hobbyking SK8 Vesc 4.12, 12T Motor Pulley 36T Wheel Pulley, 10mm 265 Belt 5M, I weigh 95KG.

**How it rides:**
With the existing setup I get up to a max of 20mph and gives me a range of 5.7 miles riding on a mix of flats and gentle hills.

**Why I'm upgrading:**
I want a better range about 10 miles. I experience some belt slippage due to weight and torque/braking I need to eliminate this as much as possible. Maybe some more speed:wink:

**What I'm considering:**
Another 5065 270KV Motor
2 More Batteries which I will wire in parallel so instead of 6S I will have 6S2P (10000mah)
15mm wide belts and moving up from 12T to 15T on the motor pulley.
Better mounts maybe with idlers.

**Questions/ Concerns:**
With the extra batteries I'm hoping my range will increase to near 10 miles BUT having having that extra motor will the voltage be reduced from 25 volts to half?  I guess this is to do with wiring. Do I run a parallel connection from battery to the additional VESC? Will this keep same voltage across both vescs?

The change in pulley from 12T to 15T will according to the calculators give me more too end, but will it have a massive difference with low speed torque or will the extra motor compensate.

Comments and recommendations?
```

---
## \#2 Posted by: mmaner Posted at: 2018-09-02T14:37:38.337Z Reads: 121

```
Adding a 2nd motor will effectively double available torque. Your batteries won't fully support it but you will see a bug difference. 

Moving to15mm belts will reduce slippage, just make sure you get your belt tension correctly, maybe consider idlers. 

I don't know if I'd move to 15t motor pulleys on 6s, you may gain some top end but loose so much bottom end as to make it unusuable. I would just experiment and see how it performs.
```

---
## \#3 Posted by: UKRider Posted at: 2018-09-02T14:49:10.193Z Reads: 106

```
Would not wiring a parallel connection from the battery to each Vesc still provide 25 volts? In essence both motors will have the same voltage as before??
```

---
## \#4 Posted by: mynamesmatt Posted at: 2018-09-02T21:21:35.827Z Reads: 66

```
yes when both vescs are in parallel they receive the same voltage. the current is what is spread evenly across them
```

---
## \#5 Posted by: UKRider Posted at: 2018-09-02T22:17:11.308Z Reads: 57

```
So that means that same rpm as before due to the same voltage.  If the current is shared then I guess it would be equal torque over the motors just what I want.

Not sure if the range would double due to extra belt and drag and general efficiency.
```

---
## \#6 Posted by: UKRider Posted at: 2018-09-03T20:56:45.966Z Reads: 39

```
Hmmm, anybody else who can comment on keeping 6S setup with dual motors and possible change to a 15 teeth motor pulley?
```

---
## \#7 Posted by: Acido Posted at: 2018-09-03T21:35:19.894Z Reads: 30

```
Yould you fit another 6s battery inside?
```

---
## \#8 Posted by: UKRider Posted at: 2018-09-03T21:54:27.260Z Reads: 29

```
I was thinking 6S2P, is that what you mean? I could fit that in.
```

---
## \#9 Posted by: Namasaki Posted at: 2018-09-04T03:08:45.563Z Reads: 19

```
if you add 2 more 3s packs and wire them all in series for 12s/5000 it would give you more available power and speed and would also increase range.

6s/10000mah or 12s/5000mah will theoretically  yield the same range.

But higher voltage will yield more power and speed.
However, 12s might be too high for the HK Vescs. I don't know what components they use.
You could either upgrade to Focbox's or you could try just adding one more 3s in series for 9s.
I can get 12 miles with 10s/5000 so 9s would probably get you close to 10 miles.
Adding a second motor is always a good idea.
Better torque as @mmaner mentioned  and also greatly improve braking.
```

---
