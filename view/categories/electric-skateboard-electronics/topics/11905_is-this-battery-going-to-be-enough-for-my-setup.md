# Is this battery going to be enough for my setup?

### Replies: 16 Views: 1033

## \#1 Posted by: AbdeTy Posted at: 2016-10-26T00:57:01.352Z Reads: 110

```
Hi guys, i am putting the plans for building my battery pack from 18650 cell and i am a bet confused about the amp draw they can support, i am planning on doing a 10s4p from 4 types of batteries that are recycled from laptop batteries, i tested them over and over again( capacity, discharge , charge, internal resistance)  so they are all good cells with capacity from 2000 to 3400 mah, so after reading a bet this is what i got as results , if i choose 2.5 Ah as a nominal capacity for each cell, the total capacity of the battery will be 2.5*4=10 Ah and since these cells only have a 2C rating that means the maximum continuous current will be 10*2=20 Amps, is that correct ? and if so is that going to be enough to power my set up ? btw i am using a vesc and an Sk3 6374 , thanks in advance guys
```

---
## \#2 Posted by: Jinra Posted at: 2016-10-26T01:28:49.996Z Reads: 102

```
Laptop batteries aren't feasible due to their low discharge rate. Having a 2C rating at 2500mah leaves you with 5A discharge, times 4 cells in parallel = 20A as you said. That's probably what you'll draw going 20mph on flats, but is not good enough for any hills, faster acceleration, or anything that will require torque. You'll easily burn out the pack at this discharge rate.

You generally want to give yourself as much buffer room as possible between the max rated discharge rate and your actual discharge rate. I run 80A discharge minimum on my boards. A 10s4p Samsung 25R pack will give you just that.
```

---
## \#3 Posted by: AbdeTy Posted at: 2016-10-26T09:16:22.277Z Reads: 77

```
thanks bro , i see now, do you think its worth it to add more cell in parallel , maybe a 6s6p configuration , but then i will give up voltage again, we now the more voltage the better it is for the system , at the moment i can't afford to buy new cells this is my first build and i have already spent 600$ so i guess i will just give it a go and see how it works
```

---
## \#4 Posted by: Aborn Posted at: 2016-10-26T11:20:54.354Z Reads: 68

```
Lowering the voltage will cause a higher amp draw, just go with your 10S4P and set the max amp in the VESC to 20 Amps so you dont damage them, and you will just have to deal with only going 20 mph for now.
```

---
## \#5 Posted by: mountainboardlover69 Posted at: 2016-10-26T11:49:27.418Z Reads: 60

```
go to a car dealer  and get a 20 amp fuse so u dont blow ur  battery but just the fuse get e few
```

---
## \#6 Posted by: AbdeTy Posted at: 2016-10-26T12:05:15.912Z Reads: 56

```
yes thats what i am planing to do for now, i also read that the vesc can output more amps than what it gets from the battery is that true ? i guess something to do with converting voltage to amps or something
```

---
## \#7 Posted by: AbdeTy Posted at: 2016-10-26T12:07:11.826Z Reads: 55

```
yes i will do that, i already got a 60 amps circuit breaker but its useless now , i thought that if i had a pack of 30 cells it will handle up to 60 amps but i was wrong lol, you can never learn enugh lol
```

---
## \#8 Posted by: mountainboardlover69 Posted at: 2016-10-26T12:21:13.851Z Reads: 51

```
that is true especially lipos the are confusing
```

---
## \#9 Posted by: AbdeTy Posted at: 2016-10-26T12:38:01.836Z Reads: 50

```
well these are Li ion but i guess its the same rule for all kinds of batteries
```

---
## \#10 Posted by: Aborn Posted at: 2016-10-26T12:40:25.058Z Reads: 47

```
Lipo = Lithium ion polymer, 
they're just flat li-ion cells. Exect same chemistry.
```

---
## \#11 Posted by: AbdeTy Posted at: 2016-10-26T12:52:09.095Z Reads: 44

```
yeah i know they are close but they are some differences between them i guess
```

---
## \#12 Posted by: Aborn Posted at: 2016-10-26T12:53:17.049Z Reads: 43

```
Well no?, except the lipo that you usually buy are for hobby race cars and stuff, and they are therefor made for high discharge current, but it's still the same chemistry.
```

---
## \#13 Posted by: DeathCookies Posted at: 2016-10-26T13:00:44.769Z Reads: 46

```

[quote="Aborn, post:10, topic:11905, full:true"]
Lipo = Lithium ion polymer, they're just flat li-ion cells. Exect same chemistry.
[/quote]

Well not really.
LiPo = Lithium Polymer
LiIon = Lithium Ion

Different chemistry, different formfactor.
[quote="Aborn, post:12, topic:11905"]
except the lipo that you usually buy are for hobby race cars and stuff, and they are therefor made for high discharge current,
[/quote]

Kinda...
LiPo have a better energy density and a lot higher discharge rate.
The only problem with lipos is the safety. They can easily burn, revive harder and does not have as much charge cycles as LiIon ;)
```

---
## \#14 Posted by: Aborn Posted at: 2016-10-26T13:03:57.595Z Reads: 45

```
Im bringing in Wikipedia to support my arguments.!

A lithium polymer battery, or more correctly lithium-ion polymer battery (abbreviated variously as LiPo, LIP, Li-poly and others), is a rechargeable battery of lithium-ion technology in a pouch format. Unlike cylindrical and prismatic cells, LiPos come in a soft package or pouch, which makes them lighter but also less rigid.

The designation "lithium polymer" has caused confusion among battery users because it can be interpreted in two ways. Originally, "lithium polymer" represented a developing technology using a polymer electrolyte instead of the more common liquid electrolyte. The result is a "plastic" cell, which theoretically could be thin, flexible, and manufactured in different shapes, without risk of electrolyte leakage. The technology has not been fully developed and commercialized[1][2] and research is ongoing.[3][4][5]

The second meaning appeared after some manufacturers applied the "polymer" designation to **lithium-ion cells contained in a non-rigid pouch format. This is currently the most popular use, in which "polymer" refers more to a "polymer casing" (that is, the soft, external container) rather than a "polymer electrolyte".** While the design is usually flat, and lightweight, it is not truly a polymer cell, since the electrolyte is still in liquid form, although it may be "plasticized" or "gelled" through a polymer additive.[6] These cells are sometimes designated as "LiPo"; however, from a technological point of view, they are the same as the ones marketed simply as "Li-ion", since the underlying electrochemistry is the same.[6]
```

---
## \#15 Posted by: Jinra Posted at: 2016-10-26T13:13:31.107Z Reads: 45

```
liion actually has better energy density per pound
```

---
## \#16 Posted by: mountainboardlover69 Posted at: 2016-10-26T19:48:52.631Z Reads: 36

```
Nobody cares about safety right
```

---
