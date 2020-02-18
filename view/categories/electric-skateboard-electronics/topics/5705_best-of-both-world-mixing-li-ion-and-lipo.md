# Best of both world mixing li-ion and lipo

### Replies: 84 Views: 7795

## \#1 Posted by: edwardlui531 Posted at: 2016-07-07T08:23:04.152Z Reads: 441

```
I have a really nice high c rating 6s lipo battery with only 3300mah. As you might know, that doesn't offer a lot of range. At the same time, I have a bunch of free 18650s(salvage from laptop) that I have left from building my ebike. 
These 18650 are rated for 2c (they are usually 1-2ah) and there is no way I am putting 6s25p to give me 100amp draw.

So, what if I I just say make a 6s4p lion and parallel them with my lipo pack so I have range AND torque(high amp) when I need to.
```

---
## \#2 Posted by: DeathCookies Posted at: 2016-07-07T08:51:16.999Z Reads: 416

```
Like @lowGuido would say: "Do it for science" ;)
```

---
## \#3 Posted by: edwardlui531 Posted at: 2016-07-07T08:54:46.758Z Reads: 419

```
I have a lion blow up next to me before and now I am scared. But I might, I just wonder have anyone in here done that b4.
```

---
## \#4 Posted by: DeathCookies Posted at: 2016-07-07T09:02:34.560Z Reads: 411

```
[quote="edwardlui531, post:3, topic:5705"]
But I might, I just wonder have anyone in here done that b4.
[/quote]
I dont think so.

Normally everyone would advertise you to not mix different C rating because the higher rated cells could potentially overdischarge.

You should not use different Ah rating --> same effect.


But i can imagine that the higher c and ah will equal the liion batterys but i dont know.
```

---
## \#5 Posted by: Nordle Posted at: 2016-07-07T09:08:49.712Z Reads: 377

```
You can use diefferent C rating batterys in a pack as long as they have same capacity and min/max voltage.
But nothing best from both worlds, cause you'll be limited to the C rating of the weakest battery in your pack.
```

---
## \#6 Posted by: DeathCookies Posted at: 2016-07-07T09:15:50.088Z Reads: 373

```
[quote="Nordle, post:5, topic:5705"]
You can use diefferent C rating batterys in a pack as long as they have same capacity and min/max voltage.
[/quote]



You can do everything you want ;) I just said that nobody would **advertise** you to mix batteries![quote="Nordle, post:5, topic:5705"]
But nothing best from both worlds, cause you'll be limited to the C rating of the weakest battery in your pack.
[/quote]

Could you explain that in a bit more detail?
```

---
## \#7 Posted by: PB1 Posted at: 2016-07-07T09:29:14.331Z Reads: 342

```
@edwardlui531, I think it should work. 
Higher C rating akkus have lower internal resistance, so if the need for lots of amps arises the amps will come from the Lipos. If the lipos voltage sags they will be supported by the 18650. Similar functionality like a capacitor. 
Don't think its dangerous to parallel these akkus as long as they have the same voltage when they are connected. 

The worst thing that could happen is you destroy or weaken your 18650 because they are also providing amps.  

And of course, if you mix different C rating akkus in series, only draw as much current as the weakest can handle and monitor the individual cell / pack voltage. 

Do it and tell us how it went. :yum:
```

---
## \#8 Posted by: Nordle Posted at: 2016-07-07T09:32:05.319Z Reads: 316

```
When i said ''you can'', i meant ''it would work totally fine''...
...better?

More detail here:
2 batterys, both 3V-4.2V, both 1000mAh, one is 5C (x1Ah= 5A) the other is 10C (x1Ah=10A)
now we wire both batterys in parallel to get 2Ah, but the C rating stays 5C, cause the weakest cell in our parallel group has 5C. 2Ah x 5C = 10A. 10A is what you could draw from this example battery.
Draw more, for example 15A, would be 7,5A per cell, but as you can see above our weakest cell only can handle 5A. Puff magic smoke inc.
```

---
## \#9 Posted by: PB1 Posted at: 2016-07-07T10:48:48.412Z Reads: 290

```
ok, let's all agree that @edwardlui531 should do this ... :grin:

@Nordle, just for the sake of it, I have a correction. 
[quote="Nordle, post:8, topic:5705"]
Draw more, for example 15A, would be 7,5A per cell, but as you can see above our weakest cell only can handle 5A. Puff magic smoke inc.
[/quote]

Current will not be symmetrical because batteries with different C ratings also have a different internal resistance. 

So in the example of the OP, his 6s4p pack can maybe supply 16 Amps, the lipo maybe 40 Amps (no C rating mentioned). In theory the total system can supply 56 Amps, however when we pull those Amps we don't know which pack will supply how much. But we know it will not be symmetrical. In order to calculate it we have to measure the internal resistance. 
It could also be that even if the motor only draws 40 Amps (below the limit of the lipos) too much current comes from the 18650. 
As mentioned, the biggest risk is that the cheap 18650 are aging more quickly than normal. 

Oh, and btw, some charger can measure the internal resistance of an akku pack. If the resistance of the lipo is significantly lower than the resitance of the 18650 pack and total current does not go over the limit of the lipo then everything is fine.
```

---
## \#10 Posted by: Nordle Posted at: 2016-07-07T11:48:39.830Z Reads: 243

```
However, i still think as long as you don't exceed the lower C rating you're fine. I read a long thread on ES about this just can't find it atm..
```

---
## \#11 Posted by: Namasaki Posted at: 2016-07-07T15:40:09.499Z Reads: 219

```
My opinion, it's a bad idea to mix different types of batteries together in series or parallel. 
You could be playing with fire.
```

---
## \#12 Posted by: treenutter Posted at: 2016-07-07T16:11:59.147Z Reads: 211

```
[quote="Namasaki, post:11, topic:5705"]
You could be playing with fire.
[/quote]

I completely agree with @Namasaki. Don't do this. You spare yourself from having to buy a second $30 LIPO, but that's the only benefit.

If you really want to use your 18650s, you can buy a few more salvaged laptop batteries on Ebay, fully test them, and build a pack with the ones you already have. 

I think proper respect is due here; when you use LIPOs it's better to play it safe.
```

---
## \#13 Posted by: laurnts Posted at: 2016-07-07T17:20:33.119Z Reads: 198

```
To be very honest, I don't see any problem combining lipo and liion as long as they are in parallel. The higher c rating will provide the burst when needed. Battery connected in parallel have a tendency to equalize on discharge, so they will naturally balance out each other. Same to capacitor, they also actually a battery, only short burst connected in parallel. Hence I don't see the problem doing so, correct me if I am wrong.
```

---
## \#14 Posted by: edwardlui531 Posted at: 2016-07-07T17:24:30.006Z Reads: 196

```
[quote="Namasaki, post:11, topic:5705"]
You could be playing with fire.
[/quote]
When I built my ebike battery, I already knew what I got myself into. Thanks for looking out for me tho, I really don't want to burn my house down.

[quote="treenutter, post:12, topic:5705"]
If you really want to use your 18650s, you can buy a few more salvaged laptop batteries on Ebay, fully test them, and build a pack with the ones you already have.
[/quote]
Again, according to my calculation, I will need 6s25p to get me 100amp draw. 

[quote="PB1, post:7, topic:5705"]
Similar functionality like a capacitor.
[/quote]

Yes that is exactly what I am thinking. Now, upon connecting them in parallel on the big terminal, should I also connect them via balance lead?
```

---
## \#15 Posted by: Namasaki Posted at: 2016-07-07T17:39:05.631Z Reads: 175

```
[quote="edwardlui531, post:14, topic:5705"]
Again, according to my calculation, I will need 6s25p to get me 100amp draw.
[/quote]

I'm curious, why would you need 100a capability. 
I've done some real life testing with 6s and dual motors going uphill and pulling less than 40a from my batteries.
```

---
## \#16 Posted by: Okami Posted at: 2016-07-07T17:39:41.301Z Reads: 188

```
Report when you have some more info on this. 

I also played with the idea of connecting lipos and liion together.. Although, what seemed safer for me, was to make a ''battery switch'' to be able to switch between lipo and liion.

 Although, Im also scared of the low discharge / c rate of the liions.. Im also planning on using laptop batteries with 2c rate, that would give around 4A for 1 cell (2250mah original capacity).. which is not very bright, 16A total (for 6S 4P connection)

So, if you do find a way and it works, that would be awesome! Please give all info you find on this topic, if you find that someone has done similar!
```

---
## \#17 Posted by: edwardlui531 Posted at: 2016-07-07T18:16:26.155Z Reads: 186

```
[quote="Namasaki, post:15, topic:5705"]
less than 40a
[/quote]

<img src="/uploads/db1493/original/2X/c/c90de45cefa7801390594b02369d647eed19755c.png" width="690" height="431">
screenshot of my single motor bench amp draw test, you can see it peaks at 56 but I put a lot of presure. I plan on doing dual motor, so I say 80-100amp is probably a guide line. Also I live in san francisco which have some steep hills.
[quote="Okami, post:16, topic:5705"]
I also played with the idea of connecting lipos and liion together.. Although, what seemed safer for me, was to make a ''battery switch'' to be able to switch between lipo and liion.
[/quote]

that means you will also need to switch in the bldc bat min(regen) setting which I don't think you can change vesc on the fly.
```

---
## \#18 Posted by: devin Posted at: 2016-07-07T18:59:09.087Z Reads: 175

```
<p>This post was flagged by the community and is temporarily hidden.</p>
```

---
## \#19 Posted by: Namasaki Posted at: 2016-07-07T19:05:30.814Z Reads: 171

```
Running dual motors doesn't double the load, it devides the load between the motors. 
So you have 23a peak per motor
```

---
## \#20 Posted by: Namasaki Posted at: 2016-07-07T19:06:30.858Z Reads: 169

```
You should never mix batteries of different chemistry
```

---
## \#21 Posted by: PB1 Posted at: 2016-07-07T19:10:17.946Z Reads: 161

```
Again,  it depends on the internal resistance of the battery packs.  If the resistance is not the same (and it will not be),  then the packs will not provide the same amps.  The lipo with the higher C rating should have lower resistance and will provide more amps.  
So would say that if you are within the limits of the lipo then you are safe.  You might deteriorate your lions,  but that's not so bad if they are old and used already...
```

---
## \#22 Posted by: barajabali Posted at: 2016-07-07T19:10:50.835Z Reads: 157

```
In E-skate you can cheap out on a lot of things... but not the battery.  Just buy this and youre fine. 
http://www.ebay.com/itm/6S-8000mAh-30C-LiPo-Perfect-For-The-FreeWing-ME-262-Free-Fast-Shipping-/301870715688?hash=item4648e59328:g:-gQAAOSwG-1Wu3ob
And follow my thread 
http://www.electric-skateboard.builders/t/how-i-made-my-lipo-packs-slimmer/1415

there you go for about $100 you get a  177 WH pack which is 1.77 times larger than boosted board.
```

---
## \#23 Posted by: Namasaki Posted at: 2016-07-07T20:16:52.980Z Reads: 146

```
Please consider this:
The C rating of a battery does not limit the current load that you can put on it. 
It only tells you how much load you can safely put on it. 
So, if you put low C rated li-ions together with high C rated Lipos and try to put a high amp load on them, you will have a recipe for disaster. 
Because the Lipos and the li-ions will be exposed to the same high current regardless of there C rating.
```

---
## \#24 Posted by: Jinra Posted at: 2016-07-07T20:19:19.719Z Reads: 133

```
Is that how it works? I've also thought of an analogy where the current is like water being blocked by a gate, and completely opening the gate is the full discharge rate of the battery. You're saying that a controller can attempt to pull more than the rated discharge of the battery?
```

---
## \#25 Posted by: Namasaki Posted at: 2016-07-07T20:23:04.446Z Reads: 127

```
[quote="PB1, post:21, topic:5705"]
The lipo with the higher C rating should have lower resistance and will provide more amps.
[/quote]
Amps are not provided by the battery. 
Amps is the measurement of current flowing through the circuit. Starting at the pos side of the battery and ending at the neg side of the battery.  And the current flows equally through every component of that circuit.
```

---
## \#26 Posted by: Namasaki Posted at: 2016-07-07T20:25:24.880Z Reads: 119

```
Yes, that is what I'm saying. 
A good example is when you short the battery which flows enough current through it to make it explode.
```

---
## \#27 Posted by: Jinra Posted at: 2016-07-07T20:26:09.771Z Reads: 114

```
Ah okay. I just assumed that shorting it would just produce the discharge current on the wire and since the energy has nowhere to go, it turns to heat.
```

---
## \#28 Posted by: Namasaki Posted at: 2016-07-07T20:28:08.012Z Reads: 119

```
[quote="Jinra, post:24, topic:5705"]
You're saying that a controller can attempt to pull more than the rated discharge of the battery?
[/quote]
The C rating does not protect the battery. 
It only give you a guideline.
```

---
## \#29 Posted by: treenutter Posted at: 2016-07-07T20:38:33.206Z Reads: 120

```
[quote="edwardlui531, post:14, topic:5705"]
I will need 6s25p to get me 100amp draw
[/quote]

Why do you feel that you need 100A draw? We rarely exceed 30A-40A continuous draw on an esk8.
```

---
## \#30 Posted by: devin Posted at: 2016-07-07T20:51:02.897Z Reads: 121

```
<p>This post was flagged by the community and is temporarily hidden.</p>
```

---
## \#31 Posted by: PB1 Posted at: 2016-07-08T11:43:21.529Z Reads: 126

```
With all due respect here @Namasaki I have to disagree. Now I'm arguing just for  the sake of it :-) 

When components are connected in parallel, current does not flow equally. And yes, the battery provides the amps (current). 

I fully agree that a battery can deliver more amps than their C rating, but it's not good for them and might event destroy them. Never said anything else.  
Below I tried to make a somewhat simplified diagram. 
- Let's assume the motor has to provide 1000 Watts in order to move the rider forward.  
- Let's assume the batteries both have 6 * 3,7 Volts = 22,2 Volts
- Then 45 Amps will have to flow into the controller (I'm neglecting inefficiency here) (P = U * I) 

Where will these Amps come from? The batteries will have to provide them. If they can't, power will drop. If the batteries can, they will provide the current, regardless if this is within their C rating or not. 
Now how is the amps provisioning split up between the packs? Here the internal resistance comes into play.
Assumption is that the internal resistance of a Lipo cell is around 6mOhm per cell so 36mOhm in total.  
Now the internal resistance of one 18650 cell is around 100mOhm, so for a 6s1p pack its 600mOhm and for a 6s4p pack it's 150mOhm (paralleling resistance decreases overall resistance). 

The total current (45Amps) will come from the two sources in the same ration 36:150 as their internal resistance. 
So the lipo will provide 34,2A and the 18650 pack will provide 10,8A or 2,7A per cell (10,8A / 4) 

Both battery packs are within their limits in this example and we are safe!

<img src="/uploads/db1493/original/2X/2/25ec1bd6168cdfd191fcb2c845bb561ced9fe92c.jpg" width="247" height="500">

If the motor has to provide 2000 Watts, this is double the current for the batteries. The lipo might still be ok providing 68,4A because it is within its C rating. The 18650 pack will also provide its needed share of the amps and it will provide 21,8A. So this is 5,6A per Cell. If this is above their C rating they will deteriorate quickly (its probably not above their max current, especially not for a short time). They will not explode, just not last forever. 

The example should be very close to reality, in real life you could measure the internal resistance of your batteries e.g. using a good battery charger. 


Btw, the actual electrons flow from minus to plus but that doesn't matter. 
btw2, I simplified some things here, e.g. the voltage drops while the batteries provide the amps by the value R(i) * I = U(i), so if power demand stays the same the current will increases in order to compensate that
btw3, internal resistance increases with the age of a battery, this leads to more heat which deteriorates the battery and increases their internal resistance, which lead to more heat, .... 
btw4, I stop here because nobody will be reading this anyway ... ;-)
```

---
## \#32 Posted by: DeathCookies Posted at: 2016-07-08T11:59:09.326Z Reads: 110

```
[quote="PB1, post:31, topic:5705"]
btw4, I stop here because nobody will be reading this anyway ... :wink:
[/quote]

Nope, your comment is very informative! I still learn new things everyday.

So thumbs up for the nice answer! :thumbsup:
```

---
## \#33 Posted by: Namasaki Posted at: 2016-07-08T12:34:41.603Z Reads: 104

```
Btw5 I read the whole thing. I'll have to respond later because my work shift starts now. 
Btw6 I love a good argument. This is how we get to the bottom of things.
```

---
## \#34 Posted by: Namasaki Posted at: 2016-07-08T15:50:25.812Z Reads: 110

```
[quote="PB1, post:31, topic:5705"]
Btw, the actual electrons flow from minus to plus but that doesn't matter
[/quote]

Direct current or DC electricity is the continuous movement of electrons from negative to positive through a conducting material such as a metal wire. A DC circuit is necessary to allow the current or steam of electrons to flow. In a circuit, the direction of the current is opposite the flow of electrons.Jan 11, 2004
Direct Current (DC) Electricity - Physics Lessons: School for ...
www.school-for-champions.com › science
CURRENT FLOWS FROM POS TO NEG
```

---
## \#35 Posted by: devin Posted at: 2016-07-08T15:59:54.810Z Reads: 100

```
<p>This post was flagged by the community and is temporarily hidden.</p>
```

---
## \#36 Posted by: Namasaki Posted at: 2016-07-08T16:08:24.112Z Reads: 106

```
<img src="/uploads/db1493/original/2X/d/d0428adf2cb3172da23efadd59b5e27320550ddc.jpeg" width="247" height="500">
The problem with this drawing is that the Esc is going to try to draw equal current from the Lipo and the Li-ion.  34a.  If the Li-ion can only handle 10a, the rest of the current will turn into heat. So the li-ion will get hot in this situation and if you do it too much, the battery will fail.
```

---
## \#37 Posted by: PB1 Posted at: 2016-07-08T16:30:21.233Z Reads: 102

```
[quote="Namasaki, post:36, topic:5705"]
The problem with this drawing is that the Esc is going to try to draw equal current from the Lipo and the Li-ion.
[/quote]

No. Not equal because internal resistance is different. 

In my diagram something got cut off. the lowest arrow should be marked with 45A (10,8A + 34,2A).

BTW 7 I just measured the internal resistance of one of my lipo packs and of one 18650 cell. 

5S Turnigy Nano-tech 4000mAh 25-50C: the internal resitance of the whole pack is 22mOhm, so 4,4mOhm per cell. 
Samsung 18650 25R (one cell): 42mOhm

So the figures I gave above are not too far off. Again, the bigger the C rating, the lower the internal resistance, the more current will flow through the battery. This is why they are more efficient.
```

---
## \#38 Posted by: PB1 Posted at: 2016-07-08T16:33:32.272Z Reads: 99

```
[quote="Namasaki, post:34, topic:5705"]
Btw, the actual electrons flow from minus to plus but that doesn't matter

Direct current or DC electricity is the continuous movement of electrons from negative to positive through a conducting material such as a metal wire. A DC circuit is necessary to allow the current or steam of electrons to flow. In a circuit, the direction of the current is opposite the flow of electrons.Jan 11, 2004Direct Current (DC) Electricity - Physics Lessons: School for ...www.school-for-champions.com › scienceCURRENT FLOWS FROM POS TO NEG
[/quote]

so I'm being a smartass here. I seems you are agreeing. 

Current flows from Pos to neg, this is what everybody says. 
Actually, the electrons go from negative (minus) to positive (plus) - just what I said. But it doesn't really matter for this argument.
```

---
## \#39 Posted by: Okami Posted at: 2016-07-08T17:09:07.808Z Reads: 93

```
But can you comment on capacity differences after continous discharge? 

What will happen when these liions will be discharged at 10A, while Lipo's at 30A.. the voltage will be (?) different at some point, I think. 

Otherwise, there needs to be a circuit which cuts off the depleted battery or something like that.. (btw, I would not be using Vesc, but regular car esc)

Have not done any real life tests.. so dunno how this might work out in the field, what I only know, there tends to be a thing, where batteries balance themselves out, if they are connected in parallel directly..
```

---
## \#40 Posted by: treenutter Posted at: 2016-07-08T17:13:50.007Z Reads: 96

```
@Namasaki and @PB1 just wanted to thank you both for a great discussion; I'm learning from it! Also thanks to you both for being able to have a respectful discussion even when you disagree w each other.
```

---
## \#41 Posted by: PB1 Posted at: 2016-07-08T17:21:23.510Z Reads: 89

```
If the components,  in this case the batteries,  are in parallel then  the voltage is the same.  

So true,  one battery pack has higher capacity.  But because it provides less amps its capacity will not go down as fast.  The system will regulate itself.
```

---
## \#42 Posted by: Okami Posted at: 2016-07-08T17:22:17.887Z Reads: 82

```
Ok, thanks for input.. now we need someone to test this out!
```

---
## \#43 Posted by: PB1 Posted at: 2016-07-08T17:28:26.082Z Reads: 84

```
Agreed,  now back to @edwardlui531 for some testing.  
And to answer your question,  I think paralleling the balance leads would help stabilizing the battery system.
```

---
## \#44 Posted by: Namasaki Posted at: 2016-07-08T17:48:38.434Z Reads: 86

```
[quote="PB1, post:38, topic:5705"]
Current flows from Pos to neg, this is what everybody says. Actually, the electrons go from negative (minus) to positive (plus) - just what I said. But it doesn't really matter for this argument.
[/quote]
Electrons stream from neg to pos but
Current flows from pos to neg. 
It really does matter because it is important to know what direction current is flowing. For example, when deciding where to place a fuse.
```

---
## \#45 Posted by: Namasaki Posted at: 2016-07-08T17:56:42.682Z Reads: 80

```
So, have you tested your theory?
Or can you provide some other evidence that proves it?
```

---
## \#46 Posted by: Namasaki Posted at: 2016-07-08T18:09:29.733Z Reads: 79

```
your theory seems to suggest that the internal resistance regulates curren flow. 
I don't believe this is correct. 
If it was, then C rating wouldn't matter at all. 
And a battery wouldn't explode when shorted with a wire because the internal resistance wouldn't allow current to flow excessively. 
I'm sorry, but in my opinion, your theory doesn't seem to hold water.
```

---
## \#47 Posted by: PB1 Posted at: 2016-07-08T18:16:46.870Z Reads: 81

```
C rating is a function of internal resistance. It's used for convenience because most people can't deal with internal resistance.  

I believe my theory is correct and I could provide more evidence by providing more calculations.  

But I can't ...  Because I have to go ride my board until my Akku is empty and I can't post here while riding...  :innocent:
```

---
## \#48 Posted by: edwardlui531 Posted at: 2016-07-08T19:02:23.812Z Reads: 83

```
Thank you for the input, that is exactly what my theory is :grin:
now, do you think I can add a resistor to the liion pack so it will never exceed the amp draw that I wanted? or is there some sort of special resistor that only limits when it gets to certain current?

Guys, I still start by testing the internal resistant of my pack.
```

---
## \#49 Posted by: PB1 Posted at: 2016-07-08T19:29:20.466Z Reads: 85

```
And I have to admit that I was wrong ....  

<img src="/uploads/db1493/original/2X/6/643309a3b177b63cdae4e73a13e955793a19a0be.jpg" width="375" height="500">

...  I am able to post while out riding.  

All the other stuff was correct  -  of course.
```

---
## \#50 Posted by: Hummie Posted at: 2016-07-08T19:43:36.141Z Reads: 86

```
http://diydrones.com/m/discussion?id=705844%3ATopic%3A1095758


The end of this says the internal resistance and lower mah pack can balance as the resistance will reduce draw from that pack regardless of c rating
```

---
## \#51 Posted by: Okami Posted at: 2016-07-09T07:59:49.991Z Reads: 93

```
I hope that ''Roger Sterling'' from that diydrones.com topic does not mind, that I quote his contribution to this topic. So here it is goes (for the benefit of continuing this thread and educating others)

> **Roger Sterling, Dec 21, 2015, diydrones.com: ''Different batteries in parallel?''**

> A very accurate model of a battery is an ideal battery in series with a resistor equal to the batteries internal resistance. When under an external load the voltage at the battery's terminals is the no load voltage minus the voltage drop across the internal resistance. 

> For batteries in parallel and under a load, **it is the terminal voltages that must be equal**. This will differ from the no load voltage ( ideal voltage). For two batteries in parallel with the same zero load terminal voltage, the ratio of the current supplied when a load is switched on  by each battery would be the inverse ratio of the internal resistance.

> The instance a load is switched on, the battery with the lowest internal resistance would supply more current and this has nothing to do with the batteries capacity. Depending on the capacity of each battery, it's contribution to the total current, and the discharge characteristics, the no load voltages difference (Bat1 - Bat2) could be positive, negative or zero. 

**Statements:**
>  As long as each Battery can handle the entire load without damage none of this imbalance in discharge rate really matters much until one of two things happens.
> _1) The load is suddenly switched off_
> _2)_ _One of the batteries reaches it's full discharge voltage before the other._

**Situations:**

> **In case 1**, each battery's voltage will instantly increase. I measured this increase on 4 parallel 18650's under a 1 amp load to be about .2 volts. Each battery in a parallel pack will increase in voltage by the product of their contribution to the previous total current times their internal resistance at whatever SOC, they are at. For different battery types there will no doubt be a voltage imbalance and current will surge from one battery to another. The higher the previous load current the higher this voltage difference will be. If it were only .3 volts and the combined internal resistance of the batteries was 50mOhms the instantaneous surge current would be 6 amps, which may exceed one or both max current rating. Of course this current would discharge one and charge the other and rapidly balance the batteries. 
But there is a slight potential to cause one or both to suffer a capacity 
--
> **Case 2** can have devastating impact on a battery. Say one battery safely can discharge down to 2.8 volts and it's parallel partner can drop to 2.5. If there is no protection circuit the 2.5 battery will happily continue to drain current into the load after the 2.8 is already in dangerous territory. The best solution is individual protection on each. The parallel pack could share a single protection circuit that shuts them down above the 2.8 volts. There would be a loss in usable capacity of the 2.5 volt battery, but at those voltages it wouldn't amount to much.

**Conclusion:**

> A good rule of thumb is to try to use batteries of **near equal capacity and similar internal resistance**. 




> **If you do use different capacity batteries try to make sure the smaller one has a higher internal resistance.**

> Example: **1/2 the capacity with double the resistance.** This will make sure each battery follows the same discharge curve and the voltage surges from sudden load change shouldn't be a concern
```

---
## \#52 Posted by: laurnts Posted at: 2016-07-09T08:13:20.115Z Reads: 80

```
--- might be slightly different than the topic ---To be very honest with you guys. I agree that if you run VESC monitor mode, you can see the peak current draw of a motor would be around 20A - 40A. That means 10c - 15c battery from a 5000mah pack would be good enough. This is true! however if you try buy those 45c battery or setup some more parallel batteries, you will see more power could be delivered to the motor. You get more aggressive respond. This just a FACT! you can roll whatever number there is, but the truth is the higher c rating improve performance to a certain point around 65C 5000mah (more than that) doesn't do much improvements.
```

---
## \#53 Posted by: Okami Posted at: 2016-07-09T08:17:00.055Z Reads: 80

```
So that brings us to the point, that it's just not going to be as agressive / fast as it could be (2 batteries with different c ratings).. I suppose
```

---
## \#54 Posted by: laurnts Posted at: 2016-07-09T08:29:06.387Z Reads: 91

```
Trust me. If you ever go racing with same board on same track. I guarantee you the higher c rating battery wins. It gets you accelerate faster, those burst of energy when acceleration are provided by the batteries, not the esc.

Well if you confuse with all this mixing c rating, theres a simple case that might help you clear out why it's actually okay.

You have several batteries of 5000mah 20c rating connected in parallel. Lets say one of it is damaged, so it can only store 4000mah (memory effect / other cause). Although the c rating stays the same 20c, but different in mah means different max discharge capacity. The board will still runs... ofc with the fact that if you throttle up / accelerate, the 5000mah 20c battery will do most of the heavy lifting.

----

Any how anyway, why do you want to mix - match different batteries in the first place in order to get best of both worlds? the benefit is so insignificant compared to full lipo or full lion. Mix batteries makes your build more complex and charging is more complex, which may is prone of breaking.

If you think lipo is super cheap but cant quite bear the low life cycle, then add more lipo in parallel. The least you put the battery under pressure / heavy load, the longer it live.

If you think li-ion is better in terms of life cycle, but poor in discharge, then please add more li ion in parallel. The more the parallel connections, the higher the discharge capability.

Stop making yourself too difficult :slight_smile:
```

---
## \#55 Posted by: Okami Posted at: 2016-07-09T08:57:31.590Z Reads: 86

```
I think the point here is in utilizing / using the low discharge batteries (if you have lots of them), that way saving the lipo's a few cycles or improving your ride distance.. Otherwise, as always, if you have shitload of money and can build a high quality / premium cell, do it that way.. 

There will be always someone who will see the bad sides and good sides.. mixing of both worlds, at least in my case, just means that you don't spend, say 200$ for new batteries, but use the available ones (40$-50$ value?).. and try to make the best out of them.. not saying it's the best option or whatelse, it's just gaining some experience (like building a low grade battery first) and testing out what comes after.. if it's a crap / waste of time.. then gladly someone will come to this realisation and post it online for others not to try it..

not saying it is the best option,.. it won't be, if it won't work, just ditch it, use these batteries elsewhere and think about ways of gettings hands on some good cells / pre made battery. It's the idea about being able to use lower discharge batteries and still gain some benefit from them.. Are they 100% up for this application? not quite.. Is it possible to at least get mild / average results? Possible yes.. 

Ok, I think you should have got my point already.. It's just a matter of perspective / resources and motivation to try something out.


----------

I think they should work.. You won't get as much power as from lipo's, but you should be able to pull, let's say these 400-500w out of them, and if they do work in parallel with lipo's, that may improve their chances even more..As someone already suggested, peak amp draw was around 30-50a.. So, if you do use your board only on flats and don't speed it / accelerate it nonstop, you should be able to get at least a mildly satisfying result.. Some people are still using lead acid akkus. (e-scooters, old type e-boards).. their distance and speed sucks in comparison what ppl achieve with lithium akkus.. but there were and probably still are ppl who use such tech.

It is a matter of application and experimentation. I still have not seen a comprehensive chart of how many amps does a motor / system needs, at what movement speed, rider weight, wind speed, rolling resistance and other parameters.
```

---
## \#56 Posted by: edwardlui531 Posted at: 2016-07-10T04:12:14.800Z Reads: 80

```
After thinking about safety and practicality, I think I am just going to build a 18650 battery bank and have a switch to charge the lipo when the lipo is low. But no charging while riding since I think that will kill the lipo even more.

Kinda like how you carry a battery bank for you phone when it runs low.

My dad even have a crazier idea. Having a foot switch that switch to lipo, kinda like a turbo. Thats sounds too cool
```

---
## \#57 Posted by: Okami Posted at: 2016-07-10T07:29:16.470Z Reads: 78

```
I think the idea is not that bad, only downside is that, it is recommended that the li ion pack has lower capacity than lipo's, for it to work great, at least that's what Rogers from diydrones.com recommend.

> If you do use different capacity batteries try to make sure the smaller one has a higher internal resistance.

Which makes it kind of difficult to implement, since it would be easier the other way around and build a larger liion pack (low discharge, lots of extra batteries, if they come from laptops).

If you do come closer to making some of this work, report back so we know how it went!
```

---
## \#58 Posted by: edwardlui531 Posted at: 2016-07-10T07:32:31.265Z Reads: 80

```
[quote="Okami, post:57, topic:5705"]
Which makes it kind of difficult to implement, since it would be easier the other way around and build a larger liion pack (low discharge, lots of extra batteries, if they come from laptops).
[/quote]

this is why I might add a resistor to limit the current
```

---
## \#59 Posted by: Okami Posted at: 2016-07-10T07:47:59.411Z Reads: 93

```
http://www.rcgroups.com/forums/showthread.php?t=733543

Someone tossed in another idea - to think about cooling. 

And someone also told that these discharge rates seem to be conservative, which just means, that the battery will be able to put out more amps, perhaps won't last as long (higher discharge, lower capacity).

 I think if you can push out similar life cycles out of li ions compared to lipo's and you have gotten these batteries for little cost, then why not.. (another point, why try to make this work)..

So yeah, we are not the only one's who have though about doing this..
--
Edit:
Another resource, where it seems someone has already done this:
https://jacklithium.wordpress.com/2013/12/22/mixing-battery-chemistry-li-ion-and-li-po/

(have not read all of it yet)
```

---
## \#60 Posted by: Hummie Posted at: 2016-07-10T08:34:05.987Z Reads: 90

```
This last link is about mixing in series, which I'm doing with 5ah 30c and 4.5ah and 90c.  12s, 3 and 9, and can't find info on this connection other than the one u also found.  I think I'd be ok in parallel right?  Nothing gets warm.
```

---
## \#61 Posted by: Okami Posted at: 2016-07-10T08:42:49.987Z Reads: 91

```
Not entirely sure, still new to all of this also.

Maybe this might clear something up:

> In paralell connections, different chemistry OK, different ah size OK but best if not hugely different. Different voltage, Not OK. Voltage can be a little off, like the difference between 24v sla and 24v lifepo4.

> Series connections, Idealy eveything the same except for voltage. Some have gotten away with different chemistries but whether it works or not depends on how similar the internal resistance of each one is. Different voltages are ok, like a 24v with a 36 v.

> In general, paralell connecting is not too fussy, but series is. In paralell, a weaker battery will not put out 50% of the current. The stronger battery will pull more amps and the weak one less, till they both run out at nearly the same time. Some chemistries like you to stop sooner that others though, so for example, a nicad and an sla together is likely to hurt the sla more if the whole pack is discharged 100%. Or a lifepo4 could have a higher bms cutout, and leave the paralelled sla carrying it all at the end.

Taken from: 
https://endless-sphere.com/forums/viewtopic.php?f=3&t=12537
--
Perhaps you could charge one pack to just only 4500mah, you would lose 500mah, but at least they would be more similar.. I think someone mentioned it would be great to stay between 200mah difference in capacity and not go higher.
```

---
## \#62 Posted by: laurnts Posted at: 2016-07-10T10:02:32.843Z Reads: 79

```
I agree with no voltage difference. That should NOT be used. So li ion lipo setting would be like combining space cell 36v which is known for 10s4p li ion with a 9s1p lipo.

Seriously changing liion and lipo on the go wouldnt matter so much like a turbo. Doesntworklikethis.com

Provide each battery setup with higher amps discharge with more parallel connections would do the trick. Electric drive is not a combustion that can benefit from turbo. The turbo of electric drive is a big capacitor, as they can discharge so high in short amount of time. The bigger the caps, the more boost youll have. My caps can hold so much power that enable 2seconds rapid acceleration. So you can feel the power climbing short steep road incline or burst power during stating off.
```

---
## \#63 Posted by: PB1 Posted at: 2016-07-10T12:24:40.908Z Reads: 79

```
I'm not agreeing with 2) made by Roger sterling.  

Two components in parallel have the same voltage.  So if the smaller battery pack is drained it will drop voltage which makes the larger battery pack provide current that will charge  / re-balance the smaller pack.  

(I've stated that I neglected the voltage drop created by the internal resistance  which has an effect under load.  When the load lessens the balancing will start) 


 You can't overdrain one battery in parallel while the other still has juice.  In series this is a different story.  

One thing is clear : if you go with a setup as described by the OP you have to know what you are doing and you have to monitor your batteries.  

It will work though similar to a capacitor.  The lipo providing the amps for aggressive riding,  the lions providing the range. I'm fully in line here with  @laurnts.
```

---
## \#64 Posted by: Hummie Posted at: 2016-07-10T16:57:29.948Z Reads: 75

```
From my looking into capacitors supplying burst power, caps do behave like that I general but I found a lot of evidence stating you can't get more instant power from bigger caps.  Scorpion sells their power bank capa but I hear it's marketing bunk
```

---
## \#65 Posted by: Hummie Posted at: 2016-07-10T17:01:02.631Z Reads: 75

```
With the parallel connection of dissimilar cells it seems u want the weaker cells to have more juice to compensate, I think maybe the same helps for series.  The weakest series linked cell I guess takes the most beating? How does that work?
```

---
## \#66 Posted by: Okami Posted at: 2016-07-10T18:23:04.924Z Reads: 85

```
Not entirely sure. What comes clear now is that it is hard to speculate about any of this any further and some tests should be done. Will see how it goes when I get the chance to test and assemble my liion pack. Though, it might still take a month till I get any sort of results. 


[quote="PB1, post:63, topic:5705"]
You can't overdrain one battery in parallel while the other still has juice.  In series this is a different story.
[/quote]

I think we could replicate this on smaller scale and see what happens. 

Do you know anyone who already used different capacity batteries in parallel? I do believe this should work ok, when there are little difference between capacities.. but what about when one pack has 5000mah and the second one 8000mah? Will one battery be able to charge the second one while also supplying current for the load? If someone can explain this process and how it should work, then that would shed some clarity on this, whenever it would balance/charge the second battery or not.
```

---
## \#67 Posted by: Okami Posted at: 2016-07-11T20:33:10.319Z Reads: 82

```
Some more info about the topic:

Taken from:
http://www.candlepowerforums.com/vb/showthread.php?407738-Mixing-batteries-18650

_Post author: magellan_ 
_ / 09-07-2015, 11:49 PM #6 / _ 
_Knowledge Credit goes to: ''mattheww50 and mdocod'' from candlelightforums.com_

> Default Re: **Mismatching chemistries question**
> If the **cells are in series** in that flashlight, then you need some sort of protection to prevent any one or more cells from being completely discharged, or reverse charged by the others. 
This applies whether or not the cells are the same or not, but obviously, with a cell mismatch, global cell-by-cell protection (or every cell in the bunch being individually protected) is even more important than it otherwise would be. As long as all the cells in series are rated to handle the current that the flashlight draws, and each cell has its own protection (provided either by a global or built in device) to kill the circuit when discharged, then mismatched cells wouldn't be too big a deal. I don't really know what Mathew is talking about above there, there is no "forcing" issue here. The resistance of all of the components in the circuit adds up, including all of the cells in series, and the final flow of electrons from the battery is voltage/resistance=current. The current flowing will be the same across all the cells in series. The cells with higher resistance will drop more voltage then those with lower resistance, but this is only a problem if the rate at which energy is dissipated in the cell causes a thermal problem, which, shouldn't be a concern if all of the cells in the pack are indeed a good match to the load in the first place. 


> That's all pretty academic at this point. If your flashlight employs 18650s in series, then global-cell-by-cell protection or individual cell protection is highly recommended regardless of whether the cells are the same or not, and the mismatch just creates a much greater demand for individual cell protection. I would not want a flashlight that runs a bunch of any lithium chemistry cells in series without over-discharge protection on every cell. 


> --------


> If the **cells in the light are all in parallel**, you may have more wiggle room to get by with mixed cells without concern, but I would still have some concerns...


> The current flowing from each cell in parallel, will NOT be fixed like it is when they are in series. Cells in parallel with different internal resistance and capacity, will always remain nearly "balanced" in terms of voltage, but that doesn't always mean they will be balanced in terms of state-of-charge, and doesn't always mean they will deliver the same current under a load. Though most of the discharge, the minor variations in current flow from mismatched cells in parallel would likely be a non-issue between "similar" cells. The problem is towards the end of the discharge, especially if the flashlight has boost regulation to maintain constant brightness. If it does, then the highest current load, could wind up coinciding with a condition where some of the cells in the pack are effectively drained, while others still have lots of energy left in them, and those cells which had higher capacity, could wind up forking over 2-3X the current expected towards the end of a discharge as a result of this mis-match in discharge characteristics between cells..


> Consider the following:


> - http://lygte-info.dk/review/batterie...comparator.php


> Lets assume these 2 cells were in parallel, discharging together at ~6A total, or ~3A per cell. Things would be fine from ~4V down to ~3.3V under a load, but below that, what happens? Suddenly, the NCR18650B has all this capacity still available below 3.3V, while the other cell is "dead," thus, the NCR18650B winds up delivering all 6 amps for the remainder of the discharge. 


> Now, if the cells being "paired" in parallel (or in your case, "quaded"), have similar discharge profiles, and plenty of headroom between the load and max current rating for the cells, then mixing cells in parallel is far less of a concern, even if they are a bit different. If the flashlight in question has a boost regulator, then mismatched cells are going to see more "abuse" towards the end of a discharge than matched cells. Something to keep in mind.
> -Eric

> Default Re: Mismatching chemistries question
> Quote Originally Posted by RetroTechie View Post
> Oooohhh... then there is no problem, right?


> With mixed cells in parallel, there is no chance of cells driving one another into polarity reversal, all cells produce the same voltage, and higher impedance cells just deliver a smaller % than their "fair share" of total current. And with the smaller current delivered, self-heating drops too. The cells that take the bigger share of total current, are precisely those cells with the lowest impedance (lowest self-heating @ same current).
> The cell that will wind up delivering the highest average current through a discharge in a bank of mismatched parallel cells will be the cell with the highest capacity, not necessarily the cell with the lowest internal resistance. Granted, at certain times during a discharge, a lower resistance lower capacity cell may run slightly higher current, but on the overall, the highest capacity cell has to discharge at the highest rate...


> To help understand this. Imagine placing an IMR18500-1100mAH cell with 60mOhm resistance in parallel with an NCR18650B-3400mAH cell with 110mOhm resistance and discharging the pair. 


> Think about how that discharge would go, considering that they are effectively "locked" to hold similar states-of-charge through the discharge. Which cell would deliver more current? 


> After pondering that a bit, it should be pretty obvious that the 3400mAH cell will wind up averaging ~3X higher current than the 1100mAH cell when discharged in parallel. Capacity trumps resistance in this situation, and even when the difference in cells is narrower, the same will remain true. 


> ....any cell rated for 10A continuous could do that on its own, and stay within spec. So even the worst case is okay, adding more cells just increases runtime, and reduces stress on each cell. And even increases efficiency (slightly) because less of the cells' energy is wasted in internal impedance.
> Yes, if the light draws UP TO 9A, and the cells are all designed to run up to 10A, then it should be a non-issue.

I think the best bet would be to go with bms / pcm to monitor / shut off, if any of the parallel packs starts to act weird..

Found this comprehensive resource of different types of bms / pcm's:

http://liionbms.com/php/bms_options.php

--

Resource for gaining more insight into batteries (unbalanced including):

http://liionbms.com/php/white_papers.php
```

---
## \#68 Posted by: Okami Posted at: 2016-07-13T15:02:27.183Z Reads: 68

```
Will try not overhelm the topic but been reading a lot lately concerning battery making and this is what I found related to mixing batteries. 

It partly gives some clues about that resistance thing and suggests using different gauge wires.

He used lead acid / lifepo system, so the requirements for lipo/li ion might be a little bit different.

> **''Mixing chemistries for most economic performance and range''**
> _Postby Aerowhatt » Sat Mar 07, 2009 4:49 am_

> Just a note about resistance and paralleling two non matched batteries. If they are both conected to the load then having resistance in between one of them and the load isn't as bad as it seems. Intuatively adding resistance produces alot of heat and wastes power. This is very true in a single source system. But with dual sources the system just askes more of the second source of power rather than forcing the power through the resistance causing a large loss to heat. 

> Similar to the difference between adding resistors in series and adding them in parallel. The results are very different! For example on my motorcycle which has some pretty large peak amp demands. A direct paralleling of the LiFePO4 with the SLA's using the same guage and length wires would yield higher than desired peak loads on the LiFePO4. A simple solution is to use smaller gauge cable for the LiFePO4. So that at the controller (or junction of the two batteries) it's voltage drop is more than it otherwise would be. Intutition jumps to the conclusion that the wires would heat significantly and waste power. Why, because if you add resistance and have to pull the same amount of power you get a big voltage drop and an increase in amps resulting in hot cables. What intuition forgets is that there is another source of power (similar to parallel connected resistors)! So rather than FORCE the higher resistance line it pulls from the other one. Basically it doesn't take much additional voltage drop on the LiFePO4 to get the SLA's to step up a bit more and give a more ideal balance of current delivery during peaks loads. So if you have a dual battery system that is naturally pretty close to each performing where you want them too. Changing the harness resistance of either, or both batteries to fine tune it results in a very low loss. 

> In the case of the motorcycle going from a 6ga cable to 10ga cable on the LiFPO4 fine tuned the balance of load for each battery with only a 3 degree F increase in the harness for the LiFePO4. Arguably this is less loss than the losses associated in throttling that battery with electronics would be. With the added advantages of no additional cost or complexity.

> Aerowhatt

Taken from:
https://endless-sphere.com/forums/viewtopic.php?p=138760#p138760
```

---
## \#69 Posted by: Okami Posted at: 2016-07-16T07:44:17.435Z Reads: 73

```
Hello everyone! A topic about what is the real amp draw / current needs for a system surfaced on another topic.

I think users would benefit, if they could know more precisely what their current needs are, when designing their battery setup!

---

So, gladly @DeathCookies made a simple template for everyone to enter their data into.

Any feedback / improvements would be great, as I think it is still possible to be changed and should be improved.

----

Poll for entering Amp draw data:
---
http://gct-hp.de/esk8/index.php1
---
<img src="/uploads/db1493/original/2X/3/3ad8a772101ce4dca252a38fe56363a198646db7.png" width="300" height="300">

---
Feedback can be posted here: 
http://www.electric-skateboard.builders/t/custom-poll/6171

---
I apologize for ''kidnapping'' this thread with so many replies, but the text would be just unreadable, if I posted all of that info in one reply.
```

---
## \#70 Posted by: Michaelmccarron Posted at: 2016-10-02T02:21:30.631Z Reads: 55

```
Hello, 

I just thought of this very idea, how ever, instead of putting the two batteries together in parallel, what if you had the two batteries working together, with the addition logical piece of hardware that dictates when each battery should be used. e.g. When cruising the power source would be li-ions and when you need a burst of power it switches to the lipo??
```

---
## \#71 Posted by: Okami Posted at: 2016-10-02T09:14:34.949Z Reads: 51

```
I think someone has suggested this idea also, the guy who mentioned it called it booster switch or similar.

 I think it could be tried with some high amp switch or a smart switch where you hook it up to a receiver or install a foot switch somewhere on your board. 

This could perhaps work better than running with mixed lipo and liion all the time.
```

---
## \#72 Posted by: paul1 Posted at: 2016-10-02T11:07:21.869Z Reads: 53

```
i have mixed different battery types and have had no problems with this, just kept the voltage the same of course,
```

---
## \#73 Posted by: paul1 Posted at: 2016-10-02T11:09:46.820Z Reads: 53

```
the link doesnt work (amp draw data),
```

---
## \#74 Posted by: Okami Posted at: 2016-10-02T12:07:50.003Z Reads: 53

```
the new link for esk8 board database is here:

http://ej.uz/e8base
---
Although, we are still improving the database so we have not had the chance to massively start inviting people to join and post & share their eboard data there.

---
We plan to start inviting more people there, once we have finalized the design and some extra features for the page.
---
```

---
## \#75 Posted by: Okami Posted at: 2016-10-04T18:29:44.073Z Reads: 53

```
As of right now, I've only seen reliable amp draw data from about 3 users. 

One of them (I think @whitepony pushed till about ~80A but I think he was going crazy fast.. (over 40km/h / +25mph)..
```

---
## \#76 Posted by: Maxid Posted at: 2016-12-02T05:11:01.638Z Reads: 50

```
This test is from 3years ago. https://www.google.de/amp/s/jacklithium.wordpress.com/2013/12/22/mixing-battery-chemistry-li-ion-and-li-po/amp/

It will work just like @PB1 said.

@PXSS do you have some experience with this? I am planning to make one large 6S battery out of 6S4P 25Rs and two 3S 5000mAh Turnigy Lipos.
```

---
## \#77 Posted by: PXSS Posted at: 2017-01-22T20:59:14.235Z Reads: 47

```
Eeek. Mixing chemistries isn't a good idea. I'll think about it a little more after the football game
```

---
## \#78 Posted by: PXSS Posted at: 2017-01-23T06:00:04.138Z Reads: 50

```

LIPO VS LI-ION
I don't know much about the subject as I am not a chemical engineer and the stuff being explained to me went way over my head when I took a 4 hour crash course from an actual battery chemistry engineer with a PhD and several years of experience but here is the main takeaway. 

You can produce a high power/low energy cell (VTC6) or low power/high energy cell (Sanyo GA) out of the exact same chemistry by varying the ratios of the chemicals inside the cells ever so slightly (we're talking 1-2% changes).

Now, these are kind of sheets coated in chemicals and stuff. You can either roll them up as tight as possible and stick them in a tube, 18650 style, the advantage of this is that you get more contact surface between sheets and therefore you can have a more energy dense cell or you can lay them flat in layers in order to have slim packs that can be shaped in a thousand ways.

The bad thing about rolling the sheets into a tube is that you do not get as much heat transfer to the outside so you're limited as to how much power you can run through them before the chemicals start degrading due to heat and reacting too fast. 

The sheets on the other hand have the same reaction occur over a larger volume so the heat is dissipated better and the chemicals remain happier which is why they can produce more power. 

That is abouf as much as I remember without going into excruciating details. 

All of this of course has an effect on the voltage operating range, internal resistance and therefore discharge curves. So based not only on the chemistry but also packaging, your internal resistance can vary throughout the discharge cycle. The internal resistance is a direct product of the chemical reaction. 

Internal resistance is NOT a constant. Not within a single discharge, nor at the same point of the discharge on different cycles. It is always rising as the chemicals brake down. 

The problem with mixing Lipos and Liions in parallel then becomes who is providing more power, why, and is it exceeding the safety limits at ALL TIMES. 

The internal resistance of LiPos is lower than Liions which is good, it means that they'll carry the larger current for the same voltage drop. The problem arises when LiPos reach ~3.4V and their internal resistance is almost the same if not higher than that of a liion at the same voltage which means the power distribution is equal or slightly higher on the liions. Are you harming the liions at this point? 
What about in 10 cycles, do you know what the internal resistance of each cell is then? How about in 50 cycles half way through the discharge curve? 
If your LiPos deteriorate faster than your Liions then they would have a higher internal resistance and you could be harming your Liions. 

It's a very slippery slope and unless you know exactly what you're doing, I'd recommend against it. 

I do however think that you could run on LiPos during high power conditions and then switch over to Liiions on cruise conditions. My company is working towards this in the future with the exception that we would use a fuel cell in combination with a gas engine instead of liions and lipos. But the end goal is similar. 

Your controller would be connected to both power sources and based on the power draw, you could choose power source A or B.

I could write more on the subject but have a flight test scheduled in a few hours so I'm calling it a night.
```

---
## \#79 Posted by: Okami Posted at: 2017-01-23T10:07:37.399Z Reads: 46

```
Thanks for posting this! I think we could finally make a ''summary'' with all the info you have already told on this forum about batteries!

Had one question though, you mentioned this:
[quote="PXSS, post:78, topic:5705"]
If your LiPos deteriorate faster than your Liions then they would have a higher internal resistance and you could be harming your Liions.
[/quote]

So do you really agree here that lipo would detoriate faster than li-ions? I understand that in this ''application'', where both of them might be working at the same time, the lipos would be the ones which would take the most ''load'', so it would be logical to assume they detoriate faster than the li-ions only because of the size of the load.. 

But anyways - I still have not found a source for a good lipo vs li-ion comparison as im not sure how both of these ''chemistry compositions'' work in the long run, if they are discharged / charged in the same way..

You told it very good about the ''layout of layers'' in a battery - for lipo vs li-ion. The physical structure of the battery itself gives it its attributes when it is operating.. that is why we could sort of say that lipos ''dont heat as much as li-ions'' or that their heat dispersation is just way better because of the somewhat bigger volume.

Anyways.. some good stuff you got there.. I wished more ppl would get the chance to speak with battery chemical engineers like you did :D

--

I think you should agree that there are ppl runing mixed chemistry setups.. they just monitor their cells better and for newbie who does not know the difference between 3.4v and 4.2v, of course, you wont let him run both of them in parallel.
```

---
## \#80 Posted by: Maxid Posted at: 2017-01-23T11:02:15.032Z Reads: 42

```
I get that it might be damaging the cells when the load exceeds the limits the batteries are rated for - but that is true no matter if they are mixed or not. Shouldn't a parallel setup like this always be better than the single packs?
I mean when you have a load of say 100A and you only use the Liion pack it will not be healthy for it.
The same is true for the Lipo. Combining them in parallel however should make it at least healthier for them to supply the 100A (the load obviously doesn't double just because you use two packs in parallel). 
Isn't it also like having a charger with you the entire time? The Lipo will supply the high currents and in times of little load the Liion will actually "charge" the Lipo back to an even voltage across the packs. 
Could it maybe even make sense to hook the single liions to the balance wire of the Lipo? Say having multiple 1S4P Liion packs hooked up to the balance leads charging the Lipo while riding and supporting the cells in case of voltage sag.

I also agree that the voltage cut off needs to fit to the Lipo - so you lose some capacity in the liions but that should still be less than what you gain by adding the Lipos to the system, no?
```

---
## \#81 Posted by: PXSS Posted at: 2017-01-23T13:01:10.381Z Reads: 40

```
The thing is you dont know what happens to the internal resistance of both packs at lets say "100Amps", the power could be split evenly, or 4 to 1, or 8-1. The liions do not act as a charger, not really how that works. They just provide as much power as is needed to keep both cells at the same voltage. 

I'm not sure what would happen when you unload the system, but you could have current flowing one way or the other. If the load is big and you shut it down instantly, you might get a massive inrush from one cell to the other which could be fine or devastating for the liions. The best thing you could do is unload the system as slowly as possible (not going from hard acceleration to cruising or braking) as to give the batteries more time to stabilize lower voltage differences. 

The reason I say it could be totally fine is because maybe a load of 0.01A increases the internal resistance of one cell enough to balance the voltages. 

Point is I don't know what happens, and my OCD just screams dont do it unless I absolutely 100% know that there are no adverse effects and understand what is going on. 

You may get more out of both worlds, I would not call it the best of both worlds. By stopping Liions at 3.4V you waste 20ish% of their rated capacity. The question then becomes, are they more energy dense (volumetrically or gravitationally) at that reduced capacity than a LiPo of equivalent volume/weight? I think not but I dont have the appropriate plots in front of me to make a better call. 

@Okami. 
I don't know which one deteriorates faster. Could be the LiPos, could be the Liions. Only testing would tell.  LiPos are made to handle higher loads than liions so it really is hard to tell.
```

---
## \#82 Posted by: Maxid Posted at: 2017-01-23T13:46:44.305Z Reads: 34

```
What about mixing 18650 cells in parallel?
What happens when you connect 4 25Rs and 4 30Q cells together in parallel? The internal resistance should differ as well so would this be similar to the Lipos?

This is super interesting and I just want to understand. If you have links for me to do some research on my own please let me know.
```

---
## \#83 Posted by: PXSS Posted at: 2017-01-23T14:11:08.192Z Reads: 36

```
Search modelling discharge of Lithium batteries. There are a few technical papers that describe the hardships of doing this and explain how the internal resistance is tied to the chemical reaction. It is all very complex stuff and might take reading over and over and over again to understand but it's something. There's really no substitute to just going to a chemical engineering department if you are still in school and talking to one of the professors familiar with the topic. They can shed way more light than I can. 

It's similar, yes. Same thing with mixing new and old cells. It's all possible but it doesn't mean you are not damaging the cells. 

The main issue with mixing Lipos and Liions is the lvc difference. If you do not set your limits right, you will eventually blow a cell and as we have all seen there are a lot of people trying to make these with absolutely no experience or understanding. Blowing up a BMS because you shorted a cell is very different than blowing up your liions or lipos because you weren't careful enough and just read that it was possible on some forum online. 

Lipo/Liion fires cannot be stopped with a regular fire extinguisher, you need a Halon extinguisher (which are very expensive) and even those usually have a hard time. So beware.
```

---
## \#84 Posted by: Okami Posted at: 2017-01-23T16:14:50.299Z Reads: 31

```
<img src="/uploads/db1493/original/3X/0/d/0d61e1961ea68ee91c4cbe1ea7f3882e1e89d859.jpg" width="690" height="487">

I think this one is a good example..

But I will get the chance I will make a translation for this.. I think this is a really good comparison
```

---
