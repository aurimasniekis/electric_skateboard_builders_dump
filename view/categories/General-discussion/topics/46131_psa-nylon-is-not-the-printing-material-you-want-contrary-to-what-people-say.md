# PSA: Nylon is not the printing material you want, contrary to what people say

### Replies: 51 Views: 2229

## \#1 Posted by: notepad Posted at: 2018-02-11T19:41:14.375Z Reads: 314

```
In short i've have been seeing various posts about printed parts and everyone eventually says that Nylon ( or an Nylon alloy ) is what the part should be printed out of for the best performance.

Nylon is Hygroscopic, and will absorb moisture.  even after printed and will slowly affect its characteristics and will weaken the overall part.

The real reccomendations should be PETG or any material that is not hygroscopic.  This means that nylon and PolyCarbonate are inadaquate choices.
The best thing to do is  **DONT** try to make it like if it was machined out of metal.  design parts that are specifically intended to be printed and keep it in mind.

>

If you want to print something. consider these materials instead:

Is the part not going to get hot - PLA/PLA+

Is the part going to get hot - ABS/ABS+/PETG

Is the part going to be under stress - PLA+/ABS+/PETG

Do you need dimentional accuracy - PLA/PLA+/PETG

If I had to choose one material - PETG ( if your printer is allmetal, otherwhise PLA+ )

_Note: ABS/ASA is quite ductile and suprisingly bendy under stress. keep that in mind if you want to use that material._

    Source: Worked with and around industrial printed parts and the people who design them.

EDIT: PLA is also Hygroscopic. at worst it seems like the material will loose 30% of its strength.
```

---
## \#4 Posted by: PXSS Posted at: 2018-02-11T19:51:24.604Z Reads: 295

```
PLA is also hygroscopic
```

---
## \#5 Posted by: bigben Posted at: 2018-02-11T19:53:35.075Z Reads: 287

```
This is music to my ears.
I have just got a 3d printer and seem to be managing to get pretty tidy prints out of PTEG.
```

---
## \#6 Posted by: PXSS Posted at: 2018-02-11T20:03:17.587Z Reads: 278

```
Thoughts on this data?

![image|512x343](upload://1TZWxT59hL5jCnR6j74mxf3AklU.png)
```

---
## \#7 Posted by: deucesdown Posted at: 2018-02-11T20:12:27.107Z Reads: 260

```
Charts like these don't have enough info. Usually ductility is missing.

I've been trying to figure out properties of filaments too. petg has a good balance unless you need high heat or lots of bridging. Nylon and polycarbonate have good properties but are a pain to work with, almost prohibitively so. Abs is almost not worth considering.

And the more I try, TPU/flex is good for many of our nonmechanical applications. Horrible for motor mounts but might be great for risers, cable brackets, mounts for lights, bumpers, maybe even panel mounts.
```

---
## \#8 Posted by: notepad Posted at: 2018-02-11T20:15:03.852Z Reads: 250

```
Completely forgot about pla being Hygroscopic.  will edit it in.
```

---
## \#9 Posted by: ShutterShock Posted at: 2018-02-11T21:36:56.339Z Reads: 227

```
Why would you say that ABS is not worth considering?  I always get almost perfect prints with ABS and they hold up really well
```

---
## \#10 Posted by: akhlut Posted at: 2018-02-11T21:59:50.187Z Reads: 219

```
https://www.youtube.com/watch?v=8_adY2K-YIc

https://www.youtube.com/watch?v=YCdvL87bv0w
```

---
## \#11 Posted by: deucesdown Posted at: 2018-02-11T22:25:13.824Z Reads: 205

```
I'm still learning but abs seems to shrink/warp a lot so not as good for dimensionally correct parts. High temp tolerance is just a bit more than petg, and strength of printed parts don't seem much better than pla, and overall seems not as strong as petg.

And abs smells bad when printing :)

Oh I forgot, abs I believe has better UV resistance than pla or petg so will hold up better outdoors.
```

---
## \#12 Posted by: ShutterShock Posted at: 2018-02-11T23:39:16.676Z Reads: 190

```
Ah okay I see where you are coming from.  I would agree that it is a bit harder to get dialed in, but once you've got the settings finished, I got warp free prints and it was one of my favorite materials to print in.

And yes abs is way better for outdoors cuz it's not hygroscopic.  Would be bad for my enclosures to fall apart because of water haha
```

---
## \#13 Posted by: Riako Posted at: 2018-02-12T10:49:59.555Z Reads: 179

```
Hi, maybe not the write place but, I post this on esk8-fr neighbour fourm : 
https://youtu.be/CZX8eHC7fws
Did somebody already test that method ?!
```

---
## \#14 Posted by: Der6FingerJo Posted at: 2018-02-12T11:43:56.782Z Reads: 169

```
I wrote with taulman3d about water resistance of Alloy 910, the Polycarbonate - Nylon blend and described my usecase as exposed to heavy dirt, mud and water. They told me the material will be fine as long as I don't fully submerge it for extended periods of time. 
Take it how you want, I didn't find any soft spots or stuff on my gears after 6 weeks of using them in rainy/snowy conditions.
```

---
## \#15 Posted by: Vanarian Posted at: 2018-02-12T23:40:54.796Z Reads: 164

```
Now that's a useful thread! Note that nylon and PETG has their own advantages but clearly for e skate parts PETG is the best. Cost effective and strong, stiffer and easier to print.

When comparing both I got stronger part out of PETG. I was using Taulman Bridge BTW. 

Another material which needs to be known is HIPS filament, it is not hygrophobic, and is super accurate to print and resistant. It resists heat too.
```

---
## \#16 Posted by: fottaz Posted at: 2018-02-13T00:19:38.285Z Reads: 156

```
Is this just theoretics? or have you tried nylon to say this?
I'm asking since I'm printing Nylon pulleys since 13-14 months, they are in all my builds and I live in a very soaked area in Italy, and they all still be like new as the first days.

Moisture, hot, rocks, seem not to be a problem.

I think a lot of people avoid nylon just because is hard to print , I would never say it's not one of the best materials, since it is, for our applications
```

---
## \#17 Posted by: Der6FingerJo Posted at: 2018-02-13T06:23:39.613Z Reads: 143

```
I always thought about testing this but was put off by the deformation. iirc tom said about 2-3% shrinkage in z and 5% extension in x and y direction (might have been the other way around). When printing gears that are exactly planned to go along with motor mounts i don't want either one of these to have different dimensions than what i planned and i don't think you could exactly plan those deformations ahead.

[quote="Vanarian, post:15, topic:46131"]
Another material which needs to be known is HIPS filament, it is not hygrophobic, and is super accurate to print and resistant. It resists heat too.
[/quote]
@Vanarian how hard is it to print this? I heard it's harder than ABS which is way out of my comfort zone already.
```

---
## \#18 Posted by: chuttney1 Posted at: 2018-02-13T06:51:22.419Z Reads: 134

```
I'm for sure all the plastics listed here are hygroscopic to some degree. That being said ABS, Nylon, PLA, or PETG are fine depending on where it is used.
```

---
## \#19 Posted by: Vanarian Posted at: 2018-02-13T07:41:11.861Z Reads: 132

```
You can print it starting around 220 degrees C but 230-240 might be the sweet spot.

If you have a heated bed it is better :+1: if you can print ABS I see no reason why you couldn't print  HIPS (and it doesn't retract BTW)
```

---
## \#20 Posted by: psychotiller Posted at: 2018-02-13T07:58:16.969Z Reads: 132

```
I can say, without a doubt, Nylon will outlast petg and abs in any pulley or hub application. Nylon also will not crack or shatter when impacted by rocks or flexed too far. Glass filled nylon pulleys are more durable than aluminum and steel pulleys. We've tried, PLA, PETG, ABS and Nylon. Whether it is hydoscopic or not. Nylon is more durable.
```

---
## \#21 Posted by: Vanarian Posted at: 2018-02-13T08:26:44.712Z Reads: 133

```
Funny we got inverted results. 

If you can print it properly sure nylon is strong, elasticity and low friction are a must (if you don't need stiffness). But when it fails it shreds. Being able to cast it instead would tremendously improve  parts structure though (no more layers shredding). 

Best settings I got with Nylon were 240 nozzle, 85 bed for three first layers then cooled down bed (else it warped the base), no fan on nozzle. 

I didn't try rock impacts, instead I went for good ol' hammer experiments and also bolting through on both, I found PETG more durable upon smashing attempts. Layers simply melt together during print, it holds itself until breaking but no "layer splitting". Impacts remain on surface, internal structure doesn't get damaged unless hit is strong enough to crack through.

Nylon has this nice rebound against hits and until a certain point, can extend and come back. But layers shreds too easily losing the benefit of the elasticity. 

Since I don't have a more performant printer I wouldn't go back to nylon, too much restrictions plus steep price (super expensive compared to PETG or HIPS). And again I need stiff parts over elastic parts, this might not be the case for pulleys (people should experiment both if possible). 

Maybe you could share your print settings?
```

---
## \#22 Posted by: Der6FingerJo Posted at: 2018-02-13T08:35:16.710Z Reads: 127

```
[quote="Vanarian, post:19, topic:46131"]
You can print it starting around 220 degrees C but 230-240 might be the sweet spot.

If you have a heated bed it is better :+1: if you can print ABS I see no reason why you couldn’t print  HIPS (and it doesn’t retract BTW)
[/quote]

Sounds good, i've got a CR10 and it should be able to do that. Just need an enclosure for the damn thing because i don't want the smelly smells that smell in my room.
Also thinking about getting a CETUS Printer for those more exotic filaments.

[quote="Vanarian, post:21, topic:46131"]
Best settings I got with Nylon were 240 nozzle, 85 bed for three first layers then cooled down bed (else it warped the base), no fan on nozzle.
[/quote]
Speed would also be a huge factor as well as what kind of nylon and petg filament you are using (sorry if i missed it in a post above).
I know i'm repeatedly praising Alloy 910 but it is really great. Stiffer than Nylon with even more impact resistance, can print my gears with 50mm/s speeds and with glue and a brim there's no warping at all at ~30°C to 35°C in my plastic bag enclosure.
Bridges the Gap between Nylon and stiffer materials for me. For Motor mounts i'm still using PLA but everything else will be Alloy 910 soon.
```

---
## \#23 Posted by: fottaz Posted at: 2018-02-13T12:18:37.999Z Reads: 109

```
Yes man. And also nylon carbon fiber is very very good, you should try!
```

---
## \#24 Posted by: fottaz Posted at: 2018-02-13T12:20:53.928Z Reads: 113

```
Im printing nylon carbon at 260 Celsius and hot hot bed at 110°

Glued bed too

And skirt brim of 30 outlines 😁 

It's HARD to print yes 👌😁
```

---
## \#25 Posted by: psychotiller Posted at: 2018-02-13T15:49:19.969Z Reads: 102

```
@mccloed is our printmaster. He brought a pulley over that was made out of the Nylon carbon and it seems really nice. He said the size increases though, so the finished product wasn't actually htd5.
```

---
## \#26 Posted by: Achmed20 Posted at: 2018-02-13T15:58:30.480Z Reads: 107

```
nah, im not with you on this on here.

- While PETG is pretty awesome, its also rather "explosive". meaning it wont realy bend, but rather shatters into thousends of pieces. thats why PETG is not the greatest merterial parts which are under mechanical stress.

- PLA is OK for everything which doesnt have to move. like cases or covers. maybe also for the large pulley but definatly not for the small one. but then again, PLA deteriorates rather fast and bercomes very brittle.

- nylon has a certain amount of flex to them and thats why they are so great for mechanical parts.

also, the hydroscopic part doesnt realyy matter. it not like they are going to absorb their weight in water. it jsut sux for printing. nearly Every filament out there is hydroscopic, even PETG. but once printed, it doesnt matter.
```

---
## \#27 Posted by: notepad Posted at: 2018-02-13T16:04:50.426Z Reads: 106

```
I have had experiance with nylon, but I havent had anything fail due to moisture absorbtion.  I have however noticed a difference in the materials properties over time which meant the part wasnt in its intended use case and got remade in PETG.

Im not saying Ny isnt a good material, Im just relaying information which I and many others use in industrial aplications as a change in properties tends to lead to catastrophic faliure.
```

---
## \#28 Posted by: riva_00 Posted at: 2018-02-13T16:13:39.312Z Reads: 105

```
I wouldn't have thought you could print a motor mount or motor pulley, I've seen a couple of motor mounts on here i think, but they were very bulky and were very much in the experimenting phase.
```

---
## \#29 Posted by: Achmed20 Posted at: 2018-02-13T17:30:40.735Z Reads: 104

```
printed pulleys work great with PETG, Nylon or ABS. 
Mounts however usualy need some sort of reinforcement like insert metal rods.  at least the PETG ones. 
A nylon mount might be a tad bit to flexiable as mount but i never tried that.
```

---
## \#30 Posted by: notepad Posted at: 2018-02-13T18:03:26.735Z Reads: 105

```
[quote="Achmed20, post:29, topic:46131"]
nylon mount might be a tad bit to flexiable as mount
[/quote]

Can confirm, and gets worse with time.
```

---
## \#31 Posted by: fottaz Posted at: 2018-02-13T19:23:39.058Z Reads: 100

```
Over extruded or something like?
```

---
## \#32 Posted by: fottaz Posted at: 2018-02-13T19:30:12.423Z Reads: 98

```
I'm using Nylon mount on Mountainboard, with 20mm thickness, no problems :smiley:
```

---
## \#33 Posted by: longhairedboy Posted at: 2018-02-13T20:41:45.684Z Reads: 98

```
[quote="fottaz, post:16, topic:46131, full:true"]
Is this just theoretics? or have you tried nylon to say this?

I’m asking since I’m printing Nylon pulleys since 13-14 months, they are in all my builds and I live in a very soaked area in Italy, and they all still be like new as the first days.

Moisture, hot, rocks, seem not to be a problem.

I think a lot of people avoid nylon just because is hard to print , I would never say it’s not one of the best materials, since it is, for our applications
[/quote]

yeah, same here. I've been using sintered nylon wheel pulleys for well over a year now with zero issues. They perform better than even aluminum in my opinion. They last just as long and don't shred belts every time a rock deforms a tooth. 

i think he's talking about regular 3D printers though and not industrial scale sintering.  Running wheel pulleys from a desktop 3D printer probably wouldn't be the best idea.
```

---
## \#34 Posted by: Achmed20 Posted at: 2018-02-13T21:34:22.215Z Reads: 96

```
[quote="fottaz, post:32, topic:46131, full:true"]
I’m using Nylon mount on Mountainboard, with 20mm thickness, no problems
[/quote]
pics and STL please ;)

[quote="longhairedboy, post:33, topic:46131"]
Running wheel pulleys from a desktop 3D printer probably wouldn’t be the best idea.
[/quote]
nope, all fine. works like a charm if you print it properly.
```

---
## \#35 Posted by: TarzanHBK Posted at: 2018-02-13T22:14:00.661Z Reads: 93

```
What printer are you running by the way?
```

---
## \#36 Posted by: notepad Posted at: 2018-02-13T22:27:52.994Z Reads: 93

```
[quote="longhairedboy, post:33, topic:46131"]
i think he’s talking about regular 3D printers
[/quote]

Hit it right on the head.  Sintered parts are chemically much more resistant.  if you have the machine, your golden ( and IM jelous :P )
```

---
## \#37 Posted by: fottaz Posted at: 2018-02-13T23:26:00.238Z Reads: 93

```
I've built my own black widow from Tevo 

Titan extruder
```

---
## \#38 Posted by: fottaz Posted at: 2018-02-13T23:29:30.604Z Reads: 92

```
Pics coming soon, sharing the STL it's a problem for me since I'm selling them.
```

---
## \#39 Posted by: fottaz Posted at: 2018-02-13T23:33:21.882Z Reads: 90

```
I'm printing with desktop 3d printer, nothing more than a fdm printer
```

---
## \#40 Posted by: fottaz Posted at: 2018-02-13T23:36:27.920Z Reads: 95

```

![IMG_20170915_005453|377x500](upload://rVC6pg8v8PSkGimjIcUp0vfQNJp.jpg)
![IMG_20171130_112252|377x500](upload://8pxyP7wa8Z1GORcDyX0sfCClqju.jpg)
```

---
## \#41 Posted by: topcloud Posted at: 2018-02-13T23:37:03.304Z Reads: 96

```

edited: not that soon (just checked, it's Q4) :frowning:

https://formlabs.com/3d-printers/fuse-1/

https://www.youtube.com/watch?v=BALUeGV57dE
```

---
## \#42 Posted by: mccloed Posted at: 2018-02-14T05:13:24.264Z Reads: 91

```
I have been running 3D printed pulleys for hundreds of miles with very little sign of wear. They are printed on a desktop Flashforge creator. I’ve been using cheap nylon from Microcenter http://www.microcenter.com/product/485160/175mm_Natural_Nylon_3d_Printer_Filament_-_05kg_Spool_(11_lbs)
Unfortunately, this is the only color they have. Kinda lame.:grimacing: I’ve had a couple pulleys printed by shapeways and they are good in the sintered nylon but they are no better than what I can print except for the aesthetics.
```

---
## \#43 Posted by: riva_00 Posted at: 2018-02-14T10:40:50.873Z Reads: 86

```
I'm interested mainly in a printed *motor* pulley, i can do a wheel one easily as i use a 6" tyre with a 60+ tooth pulley there, the stresses and heat are spread over a wide area. I haven't yet seen a printed motor pulley (at least not one that survives very long).
I've also never seen anyone mention a motor mount printed in PC, however that's not exactly easy to print with. PC-Max is probably the right stuff for that, but I'm only just beginning the 3d printing journey, and regardless the best way of testing would be to just print it and see if it disintegrates :slight_smile:  ....

Thinking about it i suppose the motor gear is small enough to 1st print to test, then get shapeways to make it in metal......
```

---
## \#44 Posted by: fottaz Posted at: 2018-02-14T10:58:19.327Z Reads: 85

```
I desperately tried at the beginning (end 2016) to print motor pulleys, with a m4 set screw. 
The best worked for 100 meter 😂

14-15 teeth are too small diameter and the print could be not strong as needed , i did not try with 16-18T that would be great and more feisable, with keyway.
```

---
## \#45 Posted by: Achmed20 Posted at: 2018-02-14T11:10:31.668Z Reads: 81

```
[quote="fottaz, post:44, topic:46131"]
I desperately tried at the beginning (end 2016) to print motor pulleys, with a m4 set screw.
[/quote]
yup. screws wont last unless its going all the way through the motor shaft. learned that the hard way as well.
now, i filed a D shape into the motor shaft and just glue the pulley onto it.
```

---
## \#46 Posted by: Der6FingerJo Posted at: 2018-02-14T11:17:02.201Z Reads: 80

```
[quote="Achmed20, post:45, topic:46131"]
yup. screws wont last unless its going all the way through the motor shaft. learned that the hard way as well.

now, i filed a D shape into the motor shaft and just glue the pulley onto it.
[/quote]

I was also thinking about printed spur gears with keyway and a filed spot. What kind of glue do you use?
Printed gears would maybe allow for helical gear setups.
```

---
## \#47 Posted by: telnoi Posted at: 2018-02-14T11:44:35.485Z Reads: 76

```
hmm, your typical soft drink bottle is made out of PETG. It deforms rather than shatters/explodes, which is also my experience when using it for motor mounts. It flexes way more than PLA does (in fact, to such a degree where it no longer returns to its original shape), but less so than nylon.
```

---
## \#48 Posted by: Der6FingerJo Posted at: 2018-02-14T11:52:39.748Z Reads: 75

```
I had similar experiences with PETG, the motor mount flex more under the weight of the motor and my threaded inserts cracked the part open from within (should have screwed them in hitter but still). Both not as present when using PLA.
```

---
## \#49 Posted by: telnoi Posted at: 2018-02-14T11:57:59.726Z Reads: 75

```
Threaded inserts are a no-go for PETG & PLA, unless the screws are relatively large and you are using loads of perimeters. I tend to go with clamped designs. Now switched to CNC alu....sadly, 3d prints don't compare :slight_smile:
```

---
## \#50 Posted by: Der6FingerJo Posted at: 2018-02-14T12:06:17.885Z Reads: 77

```
I'm using inserts originally made for wood applications so the thread itself is really big and chunky, then i print the part with a hole 2mm smaller than the insert and heat it up to gently screw it in. When all is cooled down the insert is surrounded by plastic that melted into every nook and cranny of the thread and it holds beautifully, didn't manage to break an insert free when screwing in the grub screw.
A clamped design sounds good too, maybe i'll try next revision.
```

---
## \#51 Posted by: longhairedboy Posted at: 2018-02-14T12:06:29.772Z Reads: 75

```
[quote="notepad, post:36, topic:46131"]
Hit it right on the head.  Sintered parts are chemically much more resistant.  if you have the machine, your golden ( and IM jelous :stuck_out_tongue: )
[/quote]

maybe one day. For now i use Shapeways. We couldn't be happier with the wheel pulleys's performance. The price is kind of terrible per unit, but if you want a functional, long lasting part on demand in any color with decent tolerances you have little choice. Its either a bunch of money for the part with access to 26 other variations in tooth count and all the primary colors, or a bunch of money for the mold fees and only one variation in tooth count in one color. 

didn't seem like much of a choice really.
```

---
## \#52 Posted by: telnoi Posted at: 2018-02-14T12:08:09.150Z Reads: 77

```
Good approach. The small threading is usually what causes the issues (even when working with softer alu types).
```

---
## \#53 Posted by: Achmed20 Posted at: 2018-02-14T14:10:54.945Z Reads: 75

```
[quote="telnoi, post:47, topic:46131"]
hmm, your typical soft drink bottle is made out of PETG. It deforms rather than shatters/explodes,
[/quote]
if its thin its flexible, but the more solid i gets, the more unstable it becomes. thats at least my experience.
ps: bottles are made from PET. the Glycol is missing there

[quote="Der6FingerJo, post:46, topic:46131"]
I was also thinking about printed spur gears with keyway and a filed spot. What kind of glue do you use?
[/quote]
i was using the luctide 910?. cant remember its name but technicaly its for glueing metal and not nylon.
took ages to cure but i did it during the winter time. 
probably not the best glue you could use. normal supoerglue would be enough i think but i havent had that at hand at the time.
```

---
