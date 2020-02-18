# 3D Printed MTB Inner Gear Drivetrain &#124; Trampa Holypro &#124; VESC 6 &#124; OVERION 130kv &#124; Graphene 12S12AH

### Replies: 146 Views: 9490

## \#1 Posted by: Der6FingerJo Posted at: 2018-01-07T20:40:05.824Z Reads: 673

```
Hello Everyone!

Over the last few months i've been working on an E-MTB after building a regular Longboard which i liked very much, but it isn't the right thing for my somewhat rural region (middle-ish germany).

My current state is that i tested it today in the garden. Climbed some small but steep hills to test the gears, but it was dark and fucking cold so i didn't drive that much. Just thrashed it around for a bit. There's still much on the to-do list but i'm very glad it actually worked.

<img src="/uploads/db1493/original/3X/2/6/266c9b93f67027dfea98e709581aec5da9ad70ee.jpg" width="666" height="500">

That's the current state of the board, functional but not at all finished.



My Goals for the Build are:
- VESC 6 for reliability
- more torque than speed 
- reasonable range of ~20km 
- arduino based remote and telemetry system in a trigger style remote

and most importantly:

## a 3D printed Drivetrain

<img src="/uploads/db1493/original/3X/0/c/0c8b9081c2a47095de5f3df05b2e98857ce526f7.jpg" width="690" height="479">

My design started with a Nowind style gear setup which consists of regular encapsulated gears, but after roughly estimating the print time it was clear that ~40 hours of printing for just a single drive just wasn't feasible.

So then i remembered [Lee 13's Website](https://www.lee13.net/trampa-i-drive-e-mountainboard) and his Inner Gear Drive that really resonated with me. It's just so elegant and as space efficient as imaginable (at least until hubs for MTBs arrive).
Drawbacks of this design are mainly that you cant use 8072 Motors anymore, but that's ok for me because of the higher gear ratio that is achievable. I want torque for this board, not speed.

So i started up Fusion 360 again and ended up with this:

<img src="/uploads/db1493/original/3X/1/0/10b45a0ec4995e7dc689ee30bd872dadd0f52f99.jpg" width="690" height="326">

Lee uses custom made gears for his drive, but i wanted it to be compatible with readily available steel gears, mine are modul 2 gears so that i can use the same same spur gears as Nowind does.

This design would in theory allow me to convert it to a regular outer gear drive using a very small wheel gear (probably with gummies :heart_eyes:), which is why i made the enclosure detachable to in future switch between both modes of operation and their enclosures easily. 

The cover for the big inner gear is still WIP, i wanted to wait until all dimensions are final and i had proof that it works.

<img src="/uploads/db1493/original/3X/9/c/9c31a85be395d9415507a62c606100bc8eb48c26.jpg" width="666" height="500">

This is the part attached to the wheel, there's a 6mm spacer beneath and the screws are flush with the surface in the final version.
It's a 55t gear with a 10t gear on the motor, so combined with a 130kv Overion motor - torque won't be an issue.
I didn't dare go more than 25% of throttle as of yet on flat terrain from standstill :sweat_smile: 
(also holy fucking shit, foc + hall sensors is pure heaven coming from a vesc 4.12 sensorless longboard)


Next thing to do was the material choice. Originally i wanted to use Polycarbonate for everything in the drive, but i found and used Taulman Alloy 910 which is a blend of polycarbonate and nylon. 

I had to change my original Creality CR 10 Hotend to a Micro Swiss one to reliably reach 250°C and i think it works a treat. Printing one gear with 3.2mmm wall and top/bottom thickness as well as 100% infill takes about 11.5 hours. Also the printer hast to be in a closed build chamber for this filament to work best. 
I used a big old plastic bag, works too :smile: 

<img src="/uploads/db1493/original/3X/3/b/3bec46cb352bec80ac056db6939bf835827ba6b7.jpg" width="375" height="500">

This is the motor mount, it's a fairly simple design with 4 grub screws. I melted some threaded inserts from Rampa into printed holes and they hold tight very well. It's printed in PLA and i'm very impressed with how durable it is, but in the long run i will do them again with petg or polycarbonate. Since the gap between motor and truck is so small there aren't big forces acting on the mount, which is why it holds up using only PLA.

<img src="/uploads/db1493/original/3X/a/b/ab0155bc473a5efce7048844f37f7bb736ab3fb0.jpg" width="375" height="500">

No motorisation here, Officer :D

<img src="/uploads/db1493/original/3X/7/f/7f4dd26a970da15c40cd2420e8685e8ee72798fd.jpg" width="375" height="500">

This is a prototype for the gear cover (actually for the whole drive on the picture). I think it will be sufficient, maybe i will add a net or something in the middle.

<img src="/uploads/db1493/original/3X/a/f/afb55b3fd18442490b00c772df8c6d7de3293528.jpg" width="666" height="500">

I think it looks quite cool :sunglasses:


I think the shortcoming of this drive is the lack of precision you only get from professional cnc machines. On the other hand, my printer cost around 450€ with the upgrades i did to it so i'm quite fascinated with what i could achieve with that. I'm not sure if i need to file or mill the hanger flat, the part of the hanger it screws on is the flattest on the truck i think.


## Controlling the Beast

This is more or less a sideproject, it's mainly to learn stuff about arduino, coding, communication and such.

I wanted a trigger remote like the GT2B and chose okp's design, the SPARKLE remote, as basis for this.

<img src="/uploads/db1493/original/3X/e/1/e1690d521d4889eb5ea02487ed067a448d9a1881.jpg" width="375" height="500">

The amount of functions is nowhere near the remote @Wajdi is doing, but i like the ergonomics much better than the nunchuck style remotes.
For now it only displays data from the VESC, including permanent distance tracking (which is totally wrong as of yet but i'm working on it), but i want to implement a simple menu to change power and stuff sometime. It sort of works right now but i'm not satisfied completely. I might get a regular GT2B for inbetween if i can't bring this to a polished, working state soon.

Bonus feature: A dead man switch in form of cherry MX blue switch, which pleases the mechanical keyboard geek inside of me and provides an excellent tactile feedback when pushing it in.

##the rest

As of right now, the board definitely isn't finished. I had 2 weeks off over christmas and new year of which i nearly used 100% of the time for the Board.

On my to do list are many things, including lights, a finished VESC enclosure (only printed the baseplate so far), finishing touches and prints for the drivetrain, getting the remote to work flawlessly and so on...

If that's all done i will ride and ride and ride and ride to test the drivetrain. Obviously i can't say how well it will hold up in the long run, but immediate failure didn't occur today when i really pushed the torque so i'm quite optimistic. And then again, i can always just print a new gear.

I'm an electric engineering student so i don't have any formal knowledge of gears and stuff, and i would really appreciate your thoughts on all of this and the board in general, what i missed and what could be improved.

Many thanks to all the following people for inspirations and guidance in form of their build threads here on the forum and elsewhere!

@NoWind @Duffman @Riako @Trampa @Pimousse @squad @okp (and probably many more, this forum is full of great people - sorry if i missed some great trampa builders, i read all of your threads!)

And of course special shoutout to @Rich for answering all my MTB noob questions over the course of 400 messages :joy:

Here's a glamourshot of a burnout, no point in shooting other videos in the dark so you have to believe me that it works :smiley:
 
https://www.instagram.com/p/Bdp-VgZBgb2/?taken-by=der6fingerjo
```

---
## \#2 Posted by: FredrikHems Posted at: 2018-01-07T21:18:32.216Z Reads: 510

```
Really cool design mate!. As I got a 3d printer and plan to build a emtb future this is just perfect :smile: However, do you plan to switch to a metal drive gear? I think the plastics one will wear fast, but time will show i guess
```

---
## \#3 Posted by: Der6FingerJo Posted at: 2018-01-07T21:38:59.041Z Reads: 503

```
Hey thanks man, i'm actually really curious to see how the wear is. Taulman states that Alloy 910 can be used for high load gears and different gear designs depend on POM, so i think plastic gears are a valid option. 

Only time will tell for sure how it is with the Alloy 910, if this fails, there's still Polycarbonate or actual POM Filament to try out.
```

---
## \#4 Posted by: SOICDIP Posted at: 2018-01-07T22:23:35.083Z Reads: 473

```
Let us know how the gears work out.

How did you mount the motor to the motor gear? Using a set screw for the keyway? That might be the weakest part.
```

---
## \#5 Posted by: Achmed20 Posted at: 2018-01-07T23:10:50.098Z Reads: 451

```
awesome!
i've seen you pic a few days ago in the pic no words thread which alrleady made me curious. glad you made a thread.
```

---
## \#6 Posted by: Riako Posted at: 2018-01-07T23:46:26.347Z Reads: 450

```
**Absolutly gorgeous prototypes !!!**
So cool it ride already !!! !! Ha ha :smile: 
**Well done DFJ** ;) 
Thanks for sharing all of this genious thing and to inspire us again and like you said their is so mutch people here who inspire itch other ! Thanks to this forum :blush:
 The setup looks perfect, maybe  add a middle support like you said 1st and how it work yes
```

---
## \#7 Posted by: notepad Posted at: 2018-01-07T23:58:22.425Z Reads: 452

```
How is the printed mount holding up.  Ive just started designing a dual motor belt drive for trampa infinity trucks, but in PETG ( mostly because its a cheap printer)    would be good to see how your PCNY blend survives. might push me to get some!
```

---
## \#8 Posted by: Sapphirinia Posted at: 2018-01-08T04:05:55.647Z Reads: 454

```
I'm building something similar, although not as complicated. I'm waiting on my skate wheels to come though. I wanted to use a bigger wheel that was lighter so I ordered some huge inline skate wheels. It will fit between this and the holes are where the holes are on the wheels so I will thread my "connectors" through them. Reprinting the connectors since I added wrong and they're 10mm too short. I made the whole thing solid in hopes that my ABS will be strong enough. <img src="/uploads/db1493/original/3X/8/7/87e367034bca5b1608af9576575ed03f8c5a6f47.jpg" width="568" height="499">
```

---
## \#9 Posted by: Der6FingerJo Posted at: 2018-01-08T08:12:34.807Z Reads: 449

```
[quote="SOICDIP, post:4, topic:43108"]
How did you mount the motor to the motor gear? Using a set screw for the keyway? That might be the weakest part.
[/quote]

Used good ol' green and smelly Loctite 648 (I believe) for mounting, no holes for set screws in the maedler gears. [quote="Achmed20, post:5, topic:43108, full:true"]
awesome!
i've seen you pic a few days ago in the pic no words thread which alrleady made me curious. glad you made a thread.
[/quote]

Didn't actually think I would get to this point that fast, that's why I started to tease earlier :D[quote="Riako, post:6, topic:43108"]
Absolutly gorgeous prototypes !!!
So cool it ride already !!! !! Ha ha :smile:
[/quote]

Thanks man, as far as gears are concerned this is the final stage I think. Just have to redo one motor mount and add a cover (and of course learn to properly ride a Trampa) before the madness truly begins :smile:[quote="notepad, post:7, topic:43108, full:true"]
How is the printed mount holding up.  Ive just started designing a dual motor belt drive for trampa infinity trucks, but in PETG ( mostly because its a cheap printer)    would be good to see how your PCNY blend survives. might push me to get some!
[/quote]

Hey man, the motor mount is made of plain PLA, only the gears are Alloy 910. For a belt drive I would at least use PETG but possibly an even stiffer plastic because of the leverage the motors generate in this design. [quote="Sapphirinia, post:8, topic:43108"]
I'm building something similar, although not as complicated. I'm waiting on my skate wheels to come though. I wanted to use a bigger wheel that was lighter so I ordered some huge inline skate wheels. It will fit between this and the holes are where the holes are on the wheels so I will thread my "connectors" through them. Reprinting the connectors since I added wrong and they're 10mm too short. I made the whole thing solid in hopes that my ABS will be strong enough.
[/quote]

I'm assuming this is for street style boards? That would be great, no gears yet for those. It would be great if ABS holds up, I chose Alloy 910 mostly because of its durability in a sense that is bends instead of breaking, so ABS would be the exact opposite of that.
```

---
## \#10 Posted by: rich Posted at: 2018-01-08T13:00:36.222Z Reads: 400

```
Excited to see the first version running! 
Really nice and unique drive train, very curious to hear how reliable it is, looks awesome! And I have to drool when I see the position of your motors :heart_eyes:, very well done bro!

[quote="Der6FingerJo, post:1, topic:43108"]
i tested it today in the garden. Climbed some small but steep hills to test the gears,
[/quote]


Jesus, how big is your garden? :laughing:
```

---
## \#11 Posted by: Sapphirinia Posted at: 2018-01-08T13:35:13.982Z Reads: 390

```
Cool. Yea, street board. I will probably try that filament out. Never heard of it until now. Would be pretty useful. I'll see how the abs does for now though.
```

---
## \#12 Posted by: Der6FingerJo Posted at: 2018-01-08T15:44:45.587Z Reads: 386

```
[quote="rich, post:10, topic:43108"]
Jesus, how big is your garden? :laughing:
[/quote]

i mean like some pile of earth laying around, no hill really. but enough to max out the torque on the wheels for a short bit.
```

---
## \#13 Posted by: Pimousse Posted at: 2018-01-08T18:42:52.714Z Reads: 382

```
Very nice build dude !!
Glad to be mentioned !
Can't wait to see some action videos with that monster ! ;)
```

---
## \#14 Posted by: Der6FingerJo Posted at: 2018-01-08T21:26:45.948Z Reads: 356

```
Thanks, i'm still playing with the idea of stealing that LED Ring from your PirCac Build :sweat_smile:
```

---
## \#15 Posted by: Pimousse Posted at: 2018-01-08T21:48:05.009Z Reads: 371

```
I did a batch of it for French guys but it still not tested.
Once it's approved, I may throw a few to those interested ;)

(if you're not afraid by French language : http://e-sk8.fr/forum/viewtopic.php?f=25&t=2731 )
```

---
## \#16 Posted by: Der6FingerJo Posted at: 2018-01-08T22:26:44.408Z Reads: 369

```
Looks really nice on your enclosure! But it all depends on the rest of the remote system i'm going to be using, i already got an arduino in the box so i might as well add the led ring to that.
```

---
## \#17 Posted by: Pimousse Posted at: 2018-01-09T08:28:52.633Z Reads: 364

```
If you only want to display battery state of charge on the ring without any interaction (the rear light too), it's even more simple.
Feel free to fork the code. ;)
```

---
## \#18 Posted by: Alobert Posted at: 2018-01-10T10:18:19.367Z Reads: 357

```
awesome!
But what about the quality, is it durable?
```

---
## \#19 Posted by: Der6FingerJo Posted at: 2018-01-10T11:07:12.404Z Reads: 359

```
That's what I'm trying to test out in the long run. The filament manufacturer Taulman said that Alloy 910 is made for high load gears so I'm being rather optimistic about the whole thing after my first tests.
```

---
## \#20 Posted by: FredrikHems Posted at: 2018-01-10T11:15:33.193Z Reads: 362

```
Got any riding videos  you wanna share?:heart_eyes::wink:
```

---
## \#21 Posted by: Der6FingerJo Posted at: 2018-01-10T11:21:46.979Z Reads: 335

```
Unfortunately not yet, I only rode it once in the dark so far. There are too many things lift to do/print for a proper maiden ride. But I might try again on the weekend if I manage to print the gear covers.
```

---
## \#22 Posted by: Der6FingerJo Posted at: 2018-01-11T16:49:54.488Z Reads: 360

```
Today i did the first little test ride on the street. I'm very pleased with how the board handles, just needs some tuning on the throttle curve (as in it accelerates too bloody fast (which is how i wanted it but still)). 

Still no Enclosure for the Drivetrain and the Electronics, but i updated my Motor Mount Design. 
On the left is the old one which, in retrospect, wasn't too brilliant especially the placement of the grub screws. It resulted in the motor being not parallel with the truck. The new design fixes all that with a double grub screw on the opposite side of the motor.

![image|690x345](upload://cIkUpTbtEFFp3TYJpPHO2DMqV1X.jpg)

My current roadmap is to try and make a cover for the gear, looking something like this and using some sort of sieve to cover the rest of the exposed parts.

![image|603x500](upload://lUBCrBMwq4OEB7oFacUvsMOPG08.jpg)

And finally a enclosure for the electronics for which i already printed the bottom part, currently hesitant to print the cover because i can't decide on a design for it.
```

---
## \#23 Posted by: Sapphirinia Posted at: 2018-01-11T17:57:00.587Z Reads: 322

```
Do you think you can help me with modeling the Pulley correctly? I measured the belt teeth when I made my Pulley but the grooves don't match up perfectly.
```

---
## \#24 Posted by: Der6FingerJo Posted at: 2018-01-11T19:15:52.009Z Reads: 322

```
Sure, hit me up
```

---
## \#25 Posted by: FredrikHems Posted at: 2018-01-11T19:24:52.338Z Reads: 322

```
Just for your information so can you find files of HTD 5M (most likely What you use) profiles on thingivers. You can just bring these STL files in to your cad and work from there. :grinning:
```

---
## \#26 Posted by: Der6FingerJo Posted at: 2018-01-13T17:42:42.186Z Reads: 325

```
So today i made the first multi-kilometer trip with the board on all kinds of surfaces. Started with a short ride on the street - massive improvement over the longboard because of all the potholes here. Then went on a path with a lot of gravel and small rocks. Board handled it excellent but definitely not my favorite riding experience. After that i got to a place with trimmed grass and it was just great. Such a soft ride with the pneumatics and  the deck.

However one if my gears drive began to rattle whenever i was braking or applying no power. 
Found out that the Motor Mount became loose even though i just applied loctite before the the ride. I don't know if that was the cause or the symptom of the rattling. Will try again, if that doesn't work i will have to redesign the motor mount with m6 instead of m4 grub screws and narrower tolerances against the truck. 

Still no sign of wear on the gears even though i was making sure to torture them hard :D
```

---
## \#27 Posted by: Pedrodemio Posted at: 2018-01-13T18:54:24.178Z Reads: 295

```
How "just"? loctite needs a few hours to cure

Looking forward to hear how long those gears last
```

---
## \#28 Posted by: Der6FingerJo Posted at: 2018-01-13T18:57:13.204Z Reads: 306

```
[quote="Pedrodemio, post:27, topic:43108"]
How “just”? loctite needs a few hours to cure
[/quote]

Ooooooooooooh. Then it might work better tomorrow, thanks! :sweat_smile:

I used the regular blue stuff. 

[quote="Pedrodemio, post:27, topic:43108"]
Looking forward to hear how long those gears last
[/quote]

Pretty optimistic by now, I hope it's justified :slight_smile:
```

---
## \#29 Posted by: Pedrodemio Posted at: 2018-01-13T19:00:18.437Z Reads: 289

```
So that's it probably, but i don't know how well it works on plastic, maybe not at all, it may even dissolve the motor mount a bit, if that not work you can try MEK (methyl ethyl ketone), its the best thing to glue ABS, just dip the grub screws and insert, give a few hours, it will melt the plastic on the thread and give a pretty good bond, if all fails, just a tiny drop of CA glue
```

---
## \#30 Posted by: Der6FingerJo Posted at: 2018-01-13T19:12:56.837Z Reads: 282

```
Thanks for the detailed answer, it will sure come in handy in the future with 3d printed projects!
However for the mounts I'm using threaded inserts that I molted into the plastic so there's no reason Loctite shouldn't work. 

And I might be able to further reduce the gap between truck and mount so it sits more snugly by default without screws.
```

---
## \#31 Posted by: Pedrodemio Posted at: 2018-01-13T19:17:33.465Z Reads: 282

```
Oh sure, where did you buy the inserts? a few months ago i needed them but couldn't find
```

---
## \#32 Posted by: Der6FingerJo Posted at: 2018-01-13T19:21:17.825Z Reads: 298

```
Uh I just got them off eBay, they are called Rampa Inserts. Can't say anything about the availability outside of Germany. But generally they are made for wood applications. 

I made holes in the model for them (around 1-2mm smaller in diameter than the outer thread of the insert) and put the inserts on my soldering iron tip and screwed them in with it.
```

---
## \#33 Posted by: Pedrodemio Posted at: 2018-01-13T19:22:22.612Z Reads: 307

```
Thanks, I will see what i can find
```

---
## \#34 Posted by: Der6FingerJo Posted at: 2018-01-14T16:38:41.271Z Reads: 316

```
So TECHNICALLY i got the first gear failure today, however on this particular gear the printer fucked up before. During the print some layers weren't fully extruded which is why the gear seperated in the middle. Originally i filled up the gaps with some glue and it held well until yesterday but i guess it wasn't enough. 
Bummer, i can only print these 12 hour prints on the weekends when im home.

![image|666x500](upload://66hWlea0LGOdyXG2UELmGzfrEpf.jpg)
```

---
## \#35 Posted by: Achmed20 Posted at: 2018-01-14T16:50:54.616Z Reads: 307

```
thats fine for a prototype i guess. 
i would print the final gear in nylon anyway and you have to print nylon so ridicoulus slow that underextrusion probably wont happen there.,
```

---
## \#36 Posted by: Der6FingerJo Posted at: 2018-01-14T16:57:17.546Z Reads: 304

```
I'm quite satisfied with the Polycarbonate/Nylon print and i guess the underextrusion happened because i tried to keep the filament in the original box while printing (because of humidity). Stupid mistake, i will probably print a better spool holder for the next time. 
I really need more  printers for prototyping :sweat_smile:

But still no wear on the other gear!
```

---
## \#37 Posted by: Achmed20 Posted at: 2018-01-14T23:40:41.047Z Reads: 293

```
what filament are you using right now?
```

---
## \#38 Posted by: Der6FingerJo Posted at: 2018-01-15T05:13:52.696Z Reads: 287

```
Still using Alloy 910 for the gears and PLA for the mounts
```

---
## \#39 Posted by: wafflejock Posted at: 2018-01-15T10:09:23.577Z Reads: 304

```
I printed some nylon motor pulleys (pretty sure Taulman 645 is what I used, was either that or bridge, the amazon link is dead) You definitely need to dry it out like crazy in a toaster oven that isn't used for anything else or dehumidifier for a good amount of time before using it at all, the steam in there really makes the layers weak compared to a completely clean print.

You also want to go pretty hot and really slow, like @Achmed20 mentioned already slow is your friend when it comes to nylon but that also makes it terrible for printing big parts. Personally have started taking my 3d prints and making molds of them using silicone and then pouring resins into the silicone mold to get a solid part, it adds a few steps but once you have the mold it's much faster/easier to make solid parts and can choose from a variety of hardness plastic/urethane resin mixes to pour into the molds depending on what exactly you're making.  Have been using this 85D hardness stuff called task-9 for some wheel pulleys but have only done hard bench testing and light on the road testing (been too cold to go ride much recently).

[Custom wheel pulleys](https://photos.app.goo.gl/HUOVVVXtyQYjQy9T2)
[Nylon motor pulley](https://photos.app.goo.gl/27c44OZkqqXwz9o62)

Nylon motor one held up for a couple of months of riding, but that was the best one I'd made the other attempts had delaminated in different ways (either through the grub screws or internally so the motor would spin free).
```

---
## \#40 Posted by: Der6FingerJo Posted at: 2018-01-15T11:44:11.801Z Reads: 305

```
That was an interesting read, thanks! 

Originally I was also looking into pure Nylon like 645, but on the Taulman Website they say that Alloy 910 is for high load gears, opposed to medium load gears for nylon 645, which is why I chose 910. 

I do keep the filament very dry at all times and I hope that this isn't causing the issue, after all there's also a good part of polycarbonate in the filament which should be less prone to humidity than nylon. 

I print with 250°C/60°C at 50mm/s and the printing process itself looks pretty ok. Just had to tweak retraction a bit, but that doesn't matter that much for gears. 

The gear delaminated right at the point where the extrusion failed and where I later applied glue to hold it together for a while at least, so I'm pretty confident that the teeth are strong enough for this application.  The glue just wasn't enough, there were parts in the gear that you could look through so the layer bonding was barely there at that point.

The mold making sounds really interesting, I will definitely check that out a bit. It's really a pain in the ass to print 12h for a single gear so I'm very open for different methods.  

Personally I wouldn't use plastic parts on the motor pulley so I'm impressed you got it to stay on there at all :smiley:
I'm using regular steel gears on my motor shaft.
```

---
## \#41 Posted by: xilw3r Posted at: 2018-01-15T14:20:58.601Z Reads: 276

```
My god this is amazing.

If you told someone several years ago, that people would use FDM printers to make gear reduction systems that handle like 2kW+, most of them would have called you a nutjob spreading blasphemy. A lot would still do that today I'm sure :D 

Loving the inner gear design!
```

---
## \#42 Posted by: Der6FingerJo Posted at: 2018-01-15T15:21:23.059Z Reads: 283

```
Yeah, many still do :smile: 

 I'm really impressed by how it all works, wasn't too sure if it would work but hey apparently it was worth a shot. 

The credit for the designs is all Lee13's, I took the idea and made it module 2 compatible.
```

---
## \#43 Posted by: Der6FingerJo Posted at: 2018-01-20T16:56:13.089Z Reads: 295

```
Time for another update!
Went out today after reprinting the gear that failed last week.
Only problem was something with one of the motor mounts which i will redo in petg and with bigger grub screws, so that should be fixed by next week. It gave a rattling noise while braking.

![IMG_20180120_152151|374x500](upload://k1rfQLBgZf53774xNH4c3waSnpE.jpg)

After riding under those conditions i consider my inner gear drive testes and tortured, it never failed  and no debris or dirt got stuck inside!  Only a bit of mud on the outside of the  gear but oh well.

![IMG_20180120_162600|666x500](upload://qKrV9urE9pNp6xp9j2CFvV6rqiY.jpg)
(ignore the steel gear, it was dirty before)

All in all a pretty great run, many situatios where i had to give full throttle and nothing broke.

 ![IMG_20180120_161200|666x500](upload://1ObTKlZEActNHHT2XQrrIw4b6Sz.jpg)

Unfortunately @rich never told me that you have to clean those things as well :rofl:
```

---
## \#44 Posted by: rich Posted at: 2018-01-20T17:31:26.641Z Reads: 295

```
[quote="Der6FingerJo, post:43, topic:43108"]
Unfortunately @rich never told me that you have to clean those things as well :rofl:
[/quote]


You are right, I'm endlessly sorry, hope you can forgive me.
I recommend seperate shoes and clothes, too if cleaning is not a hobby of you.

Nice test of the gears and great they survive such conditions. :sunglasses:

But this fresh mud on your board is disgusting, let it dry then it looks much cooler :joy:

![20170731_155704|690x388](upload://zAvZDWKpXt2K8mydqnw9wDSW1RT.jpg)
```

---
## \#45 Posted by: Der6FingerJo Posted at: 2018-01-20T17:33:12.228Z Reads: 291

```
Scrubbed it already off like a mad man :smile:
```

---
## \#46 Posted by: Maxid Posted at: 2018-01-30T16:04:57.142Z Reads: 285

```
Are the design files somewhere? I'd love to try this on a 218mm Torqueboards truck with my 6inch pneumatics.
```

---
## \#47 Posted by: Der6FingerJo Posted at: 2018-01-30T16:58:13.015Z Reads: 288

```
I haven't released anything as of yet because i'm constantly changing stuff atm. But i honestly doubt that you can fit a 63xx motor in 6" wheels with reasonable ground clearance and even if so, you would have to redo every part. Shoot me a pm if you want to work something out!
```

---
## \#48 Posted by: Der6FingerJo Posted at: 2018-02-16T20:23:44.213Z Reads: 288

```
i FINALLY found my action cam so here is some video!

https://www.youtube.com/watch?v=d5DVDUb6O9k&t=2s

The terrain was much muddier than it looks in the video and i left out the many times i was stuck because that would be very boring to watch. **Still no wear on the gears.**

![IMG_20180216_154516|666x500](upload://AkKbdHhcWnf6HBDW8cyz0THGsRT.jpg)

As you can see i was a bit inspired by @Nowind's Mad Max look :laughing:

Also got distance tracking to work, verified it with google maps and it should be reasonably accurate. In the end i rode 20km and used 7800mAh out of 12000, i'm pretty happy with this result.
```

---
## \#49 Posted by: Riako Posted at: 2018-02-17T14:07:36.442Z Reads: 276

```
:heart_eyes: video 
:star_struck: photo
:hushed: consumption 

Thanks for sharing this :+1: This is crazy D6FJo !! Sound really good (about noise) too ! Really quiet at low speed. Love it !
17Wh/km thats really impressive (for me) with all the off road trail ! (whats your VESC config actually ?)

Visualy your setup looks incredibly light man ! you weighed it ?
I got to finish my custom motor and trucks to test it your way - full 3d printed. Did I miss something or even your mount is printed ? I will reread all here cause its needed :blush:

Big Up :v:
```

---
## \#50 Posted by: Der6FingerJo Posted at: 2018-02-17T14:31:15.085Z Reads: 280

```
Thanks Riako, really appreciate you positivity :smiley:

[quote="Riako, post:49, topic:43108"]
17Wh/km thats really impressive (for me) with all the off road trail ! (whats your VESC config actually ?)
[/quote]

So my VESC Config is 2x VESC 6 connected via CAN BUS and regular Firmware, 60A Motor Max and 60A Batt Max per ESC. I think the efficiency comes from the 130kv motors and the 1:5,5 gearing ratio. Since my max. speed is only 35km/h i pull less amps at cruising speeds of around 20 km/h than someone with a top speed of 50km/h and higher kv and/or shorter gear ratio. Hope that makes sense :smiley:

My Max amps might be 60A, but i never dare to pull more than maybe 60% of throttle during regular riding on the street :smile:

[quote="Riako, post:49, topic:43108"]
Visualy your setup looks incredibly light man ! you weighed it ?
[/quote]

The Board is 11kg and the batteries 3,2kg, so maybe between 14 and 15kg all up weight. My drive itself should be around 600 grams and the 3d printed box for the electronics is fairly light as well. Also there's no big battery box and no big lights, basically im running only what's really necessary.

[quote="Riako, post:49, topic:43108"]
I got to finish my custom motor and trucks to test it your way - full 3d printed. Did I miss something or even your mount is printed ? I will reread all here cause its needed :blush:
[/quote]

I'm curious to see your project man :smiley:
Yes my motor mounts are 3d printed also. Everything of the inner gear drive is 3d printed, motor mount, gear itself and cover for the gear. No major failure so far, only little things that could be avoided using different filament and/or design. Only metal parts are the motors themselfes and the pinion gears.
```

---
## \#51 Posted by: rich Posted at: 2018-02-17T15:52:07.859Z Reads: 260

```
Nice video, expected more noise from the drivetrain, sounds good!

Love the pic, that's how it should look ater a nasty ride :laughing:
How much mud is on the gears when your board looks like that?
```

---
## \#52 Posted by: Der6FingerJo Posted at: 2018-02-17T16:24:36.409Z Reads: 259

```
[quote="rich, post:51, topic:43108"]
How much mud is on the gears when your board looks like that?
[/quote]

While riding both covers for the gears broke on the underside (because i was lazy and only used my pla prototypes, didn't reprint them in alloy 910 so far) but the gear stayed resonably clean. Just a bit of dirt on the outer edges on the gears, nothing that would actually interfere i think :smile:
```

---
## \#53 Posted by: Riako Posted at: 2018-02-17T16:26:05.974Z Reads: 262

```
Ok, wow perfect offorad ratio with this kv (imo) ;) sure the full shoudnt be that necessary :smile: 
we got almost the same setup,.. except transmission and ratio. (Im more about 30/40kmh cruising on bicyle road, and juste 4.7:1 in 9" = 48kmh and not that confortable when ceiling that topspeed on the 9" low pressure ... that is the lack of efficiency I get for sure. But the setup is already insane and effective in all the road/trail configuration. I'm mean the wheels spinning the ground is my limitation crossing. I'm around 20/24Wh/km.)
So I'm conna mod it a bit your way Sir !! But I'm almost already at my maximum ratio with the 6B chain (dont want bigger wheels (for ground clearence) or smallest motor sprocket (for noise and chain angle turn)...
You could expect richting the 30km off riding so  :hear_no_evil: ?

Yes I'm was at 14.7kg. I think you win 1kg maybe a bit more.
I'm making a little emtb for training - I would plan less than 10kg and it could be possible with your transmission setup ! 
**Raaah I love this forum and all the inspiration that you share guyz !!!**

In fact, this project is just a Frank geared hub mixed your way for emtb and air tire :blush: all because of you once again guys ! haha (this will not be used on my 2nd trainaing board cause I guess it will weigh more thant all the actual Dart Vapor rear trucks). Waiting to lathe the motor and show you guys ;)
```

---
## \#54 Posted by: Der6FingerJo Posted at: 2018-02-17T16:42:20.267Z Reads: 270

```
[quote="Riako, post:53, topic:43108"]
(Im more about 30/40kmh cruising on bicyle road, and juste 4.7:1 in 9" = 48kmh and not that confortable when ceiling that topspeed on the 9" low pressure … that is the lack of efficiency I get for sure.
[/quote]

I'm still getting my bearings at 20-30km/h so i wouldn't think that 20-24Wh/km is totally unreasonable when i'm hitting 30+ km/h more often. I'm using 8" tires on ~50psi for reference.

[quote="Riako, post:53, topic:43108"]
I’m mean the wheels spinning the ground is my limitation crossing.
[/quote]
Same here, way more power on the wheels that it can actually transfer to the ground off road :laughing:

[quote="Riako, post:53, topic:43108"]
You could expect richting the 30km off riding so  :hear_no_evil: ?
[/quote]

Might be possible if i stretch the lipos a bit, but i prefer to run them from 4.1V to 3.6-3.7V per cell. From the 20km i got maybe 8 of them were heavy offroad, rest was street or light offroad.

[quote="Riako, post:53, topic:43108"]
I’m making a little emtb for training - I would plan less than 10kg and it could be possible with your transmission setup !
[/quote]

If you want to test my drive you can hit me up, unfortunately i can only provide the files as i can't produce the drive for other people right now due to time constraints.

[quote="Riako, post:53, topic:43108"]
In fact, this project is just a Frank geared hub mixed your way for emtb and air tire :blush: all because of you once again guys ! haha (this will not be used on my 2nd trainaing board cause I guess it will weigh more thant all the actual Dart Vapor rear trucks). Waiting to lathe the motor and show you guys :wink:
[/quote]
Sounds really great, i like this concept better than using regular hub motors without gearin on MTBs.
```

---
## \#55 Posted by: Riako Posted at: 2018-02-17T17:01:35.790Z Reads: 264

```
Ok, yes, maybe I'm not in a so bad configuration ... but 4.15v to 3.55v ... (70a Motor max, 70a batt max).
Yes on full flat street like in paris, I could be down to 14/15Wh/km
https://media1.tenor.com/images/8536a69dd2f2c9114a14ed98ca1281f8/tenor.gif?itemid=8844243
You get me ! It will be on honor to test it mate !! It will be on mbs matrix II pro but I will make it fit :+1:
I will share mine to you after ;)
```

---
## \#56 Posted by: Silverline Posted at: 2018-02-18T09:27:39.163Z Reads: 257

```
So freaking cool...

Are you planning to release the STL files, at some point ??
```

---
## \#57 Posted by: Der6FingerJo Posted at: 2018-02-18T09:41:54.327Z Reads: 247

```
I'm thinking about it. There are still a few things i'd like to change that i don't have time for right now, so it might take a few weeks.
```

---
## \#58 Posted by: TheFluffiest Posted at: 2018-02-19T08:30:41.447Z Reads: 244

```
Are both the motor and wheel gears printed? Or is the motor gear steel? I'm sure you said this somewhere, I just can't find it. Thanks! Amazing idea, looks badass!
```

---
## \#59 Posted by: Der6FingerJo Posted at: 2018-02-19T09:32:06.460Z Reads: 248

```
The motor gear is steel, mainly because I couldn't think of a way to attach a printed gear to the metal shaft. Might try a printed gear someday for science.
```

---
## \#60 Posted by: FredrikHems Posted at: 2018-02-19T11:19:47.733Z Reads: 243

```
A keyway and some set screws so it wont slide back and forth, maybe?
```

---
## \#61 Posted by: Der6FingerJo Posted at: 2018-02-19T13:17:14.622Z Reads: 232

```
Set screws are hard to do with 3d prints i don't actually believe in them so much. I was thinking about keyway, flattened shaft and helical gears that would naturally push the motor gear against the shaft.
```

---
## \#62 Posted by: Apolo Posted at: 2018-02-19T14:36:27.668Z Reads: 224

```
Your cad looks like it was an stl converted to a brep format, any reason why? Just curious since it makes it a lot harder to work with.
```

---
## \#63 Posted by: Der6FingerJo Posted at: 2018-02-19T14:42:03.774Z Reads: 237

```
Good eyesight :stuck_out_tongue_winking_eye:

I used a seperate file for the whole assembly, so i only converted the parts from different files to stl and reimported them into the assembly file. That way i wasn't tempted to make changes in the assembly file that wouldn't be carried over to original files. 

I know that's not a proper workflow, but i had to convert everything to STL anyways and i am no CAD professional :smile:
```

---
## \#64 Posted by: TheFluffiest Posted at: 2018-02-21T08:55:24.287Z Reads: 227

```
Haha, created a thread asking about this a few days ago. @Achmed20 said he printed a pulley with a D shaped hole, ground the motor shaft down to the same shape, and glue it on. He said it was reliable so far, with roughly 100km clocked. However, this was with a belt driven system, I'm not sure how it would work with gears. Taulman Alloy 910 nylon or polycarbonate might be up to it, but I'm not sure how long. Probably best to keep the steel gear for the build, but please do it for science!
```

---
## \#65 Posted by: Der6FingerJo Posted at: 2018-02-21T09:13:10.393Z Reads: 228

```
If i hadn't glued it to the shaft with loctite 638 i would totally try it, but removing this stuff isn't a joke :smile: 
 so it has to wait for my next build. Or maybe @Riako can try when he's ready.
Unfortunately i don't have anything big with new motors in the pipeline for the next few months so it will be a while until i can try it.
```

---
## \#66 Posted by: DanSkates Posted at: 2018-02-21T10:17:58.575Z Reads: 217

```
Wow!!! Beautiful work dude - what a dirt monster! I love how you started so clean and came back like you had been mud wrestling 😀
```

---
## \#67 Posted by: Der6FingerJo Posted at: 2018-02-21T10:36:15.922Z Reads: 223

```
Thanks Dan :D

Yeah the mud put on a good fight but the trampa always won, it might have been faster to just get off and walk sometimes but screw that :smile:

I was thinking about bigger tires a few times during this ride, maybe even with custom printed hubs. We'll see :grin:
```

---
## \#68 Posted by: Riako Posted at: 2018-02-22T14:09:21.872Z Reads: 219

```
Ok, I'm almost done for a test with Matric truck, just a bit late cause I see that for TA910 I need a confortable 250°C possible (actualy my cr10 cool do it, or at 240/245 but for a long print I prefer to make the upgrade). So I'm waiting for the little 1st coil of it and a e3d v6 like hotend and yes for sure I just could make a try of it for science :smile:
 You should have find nice parameter for your print with it already ? Also what is your printer ? (just curious :blush: )

thanks Tom ;)
```

---
## \#69 Posted by: Der6FingerJo Posted at: 2018-02-22T14:32:38.111Z Reads: 240

```
I'm also using a CR 10 with a Micro Swiss Hotend. I chose Micro Swiss because it is a no modifications replacement for the original hotend but i considered the e3d as well!

My printing temps are 255°C on the Nozzle, 60°C on the bed and no BuildTak on the glass plate, just glue stick and pva glue. Be sure to use some kind of enclosure for the really long prints (i'm using a big ass old plastic bag that i pre-heat with a hair dryer to 30-35°C). And don't forget a brim for the allo 910, at least 6mm.
Oh and speed is 50mm/s, i always wanted to try faster but didn't want to take the risk.
I'm also thinking about a .06mm nozzle for the big gears. 

I got one or two situation where no more filament would come out of the nozzle, so be sure to check the print at least once per hour.

Also i'd recomment to try a benchy first, i printed my first benchy with 245°C and could rip it apart fairly easily, but with 255°C the benchy was damn near invincible!

Good luck with you prints, saw your files on Fusion 360 and would only suggest that you don't do it 100% like the measurements but leave a tiny bit of wiggle room. But i don't really know the matrix trucks, so it could be much flatter than the trampa ones :smile:
```

---
## \#70 Posted by: Riako Posted at: 2018-02-22T15:59:15.898Z Reads: 239

```
:grinning: as usual, **thanks for this complet feedback Tom !**!
Perfect, I will try it with all your recommandation ;) :+1: 
I am so impatient to finally test a new filament and especially a new transmission your direct internal ...
https://media.giphy.com/media/MEtSuIu6qu0HC/giphy.gif
```

---
## \#71 Posted by: telnoi Posted at: 2018-02-24T15:33:26.958Z Reads: 233

```
Awesome project. Where did you source the motor spur gear and what is the bore size in your case?
Seems difficult to find spur gears with a low tooth count :frowning:
```

---
## \#72 Posted by: Der6FingerJo Posted at: 2018-02-24T17:59:20.197Z Reads: 227

```
I got it from maedler.de 
It's 10 teeth modul 2 with 8mm bore. They also have 12t 10mm bore.
```

---
## \#73 Posted by: telnoi Posted at: 2018-02-25T05:46:15.267Z Reads: 216

```
Thanks. Did they also drill the set screw for you?
Does fusion 360 offer a type of spur gear generator, or did you use an online generator for it?

I came across this tool (http://hessmer.org/gears/InvoluteSpurGearBuilder.html), but circular pitch is something I can't make sense of yet. Wondering how you created the counterpart for the modul 2 spur gear.
```

---
## \#74 Posted by: Der6FingerJo Posted at: 2018-02-25T12:12:03.631Z Reads: 220

```
Fusion 360 has a gear generator, but I don't know if it works for inner gears. 

I used an openSCAD script from Thingiverse for my gears. I put out an STL which I converted to dwg and imported to fusion. I know that sounds ridiculous but it was more of an accident than a part of my plan. 

For the small gear I used maedlers .STEP files. I actually printed one from those step files and it kind of felt like a futuristic version of pirating things :smile:
```

---
## \#75 Posted by: telnoi Posted at: 2018-02-25T12:44:07.342Z Reads: 222

```
Yeah, noticed that Maedler offers stp files for download. At least you can prototype before ordering parts.

Contemplating what to do. Noticed a few times that my belts were nicked and partly rippes due to stones. I imagine the outer part of the wheel gear would come into contact with stones where I ride. A smaller wheel tooth count would be preferable in my case with a larger motor gear to get more ground clearance and reducing the chance of damaging gears. Means I need to use regular gears instead of involute.
```

---
## \#76 Posted by: Der6FingerJo Posted at: 2018-02-25T15:15:39.925Z Reads: 221

```
I actually pulled few small rocks out of my gears when i rode them without cover. You hear and feel that something is blocked, but the rocks are pretty much pressed into the valleys of the teeth. So far no visible damage on those spots, bonus points for a slightly flexible material i guess.

With covers however, nothing really gets into the drive. Only condition i haven't tested so far is sand but i'm also not keen to do so.
```

---
## \#77 Posted by: Miraclepenguin Posted at: 2018-02-28T19:18:16.679Z Reads: 214

```
What trucks are you using? And do you think this setup would work well on a normal cruiser with caliber trucks?
```

---
## \#78 Posted by: Der6FingerJo Posted at: 2018-02-28T19:58:13.398Z Reads: 213

```
I'm using trampa vertigo trucks and no, i think it won't work on caliber trucks because you really can't use 8" wheels on those.
```

---
## \#79 Posted by: telnoi Posted at: 2018-03-01T19:22:03.708Z Reads: 214

```
have you adjusted any of the measurements for 3d printing?
noticed that the bolt to bolt distance of the superstar hubs = 42.3205 mm, which seems to be an odd distance.
```

---
## \#80 Posted by: Der6FingerJo Posted at: 2018-03-01T19:27:45.762Z Reads: 218

```
No i haven't. They are 72° apart and 36mm from the center each. I didn't consider bolt to bolt distance.
```

---
## \#81 Posted by: telnoi Posted at: 2018-03-01T19:28:32.912Z Reads: 215

```
I see. Makes sense.
Just wanted to make sure :slight_smile:
```

---
## \#82 Posted by: telnoi Posted at: 2018-03-02T13:34:20.673Z Reads: 235

```
Playing around for now. Different direction (mixture of different designs I have seen here).
Wheel spur drive needs to be adjusted based on measurements after I receive my Trampa, along with the truck clamp. Those would also be the only CNC'd parts. 

![44|601x500](upload://cySdrEvtGvCzOEThqJcitFnezo8.jpg)
![53|455x500](upload://xjPbzWNJGMlf9wAYpHdDdE6iaXn.jpg)
![54|441x500](upload://2Iv6FiQJbjFS5BUWU8hNvhHn3yM.jpg)
```

---
## \#83 Posted by: Der6FingerJo Posted at: 2018-03-02T13:41:13.026Z Reads: 226

```
That looks nice!
I played around with a regular outer gear drive in the beginning too, but i found that to be quite a lot more to print and it would take more than 30 hours for just one side. But no reason for it not to work!
```

---
## \#84 Posted by: telnoi Posted at: 2018-03-02T14:35:39.137Z Reads: 221

```
Thanks. Only reason for going with outer gear is due to wanting to use a 5:1 gear ratio with a 10T module 2 spur gear.

The two grey plates will be milled out of a thin sheet of alu or steel. The beveled part to which the motor is attached will be printed. Should save on milling cost and printing time. 

The prototype itself will be printed at a low infill/just need to know if it all fits :slight_smile:
```

---
## \#85 Posted by: Der6FingerJo Posted at: 2018-03-02T14:43:58.682Z Reads: 220

```
true.. i wanted to go for 1:5 too in the beginning but it was just too close with the inner gear drive. On the positive side i got all the torque :smiley:

Milling the plates is a really good idea, that saves most of the print time. I think printing the  box would have been 20 hours or so using polycarbonate and somewhat thicker walls if i remember correctly.
```

---
## \#86 Posted by: telnoi Posted at: 2018-03-04T09:46:09.570Z Reads: 220

```
These look rather interesting for ensuring that screws are not stripped from the plastic motor mount/adds some stability. If I understand this correctly, the M size refers to the inner thread.

https://www.ebay.co.uk/itm/M4-M5-M6-M8-M10-THREADED-HEX-DRIVE-FIXING-TYPE-D-WOOD-INSERT-NUTS-ALL-SIZES/321618140748?hash=item4ae1ef5e4c:m:muBI5Lf5R8r2Xdnbc_ZojRA
```

---
## \#87 Posted by: Der6FingerJo Posted at: 2018-03-04T10:20:24.382Z Reads: 212

```
That's kind of what i use with the Rampa Inserts. They aren't segmented though, so it's a continous outer thread. I think it would work the same so it's all good.
```

---
## \#88 Posted by: telnoi Posted at: 2018-03-04T10:32:19.933Z Reads: 214

```
Do you have a link to the ones you use?
Edit: never mind. Did not realize ''rampa'' is the actual name of the type of screw. Sounds like something Trampa would use for marketing.
 :smile:
```

---
## \#89 Posted by: Trdolan03 Posted at: 2018-03-06T05:24:52.855Z Reads: 205

```
Can you release the Fusion files?
```

---
## \#90 Posted by: Der6FingerJo Posted at: 2018-03-06T12:34:46.317Z Reads: 209

```
I can send them to you if you are serious about testing the drive, but i wont upload them for everyone since i'm still finding things that need to be optimized.
```

---
## \#91 Posted by: Riako Posted at: 2018-03-06T13:10:26.970Z Reads: 214

```
Yes sorry I'm late, still waiting for my upgrade hotten for CR10 ...
But I start printing parts in raw quality just a testing montage and I have mod it for Matrix 2 trucks : 
https://monlongboardelectrique.files.wordpress.com/2018/03/rps20180305_201514.jpg
Thanks a lot once again @Der6FingerJo for your sharing !! Be sure I will give it a blank test And more when I could print with the good filament.
Now I have modified it slightly a bit, with my need and regarding the grateful and simply one of @Kug3lis  :+1: 
(you could find it in your folder Tom ;) I will show you soon guys)
**All of it cause you guys !!! Thank you so much**
```

---
## \#92 Posted by: Der6FingerJo Posted at: 2018-03-06T13:28:51.078Z Reads: 207

```
Haha no need to hurry, we're not under a production schedule or anything :smile:

I like the sliding design as well but i wasn't too sure about it when 3D printed (out of regular PLA at least) but you should definitely try it :smiley:

Im doing some revisions when i break my current setup somehow, but it holds up strong so far :stuck_out_tongue_winking_eye:
```

---
## \#93 Posted by: Riako Posted at: 2018-03-06T13:46:19.221Z Reads: 197

```
:smile: Yes ! I really can not wait to ride that! And re-rider anyway ^^ I could test that chain and strap then to tater something else :blush:

Your build is simply so grateful for those who want to test or embark on the adventure easily, it smells good so far !!!
```

---
## \#94 Posted by: Der6FingerJo Posted at: 2018-03-06T13:48:30.352Z Reads: 194

```
[quote="Riako, post:93, topic:43108"]
Your build is simply so grateful for those who want to test or embark on the adventure easily, it smells good so far !!!
[/quote]

Actually i had to wash the rear tires yesterday because they smelled a bit like dog poo but i guess you didn't mean that in a literal sense  :rofl:
```

---
## \#95 Posted by: Trdolan03 Posted at: 2018-03-06T15:33:15.142Z Reads: 198

```
I'll pm you
```

---
## \#96 Posted by: Der6FingerJo Posted at: 2018-04-14T18:30:21.663Z Reads: 205

```
![IMG_20180414_171228|666x500](upload://dBaTQAi4lfIK01un3OIN5UsDVEs.jpg)

Just wanted to give  a quick update on the 3D Printed Drivetrain. 

Today i rode 28km on mostly paved bicycle streets and had an absolute blast. The Board seems to top out at around 31km/h, which might sounds low to some of you but for me it's absolutely fine and the hill climb performance is great. It isn't just about how fast it can climb hills but most importantly that my motors don't overheat after a longer climb. Since there are many many steep hills around here this is exactly what i need.

Funny thing is just that with 31km/h on a flat street i only need to pull the trigger about one third, so even when i pull through nothing happens anymore. Oh well.

The gears are still holding up very well, only the motor mounts occasionally make problems when braking. Seems to be an alignment issue and they also came loose several times after riding very bumpy parts. (funnily enough i don't notice loose mounts at all while driving). I printed new ones and filed them to the contours of the trampa hanger, used proper loctite on all grub screws and even heated the edges of the mount up to let them flow exactly to the shape of the hanger. Time will tell if this will be enough, might have to use bigger grub screws and/or a flat cnc'ed hanger. 

I'm well aware that this drive isn't as precise or bulletproof as other Gear Drives (Direct Drives :laughing:) but i never expected that. I think it is still an awesome way to demonstrate what's possible with relatively low budget 3D Printing and i aim to improve it as much as i can. Or at least until i'm fed up with it and buy one of Jensos Drives :smiley:

If you want the files you can message me. I decided against uploading this stuff publically mostly because i want people to at least read this thread so that they know the risks involved when using ist.
```

---
## \#97 Posted by: rich Posted at: 2018-04-14T19:31:01.314Z Reads: 186

```
Wow, nice picture!
Glad to hear your new mounts hold better, or did they move on the ride today?

[quote="Der6FingerJo, post:96, topic:43108"]
Gear Drives (Direct Drives :laughing:)
[/quote]

You play with fire bro :joy:
```

---
## \#98 Posted by: Der6FingerJo Posted at: 2018-04-14T21:33:06.753Z Reads: 193

```
[quote="rich, post:97, topic:43108"]
Glad to hear your new mounts hold better, or did they move on the ride today?
[/quote]
They moved today but i tightened them once in a while. I suspect it was the lack of Loctite, didn't reapply it after switching over to the new mounts. A bit was left from the original installation on the grub screws but it wasn't enough.

[quote="rich, post:97, topic:43108"]
You play with fire bro :joy:
[/quote]
Better than playing with fucking tubes i guess :rofl:
```

---
## \#99 Posted by: Achmed20 Posted at: 2018-04-15T17:49:55.195Z Reads: 189

```
dam! i'd realy like to give it a try sooner or later (probably later, quite busy right now).
```

---
## \#100 Posted by: Der6FingerJo Posted at: 2018-04-15T19:48:00.331Z Reads: 199

```
Sure, shoot me a message when you're ready.



I'm out of luck for a while, the loctite 638 on my spur gear gave up today and i can't fix it for the next few days.

Sitting here like
![image|502x277](upload://x1LJrhHXGm9KpHZPSdpjBpsJdVa.jpg)
```

---
## \#101 Posted by: Achmed20 Posted at: 2018-04-15T19:58:24.578Z Reads: 188

```
will do!

also, hope you have a backup board ;)
```

---
## \#102 Posted by: Der6FingerJo Posted at: 2018-04-19T13:36:49.032Z Reads: 183

```
So after i performed some dark rituals with my 60W soldering iron and some tin i managed to "weld" the gear good enough to the shaft that i holds up my daily casual abuse. However the other gear now came right off the damn motor. The previous one just didn't spin with the axle but now i was able to pull the last one that failed off by hand.

Think about it, the bottlenecks of my 3D printed drive train are the metal gears :rofl:
```

---
## \#103 Posted by: Nordle Posted at: 2018-04-19T13:42:03.474Z Reads: 176

```
No, the way you mount them is the bottleneck :P
```

---
## \#104 Posted by: Der6FingerJo Posted at: 2018-04-19T13:45:15.757Z Reads: 173

```
Yeah i know it just sounded so good :smile:
However my printed gears are still holding up great :grin:

I will try again after really cleaning them up  and roughing up the surface a bit, i hope it's enough.
```

---
## \#105 Posted by: Ackmaniac Posted at: 2018-04-19T14:22:32.968Z Reads: 177

```
Are you aware that after you apply loctite to the shaft it should rest for 24h?
```

---
## \#106 Posted by: Der6FingerJo Posted at: 2018-04-19T15:19:10.915Z Reads: 183

```
Yes of course :smile:
Though i think i got a little overexcited the first time around and only let it cure over night. I hope that's the culprit.
```

---
## \#107 Posted by: Der6FingerJo Posted at: 2018-04-25T15:30:04.296Z Reads: 190

```
Another update on my odyssey:

![IMG_20180420_203652|374x500](upload://wjYIYF3fpokygBlpM7YE39eHOo1.jpg)

Even after heating the whole gear up with 1000°C flame for a few minutes the fucker didn't move. Well, saying it didn't move is wrong because it pulled the WHOLE DAMN SHAFT out of the motor instead of simply sliding off the shaft. God damn it. 
But in the end i was able to hammer it loose from the shaft (which, thank skatan, wasn't bend or took other damage) and attach it back again after proper cleaning and roughing up the surface. So after somehow getting the shaft back in the motor and reattaching the shaft's grub screws everything seems to be working fine now. Did my usual 5km of torturing the gears with hill stalls and such and nothing moved so far.

If no major problems occur from here on i think i can finally say that the development of my drivetrain is completed. Let's hope for the best :D
```

---
## \#108 Posted by: Der6FingerJo Posted at: 2018-05-05T21:18:35.260Z Reads: 188

```
Today i had a very annoying crash and i wanted to share some details people might overlook. I was riding a very bumpy offroad path with many loose rocks and the rear of the board naturally vibrated like crazy. 

Unfortunately this resulted in the power of my receiver coming loose which mean the VESC was getting absolutely no signal, not even failsafe. That in turn meant that it applied breaks on both sides with 3A respectively, which was enough to catch me completely off guard and i kind of did a stoppie with the board and went down front-facing. I'm sure it looked hilarious. 

Nothing serious happened, although my whole body still feels a bit sore and shaky. Glad i wore protection and my helmet. It was with maybe 10-15km/h. Funny thing was that i didn't feel scared or anything during the fall itself, just annoyed that something on my board wasn't working even before i touched the ground :smiley:
Also took me a few minutes to remember that i should check my body because all i did was look at the board for possible faults. 

Guess what i'm trying to say is that everyone should be cautious about those little things as well as the failsafe-settings in the VESC. I fly racing drones and rode the board for 300km without ever facing such an issue until now..
I'm reworking my enclosure right now and will print a better one, but until then i'll add a lot of hot glue to all the small solder joints to keep them from vibrating.
```

---
## \#109 Posted by: mmaner Posted at: 2018-05-05T22:06:33.809Z Reads: 178

```
Hot glue FTW.  A small drop in all of your connectors will save you a lifetime of pain and suffering.
```

---
## \#110 Posted by: GrecoMan Posted at: 2018-05-06T00:50:06.726Z Reads: 178

```
i personally use zip ties on every single xt60 or xt90 connector, hot glue on the rest
```

---
## \#111 Posted by: telnoi Posted at: 2018-05-06T05:38:21.466Z Reads: 180

```
Sadly, failsafe worked as intended. It's a constant worry of mine.

Alternative is the board using a curve for braking or shooting off in the distance or not braking at all. In all cases, it would have enough time to do serious damage.
```

---
## \#112 Posted by: rich Posted at: 2018-05-06T07:02:38.793Z Reads: 182

```
Glad to hear you are OK, I know how dangerous it can be even with drop outs but the brake thing sounds scary.

So do you mean the ppm connector on the vesc was disconnected due to vibrations?
```

---
## \#113 Posted by: Der6FingerJo Posted at: 2018-05-06T07:54:57.323Z Reads: 197

```
[quote="mmaner, post:109, topic:43108, full:true"]
Hot glue FTW.  A small drop in all of your connectors will save you a lifetime of pain and suffering.
[/quote]

I actually used a lot of hot glue on those connections already. At least on the solder joints directly, seems like the longer end of the cable still vibratet enough to shake the joint inside the glue loose. Anyways, i fixed it with even more glue.

[quote="GrecoMan, post:110, topic:43108, full:true"]
i personally use zip ties on every single xt60 or xt90 connector, hot glue on the rest
[/quote]
Never heard of a XT60/XT90 come loose, that would need a lot of hardcore offroad riding :smile:

[quote="telnoi, post:111, topic:43108, full:true"]
Sadly, failsafe worked as intended. It’s a constant worry of mine.

Alternative is the board using a curve for braking or shooting off in the distance or not braking at all. In all cases, it would have enough time to do serious damage.
[/quote]

In this situation a weaker break would have been perfect, in other situations a weaker break would be even more dangerous when going downhill or so. You can't really win in this case.
But some kind of intelligent breaking would of course be cool. Now i can see why the VESC 6 schematics has the connections for Accelerometers.

[quote="rich, post:112, topic:43108"]
Glad to hear you are OK, I know how dangerous it can be even with drop outs but the brake thing sounds scary.
[/quote]

If i had captured the stoppie part before falling i would have totally rocked the S.K.A.T.E. challenge :rofl:

[quote="rich, post:112, topic:43108"]
So do you mean the ppm connector on the vesc was disconnected due to vibrations?
[/quote]

It was actually the power cable to the nrf24 module (the actual RF receiver module) that came loose. That way the Arduino didn't get any data from the remote.
Now that i think about it - i believe it was the arduino that sent the brake signal to the vesc because it didn't get any data and the actual ppm cable was still fine. But in the end it was the same effect - too much braking without a warning. Maybe i should implement some kind of buzzer that gives a warning before throwing me off the board.
```

---
## \#114 Posted by: Ackmaniac Posted at: 2018-05-06T10:16:39.816Z Reads: 188

```
For that reason i modified the failsafe function in the ACKMANIAC-Tool firmware mod (Version 3.100 and 3.101).
I added a ramping when the failsafe becomes active. So you have a smooth transition from acceleration to the failsafe brake current. In the original you can go from full power to failsafe current immediately.
And even worse, when the connection comes back full power is immediately active again. So it can happen that you experience full power, failsafe brake and full power in 100 ms which can easily throw you off the board,
So my firmware mod also rams back to power when the connection comes back. And you can test that by simply switching off the remote. Even under power (but please do that carefully).
I said it would be great if everybody can donate something when they realise that this function safed their skin. But i am pretty sure most don't even recognize it. Because most times you loose connection for a couple of milliseconds (like the scenario above). In in this case it would be only only a short ramp.

I also recommend to set the timeout o 250ms so that the ramping happens quick after a timeout. Otherwise with 1000 ms  it can happen that you do full power for another second while you already released the throttle.
And because of the smooth ramping you can also set the "Timeout brake current" higher so that it would brake you to a safe stop even when you go don hill (like 10A or 15A).
```

---
## \#115 Posted by: GrecoMan Posted at: 2018-05-06T13:04:49.016Z Reads: 181

```
[quote="Der6FingerJo, post:113, topic:43108"]
Never heard of a XT60/XT90 come loose, that would need a lot of hardcore offroad riding :smile:
[/quote]

I have a street board 😉
scary as fuck when main power disconnects 🤣
```

---
## \#116 Posted by: telnoi Posted at: 2018-05-06T13:09:50.575Z Reads: 174

```
I'll switch this evening, though as I understand it doing this for a ppm Signal with programmed failsafe will be a bit harder. Have to research it a bit more.

Do I have to do motor detection again, or can I copy the bldc settings across vesc tool/ackmaniac?
```

---
## \#117 Posted by: Ackmaniac Posted at: 2018-05-06T14:33:06.794Z Reads: 181

```
I explain everything for PPM here in the first post in the Chapter "Timeout Behavior"
http://www.electric-skateboard.builders/t/extended-ackmaniac-esc-tool-based-on-vesc-tool/35116?u=ackmaniac
```

---
## \#118 Posted by: AndyBigD Posted at: 2018-05-06T18:24:26.639Z Reads: 174

```
You might have just made my mind up for me... Think I want the ackmaniac tool on my build too now! Are the failsafe ramp/settings adjustable?
```

---
## \#119 Posted by: Ackmaniac Posted at: 2018-05-06T18:30:24.149Z Reads: 180

```
No. It ramps down 50A per second till it is at 0 amps and then ramps up the regen by 20A a second. So if you accelerate with 50A you feel in 1 second gently that the power goes and if failsafe is set to 20A you will feel that the brakes get stronger over a second. If I would leave that adjustable people will be confused. Not many here totally understand the nunchuk ramping. (which works a bit wrong in the original firmware BTW)
And when the signal comes back it does the same on the opposite direction. So instead if immediate power on, off and on again you have a smooth ramping.
```

---
## \#120 Posted by: Der6FingerJo Posted at: 2018-05-07T14:41:03.777Z Reads: 191

```
[quote="GrecoMan, post:115, topic:43108"]
I have a street board :wink:

scary as fuck when main power disconnects :rofl:
[/quote]

A trick i used with XT60's on my racing quad was that i shoved the tip of a tooth pick into the plugs inside of the connector. Makes the prongs go further apart and holds them much tighter. No guarantees though :smile:

@Ackmaniac i have to admit that i am skeptical about putting custom firmware on the VESC, though you made a couple of very good points about using your version. I'll definitely look into it some more and decide when i redo the box. Adding more cool user-oriented features sure isn't a strong point of BV's development.



Since many people were interested in this and i put about 300km to 400km on the original gear at least, here are some comparison pictures:

This is a relatively new gear, printed it 50km ago to test my new 0.6mm nozzle setup on the printer:
![whole_new|375x500](upload://sWunrlhUtZpD4bcCK7rRaL2L8dA.jpg)

And this is the very original gear i had on my board since day one:
![whole_old|375x500](upload://ztptamrPCZGveKfoGv0WiQHwCPX.jpg)

Close-up of the newer gear:
![detail_new|375x500](upload://z5ulk9RRYZNb3l8Bjy1e75Kaw13.jpg)

Close-up of the OG gear:
![detail_old|375x500](upload://ztiVSDkotS8FImAmnVdE1cbiUvt.jpg)

It's not that detailed since it's hard to photograph the black filament on black gears and black stuff etc etc, but the main point is that besides dirt i can't see any real wear so far. Makes me very happy to see this working, imagine how much easier it would be to manufacture helical and double-helical gears like this compared to a over 9000-axis CNC :laughing:

Wouldn't have thought at the beginning that the motor mounts were the hardest thing to design right, but at least they seem to work ok right now. Only problem i still have is teeth skipping on very hard braking maneuvers that i didn't encounter in real riding conditions so far. I assume that either the gear to gear distance is a bit too high or it's just the flexible part of the Nylon+PC filament. When i slowly ramp up the braking i have no problems.
```

---
## \#121 Posted by: Donson Posted at: 2018-05-12T00:40:57.908Z Reads: 175

```
can i use your drive for my trampa :pray:
```

---
## \#122 Posted by: naranga Posted at: 2018-06-01T09:09:23.803Z Reads: 169

```
This is an awesome project! :heart_eyes: I started designing basically the same thing but haven't completed the design yet. It would be awesome to get the model to draw some inspiration from it. There are some things I already like better in yours! I'm not managing to send you a PM. I guess it's because I just created an account so I can PM you. :joy: Been only reading so far! If you could send me a PM, that would be awesome! @Der6FingerJo
```

---
## \#123 Posted by: Trdolan03 Posted at: 2018-06-23T18:30:57.811Z Reads: 155

```
@Der6FingerJo Does your design allow for you to change the gear mesh?
```

---
## \#124 Posted by: Der6FingerJo Posted at: 2018-06-24T11:43:59.996Z Reads: 156

```
What exactly do you mean? Tooth count or design of the gear itself?
I can send you STEP files so you can modify it more easily.
```

---
## \#125 Posted by: Trdolan03 Posted at: 2018-06-24T16:29:59.302Z Reads: 156

```
I mean can you slide the motor forward back to change the space in between the gears
```

---
## \#126 Posted by: moon Posted at: 2018-06-24T16:39:10.076Z Reads: 159

```
Like this?

![image|690x451](upload://8u9xqyjIaRIEvFFCv6ckXoFMyMs.jpg)

3 gear system, the wheel gear cannot move position but the other two gears can move easily. Then it is secured after allignment
```

---
## \#127 Posted by: Trdolan03 Posted at: 2018-06-24T18:34:41.573Z Reads: 158

```
I'm not sure if you were asking me but yes, that is what I was wondering on his 3d printed drive setup. He said that there was some slippage under heavy breaking and that it may be related to the gap between the gears so I was wondering in he would move his motor, and pinion gear, closer to the wheel gear to reduce this slipping.
```

---
## \#128 Posted by: Der6FingerJo Posted at: 2018-06-24T18:35:11.220Z Reads: 158

```
Oh yeah sure, you should see it in the files. Actually i'm gonna make a new version of the .zip tomorrow, i changed a lot of minor things in the files that i have now tested.
```

---
## \#129 Posted by: Trdolan03 Posted at: 2018-06-24T18:36:19.490Z Reads: 160

```
@Der6FingerJo Sounds good, send the new zip once you have it.
```

---
## \#130 Posted by: Der6FingerJo Posted at: 2018-12-25T20:21:48.313Z Reads: 131

```
Guys! It's thread resurrection time! :D

So over the last year i really tried to test my printed drive and came to the following conclusions:

- the 3D printed gears are durable enough for this application, however the filament choice was not perfect
- the alignment of the motor mounts wasn't good enough
- the motor mounts had too much flex in them
- trampa wheels are wobbly af 

Now, i understand that developing a 3D printed [s]direct[/s] ohmygodiamsoterriblysorryhowcouldidothatohno
GEAR drive might not be the most efficient solution, but it's more of a pet project for me at this point. The first version carried me through the summer, although i had to do a lot of botching to get it working, but also learned a lot about printing and mechanical design.

I recently got myself a Cetus 3D Mk3 printer, which is way more precise and all around better than my old Creality CR10 (and also soooo much better to handle since it's way smaller), so this is what my current pieces were printed on.

Anyways, here are the new parts i worked on:

![IMG_20181219_203509_Bokeh|375x500](upload://phwYewyEry2cylR3htDurJHrHvn.jpeg) 

This is the new motor mount with a direct connection to the axle, which makes it pretty much perfectly aligned and center, like the adapters Trampa themselfes use. I also integrated some steel rods (borrowed the idea from @solidgeek) and basically made the mounting surface reallyｔｈｉｃｃ. Right now it's printed with plain ol' PLA and its really stiff. I'm actually pretty impressed by how much more rigid it is compared to before.

The next part is the gear itself. A byproduct of the new motor mount is a mounting position for an extra support bearing, which you can see here:

![IMG_20181222_230141|666x500](upload://5B3Jir1hYbg6aZnQvSp1gKXTfar.jpeg) 

This pretty much reduces the wobble of the gear by 99%, which really does help a lot. 
I will probably print the final gears with Polymaker PC Max filament to make them a bit stiffer than the original Nylon+PC gears, as i suspect that they deformed a bit over time.

So that's the status right now. I'm also working on a redesigned remote with a proper PCB, a better VESC Box and i'm probably replacing my trampa wheels because they are wobbly af (even the front ones). 

Since Cetus didn't release a heated build plate yet it will be a while until i can test again and it's cold outside anyways, so i'll take my sweet time to optimize everything on the bench.

Can't wait to test this all around improved version of the drive next year. Cheers guys, and thanks for the continued inspiration on this forum :slight_smile:
```

---
## \#131 Posted by: rich Posted at: 2018-12-26T01:25:55.923Z Reads: 127

```
Great to see an update :ok_hand:
The mount looks really sturdy and the support bearing is a clever upgrade, nice!

[quote="Der6FingerJo, post:130, topic:43108"]
Can’t wait to test this all around improved version of the drive next year.
[/quote]
Next year? :roll_eyes:
Go for a ride **now**!

Is the alignment better with the new mounts? If you still have problems you could buy a [precision hanger/truck](http://www.trampaboards.com/cnc-precision-vertigo-emtb-truck---16-inch-wide-with-12mm-hollow-axles-with-vertigo-baseplate--steel-kingpin--p-26391.html) with cnc'd hanger. 

![PNG|690x333](upload://5sPH3385moEimfdlK7r8DRNS665.jpeg)
```

---
## \#132 Posted by: Der6FingerJo Posted at: 2018-12-26T13:45:09.457Z Reads: 127

```
[quote="rich, post:131, topic:43108"]
Go for a ride **now** !
[/quote]
Hah i wish, but i don't have the components and filaments yet. Also i really wanna test everything through on the bench before i jump in the snow and find it out the hard way :smiley:

[quote="rich, post:131, topic:43108"]
Is the alignment better with the new mounts? If you still have problems you could buy a [precision hanger/truck ](http://www.trampaboards.com/cnc-precision-vertigo-emtb-truck---16-inch-wide-with-12mm-hollow-axles-with-vertigo-baseplate--steel-kingpin--p-26391.html) with cnc’d hanger.
[/quote]

Yeah i saw those... 
My alignment is done exclusively by the axle, the mount isn't touching the uneven surface of the hanger. Once it's in position, i fill the remaining gaps with hot glue (for testing) and eventually sugru. Compared to my old way of mounting with the grub screws, it's soooo much better aligned and i think it won't be an issue now.

If everything else fails i will take a second look at the machined trucks, but for now i remain stubborn :D
```

---
## \#133 Posted by: Falcon87407 Posted at: 2018-12-26T14:44:04.752Z Reads: 126

```
are you supplying the STL for these prints? I would like to test this setup as well.
```

---
## \#134 Posted by: Der6FingerJo Posted at: 2018-12-26T15:28:33.426Z Reads: 124

```
I will do once i test them, they aren't 100% final yet :sweat_smile:
```

---
## \#135 Posted by: Fraserrazor Posted at: 2019-04-08T12:52:47.444Z Reads: 104

```
Updates? Re-resurrection.
```

---
## \#136 Posted by: Der6FingerJo Posted at: 2019-04-08T15:14:03.400Z Reads: 103

```
i know i know :sweat_smile:

I've printed both motor mounts and polycarbonate gears, as well as a new VESC Box and i'm now waiting to be back home again and build everything up. I still have to do the remote though, but i hope i can report something in the next month. Uni is a bit tough right now :smile:
```

---
## \#137 Posted by: Flexboardz Posted at: 2019-04-14T17:00:09.880Z Reads: 93

```
Thanks a lot for all your great work and all the experiences you shared with us.

Considering your taste for big torquey motors, big wheels and offroad and the fact that your gearings handle all this without problem, would you advice reducing the gear module (or width) for a 8" urban mtb with smaller motors?
```

---
## \#138 Posted by: Der6FingerJo Posted at: 2019-04-15T07:39:34.236Z Reads: 93

```
@Flexboardz
 I've actually thought about decreasing the size of the teeth, but didn't do it because of the steel gears I already have on the motors. I would also need to switch to a smaller nozzle for printing module 1 I think, so I'd say 1.5 would be the next logical step. 

I'd see no problem in using smaller motors for an urban board. I'm at 100kg with full gear and I almost never need more than 50% of the power this board has. I have it set up the way it is because I never wanted to ride fast anyways, and this way I have enough power for all off-road stuff and the motors and controllers stay cool when riding in hilly areas, which is most of the time for me. 

The bottleneck for this board are definitely the tires. The power is there, it's mostly grip that's limiting off-road riding in really really messy conditions.
```

---
## \#139 Posted by: Flexboardz Posted at: 2019-04-15T12:04:27.156Z Reads: 81

```
Thanks for your answer.
I agree with you that the final bottleneck is the tire, its grip and/or wear... which is limited.

I have the feeling that except for real offroad use with hills and mud (your case), it should be possible to seriously downsize the powerchain (motor/gear/esc) to make it lighter/cheaper/reliable.
```

---
## \#140 Posted by: Der6FingerJo Posted at: 2019-04-15T14:51:38.096Z Reads: 77

```
I agree. Although for exclusive urban use, i wouldn't go for 8" tires. 7" or the 6.5" Urban threads seem to be made for exactly that scenario.
```

---
## \#141 Posted by: Flexboardz Posted at: 2019-04-15T15:43:40.665Z Reads: 72

```
Agree for the tire diameter and it made the question of the gearing size/module even more critical (specially in my case with leaning wheels )
```

---
## \#142 Posted by: Flexboardz Posted at: 2019-04-15T20:18:08.862Z Reads: 72

```
And I keep in mind that a bicycle rider (even on steroids) delivers 300/400 W max and still reach 40+ km/h, climb mountains, ... so why do we need 2000 W on our boards?
```

---
## \#143 Posted by: Der6FingerJo Posted at: 2019-04-15T20:22:55.389Z Reads: 75

```
It would be really cool to see thist drive on the leaning wheels :smiley:

Our Boards can't tap into all the gears a bicycle usually has, so you have to find a sweet spot for your board. Personally i don't like boards that can potentially reach 70km/h or so while constantly overworking the motors on small inclines, but it really comes down to your weight and riding conditions.
```

---
## \#144 Posted by: ducktaperules Posted at: 2019-04-15T22:52:19.593Z Reads: 68

```
[quote="Flexboardz, post:142, topic:43108, full:true"]
And I keep in mind that a bicycle rider (even on steroids) delivers 300/400 W max and still reach 40+ km/h, climb mountains, … so why do we need 2000 W on our boards?
[/quote]

just like to point out that a bicycle rider has gears. low gear on a bike can be up to 5:1 and so produces lots of torque. We dont have changeable gear ratio so we need more watts to get the required torque for acceleration and hill climbing. In reality high speed cruising does not use that much power but you need that power when you get to a hill.

You never see that 400W steroid fuelled bicycle rider doing 40+ km/h while he is climbing mountains.
```

---
## \#145 Posted by: Flexboardz Posted at: 2019-04-16T10:07:20.330Z Reads: 69

```
I agree with Der6FingerJo and ducktaperules that : 
1) the gearing ratio is critical (that's the meaning of all your work above with a "sweetspot" around 1/5, if I read well) 

and 2) if we are more "reasonable" in our expectations (on/offroad, speed, torque/climbing ability...) it might be possible to design lighter/better/cheaper boards... 

For an old rider like me, being able to cruise at 30km/h on a flat beachwalk is already a phantasm and riding roads, beaches or dirt tracks at 50 km/h is serious s**t (don't even mention 70 km/h)...and as skier, I am used to manage my speed/ride according to slope (that's even a large part of the fun)...so few 100W (effective) could makes me happy...

One of my Flexscoot basically did it with +-1000W ...but it was a scooter (large/heavy).

Thanks for your kind words. I'm now building a new EFlex (see below) trying to integrate smartly electric components and as you all know, transmission is the key point today (so you know why I'm polluting your post)...
http://flexscoot.com/img/cms/BLOG/EFLEX/EFLEXGP1.JPG
http://flexscoot.com/img/cms/BLOG/EFLEX/EFLEXside1.JPG
```

---
## \#146 Posted by: Der6FingerJo Posted at: 2019-05-01T21:02:11.812Z Reads: 56

```
Guys...
I've just been finishing up the remote part of the board when one of my Trampa VESC 6 died on the bench. I wanted to test everythin out tomorrow... ugh.

While i'm searching for a possible fix, here are the details if any VESC guru's stumble upon this and can help me:

(keep in mind, both vescs were working fine and i see **no obvious electrical fault**)

- both VESC 6's sitting on the bench with battery connected, no motor connected, no can connected
- on one vesc an Arduino Nano is connected via **5V, GND from Servo port and RX/TX on serial port**
- on and connected for about **15min** at this point
- Arduino is transmitting Data via a LoRa Module
- when i turned on the other Arduino (a.k.a. VESC Arduino now receiving data) i heard a pop
- Diode on the VESC Arduino popped, Arduino is dead
- VESC is dead, too, **only blinking red once at startup**
- no visible damage on the VESC PCB at all
- STM gets a little bit warm after a minute, but i think thats normal
- 5V still available on the ports

so my idea is that something in the arduino went bad and it somehow broke the STM MCU via the rx/tx lines. 

I'll appreciate any input on this!

(sorry if this all is a bit scrambled, it's late and i'm tired from this stuff :sweat_smile:)
```

---
