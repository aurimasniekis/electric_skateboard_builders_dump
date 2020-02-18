# Rolling Fortress &#124; LaCroix Prototipo &#124; Dual Focbox/6374 &#124; DIY MBS Geared Drive &#124; 12S4P

### Replies: 139 Views: 8888

## \#1 Posted by: ervinelin Posted at: 2018-06-15T16:19:02.490Z Reads: 972

```
![DSC06961|690x461](upload://h1SUsoPWRM1IpJlnkyRcGEBZLXM.JPG)

I never liked the idea of placing electronics in pelican boxes (although I can understand why) so when I first saw builds of mountainboards with flexible underslung enclosures (like the LaCroix) I was hooked... But I neither had the space, time nor skills to build a flexible enclosure.

So when Alex & Pat from LaCroix decided to start selling their Prototipo deck with [enclosure at a discounted introductory price](https://www.electric-skateboard.builders/t/lacroix-board-co-wood-and-cf-deck-segmented-flex-carbon-fiber-enclosure-group-buy-completed/49051), I jumped in for the ride!

From ordering to delivery took a few months, so I had a lot of time to gather up my parts and get ready for the eventual build and my goodness it was the longest build I have ever done. This is the 5th esk8 I have built and none of the others compares to how much work this was... (FYI, I have 3 working boards now, each for a different purpose, this is for the occasional offroad experience, the smallest is a milk run board, the middle is something in between).

**Parts list:**
Deck - [LaCroix Prototipo with CF enclosure](https://www.lacroixboards.com/product-page/board-carbon-fiber-enclosure-prototipo)
Trucks - [MBS Matrix II (Hollow Axle)](https://www.mbs.com/parts/12202-mbs-matrix-ii-pro-truck-system-1)
Hubs - [MBS Rockstar II](https://www.mbs.com/parts/13231-mbs-rockstar-ii-hub-black-1)
Tires - [MBS 8" T3](https://www.mbs.com/parts/13131-8-mbs-roadie-tire-black-1)
ESC - [Dual Focbox](https://longhairedboy.com/collections/all/products/focbox-electric-skateboard-motor-controller)
BMS - [Bestech HCX-D596 with E-switch](https://www.electric-skateboard.builders/t/group-buy-bestech-bms-80a-e-switch-paused/42222)
Battery - DIY Samsung 30Q 12S4P mounted on [PCB](http://electricskateboard.repair/index.php?id_product=28&controller=product)
Motors - [Buildkitboards 6374 190kv](https://buildkitboards.com/collections/motors/products/6374-190kv-motor) 
Remote - [DIY Trigger Style Remote with Telemetry](https://www.electric-skateboard.builders/t/diy-trigger-style-remote-with-telemetry-complete-guide/48231)
Drive - DIY 1:5+ Geared Drive (see below)

Anyway, some folks have asked me to document my build so here it is.

![DSC06933|690x461](upload://oFCjPRqSis366B8mrIMW3mJctWU.JPG)

![DSC06941|690x461](upload://neYHkVUCQJILlC2tRpn0aFzi4fG.JPG)

![IMG20180609024817|690x388](upload://1NkG4kraEImFcEzRdpJsYo54Xx7.jpg)

[Front and back lights](https://www.banggood.com/XANES-2-in-1-500LM-Bicycle-USB-Rechargeable-LED-Bike-Front-Light-Taillight-Ultra-light-Warning-Night-p-1191651.html?utm_campaign=android-share-android-share-mesh.drone&utm_source=youtube&utm_content=huangguocan&utm_medium=sku860005-0319&utm_design=0&android_share=1&_branch_match_id=466492216463184787) are from Banggood and I designed and printed mounts for them to slide onto the MBS Matrix II trucks. [STLs are available here for those who want it.](https://www.thingiverse.com/thing:2954450)

![IMG20180614025805|690x388](upload://azbRRzlty72msbxE9JKyXYgO4T1.jpg)
The LaCroix itself is VERY SPACIOUS inside, fits 12S4P extremely comfortably with the oversized BMS and dual Focboxes. I soldered the 4P packs together using good quality wires instead of nickel strips because firstly I don't have a spot welder and secondly, nickel itself is not that fantastic a conductor. I heat up the iron to 480degs, pre-tin everything then solder them slowly. I took my time with this, 1 or 2 4P packs a night over several nights. In between 4P packs I use 3 x 16AWG wires for the flex, 12AWG for between battery assembly and ESCs/BMS.

![IMG20180320012827|666x500](upload://9BtLujpxNKdP44QztW5O9rbqomJ.jpg)
Remote is using the [DIY Trigger Style Remote with Telemetry](https://www.electric-skateboard.builders/t/diy-trigger-style-remote-with-telemetry-complete-guide/48231) I designed based on Solidgeek's remote. I must say the CF enclosure gives me poorer range than I prefer but still works nonetheless. Discussions on the remote are on the thread linked above.

![IMG20180614123639|281x500](upload://wOdE7H8gwetQIzOmIiYH2xZGu4m.jpg) ![IMG20180614125235|281x500](upload://sLoyC0urdUxtb5n1kMAihtAScFU.jpg)

I route the motor cables under the enclosure rather then through it so that should I need to remove the enclosure I can do so completely. I dremeled out a channel, heat shrunk and silicone taped the area where it presses against the enclosure. I then used instamorph to make a little "hood", I wanted to 3D print it but i got lazy. Of course I painted it black later.

![DSC06966|690x461](upload://ptxzfo5gFvj1esxBS1wLrRGhI5p.JPG)

The power indicator is just a simple 5v [3 LED PCB](https://banggood.app.link/urHh0ZJhKN) I had lying around from my RC quadcopter days. I removed the dip switch, hard wired it for red, then drilled 3 holes, one for each LED. I then used clear hot glue to simultaneously seal and hold the PCB in place. Lastly, I used the 5V from the spare Focbox to power it.

![MBS_Drive_1|666x500](upload://ntQp4LiiZAVsFM8act8AUICyIWQ.jpg)

I really liked the E-Toxx geared drives but they cost an arm and a leg but more importantly they don't fit MBS Matrix II trucks, so I had to design my own drive from scratch. Luckily I already had experience from designing a similar style geared drive for my smaller boards, so it was just a matter of upscaling. AT sized boards also have A LOT more space so it wasn't so critical to get everything sized absolutely perfectly.

FYI, I printed this using PLA 2.0 (from [Qwikfab](https://www.qwikfab.com/)). This is not to be confused with PLA, PLA 2.0 (or some call it PLA+) is stronger than regular PLA and has held up well for now.

And before you ask, yes I intend to share the STLs but only after I have tested the drive a little more.

![IMG20180526165339|690x388](upload://oBI8QxJoLEBtqMwRsROOgwngTH8.jpg)

![IMG20180526165642|690x388](upload://iST4UYJaRXvedK33LUk9aVBu6LB.jpg)

![IMG20180512174806|281x500](upload://6BWBZBnT3spIqr7RPk3Y31FpC6j.jpg) ![IMG20180512174732|281x500](upload://5bh4DvVuhX3zTW9pthhxW3u1Yht.jpg)
 
The drive comprises of several parts, the first being the 73T 1.5M 20degree pitch gear attached to an adapter which slides into the MBS Rockstar II hubs. The idea is you can remove the wheel without touching the gears. Also, it's in 2 different pieces so that I can swap out the gear if I wanted to, and also to provide more strength by using the M6 bolts. I also use a 6806 bearing with an adapter to keep the gear centered around the axis of the truck.

![IMG20180515205723|281x500](upload://iVYVHTLFdajTteWgPvgOXi4jZkQ.jpg) ![IMG20180523191613|281x500](upload://sbfb6T3OJHw3KCQ8TjT8XmwqYeQ.jpg) 

The mounts are also 3D printed, slide onto the trucks and held down by an M6 bolt. I desigend them extra chunky because well... it's no metal mount...

![IMG20180614145059|690x388](upload://qaVtYgR4SxofBmKWh4t5ABKKlxt.jpg)

![IMG20180614145055|690x388](upload://lOwcgeEhKW9GTjTXvoQ5nF70f6y.jpg)

![IMG20180614145551|690x388](upload://6ZZXeKJwiTiSiF0QMFAv059iiOS.jpg)

The gear interfaces with a [cheap 12T spur](https://www.aliexpress.com/item/2pcs-Spur-Gear-pinion-12T-12Teeth-Mod-1-5-M-1-5-Width-12mm-Bore-5/32845281613.html?spm=a2g0s.9042311.0.0.61654c4dnpZiYs) I found (the only one I found that could fit). This is then encased in a gear cover to keep the lubricant from flying all over the place and prevents grime from building up.

![DSC06952|690x461](upload://zNL0seWl3PDkEsyR7NBt56Asz1O.jpg)

The final drive works pretty well so far and looks pretty stealthy, I just need more time to test it. The spurs are not silent but good enough, the key is the meshing (mounting screws allow for slight adjustments) and lubricant (from which I need something thicker that doesn't get flung off).

![DSC06927|334x500](upload://16FW2doN8v2quL0jVNFVLPpdcLv.JPG) ![DSC06925|334x500](upload://xQmbOpDDS133XiIhdLWEWbKJcRJ.JPG)
Griptape wise I was so totally exhausted by the end of the build that I just went with a simple 2 squares of vicious tape leaving a nice square for the LaCroix logo. The geared drives allows the motor mounts to be short enough that I can lean my board against the wall, as well as to drag it around on its back wheels when I am not riding or moving around in very tight spaces.

Here are some other shots of the final build... Can't wait to ride it more once the weather clears up!

![DSC06933|690x461](upload://oFCjPRqSis366B8mrIMW3mJctWU.JPG)

![DSC06956|690x461](upload://gLfBxfF8qViu2IdmZWhut3u5Bxx.jpg)

![DSC06929|690x461](upload://ygaEC8TR1gxXAZYp03JuVicPSc5.jpg)

Hit me up if you have more questions!

Thanks for reading!

PS: I nicknamed it rolling fortress because it feels so different from my other decks, feels more massive and solid...
```

---
## \#2 Posted by: Linny Posted at: 2018-06-15T16:26:52.413Z Reads: 663

```
An honor to be able to ride this last night. Acceleration is really smooth and quite manageable for a 12s4p. 
I'm not used to a MTB deck so my legs felt weird when turning. Nonetheless a great.. no, an awesome build!
```

---
## \#3 Posted by: Der6FingerJo Posted at: 2018-06-15T16:28:05.018Z Reads: 660

```
This looks great, especially the drive. I wonder how the motor mounts hold up since this is a problem with my 3d printed drive. Is PLA 2.0 stiffer than regular PLA? I printed mine in PETG.
```

---
## \#4 Posted by: ervinelin Posted at: 2018-06-15T16:31:51.383Z Reads: 638

```
It's definitely stronger than PLA and I think in specs even ABS.

Not sure how long they will last though, thus the hold back on STLs just so I can give them enough time to test them.
```

---
## \#5 Posted by: Arch Posted at: 2018-06-15T16:39:12.140Z Reads: 617

```
Great build and writeup Erv! Well done.
```

---
## \#6 Posted by: mmaner Posted at: 2018-06-15T16:40:01.322Z Reads: 582

```
beautiful, impressive drive system as well...respect.  I wish I had gotten in on the lacroix group buy :frowning:
```

---
## \#7 Posted by: pat_arch Posted at: 2018-06-15T16:40:26.554Z Reads: 562

```
Great work buddy!
```

---
## \#8 Posted by: Dyspro Posted at: 2018-06-15T16:41:03.966Z Reads: 551

```
It's the perfect dream build for me. Really interested in how the gears turn out. Do you mind ballparking the total cost of the build?
```

---
## \#9 Posted by: ervinelin Posted at: 2018-06-15T16:43:13.947Z Reads: 554

```
Because I build the battery myself and essentially printed the drive, I spent approximately 1800USD give or take.

Unfortunately I live on the other end of the globe, so shipping was a real pain.... could have shaved off 300US just on shipping alone.
```

---
## \#10 Posted by: webst Posted at: 2018-06-15T19:08:02.371Z Reads: 539

```
[quote="ervinelin, post:9, topic:59021"]
Unfortunately I live on the other end of the globe, so shipping was a real pain… could have shaved off 300US just on shipping alone.
[/quote]
I know your pain (sweetened by pack of Haribo), after additional shipping costs I also paid customs that in total exceeded regular price (well, this should make @mmaner feel a little less bad for his poor reflex). 

Nevertheless: great build! I really love printed gear idea and would love to see it work reliably as it really bothers me that available solutions cost half a kidney while I've already sold one.
```

---
## \#11 Posted by: ervinelin Posted at: 2018-06-16T00:27:27.806Z Reads: 512

```
I have tortured my other printed gear drive a fair bit and it holds up well enough to abuse. The only wear was when a motor screw dislodged and got caught in the gears.. (not fun)

However I don't go fast, no where near the speeds demons I hear of here. Firstly because my I only have mortal balls as opposed to those of steel. And more importantly the laws here greatly limit electrically driven devices. Failure to adhere will mean they take your board away and destroy it after they charge you in court.

As such for my purposes the printed drive might surffice but not for others needing more durability.
```

---
## \#12 Posted by: ervinelin Posted at: 2018-06-16T05:34:29.741Z Reads: 508

```
![71ac4150-8edc-4f16-b66b-4df3ac4fa49d|375x500](upload://bUIDNKl0x4D0fMSm2974l7Ys2pt.jpg)

Wow it's such a weird feeling to be able to ride over this and still keep going!! 

My last board has MBS 100mm "All Terrain" wheels but frankly it wouldn't make it past the first 5m...
```

---
## \#13 Posted by: cap7ainclu7ch Posted at: 2018-06-16T06:59:27.962Z Reads: 480

```
Looks like so much fun.  How does it carve?  Can you slide it on the gravel?
```

---
## \#14 Posted by: ervinelin Posted at: 2018-06-16T07:14:32.552Z Reads: 474

```
I think the red shock blocks are too stiff.. doesn't carve as well as I hope. Will try swapping them out for something softer...

As for sliding on gravel didn't try! Wasn't wearing enough protection to risk getting banged up haha...
```

---
## \#15 Posted by: banjaxxed Posted at: 2018-06-16T08:39:21.148Z Reads: 456

```
Just beautiful and...awesome

More than a little interested in the drive design, what are you going to lube it with? Think @Deckoz was getting a good result with white grease. You can get good ones in marine chandlers. Resists water and very low fling
```

---
## \#16 Posted by: ervinelin Posted at: 2018-06-16T08:49:56.642Z Reads: 462

```
I am currently using a high temp lube but it's not working out for me... After riding a while I am pretty sure it gets louder and louder maybe cos the lube is being thrown all over the place...

I tried spray on white lithium and that's even more runny!

What's marine chadlers?
```

---
## \#17 Posted by: banjaxxed Posted at: 2018-06-16T09:46:22.339Z Reads: 446

```
Boat shop suppliers, the white gick used to grease parts that get immersed in water
```

---
## \#18 Posted by: ervinelin Posted at: 2018-06-16T09:46:51.624Z Reads: 445

```
Hmm.... Okay let me go hunt...
```

---
## \#19 Posted by: banjaxxed Posted at: 2018-06-16T09:48:02.380Z Reads: 451

```
In a small tub..Deckoz used it to good effect afaik
```

---
## \#20 Posted by: banjaxxed Posted at: 2018-06-16T09:49:27.731Z Reads: 468

```
Something like this, but cheaper in a tub
https://www.amazon.co.uk/Johnson-Evinrude-Triple-Guard-Marine-Cartridge/dp/B00R55K544

Looks promising 
http://www.rccrawler.com/forum/tools-supplies/389184-wheelworks-black-n-tacky-gear-lube***-stock***.html
```

---
## \#21 Posted by: Michaelinvegas Posted at: 2018-06-16T09:49:52.573Z Reads: 421

```
Superb build 👌🏻 Well done
```

---
## \#22 Posted by: Deckoz Posted at: 2018-06-16T11:46:01.524Z Reads: 418

```
Yea. I used white lithium paste. :)
```

---
## \#23 Posted by: ervinelin Posted at: 2018-06-16T12:19:46.596Z Reads: 423

```
Lithium paste...that sounds thicker... Mine is a spray which doesn't seem thick at all
```

---
## \#24 Posted by: deucesdown Posted at: 2018-06-16T12:23:04.584Z Reads: 445

```
I don't actually know if it would be good but it sounds like a job for 

https://www.amazon.com/Maxima-74920-Chain-Wax-Aerosol/dp/B0012TZ1RU
```

---
## \#25 Posted by: ervinelin Posted at: 2018-06-16T12:23:40.107Z Reads: 429

```
I have some chain lube...too thin
```

---
## \#26 Posted by: deucesdown Posted at: 2018-06-16T12:24:56.988Z Reads: 423

```
Chain wax is quite thicker than typical. It still flings but stays on way better.
```

---
## \#27 Posted by: Sn4pz Posted at: 2018-06-16T12:27:41.817Z Reads: 435

```
off the chain wax bro :call_me_hand:

https://www.youtube.com/watch?v=He7TnoCM7fo
```

---
## \#28 Posted by: deucesdown Posted at: 2018-06-16T12:32:42.952Z Reads: 423

```
There's also this but it's for metal on metal I believe

https://www.wurthusa.com/Chemical-Product/Lubricants/Specialty-Lubricants/HHS-K-Hinge-Lubricant/p/0893106050

Some guys on silverfish tried the old version (hhs-2000) for a durable waterproof bearing lube, to great effect. Forms a film that stays put.
```

---
## \#29 Posted by: ervinelin Posted at: 2018-06-16T12:34:26.042Z Reads: 411

```
I think the white marine grease will be the one to use.. all of them will be lubricating but I suspect the noise reduction will be using the really thick ones...
```

---
## \#30 Posted by: banjaxxed Posted at: 2018-06-16T12:36:44.933Z Reads: 408

```
Chain wax may be worth a look
```

---
## \#31 Posted by: Ackmaniac Posted at: 2018-06-16T12:59:15.069Z Reads: 405

```
Please make a video of the drive where we can hear the sound. Really cool would be in combination with my app to see how it behaves at different power levels if you have a BLE module.
```

---
## \#32 Posted by: Deckoz Posted at: 2018-06-16T13:46:54.592Z Reads: 430

```
![15291567381612011453396|375x500](upload://fTZFV4LsuoTOdFgobvkd5Fmp2ge.jpg)

![1529156782502601692578|375x500](upload://pJMNQH0aNKxqmbldn8t7pSH164C.jpg)

Yes it's thick.
```

---
## \#33 Posted by: ervinelin Posted at: 2018-06-16T14:03:56.036Z Reads: 414

```
Would that be on the bench or off?
```

---
## \#34 Posted by: ervinelin Posted at: 2018-06-16T14:04:41.036Z Reads: 411

```
That's what I need!!
```

---
## \#35 Posted by: Ackmaniac Posted at: 2018-06-16T16:13:21.056Z Reads: 422

```
The app has the possibility to place the realtime data over your video that you record with your smartphone.
More info here
https://www.electric-skateboard.builders/t/vesc-monitor-android-app/20888?u=ackmaniac

And here is a example how it looks like
https://youtu.be/c9MuFeAyqTo
```

---
## \#36 Posted by: banjaxxed Posted at: 2018-06-16T16:19:50.753Z Reads: 397

```
Also a remarkable moisturiser
```

---
## \#37 Posted by: RyuX Posted at: 2018-06-16T16:56:11.579Z Reads: 398

```
yay my video is famous.. haha xD
```

---
## \#38 Posted by: Blacksheep Posted at: 2018-06-16T19:00:47.394Z Reads: 396

```
Does anyone know where I can get some matrix 2 trucks hallow?
```

---
## \#39 Posted by: Mobutusan Posted at: 2018-06-16T19:17:03.785Z Reads: 402

```
Fantastic build. So clean and functional...and fuqqin' beautiful. Your photo skills compliment the board nicely too. 

And your drive system looks great. I'm surprised it hasn't been asked yet, but do you have any plans to try helical gears as well? Honestly, I think that's about the only thing you could "improve" on, if it holds up, of course. I love the sealed gear drive especially with the silent helicals.
```

---
## \#40 Posted by: philvanzu Posted at: 2018-06-16T19:58:22.729Z Reads: 403

```
Only @longhairedboy  could provide you hallowed MatrixII since he has a special relationship with Skatan.
```

---
## \#41 Posted by: Blacksheep Posted at: 2018-06-16T19:59:27.120Z Reads: 383

```
Where did you get yours ?
```

---
## \#42 Posted by: philvanzu Posted at: 2018-06-16T20:00:28.251Z Reads: 393

```
Some shop in Berlin : https://www.coronation-industries.de/shop/fr/trucks-mountainboards/8253-mbs-matrix-ii-pro-truck-system-black.html
```

---
## \#43 Posted by: ervinelin Posted at: 2018-06-16T21:58:51.357Z Reads: 399

```
I tried helicals on my smaller drive. They gave me more problems than it was worth and weren't super quiet either... 

![IMG20180516215618|690x388](upload://e0AYCr4pjbl9WaI1OBcjWSHphv5.jpg)

Not to mention they were very costly to manufacture and were a real bitch to align.

Probably the biggest problem was the axial loads, this puts a lot of strain on the mount and other components... 

I ditched helicals after I heard Arc boards Fenix drives which were spurs and quiet enough.
```

---
## \#44 Posted by: ElectricCoast Posted at: 2018-06-17T03:39:52.052Z Reads: 389

```
I absolutely love this build!!!  I just found the LaCroix board a few days ago on here.  I'm still a newb but I would have bought a LaCroix at the special pricing but I can't justify the expense of one now.  The build looks amazing.
```

---
## \#45 Posted by: ervinelin Posted at: 2018-06-17T03:58:44.401Z Reads: 391

```
Just so you guys know... 3D printing was just for prototyping... I always meant for it to milled out but just can't justify the expense.

![IMG20180617115617|690x388](upload://9gUXIQT8bWrRZoYpCzwrLVFj6T8.jpg)

Here's the prototype geared drive mount for caliber ii trucks that I am working on.
```

---
## \#46 Posted by: ervinelin Posted at: 2018-06-17T04:05:12.153Z Reads: 387

```
Found a source for this locally.. will give it a try
```

---
## \#47 Posted by: ervinelin Posted at: 2018-06-17T04:10:33.572Z Reads: 383

```
I haven't tried your firmware yet simply because the thread is now 700 posts long and I was too busy to read through all of it!

I am also already using UART on my master to get telemetry to my remote, can I stick in a Bluetooth module on the slave?

I will try to get at video out soon when I have the time... Had to work over the weekend..
```

---
## \#48 Posted by: ervinelin Posted at: 2018-06-17T05:38:16.540Z Reads: 393

```
![IMG20180617132206|281x500](upload://9B7PC0o5ZjSdgo4fwdjy2UGi0ss.jpg)

Found it... But its not white...
```

---
## \#49 Posted by: banjaxxed Posted at: 2018-06-17T06:01:53.340Z Reads: 368

```
The one deckoz posted may be thicker can you swap for white lithium in the same place? Iirc evinrude is blue but maybe not as thick as the white goo
```

---
## \#50 Posted by: Ackmaniac Posted at: 2018-06-17T06:35:22.660Z Reads: 353

```
Yes you can use it at the slave.
```

---
## \#51 Posted by: ervinelin Posted at: 2018-06-17T13:22:16.729Z Reads: 359

```
No I bought it of a guy who was selling it.. not a proper shop. I know where to get white lithium paste but it was of a generic house brand...

Anyway I applied the Evinrude, man it's reeaalllly thick and sticky... Now when I turn my wheels I hear the grease... 

Will have to ride it to know if it helps...
```

---
## \#52 Posted by: dareno Posted at: 2018-06-17T18:38:22.241Z Reads: 344

```
What a beautiful build,  really gutted to have missed that lacroix deal. I'm still tempted though especially when you see such a epic finished product.
I wouldn't mind hearing a bit more about the battery build.  I don't have a spot welder either and your set up looks the most professional soldered solution I've come across.
I'm going to thank you for the inspiration but my wife isn't :smile:
```

---
## \#53 Posted by: banjaxxed Posted at: 2018-06-17T22:26:20.738Z Reads: 345

```
Hopefully it does the trick interested to see your update on it
```

---
## \#54 Posted by: ervinelin Posted at: 2018-06-17T23:28:30.373Z Reads: 373

```
Basically I soldered then in stacks of 4. There are PCBs (see link above) you can buy that basically help a little in building these packs. What I like about them is that it's much much easier to solder to the PCB than it is directly to the cell. So when connecting wires between 4P packs or large 12AWG wires, it's just much easier with the PCB.

Here's how I do up each pack:
1. Hot glue the cells together
2. Hot glue the glued cells to the underside of the PCB
4. Paste stickers meant to protect the positive end of the cell from accidental shorting with the cell body
4. Cut a piece of wire to length (solid copper is good but I used high quality silver coated wire meant for speakers just cos it works for me)
5. Bend the wire such that it touches all the cells and then folds up and over the PCB
6. Use a penknife and scratch the surface of the cell to roughen it slightly
7. Heat soldering iron to 480deg using a large wedged soldering top
8. Tin all cell ends, wire and the PCB
9. Solder bent wire to cells and PCB careful not to spend too much time heating up each cell
10. Repeat on other end of cell
11. Tape the bottom half of the packs and cover the top with masking tape temporarily just in case.
12. Move on to next 4P pack, rinse and repeat.
13. Layout and connect all packs as per your design
14. Connect BMS (I didn't use the PCBs cell pads, I soldered directly to the PCB main pad)
15. Tape everything up and hope nothing smokes!
```

---
## \#55 Posted by: dareno Posted at: 2018-06-18T06:40:16.206Z Reads: 342

```
Thanks man really helpful!
```

---
## \#56 Posted by: skslingo21 Posted at: 2018-06-18T16:22:05.798Z Reads: 353

```
Transmission is awesome!! Props to you!!!!  Do you sketch your own gear teeth or import them?

The Board is sweet as well, the blocks of griptape do not detract the sweetness :sunglasses:
```

---
## \#57 Posted by: ervinelin Posted at: 2018-06-18T16:44:57.433Z Reads: 349

```
Thanks! Gears are from a gear generator for Rhino. Seems to work well enough to get me the outline, then I do the rest of the modelling myself.
```

---
## \#58 Posted by: moon Posted at: 2018-06-18T16:52:55.495Z Reads: 356

```
[quote="ervinelin, post:57, topic:59021"]
gear generator for Rhino.
[/quote]

Whats this?

I have just been using CAD files from maedler or KHK , but I don't like doing that
```

---
## \#59 Posted by: webst Posted at: 2018-06-18T16:56:07.702Z Reads: 362

```
It's gears generating plugin for 3D modelling software called Rhino.
You could also use http://geargenerator.com or http://www.instructables.com/id/The-Easy-Way-to-Design-Gears-in-Fusion-360/
```

---
## \#60 Posted by: moon Posted at: 2018-06-18T17:55:33.789Z Reads: 374

```
I found this instead

http://www.jamesgregson.ca/metric-spur-gear-generator/

The instructuables link is good for people who use imperial system :)
```

---
## \#61 Posted by: ervinelin Posted at: 2018-06-19T02:56:09.757Z Reads: 361

```
https://youtu.be/pN4pcO8OzJs

Here's a quick outdoor video showing how loud the gear drive is... Not sure if this is comparable to other drives out there cos I haven't heard any of them in person.

Didn't manage to go very fast either as the park was quite busy this morning.
```

---
## \#62 Posted by: Eboostin Posted at: 2018-06-19T03:26:18.075Z Reads: 354

```
Sounds slightly noisy. Is it in FOC or BLDC? 

Also, how do you like the gears compared to belts? Worth the extra hassle?
```

---
## \#63 Posted by: ervinelin Posted at: 2018-06-19T03:52:00.901Z Reads: 354

```
FOC, noise is all in the gears..

Of course the camera being right next to the motors makes it louder than it actually is.

Other than belts being quieter, I wouldn't touch belts again. Less efficient, prone to slippage, add an idler but that makes it even less efficient. Not to mention the mount becomes longer and thus needs more supports.

Really my only gripe is the noise... It's not screamer but it certainly doesn't allow me to sneak up on unsuspecting pigeons...

FYI traffic noise will drown this, as will the noise of riding on rougher surfaces. I didn't get death stares from joggers but they definitely knew I was around... (again can't ninja around with spurs).
```

---
## \#64 Posted by: Adam0311 Posted at: 2018-06-19T04:35:55.717Z Reads: 348

```
Seems like it might get a bit loud at high speeds. That said, this is sweet build and it’s yours, if the noise doesn’t bother you, then you’re good to go.
```

---
## \#65 Posted by: ervinelin Posted at: 2018-06-19T04:48:34.735Z Reads: 354

```
Yup gets a Tie Fighter squeal when it gets zippier
```

---
## \#66 Posted by: ervinelin Posted at: 2018-06-19T12:32:53.559Z Reads: 363

```
Now downsizing the AT setup back to use on flywheels...

![IMG20180619152109|690x388](upload://m0s6W1vIPA6xNZCBccyq8mbdUq7.jpg)

![IMG20180619153901|690x388](upload://i9TElsioNyz94CwFcUTpMDudRZe.jpg)
```

---
## \#67 Posted by: legend27 Posted at: 2018-06-19T13:28:26.738Z Reads: 341

```
Wow! That's some next level stuff! Good job!
```

---
## \#68 Posted by: mixedcreation Posted at: 2018-06-19T14:34:08.478Z Reads: 346

```
I find the noise good.  Unlike some ESk8's that have to be stealth for legality reasons, I like being loud or at least being heard.  I want ppl to know I am there, I don't want them accidentally riding in front of me, or jogging into my path, etc.  

BUT that is JMHO.  I know people love the quiet FOC mode setups.  I do have a hub setup like that, but I actually like that whine!  Also, I appreciate the crazy joggers giving me death stares and the kids waving, LOL!  I am a rather big kid in that way.  

In other words, I need this!  Great work @ervinelin
```

---
## \#69 Posted by: Adam0311 Posted at: 2018-06-19T17:24:14.158Z Reads: 343

```
I tend to agree about the noise...within reason. I want to be heard approaching, helps avoid potential mishaps while riding through high pedestrian traffic areas...especially near the beach. They’ve actually done studies that show loud motorcycles are statistically safer than quiet motorcycles, because motorists can hear them coming. I imagine a similar statistic could potentially be applied to louder esk8s, because pedestrians and bicyclists can hear them approaching.
```

---
## \#70 Posted by: mixedcreation Posted at: 2018-06-19T18:28:36.652Z Reads: 336

```
exactly what I was thinking when I was writing my last reply.  I had exhaust on my R6 and Ninja for that reason.  Well yeah of course performance, but mostly for a safety standpoint.  I had to make most of these fools in Northern VA aware as I battled the mindless texting fools in their SUV's.  My bike was noticeable on the streets when I needed it to be.  

Thus the reason I guess I like the noise of the esk8 boards.  Also the reason I really like BLDC.  I like the noise.  I haven't heard a board that is obnoxious, although I am no where near as skilled at building or around enough people that have been around many different boards.  So my knowledge is limited to a few chinese replica's, cheap Chinese DIY kits, boosted, evolve and a couple of solid envious builds. :slight_smile:
```

---
## \#71 Posted by: slybarman Posted at: 2018-06-19T21:06:40.331Z Reads: 315

```
What is your opinion, if you have one yet, of the board itself. How does it feel/ride? Have you ridden a Trampa or Evolve for comparison sake?
```

---
## \#72 Posted by: ervinelin Posted at: 2018-06-19T23:23:02.393Z Reads: 314

```
I agree... In fact I usually have to slow down and tell them I am passing them. But this is loud enough that they do it automatically without being alarmed.
```

---
## \#73 Posted by: ervinelin Posted at: 2018-06-19T23:27:45.177Z Reads: 328

```
I only can compare it to my other two decks and whatever esk8 I have tried. I have not ridden a Trampa so I don't know.

Compared to my jet spud and loaded tesseract this is just completely different. 

My only gripe or maybe personal preference is the lack of noticable concave where your feet touch the deck... Again my spud and Tessy have very pronounced wheel wells which give me a very solid indication of foot placement while providing a platform for me to stomp on when I need to make very tight turns.

The LaCroix however doesn't have this pronouced concave or wheel wells at the toes or heel. So i am having some trouble carving as hard as I am used to.

Compared to an AT evolve, evolve feels like a solid plank of wood... Not fun..

That aside, it's suddenly so much easier to ride without constantly having to look at the ground ahead. But that's more due to the wheels than the deck I suppose.
```

---
## \#74 Posted by: slybarman Posted at: 2018-06-19T23:32:20.471Z Reads: 317

```
Thank you for the info.
```

---
## \#75 Posted by: Wraith Posted at: 2018-07-06T04:05:42.851Z Reads: 313

```
Noob here but looking at a Lacoix complete. Their site doesn't show anything on gear drives which I think is the right move for my needs hence why I think your setup looks amazing! Is it possible to convert the DSS60/DSS50+ complete into a gear drive such as yours? @ervinelin are you able to switch sizes of pneumatics as well? Sound isn't a problem for me, I want the reduced maintenance of gear drives but would like to be able to switch from AT Pneumatics to 107mm street wheels as well!
```

---
## \#76 Posted by: ervinelin Posted at: 2018-07-06T11:52:03.906Z Reads: 319

```
Why would you think geared drives are right for you?  Gears come with their own set of problems.

As for swapping from stock to geared yes it's possible of course, just change the mounts and pullies.

As for dropping down to 107mm no, the deck wont allow it, minimally is 7" or 6" wheels with risers if I am not mistaken.

Also the geared drive will not work for 6", clearance will be poor for 7".
```

---
## \#77 Posted by: Wraith Posted at: 2018-07-06T12:40:02.088Z Reads: 325

```
Thanks for the insight! I feel that gear drives offer the least amount of maintenance as you only really need to use lubricant on the gears as opposed to swapping out belts and checking the tensioning and positioning and having the gears enclosed prevents debris from finding its way in-between the gears and damaging them. True that each drive train type has its pros and cons though I haven't seen any deal braking issues for gear drives, Just concerns with noise and the pricing. It's possible that I may not have seen any posts about frequently occuring problems with gears but I think it may also be due to the small amount of gear drives currently out right now as compared to belts or hubs.

I have yet to delve deep into DIY-ing as my budget is for the Lacroix but thats about the biggest mod I see myself doing on it so I didn't know that the mounts would need to be changed as well thanks for that.

Alright thats no problem if the 107's won't work due to clearance though not sure how someone on the forum is able to get the 107's in his photo to clear the enclosure enough off the ground(thats how I started to entertain the idea)

Could you elaborate why the 6" wouldn't work? also, clearance for 7" in terms of the height from the ground? so does that only leave 8" for it?

Appreciate the help in answering my questions!
```

---
## \#78 Posted by: ervinelin Posted at: 2018-07-06T13:00:40.238Z Reads: 302

```
I think properly setup gears should be fine.. but my 3D printed drive train might not be the most durable.

As for wheel size. Pat and Arch were the ones which said 6" might be too small (if I remember correctly).

7" clearance I meant for the gear cover, should still work but I haven't made measurements for 7" wheels.
```

---
## \#79 Posted by: Wraith Posted at: 2018-07-06T13:11:36.795Z Reads: 317

```
oh alright I understand. I think having a 3D printed drive train is really interesting and could save significant amount of cash before transitioning to a CNC version. 

As for clearance from the gear cover it shouldn't be too difficult I feel with such wide Caliber 2 trucks but You'd be the best to figure that lol I know a friend who has a 3D printer but I've got no experience using one myself though seeing your build does give me hope that it may be possible for me to do something similar! How is the ride so far and how do pneumatics feel on it as compared to urethanes? I saw your photo of converting the setup for flywheels, how did that work out?
```

---
## \#80 Posted by: ervinelin Posted at: 2018-07-06T14:10:07.962Z Reads: 327

```
These are very large pieces and takes days to print them all. Yes saves cash but I have been having some issues with them likely owing to them being not as rigid as CNC mounts.

I have the smaller version running a single drive off caliber trucks pushing 90mm flywheels. So far so good but cant expect much from single drive. Also it's my lunch time board so it doesn't do anything crazy...

![IMG20180619152110|690x388](upload://eW2ILTyiu3WKXrnNBJXM6yMskOq.jpg)

![IMG20180702204429|281x500](upload://86FVwFGtYm9P6MY8qEPolosWlpB.jpg)

8" pneumatics are COMPLETELY different from urathanes. You can just power through everything - twigs, leaves, cracks, cobble stone, manhole covers, everything! You won't even notice them!

What this translates to is not only a more comfortable ride but also a safer one without having to constantly scan the ground ahead for potential obstacles.
```

---
## \#81 Posted by: Wraith Posted at: 2018-07-06T22:52:29.406Z Reads: 310

```
[quote="ervinelin, post:80, topic:59021"]
8" pneumatics are COMPLETELY different from urathanes. You can just power through everything - twigs, leaves, cracks, cobble stone, manhole covers, everything! You won’t even notice them!

What this translates to is not only a more comfortable ride but also a safer one without having to constantly scan the ground ahead for potential obstacles.
[/quote]

This is exactly what I’ve been looking for in a riding experience! I usually have to keep an eye on the road for objects especially when riding near the curb when going through traffic or allowing cars space to go by. So swapping out the 6” to an 8” on a stock Lacroix can be done easily without having to change any pulleys? 

Sorry I thought you were making the street version for flywheels on your lacroix, my mistake. Have you gotten a hold of your CNC version for your gears? Given that there’s only a handful of gear drives available like nowind’s would using your design to have one CNC’d be cheaper to do instead of buying one from the forum?
```

---
## \#82 Posted by: ervinelin Posted at: 2018-07-06T23:57:18.592Z Reads: 305

```
6" won't fit, the gears are too big, the cover would hit the ground or be really close.

No, not planning any flywheel drives for the LaCroix again it's just too small, doesn't make sense.

No CNC version planned, sorry but I need to tighten purse strings as my second kid is here. I do plan to get them printed using a HP fusion in nylon, industrial level stuff and should be good enough for my purposes.

Also CNC only becomes cheaper if I mass produce. If I do a single piece of each of the parts it will cost me an arm and a leg.
```

---
## \#83 Posted by: Wraith Posted at: 2018-07-07T01:39:10.405Z Reads: 299

```
Alright, I may just go the 3D print route as well if it comes to it. Thanks for all the input! It's good that having the option to swap drive trains without too much trouble is there. Totally understandable that there are budget constraints for your setup as would mine be(If I'm able to place the order for a Lacroix) I'd like to experiment and try other things so the deck and enclosure will be the main stay of my build with the trucks as well while the wheels and drive train/motors I may play around abit but not till much later as the Lacroix out of the box is already such a great machine.
```

---
## \#84 Posted by: philvanzu Posted at: 2018-07-07T05:45:24.418Z Reads: 297

```
Huge respect for this build it's really impressive, but beltless transmissions come with their own set of problems and when they happen you're in for a lot more work than changing a belt or greasing a chain. I for one have yet to be convinced they are that big an upgrade, considering the cost, the noise and the added complexity.
Look at these pics for example by @DavidC 
http://e-sk8.fr/forum/viewtopic.php?f=29&t=2698&start=30

It's totally possible to put 107mm wheels on the lacroix deck, It's just that you would put the deck 1.5 inches below it's recommended height, so you would need 1.5 inches of risers to compensate, angled or not depending on the trucks you wanna use.
```

---
## \#85 Posted by: Adam0311 Posted at: 2018-07-07T06:37:13.695Z Reads: 299

```
I’m also intrigued by the geared drive. @Nowind and @ervinelin make them look sexy, but if I’m honest with myself, I’d admit that its more want than need. Especially on the LaCroix which is designed to be a urban cruiser/carver, not a mountain board kicking up dirt and rocks on every turn. 

I’ve been riding esk8s for over 2 1/2 years (urban environment only) and in that time, I’ve only had one belt break while I was riding...it was 9mm belt on my dual raptor 1. I was still able to to ride home safely and it took me about 1 min to replace the belt and restart my ride. 

My point is...I get where you’re coming from, I too drool over the geared drive train (especially the helical gears!!!), but we are both likely over thinking our needs for LaCroix board, belts may not be sexy, but they are cheaper, lighter, easier, and most importantly they simply work.
```

---
## \#86 Posted by: Wraith Posted at: 2018-07-07T06:38:35.847Z Reads: 286

```
Thanks @philvanzu. I tried translating the page via Google and from what I understand, the dust and pebbles were lodged between the housing  and wheel causing the laceration? I'm reconsidering my plans for going with 107mm wheels due to that clearance now. My concern with belts is that I'd lose control over the brakes and acceleration should it happen to snap while I'm out riding although I do know how to foot brake, It would be one less things to worry about. I don't own a belt drive at the moment so I don't have first hand experience with long term maintenance with them until I can pull the trigger on the Lacroix.
```

---
## \#87 Posted by: ervinelin Posted at: 2018-07-07T06:50:00.570Z Reads: 277

```
I agree belts work percectly fine.. add an idler and you almost won't have any issues with brakes anymore.
```

---
## \#88 Posted by: philvanzu Posted at: 2018-07-07T07:00:31.530Z Reads: 285

```
Your translation is right, and he also says that he's got some kind of sealing joint problem, grease leaking out and dust coming in, aligning the gears is very difficult making maintenance a hassle and that in the end the direct drive is in no way bullet proof.
The only problems I ever had with belts is I had to replace the cheap HTD3M coming with my leiftech because the teeth werent strong enough. I replaced with Gates belt, and they are still as new one year later. You just need to ensure they are not too tense and correctly aligned then the wear stays very limited.
```

---
## \#89 Posted by: Wraith Posted at: 2018-07-07T07:09:00.821Z Reads: 288

```
From what I've read this allows consistent tension across but doesn't this increase wear on the belt due to higher tension? given the @philvanzu uses quality Gates belts for over a year that makes just sticking to belts out of the box much more promising.
```

---
## \#90 Posted by: philvanzu Posted at: 2018-07-07T07:20:11.234Z Reads: 287

```
Idlers increase the amount of teeth that are engaged in the pulleys, which is good to prevent slippage at a given tension, allowing you to slacken the tension a bit, and that's better for longevity.
```

---
## \#91 Posted by: ervinelin Posted at: 2018-07-07T07:31:21.463Z Reads: 297

```
For what it's worth, if you want a solution u know will work, go with belts.. tried tested proven

Gears can end up giving you more trouble if not setup correctly
```

---
## \#92 Posted by: Wraith Posted at: 2018-07-07T08:10:06.023Z Reads: 305

```
@philvanzu Oh now I understand it better so theres better contact for the pulleys and belts! @ervinelin right its still fairly new to esk8 and I think I may be better off using belts until gear drives become more tested and proven then I can switch the Lacroix belts over to gears. Lots more support as well in the forum from builders like you guys now that I realize it.
```

---
## \#93 Posted by: azninferno Posted at: 2018-07-17T15:47:29.025Z Reads: 302

```
Would love to see the STL files for everything.  Great build/thread!
```

---
## \#94 Posted by: ervinelin Posted at: 2018-07-23T15:34:50.666Z Reads: 307

```
![IMG20180723215006|690x388](upload://maAKYeNAQpq81dSKv7EO9gGhiQQ.jpg)

![IMG20180723215703|690x388](upload://seyJ7hnSdiEBnGqJ4xJcMOJVXvt.jpg)

Preparing to upgrade my dual drive Tesseract to geared drive as well... Swapped to 15/41 instead of 12/41 on my single drive..

Also planning to use 15/71 instead of 12/71 on the LaCroix...
```

---
## \#95 Posted by: Hogo Posted at: 2018-08-01T11:21:59.429Z Reads: 288

```
Hello, are you able to use the clamp style light mount on the front trucks as well? I’m getting ready to order prints of your mounts but was hoping I could order that style for both front and rear trucks. Thanks! Great work all around by the way.
```

---
## \#96 Posted by: ervinelin Posted at: 2018-08-01T11:33:44.307Z Reads: 291

```
Should work on front as well but I suggest printing the slide on ones instead, the clamped ones I THINK are offset to account for the motors.
```

---
## \#97 Posted by: ervinelin Posted at: 2018-08-10T17:08:58.051Z Reads: 296

```
![IMG20180809034555|281x500](upload://vB1z8vXQPm0dVXhMJsqdFrIl9GQ.jpg)

![IMG20180809213706|690x388](upload://hMarffj0TdUtf1y2VwyjmbNxW4B.jpg)

Trying out HP fusion Nylon PA12 prints... So far very promising for the gears...
```

---
## \#98 Posted by: skatardude10 Posted at: 2018-08-10T17:39:17.773Z Reads: 290

```
Been drawing up some designs myself... I see metal motor gear, but assuming I get one of those, in general how do you think a nylon motor gear on nylon wheel gear would fare?
```

---
## \#99 Posted by: ervinelin Posted at: 2018-08-10T17:56:14.748Z Reads: 288

```
Problem with plastic on the pinion is that I don't think they will take the torque the motor puts out.... I might be wrong but I much rather stick to metal on nylon...
```

---
## \#100 Posted by: Trdolan03 Posted at: 2018-08-16T22:47:30.374Z Reads: 287

```
Where did you source a gear with 8mm note?
```

---
## \#101 Posted by: ervinelin Posted at: 2018-08-17T05:33:15.322Z Reads: 279

```
Here [2pcs Spur Gear pinion 15T 15Teeth Mod 1.5 M  http://s.aliexpress.com/ZVFVRJjm?fromSns=Copy to clipboard](2pcs Spur Gear pinion 15T 15Teeth Mod 1.5 M  http://s.aliexpress.com/ZVFVRJjm?fromSns=Copy to clipboard)
```

---
## \#102 Posted by: ervinelin Posted at: 2018-08-17T13:17:24.800Z Reads: 278

```
[https://youtu.be/yG2-4DqIaEU](https://youtu.be/yG2-4DqIaEU)

HP fusion dual geared loaded Tesseract works well! Now to upgrade the LaCroix!
```

---
## \#103 Posted by: ervinelin Posted at: 2018-08-27T08:59:54.811Z Reads: 280

```
Upgraded the gears and mounts to HP fusion PA12. I think it got slightly quieter.

Definitely feel safer than riding around in FDM 3D prints!

![IMG20180827134741|281x500](upload://8ijs3RESastvBUCO4Wwc57IVCFf.jpg)

![IMG20180827134752|690x388](upload://rw9x8S5HUkrpRZ2mbWvLLzmPcCq.jpg)

![IMG20180827135311|281x500](upload://lLtJGgjbVk5P6IDtj37obEgdz6m.jpg)
```

---
## \#104 Posted by: aethyr Posted at: 2018-08-28T06:05:39.899Z Reads: 265

```
I tried polycarbonate motor gear on polycarb wheel and the motor gear wore out in 1 day. Polycarb can handle the force/stress, but it can't handle the friction.
```

---
## \#105 Posted by: Riako Posted at: 2018-08-28T08:58:21.119Z Reads: 262

```
**Awesome build man !!!**
Congrat, it looks just perfect & thanks for all the tips and sharing here :+1: :+1: :+1: 
https://media.giphy.com/media/eZRdEIzkAM3gk/giphy.gif
I stay close !
```

---
## \#106 Posted by: Dr.Octogon Posted at: 2018-08-28T10:08:13.499Z Reads: 257

```
Yea, you need Nylon for the friction. NylonX is reinforced with Carbon fiber. Regular Nylon should work as well.
```

---
## \#107 Posted by: ervinelin Posted at: 2018-08-28T11:03:25.558Z Reads: 257

```
Not even with lube?
```

---
## \#108 Posted by: Mobutusan Posted at: 2018-08-28T15:29:31.152Z Reads: 247

```
[quote="ervinelin, post:107, topic:59021, full:true"]
Not even with lube?
[/quote]

As my wife would say, not a chance in hell. :kissing_heart:

Sorry, I just had to.
```

---
## \#109 Posted by: ElectricCoast Posted at: 2018-08-31T11:22:59.185Z Reads: 239

```
How are you gears holding up so far?
```

---
## \#110 Posted by: ervinelin Posted at: 2018-09-01T23:57:08.635Z Reads: 236

```
Holding up fine for my style of riding...
```

---
## \#111 Posted by: ElectricCoast Posted at: 2018-09-03T19:05:06.343Z Reads: 242

```
What board is that you built with the all natural finish?
```

---
## \#112 Posted by: ervinelin Posted at: 2018-09-04T00:03:32.256Z Reads: 246

```
You mean this? 

![IMG20180902122807|690x388](upload://h6m5IYMgbDEsqtWwh5qfgl8tRGH.jpg)

It's my new mini AT build thats still in progress. The deck is actually a bamboo skateboard 8.5" that I cut off a bit of the kicks and mounted the TB 218 on them with custom risers.

https://bambooskateboards.com/skateboards.html

Here's how it looks beside the LaCroix.

![IMG20180901075602|281x500](upload://1aRJka1eHvbjcf27NjvbqTSzn85.jpg)
```

---
## \#113 Posted by: ElectricCoast Posted at: 2018-09-04T05:52:26.388Z Reads: 233

```
Yep thats the one.  I recognized the wheels as the 6" set from alibaba I think they're about $16.00 each and I suspected that those were TB218's.  Forgive my igorance but where did you get the adapaters for the trucks?  I'm still pretty new to this e-board scene.
```

---
## \#114 Posted by: jaatis Posted at: 2018-09-04T07:09:40.647Z Reads: 231

```
The truck risers/adapters look 3D-printed @ElectricCoast

Rally amazing stuff here @ervinelin! Did you ever experience any breakdowns with the FDM printed gears?

Would definitely like to see more on the mini AT build. Seems like the ultimate DIY AT board. How is the bamboo skateboard deck like?
```

---
## \#115 Posted by: ervinelin Posted at: 2018-09-04T08:02:03.025Z Reads: 227

```
Adapters are DIYed... as are the gears and angled riser...
```

---
## \#116 Posted by: ervinelin Posted at: 2018-09-04T08:03:43.809Z Reads: 235

```
I've stopped using FDM printed gears and swapped to HP Fusion printed ones instead, much sturdier... also more expensive.

I supposed if my printer could print nylon it might have been better.

Yes risers are printed.

Bamboo deck is nice and bouncy... will have to wait and see about the durability and ride... I did use it as an esk8 deck previously but didn't really like it back then because the wheels were too small.
```

---
## \#118 Posted by: Organisedrhyme Posted at: 2018-09-16T03:16:08.313Z Reads: 230

```
Hi there, Absolutely awesome build and inspired me todo similar - hence a quick question. I have a lacroix stock full build OTW but am looking to change it to a helical gear drive from e:Toxx. Whats the easiest way to change the motor setting to invert without overwriting all the stock lacroix settings in the FOCBOX? WOuld it be just to do it in software (VESC tool or FOCBOX tool?) as I also wnna keep it in FOC mode. Am pretty new to the whole VESC stuff so nervous about accidently writing over something. As all i want to do is to be able to read the current FOCBOX settings and just “invert direction” without touching anything else. 

Thanks in advance!
```

---
## \#119 Posted by: ervinelin Posted at: 2018-09-16T03:51:09.552Z Reads: 227

```
I think you need to swap the motor leads. Then run the motor calibration again to make sure everything is in order. 

Most other settings you can leave alone. I recommend you read up more about setting up the vesc first. It's not rocket science but it can be daunting when u first do it.
```

---
## \#120 Posted by: philvanzu Posted at: 2018-09-16T08:47:57.520Z Reads: 220

```
There's a setting to invert motor direction under Motor Settings / General.
Just read motor config, reverse direction then write motor config, repeat for the second focbox and you're set.
```

---
## \#121 Posted by: ervinelin Posted at: 2018-09-16T09:00:02.535Z Reads: 236

```
Some people have reported issues when doing this in some versions of the software. 

I typically would just swap the leads and redo the motor calibration.
```

---
## \#122 Posted by: ervinelin Posted at: 2018-09-17T23:41:59.930Z Reads: 241

```
So I made myself a mini rolling fortress...

![IMG20180918020634|666x500](upload://tWYomzzbiEySoIQtNTkRp2npaeb.jpg)

![IMG20180918012708|690x388](upload://cLP3RonF7cM0CTrOtvP7i0J3Hhu.jpg)

![IMG20180918013920|690x388](upload://tRnuNPKrRTvSKNeybEXfA5ngaFf.jpg)

![IMG20180909113353|281x500](upload://eH0wM9xZdp3aeRK2kvP8Kxk7nES.jpg)

![IMG20180909112849|690x388](upload://sJki7UtJuOZ6qVCzCdAcQrqQFWm.jpg)

Will create a thread for it by itself soon...
```

---
## \#123 Posted by: BOOSTEDO Posted at: 2018-09-18T03:45:11.683Z Reads: 233

```
I had a friend print out two sets of the stl files for the light mounts...
Two one piece and two four piece mounts. None of them worked...
Your trucks are matrix pro ii but my Lacroix came with matrix ii trucks (non pro)
Is that the difference? I thought the only difference was the hollow axel but maybe
you uploaded the wrong stl files??
```

---
## \#124 Posted by: ervinelin Posted at: 2018-09-18T04:06:35.475Z Reads: 229

```
They don't work? Odd... Mine are the hollow axel but that's just the axel.

In what way do they not work, the profile is different? From my understanding it's the same, heck I have seen people using my mount on their stock LaCroix.

STL's cant be wrong, again I've seen people using them. Got a photo of yours?
```

---
## \#125 Posted by: BOOSTEDO Posted at: 2018-09-18T07:27:32.566Z Reads: 231

```
![image|374x500](upload://wiKtMUeXAJE1R2N2JzahNXrPjcG.jpeg)

I dunno what gives but they will not slide onto the axel...(the one piece) and to add insult to injury the two piece won’t clap either...
I gotta admit this DIY stuff will keep you on your toes... Maybe my matrix II trucks are like rejects or something... well at least I got the evolve tires on... Give Thanks
```

---
## \#126 Posted by: ervinelin Posted at: 2018-09-18T08:04:27.968Z Reads: 214

```
Can u take a photo of them next to the truck?
```

---
## \#127 Posted by: xilw3r Posted at: 2018-09-18T10:33:47.519Z Reads: 224

```
Your friends printer might not be calibrated. Did you measure the parts? does not take much to prevent parts from fitting on your trucks

@ervinelin very nice build. What fillament are you using for you mini fortress? Have you tried pla/ petg for gears?
```

---
## \#128 Posted by: ervinelin Posted at: 2018-09-18T10:38:02.262Z Reads: 217

```
I started with PLA2.0 (some call it PLA+) but have since sent it out to get printed my a HP fusion jet in nylon PA12
```

---
## \#129 Posted by: nuttyjeff Posted at: 2018-09-18T11:04:27.749Z Reads: 220

```
fancy fancy~
```

---
## \#130 Posted by: BOOSTEDO Posted at: 2018-09-28T06:50:36.593Z Reads: 216

```
@ervinelin I finally flipped the trucks and everything worked(as you already know from the Lacroix thread).... The flipped modified ones are gonna be printed soon as well as the concave inserts...
You deserve a DIY medal!!!:+1:t6:


**Funny Story:** I was on my way home from Bronx HQ aka @Kaly Shop and I had my Evolva headlights on and my front mounted Xanes (Red/White flashing) chilling at a red light when an undercover cop car sped past me and up the block (Red/White lights flashing) - Then from out of traffic another one came right at me - hit the brakes and the driver had this confused look on his face!!!! I gestured _**thataway**_ and the cop nodded his head and took off up the block... Took me a couple of seconds to realize that the Evolva Lights look like car headlights and with the Xanes flashing Red/White they must've thought I was the other undercover cop car they was following... :laughing::laughing::rofl::rofl::rofl:

Peace...:v:t6:
```

---
## \#131 Posted by: ervinelin Posted at: 2018-09-28T07:00:39.783Z Reads: 213

```
Cool story...

Let me know if the concave works for you, I'm still uncertain as to how thick they need to be.

As for the flipped holders, please print one first to test... I flipped the model based on what I THINK should be correct, but I might have gotten the mirror axis wrong.
```

---
## \#132 Posted by: skslingo21 Posted at: 2018-09-29T12:17:54.956Z Reads: 200

```
Do you own the hp fusion? @ervinelin
```

---
## \#133 Posted by: ervinelin Posted at: 2018-09-29T12:30:03.577Z Reads: 200

```
I wish... 10char
```

---
## \#134 Posted by: ervinelin Posted at: 2018-11-25T01:26:11.959Z Reads: 182

```
Rolling Fortress Meets Kushboard Titan

https://youtu.be/8zSD96h8o9I

Having fun with my new Insta360 One X camera.. it's awesome...
```

---
## \#135 Posted by: TheArus Posted at: 2019-02-17T23:28:22.543Z Reads: 144

```
Are you going to share STL files for direct drive? Or can I buy it from you?
```

---
## \#136 Posted by: BuddyPR Posted at: 2019-05-15T10:24:25.864Z Reads: 102

```
I have the original tucks that comes with the LaCroix, would you print and sell a pair or mounts for the bang oof front and back light?
```

---
## \#137 Posted by: ervinelin Posted at: 2019-05-15T11:05:31.954Z Reads: 104

```
You can download them and print them yourself. No sense sending them halfway across the world.
```

---
## \#138 Posted by: Adstars Posted at: 2019-05-16T04:24:27.336Z Reads: 97

```
I've printed headlights mounts modded for the MBS trucks, happy to share the file.

I used flexible filament, at 80% infill
![IMG_20190324_120521|666x500](upload://m9dkRQG9pFeVcBayiFHPmznIehd.jpeg)
```

---
## \#139 Posted by: Vagner Posted at: 2019-07-11T00:25:51.856Z Reads: 69

```
Olá, boa noite.
Onde compro as baterias igual a que você tem?
```

---
## \#140 Posted by: Grozniy Posted at: 2019-07-11T22:26:10.461Z Reads: 64

```
Aqui tem que falar em inglês. Ninguém lhe consegue ajudar em português.
Essa bateria é feita à mão com várias celulas individuais. Não sei onde se pode comprar no Brasil. O mais simples é comprar baterias LiPo.
```

---
