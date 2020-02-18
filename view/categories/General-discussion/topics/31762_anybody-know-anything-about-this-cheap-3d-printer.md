# Anybody know anything about this Cheap 3D printer?

### Replies: 25 Views: 1483

## \#1 Posted by: Dougieman1001 Posted at: 2017-08-29T18:22:31.825Z Reads: 191

```
So I'm leaning towards getting a 3D printer for longboard parts and other various small projects. I came across this kind of printer on eBay, I'm guessing its a chinese clone of a better printer maybe? There are loads of them around:

Here's the link: 
http://www.ebay.co.uk/itm/CTC-3D-Printer-Makerbot-Replicator-2-2-Extruders-1KG-ABS-or-PLA-filament/271381955044?ssPageName=STRK%3AMEBIDX%3AIT&_trksid=p2055119.m1438.l2649

I have no experience with buying 3D printers or anything, this looks like quite a good deal but I could be wrong... 
Anybody have/had this and could shed some light?

Thanks
```

---
## \#2 Posted by: wafflejock Posted at: 2017-08-29T19:46:26.189Z Reads: 166

```
I personally went with a prusa i3 based kit one where you piece it together like 3 years ago was $330.  I'd say go on YouTube search 2017 best budget (or just best) 3d printers and you'll find some options I trust Thomas and MakersMuse on YouTube they both know their stuff.  Josef Prusa makes open hardware/open source based stuff so easy to upgrade and relatively easy to upgrade firmware and stuff if you need to.  Get a raspberry pi with wifi and download octopi and turn basically any 3d printer into a wireless networked one (much better than having a computer dedicated to it or running SD cards back and forth IMO can also get a camera for live feed and timelapses from the raspi)

---
https://www.google.com/search?q=prusa+i3&oq=prusa+i3&aqs=chrome..69i57j69i60j69i61j69i59j69i60.2103j0j7&sourceid=chrome&ie=UTF-8

The mk2 is the new model it can have extra extruders attached if you want mixed materials or colors but most people just sand and paint things afterwards if they want coloring.  Can also use dual extruders for different materials but only certain materials will stick to each other well so not a huge advantage there.  Having auto bed leveling would be really nice to have, having a heated bed is absolute must for ABS or anything other than PLA really, enclosure is great but personally just built a box around my kit after it was done.

---

One other thing to keep in mind here is size.  If you plan to print battery enclosures you're going to probably want a pretty large print bed and cheaper printers will typically have a smaller print bed size since that reduces the size of everything around it (heaters, framing etc.)  Mine is 200x200x185mm build volume which is pretty typical but just be aware there are 150x150 or smaller ones in the low price range too so don't get something so small you can't print the parts you want on it.   Ideally you don't want to print all the way to the edge since running off the edge for a brim of plastic that helps hold the model down.
```

---
## \#3 Posted by: wafflejock Posted at: 2017-08-29T20:06:41.716Z Reads: 134

```
Also I just looked at the one you linked more closely it's a clone of the flash forge.  I have one in the other room here a friend left at my place because the heater cartridge started having thermal runaways so either it fried or the thermocouple that measures the temperature crapped out and this is on an "original" not even a clone.  Not saying it can't happen to any printer but think he also had a lot of wobbles with that one.

Prusa i3 is basically the VESC of 3D printing, that's the best way I can put it :)  Most versatility most open option, although lulzbot also does a lot to open all their work they're also big and expensive.

Oh also dual extruders with this setup with 2 nozzles doesn't work really because you have to know exactly the relative alignment of the nozzle tips and it changes depending on how tightly screwed in they are, so they never match.  The new i3 uses 1 nozzle and multiple tubes feed into one before getting to the nozzle so different filament can be fed in through one main tube.
```

---
## \#4 Posted by: nikoli280 Posted at: 2017-08-29T20:42:58.455Z Reads: 117

```
I dont know it. But i can recommend that you buy a Tevo Tarantula or a Icubic Mega. Both great machines at great prices
```

---
## \#5 Posted by: Dougieman1001 Posted at: 2017-08-29T20:49:43.561Z Reads: 111

```
Funny you should say that, I was just looking at the Tevo Tartantula! Was about to ask about it
```

---
## \#6 Posted by: Dougieman1001 Posted at: 2017-08-29T20:53:44.304Z Reads: 112

```
As you can see (^) I was just looking at the Tevo Tarantula Pursa i3. It looks pretty nice, Their Black widow also looks nice but is almost twice the price! If I go for it, I'd probably get the auto levelling large plate, what do you think? (Imo I the price is pretty good from what you get)

Link:
https://goo.gl/f6kpMi
```

---
## \#7 Posted by: nikoli280 Posted at: 2017-08-29T20:53:46.406Z Reads: 110

```
If you find 3d Printing interesting and want to put some time into printing improvements and fiddling with it. Then it can be a fantastic printer. I own one and im very happy with it. Se bellow a test print i made. Quite nice if i should say it myself.


 <img src="/uploads/db1493/original/3X/f/9/f9bee519c5a6998c8c74e5a663fe53389b9fdd0b.jpg" width="375" height="500">
```

---
## \#8 Posted by: Dougieman1001 Posted at: 2017-08-29T20:55:00.785Z Reads: 104

```
Oh yeah that is nice, I'm sure I can tinker with it to make it right. What model/version do you have? Like what option? 
https://goo.gl/f6kpMi
```

---
## \#9 Posted by: wafflejock Posted at: 2017-08-29T21:00:25.474Z Reads: 106

```
Yeah can't really knock it I don't see any major problems.  Things I look for are open source based stuff (ideally using ramps based boards since they are cheap to replace if something goes wrong like $20 to replace the power/motor control shield sits on top a $30 arduino mega), all i3 based kits should use that under the hood basically then look for rigid design and an all metal hot end.

Bigger build area sounds like a good idea and auto levelling will save you time and sanity.   Down the line you can print parts to make printing flexible material easier, I made a custom extruder motor mount that I feed the PTFE tube straight from there to the hot end and just cut a notch in the PTFE tube for the extruder to push on the material so there's no place it can bind up on flexible plastics (ninja flex or some nylons), but that's all kind of stuff you'll want to mess with after all the basics are tuned and working well with PLA and ABS.
```

---
## \#10 Posted by: nikoli280 Posted at: 2017-08-29T21:00:30.803Z Reads: 103

```
I bought the Large Build plate with Auto sensor. But the Auto leveling sensor is shit. So i bought a BLtouch clone and it works flawlessly. I have never since touched the manual leveling.

https://goo.gl/QFpsyS
```

---
## \#11 Posted by: nikoli280 Posted at: 2017-08-29T21:02:42.480Z Reads: 102

```
The Tarantula is Great. But if you want something a bit better. Go after the CR10, or Tevo Tornado. Its build on the same platform, and its just alot more stabil compared to the Tarantula. But it also cost 380-450 dollars. Tarantula cost 200. 

The Tarantula is the clear winner in price-performance i think
```

---
## \#12 Posted by: wafflejock Posted at: 2017-08-29T21:03:02.310Z Reads: 99

```
Good to know on the bed leveling sensor, I upgrade my firmware to support that but need to get the hardware still... this is the ramps board/brains I was referring to:

https://www.newegg.com/Product/Product.aspx?Item=9SIADG45WH9601&ignorebbr=1&nm_mc=KNC-GoogleMKP-PC&cm_mmc=KNC-GoogleMKP-PC-_-pla-_-Gadgets-_-9SIADG45WH9601&gclid=Cj0KCQjwoZTNBRCWARIsAOMZHmEuwtG4HrMaRAj7D56ZdJVRolY5lDuffilamhAL0ADr_ortQXBiag0aAkrAEALw_wcB&gclsrc=aw.ds
```

---
## \#13 Posted by: Dougieman1001 Posted at: 2017-08-29T21:06:19.823Z Reads: 91

```
So really, is it worth buying the model with the levelling feature and just buying that other one instead? Glad you said that though as otherwise I would have had no idea that could happen.
```

---
## \#14 Posted by: Dougieman1001 Posted at: 2017-08-29T21:08:55.867Z Reads: 91

```
Ah right okay. Not going to lie, I had no idea what you were talking about the flex materials etc :joy: Literally went straight over my head, but I guess once I have learned more, I'll be able to come back and read it and understand :joy: 
Think I've made my decision on the printer I'll buy!
```

---
## \#15 Posted by: nikoli280 Posted at: 2017-08-29T21:09:31.548Z Reads: 82

```
Yep exactly buy the large bed if you need it and then buy the auto leveling in another order
```

---
## \#16 Posted by: Dougieman1001 Posted at: 2017-08-29T21:10:49.739Z Reads: 84

```
So it just plugs in to the logic board?
```

---
## \#17 Posted by: wafflejock Posted at: 2017-08-29T21:10:57.234Z Reads: 85

```
Yeah no worries was just rambling anyhow at that point :)  But yeah basically wouldn't worry about the flexible stuff just yet.  Basically there are rigid materials like PLA and ABS (slightly less rigid than PLA) that are the common kinds of filaments everyone starts off with but once you get that working well if you want to print rubbery parts like grippy wheels or custom washers or nylon gears then you sometimes need better parts for gripping and pushing the filament (the extruder is what that motor is called usually).
```

---
## \#18 Posted by: Dougieman1001 Posted at: 2017-08-29T21:14:34.371Z Reads: 82

```
Oh yeah, I knew that PLA and ABS were common but wasn't sure the properties of each, super interesting about all this 3d printing lark :)
```

---
## \#19 Posted by: Mikaelj Posted at: 2017-08-29T21:16:04.616Z Reads: 86

```
I have the prusa i3 mk2s. Its very good. Not perfect, I even found a "fault" in their open source 3D file that makes the x-axis skewed. I see that the creality cr-10 is really popular and cheap, with large build volume. I have used PETG material for enclosures and they seem to hold up nicely :)
```

---
## \#20 Posted by: Dougieman1001 Posted at: 2017-08-29T21:18:42.834Z Reads: 87

```
Yeah Just seen the build volume and its pretty large, just twice the price of the i3 so maybe in the future.. Thats good to know about the PETG too :D
```

---
## \#21 Posted by: gee Posted at: 2017-08-30T16:28:17.630Z Reads: 68

```
anet A8 for budget. tevo is still budget but better frame and all that.
```

---
## \#22 Posted by: gogomrrobot Posted at: 2017-09-12T12:10:42.622Z Reads: 60

```
Yes I am debating between a Creality3D CR - 10 ($389) , Prusa i3 mk2s ($699), and a Lulzbot Taz 6 ($2500).

I want to be able to print Nylon gears and prototypes without too much headache.  Any suggestions on the above 3?
```

---
## \#23 Posted by: rolexbene Posted at: 2017-09-12T12:59:22.172Z Reads: 61

```
I bought a TronXY X1 and the quality is amazing, and only £100. Only thing is I need to upgrade the bed in order to print anything but PLA.
```

---
## \#24 Posted by: mmaner Posted at: 2017-09-12T13:29:48.450Z Reads: 60

```
The Lulzbot Taz 6 is frikkin amazing, it will literally always print correctly with very little throw away.  Its also expensive as hell :), but you get what you pay for.  I'm using a Prusa MK2 clone right now and it pretty good, but not great and takes a significant amount of maintenance.
```

---
## \#25 Posted by: Mikaelj Posted at: 2017-09-12T16:33:16.011Z Reads: 56

```
If I had a choice between these, I would take the Prusa because its in the sweetspot regarding features and price for me. Also it is simple to modify.

If you want to go with the i3, I can recommend swapping out bearings with igus rj4jp-01-08. And use these files for mounting them: https://www.thingiverse.com/thing:2542168
```

---
