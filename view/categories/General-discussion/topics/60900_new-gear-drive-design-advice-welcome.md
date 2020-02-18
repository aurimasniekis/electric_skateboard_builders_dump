# New - gear drive design - advice welcome

### Replies: 82 Views: 1399

## \#1 Posted by: moon Posted at: 2018-07-04T19:22:22.608Z Reads: 348

```
I have been designing a three gear system for a while now, but I have been always stuck on what gear ratio to use, since there are so many conflicted opinions here. 

Here are some pictures of what I have designed a couple weeks back

![image|690x280](upload://6RG1RUZMGiZWwUyETXJ1eBN8kpY.jpg)

Working with @uigiroux

@pixelsilva since you have seen some of this design before, you might have something to say

@MonkeyM since you have a mecheng background
```

---
## \#2 Posted by: uigiroux Posted at: 2018-07-04T19:32:15.977Z Reads: 329

```
Currently thinking of gears being 16-27-38 with ratio of 2.375:1.

The middle idler gear is 11 teeth from both the motor gear and the wheel gear so it should have equal torque from both sides... That's the idea at least.
```

---
## \#3 Posted by: linsus Posted at: 2018-07-04T20:15:43.269Z Reads: 316

```
... any particular reason for three gears?.. two points of friction vs 1 with only 2 gears? :o
```

---
## \#4 Posted by: uigiroux Posted at: 2018-07-04T20:35:04.152Z Reads: 314

```
Yes, specifically for clearance.  It was found out in the fatboy prototype for TB trucks and PU wheels that there wasn't enough clearance from the base plate and king pin when running motor larger than I think it was 6364's.  We want to be able to run any motor, up to 6384 and have no issue with clearance of any kind.  This is really the only way we can do it while keeping the wheel gear small enough that the drives clearance from the ground is able to be a sufficient amount without worrying about the drive case scrapping the ground.
```

---
## \#5 Posted by: uigiroux Posted at: 2018-07-04T20:36:49.959Z Reads: 305

```
This drive is specifically meant for PU wheels, so the gears need to be small and 2 gears doesn't place the motor far enough away from the truck base plate.  3 gears does.
```

---
## \#6 Posted by: FredrikHems Posted at: 2018-07-04T20:39:04.919Z Reads: 293

```
Remember for the gear ratio, that only the motor gear and the wheel gear will affect the final ratio :grin: I guess you already know this, but a reminder can never hurt anyone :grinning:

I have just finished my 3D printed 3 gear drive system like this, and I would strongly advice you to support the middle gear on both sides (hard to tell if it is already) Not only for better alignment, but also because it is subjected to alot of stress.
```

---
## \#7 Posted by: uigiroux Posted at: 2018-07-04T20:40:16.792Z Reads: 283

```
It will be, this is just an opened version so the internals can be seen.
```

---
## \#8 Posted by: FredrikHems Posted at: 2018-07-04T20:41:55.521Z Reads: 280

```
Will this be of plastic or cnc`d metal?
```

---
## \#9 Posted by: linsus Posted at: 2018-07-04T20:43:04.703Z Reads: 282

```
I run 2 gears on my carver :o with aliens. they sit good where they are.
```

---
## \#10 Posted by: uigiroux Posted at: 2018-07-04T20:43:32.138Z Reads: 276

```
Gears will be POM, the case will be aluminum.
```

---
## \#11 Posted by: uigiroux Posted at: 2018-07-04T20:44:46.396Z Reads: 270

```
That's a totally different type of truck though, we're making this for normal trucks.
```

---
## \#12 Posted by: Bor.inc Posted at: 2018-07-04T20:45:26.181Z Reads: 262

```
What is POM? is that a 3d print filament?
```

---
## \#13 Posted by: moon Posted at: 2018-07-04T20:47:46.325Z Reads: 266

```
[quote="FredrikHems, post:6, topic:60900"]
I have just finished my 3D printed 3 gear drive system like this, and I would strongly advice you to support the middle gear on both sides (hard to tell if it is already) Not only for better alignment, but also because it is subjected to alot of stress.
[/quote]

I've designed a shaft where the middle gear can spin. It also makes for great allignment 

Is this what you meant?
```

---
## \#14 Posted by: uigiroux Posted at: 2018-07-04T20:50:05.039Z Reads: 250

```
POM is a type of plastic I think... It's CNC'd and is self lubricated. It's what a lot of the gears are made of in the drives currently offered.
```

---
## \#15 Posted by: FredrikHems Posted at: 2018-07-04T20:59:21.728Z Reads: 244

```
I mean like, you should support the axle that the gear spin on, on both sides. :grinning:
```

---
## \#16 Posted by: MonkeyM Posted at: 2018-07-04T21:03:50.602Z Reads: 248

```
Gear ratio is very much personal preference, motor and battery specific. Sorry, it isn't much help!

When you know what speed/torque you want use an online eskate calculator to work out the ratio and ensure you have that overall ratio. 

Best to make the design such that you can adjust the ratio after building by a simple modification, ie change one gear. Then you can fine tune it later without having to start from scratch.

The gear profiles (module etc) have pros and cons, like noise, strength and efficiency. Best to have a look around if you haven't already. Bear in mind you could buy gears off the shelf in metal. Might be cheaper and less problematic than 3D printing; just thinking out loud.
Daval gears is a supplier in UK that comes to mind, use the knowledge on their site/catalogue but they probably wont sell 1s and 2s.
```

---
## \#17 Posted by: moon Posted at: 2018-07-04T21:04:03.754Z Reads: 240

```
Ok will do that, thanks!
```

---
## \#18 Posted by: uigiroux Posted at: 2018-07-04T21:08:02.316Z Reads: 240

```
For the production drives we won't be 3d printing anything, they'll be either bought or CNC'd.
```

---
## \#19 Posted by: moon Posted at: 2018-07-04T21:11:01.620Z Reads: 253

```
[quote="MonkeyM, post:16, topic:60900"]
Gear ratio is very much personal preference, motor and battery specific. Sorry, it isn’t much help!
[/quote]

Yes of course, no one has the same build :slight_smile:

[quote="MonkeyM, post:16, topic:60900"]
When you know what speed/torque you want use an online eskate calculator to work out the ratio and ensure you have that overall ratio.
[/quote]

Noted

[quote="MonkeyM, post:16, topic:60900"]
Best to make the design such that you can adjust the ratio after building by a simple modification, ie change one gear. Then you can fine tune it later without having to start from scratch.
[/quote]

That is exactly whats been done in the design. Although the wheel gear and middle gear are both customised but based on module 1.5 POM gears (not 3d printed) . So in the future ratio could be altered.

What are your thoughts on the current ratio,  16-27-38 Teeth with ratio of 2.375:1

Initially we went with module 1.5 gears, but when we realised 40T was not going to have any clearance at all we decided to drop down to module 1, then when I 3d printed it all it didnt seem right. So gone back to module 1.5
```

---
## \#20 Posted by: linsus Posted at: 2018-07-04T21:12:15.403Z Reads: 243

```
[quote="moon, post:19, topic:60900"]
2.375:1
[/quote]

3 or higher imo.
```

---
## \#21 Posted by: uigiroux Posted at: 2018-07-04T21:16:00.716Z Reads: 214

```
What ratio is your drives at if I may ask?  Are you also making yours specifically for PU wheels?
```

---
## \#22 Posted by: uigiroux Posted at: 2018-07-04T21:18:17.422Z Reads: 214

```
3 or higher would be if we were using bigger wheels like pneumatics, since we're using this drive for PU wheels, we definitely want below 3, but higher than 2.  We originally were going for right in the middle with 2.5, but circumstances came up and we opted for our current ratio.  It of course can be changed to a higher ratio if we change the motor gear down 1 or 2 teeth.  So we have room to play around with should it be needed.
```

---
## \#23 Posted by: Aeroquiv Posted at: 2018-07-04T21:18:35.322Z Reads: 216

```
I'd say 2.25 is a good medium of speed and torque. At 10s, 200kV motors, and 90mm wheel it would give you 30 mph and 36 mph at 12s.
```

---
## \#24 Posted by: uigiroux Posted at: 2018-07-04T21:21:05.730Z Reads: 216

```
We're thinking about wheels from 97mm up.  It could be used with the smaller wheels, but then the issue of ground clearance comes up.
```

---
## \#25 Posted by: Benjamin899 Posted at: 2018-07-04T21:22:16.192Z Reads: 213

```
if the gears are changeable, does it even matter?
```

---
## \#26 Posted by: moon Posted at: 2018-07-04T21:23:44.534Z Reads: 214

```
Because I want to go for a good standard, and also want to get some sound advice

Gears are not easily interchangeable, extra costs are inflicted because of that
```

---
## \#27 Posted by: Aeroquiv Posted at: 2018-07-04T21:25:11.912Z Reads: 208

```
I guess i'm in the minority, since I prefer wheels smaller than 90mm.
```

---
## \#28 Posted by: Benjamin899 Posted at: 2018-07-04T21:25:40.297Z Reads: 211

```
mmh true, havnt thought that out....you always need a set of gear if you want to change the ratio right?
```

---
## \#29 Posted by: moon Posted at: 2018-07-04T21:29:24.723Z Reads: 207

```
Yes, I suppose the motor gear can be changed with ease ,but I will look into that in a bit
```

---
## \#30 Posted by: Kug3lis Posted at: 2018-07-04T21:53:25.196Z Reads: 199

```
BTW, 3 gears as gear drive will be longer and it will introduce other clearance issues ;) We already have solution for 2 gear system.

Also 6384 will not fit on TB218 if you want to keep decent width of gears otherwise they will strip as contact width will be too small.
```

---
## \#31 Posted by: linsus Posted at: 2018-07-04T22:27:43.006Z Reads: 187

```
[quote="uigiroux, post:22, topic:60900"]
or higher would be if we were using bigger wheels like pneumatics, since we’re using this drive for PU wheels, we definitely want below 3, but higher than 2. We
[/quote]

I have no boards with pneumatics. My loaner board with kegels even has 3:1
```

---
## \#32 Posted by: FredrikHems Posted at: 2018-07-04T22:30:33.433Z Reads: 184

```
I’m using a gear ratio of 10:13:25, so a 1:2,5 ratio. Mine fits PU wheels from 80mm and up.. Not much clearance on 80mm though.. I have about 15mm of clearance on 90mm wheels, and this seems to be more than enough
```

---
## \#33 Posted by: moon Posted at: 2018-07-04T22:33:39.332Z Reads: 179

```
I did try something like that, probably tried 5 different setups. Just want a good place to start :)
```

---
## \#34 Posted by: uigiroux Posted at: 2018-07-04T22:47:42.056Z Reads: 181

```
Well that's great you have a solution now for a 2 gear system for PU wheels that fixes the clearance issues, but just a few weeks back when I was asking if you had anything in the works, so I could get that instead of a refund you said you didn't.  That's why we started this design.  We're not trying to make it so far that other clearance issues become a problem, just long enough that this main one with the truck base plate can be addressed.  Also we never said what trucks we'll be using these with so not really concerned about the TB 218's :wink:
```

---
## \#35 Posted by: Kug3lis Posted at: 2018-07-04T22:52:00.360Z Reads: 170

```
I said I didn't have anything to sell for you at that moment... I didn't say nothing is in the works. Do some simulations/test fits before going into making will save some money later on :)
```

---
## \#36 Posted by: uigiroux Posted at: 2018-07-04T22:57:44.755Z Reads: 168

```
Well I knew you didn't have anything in stock as you told me everything had to be made still since you were waiting on inventory.  I thought I had made it clear I was willing to wait if something was being developed...  Regardless, no harm done, it's in the past :slight_smile:

Yes we plan on making multiple iterations of prototypes before we actually land on a completed design.  We are about to start prototyping very soon, that's why we started this thread too see if anyone could point out things that may need to be changed or improved.  Hopefully all goes well :smile:
```

---
## \#37 Posted by: moon Posted at: 2018-07-05T00:19:59.602Z Reads: 169

```
Guess you went for module 2 spur gears
```

---
## \#38 Posted by: Lospalaz Posted at: 2018-07-05T01:02:46.940Z Reads: 181

```
I've been working on this for 6 months.  Half of the time spent is remembering how to use Blender!

I will never be finished. T_T

![57%20PM|687x500](upload://h3bC5VZ5naB89JsLk0PaWlxYfFD.jpg)![43%20PM|684x500](upload://2KtWDKoObpsMDyZVEj7fIn3IkX1.png)![07%20PM|690x470](upload://fhErLHXgOc0VjiXddN97sVHOF8A.jpg)![06%20PM|684x499](upload://nUWxlSFibi3es1ByXMcyHQqYbyp.png)
```

---
## \#39 Posted by: Benjamin899 Posted at: 2018-07-05T01:06:16.720Z Reads: 175

```
well thats a first i see something like that here
```

---
## \#40 Posted by: moon Posted at: 2018-07-05T01:12:31.442Z Reads: 178

```
You gotta start somewhere, I've only been messing around with fusion for about half a year too
```

---
## \#41 Posted by: Lospalaz Posted at: 2018-07-05T01:13:55.917Z Reads: 177

```
inspired by @GrecoMan and @florr

https://www.electric-skateboard.builders/t/jenso-style-direct-drive-for-street-boards/34811?u=lospalaz
https://www.electric-skateboard.builders/t/custom-deck-mount-bevel-gear-racerstar-6368-6s-5000mah-arduino-uart-514/35189?u=lospalaz
```

---
## \#42 Posted by: Lospalaz Posted at: 2018-07-05T01:25:12.528Z Reads: 169

```
I've been half-heartedly "getting into Blender" for about 8 years... T_T

I didn't have the motivation until I realized my motors are waaay too long for my generic trucks =P
```

---
## \#43 Posted by: Pedrodemio Posted at: 2018-07-05T03:16:06.039Z Reads: 161

```
One thing to improve reliability is make the number of teeth non multiple of each other, this way all tooth from one gear mesh with all other tooth of the other gear. This way you spread out the wear since no two tooth are exactly equal

Another point, make the middle gear more robust, it doesn’t appear, but the loading is way higher, almost two fold, maybe make it metal

I don’t know if it’s a good idea to make all gear plastic since you don’t have a gear that keep the profile with wear, making the middle gear metalic solves this too
```

---
## \#44 Posted by: skatardude10 Posted at: 2018-07-05T03:48:16.522Z Reads: 154

```
You use Blender for CAD?
```

---
## \#45 Posted by: Lospalaz Posted at: 2018-07-05T04:07:36.942Z Reads: 156

```
Yes. So far, so good!
```

---
## \#46 Posted by: FredrikHems Posted at: 2018-07-05T09:51:40.148Z Reads: 153

```
Yup, module 2 seems to be more than strong enough with 3D printed plastic
```

---
## \#47 Posted by: Schulerbible Posted at: 2018-07-05T10:13:09.979Z Reads: 154

```
Use F360 / Inventor or any free CAD modeling software. Blender is just too complicated to get a thing done. I would never even think about using Blender for such a purpose.
```

---
## \#48 Posted by: moon Posted at: 2018-07-05T14:46:15.029Z Reads: 141

```
Sounds pretty good, we have gone for 15mm wide spur gears, is there any reason for us to go wider
```

---
## \#49 Posted by: moon Posted at: 2018-07-05T14:46:35.343Z Reads: 139

```
Thanks for the good advice
```

---
## \#50 Posted by: FredrikHems Posted at: 2018-07-05T14:49:34.408Z Reads: 142

```
I am using 15mm aswell, I dont think any thicker is needed. And your gears out of cnc`d POM should be even stronger than my 3d printed plastic ones :smiley:
```

---
## \#51 Posted by: moon Posted at: 2018-07-05T14:51:49.947Z Reads: 136

```
Yes of course POM is very good.

We have reduced the overall size of the gear box now, going for 25-17-10
```

---
## \#52 Posted by: FredrikHems Posted at: 2018-07-05T15:18:12.493Z Reads: 129

```
You have some more pics? :grinning:
```

---
## \#53 Posted by: moon Posted at: 2018-07-05T15:19:07.014Z Reads: 131

```
I will do soon, I will PM when I done - share some ideas 

3D printer is broken down right now so nothing physical yet.
```

---
## \#54 Posted by: Lospalaz Posted at: 2018-07-05T15:24:22.984Z Reads: 127

```
I keep hearing about Fusion. I'll see what's on Youtube, but I have unfinished business with Blender! ^_^
```

---
## \#55 Posted by: moon Posted at: 2018-07-05T15:25:00.694Z Reads: 128

```
Its not the  enemy :joy:

Fusion is great, basic and simple to use
```

---
## \#56 Posted by: Holyman92 Posted at: 2018-07-05T15:42:08.702Z Reads: 128

```
i love this design, are y'all gonna post the files or is this going to be intended to be sold?
```

---
## \#57 Posted by: Holyman92 Posted at: 2018-07-05T15:43:51.371Z Reads: 135

```
i was wondering if this was going to happen, now my question is, since it has 3 gears can this be made to fit SR trucks? the issue me and Kug talked about was clearance but this solves that problem
```

---
## \#58 Posted by: moon Posted at: 2018-07-05T15:44:37.199Z Reads: 132

```
It can be made to fit SR, but I dont have SR so at the moment it cant be done

SR = surfrodz right?
```

---
## \#59 Posted by: L3chef Posted at: 2018-07-05T15:44:47.454Z Reads: 131

```
What's your mounting solution? Can I see the backside?
```

---
## \#60 Posted by: moon Posted at: 2018-07-05T15:45:12.862Z Reads: 132

```
Maybe a bit later :)
```

---
## \#61 Posted by: Holyman92 Posted at: 2018-07-05T15:45:39.643Z Reads: 129

```
@moon i can give you w/e measurments you need... considering they are precision trucks their tolerances should be fairly tight across their batches
```

---
## \#62 Posted by: moon Posted at: 2018-07-05T15:46:06.853Z Reads: 127

```
Yes go ahead, Im going to go offline for a bit so just drop a PM
```

---
## \#63 Posted by: Holyman92 Posted at: 2018-07-05T15:48:25.780Z Reads: 131

```
shoot me a pm w/ w/e measurements you need... I am not a 3D/cad guy but i do know how to measure and have calipers, i'm in no rush but i really want a gear drive... im growin tired of belts lol
```

---
## \#64 Posted by: uigiroux Posted at: 2018-07-05T15:50:12.506Z Reads: 132

```
Intend to sell.
```

---
## \#65 Posted by: Holyman92 Posted at: 2018-07-05T16:10:26.337Z Reads: 128

```
Fair enough, If u make it mount to SR trucks I'd be down for a set
```

---
## \#66 Posted by: uigiroux Posted at: 2018-07-05T16:20:17.847Z Reads: 126

```
We haven't decided on what trucks the first sets will be used with, but I think we'll be able to make it fit with most trucks, just need to create different mounts that can be easily switched out.
```

---
## \#67 Posted by: Holyman92 Posted at: 2018-07-05T16:27:44.380Z Reads: 127

```
Well I will be eagerly waiting... until then the guys at my makerspace are itching to help me make a gear drive system lol
```

---
## \#68 Posted by: uigiroux Posted at: 2018-07-05T16:29:15.193Z Reads: 127

```
Lol, I don't think it'll be too much longer before we have a working model.  Starting prototyping now.  Just gotta work out a few things and we should be good to go :smile:
```

---
## \#69 Posted by: moon Posted at: 2018-07-05T18:54:34.352Z Reads: 115

```
Guys at your makerspace? Are they esk8ers too
```

---
## \#70 Posted by: Holyman92 Posted at: 2018-07-05T21:16:32.905Z Reads: 106

```
No lol, they are old machinist, but they are fascinated by my VERY crude board lol
```

---
## \#71 Posted by: wafflejock Posted at: 2018-07-05T21:21:06.840Z Reads: 108

```
Blender is really rough to do CAD in whenever you need to change the size/position of a component it becomes a cascading mess since they don't seem to really have any parametric modeling stuff built in (I saw a plugin for it but not sure how well maintained that is).  I started off doing my designs in Blender at first as well but moved over to onshape since it's also free so long as you're cool with your models being in the public and able to copied/forked and edited by anyone.  There's also freecad but that seemed to be pretty unstable to me and I was looking for something easier than blender not harder :)
```

---
## \#72 Posted by: moon Posted at: 2018-07-05T21:29:58.565Z Reads: 108

```
That's pretty cool, I guess there's a little workshop with a lathe or a cnc machine or something?

Let's stay on topic ;) @wafflejock
```

---
## \#73 Posted by: wafflejock Posted at: 2018-07-05T21:31:06.469Z Reads: 105

```
Yah sorry didn't mean to derail just wanted to throw it out there... have been through that struggle myself before :)
```

---
## \#74 Posted by: Holyman92 Posted at: 2018-07-05T21:40:10.142Z Reads: 108

```
It's more of a warehouse w/ a blacksmithing forge, 3d printers, laser cutters, 2 or 3 lathes, a large cnc mill, a small cnc mill and I'm sure there's more but I haven't been past those parts of the warehouse yet
```

---
## \#75 Posted by: moon Posted at: 2018-07-05T21:41:21.617Z Reads: 112

```
Wow that sounds amazing, I wish I was where you were lol.

About the SR I will pm you now
```

---
## \#76 Posted by: Holyman92 Posted at: 2018-07-05T21:45:46.571Z Reads: 114

```
Yea I just found it XD and for sure... I'm just threading some PETG gears and about to go see why my printer melted a part on the board >:(
```

---
## \#77 Posted by: moon Posted at: 2018-07-05T21:47:59.514Z Reads: 117

```
My 3D printer burnt aswell, the PCB. Its because the connectors cheaper 3D printers use are low quality and for the hotend and heat bed its best to have a mofset like this hooked up

https://www.amazon.co.uk/PChero-Expansion-Current-Module-Printer/dp/B071XBZGXG/ref=sr_1_4?s=industrial&ie=UTF8&qid=1530827220&sr=1-4&keywords=3D+Printer+MOSFET
```

---
## \#78 Posted by: Holyman92 Posted at: 2018-07-05T21:51:15.562Z Reads: 119

```
Thanks :D... Yea this one was free so I mean it preformed waaay better than expected as far as print quality 

![1530827415581878042455|374x500](upload://hSybZdDGISenASAN2Zb654saf1H.jpg)
```

---
## \#79 Posted by: Vanarian Posted at: 2018-07-05T23:04:48.353Z Reads: 117

```
How sick is that drive? I'll PM the hell outta your box right now :joy:
```

---
## \#80 Posted by: moon Posted at: 2018-07-11T16:30:50.050Z Reads: 103

```
Sending a DM now
```

---
## \#81 Posted by: Underoath888 Posted at: 2019-09-06T21:35:28.815Z Reads: 40

```
Any chance you could make one for me?
```

---
## \#82 Posted by: moon Posted at: 2019-09-06T21:37:59.028Z Reads: 40

```
Check the other forum :)

https://forum./t/lycan-3gdrive-testing/5340/164
```

---
