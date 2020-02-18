# Thiccn&rsquo;t &#124; Dual 5065 200kv &#124; 10s4p &#124; Dual FOCBOX &#124; Abec 11 107mm &#124; TB 218 trucks&#124; Hummie deck

### Replies: 18 Views: 866

## \#1 Posted by: jasonbhuynh Posted at: 2018-10-03T21:46:37.290Z Reads: 253

```
This is a build that's been working for about a month now. I call it Thiccn't because it's fairly sleek but relatively heavy, just enough that it's a pain to carry around campus when I have to be social and walk with my friends. At least I have an excuse to start another build (jk, I'm starting 2 more cause why not).

There was actually a previous iteration that was using Hummie v2 hubs, but I think their mileage finally got to them (I was at least the 3rd owner) and they were having overheating issues even though I'm 155 lbs fully geared. 

So I opted to replace them with a reasonably powered satellite motor drivetrain using racerstar 5065 200kv motors that I got from @hyperIon1 and mounts from @marcmt88 with a gear ratio of 15/38. I'm running sensored FOC with 35/70 and -10/-65 on each focbox, although I change it so often that those numbers are probably wrong. It's working flawlessly on one motor, the other motor jitters inconsistently because of reasons I have yet to pinpoint. Suggestions are welcome! 

Here are the pictures (parts list below):

![IMG_9315%202|375x500](upload://dC8GwTuTBv3iCRGSym958kObtKi.jpeg) !![IMG_9737%202|375x500](upload://nFK5qtzWNKVZqlU4xekcJCllNTF.jpeg) ![IMG_6688|375x500](upload://g3tX9mt3todBPDHvQYYByo1VMHM.jpeg) ![IMG_1435%202|375x500](upload://bqezQsswuFjhXsFVYlRgZMdjL2k.jpeg) ![IMG_6904%202|666x500](upload://xLAxPEZfpNmV0Nh4gz2j4CZzI9y.jpeg) 

Yes, the enclosure is crooked cause I'm an impatient person. Yes, I fucked up the drill holes for the inserts in the deck and the holes in the enclosure cause I'm an impatient person. And yes, the battery has a patchwork of fish paper because I had to go in a bunch of times and check cell life. I recently redid it and it looks much cleaner. I also taped down balance wires probably, don't remember. All parts inside the enclosure are velcro'd down or glued down depending on when they were installed and when I ran out of velcro.

Side note: I ended up JB welding the motor mounts at their final angle as I couldn't get them to stay properly angled without drastic measures. As such, the motors are the only thing I can change. I wanted to try surf-rodz anyway :rofl:.

Here's the parts list:

* Hummie deck (the older version with the 140mm cutout)
* 2x FOCBOX
* 2x Racerstar 5065 200kv from @hyperIon1  
* 15/38 gear ratio, wheel pulleys from @marcmt88 
* TB 218mm trucks
* ABEC 11 107mm superflys with zealous bearings
* @psychotiller Arc v2 enclosure
* 10s4p 30q battery built by myself using cell level fusing and spot welding, discharge bypassed
* hm-10 bluetooth module from aliexpress, courtesy of @Winfly  

Also, some local people have been curious as to what my lights setup is, so I'll just lay it out here in case someone else is. I used 4x sk98 clone flashlights from Amazon and mounted them on top of my trucks using .75 - 1.25 inch bar clamps (also from Amazon), 2 for each light. For the rear lights, I also jb welded red filters to the lenses. This can all be done for much cheaper than I did it, but I used Amazon because, again, I'm an impatient person.

Heres the link to the lights - note that these don't come with spacers so your 18650 cells will bounce around unless you make some yourself: https://www.amazon.com/gp/product/B01IQMIFR8/ref=oh_aui_detailpage_o00_s00?ie=UTF8&psc=1
the clamps - a bit pricey for what they are but pretty beefy:
https://www.amazon.com/gp/product/B0791NB4FM/ref=oh_aui_detailpage_o09_s00?ie=UTF8&psc=1
the filters - also pricey for what they are:
https://www.amazon.com/gp/product/B00X3J8KEI/ref=oh_aui_detailpage_o00_s00?ie=UTF8&psc=1

This build is basically in its final iteration because I have too much money spent and/or planned on being spent in the near future on this damn addiction. The only thing to do is to rebuild the battery as I think I have at least 2 dead cells. 2 of my parallel groups refuse to charge above 4.1v (on 2 different BMS). But I have a cells coming in so I can do so with very little down time on the board.
```

---
## \#2 Posted by: hyperIon1 Posted at: 2018-10-03T22:08:41.956Z Reads: 188

```
One has the gitters? Try switching focboxs to rule those out. If it runs flawlessly on the other focbox it could be a bad can-bus connection. 

So during setup, detection was fine?
```

---
## \#3 Posted by: jasonbhuynh Posted at: 2018-10-03T22:12:09.953Z Reads: 182

```
I'm using split ppm, I'll try switching focboxs as well as switching the order of the phase cables. Detection worked most of the time, but there were some errors, so it might just be a sensor cable is losing continuity as the motor either jitters or doesn't, and vibrations are affecting it.
```

---
## \#4 Posted by: thiswasandy Posted at: 2018-10-03T22:13:47.101Z Reads: 175

```
Whenever you switch make sure you redo motor detection (you may already know this).
```

---
## \#5 Posted by: jasonbhuynh Posted at: 2018-10-03T22:15:36.700Z Reads: 167

```
Yep, makes it a little bit of a pain to troubleshoot but I think it's worth it. Sensored is just amazing :heart_eyes:
```

---
## \#6 Posted by: hyperIon1 Posted at: 2018-10-03T22:20:54.844Z Reads: 154

```
I tested both, for setup on the bench because of the re-pined jst connectors.  They both detected fine for foc / bldc. One thing I do know is the solid wire used for the sensors is a pain.
```

---
## \#7 Posted by: trancejunkiexxl Posted at: 2018-10-03T22:27:09.576Z Reads: 152

```
Where did you get the braided cable protectors. I ordered some but the size ended up being way to small 😯
```

---
## \#8 Posted by: jasonbhuynh Posted at: 2018-10-03T22:27:53.320Z Reads: 152

```
They were already installed on the motors, so I can't help you there :frowning:
```

---
## \#9 Posted by: FranciscoV Posted at: 2018-10-03T22:28:32.077Z Reads: 143

```
Your shit is fassst 🤘🏼😆🤘🏼
```

---
## \#10 Posted by: jasonbhuynh Posted at: 2018-10-03T22:29:40.505Z Reads: 138

```
Maybe I should upgrade the battery to 12s to go faster :rofl::laughing:
```

---
## \#11 Posted by: FranciscoV Posted at: 2018-10-03T22:31:09.387Z Reads: 139

```
Do that and you’ll leave me in the dust 😬
Lmk when you’re ready for next round haha
```

---
## \#12 Posted by: dareno Posted at: 2018-10-04T11:56:42.478Z Reads: 134

```
Nice build love the hummie deck with the industrial lighting!  Oh and I couldn't see the crooked enclosure btw.
[quote="jasonbhuynh, post:3, topic:70062"]
the order of the phase cables.
[/quote]

That shouldn't be the issue if the motors are running the same way round.  If you had a phase short then poof.
try this process for determining correct phase wiring
Disconnect the motor from everything and disregard the sensor cable, if present.

Connect phase A to phase B and verify by hand spinning that there is choppy braking
Connect phase A to phase C and verify by hand spinning that there is choppy braking
Connect phase B to phase C and verify by hand spinning that there is choppy braking
Connect phase A to phase B to phase C and verify by hand spinning that there is strong, smooth braking

If any of the first 3 brakes feel different, the motor has an issue. They should feel  *identical* . The last brake should feel smooth and not be cogging.

This was given to me by a wise man and now I'm giving it to you.

[quote="jasonbhuynh, post:3, topic:70062"]
Detection worked most of the time,
[/quote]
detection should work all of the time or don't run it.  

[quote="jasonbhuynh, post:3, topic:70062"]
but there were some errors,
[/quote]
there shouldn't be errors and if there are what are they?

[quote="jasonbhuynh, post:1, topic:70062"]
cause I’m an impatient person.
[/quote]
Don't be impatient.  It will cost you in the end
```

---
## \#13 Posted by: jasonbhuynh Posted at: 2018-10-04T15:33:18.374Z Reads: 103

```
It was the sensor detection that occasionally failed, motor detection always worked. I think it’s fine cause sensors only run at very low speeds anyway and I usually just kick push if I’m having poor behavior.

Edit: by errors I just meant failed hall sensor detection
```

---
## \#14 Posted by: dareno Posted at: 2018-10-04T21:33:34.295Z Reads: 102

```
Be a little careful with hall errors too my friend.  My sk8 returned a hall error on a detection and still worked so off I went (I'm impatient too btw) and the vesc packed up first run.   Its a bone of contention that a hall sensor can cause this but nothing else was wrong.  Its one reason I don't use sensors anymore.  I suspect a short on the cabling caused it.
```

---
## \#15 Posted by: thiswasandy Posted at: 2018-10-05T01:08:05.593Z Reads: 102

```
If you're not using the hall sensors at this point disconnect the sensor wires to prevent a short to your VESC just in case.
```

---
## \#16 Posted by: jasonbhuynh Posted at: 2018-10-21T19:41:45.851Z Reads: 98

```
Small update: Upgraded to TB 6355 190kv motors. I had an older one (only like 100 miles, scratched up because it was riding really low on shitty streets), so I just bit the bullet bought another. 

![IMG_ADFC4F890B04-1|230x500](upload://3MxWJ7G84u2B8cR9ZbkHfG4E1Jj.jpeg) 

I ran out of electrical tape, so the bullet connections are insulated with kapton tape, as the heat shrink jobs were not perfect (on my end).

As for the performance, I have more torque at every speed from 0-32mph compared to the racerstars that were on here before. I can also hit 32mph compared to the 30-31mph I hit with the racerstar motors, although ymmv as kv is usually not what the specs state.

A new direction for the build:
I ordered a subsonic talon 37. I'll likely put this drivetrain on that deck, along with a 12s4p battery (maybe 5p, depending on enclosure width). I'll also change the wheel pulley to 40t for that extra torque. On this deck I'll put a 13s4p battery with my metasurf drives. Or maybe 13s2p with the metasurf drives and 10s2p with the carvon torquedrives :wink:
```

---
## \#17 Posted by: 702vegas Posted at: 2018-12-11T18:12:02.081Z Reads: 63

```
Hows the turning? Any bite?
```

---
## \#18 Posted by: jasonbhuynh Posted at: 2018-12-11T18:24:21.572Z Reads: 61

```
No bite on this build.
```

---
