# Vesc Capacitor Replacement

### Replies: 22 Views: 546

## \#1 Posted by: AlanZhou Posted at: 2019-01-17T21:33:43.715Z Reads: 68

```
Hey was just woundering if i could replace my TB caps with one big cap eaualivent to the 3 small capacitor?

I'm trying to save space for a mini build and I know that the original vesc design used one big cap. If I can links, anyone😅

![IMG_20190117_162755|666x500](upload://7C8x1klA0CxDEtuqjlAPzB6WVOx.jpeg)

@torqueboards
@b264
```

---
## \#2 Posted by: b264 Posted at: 2019-01-17T21:36:33.125Z Reads: 61

```
You can peruse digikey and find one that's ***at least*** 63V and ***approximately*** 2mF

The three 680μF are 2.04mF in parallel like that.
```

---
## \#3 Posted by: AlanZhou Posted at: 2019-01-17T21:37:21.727Z Reads: 59

```
Was gonna tag you but i was scared... Also is these a certin kind of cap to look for? any name brands?
```

---
## \#4 Posted by: Indiangummy Posted at: 2019-01-17T21:41:02.367Z Reads: 55

```
i think your going to have a hard time finding a capacitor rated for 2.04mF and 63V.
Also @b264 what's the tolerance on these 10%?
```

---
## \#5 Posted by: AlanZhou Posted at: 2019-01-17T21:41:33.751Z Reads: 53

```
I was thinking maybe going for more uf as there more common

Will this work?: https://www.amazon.com/gp/product/B0188FWIFS/ref=oh_aui_detailpage_o00_s00?ie=UTF8&psc=1
```

---
## \#6 Posted by: b264 Posted at: 2019-01-17T21:43:03.680Z Reads: 51

```
[quote="Indiangummy, post:4, topic:81221"]
what’s the tolerance on these 10%?
[/quote]

Typically, yes.  5% or 10%

Some are like -5% +25%
```

---
## \#7 Posted by: b264 Posted at: 2019-01-17T21:45:25.521Z Reads: 50

```
6800μF / 6.8mF  63V will work fine if you use a loopkey.  If you use an antispark switch without a separate precharge resistor, you will [roast your antispark](https://www.electric-skateboard.builders/t/vedder-antispark-design-problem-or-implementation-problem/77967/4?u=b264).

You might want to put an additional 10μF 63V in parallel with that 6.8mF capacitor.
```

---
## \#8 Posted by: AlanZhou Posted at: 2019-01-17T21:46:59.653Z Reads: 48

```
hehe already roasted 2 antisparks and dont know why.

these maybe or can you recommend one?

https://www.ebay.com/itm/63V-2200uF-63Volt-2200MFD-Electrolytic-Capacitor-18mm-35mm-/253978272710?_trksid=p2385738.m4383.l4275.c10&var=553302392014
```

---
## \#9 Posted by: b264 Posted at: 2019-01-17T21:47:54.942Z Reads: 47

```
That one would work if it's not fake.  For $1.29, it's probably fake.

Just use digikey or mouser
```

---
## \#10 Posted by: b264 Posted at: 2019-01-17T21:49:06.854Z Reads: 46

```
[quote="AlanZhou, post:8, topic:81221"]
already roasted 2 antisparks and dont know why.
[/quote]

If you follow my link, you will learn why
```

---
## \#11 Posted by: AlanZhou Posted at: 2019-01-17T21:49:47.513Z Reads: 39

```
Easy enough. its 20% and 2200uf dont know what the 20% means though
https://www.digikey.com/product-detail/en/nichicon/UVR1J222MHD/493-1130-ND/588871

and you mentioned something about a mcu, thats what multiple vendors told me too, without one all antisparks will have the same fate.
```

---
## \#12 Posted by: b264 Posted at: 2019-01-17T21:54:43.499Z Reads: 37

```
Sure.  You might want to put an additional 10μF 63V in parallel with that.

[quote="AlanZhou, post:11, topic:81221"]
and you mentioned something about a mcu, thats what multiple vendors told me too, without one all antisparks will have the same fate.
[/quote]

That's a question for the other thread
```

---
## \#13 Posted by: AlanZhou Posted at: 2019-01-17T21:56:51.652Z Reads: 30

```
[quote="b264, post:12, topic:81221"]
10μF 63V in parallel with that.
[/quote]

why? also whats a safe company for caps, Nichicon, rubycon? also i should get a cap that last a long time in terms of hours?
```

---
## \#14 Posted by: b264 Posted at: 2019-01-17T21:58:08.790Z Reads: 28

```
Capacitors are pretty low-tech, not sure any is better than the other.  I'm sure the more you spend, you will probably get better stuff.
```

---
## \#15 Posted by: Indiangummy Posted at: 2019-01-17T21:58:13.535Z Reads: 29

```
[quote="AlanZhou, post:11, topic:81221"]
what the 20% means though
[/quote]

the 20% means the Farad rating can be of by +or- 20%
```

---
## \#16 Posted by: AlanZhou Posted at: 2019-01-17T21:59:44.819Z Reads: 28

```
hehe lol i feel stupid now. why 10μF 63V in parallel with that though?
```

---
## \#17 Posted by: b264 Posted at: 2019-01-17T22:01:19.717Z Reads: 28

```
The frequency response of capacitors is highly dependant on the capacitance and the 10μF will smooth out high-frequency ripples that the larger one may be quick enough to smooth over.  Increasing from 680μF to 6.8mF means you've lost some of the high-speed response, so that gets it back.
```

---
## \#18 Posted by: AlanZhou Posted at: 2019-01-17T22:02:47.211Z Reads: 28

```
im not going with the 6.8mf cap anymore im going with a 63v 2.2mf cap which sould be the same rating as vedder used
```

---
## \#19 Posted by: b264 Posted at: 2019-01-17T22:04:56.717Z Reads: 28

```
The 10μF won't hurt even so you are decreasing the response slightly with one big versus 3 smaller ones.  But not as much as if you went to a single 6.8mF
```

---
## \#20 Posted by: AlanZhou Posted at: 2019-01-17T22:05:43.548Z Reads: 29

```
i cant fit it in my small build lol. im tight for space and ive settled on rubycon
```

---
## \#21 Posted by: b264 Posted at: 2019-01-17T22:06:38.174Z Reads: 29

```
The 10μF is slightly bigger than a rice grain.  You can certainly omit it.  It's advice, you don't need to heed it.  It's also not a terribly important piece.
```

---
## \#22 Posted by: AlanZhou Posted at: 2019-01-17T22:08:47.444Z Reads: 29

```
alright gonna do it than but im gonna need to find a way to connect the caps

and thanks for the help @b264 @Indiangummy
```

---
