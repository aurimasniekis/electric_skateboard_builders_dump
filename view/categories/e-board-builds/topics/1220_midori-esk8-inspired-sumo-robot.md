# Midori ESK8 inspired Sumo Robot

### Replies: 12 Views: 4636

## \#1 Posted by: Blasto Posted at: 2016-02-04T04:56:22.281Z Reads: 144

```
Well I know this is not a Eboard, but I designed this robot with most of the information I got from trolling around this forum, so i thought i'd share.

First off, what is a sumo robot, well in a nutshell, you take 2 sumo robots, stick them in a dohyo (arena) last one standing in the dohyo wins. The catch is, robots must be autonomous, max size of 20cmX20cm and under 3Kg. No circular saw nor flame throwers. Oh and the Dohyo is made out of steel, so the use of magnets to increase your down force on your wheels is encouraged.

<img src="/uploads/db1493/original/2X/f/fb285f2d571e4f6c0a15b6b4c8bad77764e0d14d.JPG" width="690" height="335">

What so eboard about it? Well it's wheeling a pair of VESC, TB's 5065 170Kv sensored motors and a 3:1 pulley reduction. Wheels will be 2.5", shore A60, casted by myself with smooth-on vita flex 60 polyurethane. Powered by 12S lipos.

<img src="/uploads/db1493/original/2X/7/776b88a2580d57aca95deaceb73086598c60c173.JPG" width="690" height="416">

for the moment I only have 3D renders of the whole thing, all the parts are being manufactured and will be receving them in the next weeks. I'll post the progress of the build.

<img src="/uploads/db1493/original/2X/0/038f163d27f74d6f3ac1984bc11845e51acb1db4.JPG" width="541" height="500">
under, showing off the magnets

<img src="/uploads/db1493/original/2X/a/a2d684d963732e47987e3d662f17e33626206a43.JPG" width="690" height="317">

The main PCB, where all the sensors and VESC interface, i'm using the Teensy 3.2 for a MCU.

<img src="/uploads/db1493/original/2X/c/cc842936eb034301e11113eb678faffe4a75aa43.JPG" width="625" height="500">

Power input pcb, same as vedder's anti spark board, but with 3 XT60 connectors to put the lipos in series.
```

---
## \#2 Posted by: torqueboards Posted at: 2016-02-04T15:15:40.428Z Reads: 119

```
Nice... Thanks for sharing.. Very interested in seeing the final results :smile:
```

---
## \#3 Posted by: trbt555 Posted at: 2016-02-04T15:23:39.328Z Reads: 120

```
I like the power PCB, how many Amps can it handle ?

Autonomous: like in "*no human controlling the robot by RC*"-autonomous ?
Can you elaborate on the logic ?
```

---
## \#4 Posted by: lowGuido Posted at: 2016-02-04T15:53:37.562Z Reads: 114

```
Id guess 100A


----------
```

---
## \#5 Posted by: Blasto Posted at: 2016-02-05T16:22:57.338Z Reads: 105

```
@trbt555 yes to robots are autonomous, you press the start button and cross your fingers.

They're equiped with infra red sensors to find the oponent and edge sensors so it does not fall of the arena.

Juste received the wheel pulley, sending that off again for some more machining
 <img src="/uploads/db1493/original/2X/6/6d87a56742349720910613c162f5f8f98a145907.jpeg" width="375" height="500">

I don't have an exact number for the power input pcb, But i'm sure i have more than enough copper on the pcb, i rittled the thing with vias

Printed the wheel hubs, 100%infill
<img src="/uploads/db1493/original/2X/b/be6145e282390d162551f4a6bf66818e7f89b719.jpeg" width="375" height="500"><img src="/uploads/db1493/original/2X/a/a3b95aa87a638832e37a9b9022d537714f9cdb55.jpeg" width="375" height="500">
```

---
## \#6 Posted by: Blasto Posted at: 2016-03-02T02:28:56.638Z Reads: 96

```
Finally received my billet, nice and green

<img src="/uploads/db1493/original/2X/d/d6d1f087099b5cbc11d2d4b886680f7dc94fd5d8.jpeg" width="375" height="500">

Motors are a tight fit!

<img src="/uploads/db1493/original/2X/c/c23291ef3faa5b1ae464fc0f92411440f3f6db36.jpeg" width="375" height="500">

<img src="/uploads/db1493/original/2X/5/55b72621b44e8a3d2dc22ef467e134a941af7494.jpeg" width="666" height="500">

<img src="/uploads/db1493/original/2X/1/12d50f46f029c2188ecb51baab1583d57bfe342c.jpeg" width="666" height="500">

More to come

<img src="/uploads/db1493/original/2X/e/e0d4e5b4a4d362d856bac9909963098ea2bfe802.jpeg" width="375" height="500">
```

---
## \#7 Posted by: cmatson Posted at: 2016-03-03T01:45:15.634Z Reads: 87

```
we will definitely need some videos once this guy is up and running!!
```

---
## \#8 Posted by: trbt555 Posted at: 2016-03-05T08:00:10.045Z Reads: 81

```
Is that chassis custom made or is it a part that's readily available ?
```

---
## \#9 Posted by: Blasto Posted at: 2016-03-05T16:17:25.189Z Reads: 84

```
Custom made for this unique application


Pic of the pulleys
<img src="/uploads/db1493/original/2X/c/cf1f81f01663618a1b24482ff49be90ad72a7efd.jpeg" width="666" height="500">
```

---
## \#10 Posted by: Blasto Posted at: 2016-03-12T14:11:44.037Z Reads: 80

```
Midori is the green and black bot. Yes that my stupid ass falling on the ground.

https://youtu.be/dVqDHGMyW-w
```

---
## \#11 Posted by: cmatson Posted at: 2016-03-12T20:04:43.234Z Reads: 76

```
holy shit man yours was a beast!

haha even though that other guy slammed yours into the wall in the end, your robot looked 10x better. The completely enclosed green and black case makes it look pretty mean!
```

---
## \#12 Posted by: Blasto Posted at: 2016-03-12T20:11:37.530Z Reads: 75

```
Well that's nothing, we had to dumb down the max power to 40% because it's on a wood arena. The real test is on a steel arena with a bunch of magnets and blasting around the arena at 100%
```

---
