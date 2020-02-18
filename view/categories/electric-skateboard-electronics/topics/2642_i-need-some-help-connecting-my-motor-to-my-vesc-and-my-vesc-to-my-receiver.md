# I need some help connecting my motor to my vesc and my vesc to my receiver

### Replies: 71 Views: 8210

## \#1 Posted by: eskateking Posted at: 2016-04-27T04:17:31.971Z Reads: 445

```
<img src="/uploads/db1493/original/2X/2/26385d9423a5dfbfdf1c81a25218723756d56da2.jpg" width="690" height="388">
<img src="/uploads/db1493/original/2X/f/f0f567b53e347a97b4b69c14a73f3faf8f0a7f78.jpg" width="690" height="388">
<img src="/uploads/db1493/original/2X/d/d25f3568de0d87b505ff2e9eca05ec5a39fdcbff.jpg" width="690" height="388">

So these came with my motor. Not sure what they are. The motor wires don't fit into them.

Thank You for the help.
```

---
## \#2 Posted by: eskateking Posted at: 2016-04-27T05:09:32.932Z Reads: 416

```
I used a motor by @onloop and a vesc by @chaka
```

---
## \#3 Posted by: onloop Posted at: 2016-04-27T05:10:13.020Z Reads: 420

```
show a picture of the vesc....
```

---
## \#4 Posted by: makevoid Posted at: 2016-04-27T05:45:18.278Z Reads: 429

```
Hi,

I don't have a VESC yet (soon :imp:) but I have ESCs with small bullet connectors and I guess 8-10 awg wire, @onloop 's awesome and tough R-Spec motors come with big bullet connectors and 12 awg wire (big wire).

Your motor has a male connector, @onloop provides you with the additional (big) female connector, the one you're holding. I also had some spare small male connectors so, what I did was to immediately solder them together to make an adapter, here are some pics.

<img src="/uploads/db1493/original/2X/7/75c1b439582fd8a6d3698df4188c2f7709b86c02.jpeg" width="669" height="499">

When they are connected you can't see what's going on, also I applied some tape to hold the adapter to the motor wire but I removed that on one to show you.

<img src="/uploads/db1493/original/2X/a/ad932b6603359d88914a44931746da720ad65d1c.jpeg" width="669" height="499">

<img src="/uploads/db1493/original/2X/2/2790ed00d40124ee1f22fe23a94bd10159e470e0.jpeg" width="669" height="499">
<img src="/uploads/db1493/original/2X/f/fd552df020aeef9f1f4541cd8e1a364d3abeeb1c.jpeg" width="669" height="499">

I hope this makes sense to you, and that you have everything you need for soldering and small male bullet connectors,  otherwise you need to order them.

The other option if you don't want to make an adapter, would be to cut the wire on the other end so your small female connector comes off and solder the big female connector on the wire itself.

Tip: make sure they're well soldered or the current that will pass through them will heat them and they will desolder while you're running ;)
```

---
## \#5 Posted by: monkey32 Posted at: 2016-04-27T08:56:25.629Z Reads: 404

```
To quote longhaired boy - 
Christ on a cracker.....soooo much e tape!!!

Enertion motors ( at least mine )R- specs come with 3x  5mm plugs (male)

If you want beefy connections 

You need 3x female for the VESC or your ESC of choice. 

Most RC ESCs come with 4mm "banana" female plugs.

If you use RC ESC you need to adapt the motor plugs and change them from 5mm to 4 or add resistance to the system by making an adapter cable with a 4 mm male on one end and a 5 mm female on the other. However at that point you have all the parts and no adapter required.....
resoldering the connections takes all of 2 min. 


When your VESC gets there solder the female 5mm connectors ( first picture ) onto the three motor leads.

Also heatshrink is your friend-  order like 6-8 meters worth - like 10 bucks at hobbyking or wherever- works on our boards and and other e- projects and doesn't leave that shitty tack residue all over- added bonus - makes your stuff look pro.
```

---
## \#6 Posted by: makevoid Posted at: 2016-04-27T09:05:37.955Z Reads: 381

```
[quote="monkey32, post:5, topic:2642"]
To quote longhaired boy - Christ on a cracker.....soooo much e tape!!!
[/quote]

hahaha so true! I'm still waiting for a heatshrink set I ordered from amazon because the local shop (Maplin) sells it for a crazy amount, like 18 usd equivalent for 3 meters

Also yes, @eskateking  adapters may be useful to test but for your final build, if all of your stuff works and you don't need to return it back you want to have big connectors everywhere for maximum current-transfer and reliability as @monkey32 wisely said
```

---
## \#7 Posted by: Kaly Posted at: 2016-04-27T11:04:29.480Z Reads: 362

```
Direct soldering of the wires is the norm for me. Cheap weller soldering gun and no more connectors. Besides solder connections makes the system more efficient.
```

---
## \#8 Posted by: eskateking Posted at: 2016-04-27T17:55:36.735Z Reads: 344

```
Not here yet. I got the one with 5.5 mm bullet connectors motor side and xt-60 connector battery side.
```

---
## \#9 Posted by: eskateking Posted at: 2016-04-27T18:00:42.056Z Reads: 355

```
So what you guys are saying is that I need to solder the end of the connector shown in picture 2 (mine) to these motor wires.
<img src='/uploads/db1493/original/2X/4/46cbb1ac8013a8fcd8e1a1123f1ebdf86752d4b2.jpg'>
```

---
## \#10 Posted by: monkey32 Posted at: 2016-04-27T21:25:22.923Z Reads: 339

```
No, solder the piece shown in this threads pic 1,2,3 to one of the three motor wires coming out of your VESC when u get it, unless it already has 5mm connectors. If the connectors are aleady on the the VESC then you are set and you can toss this in a box - plug stuff together and ride.

If the motor side of vesc has no connectors you will need to solder one onto the side of the VESC with three wires. Solder one female end to each of the three wires.....this will be the easiest way.
```

---
## \#11 Posted by: eskateking Posted at: 2016-04-27T22:17:46.570Z Reads: 337

```
OK thank you @monkey32. I got the one from Ollin board CO with 5.5 mm bullet connectors so I should be good to [quote="monkey32, post:10, topic:2642"]
toss this in a box - plug stuff together and ride.
[/quote]
```

---
## \#12 Posted by: eskateking Posted at: 2016-04-29T21:34:28.133Z Reads: 340

```
Ok so I have this receiver from @onloop. I need to connect it to my vesc from @chaka. How does they connect?

<img src="/uploads/db1493/original/2X/a/a525596b3f0226a41e928a721c34a42667d14a9a.jpg" width="690" height="388">
<img src="/uploads/db1493/original/2X/5/5e151533dd62692d28c92b3d8454ea76891ca99d.jpg" width="690" height="388">
<img src="/uploads/db1493/original/2X/a/a3c65e3151c2d2c5ebcde5b5a2f1dc0bdc54824e.jpg" width="690" height="388">
<img src="/uploads/db1493/original/2X/b/bfff9e773053662b5449799b7f410bc98228935e.jpg" width="690" height="388">
```

---
## \#13 Posted by: trbt555 Posted at: 2016-04-30T10:11:58.159Z Reads: 326

```
The receiver has two sets of three pins somewhere around the middle of the pcb. You need to connect one set of three pins with the pwm input on the vesc.
Beware of polarity, which is marked on the pcb as well as the vesc.
Schematic:
<img src="/uploads/db1493/original/2X/6/6524598ba6aa4294b4e1a9a1eb0ec70cfd928702.png" width="690" height="265">
```

---
## \#14 Posted by: eskateking Posted at: 2016-04-30T20:22:02.795Z Reads: 322

```
So vesc from @chaka or ollin board company came. Very disappointed.
It doesn't fit. I got the one with 5.5 mm bullet connectors motor side and XT-60 connector battery side like he @chaka recommended. It does not fit.
<img src="/uploads/db1493/original/2X/5/513b21db0429801a0d007b1a19e0ae5b5a41b3df.jpg" width="375" height="500">
<img src="/uploads/db1493/original/2X/1/1adc9f74a5f2f089f47ed622cfdac54b51f536b4.jpg" width="375" height="500">
```

---
## \#15 Posted by: monkey32 Posted at: 2016-04-30T20:26:08.229Z Reads: 306

```
@eskateking That's because they both have the male ends included and plugged into the ends. Pull on the end piece of Chakas parts.....he included both male and female.....you needed ( so you don't have to buy half the plugs, just solder.
```

---
## \#16 Posted by: eskateking Posted at: 2016-04-30T20:30:21.717Z Reads: 302

```
you mean the bullet connector of the vesc
```

---
## \#17 Posted by: eskateking Posted at: 2016-04-30T20:30:35.787Z Reads: 304

```
and what about the battery
```

---
## \#18 Posted by: monkey32 Posted at: 2016-04-30T20:39:50.514Z Reads: 310

```
Both. The XT 60 connector has the male end plugged in. Give it a good pull. The male end will slide out and u will be able to plug in the battery. Same thing with the motor wires, the male ends are plugged in....maybe pull them with pliers
```

---
## \#19 Posted by: trbt555 Posted at: 2016-04-30T21:01:03.191Z Reads: 331

```
No offense but judging by your questions I'd advise you to read up thuroughly on how to set up and configure your vesc . Search keywords VESC FAQ.
Otherwise you might end up even more disappointed.
```

---
## \#20 Posted by: psychotiller Posted at: 2016-04-30T21:17:27.787Z Reads: 332

```
This was obviously a joke right?
```

---
## \#21 Posted by: eskateking Posted at: 2016-04-30T21:18:01.612Z Reads: 322

```
NO

This post is now 20 characters.
```

---
## \#22 Posted by: eskateking Posted at: 2016-04-30T21:20:00.410Z Reads: 332

```
Got vesc plugged in. Started to configure it using long tutorial from @jacobbloy  Got this after I uploaded my firmware.
<img src="/uploads/db1493/original/2X/e/e7c07898379968ea12565785dcc591de21befbfe.JPG" width="690" height="367">
```

---
## \#23 Posted by: eskateking Posted at: 2016-04-30T21:31:49.843Z Reads: 316

```
@psychotiller I'm sorry if it seems like a joke. It isn't. If you could please help me that would be great.
```

---
## \#24 Posted by: psychotiller Posted at: 2016-04-30T22:27:05.772Z Reads: 309

```
I was referring only to the connectors...The firmware updates are down right scary and can get you into trouble quick. I can only say this. Make damn sure you know exactly what firmware to upload. Most,if not all problems with the vesc have been related to updates or shit soldering.
```

---
## \#26 Posted by: jacobbloy Posted at: 2016-04-30T23:43:59.254Z Reads: 312

```
Hey mate, for some reason the firmware files in the firmware folder are not the latest,
Just head to vesc.net.au/BLDC-TOOL/ go to the firmware folder and download the 2.16 firmware file.
```

---
## \#27 Posted by: eskateking Posted at: 2016-05-01T00:16:51.883Z Reads: 303

```
@jacobbloy i figured that out. I just finished coding my vesc using the 1h 16min tutorial you made. Then I plugged in the servo cable on my vesc to my enertion receiver like this but the remote won't control the  motor.
<img src="/uploads/db1493/original/2X/d/d2f73575e4cebb449055709cd9f93063e04c1e9a.jpg" width="375" height="500">
```

---
## \#28 Posted by: trbt555 Posted at: 2016-05-01T07:33:02.447Z Reads: 289

```
Disconnect the receiver.
Power the vesc with your batteries and connect it to bldc tool via usb.
Use the arrow keys on your keyboard to check if the motor is being driven.
That will rule out any config and or connection problems so you can narrow down the search.
```

---
## \#29 Posted by: eskateking Posted at: 2016-05-01T16:26:18.880Z Reads: 276

```
You think I'm an idiot? I've tried that a thousand times.
```

---
## \#30 Posted by: trbt555 Posted at: 2016-05-01T17:19:01.844Z Reads: 261

```
Dude I'm just trying to help but if you're gonna give me an attitude,  go sort your problem yourself.
```

---
## \#31 Posted by: eskateking Posted at: 2016-05-01T17:30:24.252Z Reads: 259

```
@trbt555 I'm sorry if I sounded like a jerk.
```

---
## \#32 Posted by: eskateking Posted at: 2016-05-01T18:30:40.755Z Reads: 263

```
I really can use the help.
```

---
## \#33 Posted by: ra.rend Posted at: 2016-07-08T05:10:05.658Z Reads: 244

```
GND is ground, right? Where's ground on the receiver?
```

---
## \#34 Posted by: trbt555 Posted at: 2016-07-08T07:55:47.021Z Reads: 243

```
GND = ground = black
It should be written on the receiver PCB
The RED wire is always in the middle. You won't blow up your receiver by inverting the two outer wires though. It just won't work.
```

---
## \#35 Posted by: ra.rend Posted at: 2016-07-08T11:29:25.599Z Reads: 242

```
I don't see any writing on the PCB of receiver. So if I connect the negative on the receiver and to the ground on the VESC, it should still work? No effect on the signal or anything?
```

---
## \#36 Posted by: DeathCookies Posted at: 2016-07-08T11:31:59.688Z Reads: 244

```
Maybe you will calculate it yourself because we dont know your setup ;)
http://toddy616.blogspot.de/2013/07/electric-skateboard-calculator.html
```

---
## \#37 Posted by: trbt555 Posted at: 2016-07-08T13:06:33.855Z Reads: 246

```
<img src="/uploads/db1493/original/2X/7/752e2a0a0b0a5b9e740c2dd23a4e06960feb4fb1.jpg" width="460" height="500">
```

---
## \#38 Posted by: ra.rend Posted at: 2016-07-08T14:15:44.226Z Reads: 240

```
Thanks for your help btw, but I have the torqueboard's mini 2.4 ghz remote.
```

---
## \#39 Posted by: ra.rend Posted at: 2016-07-08T21:09:13.682Z Reads: 239

```
This is my receiver <img src="/uploads/db1493/original/2X/3/3b00434dc55680cabe9ef04bad1dd94b04c99c53.JPG" width="690" height="388">
```

---
## \#40 Posted by: lox897 Posted at: 2016-07-09T07:12:58.580Z Reads: 238

```
Pretty sure brown wire is on the left of those pins. I will double check when I am home.
```

---
## \#41 Posted by: GhettoFab.rictation Posted at: 2016-07-31T09:57:30.360Z Reads: 226

```
@chaka dude really, you hooked this guy up with some plugs? And left me out in the cold. . Tsk Tsk lol , no but I have the mini remote too and I found it only flashes when plugged in a certain direction let me go check. I haven't installed the right firmware yet, I hardly doubt I got a defect I'll found out when I get a different system. Let me show you what order I got for the mini.
```

---
## \#42 Posted by: GhettoFab.rictation Posted at: 2016-07-31T10:00:12.960Z Reads: 219

```
@ra.rend <img src="/uploads/db1493/original/2X/f/fed5d56d5b8882acf5b6eeaebbc65a8b87f3264b.jpg" width="281" height="500">
```

---
## \#43 Posted by: chaka Posted at: 2016-07-31T12:05:51.794Z Reads: 211

```
Everyone has the choice to add them to the vesc during checkout. Did you expect me to include them for free? Are you using xt-90's on your phase wires??? Hope your motor spins in the correct direction otherwise you may need to resolder.
```

---
## \#44 Posted by: GhettoFab.rictation Posted at: 2016-07-31T12:41:00.442Z Reads: 208

```
Yeah dude I'd have given you a quick handy lol, yeah just on two and on all motor wires are bullet connectors to switch as needed. Do they have diodes in the connectors?? They aren't antispark so no resistor, if there's a diode then there might have to be some trial and error tests done
```

---
## \#45 Posted by: GhettoFab.rictation Posted at: 2016-07-31T12:46:44.762Z Reads: 212

```
<img src="/uploads/db1493/original/2X/a/aa678c8f547cfb60d25edcfeb1f9191f90acbcc9.jpg" width="281" height="500"> think they will work?? D:
```

---
## \#46 Posted by: elkick Posted at: 2016-07-31T15:13:07.501Z Reads: 207

```
Just a tip: please insulate the pins of the receiver after the binding process is done before puting it into the box! It's one of those common reasons for killed VESCs. :wink:
```

---
## \#47 Posted by: GhettoFab.rictation Posted at: 2016-07-31T18:43:10.551Z Reads: 204

```
Thank you for the tip dude!
```

---
## \#48 Posted by: CHANCE5 Posted at: 2016-08-10T04:21:06.723Z Reads: 192

```
<img src="/uploads/db1493/original/2X/f/f527d22dd16120f5d8cb6287504687d4e25c8e72.JPG" width="666" height="500">
[Uploading...]() Can 

Can someone please help me with this setup? I seem to have a male and female connector. but I'm confused how to put it together. when i put the caps on the motor wire, it doesn't connect to the vesc. Please help, im so close i can feel it.
```

---
## \#49 Posted by: Jinra Posted at: 2016-08-10T04:24:35.280Z Reads: 189

```
You have to solder the female heads onto the phase wires on the VESC and insulate. Like so..

<img src="/uploads/db1493/original/2X/1/198554bdadfa40b99bb5ad398e5b5b934df9da6a.png" width="668" height="500">
```

---
## \#50 Posted by: CHANCE5 Posted at: 2016-08-10T04:47:29.498Z Reads: 183

```
thank you so much my friend it helps
```

---
## \#51 Posted by: CHANCE5 Posted at: 2016-08-26T23:37:25.745Z Reads: 179

```
<img src="/uploads/db1493/original/2X/3/38f54787dfa3045f627f96e6fc3b4fb524cfc92b.JPG" width="666" height="500">o

I just want to be sure. do I have to solder these gold caps to the vesc like so or do I have to turn the gold caps around and solder them?
```

---
## \#52 Posted by: Jinra Posted at: 2016-08-26T23:56:54.904Z Reads: 177

```
The way you have it in the picture is correct. Make sure you insulate with electrical tape or heatshrink after!
```

---
## \#53 Posted by: CHANCE5 Posted at: 2016-08-26T23:58:25.899Z Reads: 179

```
ok great awesome. thank you buddy and much love.
```

---
## \#54 Posted by: Pablo_702 Posted at: 2016-08-27T00:29:54.117Z Reads: 182

```
Wheres your vesc from?
```

---
## \#55 Posted by: CHANCE5 Posted at: 2016-08-31T06:10:34.923Z Reads: 179

```
Enertion board
```

---
## \#56 Posted by: CHANCE5 Posted at: 2016-10-16T21:04:49.263Z Reads: 151

```
<img src="/uploads/db1493/original/3X/3/5/3577c2d7a49b348147f4da46923f7e9609adbfc4.JPG" width="666" height="500"><img src="/uploads/db1493/original/3X/f/3/f34e435ddb9edf5ebde00f54735d5ee60175780e.JPG" width="666" height="500">


Hey guys im having this problem with my motor, it wont start. it was working a week ago. but when i took it apart i saw a RED light was blinking on the vesc. what should i do? I soldered the male cape to the motor wire again and i tried reconnecting the controller over and over again but nothing worked. also im not sure if there's a website I need to got to see if i have a motor detection, but if you could refer me to the name of the site it would be very helpful. Please help and God bless.
```

---
## \#57 Posted by: lox897 Posted at: 2016-10-16T21:16:02.308Z Reads: 139

```
Check for fault codes on the bldc tool. You may have a drv error.
```

---
## \#58 Posted by: Luke Posted at: 2016-10-16T21:16:50.060Z Reads: 140

```
Have you set up the vesc with bldc tool? If you already have it then I'd use to to check if your vesc has any faults. If you don't have it I think you can still download it from vesc.com.au
Damnit lochlan is too fast
```

---
## \#59 Posted by: CHANCE5 Posted at: 2016-10-18T03:13:06.675Z Reads: 138

```
[quote="lox897, post:57, topic:2642"]
bldc tool
[/quote]

it says the motor detection has failed, so i guess, buy another huh? or is there another thing that im missing. please keep me posted and thanks for the help.
```

---
## \#60 Posted by: CHANCE5 Posted at: 2016-10-18T03:18:37.828Z Reads: 141

```
[quote="CHANCE5, post:59, topic:2642"]
it says the motor detection has failed, so i guess, buy another huh? or is there another thing that im missing. please keep me posted and thanks for the help.
[/quote]

it says the motor detection has failed, so i guess, buy another huh? or is there another thing that im missing. please keep me posted and thanks for the help.
```

---
## \#61 Posted by: lox897 Posted at: 2016-10-18T04:55:04.219Z Reads: 143

```
No I think you should be able to fix this. Is the motor connected properly? Maybe @chaka or @Jinra can help
```

---
## \#62 Posted by: Jinra Posted at: 2016-10-18T04:58:20.629Z Reads: 138

```
Do the detection again until it errors out. Then go to terminal and type 'faults'. Paste any faults here.

I was helping someone else recently with a failed detection. It faulted with an ABS_Over_current fault. We concluded it was a bad VESC given that detection on the same motor worked on another VESC with the same power source.
```

---
## \#63 Posted by: CHANCE5 Posted at: 2016-10-19T17:52:46.791Z Reads: 144

```
[quote="Jinra, post:62, topic:2642"]
faults
[/quote]

I typed in "faults" and a lot of things came up and the motor is still not responding. what else am i supposed to do?this is what came up when I typed faults-<img src="/uploads/db1493/original/3X/7/6/763a24183f5ca2587b4036aa9f25ea1260f8a7ff.png" width="690" height="431"><img src="/uploads/db1493/original/3X/c/4/c4dfca85ff05bee75b0ac848914cb9f294984e23.png" width="690" height="431"><img src="/uploads/db1493/original/3X/9/5/95889384049d0478ec789f89b4e10cb156a36c9d.png" width="690" height="431">
```

---
## \#64 Posted by: lox897 Posted at: 2016-10-19T19:24:52.539Z Reads: 116

```
That's a DRV fault. That means the chip on the board is buggered. You'll have to get it repaired
```

---
## \#65 Posted by: tonystark Posted at: 2017-02-27T01:50:56.847Z Reads: 81

```
Hi mate. I see your motor has 3 black wires. How do you know which wire is which? I have this problem with my alien drive motor. It has 3 black wires and i have no idea which to connect where? thanks
```

---
## \#66 Posted by: tonystark Posted at: 2017-02-27T01:54:58.634Z Reads: 80

```
Hi. As i see, you motor has 3 black wires. how do you know which one is which? i have this problem. i have alien power systems motor and it has 3 black wires. and i have no idea which one to connect where? can you help please? thnks
```

---
## \#67 Posted by: tonystark Posted at: 2017-02-27T01:56:53.273Z Reads: 79

```
Hi. your motror has 3 black wire just like mine. how do you know which wire is which? i cant figure out how to connect mine
```

---
## \#68 Posted by: fedestanco Posted at: 2017-02-27T02:13:32.634Z Reads: 79

```
If the wires are well insulated (you don't see bare copper) you can proceed connecting them randomly. Power them. If the spinning direction is wrong, just swap 2 cables.

Please use search function ⬆next time: faster for you, less spam for the forum.
```

---
## \#69 Posted by: tonystark Posted at: 2017-02-27T02:27:49.297Z Reads: 79

```
thanks for such fast reply. i did use search function and tried many different key word combination but was not able to find anything. so i can randomly connect those 3 wires and it will not damage neither my motor nor vesc? and just play around untill i find correct connection?
```

---
## \#70 Posted by: JohnnyMeduse Posted at: 2017-02-27T02:34:45.935Z Reads: 81

```
No It won't damage the vesc, also he the motor doesn't run in the way you want, you can just swap two cable, to change the motor direction.
```

---
## \#71 Posted by: Lucas123 Posted at: 2017-02-28T19:53:33.541Z Reads: 79

```
Hello,
About a 2 months ago I bought two Maytche VESCs from Alien power system and as I finished setting everything up and assembling everything I plugged it all in but when I turned my Enertion pace cell pro 3 the controller connected to the receiver which was getting power but I realized the VESC's where not responding so I disconnected everything and attempted to connect them to my computer. But I realized that when I plug the plug the battery in, nothing happened and the VESC's does not light up. But the receiver gets power when I connect it to the VESC's and the micro USB ports on the VESC's do get really hot in about 10 seconds.

Thank you for reading
```

---
## \#72 Posted by: JohnnyMeduse Posted at: 2017-02-28T20:42:35.597Z Reads: 77

```
Maybe this could help you

http://www.electric-skateboard.builders/t/no-power-to-enertion-vesc/7600/8?u=johnnymeduse
```

---
