# 3d Printing the clamp ring

### Replies: 35 Views: 1917

## \#1 Posted by: IsTalo Posted at: 2017-07-02T11:53:49.628Z Reads: 178

```
Good morning (Morning in Brazil of course), I had some problems with alien but I solved everything. but I still missing a part of the motor mount, the freaking clamp ring, I don't want to use aluminum and that stuff because I'm tired of using the drill, so I thought about using a 3d printer of doing the clamp ring, 100% infill with Petg, could it be possible?
```

---
## \#2 Posted by: JLabs Posted at: 2017-07-02T12:19:41.713Z Reads: 173

```
It may be, but I would only do it out of ABS. Most other filaments are too brittle. 

I would actually like to see what kind of results you get and if it will crack or not..
```

---
## \#3 Posted by: SirDiff Posted at: 2017-07-02T12:26:51.277Z Reads: 165

```
@fottaz  has done it, but surely not with petg. You have to use reinforced filaments
```

---
## \#4 Posted by: fottaz Posted at: 2017-07-02T12:54:56.529Z Reads: 156

```
Hi! Petg could crack very easily, I tried xtcf 20 colorfabb and Its working so good in dual setup All Terrain..I think ABS could works too if properly designed. I still suggest to use carbon reinforced filaments!
```

---
## \#5 Posted by: IsTalo Posted at: 2017-07-02T13:20:20.011Z Reads: 139

```
The problem is to find this filament in Brazil, also I'm using a friend's 3d printer, so I will see if he have Abs filament
```

---
## \#6 Posted by: IsTalo Posted at: 2017-07-02T13:21:05.958Z Reads: 133

```
Wait, isn't Petg stronger than Abs?
```

---
## \#7 Posted by: JLabs Posted at: 2017-07-02T13:25:26.832Z Reads: 126

```
Every filament type has different qualities, generally ABS is stronger than PETG.
```

---
## \#8 Posted by: IsTalo Posted at: 2017-07-02T13:40:09.079Z Reads: 130

```
That make me sad, I printed my pulleys in petg
```

---
## \#10 Posted by: Nordle Posted at: 2017-07-02T16:39:32.231Z Reads: 119

```
xt cf20 is carbon fiber reinforced petg, wouldnt be reinforced abs better? dunno but very interrested in this. and how is stringing with this xtcf20? cause normal petg does it alot...
```

---
## \#11 Posted by: fottaz Posted at: 2017-07-02T18:50:00.364Z Reads: 113

```
It could be good too...I dont know if Will Be that better, here Is how xtcf20 looks on my mounts <img src="/uploads/db1493/original/3X/d/2/d20cb3bd541658ce1456f84fa8f67a5196b911af.jpg" width="662" height="500">
```

---
## \#12 Posted by: fottaz Posted at: 2017-07-02T18:55:24.405Z Reads: 108

```
<img src="/uploads/db1493/original/3X/9/b/9b99eba6b59215780dc4c0ca1e4c15bbf97381ce.jpg" width="377" height="500">
```

---
## \#13 Posted by: Achmed20 Posted at: 2017-07-02T19:26:25.344Z Reads: 101

```
[quote="JLabs, post:7, topic:26581, full:true"]
Every filament type has different qualities, generally ABS is stronger than PETG
[/quote]

PETG is stronger! however,PETG breaks while ABS bends first and then breaks. thin PETG however is way more flexible then thin abs
```

---
## \#14 Posted by: wafflejock Posted at: 2017-07-02T19:30:02.915Z Reads: 103

```
Interesting I haven't worked with PETG yet at all.  Physical strength is way more complex than it sounds on the surface.  Just printed  (an enclosure) with some Nylon 645... now I realize I probably should have gotten a more rigid nylon didn't realize how flexy this stuff is, very strong but also very noodly.
```

---
## \#15 Posted by: Achmed20 Posted at: 2017-07-02T19:31:00.101Z Reads: 103

```
PLA jsut wont work for the mounter mount. ABS and PETG need metal reinforcement like a steel rods straight through the printed mount.

i tried quite alot in that direction :slight_smile:
https://www.electric-skateboard.builders/t/the-printa-6374-192kv-9s-5000mah-3d-printed-mount/22749/9
 
if you want a purely printed mount, you should go with something like nylon (a rigid one). then again, nylon is so expensive, that you are probably better off buying a metal mount directly
```

---
## \#16 Posted by: IsTalo Posted at: 2017-07-02T21:11:51.777Z Reads: 91

```
So I designed the Clamp Ring, tried to do like the Alien's one. I think I'will try PETG, but I'm asking me, why would it brake?
```

---
## \#17 Posted by: wafflejock Posted at: 2017-07-02T21:41:53.159Z Reads: 95

```
When the motor turns it creates a torque (turning force) on the pulley that force most of that force (ideally) gets transferred through the belt to the other pulley.  In the process of that power being transferred the motor mount and clamp needs to stop the motor from just spinning around the axle like it wants to (equal and opposite forces) and needs to deal with the force of the belt under tension on one side and needs to deal with lateral force since the belt is only pulling on one side of it.... long story short it needs to be able to deal with a lot of forces and some of them like during initial acceleration can crack it (particularly without FOC there are some jitters for the motor to get itself moving before things smooth out).

With an aluminum mount and clamp on the truck it would still shake on my setup until I drenched the whole part with JBWeld, now nothing moves much at all.

If the plastic you're using is in any way brittle then it's going to crack as soon as it wiggles a bit and gets some room to move, also if it's too brittle it will be hard to tighten onto the truck without cracking it.
```

---
## \#18 Posted by: IsTalo Posted at: 2017-07-02T21:57:17.224Z Reads: 81

```
So I don't should try 3d printing??
```

---
## \#19 Posted by: wafflejock Posted at: 2017-07-02T22:02:21.054Z Reads: 85

```
You can try for sure but just would be cautious about what material you choose with the motor mounting parts.  People have done it and can surely be done with thick enough ABS even but just need to take into account the details of the material you're using.  Just search for details from the company that makes the filament, taulman has a lot of information about the Nylons they produce I imagine whoever is making the PETG has specifications on what use cases it's good for.
```

---
## \#20 Posted by: IsTalo Posted at: 2017-07-02T22:06:21.667Z Reads: 85

```
The motor mount is made out of Aluminum (APS mount), I'll try the ABS, will talk to my friend that have the 3d printer
```

---
## \#21 Posted by: Achmed20 Posted at: 2017-07-02T22:26:59.511Z Reads: 85

```
[quote="IsTalo, post:20, topic:26581, full:true"]
The motor mount is made out of Aluminum (APS mount), I'll try the ABS, will talk to my friend that have the 3d printer
[/quote]

good luck with that. that is pretty much the place where my 3d printed mount constaly broke

https://www.electric-skateboard.builders/uploads/db1493/optimized/3X/a/8/a824b7d61a1477b095f14b8acbb05b3bb97580cd_1_666x500.jpg

but i was using a 2700watt motor. if you use a smaller one, it would probably work to some degree.
```

---
## \#22 Posted by: IsTalo Posted at: 2017-07-02T22:28:07.637Z Reads: 84

```
But my mount is made of aluminum, just the clamp rings is missing, to I tought of printing them
```

---
## \#23 Posted by: Achmed20 Posted at: 2017-07-02T22:31:32.927Z Reads: 84

```
clamp ring like adapter from circle to square truck mount??

yeah that will work! PETG or ABS schouldnt realy matter. just dont use PLA :wink:
```

---
## \#24 Posted by: IsTalo Posted at: 2017-07-02T22:35:56.949Z Reads: 79

```
Yeah, like this<img src="/uploads/db1493/original/3X/3/c/3c0ee365dd4a75ea35e1477dc65ed12e1f45cc52.PNG" width="281" height="500">
```

---
## \#25 Posted by: tvidotto Posted at: 2017-07-03T04:37:36.576Z Reads: 67

```
Oi :slight_smile:
 I just printed the same piece for my mount, i would be interested in following the outcome of your project
```

---
## \#26 Posted by: Pedrodemio Posted at: 2017-07-03T04:59:35.548Z Reads: 65

```
It should probably be ok, most materials fail due to traction, be it by pulling or bending, in this case the material will be confined and subject to shear and compression, and 3d printed pieces can deal very well with that since it doesn't force layer separation

If your friend don't have ABS give me a shout, I think shipping will be pretty inexpensive, 3D hubs is another way, lots of people with printers
```

---
## \#27 Posted by: IsTalo Posted at: 2017-07-03T10:40:54.677Z Reads: 62

```
Oi, Brazilian too? Nice to see some in this forum, I have a post of my build, but I have to refresh it

@Pedrodemio Shipping from your house to mine? In Brazil a 20 meters shipping is 30 reais
```

---
## \#28 Posted by: riva_00 Posted at: 2017-07-03T12:11:25.872Z Reads: 63

```
I have a 3D printed clamp ring part with Aliens Mounts.

https://www.electric-skateboard.builders/t/the-cat-gullwing-sidewinder-2-trucks-dual-enertion-r-spec-6355-190kv-alien-drive-mounts-8s2p-18650-25r-vesc-psychotiller-wheels/10305/3

They're currently holding up well, plus I drilled into them to stop the motor slipping down before I used Loctite on everything.

Also trialing 3D printed 6" hubs, which are also holding up well.
```

---
## \#29 Posted by: riva_00 Posted at: 2017-07-03T12:51:00.391Z Reads: 55

```
@fottaz how long have you had the xtcf20 motor mounts?
Never heard of carbon fibre filament, but now I'm just plain excited, where's the build thread for em?
```

---
## \#30 Posted by: IsTalo Posted at: 2017-07-03T12:58:56.436Z Reads: 52

```
That what I was looking, do you have the stl files yet? I made one Design but it was pretty simple. And how do you printed them?
```

---
## \#31 Posted by: jga Posted at: 2017-07-03T13:01:28.685Z Reads: 48

```
I wonder if Tom @Idea did not use PETG for its first attachment rings on his mountain board motor mount. He could give you a feedback.
He subsequently changed them to aluminum.
```

---
## \#32 Posted by: dedinski Posted at: 2017-07-03T13:01:40.859Z Reads: 43

```
Nobody is talking about nylon here (this thread), whats your guys opinion on that?
```

---
## \#33 Posted by: IsTalo Posted at: 2017-07-03T13:02:22.342Z Reads: 43

```
Nylon would be the best option, but it's very expensive
```

---
## \#34 Posted by: IsTalo Posted at: 2017-07-03T13:02:53.372Z Reads: 43

```
Let's see, I think Petg would work fine with 100% infill
```

---
## \#35 Posted by: wafflejock Posted at: 2017-07-03T16:00:46.668Z Reads: 41

```
I love NYLON :)  It is pricey but it is incredibly strong too... only down side is the water absorption of the material makes it a pain and need to get the retraction settings and everything dialed in (also warping).  Once you have it up and running well printing with Nylon makes super durable parts (again delamination is still the weakest link, but in the direction of the print or for compression forces or tensile strength... can't beat it in 3D printing so far as I've seen).

Long story short Nylon huge pain to work with absolutely amazing when it works.  Really good for small parts like gears or pulleys but like others said there are cheaper alternatives.  Most of the ABS and PLA I get is around $20-30 per kg the Nylon is close to twice that, but for small parts you only use an ounce or so of material so like $50 a kg is about $1.30 per ounce.

I got some of the NinjaFlex TPU, some other TPU, and some Nylon 645 (somewhat flexible) I should have gone with the 12xx series for less water absorption but just going to put my filament in a container with desiccant to keep it dry.
```

---
## \#36 Posted by: dedinski Posted at: 2017-07-03T19:37:39.621Z Reads: 36

```
I also have taulman 645, the first few prints were crap until i found out i could dry it in my oven. 60 degrees C for 6-8 hours and it comes out perfect and teady to print. I printed a 40t pulley that fits like a dream.
```

---
