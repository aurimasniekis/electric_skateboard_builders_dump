# Tooth Profile for HTD 5M pulley ( NEED HELP)

### Replies: 50 Views: 14396

## \#1 Posted by: mishrasubhransu Posted at: 2016-10-20T19:52:08.740Z Reads: 441

```
I designed a snapin pulley using some pulley I found online but I am not satisfied with the dimensions of the tooth profile. I have gathered information regarding how the tooth profile should be, but I am missing some information. Hope you guys can help me complete it. 

I have the following information:
<img src="/uploads/db1493/original/3X/5/4/5407dd5cb9fe40b583852bb29a8f1daf81006972.png" width="197" height="111">
from [here](http://www.sdp-si.com/D265/HTML/D265T015.html)

<img src="/uploads/db1493/original/3X/b/3/b326d223da9cf06561b4c16dc0539246e0abecf8.png" width="651" height="374">
page 9 of  [gates design manual](https://www.gates.com/~/media/files/gates/industrial/power-transmission/manuals/powergripdrivedesignmanual_17195_2014.pdf?la=en)

So my questions are:
1. What are the exact dimensions of the individual tooth.
2. What is the position of the belt pitch line relative to the bottom of the tooth.

<img src="/uploads/db1493/original/3X/8/9/898134b95bc5e993b8768315f56f3b717d495a05.png" width="521" height="455">
page 9 of  [gates design manual](https://www.gates.com/~/media/files/gates/industrial/power-transmission/manuals/powergripdrivedesignmanual_17195_2014.pdf?la=en)

BTW here's a dummy belt for 56T belt on a 40T and 16T pulley.
<img src="/uploads/db1493/original/3X/c/0/c04448f16af10c3bfe04bc2dff7e0b6d1205c7b7.jpg" width="690" height="361">
```

---
## \#2 Posted by: mishrasubhransu Posted at: 2016-10-20T20:30:22.459Z Reads: 395

```
summoning @JuniorPotato93, @Pantologist,  @zeinstra
```

---
## \#3 Posted by: JuniorPotato93 Posted at: 2016-10-20T20:46:39.874Z Reads: 392

```
How can we be of service.
```

---
## \#4 Posted by: Pantologist Posted at: 2016-10-20T21:13:11.972Z Reads: 388

```
I only started really learning CAD and stuff a few weeks ago lol. I am probably wrong.

1. What are the exact dimensions of the individual tooth.
According to picture from the Gates manual, each tooth has to be 1.93mm high right? Can't you just make and pattern that shape since we will probably use Gates belts?


2. What is the position of the belt pitch line relative to the bottom of the tooth.
Isn't the belt Pitch line the same thing as the height of the belt? So 3.81mm from the bottom of the tooth to the belt pitch line...
 I think I asked more questions than I answered...
```

---
## \#5 Posted by: rpn314 Posted at: 2016-10-20T22:00:27.101Z Reads: 367

```
Not understanding what you're trying to do exactly, but I would try a program called CamBam. It has a tool that will make you the profile for any tooth count you want.
```

---
## \#6 Posted by: mishrasubhransu Posted at: 2016-10-20T22:32:47.901Z Reads: 351

```
Tooth count is not the problem. I want to know how to draw a single tooth for HTD 5M belt.
```

---
## \#7 Posted by: rpn314 Posted at: 2016-10-20T23:04:38.827Z Reads: 339

```
Oh okay. Does this help?

http://www.cshbelt.com/upload/htd-5m.gif
```

---
## \#8 Posted by: Pedrodemio Posted at: 2016-10-21T00:07:21.315Z Reads: 339

```
I've found myself with this same problem

All of the images i found doesn't show the distance from the primitive circumference to the root of the tooth, for my 3d printed pulley i printed several small slices of the pulley until i found one that fits

Maybe using CamBam that @rpn314 suggested you can export the profile to your cad software and get the measurements

EDIT: Thanks a lot @rpn314, worked flawlessly, finally the correct profile

<img src="/uploads/db1493/original/3X/6/c/6c142b39ac04bb50f89314433a969843361eedeb.JPG" width="690" height="331">
```

---
## \#9 Posted by: JuniorPotato93 Posted at: 2016-10-21T00:35:36.145Z Reads: 320

```
The issue with these profiles is that they are showing you what the distance between teeth are on a flat section of the belt.  Once the belt meshes with the tooth it is no longer straight and the center to center distance is actually the arc length of the segment of the pitch diameter between two teeth.  I'm on my phone at the moment but once I get to my home computer later tonight I can upload the profile I use for a singular tooth then pattern to create any sized pulley
```

---
## \#10 Posted by: JuniorPotato93 Posted at: 2016-10-21T00:38:00.842Z Reads: 305

```
This 's almost exactly the same numbers that mine had.  I dimensions mine different to allow for changing the number of teeth and keeping other relationships intact.  @mishrasubhransu
```

---
## \#11 Posted by: Pedrodemio Posted at: 2016-10-21T01:31:43.158Z Reads: 303

```
I agree, this is not how I would draw, I just imported the profile and put the main dimensions so people can use then as base to draw any teeth count
My plan is to get some pulleys made from wire EDM since I can only find aluminum pulleys around here and they are experiencing significantly wear, but no point using EDM with a profile that is not exact
```

---
## \#12 Posted by: JuniorPotato93 Posted at: 2016-10-21T04:52:42.645Z Reads: 292

```
@mishrasubhransu

So you can use the 10 Degrees for 36T or you can do what I do which is create the tooth profile and dimension the width of one tooth to 4.898mm. The two lines coming out from the center of the 25.83 circle and meeting the radius are normal to the radius and I set a geometric constraint there. You have to then set the rest of the geometric constraints to the profile, like the tangent intersects between the .458 radius and the 1.543 and the short segment connecting the .458 radius to the lines coming out of the center is actually a straight line, there's no arc. Its so short it wont matter.  You can then circular pattern the one tooth slice as many times as you want and then select the corners and coincide them and you can create a pulley with any number of teeth. 

<img src="/uploads/db1493/original/3X/4/a/4ada23577e55385d404a5cc52d8f606e0c2a8ff4.jpg" width="510" height="458">
```

---
## \#13 Posted by: Maxid Posted at: 2016-10-21T05:34:23.832Z Reads: 286

```
Just use this:
http://www.thingiverse.com/thing:16627
```

---
## \#14 Posted by: Kaly Posted at: 2016-10-21T13:49:42.189Z Reads: 285

```
@mishrasubhransu
You can always download the profile from the vendor website in any 3D version you want like from  http://shop.sdp-si.com/catalog/product/?id=A%206A25M040NF1510 
 
Just click the download cad banner 
<img src="/uploads/db1493/original/3X/4/2/4215fc3afdabea8a391509ecccd8fb00c6097b2a.PNG" width="281" height="500">
```

---
## \#15 Posted by: JuniorPotato93 Posted at: 2016-10-21T14:43:07.792Z Reads: 271

```
This works great for commonly available sizes bur for example, 42T HTD5 does not exist commonly, you will have a hard time trying to find that online. Its quicker to create that yourself. Also, you can create odd numbered pulleys as well which also do not exist.
```

---
## \#16 Posted by: zeinstra Posted at: 2016-10-22T12:32:36.335Z Reads: 262

```
to calculate the pitch diameter you can just multiply pitch of the belt with the tooth count of the pulley and divide it by pi.
for 40t HTD 5m this wil be (40*5)/3.14... =63.66mm diameter
```

---
## \#17 Posted by: mishrasubhransu Posted at: 2016-10-26T04:03:07.061Z Reads: 261

```
Thanks everyone. The cambam profile didn't seem accurate enough. I got the actual part from the [manufacturer website](http://shop.sdp-si.com/catalog/product/?id=A%206A25M040NF1510) which @Kaly mentioned   and made my profile sketch like @JuniorPotato93 suggested. Made it match the original part as close as possible. Once the profile is done then it's just a matter of using it for different number of teeth.  

Here's that information for future reference. 

<img src="/uploads/db1493/original/3X/9/6/96927c8f6bd3cdcfbe5d703f6f087d13fe6de8a8.png" width="690" height="145">
<img src="/uploads/db1493/original/3X/c/3/c3a045fcf6a669d3f9f7ba1f40c3c701ab3e834e.png" width="653" height="500">

EDIT1:
And this is what the pulleys look(40T, 36T, 16T)
<img src="/uploads/db1493/original/3X/9/3/931e32aa507c02f069f6c68abde7ca48bc594bc9.JPG" width="690" height="363">
<img src="/uploads/db1493/original/3X/f/d/fd234d5aa31edeab784388d74d1803150d0289f9.JPG" width="690" height="366">
<img src="/uploads/db1493/original/3X/a/f/afe5207c13fccb00b76120ef67ab89ee1224fbf6.JPG" width="690" height="365">
```

---
## \#18 Posted by: JuniorPotato93 Posted at: 2016-10-26T04:21:36.094Z Reads: 239

```
looks like you hit the nail on the head with that. Hope it prints out well!
```

---
## \#19 Posted by: wmj259 Posted at: 2017-06-18T05:32:51.379Z Reads: 216

```
@mishrasubhransu
How do you calculate the OD and U values?
You calculate the U value from subtracting PD and OD, but then you use that U value to calculate OD?
```

---
## \#20 Posted by: theRoy98 Posted at: 2018-05-19T03:07:09.713Z Reads: 174

```
@JuniorPotato93 Hi I don't really understand your instructions about creating a pulley, I'm trying to make a really bit 188 T pulley and I printed one but it just doesn't seem to fit. Maybe I am misunderstading your instructions?.
I don't get why the 25.83mm is higher than the 27.464 in your diagram
```

---
## \#21 Posted by: jens_c Posted at: 2018-07-01T17:01:08.280Z Reads: 153

```
here you have the full explanation http://www.gatesmectrol.com/mectrol/downloads/download_common.cfm?file=Belt_Theory06sm.pdf&folder=brochure
```

---
## \#22 Posted by: TVO Posted at: 2018-09-17T09:15:01.664Z Reads: 129

```
Looks really good. I replicated your equations in SW, but I am missing the equations for TPR1, TPR2 and TPD1.
Are they constant regardless of number of teeth? And what about different pitch?
I would be very happy if your share this information.
```

---
## \#23 Posted by: mishrasubhransu Posted at: 2018-09-17T18:17:34.036Z Reads: 122

```
Thats a good question. Let me check.
```

---
## \#24 Posted by: mishrasubhransu Posted at: 2018-09-17T22:34:31.852Z Reads: 124

```
I checked. They are fixed values in my equation. Maybe that's what I got from the cad from the websites.
```

---
## \#25 Posted by: TVO Posted at: 2018-09-18T05:38:19.584Z Reads: 122

```
Thank you very much for your effort. 

It is a little odd, because your values are just a little different from the ones downloaded from sdp-si.com.

The reason I ask is that I downloaded and printed some wheels from a German website and they performed terribly, but they had quite different geometry from what I later purchased. So now I want to know, what is "correct" if anything is.
```

---
## \#26 Posted by: mishrasubhransu Posted at: 2018-09-18T16:20:41.006Z Reads: 124

```
I don't exactly remember which website I followed, but the designs have served me well. Haven't had a belt broken in 2 years, riding roughly 2 miles daily. 
This is a new pulley that I printed and this is how the belt fits.

![MVIMG_20180918_121535|666x500](upload://9QQbbQrvBOTnuQZol80PunpEJEK.jpeg)
```

---
## \#27 Posted by: TVO Posted at: 2018-09-19T04:55:20.089Z Reads: 121

```
Great, thank you. I will go on with your values :sunglasses:
```

---
## \#28 Posted by: Nordle Posted at: 2018-09-19T05:58:32.933Z Reads: 116

```
printing gears is also a bit trial and error imo, nozzle diameter and slice settings can change the gear tooth profile so it’s not exactly the same like in your cad software.
```

---
## \#29 Posted by: Pedrodemio Posted at: 2018-10-10T17:00:51.428Z Reads: 108

```
Also keep in mind that if you got the diameters right but the teeth fitting is tight, just run it anyway, a few minutes ridding the belt will wear the pulley and make a perfect fit
```

---
## \#30 Posted by: billy_joule Posted at: 2019-03-24T05:01:47.891Z Reads: 78

```
Hey, I've tried to replicate your sketch and have double checked the dimensions but it's still not evaluating as your's has.
![Pulley%20Sketch|651x500](upload://8ZwFsrUTsQcoOuu530sIAUW88kc.jpeg) 

What is the tangent relation to the outer circle? (tangent symbol below TPR2 dim)
I would have thought the R0.45380 would be tangent to the "OD" (24.32) circle but it becomes over-constrained if I do that.

Any hints?

Thanks
```

---
## \#31 Posted by: billy_joule Posted at: 2019-03-24T05:13:04.514Z Reads: 75

```
Perhaps there is a  short straight line (0.29 mm for 16T) hidden back there? 

![Pulley%20Sketch%202|690x484](upload://7kgoL4f6umaaAOtJCbUFY7E6jlB.jpeg)
```

---
## \#32 Posted by: TowerCrisis Posted at: 2019-03-24T05:33:10.737Z Reads: 72

```
You are much better off importing a 3d model from sdp-si.com and using that as a basis for your pulley if this is a one-off kind of part.
```

---
## \#33 Posted by: mishrasubhransu Posted at: 2019-03-24T05:39:21.740Z Reads: 70

```
Seem like you are using solidworks. PM me with your email. I'll send you the part.
```

---
## \#34 Posted by: billy_joule Posted at: 2019-03-24T05:57:23.882Z Reads: 68

```
Thanks! Unfortunately I can't for the life of me find where to send a PM, perhaps I don't have that privilege yet. but you could send it here amailboxforrandomthings@gmail.com thanks again.
```

---
## \#35 Posted by: billy_joule Posted at: 2019-03-24T05:59:25.820Z Reads: 66

```
I would, but I need a pulley with hundreds of teeth for an e-bike and spd-si only go up to 72.
```

---
## \#36 Posted by: mishrasubhransu Posted at: 2019-03-24T06:21:00.359Z Reads: 69

```
I just send it to you.
```

---
## \#37 Posted by: TowerCrisis Posted at: 2019-03-24T06:27:39.965Z Reads: 71

```
Oof, that's a dousey.

Keep in mind, they typically don't go to very high tooth counts because any small error in the tooth profile will compound over each tooth. For hundreds of teeth you're going to need a very very precise profile, and likely many tests to tune it.
```

---
## \#38 Posted by: mishrasubhransu Posted at: 2019-03-24T07:24:46.305Z Reads: 70

```
my profile is almost, if not completely, identical to sdp-si.com profile. I would be more worried about the 3D printer limits/tuning. 
![image|666x500](upload://w1LeDAUJhP2FVwnb34cm4tZBBa0.jpeg)
```

---
## \#39 Posted by: billy_joule Posted at: 2019-03-24T20:54:01.416Z Reads: 68

```
[quote="TowerCrisis, post:37, topic:11565"]
Keep in mind, they typically don’t go to very high tooth counts because any small error in the tooth profile will compound over each tooth. For hundreds of teeth you’re going to need a very very precise profile, and likely many tests to tune it.
[/quote]

Yeah, Ill be printing in 4 to 8 (TBC) sections & can add shims between the sections to adjust out any pitch errors that may accumulate. OF course, shims will make it out of round but the effect will be very small. 

Although this guy prints a 180 tooth pulley with a poor sketch and seems to do OK:

https://youtu.be/cQhZSc0dhjc?t=355

(Of course, perhaps he was lucky and the error in his sketch could have been corrected by the error in his printing )
```

---
## \#40 Posted by: Pedrodemio Posted at: 2019-03-24T20:55:46.879Z Reads: 68

```
In my experience you will have to tune the profile for your 3D printer, print just a thin ring with no infill and adjust as needed
```

---
## \#41 Posted by: mishrasubhransu Posted at: 2019-03-24T21:52:50.466Z Reads: 64

```
[quote="Pedrodemio, post:40, topic:11565"]
profile for your 3D printer, print just a thin ring with no infill and adjust as needed
[/quote]

Yep. Exactly. Your printer has to be calibrated.  Make sure when you are printing a hollow square of wall thickness 1mm, you are getting 1mm. Also the dimension of a solid cube should be very close to true dimension in all three directions and walls should be perpendicular to each other.

But like pedro said before, the belt will take care of the exact fit in a few minutes.
```

---
## \#42 Posted by: Pedrodemio Posted at: 2019-03-25T04:06:53.651Z Reads: 61

```
[quote="mishrasubhransu, post:41, topic:11565"]
But like pedro said before, the belt will take care of the exact fit in a few minutes.
[/quote]

That’s the blessing and the curse of 3D printed pulleys, in the first 10’s of kilometers they will wear down and make the fit perfectly, in that phase they are astonishing quiet, but after that they wear past the perfect point and the noise increases a lot, my board still really quiet when breaking since that face of the tooth doesn’t take load all the time

But they last and are cheap for rapid prototyping, so that’s ok for me, I’m almost at a 1000 km on this set
```

---
## \#43 Posted by: mishrasubhransu Posted at: 2019-03-25T04:09:34.236Z Reads: 66

```
Nice! I am beyond 400km on FDM printed pulley and surprised that they haven't shown signs of significant wear. In my previous board(back when I didn't trust FDM printing), I got the pulleys printed from shapeways using Nylon SLS and have lasted me more than 2000 or so kms.
```

---
## \#44 Posted by: danielz Posted at: 2019-03-25T04:29:37.039Z Reads: 67

```
https://i.imgur.com/Rmmi53H.png

https://www.thingiverse.com/thing:16627

follow the instructions for using openscad as described in the above thinverse link to generate any pulley profile, size with rims you wish, then save as stl and import into your cad software.

With my cr-10, 80 tooth HTD5 ones have printed flawless every time, 100% infill, outershell at a very low speed like 10mm/s the rest at regular speed. 

However first calibrate your extruder by measuring how much filament it actually extrudes vs requested. Then print a calibration cube.
```

---
## \#45 Posted by: Pedrodemio Posted at: 2019-03-25T11:48:34.799Z Reads: 55

```
Are you using ABS?
```

---
## \#46 Posted by: Toby-Aus Posted at: 2019-04-11T13:55:28.076Z Reads: 50

```
thought id leave this here.
5m 72 tooth and 15 tooth
https://www.dropbox.com/s/vlx74nmy020x1bu/72%20teeth.dxf?dl=0
https://www.dropbox.com/s/ue3xw6y017wqp20/15%20teeth.dxf?dl=0
```

---
## \#47 Posted by: Z408 Posted at: 2019-07-04T18:45:00.091Z Reads: 41

```
Just downloaded your dxf into Solidworks.  I think the scale might be off.  Can you double check this for me?  It is showing radius of 1448mm.

thank you.
```

---
## \#48 Posted by: Toby-Aus Posted at: 2019-07-05T05:08:32.085Z Reads: 41

```
The 72 tooth diameter measures 113.45mm the 5 holes around the inside are 4.1mm just scale your drawing off one of these holes
```

---
## \#49 Posted by: Toby-Aus Posted at: 2019-07-05T07:00:05.131Z Reads: 38

```
Your scale might be out or ur using wrong units
```

---
## \#50 Posted by: Z408 Posted at: 2019-07-06T03:24:21.212Z Reads: 35

```
Thanks, I will give that a try.
```

---
