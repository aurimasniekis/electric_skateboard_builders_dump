# First-Time Build: 10S, 190kv, VESC, SuperGlider!

### Replies: 16 Views: 1640

## \#1 Posted by: jammin Posted at: 2017-07-11T16:50:12.554Z Reads: 254

```
Hi everyone! I've been a long-time lurker of this website, and now I'm finally saving up the money to do this build! Before I pull the trigger on this, I _just_ want to make sure that all of my parts will work together... I've been riding longboards for some time now, so I'm hoping to hit a max of ~20mph and at least 10 miles range.

I live a mostly flat and smooth area, so I shouldn't need a lot of torque (hence the single motor).

<b>Drivetrain</b>
Single Bolt On Motor Mount w/ Drive Wheel:
 [DIYElectricSkateboard](diy-electric-skateboard-kits-parts/single-bolt-on-motor-mount-with-drive-wheel-kit/). I plan to buy a 255 x 12mm belt with 36T x 16T pulleys.

<b>Motor & Hardware</b>
Turnigy SK3 6364 190kv
VESC
5000mAh 5S 20C Lipo (x2)
GT2B Controller

<b>Longboard</b>
Earthwing Superglider (I already own this)
Caliber II Trucks
80a Kegel

<b>Other Random Things</b>
IMAX B6 Charger
a lot of XT60 and XT90 plugs
Charging harnesses n stuff

The goal is to have the batteries discharging in series and charging in parallel. I plan to have a cable (along with an anti-spark xt90 plug to connect the whole thing together.

Image gallery here:
http://imgur.com/a/vHyjV
```

---
## \#2 Posted by: willpark16 Posted at: 2017-07-11T19:38:41.995Z Reads: 225

```
Everything is fine except your motor at 10s I would recommend 190kv, unless u want to run the 245kv motor then you will neeed a new battery. Or you can limit Erpm but I don't recommend tha.t. If you go 190kv I can hook u up with the drive train at a good price
```

---
## \#3 Posted by: jammin Posted at: 2017-07-12T01:41:34.115Z Reads: 202

```
Could you explain why 190kv is recommended? What would be the new battery if I went with 245kv?
```

---
## \#4 Posted by: willpark16 Posted at: 2017-07-12T01:49:22.829Z Reads: 196

```
High Voltage and high rpm don't go with 
vesc so it would be 8s if u went 245kv
```

---
## \#5 Posted by: pat.speed Posted at: 2017-07-12T01:50:40.963Z Reads: 195

```
What he means is the Vesc  has a limit of 60k erpm. If you use a 10s setup and 245kv motor you will be exceeding this and will most likely get a dvr error. But if you use a lower kv motor you won't exceed the limit and will be fine. If you have already purchased the motor you could just limit the erpm in the Vesc settings
```

---
## \#6 Posted by: jammin Posted at: 2017-07-12T18:45:48.829Z Reads: 165

```
Thank you!! I'll plan to go 10S and use a 192kv motor. I just realized that I actually own a set of Kegels, so I'll be changing the setup around a little bit. I'll post again with the updated setup once I've bought everything
```

---
## \#7 Posted by: jrpwit Posted at: 2017-07-12T19:31:20.493Z Reads: 155

```
Its fine. Just limit the erpm to 60000 in the vesc settings. BTW the setting is in the first page you see when you open the program. Impossible to miss.

I say this cause I run 245kv on 10s.
```

---
## \#8 Posted by: jammin Posted at: 2017-07-12T21:07:25.996Z Reads: 147

```
Good to know. Speaking of motors, I've been looking at what's in stock at HobbyKing and they only have a SK3 - 6364-190kv motor in stock.

What's the difference between a 6364 and a 6374 motor? Does it matter for a single-motor setup?
```

---
## \#9 Posted by: jrpwit Posted at: 2017-07-12T23:09:23.123Z Reads: 137

```
Bigger is always better. The difference is size however I think you will be happy with either one! Good luck!!!
```

---
## \#10 Posted by: pat.speed Posted at: 2017-07-12T23:36:34.277Z Reads: 129

```
The 63-74 just has more torque but will most likely be fine with the 63-64 unless you have very big hills and weight quite a lot
```

---
## \#11 Posted by: jammin Posted at: 2017-07-16T03:10:02.367Z Reads: 116

```
More parts are coming in! I've already received my longboard hardware and some RC components: I have the GT2B, XT90 connectors and wiring.

Lipos, SK3, and DIYElectricSkateboard parts are all coming in on Monday / Tuesday!!
```

---
## \#12 Posted by: jammin Posted at: 2017-07-18T01:06:30.451Z Reads: 118

```
Almost all of my parts came in, I'll be taking a photo when everything is here and whatnot.

I just realized that the SK3 motor has a 4mm bullet connector, while the Torque VESC has a 5.5mm bullet connector. I don't have any spare bullet connectors lying around; how should I connect these? I'm thinking about directly soldering the phase wires to the VESC but I'm worried if one of them is DOA <i>or</i> if I reverse the polarity of the phase wires.

Another option is xt60 / xt90 connectors: could I attach each phase wire to an xt60 / xt90?

Thoughts?
```

---
## \#13 Posted by: jammin Posted at: 2017-07-18T19:22:23.857Z Reads: 104

```
<img src="/uploads/db1493/original/3X/0/c/0c69aaa7c8b821b100fefbbdd733f46ffc7f6043.jpg" width="666" height="499">

Non-electric build is complete! I also decided just to buy some 4 -> 5.5 bullet adapters, since it was the simplest solution. Unfortunately I had a bike accident 2 days ago so I won't be able to ride this until later this week.
```

---
## \#14 Posted by: jammin Posted at: 2017-07-30T02:32:45.111Z Reads: 86

```
The build is done!!!
<img src="/uploads/db1493/original/3X/9/6/96d7d3b0dbfaab2004b5c9917cd286fd9d38ce6d.jpg" width="666" height="500">

and more photos available here: http://imgur.com/a/vHyjV

Thanks to everyone on these forums for the help! :)
```

---
## \#15 Posted by: Jedi Posted at: 2017-07-30T03:27:17.986Z Reads: 78

```
Nice work! You may want to reduce the slack in those motor wires.
```

---
## \#16 Posted by: jammin Posted at: 2017-07-30T03:49:34.575Z Reads: 78

```
For sure! I actually need to velcro the whole build down, but I couldn't resist taking it around the block before then ;)
```

---
