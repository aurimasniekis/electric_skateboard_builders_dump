# 3-wheeled electric longboard

### Replies: 25 Views: 4249

## \#1 Posted by: cricrithezar Posted at: 2017-03-11T22:46:37.178Z Reads: 304

```
Thought I'd share a little project that I've been working on for about 6 months just to first kinda show off this cool design and maybe get a bit of feedback from people who've tried similar builds before (or even concerns from people who haven't, I'll post my main concerns and why I think they won't be an issue or why I can live with it).

Anyways, before I bore you with the specifics, here's a quick render of the build, with a screenshot of the CAD model. (the front truck is not mine and is just there to look nice. I'll just use an off the shelf longboard truck and deck):

<img src="/uploads/db1493/original/3X/e/2/e2936eeed2756a06ad495dfe63546302b62906d2.png" width="672" height="500">

Anyways, I'll quickly go over the components:

_The biggest component here is the battery pack. I really wanted to keep them hotswapable (because I'm kinda international-ish, and I have no idea where I'll be after university so I'd like to be able to bring all the batteries with me so I went with 18650 battery holders (didn't want to go with lipo pouches, though now that I think about it that might have been safer than soldering my own pack together), that will be holding 40 LGHE2 (or HE4, I forget), giving me a 10s4p, 37V nominal 10Ah capacity pack. This cost about $200 and is the most expensive "component" of the board
_Next we have the ESC, cheapest (new) VESC I could find was the 4.12 version from diyelectricskateboards for $99.99
_Then to power my wheel I'm going to order a Turnigy SK3 168kv motor from hobbyking for about $80
_I'll be using a 10s bms to charge all the batteries (at only 2A, the highest small-ish power supply that was 42v), which should charge ii in about 5 hours. It's only used for charging and balancing though, couldn't find one that would handle the high currents without costing significantly more. About $20 for both the BMS and power supply.
_I'm using a Fuzion 110mm kick scooter wheel (was supposed to be 100mm, ordered the wrong one, but the design allowed for switching if I wanted a bit more speed instead of torque). With a 3:1 gear ratio using HTD5 16mm found on ebay (36T:12T). The wheel uses the original bearings and the gear is mounted directly to the wheel, There's a picture of a 3d printed gear lower in this post, but the gear shattered when I dropped it two seconds after taking the picture, I'll be machining the aluminum one. Total for both the wheel and the gears and belts ~$45.
_The shaft holding the wheel was actually the biggest issue. With mechanical parts such as the wheel, I wanted as big a factor of safety as possible (anything below 7 static FOS kinda worries me considering how fast this board can go, that it's carrying me, and that I have to take fatigue into account as well as vibrations), which actually was causing really big issues when running FEA in solidworks. The stainless steel 8mm shaft was failing (not failing failing, but way too low FOS, can't remember exactly, but it was maybe around 2.5-4 for only half my weight). So that had me kinda worried but luckily, they make 8mm tungsten carbide shafts meant for mills or some kind of machining equipment which gave me a factor of safety of 9! That was only $20 shipped from Israel too so that was cool.
_ The mounts are plain old 6061 aluminum, FOS on that was like 20 so I'm not even worried, the only thing I had to change is make little stainless steel inserts to distribute the load from the shaft over a greater area, but those will be tiny steel parts, also machined in the university shop, not sure what the steel stock would cost, but the aluminum was only $35 and is big enough to allow me to mess up once.
_The motor mount is kinda boring, the nice thing about the three wheel design is the motor can be mounted directly to the board, which is really nice for clearance and looks. I tried 3D printing a mount and it turned out pretty nice, but I have no way of adjusting the belt and I might have to make a new part just for that.

Not sure exactly how much this would cost from scratch but my spreadsheet says around $650-$700 with all parts including board and controller ect.

Anyways, here's a picture of how big the holder is, and a rough idea how the other components will be layed out (still waiting on my VESC and have yet to order the motor):

https://goo.gl/photos/EN1DbuhMAZLYWNsh7

The specs:

Speed: 
_Because I'm getting 6200rpm, with a 3:1 gear ratio and a 110mm wheel, this means I should be getting up to 26mph on this board. And if I need any more speed down the road (which I really think I won't, I enjoy not dying) I can always switch the 12T for a 16T which gives me a lower gear ratio and 35mph max speed.
Range:
_Using the 14Wh/mile approximation gives me 26 miles (37V*10Ah/(14Wh/mile)).

My main concerns:
_The first one was my biggest concern, which is stability. This is a completely different design and could cause instability and wobble. However, after thinking about it, and seeing videos of other people's builds on youtube, I think that having a static wheel in the back might be the same as having a ridiculously tight back truck (like tighter than is possible probably), which means that stability should actually be better, especially at higher speeds. So I'll test it unpowered first, and hopefully it performs fine.
_My second concern is with the batteries, I've tested the resistance of the holders and seen people use the same holders for their electric scooters, but they're gonna be seeing a lot of current. I soldered copper wire as close to the contact point on the holder as possible (it's on top actually, so maybe 1mm of strip + contact resistance). I'm just slightly worried that my batteries might get hot. I'll test it and it it can't handle the current I guess I'll have to make packs (can you bring custom made packs on a plane?)
_Finally, my last concern is whether the board will twist since there's less support in the back. I know most of my weight will be in the front but I could see the whole board twisting and I'm not sure how that would affect it. If it looks too bendy though I'll just add aluminum square tubes or something, but that'll make it soo heavy. Anyways, I'd love some insight on that, otherwise I guess we'll see when I finish it.


I would really appreciate feedback and any concerns that you may have that I wouldn't have thought about!
```

---
## \#2 Posted by: Okami Posted at: 2017-03-12T00:02:34.844Z Reads: 245

```
Definately nice seeing that there is more interest in 3 wheelers.. wont be able to give much of a advice.. but I can comment about the batteries:

Im also interested on how it might be for transprting them.

Specially for this reason I made ''modular packs''. Each consisting of ~66wh pack (6cells).. they can be taken apart, though I would probably have to make some sort of 3d printed or other enclosure for them to look good.. since the connectors and extra hot glue might not look so good :D
```

---
## \#3 Posted by: cricrithezar Posted at: 2017-03-12T00:13:18.968Z Reads: 236

```
Nice, are they soldered together? What does the TSA have to say about homemade packs? The only document I've found only references "uninstalled" batteries, so I just assumed no mods whatsoever. If they don't mind DIY packs, I might solder them in small 1s4p (3.7*2.5*4=37Wh so I guess I could even go 2s4p) packs and have connectors to connect them in series.
```

---
## \#4 Posted by: Okami Posted at: 2017-03-12T00:16:54.258Z Reads: 235

```
Im not 100% sure yet either.. I think when I will need to I will try to contact the airline company to let them know I will have extra ''dis-assembled'' li-ions with me in handbaggage..

Basically with 6cells it should be the same as with laptop cells (if considering the size)..

Non the less.. im not sure do they check are they certified/ manufactured profesionally or not.. but I know that in some airline rules it is mentioned that battery terminals should be isolated and that's it..

I actually got the idea from here:

http://www.electric-skateboard.builders/t/6s5p-lg-he2-travel-battery/18609/7

A while back he posted his battery pictures in picture thread.. and I was like.. oh I need to make this, too! :D
```

---
## \#5 Posted by: cricrithezar Posted at: 2017-03-12T00:23:42.004Z Reads: 200

```
Yeah I don't think they know enough to really question it if you have the right documents. My only concern is, if I'm shrinkwrapping those myself, that they might look a bit sketchy (the ones in the thread you linked looked really nice until he used electrical tape to wrap them in a nice black pouch with just two contacts sticking out, looks a little too bomb-like for my liking). Since I already have the holders though, I guess I'll just test them and hopefully this works ok.
```

---
## \#6 Posted by: Okami Posted at: 2017-03-12T00:25:23.553Z Reads: 193

```
yeh electrical tape does not look nice :D 

The best is probably to get the right size heatshrink wrapping..to make it somewhat professional.. then maybe print out a label that it is made in unknown chinese factory or such :D
```

---
## \#7 Posted by: cricrithezar Posted at: 2017-03-12T00:42:56.532Z Reads: 190

```
Yeah clear shrinkwrap covering the terminals with a nice label stating the voltage and capacity, if done correctly, would probably look fine. I'd probably want to spot-weld them together too. I'll just do that if these holders don't work out, the university I go to has all the right equipment.
```

---
## \#8 Posted by: darkkevind Posted at: 2017-03-12T01:09:08.005Z Reads: 191

```
I think you'll find with one wheel at the back and only one truck at the front, stability will be worse than with two trucks because at least the truck at the back contributes to the resistance to not let the deck flop over from side to side.
You'd normally have two trucks with their bushings resisting flop, whereas with this design you'll have just one, so you may want to go with extra hard bushes on your front truck.

Other than that, cool design, I like that it's something different.
```

---
## \#9 Posted by: cricrithezar Posted at: 2017-03-12T01:15:01.915Z Reads: 199

```
Yeah, I thought about that, forgot to include it in my post. I'm probably gonna buy an extra-wide front truck (maybe even >200mm wide) to make the wheelbase larger. However, since most of my weight is on my front foot that should help with stopping it from flipping over while riding. Turning might be an issue though, my turn radius will probably be huge. We'll see. Worst case scenario I buy a truck and motor mount and convert my build to a regular 4-wheel design, it would be pretty easy to do.
EDIT: Also, thanks for the feedback, and I'm glad I'm not the only one that thinks it's a fun design!
```

---
## \#10 Posted by: cricrithezar Posted at: 2017-04-17T03:50:32.587Z Reads: 172

```
Ok, board got here and started building various parts. Still have to make the motor mounts and back wheel mounts but that's about it (and order the motor, but that's just a click and maybe 2 weeks shipping away whenever I decide to bite the bullet and buy it).

Anyways I don't have too many up to date picture but I built my own fiberglass enclosure a couple days ago.

2 layers of fiberglass (which is way too flexible, probably gonna epoxy some sort of stiff material on the inside, almost regret not fiberglassing onto the foam mold I created which was hollow).

Here's a picture of the layup (would not recommend using paper to protect the table, especially if using peel ply, epoxy got through all layers and the paper was a pain to remove):

https://goo.gl/photos/LHCw3MGy9rXHFoyk9

And after it was unmolded and about to get painted:

https://goo.gl/photos/m7grACydsFKg2win9

Looks decent enough, kinda wish I'd gone grey instead of black but eh, can always add another layer of paint:

https://goo.gl/photos/CFcrPxFcutPnVkFj8

Bit of door insulation strips and silicone caulk for waterproofing:

https://goo.gl/photos/whr8LoNNfumw48Vp6

Bolted on with m4 bolt wood insterts (don't have pictures of putting them in unfortunately), will be adding stiff strips along the sides to put pressure along the whole length to keep a tight seal:

https://goo.gl/photos/YgGKdS6gyYcjUHkW7

https://goo.gl/photos/cFsdQhASLanMfoEN7

Sits kinda low, but I'm gonna top mount the trucks so that should give me a nice 20mm extra to work with, I also rode it to campus a few days ago and didn't get in the way so I think it should definitely be fine after I top-mount the trucks.

Will post more pics of the back wheel pulley assembled and the battery holders with BMS connected in a bit, they're not with me now so I have to go get them.
```

---
## \#11 Posted by: cricrithezar Posted at: 2017-05-15T03:23:04.941Z Reads: 152

```
Ok! Took me a long time to update this post but I've done quite a bit of progress since last time. Just have to machine the back wheel mount and reprint the motor mount and I should be good to go!

So first of all, one issue I was having was the enclosure being way to flexible and not holding its shape too well, so I added thin balsa strips to the bottom and a third layer of fiberglass on the inside to create a kinda corrugated layer of fiberglass. That helped a lot with the rigidity of the bottom of the enclosure.
https://goo.gl/photos/FUxmRCyowszh2btH6

I also added a few aluminum strips to the sides (though I might remake them, I didn't have any aluminum sheets that were long enough and the holes don't line up perfectly which ended up with me ruining multiple brass inserts (brass is really not very strong).
https://goo.gl/photos/ioWvqZ2ccKkR7Taw9
You can also see the motor and motor mount version 1. I have a better design for the mount but it's really convenient for testing out the vesc on a table

I also finished my battery holder and soldered on my BMS.
https://goo.gl/photos/C9Y6ZWLw6NPWNTy87

And it actually charges!
https://goo.gl/photos/oRDuHaFAvrNZ1eZPA

A picture of my wheel and pulley (just bolted onto the wheel, it's 15mm wide which hopefully means I never have to change the belt ever, but that's probably not the case.
https://goo.gl/photos/JUiRWnFRtWv9EvTQ8
And a picture of the other side, just 3d printed washer thing to hold the bolts in place.
https://goo.gl/photos/rHQa2VVLjFEBTqxW7

I also got to try out the VESC and apart from a wierd problem with the temperature sensor, everything seems to work which is great news. I'll just have to make sure I test the battery holders for the kind of currents I'll be seeing (it's 10s4p though, so hopefully that's ok). Slowly making progress though I'm going to be gone for the summer so if I finish it it'll only be in september or later. Only thing left is to reprint the motor mount (or better yet machine one, but printing is less work usually) and machine my wheel mounts and I should be good to go!

I also top mounted my trucks and it looks really nice and actually rides better (cracks aren't as much of an issue because of the extra weight and inertia of the board).

Picture (corner looks a bit funny, the aluminum strips are still taped on, might just use wood strips so I want the aluminum to be removable but it doesn't look the best):
https://goo.gl/photos/eJHdPmXNasKBUZk96

Really excited to try out this board once it's finished.
```

---
## \#12 Posted by: bill_f Posted at: 2017-05-15T06:22:52.198Z Reads: 131

```
Always good to see innovative design ideas here.
Seems like your turning radius will be decreased with only one truck. The rear truck contributes to turning the board (four wheel steering).
Motor looks pretty exposed to curbs, debris, etc.  But maybe it just looks that way in the rendering.
Good luck!
```

---
## \#13 Posted by: cricrithezar Posted at: 2017-05-15T15:13:18.226Z Reads: 119

```
Yeah we'll see! I was looking for a cheaper way to mount the motor and all things taken into consideration it might be a bit cheaper than two trucks and all the mounts to attach it to the truck, but not all that much (small parts add up).

I'm hoping to 3d print (and maybe also fiberglass) a cover for the motor to shield it from debris. It will probably break if I hit something too big but at least the first thing to hit won't be the motor, and hopefully the front truck flattens the bigger debris before they get to the motor. I'll also have a bit more clearance than on the cad since I'm top-mounting my truck (and will probably make spacers so I can adjust the height of the back truck.

The turning radius is a bit of an issue as well as the fact my wheelbase is a triangle which makes balancing a bit funky, but I guess we'll see. Worst case scenario I can just buy a pair of caliber trucks, some ABEC wheels and a mount-pulley combo and I'll just have a normal board, but hopefully this works out!
```

---
## \#14 Posted by: Okami Posted at: 2017-05-15T18:41:13.469Z Reads: 107

```
@cricrithezar  Why did you choose to build such 3 wheeler in the first place? Did you also wanted to get ''snowboard'' feeling.. or is it just for better turning radius?.. The only other board with this kind of concept i know of is the commercial LeifBoard.
```

---
## \#15 Posted by: cricrithezar Posted at: 2017-05-15T19:16:16.696Z Reads: 113

```
I didn't like having the motor mounted to the truck because that either meant having to put really tall risers on (because as the truck turns, the motor mount makes an arc that can intersect with the deck) or having the motor dangerously close to the ground or sticking out the back which isn't pretty or stealthy (I want it to look like a non-electric board at a glance).

Otherwise the turn radius will probably worse and balancing on it will be a bit harder (not much, just have to make sure to keep most of your weight either near the front, which I will be doing most of the time, or near the center since the wheelbase will be smaller and triangular.

EDIT: My other option was hub motors and I actually would love a pair, but I also wanted something powerful and relatively cheap and even low kv hub motors are still pretty high kv since you don't have a gear reduction in there. This was the best solution for my purposes (at least I hope, we'll see how this turns out).
```

---
## \#16 Posted by: cricrithezar Posted at: 2017-10-12T02:01:47.679Z Reads: 92

```
Ok! Took me a really long time but slowly getting stuff done. Currently getting the motor-mount 3D-printed by a friend and just made some (hopefully temporary) wheel mounts out of a random piece of wood I had laying around. Hopefully I can machine some aluminum mounts at some point though.

https://photos.app.goo.gl/NKiPonEoL97L7x5M2

https://photos.app.goo.gl/5cJMrrxmm2Vv8pyN2

So now that I've ridden it, I'll have to say. I really don't recommend this exact design haha, it's really funky having the whole board tip as much as it does with only half the resistance to roll since there's only one truck. You also have to keep a ton of weight on the front, which isn't a terrible thing. I haven't taken it too far and it'll be very different when I don't have to push but I'm definitely considering building a board dedicated to this design rather than using an off-the-shelf deck. Might make it more triangluar and find a way to have the wheel axle right on the deck so it's not as tippy in the back. I also think I have to tighten the trucks some more. I'm going to end up with a board that can barely turn haha.

Might fiberglass the mounts, they're not quite as strong as I would want and I'm worried about cracks. Hopefully I can test the whole thing soon, motor mount is the last thing that needs to go on the board and then hopefully I can take it around and find ways to fix the issues I have with the design.
```

---
## \#17 Posted by: b264 Posted at: 2017-10-12T02:26:31.879Z Reads: 85

```

Use an evolve supercarve truck maybe?  Not only are they super-wide but they are double-kingpin so hopefully you'll get both trucks' worth of flex out of just one truck.  And the 306mm length gives you more leverage on the bushings to turn tighter
```

---
## \#18 Posted by: b264 Posted at: 2017-10-12T02:27:54.805Z Reads: 85

```
Does that wheel fit in the drop-through slot?
```

---
## \#19 Posted by: cricrithezar Posted at: 2017-10-12T02:31:17.430Z Reads: 85

```
I like the evolve supercarve suggestion. I'll definitely look into those, was looking for larger trucks but was affraid that'd limit my turning even more

The wheel doesn't fit all the way but there is extra room for it if I want to move it up a bit. Maybe I should do that. The main limitting factor is the pulley sticking off the side of the wheel hitting the base of the mounts I made. If I make them out of aluminum I can shave off a bit more thickness but still not all that much.
```

---
## \#20 Posted by: b264 Posted at: 2017-10-12T04:09:19.564Z Reads: 82

```
...thinks out loud...  I wonder what would happen if you put a 15T gear on the wheel that went to another 15T gear ... then you could scoot the wheel way up in the deck, maybe even use a 150mm wheel, maybe even run the axle directly through the deck and not have a mount at all ...
```

---
## \#21 Posted by: cricrithezar Posted at: 2017-10-12T16:23:24.689Z Reads: 76

```
The wheels would probably spin real fast and with that diameter I probably wouldn't get enough torque. The 3-1 ratio is solid at 10S and 190kv I think. Also i'd need to build a board that can fit both the wheel and pulley in the slot as well as room for the belt which means I'd probably have to either mount the motor in the slot as well, or on top of the board. Maybe something like this with a longer and wider slot in the back and some metal brackets to reinforce the board. 
<img src="/uploads/db1493/original/3X/d/2/d2c8e1a3cf9078d21cfed87ab7951d81ecdacd3b.png" width="468" height="328">
It'd probably end up being quite a bit of work to get working and wouldn't give me as much clearance on the bottom so I'd have to integrate the electronics inside the board (probably a thick deck). I'll have to look into it. Gonna try out the board as is this weekend hopefully and see what happens.
```

---
## \#22 Posted by: b264 Posted at: 2017-10-12T16:29:17.677Z Reads: 75

```
That's a good idea too.  I meant that you drive a wheelless axle at 3:1 and just transfer it 1:1 to the wheel
```

---
## \#23 Posted by: cricrithezar Posted at: 2017-10-12T16:59:16.497Z Reads: 71

```
I guess that's one way of doing it! Starts getting pretty complicated though, might be easier to drive the wheel axle directly and have the pulley off to the side, though then I have to mess with bearings and build adapters for the wheel. Right now the pulley is mounted directly to the wheel and I'm using the stock bearings that came with the scooter wheel. I also realized I can shave off a good centimeter or so by machining them out of aluminum. Hopefully that's enough to help with the tipping. Might also mount the truck drop-though again even though my ground clearance might start getting a bit small.
```

---
## \#24 Posted by: darkkevind Posted at: 2017-10-12T18:56:13.451Z Reads: 60

```
Why not have the drive train on the front wheel(s), and just have the back wheel free-wheeling?
```

---
## \#25 Posted by: cricrithezar Posted at: 2017-10-12T20:27:11.025Z Reads: 56

```
The reason for having a single back wheel was to have an easier way of mounting the motor and have it further from the ground and hopefully more protected. If I were to mount the motor on a truck I might as well have a normal truck in the back as well, which is probably better for riding. I'll probably do that if this doesn't work out.

Unless you meant having only one front wheel? Which I'm not sure how well that would ride, sounds really unstable.
But you're right if I'm dead-set on 3 wheels rather than 4 front truck is probably a good way of moving the wheel axle closer to the ground
```

---
