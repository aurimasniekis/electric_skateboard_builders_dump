# My monodrive 6374 10s bamboo eboard

### Replies: 47 Views: 4056

## \#1 Posted by: GunnarK Posted at: 2017-09-18T22:53:02.620Z Reads: 415

```
Hi! 
My name is Gunnar and I'm from the Netherlands. I am a student in Computer Science, Mediatechnology and live in Leiden. I am currently graduating at Servoy, a software company in Amsterdam.

This is my first eboard build, but I have done some hand work in the past. I build my own electric guitar in somewhat the same way as with this eboard, scrapping all parts from everywhere. Here is a pic (the white one):

<img src="/uploads/db1493/original/3X/7/d/7d00bbcc9b53094fce27242f0623401c1a8ca59c.jpg" width="385" height="500">

In case you are interested in that build, you can look it up here: 
https://www.facebook.com/media/set/?set=a.260309357333874.69478.100000644343212&type=1&l=31841c7f32


Anyways, the eboard build! 
IF YOU HAVE ANY TIPS, FEEL FREE TO LEAVE THEM BELOW!
I created an Instagram account to document the whole build, but this forum is obviously more suited to go more in-depth. I will keep posting pics to that account
https://www.instagram.com/gunnarkelders/

## Parts list

I got almost all the parts needed, except for the battery enclosure made by @bigben. Which should arrive tomorrow.
I ordered a lot of stuff from eskating.eu @fottaz is very helpful and an awesome guy to talk to.
From his webshop I ordered:
* Motor 6374 sealed & sensored
* VESC
* Remote control, nano
* Bluetooth module

The deck I ordered from blankskateboards.nl
http://www.blankskateboards.nl/LongboardDropThroughBamboo
It's four layers of maple sandwiched between two layers of bamboo. Although blankskateboards told me it was a stiff board, It was a very flexy imho (and probably yours as well).

<img src="/uploads/db1493/original/3X/7/6/76931c1fa9c1210a28aa164e02dde3ceca94b1db.jpg" width="690" height="225">
FYI; In this picture I jumped on the board ;)

So yeah, note to self; don't flex the board like this with all the equipment installed ;)

From sickboards.nl I ordered the following
Caliber 2 10s 50 trucks
Orangatang wheels
Zealous bearings

Angled risers from skateshop in Leiden called _Juhroen_

Braided copper wire from Conrad.nl
https://www.conrad.nl/nl/kabeltronik-koperdraad-geweven-band-486090.html

The mount I got from @WSB
The VESC enclosure from @Crossfire .
Pulleys (17mm) and belts (15mm) from @Idea

From Hobbyking I ordered:
5x 2s 40c Zippys
BMS extension wires (used none of it) JST-XH 2S WIRE 20cm
1m 10AWG black silicon wire
1m 10AWG red silicon wire

* More parts will be added later

## The build itself

* _18-09-2017_

I filed the truck to fit my pulley and motor mount. It took a very long time to make this perfect and I still didn't get it right. The belt wants to move over to one side of the motorpulley where it gets stuck on the side. I tried filing the truck because it was a bit misaligned, but after I got this right it still wanted to touch the side of the motorpulley. The mount bracket is straight so that is not the culprit.
This will probably mean the belt won't have the servicelife it was intended for but I can't seem to get it right.

Anyways, I installed the mount with blue loctite and adjusted the angle so the motor won't touch the deck.

The only image I have of altering the motor mount and truck. I don't have any photos of the truck, but I filed the top flat part of it to remove the slight arch that the truck has towards the middle.

<img src="/uploads/db1493/original/3X/b/7/b74c01c032a09847517106b747b33ff62b589d38.jpg" width="666" height="500">

Finally some drilling..
Bottom view. The center two holes are 3cm apart and the two holes surrounding them are 1.5cm distanced.
I might drill two extra holes for a third wire, but I don't think that is really necessary. What do you think? 

<img src="/uploads/db1493/original/3X/8/6/867adae1169157aad6a799d47c685cc0322dc468.jpg" width="666" height="500">

Top view. I used a circular file to carve the sharp edges off since the battery wires will run through there to the nose of the board. I don't want to have sharp edges which could cause breaks in the copper braided wire

<img src="/uploads/db1493/original/3X/7/5/757f2bcc3a34270234ada6a204bd325c1f0bc5b7.jpg" width="666" height="500">

And so this is how it is standing in my apartment right now

<img src="/uploads/db1493/original/3X/c/4/c4cebd8c1e2d119dbe0703670af2042ba9eb6645.jpg" width="666" height="500">

----------

* _13-10-2017_

Yesterday evening I got around to finally start soldering the batteries together. Including the BMS wiring.

<img src="/uploads/db1493/original/3X/d/c/dc1d5af0f46163d11b84c8155d32c01c0608228a.jpg" width="666" height="500">

At one time I tried cutting the red and white BMS wires at te same time and they shorted. Hope that won't be any problem for their life expectancy?
I don't have a multimeter so I was not able to check the voltage of all cells, but I did have some LEDs with which I could test at least that the cells are not dead.. (;
Might be a good idea to rent one at the shop across my place.


----------

* _16-10-2017_

Yesterday I prepared the battery enclosure for the external hardware; the on/off switch, percentage display and charging port. And I discovered two things:
1. the on/off switch was not a switch, but a button. My fault for my bad german (; (bought from amazon.de)
2. the charging port does not make complete contact. the pin does, but the outer shell does not.

So I need to order another button and have in the meantime a large gaping hole that I need to cover up. Any ideas on a temporary cheap on/off mechanism?
The chargingport I tried to narrow the outer shell with tin, but this was a bad idea to start with. the tin would not stick to the metal. After some fooling around I found out that the outer parts of the chargingport worked as a ground, meaning; I have a circuit! So I just soldered my negative lead to the outside of the chargingport.

<img src="/uploads/db1493/original/3X/2/f/2f31c9ec6468257bef3eb52ba1a3cbbca5c6136a.jpg" width="676" height="500">

<img src="/uploads/db1493/original/3X/4/6/464b3ba650928e4d9c09e1750ef8724a2d6bd6cd.jpg" width="666" height="500">

This evening I finished drilling the holes in the deck to desired width of 9mm.
That is the width needed for the insert nuts and from there on I also used it for the bridge wiring to run through.
The insert nuts I first inserted by hand but this didn't go very well. Since I twist my hand when turning with force they weren't completely aligned to the deck. For the vesc enclosure I used a drill to slowly insert them, this worked flawlessly!

<img src="/uploads/db1493/original/3X/f/3/f34584ecad6b2d333333ef3ea8d072ab6e463b0c.jpg" width="666" height="500">

<img src="/uploads/db1493/original/3X/e/8/e8bbb0b5f13fc3a7eacda05677d9d9aff9ce1570.jpg" width="666" height="500">

Then it was time to install the bridge wiring for the two enclosures!
This was a fairly easy process using kapton tape and a paper towel to rub the tape down over the copper wire.
A nice little animation

<img src="/uploads/db1493/original/3X/c/6/c6f7d94751d8aa2417a4c61e7967780b0d991fa3.gif" width="666" height="500">

And this is how it is standing across my apartment right now!

<img src="/uploads/db1493/original/3X/8/9/891ab0d53ad83cb74d0a0bcc3a71e00e5427e4c6.jpg" width="374" height="500">

----------

* _22-10-2017_

Yes guys! Today I completed the build as far as I could go!
I have 2 problems of which one I discovered this evening:

* The aforementioned on/off switch being a on/(on) 'switch'
* The battery indicator LCD does not turn of in the way I wired it to the BMS and positive battery connector

No real problems I thought as I wanted to complete most of the build so I could test it tomorrow.
I will discuss the problems down in the replies of this page so definitely check it out!

So the build is almost complete. I rode it just now across the hallway in my flat since it's raining outside. Damnn this thing is really powerfull! I set the VESC settings for Motor max and Motor min at 30A and it is still too damn powerfull!! :scream:
Not complaining of course but just really baffled about that 'little' motor pushing me forward.
I do immediately understand the pros of having a dual drive eskate. The rear truck turns to the left causing the board to wiggle a bit. It is easy to compensate but you shouldn't have to in an ideal case (and infinite money).

Oh well, here some info about the process of finishing the build:

First up was the battery pack. Almost all the components were installed for a test but then I discovered that the switch was a button and not a switch. So I had to come up with a temporary solution for the time being. My solution was to use the cut-off ends from the lipo batteries as a connector:

<img src="/uploads/db1493/original/3X/b/6/b6d858ea8f544261704f5170804e20fc637ecc5f.jpg" width="666" height="500">

From there on i checked the battery system and it all seemed to work fine. Strangely when turning off the system the battery indicator's backlight turned off as expected but the lettering on the display stayed on, displaying _0%_. The only way to turn it off was by disconnecting it briefly, afterwards I can connect it again but it won't turn back on until I turn on the whole battery system. An issue for later I thought, first let me try to charge the battery for the first time..

Before I did that I glued the battery indicator to the battery enclosure with hotglue, because I want to make testing harder on myself (;
Anyway; SUCCES!! It charged completely fine up to 100%.

<img src="/uploads/db1493/original/3X/4/d/4d0f9cfe26b6ee4cd871e8f32909fc70c895a423.jpg" width="374" height="500">

From my calculations the battery should be charged in like 5 hours. Charging the 10S (5x 2S 5000mAh 40c) at 3A, that is.

Next challenge, soldering the bridge wires together. This was somewhat a pain in the ass. My 30W soldering iron made it fine, but forcing the wires to cross each other and solder 3 wires together wasn't a joyfull task. 
Eventually I succeeded

<img src="/uploads/db1493/original/3X/5/b/5b80d9f84a4dec14fb8b8044f759409359c13323.jpg" width="666" height="500">

The extra black and red wire is to compensate for the length I need when I will detach the battery enclosure from the board for inspection or whatever. 
Just to make life easier I did the same for the VESC

Then I slapped some velcro tape to the battery and enclosure to attach them together (bought at Gamma).
From my guitar build I had some leftover foam. It had one corner cut out, but that made it almost perfect so I did the same to the other corner to leave enough space for the charging port and switch. This foam is supposed to absorb shocks and protect the BMS.

<img src="/uploads/db1493/original/3X/1/d/1dc4a8c98cc601e79baef35aeb7a4dddb04bc8a1.jpg" width="666" height="500">

I had more of this foam so to be better safe than sorry I slapped it to the back of the BMS as well. This way it also acts as a insulator for the charging port and switch!

<img src="/uploads/db1493/original/3X/3/f/3ff84eb01ca57eff491700f91b7a70de9a6b2fe8.jpg" width="666" height="500">

From @bigben I got some sealing foam to make the board water resistant (or at least dust resistant). Here is a pick of it. You can also see why the extra wire on the bridge wiring comes in handy

<img src="/uploads/db1493/original/3X/d/4/d4417d4a70b32fd91baa8f52375730bf9f2ae0fa.jpg" width="374" height="500"> 

From here on I forgot to take some pictures. But it is really straightforward, meaning the bridgewiring to the VESC. And connecting all the other parts.
Just as the battery enclosure I put some rubber sealing on the VESC enclosure.

<img src="/uploads/db1493/original/3X/9/8/981f59ccb3aa32b9af1d97eb243ed4e1ddf8f3ed.jpg" width="374" height="500">

Then I soldered the VESC to the bridge wiring. Slapped some velcro tape to the back and mounted it on the board. And the same for the receiver and bluetooth module. 

<img src="/uploads/db1493/original/3X/9/c/9c40f42d98d07816523650cd5ec154ed90dbd336.jpg" width="666" height="500">

After this it was only a matter of connecting all the parts together. And measuring by eye what length the wires for the motor needed to be and hotglueing them to the VESC enclosure to seal it from dust or water.

AND THAT'S IT! (alright, not entirely. but just let me celebrate already!)

<img src="/uploads/db1493/original/3X/7/e/7e60172b61219d6930a3fcddbab58823fbd812a7.jpg" width="666" height="500">

Charging both the remote and the board. Also; behold my beautiful temporary switch!

From here on I did some tweaks to the VESC. Unfortunately this is when I discovered that the bluetooth module doesn't power on and I have no idea what the problem is. Maybe it's faulty? I have set the VESC to PPM + UART (with baudrate 115200)

<img src="/uploads/db1493/original/3X/9/e/9e6d4f04903586dba613cd6b8df357a16f7de05b.jpg" width="666" height="500">

<img src="/uploads/db1493/original/3X/e/4/e4ac36a2701f5dcd14aa8b3785eddf18fbd2dee4.jpg" width="666" height="500">

## Thoughts on the flex
Alright, so as you probably have seen on this topic there are a few pictures of me standing on the board and showing of the flex. Standing in normal position and with my feet in the exact middle (and jumping) to show the flex.
To make a long story short: after mounting the battery enclosure, the bridge wiring on top of the deck and the griptape probably also plays a role; the flex seems to have deminished. It is still there but somewhat less.
The flex makes the board very smooth to ride.
Living in Leiden, an old city with old rough roads where there is no bicycle lane, the flex really makes a difference. It absorbs a lot of the shocks!
Till now I only scratched the battery enclosure because of me wanting to try out a very shallow pavement.

## List of problems
So as of now I have 3 problems. They are:

* Bluetooth module not working, although controllmode is set to PPM + UART
* FIXED: No switch, but temporary battery connectors
* FIXED: Battery indicator not turning off, although backlight does (disconnected for now because of that)

Hope you guys can help me with this!
Thanks!
```

---
## \#2 Posted by: gee Posted at: 2017-09-19T01:10:02.499Z Reads: 350

```
Pretty sure your pulley cover is 3D printed. Can you share your file? And how you got it to fit onto your motor mount.
```

---
## \#3 Posted by: mmaner Posted at: 2017-09-19T02:08:21.498Z Reads: 352

```
I play guitar too, I have Jackson Dinky 5 with reverse headstock and shark tooth inlay...no I didn't build it. 

Nice build.  What battery are you running?
```

---
## \#4 Posted by: GunnarK Posted at: 2017-09-19T05:12:12.703Z Reads: 350

```
The cover came with the mount that I bought from @WSB 
It is fastened with two bolts<img src="/uploads/db1493/original/3X/c/8/c84ce64f317af8e08fcbb5c6e0101ec43a310a51.jpg" width="666" height="500">
```

---
## \#5 Posted by: GunnarK Posted at: 2017-09-19T05:16:23.516Z Reads: 333

```
Nice guitar man!

I will be using 5 2s 5000mah 40c zippys. Already got them in but forgot to mention them
```

---
## \#6 Posted by: bigben Posted at: 2017-09-19T05:41:01.828Z Reads: 319

```
That is one flexy deck. Is that flex with you jumping on it? 
Have you considered laying fibreglass or carbon layers on it to stiffen it up? It looks like the enclosure is going to take a hammering!
```

---
## \#7 Posted by: GunnarK Posted at: 2017-09-19T06:44:07.795Z Reads: 323

```
Yeah it's me jumping on it. This is a frame of the video I recorded of it
When I just stand on it, the deck will bend a little bit

Thought it wouldn't mind that much since Boosted also has some real flexy decks

Frame from same video (some time ago):
<img src="/uploads/db1493/original/3X/b/3/b3dd2b04715ae1ca57e64788df9ef13fd5ed9a15.jpg" width="690" height="388">

This is when I just stand on it. Imo it does seem from me standing on it that it flexes more that in the beginning, but not sure

Video frame from last week:
<img src="/uploads/db1493/original/3X/c/c/cc6209a19c96cd513c508c66ae5f923e07ec2c4a.png" width="690" height="161">

I will try to get a better picture of the flex tonight
[quote="bigben, post:6, topic:33460"]
Have you considered laying fibreglass or carbon layers on it to stiffen it up?
[/quote]

No I haven't. Maybe I should consider it or buy a new deck. I would love your opinion on the flex when I get a good pic of it
```

---
## \#8 Posted by: Mikenopolis Posted at: 2017-09-19T22:16:56.321Z Reads: 286

```
It looks like that motor and mount would take a beating at the smallest bump. Are those angled risers?
```

---
## \#9 Posted by: GunnarK Posted at: 2017-09-19T23:27:29.725Z Reads: 289

```
Yes those are 1/2 inch angled risers. The way it is adjusted right now is to prevent the motor from touching the deck
I have flat 1/2 inch risers laying here

What would you recommend?
```

---
## \#10 Posted by: Mikenopolis Posted at: 2017-09-19T23:48:40.098Z Reads: 283

```
[quote="GunnarK, post:9, topic:33460"]
adjusted right now is to prevent
[/quote]

are you sure it touches the deck? Does your phone/camera have slow motion ability? I would suggest you jump on the board to see if the flex make the motor make contact with the ground.
```

---
## \#11 Posted by: ARetardedPillow Posted at: 2017-09-20T05:12:10.511Z Reads: 262

```
Yea the motor looks like its going to get shitted on with just a tiny bump, happened to me so I put mine outwards instead, and the flex of that board is def going to do some harm eventually
```

---
## \#12 Posted by: GunnarK Posted at: 2017-09-20T06:32:49.434Z Reads: 261

```
It doesn't touch the deck when steering. 
I will try to make a slomo of me jumping on it with the motor installed.

The angled risers should help prevent the motor+mount from touching the deck right?
I'm thinking of getting stiffer deck, but that won't fix the problem of touching the deck.
Know some nice decks?

@ARetardedPillow you're probably right. Got any recommendations for a stiffer deck that won't break the bank?
```

---
## \#13 Posted by: TehAtheist Posted at: 2017-09-20T09:01:07.058Z Reads: 260

```
Correct me if only wrong, but that won't do anything unless you put it in inside the deck? Just putting it on top or on the bottom won't help. Some manufacturers do it, but it's shit. That doesn't work?
```

---
## \#14 Posted by: GunnarK Posted at: 2017-09-21T17:35:11.050Z Reads: 263

```
Finally got the time to record what will happen if I jump on it with the motor installed.
<img src="/uploads/db1493/original/3X/8/f/8f6307d645e916aae42fb21f80a6d0a9536bae08.jpg" width="690" height="156">

Me just standing on it
<img src="/uploads/db1493/original/3X/c/9/c923c4f8e0244d11620f888caa64f3bfe66e8cc0.jpg" width="690" height="156">
<img src="/uploads/db1493/original/3X/1/c/1c20b9cd03c263b57511951097010a299d35929f.jpg" width="689" height="158">

The battery enclosure also arrived tuesday. But it was larger than I expected it to be, partly because of miscommunication with bigben but also my fault for trusting someone elses 3d boosted style design and not measuring (didn't have tape measure or anything) what the impact would be on my deck...

<img src="/uploads/db1493/original/3X/e/1/e173903a9d2712df637f2d3e0eb403e7eb81a18a.jpg" width="666" height="500">
I'm afraid this is not going to work for a flexing deck.
<img src="/uploads/db1493/original/3X/0/2/028fe15341ef5aa6e4936cdf237993fd07fdcaea.jpg" width="666" height="500">

What do you think? The enclosure has a lot of room left when BMS and battery are inside
```

---
## \#15 Posted by: chewydinosaurs Posted at: 2017-09-21T17:52:48.217Z Reads: 248

```
When you're riding you don't have your feet in the middle for one. Secondly, clearance between the ground and the motor is the more common issue with esk8. I wouldn't worry about it unless the battery enclosure is actually dragging on the ground. Worst comes to worse you can saw the battery enclosure in half to lower the height of it, then just mount L brackets on to the board and enclosure to hold it onto the board.
```

---
## \#16 Posted by: GunnarK Posted at: 2017-09-21T22:10:10.173Z Reads: 245

```
[quote="chewydinosaurs, post:15, topic:33460"]
When you're riding you don't have your feet in the middle for one.
[/quote]

Of course. The pictures are only to show the flex in two positions

I hope the enclosure will also add  strength to the deck.. I will see what i come up with concerning the enclosure. Thanks for your advice!
```

---
## \#17 Posted by: mmaner Posted at: 2017-09-22T01:42:57.304Z Reads: 233

```
You could use some aluminum U channel to stiffen the board maybe make it a cover for the cabling between the enclosures.
```

---
## \#18 Posted by: pat.speed Posted at: 2017-09-22T04:33:44.513Z Reads: 225

```
Yes, like @mmaner said you could use some sort of aluminium rod or bar and run it down the length of the deck to as stiffness. Or you could get a u shaped bar and put it on each side of the deck
```

---
## \#19 Posted by: GunnarK Posted at: 2017-09-22T06:27:35.249Z Reads: 227

```
Will look into that but I want to keep some of the flex. Your solutions sound like they don't allow any flex
```

---
## \#20 Posted by: pat.speed Posted at: 2017-09-22T06:53:04.373Z Reads: 230

```
If you use a thin enough bar it should still allow a small amount of flex
```

---
## \#21 Posted by: bigben Posted at: 2017-09-24T07:56:30.147Z Reads: 222

```
<img src="/uploads/db1493/original/3X/3/7/378ae2100441a3fd5915660f975b8886cebdb362.JPG" width="666" height="500">
You could just get a smaller enclosure made??
```

---
## \#22 Posted by: GunnarK Posted at: 2017-09-24T08:28:50.785Z Reads: 210

```
Yes! Looking great man!
```

---
## \#23 Posted by: GunnarK Posted at: 2017-09-24T08:31:15.214Z Reads: 212

```
Hey all!
Yesterday I created a new selling topic for the enclosure
You can find it here
http://www.electric-skateboard.builders/t/nl-fiberglass-boosted-style-enclosure-for-sale/33780?u=gunnark
```

---
## \#24 Posted by: daannyy Posted at: 2017-09-24T13:30:33.781Z Reads: 202

```
Nice Build Man! Which enclosure did u use for the esc, anti spark and receiver?
```

---
## \#25 Posted by: GunnarK Posted at: 2017-09-24T14:20:33.291Z Reads: 198

```
Thanks dude!
I got it made by @Crossfire
Here is the STL file
 https://www.thingiverse.com/thing:2472906
```

---
## \#26 Posted by: GunnarK Posted at: 2017-10-13T07:28:14.728Z Reads: 178

```
Updated the topic with recent 'improvements'
* _13-10-2017_
```

---
## \#27 Posted by: GunnarK Posted at: 2017-10-16T22:05:13.799Z Reads: 172

```
Updated the topic
* 16-10-2017
```

---
## \#28 Posted by: GunnarK Posted at: 2017-10-23T20:46:31.070Z Reads: 165

```
Updated the topic and FINISHED THE BUILD
* 22-10-2017_
```

---
## \#29 Posted by: GunnarK Posted at: 2017-10-23T20:49:05.512Z Reads: 167

```
Hi guys I am having two problems that I can't seem to figure out..
They are:
Bluetooth module does not turn on even though VESC is set to PPM + UART
Battery indicator does not completely turn off when whole system is turned off.

I will split them into two replies so it is easier to keep conversations apart ;-)
See below this reply
```

---
## \#30 Posted by: GunnarK Posted at: 2017-10-23T20:54:16.601Z Reads: 176

```
##Problem 1: (FIXED!) Bluetooth module not working

The bluetooth module (https://eskating.eu/product/bluetooth-uart-module-for-electric-skateboards-android-ios/) does turns on but I can't find it inside my Bluetooth settings on my Nexus 5X.. I followed the instructions on @fottaz's website. Setting the VESC to PPM + UART and the baudrate to 115200 (by default).

Using my Samsung S4 I can find it but I am not able to pair it.
My main device, Nexus 5X running Android 8.1 can't find it at all.
Please advice


FIX: downgraded my Nexus 5X to Android 7.1.2. A fix for Android Oreo will hopefully arrive soon
```

---
## \#31 Posted by: GunnarK Posted at: 2017-10-23T21:15:20.022Z Reads: 178

```
##Problem 2: (FIXED!) battery indicator not turning off

I wired the battery indicator as follows which seemed to be the most reasonable way of wiring it:
<img src="/uploads/db1493/original/3X/c/2/c2689cde2928d93d530b51de5a17e5303d0eaed3.png" width="690" height="424">
http://www.electric-skateboard.builders/t/high-power-10s-lipo-battery-pack-with-bms/10014/72?u=gunnark
I borrowed @Namasaki's wiring diagram and added the battery indicator to it. Can you give some insight in this problem, Namasaki? Would love to hear from you

I understand why the battery indicator doesn't turn off. It has a positive and a negative that never loose contact even after the system is turned off since there is still some current flowing.
So my question is: how do I wire the battery indicator so it will function normally?


**Some thoughts**
I only tested the battery indicator while the BMS was _NOT connected_ to the VESC and motor so maybe that would help to let the current escape from the system? Before taking the board apart again I would like to receive some input from you guys about this!
```

---
## \#32 Posted by: Jumpman Posted at: 2017-10-23T21:23:22.290Z Reads: 143

```
I’m no expert but if you want to measure battery voltage, why not put the meter across the battery?
```

---
## \#33 Posted by: GunnarK Posted at: 2017-10-23T21:28:45.081Z Reads: 143

```
You mean putting the indicator directly on the positive and negative wires of the battery?
Well, because then the indicator will be always on and will only turn off when the battery is dead (which will probably happen in a somewhat faster rate because of the indicator discharging it)..

I want the battery indicator to also be the indicator of the system being turned on.
I don't have access to a 12V source from the battery indicator to install a switch with built in LED
```

---
## \#34 Posted by: Jumpman Posted at: 2017-10-23T22:07:33.360Z Reads: 129

```
Ok, I understand now.  I guess you need a 12v step down voltage regulator for the led switch.  For the battery meter you could install a loop/antispark key on the battery side.
```

---
## \#35 Posted by: Namasaki Posted at: 2017-10-24T02:20:38.019Z Reads: 132

```
[quote="GunnarK, post:31, topic:33460"]
I only tested the battery indicator while the BMS was NOT connected to the VESC
[/quote]

This is why it's not tuning off. 
After you connect the Vesc, it will work properly. 
The reason is that when you turn the bms off, there needs to be a load that will drain the bms output circuit down. 
The Large caps on the Vesc do this.
```

---
## \#36 Posted by: GunnarK Posted at: 2017-10-24T08:42:50.185Z Reads: 121

```
Thanks Namasaki! Great to hear I was headed in the right direction :slight_smile:
My new switch will also be delivered today so I can get started somewhere this week with repairing these things
```

---
## \#37 Posted by: GunnarK Posted at: 2017-10-24T08:46:05.850Z Reads: 124

```
That would probably work but it kind of defeats the purpose of a switch on the BMS
I think Namasaki's solution will work.

I will keep you posted on this!
```

---
## \#38 Posted by: Jumpman Posted at: 2017-10-24T09:04:20.705Z Reads: 126

```
Yep, I realised that you probably didn’t need any additional equipment taking up more space.  I like the way that you implemented this with your voltmeter acting as an indicator, will have to look into that BMS.
```

---
## \#39 Posted by: GunnarK Posted at: 2017-10-24T09:12:21.448Z Reads: 136

```
Thanks Jumpman!
I got the BMS as a recommendation from Namasaki. Have a look at his topic I linked to with the wiring diagram.
That topic is FILLED with so much great knowledge.
Here is the specific datasheet for my BMS. It is actually for Li-Ion batteries but the higher battery cut-off will help prolong the battery life
<img src="/uploads/db1493/original/3X/5/e/5ed954d2b7bb31cbe5f6727abd814a3009bd5900.jpg" width="281" height="499">
```

---
## \#40 Posted by: Jumpman Posted at: 2017-10-24T09:21:47.984Z Reads: 130

```
Thanks for the link.  Look forward to hearing how it works out.
```

---
## \#41 Posted by: GunnarK Posted at: 2017-10-26T08:45:32.867Z Reads: 124

```
So yesterday evening I installed my new button/switch and reconnected the battery indicator.
They work great! Problem 2 is solved

<img src="/uploads/db1493/original/3X/9/4/9413dc8b206b30705b3e3b010b4d8e19642151db.jpg" width="374" height="500">

BUT the button I have, of which its original price was around 24 euro, does not take vibrations very well..
On my commute this morning I had the board turning itself off about 5 times. Very annoying!
Luckily the brakes still work because of the regenerative system 😅

Does anyone else have this problem? What button do you recommend?
The hole in the enclosure is 16mm wide
```

---
## \#42 Posted by: pat.speed Posted at: 2017-10-26T11:18:07.166Z Reads: 112

```
So your saying your brakes work when no power is going to the Vesc? How is the receiver powered then?
```

---
## \#43 Posted by: Crossfire Posted at: 2017-10-26T12:24:36.248Z Reads: 113

```
I had the same problem with the antispark switch. It once turned off the board on the rough terrain at like 20 km/h. No way I'm going through that again.

I went the antispark XT90 key route. Best decision ever. Reliable, easy, just works.
```

---
## \#44 Posted by: GunnarK Posted at: 2017-10-26T13:11:07.287Z Reads: 112

```
@pat.speed I think because the system still holds charge for a few seconds when I just normally push the button to switch it off.
But when I'm riding the motor is spinning of course and maybe that makes it harder for the load to escape?
The receiver is connected with the 3 wire servo cable on to the vesc. Just my theory

@Crossfire Yeah that is probably the best solution. It's just such a shame of having this big hole in the board (and covering it up with ducttape or something). My board looks so clean now!
```

---
## \#45 Posted by: GunnarK Posted at: 2017-10-28T10:32:29.890Z Reads: 103

```
So guys, I have edited the post 
[quote="GunnarK, post:30, topic:33460"]
Problem 1: Bluetooth module not working
[/quote]

The Bluetooth module is blinking a red LED as expected. But I am not able to find it using my Nexus 5X running Android 8.0 and 8.1
Using my old Samsung S4 running Android 7.1.2 it works!

Damn you Oreo!
```

---
## \#46 Posted by: GunnarK Posted at: 2017-10-28T11:07:23.243Z Reads: 105

```
I have created a specific topic for the bluetooth problem cause I figure this will be easy to fix and it could be of interest to a lot of people. 

Have a look

http://www.electric-skateboard.builders/t/hm-10-pairing-rejected-by-bt05/36713?u=gunnark
```

---
## \#47 Posted by: GunnarK Posted at: 2017-11-23T16:29:24.665Z Reads: 85

```
*Some updates*

It has become clear Android Oreo (8.0 and 8.1) have Bluetooth LE issues. You can look all the issues people made here issuetracker.google.com
Today I reverted from Android 8.1 beta to 7.1.2 by adb-flashing

Metr.at
I sold my previous Bluetooth module and bought the Metr.at one. Them statistics are gewwd!
```

---
