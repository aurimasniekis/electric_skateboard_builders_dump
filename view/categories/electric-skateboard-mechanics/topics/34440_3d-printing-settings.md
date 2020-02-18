# 3D printing settings

### Replies: 11 Views: 514

## \#1 Posted by: esk8guy Posted at: 2017-10-01T03:28:06.060Z Reads: 59

```
what settings have you used when printing pulley gears with abs?
```

---
## \#2 Posted by: Pedrodemio Posted at: 2017-10-01T03:37:54.197Z Reads: 60

```
You need to take it slowly, since the tooth profile is small and going fast can deform it
The most important is to adjust jerk and acceleration on the printer itself tô prevene-te vibrations and resonance, 300mm/s^2 and 5mm/s^3 on the X-Y axis

As for print speeds, 40mm/s on the interior wall and 30 on the outer, the rest you can keep as you normally use

One important detail is that as I said the teeth is small, is dificult to print the profile exactly, a little bit of tweaking is needed. First print print the original profile and them wrap the belt around it and see if it fits perfectly with no play but without being tight on each cavity, if not you have to tweak the geometry until it fits 

To save material I would recommend printing a small section of the pulley, 6mm is enough, with a large hole in the center, only when you are sure that the profile is a perfect match to the belt touch print the full size

It is also important to increase the number of walls, the default 3 is to low, 5 or more is preferred. Wall extrusion thickness may need to be changed too if on the preview you have empty spaces on the tooth, it depends on the nozzle diameter

Cheers
```

---
## \#3 Posted by: esk8guy Posted at: 2017-10-01T03:39:53.759Z Reads: 52

```
i had the settings at 40mm/s and 3 shells and the file kept getting stuck at the same point on 3 different tries. I was told to try and put it through an "stl fixer". have you had any experience with that? if not do you know why it may have stopped?
```

---
## \#4 Posted by: esk8guy Posted at: 2017-10-01T03:40:35.745Z Reads: 50

```
i will be re-printing on tuesday with 5 shells at 20mm/s just to be sure..
```

---
## \#5 Posted by: Pedrodemio Posted at: 2017-10-01T03:42:50.180Z Reads: 48

```
Unfortunately no, did you download an already made file? Which slicer are you using?
```

---
## \#6 Posted by: esk8guy Posted at: 2017-10-01T03:45:08.733Z Reads: 45

```
no its a custom made file on inventor and then i export into the makerbot software and print on the makerbot replicator 2x. im printing at a local diy shop
```

---
## \#7 Posted by: Pedrodemio Posted at: 2017-10-01T03:48:08.620Z Reads: 39

```
It gets stuck when slicing or when printing? If you share the STL and the problem is on slicing I can give a try here
```

---
## \#8 Posted by: esk8guy Posted at: 2017-10-01T03:49:24.443Z Reads: 39

```
it gets stuck when printing. It gets about 7% through and fails
```

---
## \#9 Posted by: Pedrodemio Posted at: 2017-10-01T03:52:26.219Z Reads: 40

```
It's strange but happened to me, never found out why, you can give a try by exporting you file to .step or .igs and opening it in another CAD, most of them will verify drawing integrity and try to repair and them export as STL, maybe inventor is doing something with the STL that is crashing the gcode
```

---
## \#10 Posted by: esk8guy Posted at: 2017-10-01T03:55:37.067Z Reads: 39

```
yeah i ran it though the online "stl fixer" going to give it a try and if it doesnt work im going to have to take you up on that offer of you running it though your slicer. Thanks
```

---
## \#11 Posted by: GrecoMan Posted at: 2017-10-01T12:20:18.437Z Reads: 30

```
I’m an avid Inventor user and I know from experience that Inventor struggles with stls, whether it’s importing them or exporting them, I’ve had tons of issues. My recommendation is to;

Re-export the file
Download a program from the Autodesk App Store with a slicer in it
Make sure you units are correct when you export it
```

---
