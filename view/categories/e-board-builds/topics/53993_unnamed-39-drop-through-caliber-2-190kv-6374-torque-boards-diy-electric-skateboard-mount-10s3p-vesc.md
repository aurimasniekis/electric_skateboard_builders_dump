# Unnamed &#124; 39” drop through &#124; Caliber 2 &#124; 190KV 6374 Torque Boards &#124; DIY Electric Skateboard Mount &#124; 10S3P &#124; VESC

### Replies: 11 Views: 1325

## \#1 Posted by: clistpdx Posted at: 2018-05-01T03:56:03.370Z Reads: 259

```
Hello! This is my first build. I’ve used longboards before but never an electric one. Just sounded like fun to learn how to put it all together. Still need to come up with a name for this thing. I cut the grip tape design to look like Mt. Hood (largest mountain in Oregon, where I live), so I wonder if there’s a name related to ‘Hood’ ‘In Tha’ Hood’, etc…

Part List:
**39” drop through deck** - natural (I painted the underside red enamel)
https://www.mboards.co/collections/decks/products/39-drop-through-deck-natural

**10s3p battery w/ integrated switch, charger port, and 2A charger**
https://www.mboards.co/collections/batteries-1/products/10s3p-battery-complete-battery-solution

**Nano Remote Controller**
https://www.mboards.co/collections/remotes/products/remote-controller-1

**1/8” rubber riser pads** (to soften the ride, not because I need more clearance)
https://www.mboards.co/products/1-8-rubber-riser-pads

**X-things** from @akhlut
https://www.electric-skateboard.builders/t/what-are-those-x-things-called/32370/53

**6374 190KV Torque Boards motor sensored**
collections/electric-skateboard-motors/products/electric-skateboard-motor-6374-190kv

**Single bolt on motor mount w/ drive wheel kit** (Kegel mount) 16/36T w/ 12MM 265mm belt
collections/electric-skateboard-motor-mounts/products/single-bolt-on-motor-mount-w-drive-wheel-kit

**Torque VESC 4.12**
collections/esc-speed-controller/products/torque-esc-bldc-electronic-speed-controller

**Psychotiller Stealth 18 enclosure**
https://psychotiller.com/product/stealth-18

**Orangatang Kegel 80mm wheels**
https://www.amazon.com/gp/product/B00EYDHWTQ/ref=oh_aui_detailpage_o01_s00?ie=UTF8&psc=1

**REDS Bones Bearings**
https://www.amazon.com/gp/product/B017YABO44/ref=oh_aui_detailpage_o01_s01?ie=UTF8&psc=1

**Caliber II 44 trucks**
https://www.amazon.com/gp/product/B0777T9PCN/ref=oh_aui_detailpage_o01_s03?ie=UTF8&psc=1

Miscellaneous Stuff:
**Grommets** https://www.amazon.com/gp/product/B01NAN025Y/ref=oh_aui_detailpage_o02_s00?ie=UTF8&psc=1
**Mini USB extension** (so I can program the VESC w/o opening the enclosure) https://www.amazon.com/gp/product/B01LYUFYP7/ref=oh_aui_detailpage_o04_s00?ie=UTF8&psc=1
**PET Braided Sleeving** to protect motor wires https://www.amazon.com/gp/product/B071ZV6MZ2/ref=oh_aui_detailpage_o06_s00?ie=UTF8&psc=1
**Blue Loctite** https://www.amazon.com/gp/product/B000I1RSNS/ref=oh_aui_detailpage_o08_s00?ie=UTF8&psc=1
**Assorted heat shrink** https://www.amazon.com/gp/product/B075WR9FVL/ref=oh_aui_detailpage_o09_s00?ie=UTF8&psc=1
**1” Velcro** for attaching battery, VESC and remote receiver to enclosure https://www.amazon.com/gp/product/B00FQ937NM/ref=oh_aui_detailpage_o01_s01?ie=UTF8&psc=1
**Blue grip tape** sheet https://www.amazon.com/gp/product/B0785L54DB/ref=oh_aui_detailpage_o01_s03?ie=UTF8&psc=1
I bought a **bluetooth module** from @Acido but have to switch one of the wires around before I can install it

**BLDC Tool Settings:**
Motor max: 50A
Motor min: -40A
Batt max: 40A
Batt min (regen): -13A
Absolute max: 130A
Max ERPM 60000
Minimum input voltage: 6V
Maximum input voltage: 57V
Battery cutoff start: 35V
Battery cutoff end: 33V
Sensor mode: Hybrid
FOC in ‘Hall’ sensor mode
App Configuration: PPM ‘Current no reverse with brake’

Blank deck:
![board|690x292](upload://rzUze2Z7Me3YHyNDGNJllAJOepg.jpg)

My grip tape design. I drew out the shape on the back of the grip tape sheet and then cut it out using a razor blade:
![griptape|690x373](upload://gZjpmHL9opTiaUlmZt9QLnKJrE9.jpg)

Battery:
![battery|406x500](upload://sFhtB15wztLEWqdJWwRKPA6fv26.jpg)

Unpictured: drilling holes in the enclosure for the M4 attachment screws, power switch, charge port, LCD battery gauge, and motor cables. Gluing weatherproofing strips along edge of enclosure.

After I re-shaped the enclosure a bit using a heat gun (while the enclosure was clamped to my board) I layed down 1/8" adhesive foam to the bottom of the enclosure. Over that I attached velcro strips that will hold down my battery, VESC, and receiver:
![enclosure1|690x392](upload://3uHigopPbxqPkXCqo4aSRYPzHtk.jpg)

I seated the battery, added some foam over the top of it, attached the solid-state switch hardware, mini-USB extension cable, plugged everything together. Note: this photo shows the stainless steel 10mm M4 inserts I placed around the underside of the board. My grip tape design doesn't cover everything so I didn't want the hardware to come all the way through. My board is 13mm thick, so the 10mm inserts were just right:
![enclosure2|690x427](upload://tsilsfxQ4D1HvggptMU1DLYUOYc.jpg)

Underside:
![underside|690x343](upload://jX8HjaT4P54XtzDttwZyCcBWqzy.jpg)

I've got about 3 inches of clearance below the enclosure. I could install the trucks drop-through but I'm worried that the motor will get pretty close to the ground and the deck:
![sideview|690x354](upload://hQAU7E1i4c9J6WiXpwH1rOqDwF5.jpg)

Final build weighs 16lbs:
![finalboard|690x358](upload://umZ9eZA3knoOo3sj8cuPGpH7zsj.jpg)

This evening I rode it down the street and back on level ground. It has a surprising amount of thrust! I’m 150lbs. Then I brought it into the shop and added thread lock to a number of the screws. Tomorrow it should be good to go.
```

---
## \#2 Posted by: b264 Posted at: 2018-05-01T04:35:27.839Z Reads: 182

```
This is badass!  :smiley:
```

---
## \#3 Posted by: b264 Posted at: 2018-05-01T04:36:34.565Z Reads: 177

```
I can suggest a name

`Suhrahngey`
```

---
## \#4 Posted by: rexpepper651 Posted at: 2018-05-01T04:52:43.834Z Reads: 167

```
whoa very nice!
```

---
## \#5 Posted by: rojitor Posted at: 2018-05-01T11:17:42.399Z Reads: 149

```
I'd name It dawn
```

---
## \#6 Posted by: Socalscare Posted at: 2018-10-09T17:14:13.102Z Reads: 91

```
How has your build been treating you since it's completion?
```

---
## \#7 Posted by: clistpdx Posted at: 2018-10-10T00:35:05.435Z Reads: 88

```
It was great. I just finished building my second build, based on the Jet Spud and Hummie's Hub's. It rained yesterday so I haven't taken it on the open road yet!
```

---
## \#8 Posted by: M.Hboards Posted at: 2018-10-10T00:48:45.787Z Reads: 83

```
how flexy is the deck? also is it possible to have the trucks mounted drop through and have clearance for the motor (not wondering about ground clearance rather will the motor hit the deck)? does the adjustability on the motor mount allow for that?
```

---
## \#9 Posted by: clistpdx Posted at: 2018-10-10T01:58:16.080Z Reads: 86

```
The deck has very little flex, though I'm only 150lbs. It was a cheap generic deck, nothing fancy. I'm not sure that the motor would have clearance if I had mounted the trucks drop-through. I think it would be close, but I never actually tried it when I was putting this together. The torqueboard mount DOES allow some adjustability in position. I wouldn't buy it, however, until they release the revised mount they've been talking about for some time. Mine was really tricky to lock down. They sent out emails a few months ago which sounded like they might send a replacement mount, but nothing ever came of it.
```

---
## \#10 Posted by: F11N3X Posted at: 2019-07-14T19:54:24.473Z Reads: 43

```
Hi @clistpdx,

is the mboards battery good?
```

---
## \#11 Posted by: clistpdx Posted at: 2019-07-15T15:27:55.047Z Reads: 35

```
It's still working, but I think there are some off and on issues with their customer service, though I haven't bought from them in over a year so maybe they've worked that out
```

---
