# Heat Sink Foam?

### Replies: 21 Views: 3677

## \#1 Posted by: Raf Posted at: 2016-08-03T15:51:28.042Z Reads: 191

```
Hey guys,

Whilst doing some research i thought of an idea to help release some of the heat from components in case they overheat. I know you can get aluminium heat sink but i was wondering how well does heat sink foam work?

I was thinking you could maybe put it under the vesc and other parts inside the enclosure. Does anyone know if this would work? here are some i found online....

http://www.geek.com/wp-content/uploads/2014/07/copper_foam.jpg

http://core0.staticworld.net/images/article/2014/07/silent-power-100364905-orig.png

It is copper wires coiled together to make a foam block. I was thinking of maybe having a anti-vibration foam with this on top and the the electrical components on top of that.
```

---
## \#2 Posted by: Hummie Posted at: 2016-08-03T15:57:32.085Z Reads: 181

```
Zoinks.  Looks like a lot of shorting potential.
```

---
## \#3 Posted by: sl33py Posted at: 2016-08-03T16:05:55.715Z Reads: 178

```
i would hard mount heatsinks and otherwise cushion or mount the VESC before using a bigger copper foam like this.  I would guess a regular heatsink would have more surface area (in contact of FETs) and likely better heat transfer as a result.  Venting any heat into the air or even enclosure to dissipate.

Cool idea though!
```

---
## \#4 Posted by: flatsp0t Posted at: 2016-08-03T16:08:26.180Z Reads: 171

```
May be a problem if it is conductive, as you can not really control where it goes.
```

---
## \#5 Posted by: Raf Posted at: 2016-08-03T16:10:38.122Z Reads: 167

```
i was wondering why people wouldn't use it, but i guess thats why haha, good thing i asked. I don't tend to think too much about things, i just assume they work
```

---
## \#6 Posted by: Nordle Posted at: 2016-08-03T16:20:44.913Z Reads: 158

```
Some kapton where you don't want shorts. I can immagine this cools very well in an airstream (always while riding), maybe on top of a thin alu/copper plate.

where did you get this?
```

---
## \#7 Posted by: Raf Posted at: 2016-08-03T16:22:52.429Z Reads: 141

```
just thought of it whilst searching for waterproof foam
```

---
## \#8 Posted by: treenutter Posted at: 2016-08-03T16:46:26.972Z Reads: 131

```
[quote="Hummie, post:2, topic:7074, full:true"]
Zoinks.  Looks like a lot of shorting potential.
[/quote]

Yup! That seems like a bad idea. But it does raise a new question: are there non-conducive foam materials that could dissipate heat? I would love to fill some of the gaps in my enclosure with something useful.
```

---
## \#9 Posted by: JuniorPotato93 Posted at: 2016-08-03T16:51:06.736Z Reads: 128

```
Exactly my thoughts
```

---
## \#10 Posted by: Nordle Posted at: 2016-08-03T16:56:01.610Z Reads: 128

```
[quote="Nordle, post:6, topic:7074"]
Some kapton where you don't want shorts.
[/quote]
quote myself lol
```

---
## \#11 Posted by: furryfrog Posted at: 2016-08-03T17:00:15.794Z Reads: 117

```
I have never mounted a heat sink that is not conductive, I would say try it out, perhaps mounted on another smaller heat sink, and have an insulater on the portions that need it. how does one mount a product like this? Epoxy with a smaller aluminuim plate? straps?

Do you have a link to the product, or a datasheet?
```

---
## \#12 Posted by: JohnnyMeduse Posted at: 2016-08-03T17:01:14.344Z Reads: 110

```
Kapton tape is not magical and will eventually rupture, because the vibration will make the foam scratching the surface.
```

---
## \#13 Posted by: Raf Posted at: 2016-08-03T17:03:00.488Z Reads: 104

```
just some image i found on google, with heat sink foam written on it
```

---
## \#14 Posted by: Nordle Posted at: 2016-08-03T17:03:49.618Z Reads: 103

```
Wasn't the foam there to reduce vibration? But for sure kapton isn't magic, else i would eat it and become magic myself!
```

---
## \#15 Posted by: Hummie Posted at: 2016-08-03T17:05:10.722Z Reads: 104

```
http://www.lord.com/products-and-solutions/electronic-materials/thermoset-sc-320-thermally-conductive-silicone-encapsulant

Wish I'd got this instead of the stuff I got

This stuff and a couple stick on heat sinks on the fets and I think it'd be able to take real physical abuse and survive the heat. 

I don't have any heat problems ever. Never shut down. No heat sinks.  

kampton tape would thermally insulate I'd think.  Doubt it's thermally conductive.
```

---
## \#16 Posted by: JohnnyMeduse Posted at: 2016-08-03T17:07:10.209Z Reads: 103

```
Not sure if this flexible enough to even reduce vibration, it seem to be only good for reducing weight.
```

---
## \#17 Posted by: sl33py Posted at: 2016-08-03T17:08:49.901Z Reads: 104

```
"can" and are good are two different things.  Wood can conduct/dissipate heat, but it sucks compared to any metal.

Silver, Copper, Aluminum (gold in there too between copper and aluminum if you are rich and want bling) - from most efficient to least.  Take a look at the thermal conductivity of those metals as it's pretty interesting.  Again like others mentioned why i've used Arctic Silver 4/5 for years on my PC's heatsinks.

i would stick with the tried and true heatsinks vs a thermally conductive foam.  i want small/light and easy.  Adding some fins or the mount like @Chaka offers seems like the best solution IMO.  Some thermal paste to external fins w/ airflow would be my ultimate setup (while still enclosed/sealed from elements).
```

---
## \#18 Posted by: Nordle Posted at: 2016-08-03T17:26:15.860Z Reads: 98

```
That's probably true!
Flat is always better :D
```

---
## \#19 Posted by: flatsp0t Posted at: 2016-08-03T20:20:49.721Z Reads: 86

```
Maybe wee need a 2 part system with a heatpipe, so we can dissipate heat at the bottom of the board, and rebuy the actual heatsink for cheap if it breaks / gets too scratched.
```

---
## \#20 Posted by: Hummie Posted at: 2016-08-03T20:39:37.834Z Reads: 80

```
The e-go has a fan that attaches to the motor.  That's easy if u have the holes. 

get it out instead of transferring it to the hanger and making bushings softer.  


I did thermal paste to the hanger and it's hard to notice much benefit.   Bigger motors is the solution of course.  

Maybe make sure the windings are really well insulted at the soldered leads and squirt water or blast with pressurized air on the way up a mountain
```

---
## \#21 Posted by: KMeyerson Posted at: 2016-08-04T04:18:28.622Z Reads: 67

```
I've used high end silicone thermal pads with my R9 290Xs, CPUs, and most recently ESCs.  If you get them made with good quality and you only have ~1mm or less thermal pad between the heat source and sink, they work great.
```

---
