# 3D printable #25 sprockets and HTD-5M Pullies (wheel/driven and motor/driver!): An open-source project

### Replies: 16 Views: 2992

## \#1 Posted by: Qwiksand Posted at: 2016-09-20T17:36:51.520Z Reads: 291

```
All project files can be found here: https://cad.onshape.com/documents/7c265efa9d5612eb994e2e4a/w/06e95e783c6efd3a7cc0f7ef/e/e13c9a3a0cc5a1ef48cadb6a

In order to make printed motor driver sprockets/pullies work, I've purchased a 8mm to 1/2" hex adapter and pressed/locktighted it onto the motor shafts. This is the one I've been using:
<img src="/uploads/db1493/original/3X/3/2/3231f3b1336497ad63cb1419475042451ef3936d.jpg" width="484" height="448">
It's from AndyMark and can be found here: http://www.andymark.com/8mm-Keyed-Bore-1-2-Inch-Hex-Adapter-p/am-0588.htm

VexPro makes a cheaper version, but it has been on backorder for a couple of months: http://www.vexrobotics.com/vexpro/hardware/217-3255.html

My hub adapter was inspired by brentyi's on thingiverse (http://www.thingiverse.com/thing:545345). It is a complete redraw using this grabcad file designed by andrew: https://grabcad.com/library/flywheel-skateboard-wheel-clones-1

<img src="/uploads/db1493/original/3X/e/b/ebc9771e58f17d553d6c3f3c730d2abf1817a066.jpg" width="690" height="414"><img src="/uploads/db1493/original/3X/e/7/e7cece7e8098da107ed81eac088f7470169d6615.jpg" width="690" height="414"><img src="/uploads/db1493/original/3X/4/8/483694616e4dac0bc9de1329536797a1383945e4.jpg" width="690" height="414">

I've replaced the bolt/nut attachment system with a simpler Spax screw system and it holds very well.

<img src="/uploads/db1493/original/3X/2/4/244fc49a061e93868d4d3230b6fc1ed717862ec9.JPG" width="690" height="458"><img src="/uploads/db1493/original/3X/0/2/0221111553a5bf567fb2763c3edafd5014fad7c4.JPG" width="690" height="458"><img src="/uploads/db1493/original/3X/b/c/bcb879d8f789768ddf684c33f420af29b370c92b.JPG" width="690" height="458">

This is the HTD-5M version:
<img src="/uploads/db1493/original/3X/4/c/4c63a4d8efcd76ededa6a7702ef43b15112ee1cf.JPG" width="690" height="458"><img src="/uploads/db1493/original/3X/6/4/647ab89447b1e56c03a663e1e9053386da7b2cbc.JPG" width="690" height="458">

The above pullies are printed in trimmer line nylon and don't seem to wear at all.

This is the #25 sprocket version:
<img src="/uploads/db1493/original/3X/b/c/bc710d5671feac0d1c73f2859f6673b3e55fcff8.JPG" width="690" height="458"><img src="/uploads/db1493/original/3X/6/3/63410d33c5166aef78f9a33bf947b6e1461688ab.JPG" width="690" height="458"><img src="/uploads/db1493/original/3X/1/d/1d58b65dc5ebfbd5324f3c27c6a2cfea62f0a1a0.JPG" width="690" height="458">

I've been pleasantly surprised by the durability of these printed sprockets. The wheel sprocket in the above pic is trimmer line nylon and has over 60 miles, while the motor sprocket is eSun PETG and has approx 30 miles. Obviously, these sprockets will not outlast the chain, but they seem to be holding up and should last at least to an average wheel rotation interval.
```

---
## \#2 Posted by: Qwiksand Posted at: 2016-09-20T20:57:19.578Z Reads: 222

```
Also, I'm looking for some open-source cad models of smaller (12t to 33t) HTD-5M pullies for this project. Please let me know if you have any or know where I might find some. :sunglasses:
```

---
## \#3 Posted by: theviith Posted at: 2016-09-20T22:47:27.012Z Reads: 211

```
what settings did you use for the esun PETG? I haven't been getting good results with the esun PETG and I think it's because of my print settings.
```

---
## \#4 Posted by: Qwiksand Posted at: 2016-09-20T23:30:51.103Z Reads: 201

```
I'll verify these when I'm back at the home computer, but off the top of my head:

-E3D V6 hotend, 0.4mm hardened steel nozzle (prepared for carbon fiber filled filaments) set to 245c (I used 240c with standard brass nozzles)

-80c bed temp, printed on clean glass (mirror tile actually)

-go slow, I think my fastest speeds are only at 45mm/s

-I think my retraction setting is 3 or 4mm using a direct drive (I've used upwards of 6 or 7mm on a bowden set-up and had just a tiny bit of fine stringing).

-Dry it! Everyone says PETG doesn't absorb water, but that's incorrect- it doesn't affect surface finish as much as nylon, but strength is severely impacted- E3D did some testing on this, you can find it on their website somewhere.
```

---
## \#5 Posted by: Mobutusan Posted at: 2016-09-21T04:21:24.492Z Reads: 179

```
Really nice looking pulleys. :thumbsup: Man I wish I had a 3d printer.
```

---
## \#6 Posted by: Qwiksand Posted at: 2016-10-06T16:45:10.106Z Reads: 166

```
<img src="/uploads/db1493/original/3X/6/4/645610739a3bd33ef67f03861303c55d0b52e854.JPG" width="690" height="458">

This PETG sprocket died due to impact trauma- my 5 year old likes to "ghost ride" my board full speed off of curbs and what not (he has fun, I look at it as stress-testing :sunglasses: )

This sprocket had approx 40 miles on it and no significant wear to the teeth. I'm very surprised by the durability of these things, I would have never believed it if someone told me a printed DRIVER sprocket would last more than a couple miles.

I'm running a new PETG driver sprocket (same old nylon driven is working and will probably work for many, many more miles) to see if I can get one to wear out from use rather than abuse. I'll keep this thread updated. I've got some CF reinforced nylon and PETG to try out at some point as well.
```

---
## \#7 Posted by: DeathCookies Posted at: 2016-10-25T12:12:15.604Z Reads: 148

```
[quote="Qwiksand, post:6, topic:9897"]
his sprocket had approx 40 miles on it and no significant wear to the teeth.
[/quote]

Well, for me the sprockets are bend counter clockwise. I could see it without zooming ;) They are stressed but it was a question of time when it will break or the chain slip off.
```

---
## \#8 Posted by: Qwiksand Posted at: 2016-11-18T00:16:25.642Z Reads: 134

```
To be fair, the sprocket pictured above hit a curb so it's likely you're seeing the impact damage.

I recently broke another PETG driver sprocket running 16:32 gearing and this one appears to have broken from torque loading- chain was looser than optimal and appears to have fractured the sprocket from shock-loading as I was going up a hill running over twigs, leaves and acorns. 

In my experience, PETG as a driver sprocket has a pretty short life span (best I've gotten is the 40 miles documented above). I've been running nylon (just cheap string trimmer nylon) sprockets for a while now and I've yet to have a failure. In fact, I've got a 32t wheel sprocket printed in nylon that has over 100 miles on it and is just beginning to show some teeth wear/hooking. The driver sprocket will certainly be the limiting factor in a 3d printed system. 

As to noise, nylon sprockets with chain is just a bit noisier than belts.
```

---
## \#9 Posted by: Qwiksand Posted at: 2016-11-18T00:24:16.469Z Reads: 125

```
Also, I've fixed my HTD 5M sketch and it is now fully parametric. Just go to the part studio tab labeled "30t HTD5M Wheel Mount" for the wheel pulley or "18t HTD5M 13.3mm Hex Hole" and change the Variable #Teeth and Variable #Width to whatever you need. 

Here's the On Shape file again: https://cad.onshape.com/documents/7c265efa9d5612eb994e2e4a/w/06e95e783c6efd3a7cc0f7ef/e/e13c9a3a0cc5a1ef48cadb6a17
```

---
## \#10 Posted by: darkkevind Posted at: 2016-11-18T00:46:17.631Z Reads: 122

```
@Qwiksand are you selling these sprockets?
```

---
## \#11 Posted by: Qwiksand Posted at: 2016-11-18T01:09:47.508Z Reads: 121

```
Not at this time, still too experimental- this is really only a viable drive train system if you've got a printer or cheap access to one.
```

---
## \#12 Posted by: darkkevind Posted at: 2016-11-18T01:11:30.906Z Reads: 121

```
Got neither unfortunately :disappointed:
```

---
## \#13 Posted by: krazor Posted at: 2019-07-10T13:05:32.331Z Reads: 39

```
how have you found these 3D printed sprockets holding up so far? im tempted to print some for a 12S build to test while i source some metal ones.
```

---
## \#14 Posted by: Brad99 Posted at: 2019-07-19T22:42:13.250Z Reads: 31

```
![drive|666x500](upload://7Y9o9pT6mjfj0BhLvNyrzD9ssvt.jpeg) 

Pla on the right, abs on the left (ended up breaking real quick). Going to try nylon soon. (10mm D-shaft, 16t I think)
```

---
## \#15 Posted by: Qwiksand Posted at: 2019-07-22T16:29:59.513Z Reads: 26

```
#25 printed in nylon for the driven/wheel sprocket hold up incredibly well and are much quieter than aluminum (PETG also works, but they fail unpredictably). I've only had moderate success (50 miles max) with printed driver/motor #25 sprockets in nylon, but they are super quiet compared to steel.

As to the durability of printed HTD-5M pullies, I've had the greatest success with nylon for both driver and driven.
```

---
## \#16 Posted by: krazor Posted at: 2019-07-23T08:32:05.046Z Reads: 21

```
ah nice, my sprockets actualyl came in sooner than i had thought. delivery is expected for tomorrow but i would love to continue trying to 3D print the sprockets haha. i have a few prototypes printed on ym desk here in PETG
```

---
