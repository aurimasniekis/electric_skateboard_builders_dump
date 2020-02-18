# Mountain Board &#124; MBS Comp 95 &#124; Matrix II trucks &#124; Dual SK8 6374-149KV &#124; ?Mount &#124; 8-12S &#124; Dual FOCBOX

### Replies: 24 Views: 2112

## \#1 Posted by: smikk Posted at: 2018-05-31T06:02:57.266Z Reads: 261

```
Hey guys, I built a longboard a couple of years ago on a Arbor Genesis 44 inch drop through with custom plasma cut mount, welded on to some trucks that were turned on a lathe etc. etc. I used the ESC from , and it runs 8s with a  270kv motor from the same place.

Things seem to have come A LONG way since I built that. I Love that board, but I am now ready to take it to the next level with a mountain board. I am starting to get some analysis paralysis here with all the options available now. Its a great problem to have, but it is making the decision difficult and a bit confusing for me.

I have not purchased anything yet (although I have a lot of 3s and 4s lipos from my other board and from an RC truck). I am holding off on purchasing stuff till I can make sure I get stuff that is all compatible. I don't want to buy multiples of the same thing.

Here is what i'm thinking so far:
Board - MBS Comp 95 (complete)
Trucks - Matrix 2 trucks with the complete
Wheels - Rockstar II wheels (8 inch) with the complete
Motors - Not sure, but I want dual motors
ESC - Not sure yet, but like I said, i've used the ESC from DIY skate and its its ok, but a little pricy. I have looked at the vesc, which looks very nice but unless i'm missing something it is 400 bucks by the time I get it here in the US. I would need 2 of those i think for dual motor. That is TOTALLY OUTRAGEOUS, i'm sorry... I would buy a baja board before dropping nearly a grand on 2 vesc's (sorry for the rant). Anyway, I have seen some other similar things mentioned in other threads, can someone recommend a good (less expensive) alternative to the vesc? 
Mount - I would prefer not to mess with welding and fabrication on this go around with the mount. It was a lot of work, and left very little room for error. My concern with some of the bolt ons is that things might get loose, or slide around and have play. Do people have issues like that? What recommendations do you all have for a good mount?
Pully - I have got as far as finding a pully on evolve, but that is only half the solution. It fits the rockstar 2 hubs which is good, but i'm not married to this. Ive done a lot of reading on chain vs belt, and honestly i'm still on the fence and could go either way. i I will say i would prefer torque (power) over speed. I crashed going 25 MPH on my longboard, and i'll never get going that fast again :) 

This site is a goldmine of great info, and great people from what I can tell so far. I'm very grateful to have found it, and looking forward to this build and hopefully some suggestions to get me going. Thanks!
```

---
## \#2 Posted by: telnoi Posted at: 2018-05-31T06:23:29.411Z Reads: 229

```
[quote="smikk, post:1, topic:57332"]
That is TOTALLY OUTRAGEOUS
[/quote]

check the certified focbox suppliers link at the very top of this page above the header and get a dual case for it from @Kug3lis
```

---
## \#3 Posted by: Trdolan03 Posted at: 2018-05-31T06:55:52.229Z Reads: 219

```
I paid just under $400 total from enertion for 2 FOC box and one year warranty on both. That includes shipping.
```

---
## \#4 Posted by: smikk Posted at: 2018-05-31T14:51:52.279Z Reads: 194

```
Great, thanks guys! I read a little about the FOC box last night. Is the most commonly used esc for mid to high end builds? It looks very similar to the VESC, but cheaper. 

@telnoi, what do you mean by dual case? Like a 3d printed case that holds both boards and replaces the plastic shell it is currently in?

Any suggestions for PCB? I've always just used a normal lipo charger, but I like the idea of having more permanent batteries in there with a smart charger.
```

---
## \#5 Posted by: telnoi Posted at: 2018-05-31T15:53:02.131Z Reads: 177

```
[quote="smikk, post:4, topic:57332"]
what do you mean by dual case
[/quote]

Click on his name and subsequently the link to his shop. You'll find it there.
```

---
## \#6 Posted by: smikk Posted at: 2018-05-31T19:56:31.478Z Reads: 166

```
Oh yeah, that is nice. Everything seems to always be out of stock.
```

---
## \#7 Posted by: smikk Posted at: 2018-05-31T20:01:25.810Z Reads: 175

```
Any opinions on these FOCBOX's vs something like this ESC from DIY?
collections/esc-speed-controller/products/torque-esc-bldc-electronic-speed-controller

Trying to understand the cost difference.

FOCBOX
Firmware: VESC
Peak Amps: 300
Amps: 60
Cost: 155

DIY ESC
Firmware: VESC
Peak Amps: 260
Amps: 50
Cost: 99


Any compelling reasons to get one over the other? I assume functionally they are the same since they use the same firmware.

Thanks!
```

---
## \#8 Posted by: clistpdx Posted at: 2018-05-31T20:29:56.727Z Reads: 170

```
I've been looking to build almost the same thing as you. Here's motor mounts i've been considering:
https://www.electric-skateboard.builders/t/motor-mounts-kits-for-trampa-atb-and-mbs-matrix-old-type-matrix-ii-ats/44749?source_topic_id=44815
and 
https://www.electric-skateboard.builders/t/aluminum-motor-mounts-for-mbs-matrix-ii-and-mbs-matrix-old-type/44830?source_topic_id=44815
```

---
## \#9 Posted by: smikk Posted at: 2018-05-31T20:45:50.167Z Reads: 152

```
Those look really nice, thanks for sharing. i'm hoping I can go cheaper than that to start, it looks like roughly 350 USD for a complete kit shipped to US. Are any of these designs that people know about open source? We designed the last ones we used on solid works and had a local guy water jet them out for us, and they were vastly cheaper. Maybe I can save some if I just go that route.
```

---
## \#10 Posted by: telnoi Posted at: 2018-05-31T20:46:48.265Z Reads: 147

```
[quote="smikk, post:7, topic:57332"]
Trying to understand the cost difference.
[/quote]

TB has a higher failure rate when used with FOC and 12s is questionable. Focbox uses upgraded components (higher voltage tolerances, parts making FOC more reliable) and is something in between the 4.12 and vesc6 design...that is the simple explanation. Search for upgraded bom list or similar terms if you want a deeper understanding.
```

---
## \#11 Posted by: telnoi Posted at: 2018-05-31T20:50:26.798Z Reads: 141

```
[quote="smikk, post:9, topic:57332"]
We designed the last ones we used on solid works and had a local guy water jet them out for us,
[/quote]

Should be easy enough if you can prototype with a 3d printer. Matrix 2 trucks has a relatively easy shape to clamp on to.
```

---
## \#12 Posted by: smikk Posted at: 2018-05-31T21:07:18.599Z Reads: 139

```
> TB has a higher failure rate when used with FOC and 12s is questionable.

Do you mind explaining what TB is? Also, do you mean 12S is questionable with FOCBOX or with the DIY Electric Stake one? That one says it does 14S, but I don't have plans at least not at the moment to go that high.

Thanks!
```

---
## \#13 Posted by: telnoi Posted at: 2018-05-31T21:18:16.018Z Reads: 136

```
Tb = torque boards.
Questiontable with the tb vesc due to parts with a lower voltage rating.14S is nice marketing Blabla.
```

---
## \#14 Posted by: smikk Posted at: 2018-05-31T21:23:03.985Z Reads: 148

```
> Tb = torque boards.
Questiontable with the tb vesc due to parts with a lower voltage rating.

Thanks, sounds like i'll go with a FOCBOX setup then!

I'll see if I can find some open source mounts for Matrix II trucks.

What motors do people suggest? I got the TB motor, and i've had issues with it. Maybe unrelated to quality, not sure.
```

---
## \#15 Posted by: Deckoz Posted at: 2018-05-31T21:25:29.212Z Reads: 147

```
Hey man @hyperIon1 has some focboxes

https://hyper-ion-systems.myshopify.com/collections/esc-vesc-contollers/products/focbox-vesc-brushless-speed-controller
```

---
## \#16 Posted by: telnoi Posted at: 2018-05-31T21:26:14.643Z Reads: 139

```
Been running the cheap ass SK3 149kv hard and off-road in mud/rain/stones for about 2000 km. I'd recommend getting the newer brother, sk8 6374 sensored if you are on a budget. Plenty of torque.
```

---
## \#17 Posted by: smikk Posted at: 2018-05-31T21:45:04.572Z Reads: 138

```
[quote="Deckoz, post:15, topic:57332"]
Hey man @hyperIon1 has some focboxes
[/quote]

Oh perfect!

Have you ordered from them? They weren't in the list of focbox sellers on this site, not sure if that is a concern or not. Also, are all these places selling the same exact FOCBOX? Or does the hardware versions differ at all from one place to the next?
```

---
## \#18 Posted by: Deckoz Posted at: 2018-05-31T21:45:41.175Z Reads: 132

```
It's the same exact focbox they are a reseller.

I have ordered from them.
```

---
## \#19 Posted by: smikk Posted at: 2018-05-31T21:47:39.809Z Reads: 136

```
[quote="telnoi, post:16, topic:57332, full:true"]
Been running the cheap ass SK3 149kv hard and off-road in mud/rain/stones for about 2000 km. I’d recommend getting the newer brother, sk8 6374 sensored if you are on a budget. Plenty of torque.
[/quote]

Thanks, that helps a lot. something like this? https://hobbyking.com/en_us/turnigy-sk8-6374-149kv-sensored-brushless-motor-14p.html

If this is considered budget, what would be something on the other end of the spectrum for motor that I could compare against? I think this would do the trick, just curious what it might be missing that a more expensive one would have.
```

---
## \#20 Posted by: smikk Posted at: 2018-05-31T21:48:31.402Z Reads: 139

```
[quote="Deckoz, post:18, topic:57332"]
It’s the same exact focbox they are a reseller.
[/quote]

Thanks man, great find! I might get a mount from them too.
```

---
## \#21 Posted by: clistpdx Posted at: 2018-05-31T22:50:51.688Z Reads: 137

```
[quote="smikk, post:9, topic:57332"]
i’m hoping I can go cheaper than that to start, it looks like roughly 350 USD for a complete kit shipped to US.
[/quote]

This one looks to be under $200:
https://www.electric-skateboard.builders/t/all-terrain-electric-mtb-motor-mounts-for-mbs-and-trampa-trucks/56694/3
```

---
## \#22 Posted by: telnoi Posted at: 2018-06-01T06:23:05.929Z Reads: 127

```
[quote="smikk, post:19, topic:57332"]
what would be something on the other end of the spectrum
[/quote]

https://buildkitboards.com/products/6374-190kv-motor, though would choose in between 149-170kv.
Or
MTO6374-170-HA-C

Only difference is stator size, where sk8 is something along 598x and the above mentioned closer to true 6374. Bearings are most likely to be different, but I don't know what's inside of the sk8. All are (semi) sealed keeping the dirt and stones out.

You would gain a bit of performance choosing the alternatives to the sk8, but for me personally the sk8 would deliver enough power at a total weight of 130kg including equipment. I don't ride flats either.

You can go stupid power by going 6384. Alien power system sells these, though they are all maytech rebrands.
```

---
## \#23 Posted by: ervinelin Posted at: 2018-06-01T06:52:23.983Z Reads: 118

```
![IMG20180529153502|281x500](upload://zCq2M2CPM6tSc3fLbj9kvZoZ0Pt.jpg)

Opensource? You mean like these? After I test I will likely share them... but it's plastic so durability and reliability are questionable... Again need to ride to know, waiting for my deck to finish the build.
```

---
## \#24 Posted by: smikk Posted at: 2018-06-01T15:52:42.341Z Reads: 112

```
[quote="ervinelin, post:23, topic:57332"]
Opensource? You mean like these? After I test I will likely share them… but it’s plastic so durability and reliability are questionable… Again need to ride to know, waiting for my deck to finish the build.
[/quote]

Wow, cool! I'm in the process of finishing my 3d printer, so eventually stuff like this would be an option. Thanks for sharing your idea, i'm interested to see how well it holds up!
```

---
