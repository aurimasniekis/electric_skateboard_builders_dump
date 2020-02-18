# Board is slightly curved, how to make enclosure

### Replies: 43 Views: 1915

## \#1 Posted by: dg798 Posted at: 2017-11-21T13:41:46.454Z Reads: 282

```
I have a kick tail and the bottom is a little curved on each side, how would I mount an enclosure to be flat against the board so water can’t get in? Do I just need to make a lip or do I need to make the lip curved a little bit.
```

---
## \#2 Posted by: mmaner Posted at: 2017-11-21T13:48:23.319Z Reads: 284

```
Depends on the material.  Are you buying or fabricating?  If using ABS, just hit it with a heat gun on each end and press down.
```

---
## \#3 Posted by: dg798 Posted at: 2017-11-21T13:49:19.003Z Reads: 278

```
I’m going to 3d print it with abs but I don’t have access to a heat gun, can I use a blow drier or something
```

---
## \#4 Posted by: longhairedboy Posted at: 2017-11-21T13:52:30.503Z Reads: 272

```
did you model the enclosure or is it something you found?

if you modeled it you could try to create a curve in the model for the deck then print tests with extremely low infill to see if the curve matches.
```

---
## \#5 Posted by: dg798 Posted at: 2017-11-21T13:53:31.210Z Reads: 253

```
I didn’t make a model yet but I have all the dimensions. Is there a way to Measire the curve of my board and add that to the design for the lip
```

---
## \#6 Posted by: longhairedboy Posted at: 2017-11-21T14:06:54.775Z Reads: 248

```
Sure. I'm no expert in math, but i can eyeball stuff. The way i do it is use a piece of stiff cardboard and a razor to first match the curve by hand. Once you have that sitting flush and shaved to perfection you can take measurements of that template and apply it to the model. Zoom 1:1 on your screen and you could even hold the cardboard up to the screen and see how close you got. 

From there it won't be absolutely perfect, but shoudl be damned close. Then you can make minor adjustments and do the reprint-with-low-infill thing to get it exact on a small piece of the model so you don't waste too much plastic.
```

---
## \#7 Posted by: GrecoMan Posted at: 2017-11-21T14:26:35.022Z Reads: 228

```
or he could get something rigid and lay it on the middle and measure the distance to the board from the outer edges...

your way is good too 😂
```

---
## \#8 Posted by: longhairedboy Posted at: 2017-11-21T14:35:10.807Z Reads: 215

```
that gives you three data points. A template stores infinite data points and can be referenced later and more easily for data points you didn't measure to begin with. You can make a triangle or a curve with three points. Add more points and you better define the curve.
```

---
## \#9 Posted by: GrecoMan Posted at: 2017-11-21T14:36:24.646Z Reads: 211

```
true but templates also become harder to make and less precise when you hold it up to the screen. i could make an enclosure to perfectly fit the concave of my deck in 3 points. W concave is a bit different
```

---
## \#10 Posted by: longhairedboy Posted at: 2017-11-21T14:40:33.894Z Reads: 202

```
there was a device with pins i saw once.. pins on sensors.. that could accurately measure curves with high resolution. 

i wish i had one. 

One day i will have all of the toys. All of them. That'll show them.
```

---
## \#11 Posted by: GrecoMan Posted at: 2017-11-21T14:41:21.656Z Reads: 198

```
at that point you might as well just 3d scan the board!

also, I don’t see a plane ticket in my email yet... get on it!
```

---
## \#12 Posted by: longhairedboy Posted at: 2017-11-21T14:56:02.942Z Reads: 195

```
I'll 3d scan your face!

Here's your ticket. Hope you don't mind Third Class.

<img src="/uploads/db1493/original/3X/0/d/0daef0cbb97b33302a88c623e95223c725c5a453.png" width="450" height="207">
```

---
## \#13 Posted by: GrecoMan Posted at: 2017-11-21T14:57:19.429Z Reads: 190

```
sweet! i’ll hop on the boat next week so I can be there in january
```

---
## \#14 Posted by: longhairedboy Posted at: 2017-11-21T14:58:15.429Z Reads: 186

```
You may not get there, i hear this boat likes ice water so much it got all broken up over it.
```

---
## \#15 Posted by: GrecoMan Posted at: 2017-11-21T15:02:36.689Z Reads: 186

```
my eboard is amphibious 😉
```

---
## \#16 Posted by: Pedrodemio Posted at: 2017-11-21T15:28:56.369Z Reads: 190

```
For my board I first tapped the board and made a grid on the bottom, then I using a dial indicator I measured each intersection of the grid and put the values in a spreadsheet. From there I exported the data as a cloud point and imported in the CAD, them it was a matter of fine tuning and modeling the outline using a picture. By having the actual deck on 3D it’s easy to use it to make the enclosure that fits perfectly when printed 



<img src="/uploads/db1493/original/3X/5/a/5a7d860b9a363275a0cc51f8089f9433256b7ed2.JPG" width="690" height="474"><img src="/uploads/db1493/original/3X/5/d/5df33e3ac246e997deed3b6ff3778b2243493338.jpeg" width="690" height="388"><img src="/uploads/db1493/original/3X/8/0/803a048b835565a04d0b760d4ac5413b388e3f2d.JPG" width="666" height="500"><img src="/uploads/db1493/original/3X/f/a/fa5f6e0a83da62dd2d7c43e8143c5ee3cd7728a7.jpeg" width="666" height="500"><img src="/uploads/db1493/original/3X/d/a/da423a293f5ab6edeceac9c90097135f99e3fac1.jpeg" width="666" height="500">
```

---
## \#17 Posted by: Acido Posted at: 2017-11-21T15:30:56.227Z Reads: 172

```
just use fiberglass, more work with hands but it should be done faster
than modeling printing modifying etc what ever you need to do 
when it dries just a bit of sand paper and paint and you are done
```

---
## \#18 Posted by: longhairedboy Posted at: 2017-11-21T15:47:07.180Z Reads: 174

```
but stay away from polyester resin. that includes Bondo. Its terrible.
```

---
## \#19 Posted by: Acido Posted at: 2017-11-21T17:01:14.259Z Reads: 165

```
Why do you think that, boats are made out of it especially the racing ones
I made my enclosure from it and I can basically stand on it without it breaking and its not even flat on the edges!
No cracks or anything, ive used 500-550g fiberglass and like 9 layers of it maybe that's the reason
```

---
## \#20 Posted by: longhairedboy Posted at: 2017-11-21T17:08:17.978Z Reads: 165

```
Its wretched and stinks and the fumes will destroy you. There are plenty of other resins out there that can be used in low ventilation areas without causing migraine and nausea. 

West Systems is expensive, but as an example it smells like mint and doesn't kill your head. There's also a ton of inexpensive organic stuff out there that will build a box quite well.
```

---
## \#21 Posted by: Acido Posted at: 2017-11-21T17:17:18.363Z Reads: 153

```
I do not worry about that, since I work in huge hangars/ or just a roof over my head ( no walls ), its the cheapest option out there, if you worry about the fumes go with other stuff, one small box made out of polyester wont kill you tho
```

---
## \#22 Posted by: longhairedboy Posted at: 2017-11-21T17:20:28.377Z Reads: 150

```
i built my first three boxes out of it, and several other things. It definitely does the job, but yeah, use it outside. Yuk.
```

---
## \#23 Posted by: GrecoMan Posted at: 2017-11-21T17:20:34.670Z Reads: 145

```
I think your missing the point.  Most people have to work in a sealed garage or basement, not a warehouse
```

---
## \#24 Posted by: Acido Posted at: 2017-11-21T17:55:08.856Z Reads: 141

```
Open the door maybe, you are in there for 20min tops, then just leave it outside to dry, for your annoying neighbors to smell
```

---
## \#25 Posted by: dg798 Posted at: 2017-11-21T17:57:49.415Z Reads: 139

```
@longhairedboy, I don’t know what u mean with the cardboard thing.
@grecoman how would I do your way?
```

---
## \#26 Posted by: longhairedboy Posted at: 2017-11-21T17:58:40.426Z Reads: 134

```
outside on a sunny day works. Did that a couple of times. Also you can get respirators.

Not to tip my foil hat, but 3M makes that shit smell bad on purpose then sells you their respirators so you don't have to smell it. Kind of genius actually, in a pathological kind of way.
```

---
## \#27 Posted by: GrecoMan Posted at: 2017-11-21T17:59:24.934Z Reads: 136

```
balance a ruler or something else rigid on the bottom of of the deck then use a caliper to measure the distance between the edge of you deck and the ruler
```

---
## \#28 Posted by: dg798 Posted at: 2017-11-21T18:00:08.317Z Reads: 137

```
Meaning measure it upwards toward the ruler or straight
```

---
## \#29 Posted by: GrecoMan Posted at: 2017-11-21T18:00:52.470Z Reads: 133

```
measure from the deck up to the ruler
```

---
## \#30 Posted by: dg798 Posted at: 2017-11-21T18:01:20.602Z Reads: 132

```
From both sides? Then where is the 3rd point
```

---
## \#31 Posted by: GrecoMan Posted at: 2017-11-21T18:04:51.157Z Reads: 125

```
the middle of your deck?
```

---
## \#32 Posted by: dg798 Posted at: 2017-11-21T18:05:52.444Z Reads: 131

```
Would someone mind making me a design of the enclosure with these dimensions and then when I get home I will adjust the lip and stuff?
Batteries Dimensions (LxWxH)- 5.60"x2.15"x2"
Vesc Dimensions (LxWxH)- 5.25"x2"x1"
I need 2 separate enclosures 1 for batteries and 1 for vesc.. the batteries enclosure needs to have 2 holes for xt60 to come out of and one hole in vesc enclosure for the vesc xt60 to come out of.
```

---
## \#33 Posted by: GrecoMan Posted at: 2017-11-21T18:08:02.149Z Reads: 126

```
i’ll do it for $10 😂
```

---
## \#34 Posted by: dg798 Posted at: 2017-11-21T18:08:02.426Z Reads: 131

```
So basically what your saying is, balance ruler across width of deck. Measure from both edges up to the ruler or do you mean up to the middle of the deck where the ruler is flat??
```

---
## \#35 Posted by: dg798 Posted at: 2017-11-21T18:08:39.569Z Reads: 130

```
You’ll print the enclosure for me too?😂
```

---
## \#36 Posted by: GrecoMan Posted at: 2017-11-21T18:10:41.098Z Reads: 137

```
measure where the arrows are.
<img src="/uploads/db1493/original/3X/e/3/e38fd41276225b049be0cc93118ef20c460c6472.jpg" width="375" height="500">
the three dots are where your points will be
```

---
## \#37 Posted by: dg798 Posted at: 2017-11-21T18:12:47.969Z Reads: 133

```
Sorry for all the noob questions but I just don’t get what you are saying with the ruler.
Can someone maybe post a pic of instructions on how to measure the curve?
```

---
## \#38 Posted by: GrecoMan Posted at: 2017-11-21T18:14:14.713Z Reads: 130

```
dude what is hard to understand?
```

---
## \#39 Posted by: Sk8Board Posted at: 2017-11-21T18:14:31.963Z Reads: 133

```
I had the same problem, I needed 2 enclosures and I designed the battery enclosure with the idea in mind to heat gun the thing and form it to the board, but it would use a ton of filament and I didn't model it for a series harness or a bms, both of which I wanted,  so I just bought some kydex off of Amazon. I didn't even make a form for the battery kydex and formed it by hand. 

If you decide to 3d print it, try to spray paint it with rubber coating.
```

---
## \#40 Posted by: dg798 Posted at: 2017-11-21T18:18:37.673Z Reads: 130

```
How do I measure the dot in the middle.
I get the ones on the side I just don’t get what you mean with the dot in the middle. Sorry
```

---
## \#41 Posted by: GrecoMan Posted at: 2017-11-22T13:55:50.185Z Reads: 113

```
in your cad software, create a 3-point arc. create the first two points the width of your deck apart. then create the middle point the height of one of the side measurements
```

---
## \#42 Posted by: dg798 Posted at: 2017-11-22T13:56:55.883Z Reads: 121

```
Ok got it thanks a lot
```

---
## \#43 Posted by: Tampaesk8er Posted at: 2018-11-10T17:22:18.094Z Reads: 40

```
I used Bondo resin and its no joke, i did it outside and wearing a double mask and still felt a little dizzy after i was done with it at tops 20 min.![image|373x500](upload://1FXUlw27PBZfI7zdKKWdfzppTrG.jpeg) ![image|669x500](upload://iQYqh2VnTfDiZwTVne4a3qMSXBH.jpeg) ![image|669x500](upload://un4zIBBU2j9krRbEqrBEDLpwUlS.jpeg)
```

---
