# Mini Rover &#124; 22&rdquo; Carbon Fiber &#124; 125mm Trucks &#124; Hubs? &#124; 12S1P &#124; VESC-X

### Replies: 13 Views: 3908

## \#1 Posted by: faust Posted at: 2016-11-11T02:19:39.869Z Reads: 360

```
Hi all! 

My aim is to build a pocket transporter, something I can clip on my backpack and easily make it around campus. I have a [121C Rover Deck](http://www.121cboards.com/rover/) @ (1.5 lbs), 125mm Randal Trucks, and Shark Wheels. Here's a picture of what it'd look like fully assembled: 
http://www.121cboards.com/wp-content/uploads/2016/08/basic-rover-image.png

Here are the dimensions: 
http://www.121cboards.com/wp-content/uploads/2016/08/Rover-Dimensions-v1.2-1000w.png

**Requirements**
* Swappable Battery (range without weight)
* FOC-enabled (low noise)
* 15% grade for 200lbs+ 

**Current Design/Implementation**
* Hummie Steel Hub Motors (I need low-profile hubs so that I can put them on very small 125mm trucks. These seemed like the best I could buy). 
* No shark wheels (because hubs)
* 12s1p battery from Carvon (To prevent voltage sag, I hear the A123 26650 is the way to go).
* Looking into RoPD connectors for the swappable batteries.
* 2x Torqueboard VESCs. 
* GT2B remote
* 2x 121c Decks (The current 1.5lb board, unfortunately, has waay to much flex to be safe. I'm going to try to sandwich two of these decks together to add strength, then to see where I'm at. Potentially, I could cut some of the carbon fiber to implement some nifty enclosure options, we'll see).
```

---
## \#2 Posted by: Alextech Posted at: 2016-11-11T02:41:42.150Z Reads: 329

```
To begin if your going the hub motor route, You will need to buy the appropriate wheel size for the same as the hub motor. You can drill holes into the shark wheel for a pulley maybe 32t and then ether A) Weld on a motor mount or B) custom fabricate a clamp on motor mount. You have a set budget in mind? You can pack a decent amount of power in a small size but it will cost you.
```

---
## \#3 Posted by: faust Posted at: 2016-11-11T03:00:05.482Z Reads: 328

```
I'm pretty flexible when it comes to budget, say $1500 or so. The reason I'd like to build this myself is to make it perfect for my needs, and to also get a good deal of fun tinkering in. :) So in terms of parts, I don't believe it'd need to compromise too much.  

As for the wheels, my main priority is to get the right motor, then to be able to deal with rocks and/or cracks in the road as well as possible. I hear the snake wheels are good for that, but I'm not sure, so they're not a requirement. I have an Acton Blink with 83mm wheels that works great. Maybe even get the best of both worlds with 70mm shark wheels :)
```

---
## \#4 Posted by: faust Posted at: 2016-11-26T22:21:08.921Z Reads: 298

```
Just built my remote using the GT2B remote and the Mad Munkey v2 mod. Since the folks in that thread have already moved to a new and better mod, I'll just put these pics here. 

<img src="/uploads/db1493/original/3X/3/c/3cc088c7a35efe1b4e16ecca55ecd0193540a95d.jpg" width="690" height="388"><img src="/uploads/db1493/original/3X/a/2/a2921f7a141c5350638c6378bdcbbb9587475920.jpg" width="281" height="500"><img src="/uploads/db1493/original/3X/8/f/8f125d4be5c975ef65b473aa21880d98c7fe88f2.jpg" width="281" height="500">
I had to cut the pcboard somewhat to make it fit. Notice the line. 
<img src="/uploads/db1493/original/3X/2/0/20f408d079f8fef845ffdc2a9ef302a4c2e19694.jpg" width="281" height="500"><img src="/uploads/db1493/original/3X/6/3/63effd9a083a20fd138af5841bb6ad7511d57c3f.jpg" width="281" height="500">
Next time, I'll read *all* the steps before I get started. I desoldered the USB port and glued it to the proper outlet, instead of just having it stick out. I stuck a little shrink wrap around it.
<img src="/uploads/db1493/original/3X/d/3/d3eb827299c60b15db4f94fe7857e28123d50a3a.jpg" width="281" height="500">
<img src="/uploads/db1493/original/3X/7/f/7f3cc332be7afe4161d6649531482adf1e1f031d.jpg" width="281" height="500"><img src="/uploads/db1493/original/3X/6/b/6b23b4432e35386bafb5620de635764e3aa3e952.jpg" width="281" height="500">
```

---
## \#5 Posted by: faust Posted at: 2017-03-17T05:50:33.184Z Reads: 266

```
Here's the latest: 
<img src="/uploads/db1493/original/3X/d/9/d916072bc1f12cf5f3fcb99bee5bd8789ecfd539.jpg" width="281" height="500">
Here's a quick clip: https://www.youtube.com/watch?v=0fWOcp-MFo4&feature=youtu.be

@Hummie kindly helped me mount his hubs to it, but I'm going with a single-drive belt until I get a replacement VESC. <img src="/uploads/db1493/original/3X/4/6/46256367ad0106074a7948968b4648094cffbc3f.jpg" width="690" height="388">
<img src="/uploads/db1493/original/3X/e/3/e3ac30891b6418e105cf14312fd1fbf534eb81e0.jpg" width="281" height="500">
So much power on such a tiny board!

Even better, the battery is so powerful (60A discharge; 324Wh) that it can be used for my long-distance board (using @psychotiller's wheels). 
<img src="/uploads/db1493/original/3X/e/2/e20d276d47876a1b7186eacda7dc3179e13521a4.jpg" width="690" height="388"><img src="/uploads/db1493/original/3X/2/3/23b717c6e74871dd1a22b47f97caed5acf1e5684.jpg" width="690" height="388">
```

---
## \#6 Posted by: noazark Posted at: 2017-03-20T19:25:54.446Z Reads: 248

```
Soooo what is that battery and mount? I'm looking to build a mini like yours with a swappable battery but with an all terrain mech setup. @faust
Great fuckin job by the way this little thing is dope.
```

---
## \#7 Posted by: Mikenopolis Posted at: 2017-04-05T17:59:21.458Z Reads: 233

```
looks like an Onan
```

---
## \#8 Posted by: faust Posted at: 2017-04-06T18:12:46.521Z Reads: 227

```
Thanks!

The battery case and mount is used from the Onan X2, see https://www.electric-skateboard.builders/t/onan-x2-hack-jet-spud-swappable-10s2p-2x-vesc-hummie-hubs/14965/37 

Everything else from the X2 was gutted and removed (e.g., trucks, hubs, ESC, etc...). The battery had to be rebuilt from scratch because it was not powerful enough (default from Onan is 10S2P 20A discharge @ 4400mah, new battery is 10S3P 60A discharge @ 9000mAh). Hangers were from randall 125mm's, I forget who made the baseplate for the front truck (I needed to use a different one to match height).
```

---
## \#9 Posted by: EnderWiggin Posted at: 2017-06-25T02:07:36.388Z Reads: 190

```
Have you gotten the hub motor to work yet? I would really like to do something similar but with hub motors.
```

---
## \#10 Posted by: faust Posted at: 2017-10-11T18:52:14.734Z Reads: 163

```
Unfortunately, I was never able to get the Hubs to work smoothly. This is meant to be an "urban navigator" sort of board. It was built with street faires or crowded college campuses in mind, enabling you to easily stop and go at very slow speeds. I could never get the hubs to start and stop smoothly. 

Also unfortunately, it was stolen yesterday. :( https://www.reddit.com/r/ElectricSkateboarding/comments/75qnhf/22_carbon_fiber_with_swappable_battery_stolen/

I managed to make a TON of improvements to it: 
* 9000mAh swappable battery. This makes it the longest range for any swappable battery system (30x Samsung 30Qs). For comparison, this little battery is 9/10 the capacity of the Evolve GT at about 1/3 the size.
* 125mm Randall Trucks. This is the smallest wheelbase + trucks that I've seen on any esk8, making it extremely maneuverable in tight urban spaces.
* Integrated usb connectivity (made available on left slot)
* Integrated battery meter visible while riding (opposite the USB connection, not shown in image)
* Integrated Shredlights (powered using the esk8 battery, so you never have to worry about charging them).
* Bluetooth connectivity, ollinboards 170kv motor, FOCBox, Onan enclosure.
```

---
## \#11 Posted by: Vanarian Posted at: 2018-04-14T12:55:57.846Z Reads: 107

```
Hey, did you get this back on track? Sorry for the steal of your first board.

That's a neat idea.
```

---
## \#12 Posted by: DeathByBacon Posted at: 2018-06-21T19:19:33.590Z Reads: 81

```
Where can I buy these mounts for the Randal?
```

---
## \#13 Posted by: faust Posted at: 2018-06-21T22:36:33.600Z Reads: 72

```
Shortly after my board was stolen, I got injured, so I haven't been able to ride for months. Sad because the board was in complete condition -- the best esk8 I've ever owned. It was super smooth and maneuverable at like 1 mile an hour! I could walk with friends during street fairs and just cruise. 

As for the mounts, they require heavy modification to fit on the 125mm trucks (the wheels as well).
```

---
