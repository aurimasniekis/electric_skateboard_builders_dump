# &ldquo;Path of Esk8&rdquo; Build Tree

### Replies: 24 Views: 3306

## \#1 Posted by: E-Boarding Posted at: 2017-01-27T19:30:49.913Z Reads: 347

```
Hey Builders,

the last few days I was working on something that may help visualize your build, helps with calculations and is easy to use. I came up with this Build-Tree:

<img src="/uploads/db1493/original/3X/f/b/fbd01b1e5722f6ae66cbbe84d98a87fd4f593045.jpg" width="690" height="396">

**BETA Versions**
http://esk8-dresden.de/poe/v0.2/
http://esk8-dresden.de/poe/v0.1/

**What does it?**

* it visualization your build (just for the fun of it)
* it shows beginners how eboard-technology works
* you can plan your next build
* it does basic calculations (you need to put in your params or use default values)
* add/remove/exchange parts and see performance/weight change instantly just by clicking bubbles
* range is calculate with 10km/100Wh
* you can share your build with others without explaning every parameter
* it shows a lot of features your board don't have
* you can check marketing specs of china-boards

**What it doesn't do**
* exact calculations (you can't specify every parameter and some options are not availalbe)
* show costs of your build
* show quality of your build
* features are subjective, don't take everything too seroiusly ;)
* it doesn't check if your build makes sense at all (you can specify a lot of bullshit but don't blame me if your build fails)
* it doesn't work on smartphones and shitty old browsers
* you can't read every text, because it too small
* imperial system
* mountainboards

**Examples**
_One of my Boards_
http://esk8-dresden.de/poe/v0.1/?tree=18650,Deck,Wood,Trucks,Suspension,Hardware,ESC,Battery,Enclosure,BMS,Li-ion,1S1P,5S,6S,8S,10S,2P,3P,4P,Single,Inrunner,Mount,Belt,HTD5,9mm,12mm,15mm,MotorP,WheelP,Wheels,2W,3W,4W,70mm,75mm,80mm,83mm,90mm,97mm,ABEC11,Control,Remote,Finger,Splash,&cellweight=45&cellcapacity=3500&motorweight=1&kv=170&gear=31&motorteeths=15&wheelteeths=48&durometer=75

_ACTON QU4TRO_ (not fully correct)
http://esk8-dresden.de/poe/v0.1/?tree=Deck,Wood,Trucks,Hardware,ESC,Control,Remote,Battery,Enclosure,BMS,Li-ion,LiFePO4,1S1P,5S,6S,8S,10S,2P,3P,Single,Dual,Tripple,Quatro,Outrunner,Hubs,Gear,70mm,75mm,80mm,83mm,90mm,97mm,Lights,SAM,&name=QU4TRO&deckweight=2&cellweight=45&cellvoltage=3.2&cellcapacity=2200&durometer=80

_Geared-Hub (Drive-Train only exmaple (Stary-like)_
http://esk8-dresden.de/poe/v0.1/?tree=Single,Outrunner,Hubs,Gear,Wheels,2W,3W,70mm,75mm,Clones,&durometer=80

**Whats next?**
* which important features are missing?
* which calculations are totally wrong?
* what are good default-values? (motor-weight, motor-kv, wheel-weight, battery capacity etc.)
* how to improve texts?
* how to improve usability?
* how to imporve graphics? (background-picture, pictures for features, ...)
* how to calculculate torque and hill climb ability?

Enjoy, it's free to use :)

p.s. I don't know if this the correct category for this, admin feel free to move it to general or something
```

---
## \#2 Posted by: Michaelinvegas Posted at: 2017-01-27T19:39:10.744Z Reads: 246

```
Oh my @E-Boarding .... really getting into the psychy of this whole thing...ain't you? Lol

Some one will soon diagnose ESk8 as a mental health issue .....

Get ready for the little white coats guys!!!
```

---
## \#3 Posted by: osbor Posted at: 2017-01-27T19:45:46.744Z Reads: 236

```
i am very much digging this, if you could get the code from the esk8 calculator and find a way to estimate range on flat ground this would be a super easy build estimator tool

**edit:** oh wait oops, it does estimate range actually, seems to be going by the 10Wh=1km rule, and it does calculate watt hours from the number of cells used
```

---
## \#4 Posted by: ajaynagra Posted at: 2017-01-27T22:10:47.679Z Reads: 225

```
Maybe estimate range depending on cells used?

Nice work though

Enter weight at the start? 

This is pretty cool though
```

---
## \#5 Posted by: osbor Posted at: 2017-01-28T17:22:32.683Z Reads: 185

```
giving this link copying feature a try....

http://esk8-dresden.de/poe/v0.1/?tree=18650,Deck,Wood,Kicktail,Trucks,Hardware,ESC,VESC,4.12,Control,Remote,Thumb,Battery,Enclosure,BMS,Li-ion,1S1P,5S,6S,8S,10S,2P,3P,Single,Outrunner,Mount,Belt,9mm,12mm,MotorP,WheelP,Wheels,2W,3W,4W,70mm,75mm,80mm,83mm,90mm,97mm,ABEC11,&name=Nobody&cellweight=45&cellcapacity=2500&motorteeths=12&wheelteeths=36

named it nobody because i suddenly remembered kingdom heart's excellent OST and the asthetic of the nobodies which i used to like. grip tape in the nobody sigil would be neat

https://img1.etsystatic.com/021/0/6423241/il_340x270.482065977_3v3f.jpg
```

---
## \#6 Posted by: E-Boarding Posted at: 2017-01-28T18:21:50.074Z Reads: 153

```
you've no Battery Enclosure and no BMS

Do the specs match the real specs of your board or is something totally wrong?
```

---
## \#7 Posted by: osbor Posted at: 2017-01-28T18:32:59.860Z Reads: 148

```
oh whoops, must have missed those, added them since i definitely plan on having both of those things
```

---
## \#8 Posted by: makevoid Posted at: 2017-01-28T22:46:08.736Z Reads: 147

```
@E-Boarding, that's awesome! I used it to make the diagram of my next build (added some labels on the image).

[<img src="/uploads/db1493/original/3X/c/5/c5c470a8b938bcc6bbc3c7c54927cc2d70a8cde6.png" width="690" height="352">](http://esk8-dresden.de/poe/v0.1/?tree=18650,Deck,Wood,Trucks,Hardware,ESC,VESC,4.12,Control,Remote,Finger,Battery,Enclosure,LCD,Li-ion,1S1P,5S,6S,8S,10S,2P,3P,4P,Single,Dual,Outrunner,Mount,Hubs,Wheels,2W,3W,4W,70mm,75mm,80mm,83mm,90mm,97mm,Clones,Splash,&cellweight=4)

Here are my two builds diagram, this tool is really cool because you can compare them with a glance:

Builds plan:

[MKV 3](http://esk8-dresden.de/poe/v0.1/?tree=18650,Deck,Wood,Trucks,Hardware,ESC,VESC,4.12,Control,Remote,Finger,Battery,Enclosure,LCD,Li-ion,1S1P,5S,6S,8S,10S,2P,3P,4P,Single,Dual,Outrunner,Mount,Hubs,Wheels,2W,3W,4W,70mm,75mm,80mm,83mm,90mm,97mm,Clones,Splash,&cellweight=4)

[MKV2 dual](http://esk8-dresden.de/poe/v0.1/?tree=18650,Deck,Wood,Trucks,Hardware,ESC,VESC,4.12,Control,Remote,Finger,Battery,Enclosure,LCD,Li-ion,1S1P,5S,6S,8S,2P,3P,4P,5P,Single,Dual,Outrunner,Mount,Belt,9mm,12mm,MotorP,WheelP,Wheels,2W,3W,4W,70mm,75mm,80mm,83mm,90mm,97mm,Clones,Splash,&cellweight=45&gear=42&motorteeths=15&wheelteeths=36)

---

I tried to modify the colors of the js canvas program a bit, if you want here's a version with these colors based on the one downloaded via "Save as" from your web page + did some other small changes - here's my version zip:EDIT-REMOVED  (I hope you're ok that I hosted my version here EDIT-REMOVED but if you don't want that I can take it down, also if you want to publish the non-minified js source code, that could be good if somebody else wants to customize it / improve it)

good stuff

edit - removed my version so links point all to e-boarding's version
```

---
## \#9 Posted by: Okami Posted at: 2017-01-28T22:48:24.564Z Reads: 119

```
The idea is nice.. I'll probably still need a couple of days to go into this stuff.. but other than that - great! 

Sort of reminds of ''upgrades'' for videogame characters..
```

---
## \#10 Posted by: ajaynagra Posted at: 2017-01-28T22:49:45.495Z Reads: 116

```
Whats space age materials?
```

---
## \#11 Posted by: Alextech Posted at: 2017-01-28T22:49:57.208Z Reads: 108

```
I lvor what your doing! I like to see structure when building. @Okami Totally. Gotta reach lvl.5
```

---
## \#12 Posted by: E-Boarding Posted at: 2017-01-29T07:35:54.737Z Reads: 111

```
@ajaynagra
from the ACTON Kickstarter Page:
"We built BLINK from space-age materials using completely new and patent pending construction"

@makevoid
You can download it and use it for your own, that's fine, but I don't want this to spread in different version on different domains over the internet.
I'll do updates, people use these links to share and I want them to point to my domain to keep a bit control of my work, that's the reason I don't publish the non-minified version for now ;)
If you like other colors (and/or other features), I'll add these colours and maybe a choose-your-colour option to my server.
```

---
## \#13 Posted by: Michael319 Posted at: 2017-01-29T07:45:12.540Z Reads: 103

```
Really cool man,
 

https://i.gyazo.com/3cb4956b81fedad4d8b4e49e653b391c.png
```

---
## \#14 Posted by: makevoid Posted at: 2017-01-29T12:28:00.589Z Reads: 94

```
done, removed the hosted version and the link to the zip - yes I think changing the base colors to increase contrast a bit will help with readability - also I would not tag the Flywheels Clones as "Cheap Wheels from China", just sayin ^^
```

---
## \#15 Posted by: lowGuido Posted at: 2017-01-29T13:16:33.169Z Reads: 94

```
pretty cool.
bit disappointed that it didn't have kick assist as a control method though.

also it doesn't allow for UDR drive boards.
```

---
## \#16 Posted by: E-Boarding Posted at: 2017-01-29T14:22:27.099Z Reads: 92

```
I'll add feature, not everything but important ones if needed, next update will include "LED-Wheels" and "Sharkwheels" for example and maybe an option for bigger or smaller tires

by "kick assist" you mean the "no acceleration" mode by ackermaniacs firmware?

What ist UDR, you mean pneumatics?
```

---
## \#17 Posted by: lowGuido Posted at: 2017-01-29T15:15:01.170Z Reads: 87

```
kick assist is like pedelec for skateboards. you kick the board up to speed and it will continue at the speed you kick it to.
and UDR is Uneven Dual Rear where you have a higher kv motor on one wheel and a lower kv motor on the other.

admittedly both uncommon techniques, but so are wings and spoilers..
```

---
## \#18 Posted by: E-Boarding Posted at: 2017-01-31T17:23:00.925Z Reads: 116

```
so kick assist would be an ESC-Feature
UDR would make calculation difficult, I don't even know how to calculate this...

Speaking about Calculations:

Speed:
is pretty straight foward and no problem with this tool, defined by voltage, kv, geraing and wheelsize

Range:
1km/10Wh fix

Weight:
This can be calculated pretty good when I do know the weight of all parts.
To improve this, I need better default values, so the question is, can someone tell me the weight of their parts, like
-enclose
-motor mount
-motors
-70mm/80mm/83mm Wheels (with or without bearings)

Torque/Power/Hill-Climb:
Don't know how to calculate this
```

---
## \#19 Posted by: E-Boarding Posted at: 2017-02-11T12:05:04.395Z Reads: 112

```
I included a Hill-Climb and Force-Calculation in Version 0.2.

The magic (physics) behind this is the following:
We use the ACTON QU4TRO, we don't know the exact specs but we do know:
36V (10S)
400W Hub-Motor x 4
Wheels 99mm (I know they announced to change the wheeldiameter but for this calculation we use the old specs)
TopSpeed 37km/h
7,7 kg

That's all we need, first let's guess the motor-kv, it have to be about 55 rpm/V (You can calculate this, but I simply type in different kvs in my tool until the speed matches the marketing specs)

36V x 55 rpm/v = 1980 rpm (motor rpm)
This board has no gearing, so the wheel-rpm is the same

We asume we have a power loss of 25% (to heat and shit), so the max power that is transfered to the wheels goes down from 1600W to 1200W

What torque is that: (9549 * kW) / wheel-rpm so: (9549 * 1,2 kW / 1980 rpm) =  5,79 Nm
With 99mm, the force that can be put on the road is: 5,79Nm / (0,099m / 2) = 117 N

Final step, we have a 100kg person, what is the max hill he can climb: asin(117N / (100kg + 7,7kg) * 9,81) = 6,35° = 11,14%

The downhill force of a 107,7kg mass on this hill is 117 N. That's the force the board have to produce to maintain the speed of this mass. If you want to accelerate on this hill, you need more.
And there is also friction, but we have already calculated a energy loss of 25%.

You can change all of these parameter to whatever you like and do your own calculations.

ACTON claims a hill climbability for the QU4TRO of 30%. Hm, this is possible if the person is 34kg. :rolling_eyes:
If we have 100% efficiency, the person can have 48kg, yeah maybe they tested this in china with chinese people...

Otherwise we do need more powerful motors or smaler wheel diameters, or something is wrong with my magic, äh I mean physics :)

please prove me wrong if you can ;)
```

---
## \#20 Posted by: Okami Posted at: 2017-02-12T16:25:09.791Z Reads: 100

```
Made mine - nothing fancy:

http://esk8-dresden.de/poe/v0.2/?tree=18650,Deck,Wood,Short,Bindings,Trucks,Hardware,ESC,Control,Remote,Finger,Battery,Enclosure,LCD,Charger,Li-ion,1S1P,4S,5S,6S,2P,3P,4P,Single,Outrunner,Mount,Gear,Belt,9mm,12mm,15mm,MotorP,WheelP,Wheels,2W,3W,4W,70mm,diameter,&name=TheMummy&rider=90&esc=150&cellweight=45&cellcapacity=2050&motorweight=1280&kv=192&power=2500&gear=43&mountweight=250&motorteeths=15&wheelteeths=65&diameter=230

----
**Few recommendations:**

* Add mountainboard / all-terrain wheels (at least some of them, or just the size in inches)

* Battery range calculation would be great + the size of the battery also. You could define 3 values for range or let the user choose by himself.. (10wh (longboard), 15wh (eco mountainboard), 20wh faster/dual mountainboard)

* Labels like the @makevoid made look really nice.. definately should be / could be made as a ''default feature''/..

--


Perhaps had some more suggestions.. but will add later them, if I get to remember / spot them again
```

---
## \#21 Posted by: Print3r Posted at: 2017-05-07T07:31:03.472Z Reads: 72

```
I can't enter my motor power, moter kv, loss of heat/friction. First I tried clicking and typing in the boxes (couldn't write in the box), then I tried tabbing through the boxes (tab just skipped those boxes). Am I doing something wrong or are those values fixed?
```

---
## \#22 Posted by: E-Boarding Posted at: 2017-05-07T07:37:06.362Z Reads: 70

```
if they are grey, you cant edit them because your Build-Tree is missing a motor

active the "Single-Drive"-Node in the tree to edit motor-settings
```

---
## \#23 Posted by: Print3r Posted at: 2017-05-07T08:15:49.472Z Reads: 71

```
I understand now. It is very cool. Is there any reason that in the boxes I can only enter 1 digit at at time - as soon as I enter 1 digit it exits out of that box? I like that you included 'Rear spoiler' and 'Red paint', two essential parts of any speed machine ;) !
```

---
## \#24 Posted by: E-Boarding Posted at: 2017-05-07T11:11:31.452Z Reads: 66

```
Ah I see, this happens in Chrome, I usally use Firefox which works fine, will try to change it in the next version
```

---
