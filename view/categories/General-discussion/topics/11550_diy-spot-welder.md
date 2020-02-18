# Diy spot welder

### Replies: 32 Views: 7160

## \#1 Posted by: 2-alex-2 Posted at: 2016-10-20T17:42:31.853Z Reads: 366

```
So I have 24 lg hg2 3000mah batteries arriving soon to build a 6s4p pack for my next project. I have some nickel 8mm wide strips to spot weld together. The only thing now is the spot welder I don't want to spend any money on buying one as will just add to the cost. I do have a second hand car battery which is one option but I now also have a microwave which I could make into one as well. But which will be best battery or microwave. Ideally I would rather use the battery as its a little less Voltage and less dangerous and would have to strip the microwave and buy a couple of bits for it. So who has used either options and which was best.
```

---
## \#2 Posted by: Maxid Posted at: 2016-10-20T18:12:25.268Z Reads: 363

```
just check that out:
http://www.electric-skateboard.builders/t/homebrewed-spot-welders/4500/41?u=maxid
```

---
## \#3 Posted by: sl33py Posted at: 2016-10-20T18:31:31.204Z Reads: 342

```
I built one and modified it per the [original ES thread](https://endless-sphere.com/forums/viewtopic.php?f=31&t=80315) (see page 3 for why added) w/ the additional schottky and TVS to prevent the Fets from being killed by the avalanche current.  I'm not an EE, but as best i can describe it - your 1-20ms spot weld, has about 100+ms of energy that has nowhere to go after the weld - so it goes back (in a bad way) through the mosfets.  Repeated use = cooked fets.

the schottky and tvs give a path to prevent this from hammering the fets.  Folks have said it fixes the issue.  it's a couple extra wires, and the two components - not too hard to wire up in addition to the typical Arduino board.

I actually am building another version w/ copper plate (like flangefrog's) and will probably sell my v1 when v2 is complete.  No real difference other than flat vs wire underneath and want to place in a small job box to protect all exposed wires.  I'll throw v1 up for sale when 2nd one is complete.  Slow/back-burner project.

HTH!
```

---
## \#4 Posted by: 2-alex-2 Posted at: 2016-10-20T18:44:56.633Z Reads: 296

```
Wasn't going to go out buy anything was going to try and use just the battery.
```

---
## \#5 Posted by: Maxid Posted at: 2016-10-20T18:47:15.955Z Reads: 292

```
:fearful:
Dude what did you think happens with a microwave? You would have to buy stuff and put serious work into it. You are dealing with high-current electricity here. This is no joke!
```

---
## \#6 Posted by: BornaQueen Posted at: 2016-10-20T18:52:46.516Z Reads: 287

```
https://youtu.be/KU1e-zq9hrw
```

---
## \#7 Posted by: 2-alex-2 Posted at: 2016-10-20T18:54:35.659Z Reads: 277

```
Yea I understand that it's high voltage would buy a couple of small switches to help control it and then some good insulation. Read through a few posts that show and tell me what need to do.
```

---
## \#8 Posted by: sl33py Posted at: 2016-10-20T18:57:17.981Z Reads: 273

```
[quote="Maxid, post:5, topic:11550"]
You are dealing with high-current electricity here. This is no joke!
[/quote]


This.

Seriously - we are talking major injury and voltage/amps here.  Do not fuck with a half baked solution or you can hurt yourself, or burn your place down.  

please be careful.  I'm not trying to sell you anything, just give you some links and info if you want to build one of the better DIY setup for spot welding.  There also is a good writeup on one of the microwave setups too - it just looked a lot more involved than the arduino project, so i went the arduino route personally.  

You might also check locally for one of the aliexpress plug-in spot welders that might be avaialable less than new.
```

---
## \#9 Posted by: 2-alex-2 Posted at: 2016-10-20T19:05:57.282Z Reads: 260

```
Like I said was going to try the car battery first something along the lines of this 

https://youtu.be/UU7QC5Uby6M
```

---
## \#10 Posted by: Maxid Posted at: 2016-10-20T19:13:00.750Z Reads: 250

```
so you have a huge solenoid switch at home? That switch alone is probably as much as I paid for the Arduino spot welder.
```

---
## \#11 Posted by: 2-alex-2 Posted at: 2016-10-20T19:14:25.635Z Reads: 244

```
No won't be using one going to find a suitable switch to handle it all.
```

---
## \#12 Posted by: Maxid Posted at: 2016-10-20T19:15:32.654Z Reads: 242

```
Good luck - there is a reason why he is using one you know. Personally I don't think you will find a suitable one that is cheaper.
```

---
## \#13 Posted by: Maxid Posted at: 2016-10-20T20:36:50.352Z Reads: 237

```
now I am scared of using mine unmodified - is it really that bad? Thought the guy knew what he was doing when he developed it so did not think something could go wrong using it the way it is.
```

---
## \#14 Posted by: lox897 Posted at: 2016-10-20T20:53:22.465Z Reads: 234

```
@sl33py I have the arduino side of my welder done but I need some advice on mosfets. I am going to order IRF1324PBF, this tvs: http://au.mouser.com/Search/m_ProductDetail.aspx?Littelfuse%2fSLD33-018%2f&qs=sGAEpiMZZMuNo3spt1BaV59JaOcfH3NfeKEsaAH2zCqgb1IAtfQvvA%3d%3d

and this schottky diode: 
VS-100BGQ015

Are they the right ones? And where does the schottky diode go? Thanks for the help!
```

---
## \#15 Posted by: sl33py Posted at: 2016-10-20T23:19:31.876Z Reads: 238

```
[quote="Maxid, post:13, topic:11550, full:true"]
now I am scared of using mine unmodified - is it really that bad? Thought the guy knew what he was doing when he developed it so did not think something could go wrong using it the way it is.
[/quote]

Sorry Maxid - not meant to be scary.  Worst case scenario - you have avalanche current going back into the mosfets and they fail.  When the fets fail (one or two or ... ) it will arc on contact, so in-between each weld i just touch them to some scrap or eachother quickly before next weld.  No spark - gtg!

When they fail - don't replace just one - replace them all at the same time.  I also upgraded from the IRF1405 to IRF1324PBF per others suggestions.  Supposed to be superior (but twice the cost roughly).

(*to be clear here folks i'm regurgitating what i learned from the ES threads - i'm not an EE*)

[quote="lox897, post:14, topic:11550, full:true"]
@sl33py I have the arduino side of my welder done but I need some advice on mosfets. I am going to order IRF1324PBF, this tvs: http://au.mouser.com/Search/m_ProductDetail.aspx?Littelfuse%2fSLD33-018%2f&qs=sGAEpiMZZMuNo3spt1BaV59JaOcfH3NfeKEsaAH2zCqgb1IAtfQvvA%3d%3d

and this schottky diode: VS-100BGQ015

Are they the right ones? And where does the schottky diode go? Thanks for the help!
[/quote]

It's the two components (Schottky and TVS), and a few wires.  Relatively simple and inexpensive - definitely supposed to help with longer life of the spot welder.  The original design works fine, and likely will work well for quite some time.  Some folks were doing unrecommended things like really long cables from the battery to the Arduino controller/board - and really long cables for the probes - those apparently make it more likely to fail.

My Mouser list for anyone to compare:
<img src="/uploads/db1493/original/3X/e/9/e91ee64bf410d8589430b6caf88964489f410e12.JPG" width="298" height="500">
(Note all parts are x2 to build a second spot welder - so just order 1/2 of what i did if you want to build only one)
Hopefully this will give you the specific models i found and was recommended to use.  Can't speak to "alternatives" very well, but you might pose those questions in the ES thread where the more knowledgeable experts can answer.

I realize i don't have a pic of the finished board ready to go.  So on the ES thread i'll "borrow" a pic of flangefrogs or one of the others to show the wiring and placement of the Schottky and TVS:
<img src="/uploads/db1493/original/3X/a/d/adad8fe72a4c475d58bc3af806d7833fc3b2dd0b.JPG" width="666" height="500">
(Flangefrog's lower board - note he uses copper vs aluminum, and mounts the FETs under the copper vs on top (to allow the legs to reach/contact the bottom copper wire/bar.  I mounted mine on top of the aluminum bar, and built a small solder bridge to reinforce that connection (some have burnt the traces - this is intended to help prevent))

I definitely recommend reading through the linked ES thread, and the original one regarding Riba's original DIY spotwelder kit he offered.  Last i check around 24 pages... but tons of good info if you have the patience to read through it all.  [Here](https://endless-sphere.com/forums/viewtopic.php?f=14&t=81400).

Best of luck everyone - happy to help as i can if you have a question let me know!
```

---
## \#16 Posted by: lox897 Posted at: 2016-10-20T23:56:47.155Z Reads: 205

```
Thanks sl33py. I see where the schettky diode is now. It is that thing at the bottom right? Just beneath the wire
```

---
## \#17 Posted by: Maxid Posted at: 2016-10-25T12:12:18.600Z Reads: 196

```
Just tried my spot welder with a 700A car battery.
The current is large enough so that solder melts when I hold the tips on a piece of it.
However I can't connect two nickel strips permanently. They stick to each other but can be pulled apart very easily. Any idea? Blown Mosfets? Is there a way to test if they are good or not?
```

---
## \#18 Posted by: sl33py Posted at: 2016-10-26T01:18:48.543Z Reads: 203

```
if the mosfet fails - it should allow voltage all the time and the tips should spark when contact (without foot pedal actuation).

without power - there are a few steps to use multimeter to test.  Easiest (i'm no expert) is to follow some folks who know what they are doing and the steps via a quick google search.  Some testing looks to require a more advanced DMM with features my inexpensive DMM does not have.

If you find a mosfet has failed - i've heard that it's best to replace ALL the mosfets at that time.  Any you leave will be prone to fail and replacing all is the best solution (again from the ES thread).

If you have a really powerful battery (not sure if 700A qualifies) - i know folks recommend adjusting your pulse time down, or even downgrading to a smaller battery.  What settings are you using, with what thickness?  I did some test welds on a dead AA battery w/ some 8mm .15 nickel - rock solid and hard to remove even with pliers.  I do notice a difference between fully charged vs a bit low.

From flangefrog he recommended the following pulse times (again varies depending on battery i'd assume):
[quote]
I tried both 0.2mm nickel, and 0.15mm nickel and copper. About 8ms 
worked well for the 0.15 nickel and 12ms for the 0.2mm nickel. Less time
 would probably work with a newer battery.[/quote]

@maxid - Let us know your settings, and thickness of what metal (nickel or nickel plated steel?) - i'd guess adjusting the pulse time down first.

@lox897 - yep the square schottky diode is under the wire that has the TVS diode in the middle (above/alongside the board).  The orientation is the pointed end goes towards the wire to the probe.

Hope that helps!
```

---
## \#19 Posted by: JuniorPotato93 Posted at: 2016-10-26T02:21:20.048Z Reads: 203

```
@thefer @Blacksheep 
This is the basic schematic of the one I made. Nothing fancy but it does the job. Theres also no way to accurately time the duration of weld so I practiced my pulsations with my index finger untill I was as calibrated as a torque wrench at nasa :wink: aka I spent like 30 mins trying to to melt the shit out of the strips. I also practiced on a few dead AA batteries I had laying around and that really helped.
[Lugs](http://www.excess-supply.com/site/cartpics/large/2985/XT-0.jpg) [4 Gage Cable](http://www.princessauto.com/en/detail/-4-welding-cable-sold-by-the-foot-/A-p8228041e) [Momentary Switch](https://cdn.shopify.com/s/files/1/1490/5112/products/02750016_00_a0711d55-ebdf-4421-8a7b-f38143a18f04_2048x2048_crop_center.progressive.jpg?v=1473910484) [14 AWG Copper Wire](http://www.princessauto.com/en/detail/14-gauge-25-ft-primary-wire/A-p8211062e)

<img src="/uploads/db1493/original/3X/6/f/6f5e7dc49551234d0aef4315c0a1045e3204489e.png" width="690" height="371">

Also, grounding wire goes from the transformer to the ground in the plug.

<img src="/uploads/db1493/original/3X/e/e/ee6634b04c6574ae7e5ea18e33f9fcb5ba145e61.jpg" width="690" height="388">

<img src="/uploads/db1493/original/3X/4/b/4bf0bc027ec90c8f7c0b57e0f412c463bb177fca.jpg" width="690" height="388">

<img src="/uploads/db1493/original/3X/9/f/9f55ed6d533401c752c78e103492ffab5b210164.jpg" width="690" height="388">

<img src="/uploads/db1493/original/3X/b/2/b2d4b60c12dd52686aa6214b708a648d33f6893c.jpg" width="690" height="388">
```

---
## \#20 Posted by: Eboosted Posted at: 2017-03-15T23:02:21.682Z Reads: 181

```
Is there a new version of the Arduino Spot Welder you can buy ready to use with the avalanche current problem fixed?
```

---
## \#21 Posted by: sl33py Posted at: 2017-03-16T22:37:29.082Z Reads: 174

```
[quote="Eboosted, post:20, topic:11550, full:true"]
Is there a new version of the Arduino Spot Welder you can buy ready to use with the avalanche current problem fixed?
[/quote]


@Eboosted - KaeptnBalu has a pre-made now.  There is an additional "kit" for the diode set (Shottky, TVS) - to stop the avalanche current killing your FETs.

I would want to confirm the FETs are the upgraded 1324 (iirc?) vs the "standard" in the BOM.  Worth the extra $ IMO (reading from true experts on ES).

Here's the link to his pre-made kit (waitlist unfortunately):
https://www.tindie.com/products/KaeptnBalu/diy-arduino-battery-spot-welder-prebuilt-kit/#electric-skateboard-electronics  

I built mine w/ the Shottky and TVS, and plan to build a second as it was a fun project.  I would suggest you do it if you want to make your own - not hard and the updated code from KaeptnBalu is definitely nicer than the original.

HTH - GL!
```

---
## \#22 Posted by: tonystark Posted at: 2017-05-09T17:09:03.400Z Reads: 159

```
Are you using any timing device? Does not it burn hikes through?
```

---
## \#23 Posted by: trampalovesshekels Posted at: 2017-05-11T07:08:08.428Z Reads: 153

```
Hey @sl33py have you built the spot welder v2, by any chance do you have an updated bom ?
```

---
## \#24 Posted by: akira Posted at: 2017-05-11T07:11:28.214Z Reads: 153

```
Here you go for the new BOM : 
https://github.com/KaeptnBalu/Arduino_Spot_Welder_V2/tree/master/Parts
```

---
## \#26 Posted by: trampalovesshekels Posted at: 2017-05-13T02:54:17.082Z Reads: 141

```
Damn good job flagging my cmment smarties, I guess you guys know everything amirite
```

---
## \#27 Posted by: korryh Posted at: 2017-05-27T06:30:57.332Z Reads: 137

```
Had a chance to use the arduino spot welder today that I borrowed from @sl33py.  I bought a cheapy wallyworld battery for 49.99 and started welding (after practicing a bit).  I am using .15mm x 8mm nickel, 3 layers and it worked like a champ - one layer at a time. I played with the settings for this battery (650CA) and ended up with 17 for the setting. I decided to make a segmented 10s3p for my trampa deck so it can be flexible. 

So if you are on the fence about making or buying something like this, I would highly suggest this one. This is my first battery and if I can do it then anyone can.  It works awesome and you dont have to worry about the one from China blowing out after 3 welds if it works. My 2 cents

<img src="/uploads/db1493/original/3X/6/b/6b514b8d10fdaa42c24f72ce11d60cf0acb1d35c.JPG" width="666" height="500">





<img src="/uploads/db1493/original/3X/0/a/0ac803299f45035bfba41c8fb16788363dbff34a.JPG" width="375" height="500">

<img src="/uploads/db1493/original/3X/9/8/98db1c30dda1ca56b7bcea860053e955d66d0eb8.JPG" width="666" height="500">

<img src="/uploads/db1493/original/3X/4/3/4340292d41d670d8cf65994835aa7decb388fb7a.JPG" width="375" height="500">

<img src="/uploads/db1493/original/3X/e/e/eeafd887def9fab9624a001759f17eeaf35d8c09.JPG" width="666" height="500">
Ended up using a neo magnet for a clamp to hold down the strips and a velcro strap to hold the cells close together.
```

---
## \#28 Posted by: Eboosted Posted at: 2017-05-27T06:44:07.680Z Reads: 129

```
Why are you leaving such a long nickel strip at one side? Are you using it to connect the packs? How are you securing that strip in order to avoid continuous flexing and possibly long time strip cracking?
```

---
## \#29 Posted by: korryh Posted at: 2017-05-27T08:28:16.084Z Reads: 130

```
I am standing on the shoulders (copying)of white pony with his segmented pack. I will be using copper braid so the sections will be flexible.  I am also trying my hand at CF here next week for the cover.
```

---
## \#30 Posted by: Smorto Posted at: 2017-05-28T00:59:05.642Z Reads: 120

```
Could you walk me through the wiring setup of this welder? It looks a little more complicated in these pictures then in the diagrams I saw...
```

---
## \#31 Posted by: korryh Posted at: 2017-05-28T06:28:33.460Z Reads: 114

```
This has the Shottky and TVS.  As explained above. The board is connected to the negative post with the Shottky grey ring facing away from the neg post to the other side of the board. the TVS is connected from the other side of the board to the positive post of the battery. Then one of the electrodes is connected to the other side of the board and the other electrode is connected to the positive post of the battery.   The foot petal is connected to the top of the board with the white just connector and the other black and Ted wires are to power the arduino.
```

---
## \#32 Posted by: Smorto Posted at: 2017-05-28T13:13:44.626Z Reads: 110

```
Ahhhh ok, it was more complicated due to the TVS and Schottky, my mistake!
```

---
## \#33 Posted by: sl33py Posted at: 2017-05-29T19:45:21.811Z Reads: 102

```
Nice work Korry!

I read the entire thread on ES, and this was determined to be key for longer life of the FETs (i also used the upgraded FETs which were recommended).  They stop a ~100ms waterfall voltage spike that hammers the FETs otherwise and leads to early failure for them.  And you can't just replace one FET (you technically *can*) as they should be all replaced at the same time (and most expensive component).  my reader's digest synopsis from ES experts.

Kaeptnbalu's code was an improvement over the original, and he has some for sale in EU at a reasonable price - plus he has the diodes as an add on which i recommend too.
```

---
