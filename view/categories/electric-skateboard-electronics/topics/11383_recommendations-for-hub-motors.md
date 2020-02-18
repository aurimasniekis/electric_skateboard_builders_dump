# Recommendations for Hub Motors?

### Replies: 38 Views: 2352

## \#1 Posted by: Pantologist Posted at: 2016-10-18T21:18:10.529Z Reads: 177

```
Hey guys,

I am going to change my setup a bit and I want to get a set of hub motors instead of the belt driven setup that I currently have. I weight 170lb and I don't have many hills to worry about in my area. 

I am really inspired by Mellow and Inboard's hub motor design and I wanted to make my own. What do you guys see as the best hubs on the DIY market right now? I really love the idea behind having no belts and no pulleys etc. Sounds amazing but are there issues with heat and phase wires coming loose and shorting? 

I am currently planning on a 12S2P Samsung or LG pack with two Vescs and one of the Open Source BMS units from this forum.

Side Note: Are Mellow and Inboard actually using 12S1P packs to drive dual hubs? Sounds kinda sketchy.
```

---
## \#2 Posted by: lox897 Posted at: 2016-10-18T21:18:41.955Z Reads: 173

```
Hummie's or Carvon if you have the money
```

---
## \#3 Posted by: Pantologist Posted at: 2016-10-18T21:20:45.004Z Reads: 171

```
Does Hummie have a website? I've seen Carvons from Rik. They are pretty expensive, but I'd buy them if they work great.
```

---
## \#4 Posted by: willpark16 Posted at: 2016-10-18T21:21:03.242Z Reads: 164

```
yes he does ill see if i have the link
```

---
## \#5 Posted by: lox897 Posted at: 2016-10-18T21:21:08.385Z Reads: 163

```
Steelhubs.com is hummie's site
```

---
## \#6 Posted by: willpark16 Posted at: 2016-10-18T21:21:59.392Z Reads: 160

```
http://tppsf.com/steel-hubs/
```

---
## \#7 Posted by: lox897 Posted at: 2016-10-18T21:23:50.346Z Reads: 160

```
@willpark16 I was a bit too quick :sunglasses:
```

---
## \#8 Posted by: willpark16 Posted at: 2016-10-18T21:24:48.392Z Reads: 161

```
haha I tried at least btw im still working on fixing the extruder because i use the one at my school and some moron broke it
```

---
## \#9 Posted by: Hummie Posted at: 2016-10-18T21:25:03.839Z Reads: 158

```
 thanks guys but I only have a few of the aluminum left and am only excited to sell the biggie motors that arent on the site yet and waiting till they're in.
 instead of 80x56 wheels they're 80x101 rollers.
```

---
## \#10 Posted by: Pantologist Posted at: 2016-10-18T21:26:36.890Z Reads: 151

```
So you can get Hummies with Steel and Aluminum and just Steel? Is having all steel construction that big of a upgrade?
```

---
## \#11 Posted by: Hummie Posted at: 2016-10-18T21:30:29.819Z Reads: 154

```
they're all steel now.  1144 center and 1018 rotor.  piece of mind.  the aluminum had an anodized surface as typical, which is a very thin titanium coating, but still steel has such better mechanical properties.  

i never experienced a problem of the deforming aluminum but I'm one person...and no one has complained about it yet either but I'm waiting for it.
```

---
## \#12 Posted by: anon33082420 Posted at: 2016-10-18T21:45:48.904Z Reads: 151

```
<p>This post was flagged by the community and is temporarily hidden.</p>
```

---
## \#13 Posted by: lox897 Posted at: 2016-10-18T22:02:06.705Z Reads: 150

```
@willpark16 is it a makerbot? Our school had a makerbot and I convinced them to get an ultimaker.
```

---
## \#14 Posted by: anorak234 Posted at: 2016-10-18T22:06:32.774Z Reads: 151

```
@torqueboards single hub motor works well. I had one problem with a loose magnet but epoxy made it a quick fix. Never had any urethane slippage or overheating, it's been used with 3s and 6s systems. Also by far the best deal you will see for hubs
```

---
## \#15 Posted by: Michaelinvegas Posted at: 2016-10-18T22:25:20.473Z Reads: 147

```
Talk to @ekitesurfer he's just got a dual v2.5 carvon and I'm just waiting on a VESC to try out my single
```

---
## \#16 Posted by: RunPlayBack Posted at: 2016-10-18T23:54:16.677Z Reads: 141

```
I'm currently converting all my Carvon v2 singles to v2.5 they are built like tanks
```

---
## \#17 Posted by: ekitesurfer Posted at: 2016-10-19T04:17:10.769Z Reads: 132

```
Single 2.5 probably great for flat ground, small hills. Dual 2.5 is the only way to go IMO. So nice! I have the perfect San Francisco type street to test these things on, @Michaelinvegas bring your single 2.5 over and we can test out both. Single might get the job done, but what's an extra bit of money when you get so many benefits from going dual? Single probably makes it up the hill, dual you are killing it (10s, 170#)
```

---
## \#18 Posted by: Maxid Posted at: 2016-10-19T09:38:34.821Z Reads: 124

```
Nobody mentions the underspecced battery? At 12S2P the max "healthy" current draw is way too low for esk8s - especially for dual hubs!
```

---
## \#19 Posted by: XIII Posted at: 2016-10-19T10:42:57.664Z Reads: 123

```
Are you doing this yourself? You mind making a tutorial of how you did it ? I know it's from delta config to wye. 
But what is the best way to do this?
```

---
## \#20 Posted by: Pantologist Posted at: 2016-10-19T11:24:46.439Z Reads: 115

```
I wonder how mellow and inboard are using 12S1P packs. Not sure about Mellow but it seems to be that spec.
```

---
## \#21 Posted by: Lukas Posted at: 2016-10-19T11:33:00.688Z Reads: 114

```
LiFePo 26650 cells can draw about 60 Amps continious.
```

---
## \#22 Posted by: Pantologist Posted at: 2016-10-19T11:35:38.565Z Reads: 112

```
Yea, are you referring to one of the companies I mentioned?
```

---
## \#23 Posted by: Maxid Posted at: 2016-10-19T11:36:48.890Z Reads: 112

```
like @Lukas said: They use a different type of cell. LG or Samsung Liion cells are typically rated at 20A per cell - an A123 Lifepo however is rated at 70A per cell.
https://eu.nkon.nl/a123-systems-anr26650m1b-a-grade-3-3v-a-grade.html
```

---
## \#24 Posted by: Pantologist Posted at: 2016-10-19T11:38:15.171Z Reads: 110

```
Inboard is definitely using a 12S1P Li-Ion 18650 pack. Their battery manufacturer showed them at an event.
```

---
## \#25 Posted by: Maxid Posted at: 2016-10-19T11:41:28.637Z Reads: 107

```
Which is why they are totally underspecced. Don't get me wrong: It will work - just not for long as your cells are taxed heavily that way.
```

---
## \#26 Posted by: Pantologist Posted at: 2016-10-19T11:45:37.694Z Reads: 110

```
Yeah... Maybe @Mellow uses a different pack?

I currently have a A123 pack right now. Should I just keep using that for dual hubs?
```

---
## \#27 Posted by: Maxid Posted at: 2016-10-19T11:48:32.722Z Reads: 107

```
You could either use the A123 or go with some Sony Liion cells that are rated at 30A per cell - in a 2P configuration that would give you the equivalent of a 3P Samsung pack. Voltage on the A123 is different to Liion however as Lifepo has a nominal voltage of 3.3V instead of 3.6V.
```

---
## \#28 Posted by: Pantologist Posted at: 2016-10-19T12:10:10.866Z Reads: 108

```
Yeah 12S LiFePO4 is like using a 10S lithium pack.
```

---
## \#29 Posted by: Hummie Posted at: 2016-10-19T14:18:06.968Z Reads: 106

```
I think people changing from 2.0 to 2.5 are not reterminating or even rewinding and instead putting on a new stator.  
I'm pretty sure u can reterminate the motor without opening it up though if the motor leads are an extension of the multistrand magnet wire by going strand by strand and finding circuits with a battery and led and then making a wye bundle outside and soldering it all together.   I've never done it but think it's doable.  A lot easier than a rewind.
```

---
## \#30 Posted by: Mrmoonlight Posted at: 2016-10-19T14:35:02.940Z Reads: 103

```
I have a Carvon single V2 and V2.5. The V2.5 is awesome. Worth every penny and built very well. Even if you had hills, it wouldn't be a problem.
```

---
## \#31 Posted by: Pantologist Posted at: 2016-10-19T14:37:38.798Z Reads: 103

```
If you don't mind me asking, how much do you weigh?

Also what voltage are you running at? 12S?
```

---
## \#32 Posted by: RunPlayBack Posted at: 2016-10-19T14:47:55.419Z Reads: 100

```
Sorry I worded that wrong lol. By converting I meant I sent them over to @LEVer to work his magic. :)
```

---
## \#33 Posted by: Mrmoonlight Posted at: 2016-10-19T16:27:34.563Z Reads: 98

```
I weigh 135 and I'm running a 10S. The SpaceCell3 to be exact. You should be fine at 170. My kid weighs around 30 and we stand on the board together with backpacks. It goes up hills without issue.
```

---
## \#34 Posted by: Pantologist Posted at: 2016-10-20T00:48:12.585Z Reads: 97

```
@Hummie

 So you are only selling the all steel version for $400? You mentioned that everything is steel now.
```

---
## \#35 Posted by: Hummie Posted at: 2016-10-20T03:09:15.500Z Reads: 92

```
DNothin like those rediculous prices.  I don't think I ever sold a set for that.  

If u search for the" best hub motors cheaper than anywhere  " thread It says what's being made now. Not 80x56 wheel but 80x101 coming!  Crazy rollers. Bigger bearings and on and on. 150% the power of the two smaller was selling before in the one.  Run one solo

300 with extra tires and a pair of Paris v2 trucks
```

---
## \#36 Posted by: Pantologist Posted at: 2016-10-20T16:36:06.682Z Reads: 89

```
Oh okay

Wouldn't that make turning weird with having one super wide wheel and one regular wheel in the back?
```

---
## \#37 Posted by: Hummie Posted at: 2016-10-20T17:08:29.046Z Reads: 91

```
We will see!  I don't think it will affect things negatively and it'll more so just be getting used to it. 
It'll stick out 45mm on one side. 
 I'll do front wheel drive.  
If it ends up weird I could put it further along the axle and under the board by lathing down the hanger more and adding more threading on the axle but then won't fit on a drop thru maybe so rather do it this way.
```

---
## \#38 Posted by: Mellow Posted at: 2016-10-21T18:36:15.532Z Reads: 82

```
Thanks for tagging us, Jake. Our partner Battery Kutter has 20 years of experience in custom packs. The last (looking to be our final) iteration we've designed together uses Samsung INR 18650-20R cells in 7s2p.
```

---
