# The next part of the build&hellip; BATTERY!

### Replies: 19 Views: 584

## \#1 Posted by: MrDGOrman Posted at: 2019-03-25T09:38:45.471Z Reads: 219

```
Hi everyone,

So the next part of my build is in progress. Once this is done it'll technically be "finished" although no doubt I'll add more/change things as I go!

If anyone knows any seasoned battery builders then please tag them in here!

Batteries. My current setup is 3 zippy batteries plugged together. Simple stuff really. Easy, effective, does the job. Issue I've got is range - I want to be able to go a little faster but I also want to have a good amount of range. I've heard the LeCroix has some pretty good range so I'd like to match it.

My plan was to make a 18650 pack in a 12s6p format.

What I was really hoping to know is if someone has this variation in their Hummie deck? It should fit because I bought the "double stack" enclosure type from @bigben but it would be really nice to see someone elses battery in the enclosure so I know what sort of space I'm working with.

**Target:**
* Achieve 30mph with ease. Could go faster if I really wanted to.
* Achieve 30 miles range with ease. Could go further with an "eco" mode.

**Parts advice:**
* I'd like to make each p pack into a "solid block" of some sorts. I've seen these orange clip things that you plug over the cells - what are these called? I don't mind doing the welding but if I could wrap these caps around the ends of the cells it would make life much easier!
* What BMS do people recommend? I was going to go for this one from eskating but it's only advertised as being suitable for 4/5p. I have the 10s version already and I like that because it has an eswitch built in. I'd like to keep that feature if possible! https://eskating.eu/product/12s-bestech-bms-80a-12s4p-5p/
* Insulation options. What options do people recommend?
* Cable rating. I was going to go with 10awg if I had to weld it all together but if I get the clips what would be recommended? Maybe a braided strip of some sort? I don't want the battery to be restricted in any way.
* Due to the size of the battery - should I put inline fuses as a safe guard incase of a power surge or something? I swear I heard people were doing this now but wasn't sure. I don't want all my cells to explode due to a fault somewhere. I'd prefer to lose 6 cells than 72!

This is going to be my first battery build (other than the plug and play zippys). I'd like to make it as "user friendly" as possible.

Cheers,
Daniel
```

---
## \#2 Posted by: bigben Posted at: 2019-03-25T10:06:00.720Z Reads: 198

```
@sayekim has done a 12s6p in his I believe?
```

---
## \#3 Posted by: MrDGOrman Posted at: 2019-03-25T10:55:26.809Z Reads: 181

```
Nice thank you!

Do you know what them cap things are called and where I can get them? I want to make the job as easy as possible. Also don't want to go out and buy a welder!
```

---
## \#4 Posted by: goldrabe Posted at: 2019-03-25T11:04:13.743Z Reads: 178

```
@Winfly makes the orange compression pack modules and another variant would be the N.E.S.E modules. https://18650.lt
```

---
## \#5 Posted by: MrDGOrman Posted at: 2019-03-25T11:12:43.726Z Reads: 167

```
That's exactly the thing! A lot more expensive than I thought they would be though. Half tempted to buy a 3D printer and then make my own! Thanks for sending the link though.

Is there anyone on here that's able to help with the other questions I had? Fusing the P Packs etc
```

---
## \#6 Posted by: MrDGOrman Posted at: 2019-03-25T11:14:43.468Z Reads: 159

```
I've also found a 35E battery. Has anyone done a build with these? Has a large mAh rating but lower A rating..

https://eu.nkon.nl/rechargeable/18650-size/samsung-inr18650-35e.html
```

---
## \#7 Posted by: goldrabe Posted at: 2019-03-25T11:23:10.902Z Reads: 150

```
Yes the N.E.S.E. modules costs are the same as buying a spotwelder like the maletrics with all the supplies needed. Tab Insulation, Nickel strips, heatshrink etc. If you want cell level fusing then you have to weld your pack. For a 6P pack the 35E discharge is a bit on the lower side, you can draw only 60A continuous. However if you are not drawing that much they are usable. I do a 8P pack with them and plan to not draw more than 60A. In that way I hope to extend the cycle life of the pack.
```

---
## \#8 Posted by: MrDGOrman Posted at: 2019-03-25T11:54:43.327Z Reads: 138

```
I'll go with the 30Qs instead then.

I've found a pack on the NKON website which I'll order. https://eu.nkon.nl/vruzend-diy-battery-kit-v2-0.html

I'm now wondering if I should go further and make a 7p pack instead!
```

---
## \#9 Posted by: goldrabe Posted at: 2019-03-25T12:03:35.032Z Reads: 138

```
The vruzend pack can not handle high currents and is awful to assemble. I would not recommend it. I personally bought the N.E.S.E modules but think the compression packs from @Winfly are equally good, he can do staggered custom shaped modules, it might be worth shooting him a pm.
```

---
## \#10 Posted by: MrDGOrman Posted at: 2019-03-25T12:36:20.779Z Reads: 135

```
When you say they cannot handle high currents what do you mean by this? It looks to be exactly the same format as the NESE ones but the NESE ones are in a solid box. The benefit I see with the vruzend ones is that I can add more cells to each P Pack if I wish.
```

---
## \#11 Posted by: MrDGOrman Posted at: 2019-03-25T12:37:13.192Z Reads: 133

```
Does anyone have any recommendations for chargers aswell? I'm trying to find a silent charger that does fast charging (4a).

Cheers,
Daniel
```

---
## \#12 Posted by: goldrabe Posted at: 2019-03-25T12:51:19.516Z Reads: 124

```
The V1.5 kit can only handle 3.5A continuous per cell. The V2 kit can handle up to 20A. The N.E.S.E modules are available up to 8P. One module is tested up to 200A if I recall correctly. The Vruzend kit leaves a lot of space between the single cells whereas the N.E.S.E modules fits the cells more compact. The Vruzend kit is also more cumbersome in a flat layout. Jehu Garcia tested the vruzend kit on his youtube channel and could not apply even pressure throughout his pack which lead the pack to getting unreasonably hot. Both designs I mentioned deal with compression better then Vruzend.
```

---
## \#13 Posted by: MrDGOrman Posted at: 2019-03-25T13:10:51.295Z Reads: 126

```
Surely a 20A testing is enough though, right? Otherwise no one would be using them..?

From what I can see based on one video, Jehu Garcia didn't like them because he struggled to fit them.

I'm so drawn to them because I can change the P Pack size as and when!
```

---
## \#14 Posted by: sayekim Posted at: 2019-03-25T14:51:07.826Z Reads: 123

```
[quote="MrDGOrman, post:1, topic:88206"]
My plan was to make a 18650 pack in a 12s6p format.

What I was really hoping to know is if someone has this variation in their Hummie deck? It should fit because I bought the “double stack” enclosure type from @bigben but it would be really nice to see someone elses battery in the enclosure so I know what sort of space I’m working with.
[/quote]

12s6p 30q

![image|666x500](upload://mHP8Qqozo0oJeKpA0qRqiJeo8hg.jpeg) 

![image|666x500](upload://2mxIwKF0DQLeH4CYUkkUwSiM7i4.jpeg)

I’m putting a 12s8p 30q in the next one
```

---
## \#15 Posted by: MrDGOrman Posted at: 2019-03-25T16:54:01.161Z Reads: 115

```
That's a really good picture to see how much space you have etc! How much space do you have between the battery and enclosure?

Good to know a 12s6p fits though!
```

---
## \#16 Posted by: sayekim Posted at: 2019-03-25T19:21:21.077Z Reads: 108

```
Don’t know. The battery compresses the padding when tightened down. 

Padding is this. 
https://rubber-stuff.co.uk/product/pvc-nitrile-self-adhesive-pad/

Under the battery I got 3m dual lock. 
€ 8,99 | 3M SJ3551 Dual Lock, Black Type 400 Mushroom Reclosable Fastener Tape Bacing VHB adhesive tape 3M tape (25.4mm x 2m) 
https://s.click.aliexpress.com/e/MlqMfrDdD

That battery isn’t going anywhere. 

The escapes and bms and wires aren’t held down by anything but the padding. I can’t tell for sure but it seems to stay in place.
```

---
## \#17 Posted by: MrDGOrman Posted at: 2019-03-25T21:16:02.797Z Reads: 100

```
Okay cheers mate. :slight_smile:

 @goldrabe I took your advice and went for the N.E.S.E modules. I'm hoping they're not delayed and arrive soon. Didn't get any kind of tracking or expected dispatch time or anything but I'm guessing I'll get an email from them when they've dispatched?
```

---
## \#18 Posted by: goldrabe Posted at: 2019-03-25T21:57:04.296Z Reads: 94

```
Wow man you are fast in decision making!
Are you sure everything fits in your cutout and enclosure? 
Better contact @agniusm and tell him which layout you want to do and have him look over your order that nothing is missing.
```

---
## \#19 Posted by: MrDGOrman Posted at: 2019-03-26T09:43:21.336Z Reads: 87

```
Well I want to get everything sorted so just made the order! I haven't measured everything up specifically but I should have more than enough space. If not I can always mod the board slightly to fit so no dramas in that department.

I don't think anything is missing but I'll message him anyways. I just ordered the entire kit so that comes with all of it. The only optional extra is the terminal caps but I've got something suitable for that already. I'm hoping they can be shipped pretty sharpish because my other bits arrive in under a week!

Cheers for the help boss. I'll post a picture once I've got it all set up :slight_smile:
```

---
