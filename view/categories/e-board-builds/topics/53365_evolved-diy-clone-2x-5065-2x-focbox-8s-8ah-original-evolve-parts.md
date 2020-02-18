# EVOLVED &#124; DIY Clone &#124; 2x 5065 &#124; 2x FOCBOX &#124; 8s 8ah &#124; Original Evolve Parts

### Replies: 45 Views: 3611

## \#1 Posted by: fraannk Posted at: 2018-04-24T17:56:15.639Z Reads: 446

```
Alright. As some of you might have noticed I like the looks of certain prebuilds. Especially Boosted and Evolve. But as I'm not satisfied with their performance I build clones with better specs. Here we go again! I fell in love with the Evolve Bamboo GT and I simply didn't like the way it accelerated (and the remote #triggersdisgustme). I then discovered that you can buy all the needed parts for a build, except all the electronics of course, straight from Evolve. And that was perfect for me as I then could DIY the heck out of it, and get my beloved VESC's in it. You've probably seen me post some small teasers in the pictures thread!! 

**Parts list:**
Evolve Supercarve Trucks
Evolve Bamboo GT deck + enclosure
Orangatang Kegels
5065 motors from Banggood
2 FOCBOX's (ty @BoostedBuilder) 
15/32 drive train 
4x Zippy 2s 8ah batteries (why do they not make 2s 8ah Graphenes??)
Nano-X remote
Anti-Spark switch

**Some pictures:** 
Workshop :arrow_down:
![IMG_1780|666x500](upload://5g4ipMY0QMvkHpi1eXu0HE1BlBD.jpg)

Tight fit :arrow_down:
![IMG_1760|690x388](upload://1YU395IqyY4lxV3KZiTbFllbsy4.jpg)  
![IMG_1789|690x388](upload://5mZMMU6WYl3MVAuwdyLQgERZzRx.jpg)

The baby in all it's glory :arrow_down:
![IMG_8250|666x500](upload://wqI2ck8PyNWQ1fPjAGQRTXQ8268.JPG) 
![IMG_7408|666x500](upload://mYyKH2ZuNtwhOlksstOZYKQQffO.JPG)

For now it's ridable, but there's some minor stuff I still want to do: 
:pushpin: Add my custom balance connector (v2) 
:pushpin: Add LED strips, headlights, taillights and controller
:white_check_mark: Refine and rewire the battery wires (fkn 8awg) 
:white_check_mark: Upgrade to FOCBOX'es 
:pushpin: Get an AT kit 
  
Hope you like it!! There's also an update for my [Boosted clone](http://www.electric-skateboard.builders/t/the-frankenboard-loaded-vanguard-dual-6355-dual-vesc-8s-10000mah-orangatang-kegels/20510) real soon, as (also) seen in the pictures thread :D
I'm refurbishing my boards so they're ready for summer :sunglasses:
```

---
## \#2 Posted by: myreala Posted at: 2018-04-24T18:07:48.464Z Reads: 389

```
I am surprised those massive lipos fit in that enclosure. Did you do any modifications to get them to fit? Do you have space for them to puff? Afaik lipos fuff about 15% when put under heavy load. 
Edit: So looks like they are only 15mm in height, that's very good. How are you planning to charge them?
```

---
## \#3 Posted by: fraannk Posted at: 2018-04-24T19:35:17.617Z Reads: 359

```
Right now I'm charging them individually. But I'm planning to integrate my charging system I have across all my boards. A power connector and a custom balance connector, connected to my 10s balance charger. :) I added some rubber gasket to raise the battery case a bit :)
```

---
## \#4 Posted by: BoostedBuilder Posted at: 2018-04-24T20:36:07.695Z Reads: 339

```
Aren't you worried about the flex of the board?
```

---
## \#5 Posted by: fraannk Posted at: 2018-04-24T20:36:53.352Z Reads: 328

```
What's to be worried about? :) It doesn't flex that much either
```

---
## \#6 Posted by: BoostedBuilder Posted at: 2018-04-24T20:40:29.587Z Reads: 327

```
The Li-po's are placed horizontally and not vertically (depends on the way you look at them but I think you get my point) so they'll be taking any slightest flex. I don't know if there is any room for them to move when the deck flexes but to me it kinda looks a little worrying.

Hope I'm wrong cause it looks nice!!
```

---
## \#7 Posted by: fraannk Posted at: 2018-04-24T20:44:30.748Z Reads: 315

```
Yeah, I thought about that, but after I added the rubber gasket, theres a tiny bit of room for the batteries to move. Also, the board does not flex enough to bend the individual cells. It would probably be a problem if I heatshrinked all the batteries together. :)
```

---
## \#8 Posted by: BoostedBuilder Posted at: 2018-04-24T20:46:05.145Z Reads: 299

```
[quote="fraannk, post:7, topic:53365"]
theres a tiny bit of room for the batteries to move
[/quote]
Then it's perfect!

Do you prefer the look of the bamboo over the GTX?
```

---
## \#9 Posted by: fraannk Posted at: 2018-04-24T20:49:05.915Z Reads: 287

```
Yes, I like the light, beachy look, especially since my Vanguard has black grip tape on it :slight_smile: 
I know the GTX has a cutout, but I really wanted this look :D
```

---
## \#10 Posted by: chris.hunt Posted at: 2018-04-25T06:53:18.469Z Reads: 268

```
what’s the range like on this setup
```

---
## \#11 Posted by: fraannk Posted at: 2018-04-25T07:37:48.201Z Reads: 270

```
I haven't tried riding until empty yet, but my initial calculations give me around 22-24 km :D
```

---
## \#12 Posted by: fraannk Posted at: 2018-04-30T05:40:35.412Z Reads: 266

```
Rewiring, and replacing 8AWG with 10AWG:

![image|374x500](upload://30NZaHZkveYVzjEdgLMPprrfZK5.jpeg)
```

---
## \#13 Posted by: fraannk Posted at: 2018-05-02T16:44:38.347Z Reads: 257

```
Alright, so I was on a fairly long ride and near the end of the ride, I tried accelerating rapidly and I felt at least one of the VESC's cutting out. I checked the metr log, and the fault code was DRV8302. What causes this? Both VESC still works perfectly fine, and I'll try accelerating rapidly again, when the board has recharged. I have also accelerated hard on full charge and there were no problems. :) 
https://metr.at/r/Arb36 
DRV fault at 18:08:44
```

---
## \#14 Posted by: pjotr47 Posted at: 2018-05-02T17:41:25.884Z Reads: 248

```
What settings do you use for the vesc's?
```

---
## \#15 Posted by: Bjork3n Posted at: 2018-05-02T17:57:36.568Z Reads: 251

```
Maytech vesc? Had similar issue, went away when I changed to focboxes.

Change battery max to maybe 25A each vesc
```

---
## \#16 Posted by: fraannk Posted at: 2018-05-03T19:10:30.734Z Reads: 248

```
Tried riding again today. There's no problems when it is fully charged. I can hammer it as much as I want. Only when the battery get's to around 30v (3,75v per cell) I get the error codes when accelerating hard. And only on one of the VESC's. I'll try changing the settings a bit, but it's really weird, because I used these VESC's on my other board with 63mm motors, and there I pulled a lot of amps compared to this board. Only difference is 50mm motors with sensors compared to 63mm without sensors, and the firmware. (ack 3.101 vs stock 2.18)

Settings are all stock except of the following: 
Motor detection parameters
App setting parameters
Motor max: 47a
Motor min: -47a 
Battery max: 40a
Battery min: -15a

Maybe it's just getting a little worn out. I used the VESC for (probably a lot) more than 1000km :)
```

---
## \#17 Posted by: fraannk Posted at: 2018-05-08T10:34:54.763Z Reads: 233

```
Lowered the battery max to 30a, no problems so far :) the most I have ever pulled on a board is 32a (per VESC) anyways...
```

---
## \#18 Posted by: fraannk Posted at: 2018-06-02T11:53:19.441Z Reads: 221

```
Upgraded to FOCBOX’es, and now it runs in FOC! :sunglasses:  
![image|666x500](upload://gOJGVJ68NkYcnyTV3S66r34j2vJ.jpeg)
```

---
## \#19 Posted by: Guacamoleface Posted at: 2018-06-02T12:06:18.022Z Reads: 213

```
What Vesc settings do you currently run thoose motors on? :)
```

---
## \#20 Posted by: fraannk Posted at: 2018-06-02T12:10:58.833Z Reads: 209

```
The specs say max 47 motor amps, but I just upped that to 50a, so let's see how that goes :) battery current max 40a :)
```

---
## \#21 Posted by: Guacamoleface Posted at: 2018-06-02T12:23:36.462Z Reads: 198

```
Im doing a similar build but I built myself a 10s4p 30Q pack for the batteries, and I use the 140kv motors :) wanna see how they perform, hopefully I get done today!
```

---
## \#22 Posted by: fraannk Posted at: 2018-06-02T12:26:35.285Z Reads: 196

```
Nice! I'm upgrading to the same kind of pack when these batteries doesn't cut it anymore (and when I get the funds)
```

---
## \#23 Posted by: fraannk Posted at: 2018-06-02T13:29:09.763Z Reads: 204

```
Sweet baby Jesus sensored FOC is the FOCin' sh*t!! 

https://d3vv6lp55qjaqc.cloudfront.net/items/3u1C2w2S1l2c3u442I1g/IMG_1922.TRIM.MOV

Did a little test cruise and it works amazing! Measured the temperature of the motors as fast as possible after the ride, and they were only 46 degress celsius. Considering that it is 30 degrees celsius, and full scorching sun today, on the black motor cans, I think that's pretty good.

https://metr.at/r/vuY6x
```

---
## \#24 Posted by: Guacamoleface Posted at: 2018-06-02T13:55:47.070Z Reads: 190

```
Nice! Charging mine now and then its just the programming left :heart_eyes: 
Btw do you run sensored?
```

---
## \#25 Posted by: fraannk Posted at: 2018-06-02T14:14:01.628Z Reads: 184

```
Yup! Smooth AF
```

---
## \#26 Posted by: Guacamoleface Posted at: 2018-06-02T14:25:37.155Z Reads: 179

```
Oh, can you show me how its gonna be rewired, if it doesnt require you to open your enclosure ofcourse :)
```

---
## \#27 Posted by: fraannk Posted at: 2018-06-02T14:37:47.282Z Reads: 184

```
What do you mean? :)
```

---
## \#28 Posted by: Guacamoleface Posted at: 2018-06-02T14:58:38.856Z Reads: 183

```
You had to re-wire the sensor cables to the JST to fit the focbox right? :)
```

---
## \#29 Posted by: fraannk Posted at: 2018-06-02T15:03:00.412Z Reads: 187

```
Oh, I already did that before I upgraded to FOCBOX'es. It's the same as on the MayTechs VESC's. The important part is the 5v and GND, the rest doesn't matter. (as long as there's no temp sensor) :) 

The green wire on the right in the image, goes to the red one on the motor. :) 
![IMG_6552|375x500](upload://69IPM2PwSXdO9XObBMMrGqW1npd.JPG)
```

---
## \#30 Posted by: Guacamoleface Posted at: 2018-06-02T15:03:53.747Z Reads: 186

```
Cool appriciate it! thanks! :)
```

---
## \#31 Posted by: Guacamoleface Posted at: 2018-06-03T11:33:44.594Z Reads: 178

```
You along with the weather motivated me to finish mine aswell ;) 
Thanks for the help with sensorcables!

First testrun! 

https://youtu.be/KgwtoZKH-S4
```

---
## \#32 Posted by: fraannk Posted at: 2018-06-24T14:18:37.247Z Reads: 159

```
**F I N A L L Y** found a perfect connector for balancing! I’ve been looking everywhere for a 11+ pin connector that was not too big and looked pretty. I found the Hirose HR10A connector in China, and it’s even a push pull connector 😍😍😍
![image|375x500](upload://gA6YuCT8rVH8GPeWZOt3nK0dBgX.jpeg)
It fits nicely in the evolve enclosure :+1:
```

---
## \#33 Posted by: totalgeek9224 Posted at: 2018-10-04T07:28:20.727Z Reads: 128

```
Awesome looking build!
```

---
## \#34 Posted by: fraannk Posted at: 2018-10-04T08:27:00.071Z Reads: 141

```
Expect an update Saturday or Sunday :sunglasses:
```

---
## \#35 Posted by: fraannk Posted at: 2018-10-10T18:42:23.028Z Reads: 138

```
# A little story... 

A peaceful day when I was making my new charging connector system, the disastrous thing happened. While building it, I wanted to check if I had soldered all the connections correctly, so I got my multimeter and started measuring. Oh boy was that a mistake. A little PSA is; measure the connections for continuity instead of measuring the voltage on a connector connected to the battery. My hands were shaking just a fraction too much, and I touched two (maybe more) of the pins, shorting the balance connector. Hell broke loose and the connector was suddenly a flame of about 30cm instead. 

I was thinking "shitshitshitshit what do I do.." and in the panic I put the flaming board out on my balcony. Problem is that I live on 8th floor so this was extra scary. However the problem was not dealt with yet, as now there was a board on fire on my balcony. Luckily I had a fire extinguisher with powder so I could put out the fire. Damn. Scary stuff. 

![IMG_2040|666x500](upload://ztAyHDZCb4GwcCQeCMDmR0vhLT3.jpeg) 

The deck itself took some damage, but I was able to repair it by sanding it down, getting a new foam mat from Evolve, and repainting the back side (now in matte black instead of glossy :heart_eyes:) (Sorry, no pic of the fresh deck)

![IMG_2099|374x500](upload://gmu8jFTtwwpVlztoCCFDaxX5AkG.jpeg)  

Alright, so the connector was no more, so I went back to my trusty VGA connector, but I revised the design and made a 2.0 version of both the board side and the cable side. (My other build [The Frankenboard](https://www.electric-skateboard.builders/t/the-frankenboard-loaded-vanguard-dual-6355-dual-focbox-8s-10000mah-orangatang-kegels/20510/93?u=fraannk) got this update as well). Came out great! (and no fires :wink:) Already a little dirty. :hugs:

![IMG_0059|666x500](upload://5KDN2phYeodYjNbMO15gKx41D30.jpeg) 

While is was at it, I refined the internals completely. I got the custom FOCBOX heatsink from @BoostedBuilder and it is just fantastic. Takes the build to a whole other level. :heart_eyes: 

![IMG_2115|666x500](upload://8zzhVt3VBtaQJqXM2plX5nSzrwi.jpeg) 

I also redid all the internal connections for easier disassembly and reassembly. 
As you probably noticed if you've been following the thread, I got some AT wheels as well. So here's some pictures of the final build. :tada:

![IMG_0056|666x500](upload://hH1I5svgZBMxwbgc1aCqiR74I6s.jpeg) 
![IMG_0057|666x500](upload://rTuYP2CHZWJ1E7iYTYnsz62YUKE.jpeg) 
![IMG_0058|666x500](upload://1Bjro6L6fiPpArkdtTA2k5k2KTH.jpeg) 

As you can see, I 3D printed a riser for the enclosure, and while it not only looks good, it makes everything fit snug and perfect. While I was at it, and since my trucks didn't come with the "GT" logos inserted, I also 3D printed my own logo for a personal touch. These is spray painted in chrome silver :D 

![Untitled|375x500](upload://56M6p6JmimV65dlyOqV31f1U8I.jpeg) 

Thanks for following :D
```

---
## \#36 Posted by: pjotr47 Posted at: 2018-10-10T19:21:52.932Z Reads: 125

```
Ho boy, that hurts to see such a photo :confused:
```

---
## \#37 Posted by: b264 Posted at: 2018-10-10T20:22:45.006Z Reads: 123

```
So, how's that performance compare to a genuine Evolve?  :smirk:
```

---
## \#38 Posted by: fraannk Posted at: 2018-10-10T20:33:48.907Z Reads: 122

```
I've only tried an Evolve once, and fell off on the non-smooth accelleration, it really jerked away under my feet... so I can't say. :)
```

---
## \#39 Posted by: b264 Posted at: 2018-10-10T20:34:29.220Z Reads: 120

```
Well I was poking fun.  The VESC are way better.
```

---
## \#40 Posted by: fraannk Posted at: 2018-10-10T20:35:00.641Z Reads: 119

```
I thought so ;)
```

---
## \#41 Posted by: PickSix24 Posted at: 2018-10-12T00:46:46.502Z Reads: 111

```
 Nice build ! How’s the fit on your 3d printed riser ? I had one printed from files I found online but the fit / finish is bad. Anyway you could share your files or charge me to print one for me ?
```

---
## \#42 Posted by: fraannk Posted at: 2018-10-12T12:55:48.113Z Reads: 101

```
I found this on thingiverse, but I had to print it at 101% scale to make it fit perfectly. :) To get this finish I sanded and painted it
```

---
## \#43 Posted by: PickSix24 Posted at: 2018-10-13T21:11:23.076Z Reads: 99

```

https://www.thingiverse.com/thing:2965134
Is this the one ? If it is maybe I’ll try having it printed at 101%. Mine required a lot of enlarging the holes and some of the side pieces bulge out.
Also did you print in PLA or ABS ?
```

---
## \#44 Posted by: fraannk Posted at: 2018-10-13T21:28:26.017Z Reads: 93

```
Yup, exactly that one. I printed in 101% scale with a 0,6mm nozzle, using PLA material.
```

---
## \#45 Posted by: ElectricCoast Posted at: 2019-10-17T20:18:50.103Z Reads: 27

```
I have a friend that has a Evolve GT that he ran into the water by accident.  Needless to say I am having to source a new vesc x2 and BMS for him.  The battery is ok.  My question for you all since I know nothing about Evolve is can you use the remote and pair it up to another receiver?  I'm trying to save my buddy some money if I can.
```

---
