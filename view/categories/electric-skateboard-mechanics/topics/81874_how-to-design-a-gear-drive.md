# How to design a gear drive

### Replies: 39 Views: 960

## \#1 Posted by: Gustdd Posted at: 2019-01-24T00:36:08.776Z Reads: 276

```
Hi everyone,
I'm finishing my first build but I need some help with the geardrive. I'm not a mechanical engineer so this is getting quite challenging.

I'm doing a 12s4p 190kv motor build and retrofitting an old [mountainboard](https://images-na.ssl-images-amazon.com/images/I/41HkAW65X8L._SX355_.jpg).

My idea was to laser cut the gears and motor mounts from a sheet of 8mm aluminium.
And then 3d print an enclosure too keep everything away from road debris and the lubricant inside.

My problem is how to design the gears. Is there any tool I can use? I've design the motor mounts in fusion 360, but I don't know where to start with gears.

I searched online and found https://geargenerator.com/#200,200,100,6,1,0,902.1000000000228,2,1,11,2.75,4,27,-90,0,0,48,12,4,27,-60,0,0,2,292 but if I try to import into fusion the measurement aren't correct, the gears end up bigger than stated in the website. 

(I got the 11:48 from the esk8 calculator, I would like to increase 48 to a bigger number but the size of the gear would be too big?? maximum is about 120mm~130mm with current wheels)
```

---
## \#2 Posted by: Vanarian Posted at: 2019-01-24T00:43:03.147Z Reads: 261

```
You need a CAM software to get correct gear mesh, there are few options I think but I forget names :thinking:
```

---
## \#3 Posted by: wafflejock Posted at: 2019-01-24T00:48:49.078Z Reads: 262

```
Looks like the suggested way to do it in fusion by most people is to start off with an existing model from mcmaster carr or elsewhere and then tweak it from there https://forums.autodesk.com/t5/fusion-360-design-validate/designing-spur-gears-in-fusion-360/td-p/4336688 . for Pulleys I found a OpenSCAD file that has parameters you can adjust to generate new models that is useful for trying different number of teeth... found some googling for openscad gears too https://www.thingiverse.com/akaziuna/collections/openscad-gear-scripts openscad is free you can adjust parameters in model definitions then hit F5 to regenerate the model then F6 to generate an STL and export.
```

---
## \#4 Posted by: moon Posted at: 2019-01-24T00:49:29.202Z Reads: 243

```
Aluminum isn't the best material choice for gears
```

---
## \#5 Posted by: Gustdd Posted at: 2019-01-24T08:23:57.828Z Reads: 211

```
Why? I believe bikes use aluminium sprockets sometimes. I can use other materials...
```

---
## \#6 Posted by: Vanarian Posted at: 2019-01-24T08:36:07.441Z Reads: 204

```
You want a hard material with low friction coeff and low deformation + high impact resistance IMHO

I think steel based gears are better?
```

---
## \#7 Posted by: Gustdd Posted at: 2019-01-24T09:04:26.369Z Reads: 197

```
Can be done, it'll a bit more expensive but manageable.
```

---
## \#8 Posted by: Gustdd Posted at: 2019-01-24T09:05:40.091Z Reads: 194

```
The spur gear generator works like a charm, how can it be I never found it before.

I just need to understand the concepts and I'll be good to go. Some studying tonight.
If some gear wizard comes by and is willing to review my design please say so, I'll be very happy to show. (I reckon I'll post anyway just in case)
```

---
## \#9 Posted by: pat.speed Posted at: 2019-01-24T09:38:08.283Z Reads: 178

```
You might be best with a combo of steel and plastic gears. A metal pinion gear and POM spur gear is what’s used most commonly in other gear drives
```

---
## \#10 Posted by: Gustdd Posted at: 2019-01-24T09:39:21.219Z Reads: 169

```
Do you know why? That increases the cost a bit sice I need the shop to setup the machine for two different materials.
```

---
## \#11 Posted by: TowerCrisis Posted at: 2019-01-24T10:04:15.143Z Reads: 172

```
It usually cuts down significantly on noise, plastic + metal gears are (iirc) one of the quietest combinations.

You also have significantly less wear on your wheel gear since it is much larger. Because of this it doesn't require as hard of a material, and is cheaper when produced at a larger scale.

Also, I'm more than willing to look over your design. I haven't made any gear driven esk8's, but I am quite experienced in gearbox design.
```

---
## \#12 Posted by: Schulerbible Posted at: 2019-01-24T10:40:56.826Z Reads: 169

```
Get Fusion 360 and download spur gear examples from Grabcad or Maedler catalog which you can use as a starting point. Isn't as complicated as it seems. Just need to get the tooth profile right, but there are a ton of examples which you can simply google. As pointed out earlier, get an off-the-shelf steel (stainless steel) motor gear and use POM as material for the wheel gear.
```

---
## \#13 Posted by: pat.speed Posted at: 2019-01-24T10:46:13.367Z Reads: 173

```
[quote="TowerCrisis, post:11, topic:81874"]
You also have significantly less wear on your wheel gear since it is much larger
[/quote]

This is due to have “x” many less rotations on the large gear due to the small gear rotating 3-5 times per one rotation of the larger gear
```

---
## \#14 Posted by: Gustdd Posted at: 2019-01-26T01:30:19.328Z Reads: 153

```
So this is what I created using fusion script.

I'm a bit doubtful about the shape of the teeth in the wheel side, they seem kinda pointy.

![gears%20v2|690x395](upload://sHu9JzzbLC0TiNlIq4pcedsX7cn.jpeg) 

step file here: https://drive.google.com/open?id=1b9MCSgAbDDHtzydaEZEWpb9NcB7fSTJO
```

---
## \#15 Posted by: Gustdd Posted at: 2019-01-31T16:49:25.705Z Reads: 146

```
I searched my area and couldn't find a POM machining shop.

Anyone knows one in Portugal?
Or maybe a Chinese website like they have for pcb's.

I could also buy the POM as a block and look for a milling place locally.
Any suggestions for POM sourcing?
```

---
## \#16 Posted by: CamBo Posted at: 2019-02-01T03:25:34.026Z Reads: 140

```
Search for POM, Acetal Resin and Delrin 

I buy mine here

https://www.eplastics.com/shapes/acetal-delrin/rod

Not in Portugal, but the site will give you additional product names to search.
```

---
## \#17 Posted by: moon Posted at: 2019-02-01T06:48:02.413Z Reads: 133

```
What tooth width did you go for in the end
```

---
## \#18 Posted by: Gustdd Posted at: 2019-02-01T08:44:23.634Z Reads: 121

```
8mm, but I'm yet to order the parts so it could be changed based on feedback.
```

---
## \#19 Posted by: Gustdd Posted at: 2019-02-01T14:57:55.333Z Reads: 113

```
Do you guys reckon a 3d printed PLA gear can hold for a testing?
Validating the design before milling the POM is useful.
```

---
## \#20 Posted by: FredrikHems Posted at: 2019-02-01T15:16:24.003Z Reads: 110

```
Depends on what you mean by testing. For test fit its fine, but you are not going to be able to testride it. Especially not with only 8mm width. I had 15mm width and shredded through gears within a couple hundred meters.
```

---
## \#21 Posted by: Gustdd Posted at: 2019-02-01T15:19:04.041Z Reads: 104

```
Damn, I was hopping to ride for a bit, just to guarantee that the teeth are properly designed.

I guess I'll trust fusion gear generator.
```

---
## \#22 Posted by: Pedrodemio Posted at: 2019-02-01T15:22:17.883Z Reads: 105

```
Good luck on this project

If you want to it right forget laser cutting, for the thickness a gear is you can’t get perfectly parallel faces and also the surface finish is not ideal

Your best bet is to go to some company that make gears or buy them in AliExpress, there is a lot of vendors for a reasonable price 

And take a look here to familiarize with some terms and manufacturing techniques 

https://en.m.wikipedia.org/wiki/Gear_manufacturing
```

---
## \#23 Posted by: FredrikHems Posted at: 2019-02-01T15:23:12.727Z Reads: 96

```
Did you use the built-in gear generator by Fusion? If so I think you should be good, I have used it several times myself. However 8mm may be a bit thin, most use 15mm.
```

---
## \#24 Posted by: Gustdd Posted at: 2019-02-01T15:28:36.780Z Reads: 96

```
My initial idea was to cut both gear at once and then invert one of them so the laser skew would match and I would get something like a helical gear with shallow angle.
Unfortunately I can't use POM if I do this.

I'll take a look in AliExpress again, couldn't find anything that would fit before.
```

---
## \#25 Posted by: Gustdd Posted at: 2019-02-01T15:29:14.671Z Reads: 99

```
Not sure I can cut 15mm.
```

---
## \#26 Posted by: Pedrodemio Posted at: 2019-02-01T15:31:35.413Z Reads: 99

```
If our use was low torque it would support it, but it’s not, I did the calculations a while ago and the stress the material is subject at peak torque of a high power builds is significantly even for high grade steel, if you have miss alignments it will only increase

I will see if I find the vendor I bought

EDIT: Got from them, for the price is ok, nothing precision ground or anything like that, but is good and way better than anything you will get on the laser

https://pt.aliexpress.com/store/318640?spm=a2g0s.9042311.0.0.2742b90aQyVH1U 

A good way to improve the fit on these low cost gears is instead of grease, put valve grinding compound and let it runs for a few minutes, them dissemble and clean everything really good, preferable to put some old or low quality bearings when doing this and throw them away after
```

---
## \#27 Posted by: Gustdd Posted at: 2019-02-01T16:01:52.623Z Reads: 93

```
You got standard processing? They seem to have a fine processing.

(I should've asked this before chinese new year :smiley: )

Do you think I can drill a new bore hole? They sell only 6M for the small gear.
Also, you are using metal against metal? People above recommended POM.
```

---
## \#28 Posted by: Pedrodemio Posted at: 2019-02-01T17:36:29.866Z Reads: 91

```
They have booth I think, but it will be while until they answer

If you have a lathe yes, with a drill (or even drill press) it's impossible to get it centered enough

I think I've found nylon gears there, but for steel on steel it would need oil bath, grease is not enough, but them the design gets way more complicated, if you managed to find POM gear for a good price go for it, only went steel/steel because custom made gear are too expensive
```

---
## \#29 Posted by: FredrikHems Posted at: 2019-02-01T19:12:31.077Z Reads: 89

```
I remember seeing a gear design of you with an oil bath. Did you ever work more on this? I am having a hard time working out how to make the drive oilproof.
```

---
## \#30 Posted by: Pedrodemio Posted at: 2019-02-01T19:29:08.707Z Reads: 89

```
The design is done, but since I switched to larger motors I need to see if it still fit, probably no without the motor getting to close to the ground

For the oil you would need to have a gasket all around the case and also axial retainers on the axle that exit to the wheel, but the surface finish of that have to follow a set of parameters for surface roughness or it will leak

Also depending on your motor you would need another seal on the motor shaft and somehow figure a way to make it adjustable
```

---
## \#31 Posted by: TowerCrisis Posted at: 2019-02-01T22:24:27.095Z Reads: 82

```
Regarding laser cutting, you could easily just do many layers (8x 1mm sheets) and bolt them together through the side. Only for the wheel side though, motor would (I assume) be steel or aluminum.
```

---
## \#32 Posted by: FredrikHems Posted at: 2019-02-01T22:39:12.193Z Reads: 80

```
To me this doesnt sound like a good idea tbh. Laser gutters usually have a precision of ~0.3mm, which is too much error for a gear.  

@Pedrodemio My initial plan was to use sealed ball bearings for the axial sealings, however i dont know if i should trust them. They’re not waterproof at least.
```

---
## \#33 Posted by: Pedrodemio Posted at: 2019-02-01T23:02:52.516Z Reads: 78

```
I can work with grease, with oil it will leak even when using 2RS bearings, @nuttyjeff did this with his gear drive, but you must guarantee  that the cover is concentric with the rest of the moving parts, a seal has a higher tolerance to misalignment
```

---
## \#34 Posted by: Gustdd Posted at: 2019-02-14T08:04:19.243Z Reads: 70

```
Quote from china is $72 per gear, away too much right?
Waiting on quote from local shop.

Shame I need a mill to make the gears...
```

---
## \#35 Posted by: MoeStooge Posted at: 2019-02-14T19:47:10.459Z Reads: 60

```
Hardened steel on hardened steel 
 These spurs are ready available and you will only buy it once.  Have the center machined out and print your adapter to bolt it up.  Pinions are 8mm in all sizes. Mod 1.5  
I use a shot of mx chain lube before I ride and run em open air. 
https://rover.ebay.com/rover/0/0/0?mpre=https%3A%2F%2Fwww.ebay.com%2Fulk%2Fitm%2F264175037531
```

---
## \#36 Posted by: mmaner Posted at: 2019-02-14T19:49:49.101Z Reads: 62

```
Do you know what the modulus is on these?
```

---
## \#37 Posted by: Indiangummy Posted at: 2019-02-14T19:50:40.957Z Reads: 63

```
1.5 Mod right? Or is modulus something different?
```

---
## \#38 Posted by: mmaner Posted at: 2019-02-14T19:51:22.630Z Reads: 64

```
Nope, thats what I was asking.  Thanks
```

---
## \#39 Posted by: DragonSwagin Posted at: 2019-02-17T18:04:23.515Z Reads: 55

```
Currently looking at making my own gears as well. I have access to a waterjet, so I'm tempted to grab a 1/4" steel plate and make a few sets of motor gears/mounts in one fell swoop; then just print a wheel gear out of POM or nylon. Thoughts?
```

---
