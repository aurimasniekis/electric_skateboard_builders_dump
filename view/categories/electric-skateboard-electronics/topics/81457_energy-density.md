# Energy density?

### Replies: 40 Views: 403

## \#1 Posted by: ZachTetra Posted at: 2019-01-20T00:36:43.803Z Reads: 158

```
I'm deciding between using lipo and li-ion for my new board... according to the numbers, lipo has 5x the volumetric energy density but li-ion has 1.5x the gravametric energy density...does that sound right you you guys?
```

---
## \#2 Posted by: brenternet Posted at: 2019-01-20T00:39:45.169Z Reads: 159

```
I would suggest using the search function as this topic has been beaten to death here a thousand times. Which will likely happen again right below my post.

There's loads of info out already.
```

---
## \#3 Posted by: Hummie Posted at: 2019-01-20T01:20:12.816Z Reads: 144

```
5x or 1.5x what?  lipo are much less energy dense than ion but you need a level of power too and you cant just get the most energy dense cells as they're only good for maybe a couple of amps power.
```

---
## \#4 Posted by: AlexBE Posted at: 2019-01-20T02:30:38.824Z Reads: 131

```
It sounds like you are already analysing the problem in the right way. For us to help you make a decision you also need to explain your 
* budget
* range requirement
* power requirement
* assembly ability

In general, Lipo are
* cheap
* powerful
* large (for the capacity, as you point out in your post)
* easy to assemble into skate packs as you don't need to weld them together.

In general 18650 Li-ion are
* more expensive per Wh and per W
* better energy density (weight and volume)
* lower power density
* highly configurable. Any combination of 10s4p, 12s5p, 8s10p etc.(but requires welding)
```

---
## \#5 Posted by: ZachTetra Posted at: 2019-01-20T02:46:21.292Z Reads: 114

```
I'm making a dropdeck longboard that pulls 40A continuous and 130A burst (based on motors) and I'm hoping for about 400Wh.  I'm debating between...
- a custom 12s2p 10Ah 12/24C Turnigy lipo pack
- a 12s4p 12Ah Samsung 30Q li-ion pack

I want to make the packs in 4 parts (2s2p unit on the board) because I can only charge a 6s at a time and I want to make the extra parallel cells optional for less weight and lower speed when I'm on campus.
```

---
## \#6 Posted by: J_Dizzle Posted at: 2019-01-20T02:54:07.895Z Reads: 109

```
That’s a little ridiculous, if you want to go slower buy a BT module and configure speed modes
```

---
## \#7 Posted by: ZachTetra Posted at: 2019-01-20T03:05:11.922Z Reads: 107

```
I'm not gonna pull out the batteries to go slow, I'm just going to have less amps available so I'll get less acceleration and save a kilo of battery weight, since I don't have much space to accelerate on a campus it will effectively be slower since I'll never get to top speed...but I'm not sure if there is a way to not blow the batteries by having the ESC set to the higher amp limit
```

---
## \#8 Posted by: AlanZhou Posted at: 2019-01-20T03:18:54.790Z Reads: 102

```
@psychotiller

get a 12s4p from this guy, he knows how to build a pack :grinning:
```

---
## \#9 Posted by: Hummie Posted at: 2019-01-20T03:21:49.175Z Reads: 99

```


Those lipo are unlikely to really have that c rating or discharge rating and likely half what’s stated.  


Lipo are easy though
```

---
## \#10 Posted by: AlanZhou Posted at: 2019-01-20T03:28:59.060Z Reads: 93

```
Until you make a mistake, right hummie?:sob:
```

---
## \#11 Posted by: Hummie Posted at: 2019-01-20T03:30:47.753Z Reads: 94

```
Well lipo are pretty easy not to make a mistake!   But do need protecting.  Maybe that’s my constant mistake ur alluding to.
```

---
## \#12 Posted by: AlanZhou Posted at: 2019-01-20T03:31:27.497Z Reads: 88

```
hmmmmmmmmmmmmmmmmmmmmmmmmmmmmm. youve got me thinking :rofl:
```

---
## \#13 Posted by: ZachTetra Posted at: 2019-01-20T03:32:57.025Z Reads: 89

```
I've nearly burned my house down with a 2s lipo so maybe I should stay away from Lipos...the scortch marks on my carpet attest to my incompetence
```

---
## \#14 Posted by: Hummie Posted at: 2019-01-20T03:34:13.617Z Reads: 87

```
How did u?
```

---
## \#15 Posted by: ZachTetra Posted at: 2019-01-20T03:35:16.455Z Reads: 87

```
Long story short I was making an analog robot and I crossed the leads...the wires melted into the carpet
```

---
## \#16 Posted by: AlanZhou Posted at: 2019-01-20T03:36:15.494Z Reads: 88

```
your somewhat lucky the leads didnt weld together for a few seconds.
```

---
## \#17 Posted by: ZachTetra Posted at: 2019-01-20T03:55:01.596Z Reads: 87

```
![image|666x500](upload://kOvEXFvpj4hj80NepqBPetQyXl.jpeg) ![image|666x500](upload://cXucwgvpNOEaoNti7uOTQ2B7sgZ.jpeg) ![image|375x500](upload://njFJv1CbdSGiP2hOxmJDN9jSJZe.jpeg) 

That spot is in my doorway so I walk over it dozens of times a day for years now, this is way more difficult to make than any electric skateboard BTW
```

---
## \#18 Posted by: janpom Posted at: 2019-01-20T04:30:16.430Z Reads: 82

```
It's a common misconception that LiPo are more dangerous than li-ion. They are both dangerous. LiPo are easier to use and thus used by people who don't know what they are doing more often and thus more accidents happen with LiPos. That doesn't yet make them more dangerous.
```

---
## \#19 Posted by: ZachTetra Posted at: 2019-01-20T04:33:17.618Z Reads: 84

```
I used to think that for a long time, but it is easier to puncture a lipo than a li-ion so its still kinda true
```

---
## \#20 Posted by: TowerCrisis Posted at: 2019-01-20T04:37:56.849Z Reads: 83

```
Well, lipos are designed to be placed into a hard shell. Using them without one is, IMO, foolish.

See the graphene lipo series. They've all got a hard shell around them, I'd say they're pretty safe.
```

---
## \#21 Posted by: ZachTetra Posted at: 2019-01-20T04:42:00.242Z Reads: 79

```
I'm probably putting 24 cells under a board with 34'' from wheel to wheel and an average clearance of under 3" so I'm kinda worried, do you think a thin fiberglass enclosure with standoffs in the middle is enough?  I doubt puncture risk is high but I can put 1/32" galvanized steel plates in if need be
```

---
## \#22 Posted by: TowerCrisis Posted at: 2019-01-20T04:47:29.585Z Reads: 77

```
I'd recommend using lipos (if you use lipos) that already come in a plastic case. That in combination with your enclosure should be more than enough protection.

If you use bare lipos, I would suggest using adhesive tape and permanently mounting them onto a hard plate that you can put "road side" inside your enclosure.

I wouldn't use a metal plate for that, you don't want metal near your high power electronics.

 1/16th polycarbonate would be great though. That's what I did for my first build and it worked pretty well. The cells stayed safe.
```

---
## \#23 Posted by: ZachTetra Posted at: 2019-01-20T04:49:49.724Z Reads: 77

```
Should I tape the batteries to the underside of the deck and the plates to the batteries with a gap between the plates and enclosure?  I can space it with squishy foam or conform the enclosure to hug each cell
```

---
## \#24 Posted by: TowerCrisis Posted at: 2019-01-20T05:09:47.186Z Reads: 70

```
Ah I can't seem to find the thread, but there was a very relevant discussion recently about whether you should mount to the deck or to the enclosure... Anyone else care to chime in?
```

---
## \#25 Posted by: AlanZhou Posted at: 2019-01-20T05:13:41.423Z Reads: 70

```
Depends on preference. its almost 50/50 now
```

---
## \#26 Posted by: AlexBE Posted at: 2019-01-20T07:32:03.044Z Reads: 66

```
If I had to guess, you misunderstand battery current vs motor current. What calculation gives you 40A cont and 130A burst?
```

---
## \#27 Posted by: ZachTetra Posted at: 2019-01-20T13:28:58.473Z Reads: 62

```
The motors are rated for 65A each and maintaining speed on hills is 1.75kW based on bike calculators which would be 40A at 12s
```

---
## \#28 Posted by: AlanZhou Posted at: 2019-01-20T14:38:14.177Z Reads: 59

```
Just so you know batt current and motor current are different.
```

---
## \#29 Posted by: Hummie Posted at: 2019-01-20T19:10:35.460Z Reads: 51

```
ratings are bogus.  if you ride in the arctic you'll be able to stay cool and produce more power.   worth knowing what temp the magnets in the motor can get to.
```

---
## \#30 Posted by: Deodand Posted at: 2019-01-20T19:24:01.660Z Reads: 49

```
[quote="ZachTetra, post:17, topic:81457"]
this is way more difficult to make than any electric skateboard BTW
[/quote]

Try riding 1000 miles on a board with the build quality of that robot, it will break. A skateboard may be mechanically simpler but the stresses and environment it is subjected to are much harsher. This is what makes it a very challenging problem if you want to build a board you aren't constantly having to repair. 

I'm a robotics PhD student and I also started out underestimating the complexity of the problem.
```

---
## \#31 Posted by: b264 Posted at: 2019-01-20T19:24:05.110Z Reads: 45

```
[quote="ZachTetra, post:17, topic:81457"]
this is way more difficult to make than any electric skateboard BTW
[/quote]

Sure, but it's way more difficult to make an electric skateboard last.  This thing would break in 30 seconds under the vibrations that electric skateboards have to endure their entire existence.
```

---
## \#32 Posted by: ZachTetra Posted at: 2019-01-20T20:21:16.015Z Reads: 44

```
I mean that thing wasn't meant to go 1000 miles so we never tried making it that robust

It's more of an exercise in dynamics than material science and kinetics
```

---
## \#33 Posted by: b264 Posted at: 2019-01-20T20:46:00.947Z Reads: 42

```
Well when you say "difficult to make" you act like it's easy to make an esk8.  It's really easy to make one that goes 1km.  Make one go 2000km, I dare you.  Including water and snow.  I bet you can't do it.
```

---
## \#34 Posted by: ZachTetra Posted at: 2019-01-20T20:57:27.145Z Reads: 41

```
I know I can't, and I suck a sarcasm :man_shrugging: I thought it would be fun to share a story of fire and stupidity
```

---
## \#35 Posted by: b264 Posted at: 2019-01-20T21:00:43.589Z Reads: 39

```
LoL and I thought the thing you'd say is why am I using metric incorrectly :rofl:

It's 2Mm, not 2000km
```

---
## \#36 Posted by: ZachTetra Posted at: 2019-01-20T21:12:56.696Z Reads: 36

```
The full name is 2*10^6m excuse you
```

---
## \#37 Posted by: b264 Posted at: 2019-01-20T21:14:40.775Z Reads: 34

```
That's 2E6m where I'm from
```

---
## \#38 Posted by: ZachTetra Posted at: 2019-01-20T21:16:39.954Z Reads: 35

```
Oof, what kind of calculator display heresy is this
```

---
## \#39 Posted by: dareno Posted at: 2019-01-20T21:45:41.472Z Reads: 37

```
[quote="ZachTetra, post:36, topic:81457, full:true"]
The full name is 2*10^6m excuse you
[/quote]

[quote="b264, post:37, topic:81457, full:true"]
That’s 2E6m where I’m from
[/quote]
Were you two seperated at birth?
```

---
## \#40 Posted by: Hummie Posted at: 2019-01-20T21:58:12.405Z Reads: 33

```
Is there a prize for the most confrontational member?
Mr @b264 I’m thinking you’d win!
```

---
