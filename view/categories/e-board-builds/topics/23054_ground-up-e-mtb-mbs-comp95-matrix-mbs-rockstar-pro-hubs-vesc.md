# Ground up e-mtb &#124; MBS Comp95(?) &#124; Matrix &#124; MBS Rockstar Pro Hubs &#124; VESC (?)

### Replies: 33 Views: 4806

## \#1 Posted by: dmegret Posted at: 2017-05-14T19:27:28.655Z Reads: 400

```
Hey there esk8,
 
I've been stalking the forums for a few weeks now and am finally starting my own build. 
I have lots of questions, and can't seem to DM anyone yet, so I figured starting my own build thread would be a good way to reach all you experts out there, as well as have the answers documented for others. I look forward to meeting y'all. 

I happened to have a MBS comp 95 board I used for kite boarding on land (gotten ages ago on craigslist), and I will try to re-purpose its hardware for this build. 
<img src="/uploads/db1493/original/3X/e/c/ecc6ea135e3635a1a9b7eb11fee25ed0a791cb40.jpg" width="690" height="388">

One issue though, the deck is warped. There is about a 1/2" diagonal warp (ie if you put three corners on the ground, the 4th will be 1/2" up). This isn't much of an issue for low speed, but I am wary of riding this at my target 30 mph max speed (~48 kph). Which leads me to:
**Question 1)** How dangerous is it to make a 30 mph e-board on a warped deck? Is it dangerous?
**Question 1.5)** Am I just being cheap? (given the relative cost of the rest of the project)

I also have MBS Matrix II trucks 
<img src="/uploads/db1493/original/3X/0/0/0017d8026f2ca53123303063cbcf6f291bfc4897.jpg" width="690" height="388">

So  I happen to have a MBS board to work with, which leads me to:
**Question 2)** What are the relative differences of electrifying a MBS board vs TRAMPA. I see @Trampa (is this the official brand account?) has an active presence on these forums, and the Trampa web store seems to have a lot of "off-the-shelf" support for e-MTB. Given that I have access to CNC mills + a slew of 3D printers and am not afraid of some CAD, Is one easier/cheaper to convert?

So while I'm figuring out what chassis to base this project around, I am also deep in though about the ESC. My background is in EE (Electrical Engineering), and I am pretty intrigued by the [open source ESC](http://hackaday.com/2015/10/01/open-source-esc-developed-for-longboard-commute/) made by Benjamin Vedder, I believe you guys call em VESC's (but maybe not soon given a [thread I saw this morning](https://www.electric-skateboard.builders/t/news-to-the-name-vesc/23017/30)).  
**Question 3)** Has anyone forked Ben Vedder's base design into a dual motor solution?

If I've broken any rules please let me know. I tried to follow all the guidelines I've seen. 
My final question for this first post which exemplifies my newb status:
**Question 4**) How do I earn the ability to DM /respond to Esk8 Market posts? (I want to buy some of @Kaly's motors)?
```

---
## \#2 Posted by: SirDiff Posted at: 2017-05-14T19:38:41.832Z Reads: 362

```
I've seen some builds with matrix trucks, and there should be some motor mounts available without having to modify much. 
I wouldn't use a warped deck for this, you don't wanna regret after your board splits in half at 45 km/h
The vesc right now isn't well suited for emtbs, it doesn't support more than 50/60A, and some builds here have spikes of 120 or more. If you have the money, VESC 6 shouldn't be too far away, and it should be able to deliver the needed power (but it isn't available yet and the only vendor for the first period is trampa itself, whose account, by the way, is that one you tagged ;)  ) 
People usually use beast RC escs that are powerful but not really customizable like the vesc is, brakes could be a bit noisy. 
Before you can post in the market or message people I think you have to have a certain read time and a number of comments, I can't remember how many. Keep studying the forum and It will be unlocked pretty soon 
Also, you should know from the start that these things take a lot of time to make (I started my build 8 months ago, received the last parts yesterday, but I'm an extreme case) 
Good luck! :smiley:
```

---
## \#3 Posted by: dmegret Posted at: 2017-05-14T19:59:48.523Z Reads: 351

```
Hi @SirDiff! nice to meet you :) 

[quote="SirDiff, post:2, topic:23054"]
I wouldn't use a warped deck for this, you don't wanna regret after your board splits in half at 45 km/h
[/quote]

Unfortunately, I was expecting this answer :( maybe I can develop with this deck for now, and upgrade after all the things work :p  

[quote="SirDiff, post:2, topic:23054"]
I've seen some builds with matrix trucks, and there should be some motor mounts available without having to modify much.
[/quote]

I have seen some documented builds on here for Matrix trucks, but haven't found a store front that sells em yet. One big hurdle I see is getting the profile of the truck correctly (some people here seem to have very specific custom clamp shapes). 

[quote="SirDiff, post:2, topic:23054"]
The vesc right now isn't well suited for emtbs
[/quote]

Good to know that the VESC only goes up to 50/60A. Am I correct in thinking this is only a limitation of the power electronics side of the VESC? Would laying out a new board w/ better FET's but still re-purposing Vedder's stack do the trick (That is what I am hoping to do).

[quote="SirDiff, post:2, topic:23054"]
these things take a lot of time to make
[/quote]

:grin: I was thinking I'd have a crudely working thing by winter, and an actual fun toy by next year. Hopefully estimate isn't too far off :grimacing: .
```

---
## \#4 Posted by: SirDiff Posted at: 2017-05-14T20:20:43.864Z Reads: 321

```
About the mounts, you can check this 
https://www.electric-skateboard.builders/t/motormounts-for-trampa-mtb-e-toxx-dual-direct-drive/18992/30

Or this as a more conventional one :) 
https://www.electric-skateboard.builders/t/unikboards-group-buy-trampa-mounts-angled-risers-mbs-matrix-pro-mounts/19849/6

Some people are trying improved versions of VESC, like enertion's vesc-X or @chaka's direct fet version with heatsinks 
They work better but the 4.12 version is still limited, if you get the best components you may be able to use it in a dual drive configuration if geared low enough not to stress too much 
There are some other escs that work well at something like 120A, but I'm no expert and I would let others talk about this, maybe @Nowind could help you, try to look up the mountain board section and check what escs they use there :smiley:
```

---
## \#5 Posted by: SirDiff Posted at: 2017-05-14T20:59:36.451Z Reads: 282

```
Oh I forgot to say, if you really like the deck and have access and experience with carbon fiber, you may think about keeping it and reinforcing it with carbon fiber. It may get a little stiffer, but it will hold much better. If you're completely new to this, you may be better off buying a new deck
```

---
## \#6 Posted by: dmegret Posted at: 2017-05-14T21:52:08.371Z Reads: 254

```
Great links! Those hadn't made it into my search results, I'll check em out :)
I am pretty new to this (skateboard hardware), so I'll probably get another deck in the long run. 

I didn't realize how many "brands" I associated w/ e-skateboards are actually individual contributors :D  (I like it).
```

---
## \#7 Posted by: anorak234 Posted at: 2017-05-14T21:54:13.933Z Reads: 246

```
Idk what your budget is, but if you want a good MTB deck, @trampa has a good reputation with the use of CF. Also I've ridden a slightly warped deck a motor on it temporarily and it wasn't stable at more than 15mph
```

---
## \#8 Posted by: dmegret Posted at: 2017-05-14T22:09:45.770Z Reads: 254

```
@anorak234  Yea, Trampa has definitely been on my radar from my google research. what is CF (Carbon Fiber)? 
Do MBS trucks natively fit Trampa decks? Or would you have to drill new mounting holes? 

Lets say I have a ROI limited budget. In that I COULD spend more, but am trying to spend my money wisely. 
[quote="anorak234, post:7, topic:23054"]
Also I've ridden a slightly warped deck a motor on it temporarily and it wasn't stable at more than 15mph
[/quote]

Very helpful to hear others first hand experience, will definitely be planning on getting a new deck then. 
I had tried [this technique](https://www.youtube.com/watch?v=zwbX-PWuyLo), but it didn't work :(
```

---
## \#9 Posted by: anorak234 Posted at: 2017-05-14T22:34:44.840Z Reads: 231

```
Yes, CF is carbon fiber. I don't know if MBS trucks fit Trampa decks, but I'd guess not seeing as Trampa likes to make his stuff unique. It's not hard to drill new mounting holes if it doesn't work right away. Also, I always hate to be the bearer of bad news but with these kinds of things (especially mountain boards) if you want something that you can really enjoy riding its probably going to put you well over budget. Thats what happens 99% of the time on this forum
```

---
## \#10 Posted by: Okami Posted at: 2017-05-15T00:31:17.131Z Reads: 236

```
@dmegret There is dual vesc design, if you mean 2 vesc ''modules'' on one pcb..

Check what @Duffman has done

I wouldnt agree that you cannot use vesc for mountainboard, especially in dual motor config @SirDiff

@SirDiff I dont know do you have mountainboard but how much power do you really consume usually?

I think burst current for vesc should be way over than 50A as it is for the rest of the escs

You can always add heatsinks or even active cooling but I doubt someone is going to go 60kph all the time, to use 4kw of power non stop.

I barely see more than 800w (single motor) for me and that is even with moderate acceleration (ok no vesc but I want to believe my watt meter is not 25% off)

--

@dmegret if you want to have high tech board, look into what @Nowind (e-toxx) has done, though im not sure would you need to go after high performance setup in the first build already before u have figured out what you like and what u would like to see and get.

If someone can overstate the power demand for what I said about mountainboards.. im listening..

Firstly someone should decide where he wants to ride and how roughly then I think someone can choose the motors etc.

.. I do agree though that vesc might be more prone to failures but it does not mean it is ''completely useless'' for mountainboard build.
```

---
## \#11 Posted by: DilatedPupils Posted at: 2017-05-15T01:58:17.878Z Reads: 216

```
I use VESCs on my Trampa. I've been running them for over a year and I haven't broken them yet. But of course it depends on how you ride. A few members here broke a couple vescs or so. And a few just didn't like how smooth it is. If you're not gonna be doing crazy stuff, then I would recommend the vesc.
Was also searching for matrix 2 mounts for me 2nd emtb and so far only @Idea is the only one making them and only with 3d printed rings. 
Depending on the drivetrain you want, you have a few options. Search the forums and you'll find a lot of stuff about all of em. 
Depending on your skill and dedication, since you have access to 3d printer and cnc you can probably make your own mounts and stuff. It will take a lot of time and probably would cost more than if you buy it after trial and errors. But if it's something you enjoy and good at it then it'll be better.
And lastly, unless you're very experienced. I wouldn't suggest aiming for 30mph top speed. But if you do, please make sure you wear a helmet, knee pads and elbow pads at the least. 
Welcome to the addicting world of DIY emtb. Good luck and have fun.
```

---
## \#12 Posted by: SirDiff Posted at: 2017-05-15T05:40:00.178Z Reads: 215

```
[quote="Okami, post:10, topic:23054"]
I wouldnt agree that you cannot use vesc for mountainboard, especially in dual motor config @SirDiff
[/quote]

I didn't say you can't, I said it's limited in terms of power delivery. I don't own one a mountainboard (in fact I left the esc question open to other opinions :) ) but I've seen some people burning even 120A continuous escs. Yeah, I read somewhere that vesc can have spikes of 200 amps. What I meant is, vesc is way more fragile than other escs. Not that it's worse, but you have to keep an eye on it
```

---
## \#13 Posted by: Okami Posted at: 2017-05-15T11:54:14.547Z Reads: 219

```
Well, if im not mistaken check @Duffman ''monster'' build, he still uses vescs there, they are ''reinforced'' with extra cooling and extra cap banks.. (though I think he made them himself, so if you order yours from china and something fails it might be just of manufacturing)

 Well, if you are referencing to @Nowind where one of his roxxys started to burn.. then yeh, it can always happen.. people also burn FVT 120 on longboard builds either of not decent enough cooling or some other problems.

Im not even sure can these car esc's output 120A constant, as with batteries and other hobby grade stuff it might just be a rating.. I havent seen anyone actually measuring constant ~100A on these.. i would say for about 50A they are also good maybe they have higher peaks / bursts than vesc and they are not as smooth yes, so for ''raw power'' they will always be better.

---

@dmegret ok, if you do plan to go really fast you should look into what trucks are best for that. I would actually suggest to contact @Nowind or maybe @tueboard if you plan to do high speed riding..

Then yes, you might as well need 6kw of power, which might require.. 83Amps per controller, per motor or so and then you might better go with esc (FVT 12s) @Idea has tested more and more.

Though, I think only 'Alien drive system'' motors are rated for 3kw output and they usually come with 10mm axle which might be a bit of a pain, if you dont have the right pulley.

Turnigy's usually are about 2.3- 2.7kw rated but I havent personally tested them to the max rating.. So far I have only consumed about 1500w from the constant when I went up a very steep hill and at 42A the 6374 192kv already got quite a bit hot.

--

There are Scorpion and Diamond motors @Nowind uses.. but they are from 'higher shelves'' :D so it depends on how much you want to spend and I think scorpion's still produced some annoying sound, if im not mistaken (yeh some motors, like alien's in combination with certain escs will produce a bit annoying sound)
```

---
## \#14 Posted by: Okami Posted at: 2017-05-15T23:22:22.766Z Reads: 221

```
I tested today uphill 'performance''. Couldnt get more than 1000w of power draw when going up hill, peak was about 1300W.

Though, the hill was a monster. I cannot cycle up this hill with my bicycle and even with foot it is a bit hard.

And this is just with one motor.. 

--

I know it does not give much info but I would like to pinpoint that yes - early on it should be decided whenever someone plans to 'conquer' hills or not.. whenever these will be dirt tracks or city landscapes.

For very good road I couldnt get more than 600w at about max speed I got. Though Im going more like 20mph / 30kph now, so I would estimate that for 30mph / 55kph about 1500 - 2000W of power would be needed at least. If not more.

<img src="/uploads/db1493/original/3X/d/2/d2e52c22899e633e2816c9725fb60415260e8ba6.jpg" width="690" height="387"><img src="/uploads/db1493/original/3X/1/7/177c59f5cb344ec01c606a1914f754748af413b8.jpg" width="690" height="387">
```

---
## \#15 Posted by: dmegret Posted at: 2017-05-18T02:51:39.875Z Reads: 211

```
[quote="DilatedPupils, post:11, topic:23054"]
Welcome to the addicting world of DIY emtb. Good luck and have fun.
[/quote]

Thanks! Excited to be here. 

@Okami, I am definitely still figuring out what I want (and will probably change my mind a few times! :p ).

@DilatedPupils, I've used this board with a propulsion kite, and have reached some pretty fast speeds (I think), but then again, that may feel a lot more stable because you can always lean against the pull of the kite. I do of course plan on full PPE when playing with this (still theoretical) board. 

Thanks for all the comments and insight! :) I've realized the first step is to figure out what this project means to me. After some reflection, I concluded that my goal is not an uber e-mtb, but actually an engaging side project that I can use to grow my understanding of mechanical systems, and learn more about BLDC motor control. I do want to zip around and get my adrenaline rush, but that is not the primary motivation for this build.  

I want to fully understand the trade-offs at every part of the design process. So.... this will probably be a long journey :D . Here's the last couple days of progress:

I'm starting by trying to wrap my head around the super-intertwined, multi-variable optimization that everyone here deals with. I _think_ the right place to start is the drive train and gear reduction, and then the rest of the electrical system. From what I've read, seems like the right place to start, If people have more insight (this is my first build!) into the first thing to nail down, please let me know :slight_smile:. 

That said, from looking at a variety of products, and a lot of builds on here, I have decided to use a belt drive (this may change as my understanding grows). My current understanding is that there are certain limitations on gear reduction and efficient power transfer, so I want to make sure I choose the right Battery + ESC + Motors that can give me my desired outcome (for a given drive train). Hence am trying to understand the constraints of a belt drive system first. 

I'd be curious to know what types of belts people run, but my first pass led me to the gut choice of a 5mm pitch T5 belt at 25mm width (no real science behind this yet, more of a jumping off point).

With one variable fixed, I started looking at what constraints this type of belt has. 
I'm still cobbling together knowledge, but here are some resources I found helpful:
- [Good overview of various belt types](http://www.plantengineering.com/single-article/basics-of-belt-drives/981c1be10d400323db10aa592e4cc7b3.html) (why don't people run V-belts?)
- [Good Intro to belt theory (mathy)](http://www.gatesmectrol.com/mectrol/downloads/download_common.cfm?file=Belt_Theory06sm.pdf&folder=brochure)
- [Vendor recommendations for tooth count + idler diameter (for various belts)](http://brecoflex.com/wp-content/uploads/2016/07/tensioner_idlers.pdf) 
(maybe take that last one with a grain of salt, another part of their site (looks more sloppy and w/ typos, [contradicts this...](http://www.brecoflex.com/products/pulleys/design-guidelines/minimum-pulley-diameter/#1480604033821-739e454d-fefe) ) at least for T5. 

Taking that into account, and my decision to go with an idler/tensioner, I think the largest gear reduction I can get would be 4:1 (for a T5 belt, since the MBS hub can fit at most a 60 tooth pulley, and the smallest "recommended" drive gear is 15 teeth).  I think I want the highest reduction possible, so I will do the same for other easy to get belts later. 

I think it should look something like this (a fairly common design from what I've seen, not reinventing the wheel or anything).
<img src="/uploads/db1493/original/3X/6/4/64ac5a82de592c0f601682c81c5cf62fb90d9ec2.png" width="659" height="499">

So I opened up McMaster, downloaded the STEP files (you wouldn't download an electric skate board would you? :P ) for the parts I was interested in, and modified them w/ Onshape (This was my first time using Onshape, but I have used other CAD programs in the past). These are just quick mock-ups (with dimensions hastily measured w/ cheap harbor freight calipers, on the wrong hubs) to get a feel for the size and fit. I printed them out and this is what I got (I work at a place I can print for free :D )

<img src="/uploads/db1493/original/3X/9/2/9255b82bb1c16e6e267107a0c8543183f262421b.jpg" width="690" height="388"><img src="/uploads/db1493/original/3X/4/7/4731d6658130453d31fbd3caf9d53cde6bb72669.jpg" width="690" height="388">

<img src="/uploads/db1493/original/3X/0/b/0b8e48bb27a01a179e14113b5022a761719d4e2d.jpg" width="690" height="388">>
<img src="/uploads/db1493/original/3X/3/8/3800c29add2ff435765fc73ff1669c131be6d4a1.jpg" width="690" height="388">
I also got some aluminium hubs. Should hold higher pressure + much less sketchy to mount to than the twisting hubs I had. 

After this exercise, I am re-considering my lean towards a 25mm width belt... It seems quite bulky, and would add a lot of weight to the wheels (more pulley). I also got a chance to look at a colleagues Boosted board, and it seems they use 15mm belts for 1KW motors, I guess I gotta learn more :slight_smile:.
```

---
## \#16 Posted by: DilatedPupils Posted at: 2017-05-18T05:04:54.793Z Reads: 188

```
Again, depending on what your trying to do with your emtb. 25mm for better power transfer. But other than that, 15mm should be more than adequate. Aside from the bulk 25mm is gonna have more drag as well. 
Why not go for direct drive? It seems like it's the best option right now , but it's just a little pricey.
```

---
## \#17 Posted by: Okami Posted at: 2017-05-18T12:16:28.079Z Reads: 189

```
That u found these T profile belts /pulleys is.nice.

I think @Duffman also used one of these at some point for higher power transfer.

I would actually recommend 20mm belts if u can find them.

25mm for me looks like a bit too much while 15mm sometimes could.maybe.be.more.wide. (havent.tried.25mm though )

--

Also tension plays a bit part in the equation and I kind of did the same mistake I think that I relied on calculator very much when I should have just got smaller belt and installed idler in the first place.
```

---
## \#18 Posted by: dmegret Posted at: 2017-05-18T23:37:00.513Z Reads: 192

```
I took the time to measure a MBS Rockstar Pro Hub to the best of my abilities. 
This is what I got:
<img src="/uploads/db1493/original/3X/e/f/ef5201bdd800005e87bec6a170a9c67a065f0c70.png" width="690" height="488">
Dimensions are correct to the best of my abilities, drawing is approximately to scale. 
I'm posting this here because I couldn't find a reference for this in all my previous searching. I will update the thread with a proper DXF once I get this CAD'd up :slight_smile: 

side notes: 
- I'm not sure what to expect from parts like these, but they look like a pretty shitty extrusion, that was post machined with a pretty dull tool.. 
- Anodization looks decent, but was scuffed in places when they arrived. 
- The aluminium hub spacers vary in thickness by up to 0.5mm across the circumference!! I'm thinking it might be worth it to remove some material and make the hubs more symmetric. 
[quote="Okami, post:17, topic:23054"]
Also tension plays a bit part in the equation
[/quote]

It sure seems like it will! I'm actually starting to think about a double tensioner design (so that it can pick up slack / maintain tension in both direction of travel)
```

---
## \#19 Posted by: dmegret Posted at: 2017-05-20T01:01:43.460Z Reads: 183

```
I couldn't quite figure our how to measure the matrix trucks, so I tried scanning them :D 

<img src="/uploads/db1493/original/3X/2/0/20cd02eeb455550f29ce689cbb308b6b09c3befe.png" width="475" height="500">

[link to raw-ish scan .stl](https://drive.google.com/open?id=0B0ISU0jNXGacQ09WOUhKSmNScGc) (on google drive, couldn't upload, how do people normally share 3D files on here?)
It had to be sprayed with a bit of TiO2 since it was reflective (so it may be ~5-20um thicker).
I will hopefully use this to design a nice 3d-printable motor mount (I know there are some pulley designs out there, which are definitely inspiration, but I'd like something custom and personal :) )

edit: updated to correct name for truck
```

---
## \#20 Posted by: Okami Posted at: 2017-05-20T02:00:46.715Z Reads: 181

```
I think ppl usually share theirs on Thingiverse or similar site, where you can get nice link and little thumbnail straight ahead..

woah.. nice work.. didnt know someone can do that at home? 
What kind of ''system'' / scanner you have to be able to do this?

Yeh making custom trucks for mbs with brake holes is probably a pain.. :D I think if you searched a forum u would find 1-2 who has attempted to do this and has got some results.. some just use the hole for mounting a strong screw and thats how they keep it place.. just not sure do they have any 3d models or these were just maybe diy made mounts by hand..

Worth checking to what @Idea has done, maybe he had a variety of these trucks, too now :slight_smile:
Ok gotta go now, it's pretty late here, see you some other time ;) @dmegret
```

---
## \#21 Posted by: dmegret Posted at: 2017-05-20T15:20:26.369Z Reads: 182

```
Yea, I thought about places like Thingiverse and Pinshape, but this scan data isn't printable, and those are 3d print file repositories. 

I actually scanned this at work, with a [NextEngine](http://www.nextengine.com/) 3d scanner (they are about $3k).
Process looked like this:
<img src="/uploads/db1493/original/3X/b/7/b7110078ceb32e83e309725629e2ed93a495fb15.png" width="690" height="408">

I then trimmed extra points in the NextEngine software, and exported as a non water-tight .stl
```

---
## \#22 Posted by: Okami Posted at: 2017-05-20T15:22:06.027Z Reads: 178

```
Ok I see.

@dmegret cool tech! What your work is using it for?

Mh yeh I saw stl format and thought u might as well use it too..
```

---
## \#23 Posted by: dmegret Posted at: 2017-05-20T15:25:44.440Z Reads: 176

```
@Okami I work for Formlabs, we make Desktop SLA 3d printers, so generally have a lot of 3d input/output related tech laying around the office.
```

---
## \#24 Posted by: Okami Posted at: 2017-05-20T15:26:55.617Z Reads: 172

```
Cool. Formlabs seem to be high grade printers. U probably know what you are doing very well hah
```

---
## \#25 Posted by: dmegret Posted at: 2017-05-20T15:30:54.807Z Reads: 173

```
Regarding 3d printers, hopefully :wink:, don't know much about EV's though.
```

---
## \#26 Posted by: Okami Posted at: 2017-05-20T15:40:11.834Z Reads: 178

```
All the info should be out there, somewhere :slight_smile:
More problems is when you need some real life data, like energy consumtion, power needed etc..

There are usually basic guidelines everyone tends to follow but with your skills I think u can and will be crafty enough to make your own way and things to make it work ;)
```

---
## \#27 Posted by: Mobutusan Posted at: 2017-05-20T20:19:33.473Z Reads: 181

```
That is really cool. I was thinking of trying a method to create a 3d model that I'd found on YouTube where you take a bunch of photos from different angles and the program stitches them together to create a 3D model.

https://youtu.be/NsBg-m2hrIM

And just a side note, mostly in case you ever deal with vendors for motor mount parts in the future, but I believe the trucks you have are generally referred to as "Matrix 1" or just "Matrix" trucks and not "Matrix 2". Although the photo you posted does seem to create some confusion since it appears to say "Matrix II" on them. Maybe the "II" after "Matrix" are not numerals, but just cosmetic lines? 

This photo shows the latest versions of MBS Matrix trucks in this order:
-Matrix I Pro
-Matrix I
-Matrix II

<img src="/uploads/db1493/original/3X/8/1/81ab648a75bd204691a386ca49d90daebc857fa3.jpg" width="350" height="350">
```

---
## \#28 Posted by: dmegret Posted at: 2017-05-20T21:36:24.502Z Reads: 174

```
I've used 123D catch before, and it works pretty decently when viewing the model with the overlaid textures, but the actual 3d model is often pretty wonky (kinda like low-poly video games). Funny coincidence I've actually worked with Ehsan Noursalehi in the past (small world I guess). 

I didn't realize about the naming scheme (just used what I thought was the name on the truck), I'll update my thread name + post :)
Although mine don't seem to match any of those 3 (looks closest to the Matrix I, but mine don't have the holes cut out)
```

---
## \#29 Posted by: flywithgriff Posted at: 2017-07-27T21:59:36.316Z Reads: 161

```
@dmegret  I am building a setup based on MBS Rockstar II Hubs. What was your final outcome for pulleys for them?
```

---
## \#30 Posted by: dmegret Posted at: 2017-07-28T21:05:41.815Z Reads: 164

```

@flywithgriff I have not made too much progress on this project. 
Work has been all consuming. 
I have linked to the file for the pulley I ended up making, but I have not been able to put it to use/test it yet. 
It does fit on the hub, and feels quite secure though. 

<img src="/uploads/db1493/original/3X/a/7/a7268686b894db27de9ff9fe18067ee10ac137e2.jpg" width="533" height="500">

link to stl: https://drive.google.com/open?id=0B0ISU0jNXGacN1ZYcWxZaERoZlU
```

---
## \#31 Posted by: allelectric Posted at: 2018-04-05T19:40:45.035Z Reads: 122

```
Hi there.
This is nearly a year later but I would be interested to see how you got on with your build as I am looking to do the same myself. In the end which esc/vesc did you decide to go with?
Thanks
```

---
## \#32 Posted by: Snake Posted at: 2018-08-06T11:04:40.644Z Reads: 89

```
Hi demegret,

would it be possible, to get the CAD-Data of the MBS-Pulley in your post (.step or.iges).
I want to change the dimensions for a 15mm belt and it´s hard to work with the .stl...

regards, Klaus
```

---
## \#33 Posted by: Toby-Aus Posted at: 2019-04-11T14:28:33.213Z Reads: 47

```
can you do it with the mbs ATS 12 trucks :) they are tapered arrrr
```

---
