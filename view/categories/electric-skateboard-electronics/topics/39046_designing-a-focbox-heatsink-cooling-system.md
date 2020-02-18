# Designing a FOCBox heatsink cooling system

### Replies: 23 Views: 2076

## \#1 Posted by: zhud Posted at: 2017-11-23T03:13:19.348Z Reads: 276

```
Hello, I am new to the board, and I am looking for some input from those of you that have had experience with drawing a lot of current and managing heat across the FETs and the board itself.

I have been drawing up design sketches and modeling a few ideas about how to manage radiant heat  and dissipation by heat transfer from a small sized 12V blower fan. Some of the information that I have read so far about how well heatsinks perform on a VESC of any type, MOSFET or directFET, is often associated with how well the board itself is ventilated, not just wicking heat from the FETs themselves.

Currently I have constructed a few designs that have incorporated a large array of tall pins to help with heat dissipation, but after some consideration I am looking at making a ducting system that will push/pull air through a vent across cooling fins in addition to routing a duct to cool the board.

I have done some simulations on some 6061 with only the array of pins and the results seem promising as they are, but I have a very large prototyping and fabrication lab at my disposal and I am considering doing some testing to find an optimal cooling system.

I apologize if this is a little much for the forum, but I was hoping to get some input from experienced DIY'ers and possibly let me know where the VESCs have failed them in the past, and possibly how they went about to solve these issues. 

Thanks a lot for the wealth of information on this board and others, this community is extremely helpful and it often encourages me to try something different with my project.
```

---
## \#2 Posted by: Titoxd10001 Posted at: 2017-11-23T03:26:41.337Z Reads: 261

```
I was thinking of adding a heatsink or maybe just aluminum plate if there is clearance issues that are attached to the enclosure sort of like evolve has. Then tapping some holes on the focbox that are then screwed into the heatsink. Reason would be to get some airflow as they get a little toasty in a sealed enclosure currently. Hopefully that should be enough to keep them cool enough
```

---
## \#3 Posted by: zhud Posted at: 2017-11-23T03:36:15.602Z Reads: 250

```
Clearance and having the ability to keep the vesc in an enclosure is the biggest reason I decided against the tall pins for the heatsink.

The great thing about the small blower fan is that it has a shallow form factor that can be added to the surface of an enclosure and have an exhaust sent to a different location on the enclosure. It is also good that these small form factor blower fans are cheap and readily available.
```

---
## \#4 Posted by: pixelsilva Posted at: 2017-11-23T06:23:18.704Z Reads: 240

```
We should look for ideas in other fields. Perhaps bring some of the cooling systems use in computers. They come in different shapes an sizes, and one maybe small enough to be cramed into the e-board electronic enclosure.

<img src="/uploads/db1493/original/3X/e/8/e84b9940863e362b64954d72821f77ca3baef3fe.jpg" width="690" height="388">

...small components that we can even use there...

<img src="/uploads/db1493/original/3X/3/1/31136628fb3544352b75bf91464e08300e8a43a9.png" width="500" height="500">
```

---
## \#5 Posted by: Crossfire Posted at: 2017-11-23T06:35:13.670Z Reads: 228

```
Make sure you have some airflow in the enclosure. That will always help too cool electronics down. It's fall here, temps around 5-15 degrees C and my two focboxes never get over 35-40 degrees max. Usually they stay around 30's C. 
I'd say good airflow, dual drive and common sense driving and you won't have problems with heat. Single drives are just too big of a burden in the long run.
```

---
## \#6 Posted by: wafflejock Posted at: 2017-11-23T06:36:58.760Z Reads: 224

```
Water cooling looks cool but isn't really that practical you need a water pump and typically radiator with a fan on it (perhaps could just deal with the board moving to provide the airflow over the radiator).  I had my PC setup with a liquid cooling setup until the water pump took a crap and wasn't worth replacing it really for the minor reduction in noise.

---

Random thought make a ram air driven water pump, would probably need to be moving at a pretty good clip to make that work though.
```

---
## \#7 Posted by: pixelsilva Posted at: 2017-11-23T06:38:37.044Z Reads: 223

```
<img src="/uploads/db1493/original/3X/b/e/be90f47d1ff760b4262bd547474de924ad0d3bb7.png" width="499" height="500">
```

---
## \#8 Posted by: zhud Posted at: 2017-11-23T06:44:13.592Z Reads: 209

```
The water cooling is great at absorbing heat, but the problem with water-cooling is that you have to dissipate heat from the water, which requires a lot of energy, i.e. large fan cooled radiators. There are a lot of cases in PC cooling where a well designed heatsink is superior to a water cooled system. 

That being said, one of the big concerns regarding the heatsink is that it doesn't need to be complex or expensive, but reliable and compact.
```

---
## \#9 Posted by: zhud Posted at: 2017-11-23T06:50:22.931Z Reads: 210

```
"Ram air" is essentially what I am going for with a blower fan. 

These things come in all shapes and sizes. I have a few of them in my electronic scrap bin.

[https://www.reprap-france.com/sites/default/files/styles/prod-fiche/public/externals/6cd5206880cf2b95bc2bb16d85b0df5f.png?itok=hD8y2TFC](https://www.reprap-france.com/sites/default/files/styles/prod-fiche/public/externals/6cd5206880cf2b95bc2bb16d85b0df5f.png?itok=hD8y2TFC)
```

---
## \#10 Posted by: wafflejock Posted at: 2017-11-23T06:58:24.972Z Reads: 210

```
Yeah I was really thinking something more like using the incoming air with a duct that tapers to increase the air pressure going into it and turns something similar to your fan that has a part that goes into the water line to push the water through it to avoid having an electric powered water pump, but definitely pie in the sky idea:
https://www.youtube.com/watch?v=P1-UTlnjeVg

^^ plus my water pump crapping out made me think about it, but yeah in our case passive cooling or just active cooling with a fan ought to be plenty in any case.
```

---
## \#11 Posted by: E1Allen Posted at: 2017-11-23T07:35:30.255Z Reads: 205

```
<img src="/uploads/db1493/original/3X/7/a/7ac559a168ee79b90e675526e9be5b1efb373212.jpg" width="375" height="500">

Compact and same size as FOCBOX heatsink
```

---
## \#12 Posted by: zhud Posted at: 2017-11-24T15:58:14.204Z Reads: 179

```
Here is the design that I have currently. It hasn't been decided on whether the fan will sit atop the heatsink or be position with a blower towards the fins. 

It's still a rough version, but I'm leaning towards this sort of design.



<img src="/uploads/db1493/original/3X/c/6/c607e707ffee541d1278b5e2b3260d6985cad9cb.jpg" width="690" height="388">
```

---
## \#13 Posted by: zhud Posted at: 2017-11-24T17:47:47.638Z Reads: 174

```
Here is the bottom if anyone was interested in seeing it

<img src="/uploads/db1493/original/3X/6/0/60505600b804a3b63a9d77795f4950680898a1d1.jpg" width="690" height="285">
```

---
## \#14 Posted by: banjaxxed Posted at: 2017-11-24T19:21:18.014Z Reads: 164

```
Water cooling fans etc are great but the focbox is pretty good cooling wise over a regular vesc and rally it's overkill.

I'd like to see a simple 3d printed box that you can slide a 2mm piece of aluminium strip into that has threaded holes for small cables glands to the battery/motors and optional hole for USB connection. Of course there should be room for the receiver too.

The reason being is that a lot of folks here have or have access to a 3d printer, alum pieces can be got easily off eBay etc 

The alum can be cut down to size using a small hacksaw/file then simply slides into the top of the enclosure, the other side of the enclosure could be open since it faces the deck and you can use traditional sealing
```

---
## \#15 Posted by: zhud Posted at: 2017-11-24T20:26:33.996Z Reads: 149

```
The problem is that when you push the VESC to its current limits, the FETs to produce an amount of heat that can be outside of the operating window for the FETs. Going up hills and high torque situations really do call for a better cooling solution. 

From what I’ve read from the developer, the reason fin cooling wasn’t incorperated into the design is because, in most cases, the VESCs are within an enclosure.
```

---
## \#16 Posted by: banjaxxed Posted at: 2017-11-24T20:54:29.484Z Reads: 145

```
Right but we are talking about a focbox and a cooling solution 'outside the box', while the design of the focbox helps with cooling it does little to help water resistance which would allow mounting outside an enclosure. The ability to mount outside would really really help with cooling airflow etc
```

---
## \#17 Posted by: JohnA Posted at: 2017-11-24T21:17:16.330Z Reads: 147

```
Here’s my cooling system, the focboxes haven’t ever gone over 39C when riding up hills. They used to overheat and limit amps when I had them just sitting in an enclosure <img src="/uploads/db1493/original/3X/9/3/934b4ca89427bedbdee52f6bacf6c439a40474ba.JPG" width="666" height="500"><img src="/uploads/db1493/original/3X/9/b/9b3b2eedb33753126f59524e945b4818088e5546.JPG" width="375" height="500"><img src="/uploads/db1493/original/3X/e/6/e6011bfa3a51b37067f733e847f53e3f60f58a4c.JPG" width="666" height="500"><img src="/uploads/db1493/original/3X/a/2/a21746d2358e6763be8a92efac567aff8a514d0a.JPG" width="375" height="500">
```

---
## \#18 Posted by: zhud Posted at: 2017-11-24T22:43:59.543Z Reads: 136

```
JohnA, that is awesome. So you saw a noticeable improvement by adding cooling, assuming roughly 80C to 40C? That is very good to know! 

I am going to run some trials for my design soon. I hear what banjaxxed is talking about, of course. My interest is very much trying to keep a design has the ability to have a dedicated blower fan that would keep it in an enclosure, and safely away from water.

I'll provide the final design of the open fin design below.
```

---
## \#19 Posted by: zhud Posted at: 2017-11-24T22:48:08.301Z Reads: 142

```
Here is the final design for the open top fin heatsink. If you want to use your imagination, the close top will be almost the same, but with a solid top channeling air through venting in the front.

<img src="/uploads/db1493/original/3X/7/c/7c4fab53827a39023a2c4d0841ed0002bedf08fd.jpg" width="690" height="388"><img src="/uploads/db1493/original/3X/b/6/b6d63f345aebc59b3405f103497cfdc2905addb6.jpg" width="690" height="388"><img src="/uploads/db1493/original/3X/7/1/7178b7d1c1885a0f8d34b325b39c5c8baecc1f87.jpg" width="690" height="388"><img src="/uploads/db1493/original/3X/2/6/2619920ee1131ed1490ef6f19f14923367aade24.jpg" width="690" height="388">
```

---
## \#20 Posted by: E1Allen Posted at: 2017-11-25T00:26:53.868Z Reads: 135

```
<img src="/uploads/db1493/original/3X/9/2/929f1daab2afb27854ebe0329595b3c403611f29.JPG" width="375" height="500">

Still trying to get mine hot.
```

---
## \#21 Posted by: Kug3lis Posted at: 2017-11-25T00:32:21.054Z Reads: 128

```
Guys, u need thermal mass, not fans and fins... Our cases never even went higher than 50ºC with older vesc
```

---
## \#22 Posted by: JohnA Posted at: 2017-11-25T02:50:26.263Z Reads: 122

```
Yeah roughly after looking at app data. It was also a cooler day out so that woulda helped some.  @Kug3lis for computer gpu’s or cpu’s Do they just use mass to cool them? Our application is obviously different, but combining a mass of aluminum and fins would probably be the best .
```

---
## \#23 Posted by: zhud Posted at: 2017-11-25T03:52:12.300Z Reads: 122

```
Lets assume that there is some middle ground between fins fans and thermal mass. There is a need to limit thermal mass, and I am trying to develop something that has thermal mass and incorporates fins and a fan. 

Personally, I don't think that adding thermal mass is the complete answer. Being that aluminum isn't the best for wicking heat away from the source. That being said, aluminum is great at dissipating heat whereas copper attracts heat and likes to hold it. The most ideal setup would have a copper core and an aluminum shroud that would dissipate the heat for the copper. 

Straying away from material thermodynamics, I believe the best solution would keep the thermal mass closest to the FETs at a minimum while keeping the majority of the mass away from the FETs. I think this will be able to keep some of the excess heat stored away from the FETs and allow it to be dissipated in time.
```

---
