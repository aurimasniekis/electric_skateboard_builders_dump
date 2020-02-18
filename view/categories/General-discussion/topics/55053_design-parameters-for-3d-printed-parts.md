# Design Parameters for 3D printed parts?

### Replies: 14 Views: 477

## \#1 Posted by: LAVAMAN Posted at: 2018-05-10T21:56:52.755Z Reads: 128

```
I studied plastic injection molding in college years ago. The 3 main rules for good parts were consistent part wall thickness, generous radii and draft. These 3 basic rules insured good results when molding plastic parts. My question is this. 

What are the basic rules of "3D printing" plastic parts to get good results? 

I am designing a riser/spacer for a battery enclosure but I want a generous wall thickness (.75 - 1.0 inch thick x 1.0" tall). Is that ok? Should I hollow it out with a spider web of triangles or holes so it is thick but not solid? The reason I want this thickness is to match the flange on my enclosure and also to create surface area for attachment to the bottom of skateboard with 3M dual lock tape (no screws). 

When I am done I will be looking for someone on the forum to print it for me.
```

---
## \#2 Posted by: pakue Posted at: 2018-05-10T22:06:03.168Z Reads: 124

```
The design rules I go with are usually:

* Avoid high strain between printing layers
* Design with printing orientation in mind (no/fewer support during printing)
* More than 70% infill doesn't give much more strength
```

---
## \#3 Posted by: skatardude10 Posted at: 2018-05-10T22:11:35.665Z Reads: 119

```
The only thing wrong with more walls/bottom/top surfaces is material usage and print time, which if contracting a print will drive up the cost _a lot_. A small but volume dense part can quickly add up to a lot of filament. The general rule is 3 or more walls on a 0.4mm nozzle for strength. I usually do 5 or even 6 walls for strength though. As long as you have enough walls, you can have quite low (15-20%) infill and still have a very strong/rigid part. 

When it comes to skateboard parts, especially load bearing parts... such as riser pads... I feel much safer just doing 100% infill with 5 walls. Infill itself doesn't add much to a structures strength, that's mostly the walls that do that.... but (common sense says) this mostly applies to infill percentages below 100%... a solid brick of plastic is obviously it's own beast of strength.

For a battery enclosure riser though, there is only going to be so much weight on it... not 200 lbs impact force or more that a riser pad might take though- I don't expect you are going to be torquing it down too hard... opting for threadlocker blue or something instead with a simple (quite) tight fit with just _quite a bit_ of torque instead of _a lot_ of torque with impact forces.

For the enclosure riser, i'd personally go for 4 walls, 5 if you want super _duper_ peace of mind, with 35-45% infill... and 1.2 - 1.6mm tall tops and bottoms.
```

---
## \#4 Posted by: Achmed20 Posted at: 2018-05-10T22:17:52.939Z Reads: 93

```
i'd say that more then 50% infill doesnt give more strength. 30% is usualy more then enough.

my tips would be
- keep printing orientation in mind. cutting parts and glueing them together afterwards is perfectly fine.
- orientation is also important for strength. avoid pulling forces on the layers.
- mind your printer tolerances. your printer probably cant do 0.2mm spacings between parts. so dont expect tight tolerances
- PLA, PETG, ABS and Nylon have VERY different properties. some shrink, some expand, some jsut rot with time.
- parts strength comes from wall thickness (i usualy use 4 layers) and thats way ...
- ... 30% infill usualy is enough
- and prepapre to do prototype prints alot :slight_smile:
```

---
## \#5 Posted by: skatardude10 Posted at: 2018-05-10T22:28:56.426Z Reads: 86

```
Great point. 0.25mm spacing between parts for a tight fit and 0.3mm for a slightly looser fit is a perfect tolerance for my printer. 

Hopefully, @LAVAMAN, whoever you get to print your part knows their printer's tolerances, and when you draw up your design, you can design around their tolerances. For reference, 0.4mm tolerance is pretty shit, and 0.1mm is _shit hot_. 

An enclosure riser _will_ need multiple parts glued or parted together. I'd suggest those  \_\\-/_ shaped cuts to join all the parts... they have worked well for me, with 0.3mm space between the faces along the cuts. That way, when you glue them together, they are already structurally joined, they just need glue to hold them together a bit so they don't slide apart.
```

---
## \#6 Posted by: LAVAMAN Posted at: 2018-05-11T03:37:23.537Z Reads: 68

```
This enclosure is going to contain 2 x 6S LIPO's and have a XT-90 panel mount on 1 end for antispark and maybe voltage (gas) gauge. Basically a box with no bottom and no top. I have been looking at printers and a Creality CR-10 will print something like 8.75 inches by 8.75 inches. I figured with a printer like that I might be able to do it in one piece. I might also have machined in black nylon at local machine shop. Have to get more info. before making a decision. 

I assume the tolerances get sloppier the larger the part you are trying to print?
```

---
## \#7 Posted by: TowerCrisis Posted at: 2018-05-11T04:02:33.568Z Reads: 64

```
I'm surprised by people saying that more than 50% or 80% infil doesn't help.

In my experience, 100% infill is important. It greatly increases compressive strength horizontal to layers. And it will greatly increase layer adhesion.

BUT this is only the case for some filaments. PLA will not benefit strongly from 100% infil (although I still would do it to be safe). Other filaments such as ABS are very difficult to print large pieces in 100%. Others like PETG, PET+, and Edge (based off of PETG, which is polyester) will become stronger. Edge will become a solid piece of plastic at 100% infil, will be impossible to delaminate, and will effectively be as strong as an injection molded part.

I highly recommend edge by e3d. It's the only thing I use for ESK8 and have full faith in it for wheel pulleys and entire enclosures. Had several nasty crashes and never broken a printed part.

Here's a picture of a break through layers of 100% infil. It should make sense why a solid piece will be stronger with this material.
![edge3|602x450](upload://iZUNsXEd96R4b5jpziWNhmTY0sv.jpg)

Now onto some more detail..

From my experience, the more wall surface area, the harder the print will be to make. Printers will try and make nice outer faces and typically run slower on these exposed layers. You can cut down on weight by decreasing infil, or by creating a lattice inside.

Based off of your description, I would recommend a honeycomb shaped pocketing of the part. I'd say leave 0.125 - 0.25 inch wall thickness between the hexagons, which leave the part ~50% air by volume where pocketed. On the outer edge of the part, I think a solid 0.25 inch thickness is good.

Also, I'm interested in this print. I'd do it for you, I'm actually on a flight home right now and will have access to my printer again soon. Let me know any way I can help, feel free to bring this to PM if you'd like. My size limits are 8x10x12 inches, but parts can be split up.
```

---
## \#8 Posted by: Der6FingerJo Posted at: 2018-05-11T08:58:13.938Z Reads: 52

```
In my experience, the thickness of the outer shell is way more important than infill. I'd much rather do a part with 3mm outer wall thickness and 30% infill than 1.5mm outer wall and 70% infill. If I go for a solid part I usually crank up wall thickness enough that it fills everything instead of using 100% infill.
```

---
## \#9 Posted by: skatardude10 Posted at: 2018-05-11T10:37:37.000Z Reads: 46

```
Tolerances should be exactly the same regardless of how large the part you are trying to print is... Assuming all of your axes are properly calibrated and squared.
```

---
## \#10 Posted by: LAVAMAN Posted at: 2018-05-11T17:11:12.511Z Reads: 41

```
I like your advice. I will use honeycomb pattern as you suggest. When I am further along I will contact you about printing for me, if you are still interested.
```

---
## \#11 Posted by: Achmed20 Posted at: 2018-05-11T21:07:37.145Z Reads: 33

```
[quote="TowerCrisis, post:7, topic:55053"]
In my experience, 100% infill is important. It greatly increases compressive strength horizontal to layers. And it will greatly increase layer adhesion.
[/quote]

if you just want layer adhesion, just leave the fan off ;) 
they key to strength is usualy maintaining some sort of flexibility in order to transfer the energy into more area. a 100%infill print simply cant do that.

my first itteration was solid (petg) with  3mm wall thickness in total. it could not be bent whatsoever and after a few kilometers i hit a rock pretty hard and that thing basicly shattered

second one had 30% infill and had  3 wall perimeters (about ~1.2mm per side) and i also changed the print direction. this thing was super flexible and is plenty strong. its still holding up nicely and i hit plenty of rocks with it.
but thats pretty much what you told lavaman anyway.

this video might be interesting to watch 
https://www.youtube.com/watch?v=AmEaNAwFSfI


my 2 cents: 100% infill is just waste of material. print direction and wall thickness are the key
```

---
## \#12 Posted by: LAVAMAN Posted at: 2018-05-12T16:53:44.194Z Reads: 24

```
That video is excellent! Lots of good information.
```

---
## \#13 Posted by: danielz Posted at: 2018-05-12T17:09:07.297Z Reads: 20

```
From my experience Id say infill is more important than walls for **ABS** at least. Especially thin walled parts of 3mm or so for something like a controller. The layers will de-laminate much easier if you have the filament all going ine the same direction.

I reduced to a single wall and 100% infill for vastly strong parts. My motor mounts, controller, pulleys and enclosure are all 3d printed ABS 100% infill low number of perimeter walls. Also dont have sharp edges, use fillets everywhere otherwise parts will eventually fail at the corners etc.

Oh and drill holes afterwards rather than printing them where possible.
```

---
## \#14 Posted by: LAVAMAN Posted at: 2018-05-12T17:13:21.444Z Reads: 19

```
Drilling holes rather printing, that is an interesting option. Thanks for the tips.
```

---
