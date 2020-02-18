# Help around gear ratio

### Replies: 15 Views: 298

## \#1 Posted by: Itz Posted at: 2019-01-31T01:42:31.476Z Reads: 124

```
First of all, sorry if it's not in the right category.
So I've got a 35T to 13T gear ratio or whatever. 83mm wheels. 250-5M HTD5 12mm belts.
My 13t pulley broke(8mm bore, 12mm width), it can't stay too long on the axis, it just doesn't get bolted right to the axis- probably because it's a cheap one.
Which pulley do you recommend me to replace it with? I was thinking about a 12T. Do you know any high-quality motor pulleys so I could buy some and finally have no issues with those motor pulley falling off of a shaft?
```

---
## \#2 Posted by: AlexBE Posted at: 2019-01-31T01:46:52.770Z Reads: 117

```
If the teeth aren't broken, I would just loctite it on. What is making it fall off the axle?
```

---
## \#3 Posted by: Winfly Posted at: 2019-01-31T01:46:58.655Z Reads: 113

```
if you are in Europe, grab some steel motor pulleys from eskating.eu. 

otherwise, in the US, BKB has some 15T steel pulleys.

https://buildkitboards.com/collections/pulleys/products/15t-15mm-motor-pulley

also.

https:///

Question is, how much speed vs torque do you want? lower T on motor pulley = more torque, higher T  = more speed.

use this calculator to figure it out:
https://calc.3dservisas.eu/?Rc49D8IgEAbg_8LsQEFNdT2bTiYkTexuGTARIenY-N-9ew91e-7rhc3cKZmzeT7Ky-zMShMXnQUDcw8Ry1mr7YtWatnxauR0zCoZXkCY4q6GqcXVIEdOhCh_AKV5BH9BS6J2s6SB1VvwJmN8IFNLyvi2A0ORZg_-389UsMKM88o8STeO1_ZWHOevBp2-Pw==
```

---
## \#4 Posted by: Winfly Posted at: 2019-01-31T01:53:11.773Z Reads: 86

```
yeah also not sure how it is broken, you should also just try putting loctite on the grub screws
```

---
## \#5 Posted by: pixelsilva Posted at: 2019-01-31T06:12:05.377Z Reads: 71

```
Mannn, you are putting lots of stress on your motors and belts with a those 12T or 13T (few teeth count). You should start with minimum 15T or 16T motor pulley.
```

---
## \#6 Posted by: MysticalDork Posted at: 2019-01-31T06:18:28.581Z Reads: 70

```
@Itz  If it's "broken" because it's slipping, I'd guess you're using a soft setscrew against a hardened shaft with no flat spot. 
If that's the case, do three things: 1: grind a flat on the motor shaft where the setscrew will sit. 2: replace the chinese setscrew made out of cheese with a proper alloy steel one. 3: use loctite (242 or 243. medium strength.).

If that doesn't work, you can try using loctite 648 to hold the pulley to the shaft.

If you can find one, get steel rather than aluminum since it'll wear out less quickly.
```

---
## \#7 Posted by: Itz Posted at: 2019-01-31T13:46:08.742Z Reads: 56

```
Putting Loctite didn't do anything helpful. 
My shaft does have a flat spot and yes, I've got some Chinese ones.
@Winfly do you recommend exactly that combination of the pulley(15t)? What about 14t? And I can't put a 15mm wide pulley because the flat part of my shaft is 12mm wide. I'm planning to buy from eskating.eu, but can you put together a correct combination of those "customization options" for me? I would be very grateful.
I'm generally okay with this setup as of now but wouldn't change it too much in terms of torque or speed but if I had to, that's okay.
Edit; I have 2x270kv motors (the whole skateboard is from diyeboard.com)
```

---
## \#8 Posted by: Itz Posted at: 2019-01-31T16:49:32.116Z Reads: 47

```
Correction- I have a 36t pulley installed
```

---
## \#9 Posted by: Winfly Posted at: 2019-01-31T20:37:55.546Z Reads: 44

```
 Still don't understand how it's "broken". Did you not pin the screw on the flat spot with loctite?

Did a little search. Diyeboard motor shaft is 8mm, comes with 13T motor pulley and 12mm width. Stock 13:35 ratio at 10S 270kv 83mm wheel gives you up to about 40mph top speed, which you will never hit with these small motors.

Eskating.eu doesn't make 13T so you have to go either 12 or 14. This might change the tension on the belt so here's a belt calculator to figure out what's the optimal belt length.


So:
8mm bore
12mm width
12,14T
1 or 2 set screw
With or without overhang
```

---
## \#10 Posted by: Itz Posted at: 2019-01-31T21:01:26.689Z Reads: 40

```
It's "broken" in the way that I can't screw it to the shaft because the pulley's hole is worn out (can't think of a way to describe it to you better). Plus, the pulley is low quality and after some time it just loses traction(screw falls of) even with loctite. I pin the screw to the flat spot of the shaft AND to the opposite side too.
I have the old type of their "package" where I have a 36T and 12t. I actually hit 42-43km/h on a full charged battery for approx first 5min of riding then the speed falls off.
```

---
## \#11 Posted by: murloc992 Posted at: 2019-01-31T21:15:00.373Z Reads: 37

```
[quote="MysticalDork, post:6, topic:82643"]
chinese setscrew made out of cheese
[/quote]

Hey, at least it's not made out of tofu. :joy:
```

---
## \#12 Posted by: murloc992 Posted at: 2019-01-31T21:16:32.719Z Reads: 35

```
[quote="Itz, post:10, topic:82643"]
Plus, the pulley is low quality and after some time it just loses traction(screw falls of) even with loctite.
[/quote]

Use red loctite between the shaft and the pulley and blue/purple on the screws.. Let them sit nicely in place for 24 hours. Then after some time just create a post about how you can't take the pulley off the motor shaft. :slight_smile:

I had a pulley stuck on my motor shaft so well with red loctite before, only way I could remove it was a induction heater and a puller. Good times.
```

---
## \#13 Posted by: Winfly Posted at: 2019-01-31T22:12:09.756Z Reads: 33

```
If the set screw hole is stripped there's nothing you can do. Also, blue loctite on the screw is more than enough imo. If you wants it to hold better, I recommend drilling a divot onto the shaft to let the screw dig deeper.
```

---
## \#14 Posted by: AlexBE Posted at: 2019-02-01T02:58:49.193Z Reads: 32

```
I agree with this. If you use red loctite, you don't even need a setscrew.
```

---
## \#15 Posted by: Itz Posted at: 2019-02-02T01:38:46.610Z Reads: 22

```
Well guys, thank you very much for your help! :innocent:
```

---
