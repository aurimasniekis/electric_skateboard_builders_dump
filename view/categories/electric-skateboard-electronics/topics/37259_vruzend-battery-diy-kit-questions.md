# VRUZEND battery diy kit questions!

### Replies: 52 Views: 6019

## \#1 Posted by: KeivanM Posted at: 2017-11-03T19:10:51.842Z Reads: 467

```
Hi everyone I am making my own lithium ion battery pack for my build and I decided to use  the vruzend battery diy kit, [Here](http://vruzend.com/product/vruzend_basic_kit/), and the concern i have is the clearance issue on the bottom of my board. Let me insert some pictures so you can see what my concern  is. My question here is, can I allign the batteries like this with the DIY kit? <img src="/uploads/db1493/original/3X/5/9/5934a80cd43d96fe634963605d15b2a45a34d59f.jpg" width="375" height="500">

OR does it have to be like this? 
<img src="/uploads/db1493/original/3X/e/a/eab5701c39f5ac91df7ab2a2c080a6c0bd0f0618.jpg" width="375" height="500">


The second picture has the a 12S3P config and has them standing vertical, this makes the pack very thick. Ive seen this used for e-bikes since you can get a large amount of Ah with these packs. I want to make my pack a 12s3p or 12s4p, but unlike the second picture, I want mine to be thin like i drew in the first picture inserted.
Can this be done? And if so how? any feedback will be appreciated.
```

---
## \#2 Posted by: bigben Posted at: 2017-11-03T19:39:45.876Z Reads: 424

```
Do you have the cells and the vruzend kit? You could lay them out and measure up what space you might need?
```

---
## \#3 Posted by: KeivanM Posted at: 2017-11-03T19:51:58.895Z Reads: 423

```
Not yet, I want to sort this out for sure before I buy everything
```

---
## \#4 Posted by: KeivanM Posted at: 2017-11-03T19:52:44.298Z Reads: 424

```
They have the dimensions on their website though, I’m just not sure if I can lay them out like in the first picture or if I HAVE TO make it look like the second picture
```

---
## \#5 Posted by: ShutterShock Posted at: 2017-11-03T22:58:08.574Z Reads: 401

```
Oh yeah it definitely looks like you can do it the way you want.  The first picture on their site has two packs in it, both 1S4P.  All you gotta do is lay them down and wire 12 of them together in series. :slight_smile:
```

---
## \#6 Posted by: KeivanM Posted at: 2017-11-04T00:25:16.136Z Reads: 379

```
So how would i do that? can i use the little brackets of metal they include or would i have to solder?
```

---
## \#7 Posted by: thisguyhere Posted at: 2017-11-04T00:31:35.960Z Reads: 379

```
last time I saw this, we determined it's not a viable option because the caps are rated at like 6amp continuous so you'll overheat them unless u run like a 5p and above pack, or have batt current limit set to something unreasonably low
```

---
## \#8 Posted by: KeivanM Posted at: 2017-11-04T02:12:55.598Z Reads: 369

```
ohhhh my god, is there another solution for a solderless pack?
```

---
## \#9 Posted by: thisguyhere Posted at: 2017-11-04T02:17:28.429Z Reads: 369

```
someone posted this the other day but...didn't really go through the 45min video:

https://www.electric-skateboard.builders/t/n-e-s-e-no-solder-module-battery-packs/36847
```

---
## \#10 Posted by: ShutterShock Posted at: 2017-11-04T04:45:30.877Z Reads: 364

```
Oh yeah I do recall that now. They seemed a bit small to me in the pictures
```

---
## \#11 Posted by: banjaxxed Posted at: 2017-11-04T12:47:14.023Z Reads: 355

```
There are better choices for weld-free esk8 li-ion packs, in particular the nese, see the posts by @agniusm for nese related info or 18650.lt

I say this as someone who has belligerently almost finished building a veruzend 12s7p case pack for a MTB build, but I have modified it to only use the caps, everything else I ripped out and replaced with low resistance metal, in reflection I would not bother going this route
```

---
## \#12 Posted by: banjaxxed Posted at: 2017-11-04T12:54:16.245Z Reads: 343

```
Btw you could layout a veruzend pack like your first or second picture
```

---
## \#13 Posted by: agniusm Posted at: 2017-11-04T19:00:13.303Z Reads: 335

```
Here are some sizes. Its hard  grasp when there is so much info
Vruzend 6P: 0.285l, 366g
NESE 6P: 0.200l, 364g
Energus 6P: 0.174l, 322g (Assembled modules with cells, spotwelded)
If compared to NESE to Vruzend:
3P NESE - 22x74x68.1mm, Vruzend - 22x88x66mm (0.110L vs. 0.127L) L for liters
4P NESE - 22x74x86.4mm, Vruzend - 22x88x88mm (0.140L vs. 0.170L)
5P NESE - 22x74x104.7mm, Vruzend - 22x88x110mm (0.170L vs. 0.212L)
6P NESE - 22x74x123mm, Vruzend - 22x88x132mm (0.200L vs. 0.255L)
BTW recommended current per single cell on Vruzend is 3.5A if i'm not mistaken
```

---
## \#14 Posted by: Wilsonliang777 Posted at: 2018-02-16T07:32:00.676Z Reads: 278

```
Did you finish the battery what this kit.   I am interested in trying the kit too.
```

---
## \#15 Posted by: KeivanM Posted at: 2018-02-16T15:05:28.287Z Reads: 268

```
No, I am gonna spot weld!
```

---
## \#16 Posted by: vagosofron Posted at: 2018-02-26T01:02:51.605Z Reads: 268

```
I'm interested also, but the low current limit on the tabs is a deal braker. What if we can change the metal tabs with another type of contactor?
```

---
## \#17 Posted by: MicahT Posted at: 2018-03-17T07:13:41.420Z Reads: 246

```
Hey everyone, Micah here from Vruzend. My latest tests on the V2 vruzend kit are showing caps handling at least 20 A per cell. Actually tested up to 24A so far with Sony VTC4 cells. We'll be releasing more info and final specs for the upgraded high current V2 kits in the next 2 weeks or so.
edit: in case anyone hasn't been following, the V2 is the copper based kit, hence the higher current ratings.
```

---
## \#18 Posted by: E1Allen Posted at: 2018-03-17T08:22:31.448Z Reads: 242

```
20A per cell is a huge improvement.  Thanks for continuing development.
```

---
## \#19 Posted by: Dmaxx Posted at: 2018-03-18T03:16:20.137Z Reads: 241

```
Will v2 kits be available on the website soon?
```

---
## \#20 Posted by: MicahT Posted at: 2018-03-18T21:10:00.481Z Reads: 239

```
For North American battery builders, yea. I don't have an exact date yet, but soon. If you are outside of North America, you can already preorder the V2 at https://www.vruzend.com/international-orders and it should be shipping in a few weeks.

I just did a 17A-24A test today on the V2 kit and on spot welds, and filmed the comparison to make a video soon. Basically, there wasn't a difference between the two that was larger than the margin of error in the test, so they are effectively equal performance.
```

---
## \#21 Posted by: XTLA Posted at: 2018-03-21T12:26:32.440Z Reads: 219

```
Hi micah, i already made a pre-order on your copper kit, my question is can the copper plat bended so we could make a flat pack, block type of pack seems not suitable for e-skate coz we put it under our deck.
```

---
## \#22 Posted by: MicahT Posted at: 2018-03-21T15:38:16.155Z Reads: 208

```
Hey! Yes, the copper busbars are soft enough to bend, though I'm not sure this is the best method to achieve a flat pack. In my opinion, it would be better to make a "flexible busbar" at that point using a short piece of wire and ring terminals. That way it will be easier to reach in and tighten the nut. Bending the bus bar will make it tricky to close the nuts while reaching the terminals since the bus bars are very short, less than an inch between the holes. 

In [this video](https://www.youtube.com/watch?v=clawhNsORts) (skip to about 12:34 for the wire jumpers) I made flexible connections like I mentioned above for places where I needed to reach but busbars couldn't bend to make the connection. You can do the same thing to connect two 1-cell thick rows laying next to each other to make a flat pack for skateboards.

I will be doing exactly this soon when I make a video of building a pack for an electric skateboard using the Vruzend V2 kit.
```

---
## \#23 Posted by: Mikenopolis Posted at: 2018-03-21T15:43:11.722Z Reads: 197

```
Looking forward to the skateboard pack video! I wonder how this will hold up to the vibration our vechicles produce.
```

---
## \#24 Posted by: banjaxxed Posted at: 2018-03-21T15:44:44.951Z Reads: 194

```
Hey Micah, what material are you making the spring cap terminals(not sure of name) from?

The piece that the bolt goes through on one side which pushes against the battery terminal on the other side(flap)
```

---
## \#25 Posted by: XTLA Posted at: 2018-03-22T07:00:36.245Z Reads: 190

```
Looking forward to see your e-skate flat battery pack video, thanks for sharing. 😉
```

---
## \#26 Posted by: MicahT Posted at: 2018-03-22T07:17:17.294Z Reads: 193

```
Yea vibrations are intense, so using sandwich plates on either side of the caps will be recommended. Basically some flat piece of wood, hard plastic such as a cutting board, metal sheet, etc. Then zip tie or bolt the two plates together. Pretty simple but I'll show it in an upcoming video. This will hold the caps on the cells in extreme vibration situations. Sandwich plates won't be necessary for vibration free environments, but we don't operate in those environments ;-)
```

---
## \#27 Posted by: MicahT Posted at: 2018-03-22T07:18:43.351Z Reads: 187

```
We call those the internal contacts for short, but those and the threaded terminal and nuts will all be copper alloys, probably at least 96% copper. Pure copper would be too soft and wouldn't have enough spring or strength for threads. Then the bus bars will be pure copper. And all of those parts will be nickel coated for superior corrosion resistance.
```

---
## \#28 Posted by: Tuomalar Posted at: 2018-03-22T07:39:10.719Z Reads: 183

```
That what I thought. Zip ties might work very well, but I'm also concerned how those nuts will stay or do I have to add a drop of glue on top of them? Or use guality lock nuts.
```

---
## \#29 Posted by: MicahT Posted at: 2018-03-22T08:15:26.863Z Reads: 181

```
What we've found is that because the plastic in the caps compress a bit under the busbar, it creates a compression force on the nut that actually acts like a locknut, keeping them in place. But some people still add a drop of hot glue just for insurance since it makes them feel good.
```

---
## \#30 Posted by: Tuomalar Posted at: 2018-03-22T08:27:50.772Z Reads: 177

```
How much is V2 going to cost for an european customers?
```

---
## \#31 Posted by: MicahT Posted at: 2018-03-22T08:31:29.997Z Reads: 178

```
To be honest I have no idea yet. In terms of the business side, I'm only involved in the North American affairs. My best guess is it will be somewhere around $0.50 per cap or $1 per cell, including all the hardware and everything. It will be more expensive than the V1.5 because the copper materials are more expensive and the machining processes are more complicated. Should still be less expensive than any other high power solderless/weldless kit out there that I'm aware of though.
```

---
## \#32 Posted by: Tuomalar Posted at: 2018-03-22T08:51:58.805Z Reads: 165

```
Dollar per cell is actually very reasonable price. Ofc it's more expensive imported in EU but still a good price.
```

---
## \#33 Posted by: banjaxxed Posted at: 2018-03-22T09:33:14.612Z Reads: 162

```
Cool it's not my IP or yours, far too generic but a good choice, some wiki, congrats to veruzend for upping their game

"High conductivity beryllium copper alloys contain as much as 0.7% beryllium with some nickel and cobalt. The thermal conductivity of these alloys is greater than aluminium and slightly less than pure copper and are often used as electrical contacts."
```

---
## \#34 Posted by: MicahT Posted at: 2018-03-22T16:44:17.158Z Reads: 161

```
We actually have an EU vendor in Nkon.nl and a UK specific vendor on eBay.co.uk (since I guess UK and EU are two distinct things now...). So that should reduce import costs.
```

---
## \#35 Posted by: E1Allen Posted at: 2018-03-22T17:55:45.883Z Reads: 159

```
Are we using beryllium copper?  Last time I checked that's not a metal I would want to be exposed to like working with my hands then ya know. Eat my sandwich.
```

---
## \#36 Posted by: banjaxxed Posted at: 2018-03-22T22:15:48.866Z Reads: 164

```
I'm guessing silence = yes

Don't worry it's safe outside of manufacturing, it's pretty much the only choice for a mechanical tab
```

---
## \#37 Posted by: Hariboisawesome Posted at: 2018-03-23T08:09:41.881Z Reads: 162

```
I have your V2 kit sitting on my work table currently. Excited to see how it turns out once I finish the educational videos.
```

---
## \#38 Posted by: MicahT Posted at: 2018-03-23T10:16:29.563Z Reads: 163

```
No it’s not beryllium copper. Similar, but no beryllium in our mix.
```

---
## \#39 Posted by: banjaxxed Posted at: 2018-03-23T10:37:50.411Z Reads: 168

```
Pretty good choice price wise 

Beryllium copper is non-magnetic. Its electrical conductivity is about 2-4 times as great as phosphor bronze.
```

---
## \#40 Posted by: XTLA Posted at: 2018-03-29T05:54:58.838Z Reads: 167

```
So i got the vruzend V2 Copper Kit @MicahT, i bought from international orders and it cames from India, the quality looks good, just wondering how i’ll make a flat battery pack with this 😁

![image|632x500](upload://4n2EyPOZpzbLl3EeuOhWSBDvkXE.jpeg)
```

---
## \#41 Posted by: MicahT Posted at: 2018-03-29T06:29:50.205Z Reads: 169

```
Yea I haven't made the video yet but I'm planning something along the lines of this layout. Could also do one cell wide and two deep instead too if the board is too narrow.


![IMG_0239|640x480](upload://ybS8sL9npxPgrWMgbYMHAZvfwDU.JPG)
![IMG_0242|375x500](upload://6kpGNM4I75KEdOjthteUZtWf5IY.JPG)
![IMG_0243|640x480](upload://qzbKmY224YmJnhMPCPrMn4k2Mt0.JPG)
```

---
## \#42 Posted by: XTLA Posted at: 2018-03-29T06:41:12.210Z Reads: 165

```
So what will you use for the series connection between the 2rows.
```

---
## \#43 Posted by: MicahT Posted at: 2018-03-29T12:13:30.035Z Reads: 161

```
Ring terminals on a couple inches of silicone wire, probably 14 or 12 AWG. Basically a flexible busbar.
```

---
## \#44 Posted by: clvnng Posted at: 2018-04-03T22:11:56.180Z Reads: 160

```
whats the total width of batteries lined up like that?
thanks
```

---
## \#45 Posted by: MicahT Posted at: 2018-04-04T05:22:07.773Z Reads: 153

```
Approx 187 mm without any cover. Will be a few more millimeters when I add sandwich plates on either side.
```

---
## \#47 Posted by: Itsmedant Posted at: 2018-06-20T20:09:23.903Z Reads: 117

```
Have you made the video of the esk8 build yet? I'm about to build a battery and this seems like a pretty good way to do it!
```

---
## \#48 Posted by: Benjamin899 Posted at: 2018-06-20T21:15:33.494Z Reads: 113

```
https://www.youtube.com/watch?v=1D90heZ8z4s
They are ok, some people have used them, but they are quite wide so consider that or you do deep and narrow.
N.E.S.E is the superior product but more expensive.
```

---
## \#49 Posted by: Itsmedant Posted at: 2018-06-20T21:29:09.314Z Reads: 109

```
What makes NESE superior? Is it just the fact that its in a full case and smaller profile or does it actually handle more current?
```

---
## \#50 Posted by: Benjamin899 Posted at: 2018-06-20T21:35:13.221Z Reads: 108

```
https://www.youtube.com/watch?v=93JBo87LJiU
A vibration test. 
It is compact and it does handle more amps.
Here is the thread.
I like the v2, they are super cheap. Maybe i will build one someday with those v2.
http://www.electric-skateboard.builders/t/n-e-s-e-no-solder-module-battery-packs/36847
```

---
## \#51 Posted by: Itsmedant Posted at: 2018-06-20T21:39:12.723Z Reads: 104

```
holy crap, I'd say that would hold up in a skateboard!!

Now I just gotta decide if I want to spend the money or just try my hand at spot welding. I just bought a brand new spot welder too....
```

---
## \#52 Posted by: donteatbadfood Posted at: 2019-02-02T21:56:16.722Z Reads: 50

```
hi Micah. I'm interested in your product, but was wondering if it would work for a 10s4p configuration since the amperage would be greater than the listed 20A.

THanks!
```

---
## \#53 Posted by: myreala Posted at: 2019-02-03T00:01:05.626Z Reads: 45

```
I have a 30cell v2 never used kit if someone would want it. 25$ + shipping should be 7$ in US. It should handle 30q cells just fine perfect for a 10s3p
```

---
