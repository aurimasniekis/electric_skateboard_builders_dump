# Is my FOCBOX fried after riding through salted streets?

### Replies: 24 Views: 1147

## \#1 Posted by: dAeM0N1K3 Posted at: 2017-12-14T22:21:14.682Z Reads: 204

```
So this past Monday I decided  to ride my Raptor through wet and salt filled streets to and from work. I didn't notice any problems riding either way. I wiped the board down thoroughly after each ride. The following afternoon I took the board outside and neither of the motors moved. I quickly brought it back inside my house to dry it off again and try to run the motors without any load on them. Only one would spin very slowly and the other didn't spin at all. I powered it off, opened the battery lid and powered it on again. I heard a little pop noise from one FOCBOX, then starting smoking a bit, so I quickly powered off again. I've since been hesitant to power it on again not wanting to potentially fry my other FOCBOX. 

Did I really just FOC-up my FOCBOXs riding in the shitty weather? What should I check or try next to correct the problem? Any help is greatly appreciated.
```

---
## \#2 Posted by: pat.speed Posted at: 2017-12-14T22:26:26.148Z Reads: 200

```
connect it to bldc tool and see if there are any fault codes
```

---
## \#3 Posted by: ThermalM16 Posted at: 2017-12-14T22:34:23.399Z Reads: 192

```
Can you freely turn the motors/ wheels with your hand? Also remove the plastic cover from the FOCBOX you believe is fried and post pictures of it here if you can
```

---
## \#4 Posted by: dAeM0N1K3 Posted at: 2017-12-14T22:39:40.493Z Reads: 188

```
One motor has resistance at a certain point of a 360 rotation, which is the one connected to the fried FOC'dBOX. I'll post pictures later tonight when I get home from work with the case removed.
```

---
## \#5 Posted by: onepunchboard Posted at: 2017-12-15T00:22:42.221Z Reads: 166

```
water alone is bad for electronic but with salt will actively corrod it. even the board is off
```

---
## \#6 Posted by: dAeM0N1K3 Posted at: 2017-12-15T17:21:03.299Z Reads: 142

```
okay guys, here are some pics of the FOC'dBOX. What's the damage? @ThermalM16

<img src="/uploads/db1493/original/3X/8/8/88cae68496b9063d5140db28aad767bbe3ee5622.jpg" width="666" height="500"><img src="/uploads/db1493/original/3X/3/5/3553264ded6c8366600ad677226f2ee16b469504.jpg" width="666" height="500">
```

---
## \#7 Posted by: Pedrodemio Posted at: 2017-12-15T17:27:22.811Z Reads: 137

```
@onloop

If I’m not mistaken the raptor is advertised as waterproof (IP67) so if just riding you got problems the warranty should cover
```

---
## \#8 Posted by: PXSS Posted at: 2017-12-15T17:28:56.491Z Reads: 137

```
I'd say you popped a fet based on the burn mark on the thermal pad

I would also check that your motor leads are not shorting out
```

---
## \#9 Posted by: dAeM0N1K3 Posted at: 2017-12-15T17:30:36.758Z Reads: 135

```
This is for the Raptor1, which I bought used. I purchased the FOCBOX's separately from a reseller. It's not under warranty
```

---
## \#10 Posted by: Blasto Posted at: 2017-12-15T17:41:10.513Z Reads: 128

```
Road salt is nasty stuff, wouldn’t consider this as salvageable. The fets are being chewed up as we speak
```

---
## \#11 Posted by: onepunchboard Posted at: 2017-12-15T17:45:05.294Z Reads: 125

```
U see the green stuff on fets? those are leadoxide or metal oxide, it is done. put it in garbage.
```

---
## \#12 Posted by: dAeM0N1K3 Posted at: 2017-12-15T18:05:39.355Z Reads: 125

```
You're probably right. I may take one more shot at it, maybe by thoroughly cleaning off any oxidation that I can and seeing what happens.
```

---
## \#13 Posted by: JohnnyMeduse Posted at: 2017-12-15T19:18:40.407Z Reads: 121

```
[quote="dAeM0N1K3, post:12, topic:41055"]
maybe by thoroughly cleaning off any oxidation that I can and seeing what happens.
[/quote]

The problem with salty water is that corrosion doesn't appear instantly... You will probably see more problem, especially with battery and BMS. 

as @Blasto said salty water is nasty stuff...
```

---
## \#14 Posted by: deucesdown Posted at: 2017-12-15T19:27:23.029Z Reads: 113

```
focbox has conformal coating, no? It should help at least a little bit?
```

---
## \#15 Posted by: telnoi Posted at: 2017-12-15T19:49:47.254Z Reads: 111

```
Sadly, no.
```

---
## \#16 Posted by: onepunchboard Posted at: 2017-12-15T19:52:34.503Z Reads: 111

```
even if it was coated, road salt eats away so maybe for short time but not a "proof". i burned few esc this way.
```

---
## \#17 Posted by: scepterr Posted at: 2017-12-15T19:57:57.405Z Reads: 109

```
Btw, I use this for salt cleaning after some fun snow riding 😋
http://amzn.to/2ARRu1x
```

---
## \#18 Posted by: ThermalM16 Posted at: 2017-12-15T23:02:57.331Z Reads: 95

```
Sorry for the late reply, I’ve been at work all day. Those FETs are in rough shape. If you have rubbing alcohol on hand, use that and a very very soft toothbrush to remove the corrosion and salt from the board.
```

---
## \#19 Posted by: PredatorBoards Posted at: 2017-12-15T23:20:57.598Z Reads: 85

```
Yep... it's the winter season, bois. If your city is known for salting the roads during this kind of weather, then you better start investing in some Silicone sealant and waterproof enclosures for your electronics.
```

---
## \#20 Posted by: dAeM0N1K3 Posted at: 2017-12-15T23:50:05.944Z Reads: 83

```
That's the thing, the opening where motor wires pass through the deck was completely sealed with silicone sealant. However, I'm thinking that some salt water may have leaked through the upper battery lid and pooled into the rear of the enclosure where the FOCBOXs sit. FML
```

---
## \#21 Posted by: guyguy Posted at: 2017-12-16T00:47:01.008Z Reads: 72

```
Man - that sucks. Who was your vendor? Did you talk to @barajabali
```

---
## \#22 Posted by: dAeM0N1K3 Posted at: 2017-12-16T02:59:23.040Z Reads: 62

```
Rocket-boards.com was my vendor @evoheyax . I've not spoken with barajabali. He repairs FOCBOXs/VESCs?
```

---
## \#23 Posted by: guyguy Posted at: 2017-12-16T06:04:34.249Z Reads: 51

```
He doesn't but he knows the process and may be able to help so I don't think it'd hurt to talk to him via PM. I'm not sure what the warranty process is through their resellers.
```

---
## \#24 Posted by: pat.speed Posted at: 2017-12-16T06:06:41.008Z Reads: 51

```
Speak to @JohnnyMeduse he is the repair guy for our vescs
```

---
