# Loaded Dervish/Dual R-Spec 6355/Dual VESC/Nunchuck/Paris 195/90mm Flywheels

### Replies: 90 Views: 13319

## \#1 Posted by: trbt555 Posted at: 2015-11-21T15:54:29.131Z Reads: 468

```
Ok guys, 
After reading up intensively I've decided to pull the trigger and start my own build thread. 
I'm aiming for a dual rear drive setup.

What I currently have planned:
Board: Loaded Dervish
Trucks: Randall R2 baseplates & bushings + Paris 195 hangers
Motor mounts: Torqueboards V1
Motors: dual RSPEC 6355 190kv
Motor management: dual VESC
Controller: Nunchuck

I need to sort out batteries soon, but I'll go with Lipos because I already own two balancing chargers.
More on that later.
```

---
## \#2 Posted by: trbt555 Posted at: 2015-11-21T15:59:36.410Z Reads: 446

```
First problem: the Paris hangers are not cylindrical, causing the motor mounts to diverge.
After asking for advice on the other forum, I decided to modify them.

I wish I had access to a lathe but I made do with what I have.
I put the hanger into a drill press and added a wheel at the bottom to stabilize the whole thing. Weird, even new hangers have bent axles.
<img src="/uploads/db1493/original/2X/7/779d7a74e48fdfffb791dc274deea601cbfcdf15.jpg" width="375" height="500">

I then carefully filed away ath the rotating hanger until my washer (you can see it on the wheel) went all the way over.
After some light polishing this is the end result:
<img src="/uploads/db1493/original/2X/7/7da86e4fac76d61274e93cd8a5ea776bef01423a.jpg" width="666" height="500">

I transplanted the Paris hangers to the Randall baseplates on my Dervish and I kept the conical Randall bushings, which I really like. No noticable difference in handling with the slightly wider hangers.
I left the baseplates on because I'm too lazy to remove them, I had already countersunk them, and they've acquired a very nice patina over the years:
<img src="/uploads/db1493/original/2X/b/be1505d99d459ce62bf3b1205ffe9ec78dc91dcf.jpg" width="666" height="500">

With the modified hangers the motor mount flange is now perfectly perpendicular to the axle:
<img src="/uploads/db1493/original/2X/a/a918d23db9a4df955d2f005fe77762208a891830.jpg" width="375" height="500">

Contrary to some folks I'm really not interested in the aesthetics, as long as the board shreds. This is my trusty Dervish, I can say we've both been around the block a few times.
<img src="/uploads/db1493/original/2X/5/5b8a637f4b79b2accf9f81436ebff8d76c5e4343.jpg" width="666" height="500">

I'm waiting for motors, and then I'll decide if I'll keep them inboard or go outboard to the back. The dropthrough deck doesn't allow that much clearance so I think out to the back will be my best bet.
```

---
## \#3 Posted by: jakeyb2525 Posted at: 2015-11-21T16:07:22.445Z Reads: 399

```
Looking good...going to be a nice build :+1:
```

---
## \#4 Posted by: lox897 Posted at: 2015-11-21T20:41:32.722Z Reads: 395

```
Nice build! What are you using for an enclosure?
```

---
## \#5 Posted by: trbt555 Posted at: 2015-11-21T20:45:49.820Z Reads: 392

```
I have no idea yet what I'll be using.
I haven't given that a lot of thought yet.
Winter is long enough to figure something out.
```

---
## \#6 Posted by: onloop Posted at: 2015-11-21T22:43:29.562Z Reads: 376

```
great idea with the drill press...
```

---
## \#7 Posted by: siggs3000 Posted at: 2015-11-22T01:44:54.988Z Reads: 373

```
I used to have a Dervish and they are so damn awesome. One thing to watch out for is going to be board flex. They flex like crazy (being bamboo) so it's something to keep in mind when attaching parts to the board. The board will flex and your enclosure will have to be able to as well. Screws might not like that! Straps may be the way to go for this one.
```

---
## \#8 Posted by: kai Posted at: 2015-11-22T03:01:20.645Z Reads: 366

```
I agree on the board flex. They used to have two different levels of flex. Even the stiffer one i bottomed out sometimes when stepping hard on the edge of the board. I would worry putting anything under it for me. It is an awesome cruizin board though ... still love my loaded bhangra better! =p
```

---
## \#9 Posted by: trbt555 Posted at: 2015-11-22T08:14:46.051Z Reads: 369

```
Ah yes, the flex. And its a dropthrough.
That is what I like about the Dervish.
If I keep my components close enough to the trucks, I think I might get away with it.
```

---
## \#10 Posted by: kai Posted at: 2015-11-22T12:51:53.913Z Reads: 371

```
If worst come to worse....   You can always mount the trucks on the bottom and even add risers.
```

---
## \#11 Posted by: trbt555 Posted at: 2015-11-22T17:05:45.293Z Reads: 389

```
Today was battery day.
Considering the fact that I want to use 'fragile' Lipo's and the Dervish is quite flexy, I spent some time jumping up and down on the board in my garage this afternoon.
35mm thickness would be the absolute max and in that case I would need an enclosure capable of withstanding scraping the pavement when I max the board out, which I WILL do when carving, I'm not the lightest of riders. 25mm max would be ideal.

Voltage:
I think going with 12S makes the most sense as the current will be lower and the resistive heat losses will be considerably less.
With 12S, the 190kv motor, 90m wheels and a 15/36 reduction the calculated theoretical top speed would probably be too much for me but if I'm not mistaken the VESC will let me limit the motor RPM's to a comfortable level. Am I right ?

So I went onto the Hobbyking battery selector and it turns out only 4 x 3S would allow me to keep the thickness under 25mm.
At least 5000mAh should get me far enough.
Theoretically a dual R-spec 6355-190 setup would be 4800W installed power. At 44,4V the corresponding max total current would be 108A but I'm guessing that would be peak so I think continuous discharge rate for the 5Ah Lipo's should be in the 10 to 20C range, not higher. AND I can limit the battery current in the VESC anyway right ?

This query returns 5 options for the EU warehouse:
[img]/uploads/db1493/original/2X/7/7408bc701feb8a8659e150f10b287cffdc3a097e.jpg[/img]

1. [url=http://www.hobbyking.com/hobbyking/store/uh_viewItem.asp?idProduct=56839]Multistar High Capacity 3S 5200mAh Multi-Rotor Lipo Pack[/url]
Cheap, light and compact. What's not to like about these ?
Only 10C but if I read @okp's Vanguard thread correctly I could get away with these.

The next three are very similarly priced, have 25C rating and have more or less the same dimensions.

2. [url=http://www.hobbyking.com/hobbyking/store/uh_viewItem.asp?idProduct=8579]ZIPPY Flightmax 5000mAh 3S1P 20C[/url]

3. [url=http://www.hobbyking.com/hobbyking/store/uh_viewItem.asp?idProduct=9183]Turnigy 5000mAh 3S 25C Lipo Pack[/url]

4. [url=http://www.hobbyking.com/hobbyking/store/uh_viewItem.asp?idProduct=8583]ZIPPY Flightmax 5000mAh 3S1P 25C[/url]

Finally there's this one, which I don't really see the advantage of using, its expensive but it can be charged ad 5C, which my chargers won't do.

5. [url=http://www.hobbyking.com/hobbyking/store/uh_viewItem.asp?idProduct=11935]Turnigy nano-tech 5000mah 3S 25~50C Lipo Pack[/url]

To conclude, I think I'll risk ordering 4 of those cheap Multistars, unless any experienced users here on the forum have other recommendations ?
```

---
## \#12 Posted by: lowGuido Posted at: 2015-11-22T20:57:35.181Z Reads: 331

```
I have used the Zippy flight max on all of my builds for over a year now, I have put over 500km on them and they are still going stong.
the minimum I have used is 20C and there have been no issues so far.
I think as long as you care for them properly they will be fine.
lipos are great batteries just not idiot proof.
```

---
## \#13 Posted by: onloop Posted at: 2015-11-22T20:59:48.734Z Reads: 333

```
If I ever buy lipos again ill pay the premium and get the better ones, the zippy flightmax have let me down before.
```

---
## \#14 Posted by: treenutter Posted at: 2015-11-23T02:30:15.101Z Reads: 359

```
[quote="trbt555, post:11, topic:524"]
SC will let me limit the motor RPM's to a comfortable level. Am I right ?
[/quote]

That's right @trbt555 . RPM limits on VESC work perfectly. I'm using this feature now as I get used to my build and don't need to hit its top speed. This way I can test things without any worry. Remote signal drops? Enclosure falls off? Motor wire unattaches? NBD cuz I'm only going 12 MPH!
```

---
## \#15 Posted by: trbt555 Posted at: 2015-11-28T15:41:17.018Z Reads: 365

```
I made some progress today. 
This week I happened upon [url=https://www.rostimepal.com/en/lunchtime/lunchbox-take-a-break/lunchbox-take-a-break-flat-silver.html]these[/url] lunchboxes which turned out to be perfect for my build. They're flat (33mm), they have rubber seals and reliable latches and they're quite strong.
I temporarily mounted them on rubber bushings using M5 bolts through the deck. I drilled all holes slightly bigger to have some play to account for the board flex.
I pushed a few times around the block and took a few descents carving, the mounting seems te be rock-solid.

[img]/uploads/db1493/original/2X/6/6cc10ddf48d5c81b64120e7f8a946296010883f4.jpg[/img]
[img]/uploads/db1493/original/2X/c/c37aef11fe9f73b2469ae944afce1cf93c470eca.jpg[/img]
[img]/uploads/db1493/original/2X/4/422b2ff51aa9667107e0f3cf4d6a8fcefad413e3.jpg[/img]

I also made a cutout for the anti-spark loop key:
[img]/uploads/db1493/original/2X/d/d1b0980a2f9bca4bcb325a048b869e2ae6b52a68.jpg[/img]

I'm currently waiting for my fuse to arrive, after which I'll be able to mount & wire the batteries into the box.
I did go for the Multistar batteries after all, we'll have to see how they hold up once I get the motors & VESCS.
```

---
## \#16 Posted by: onloop Posted at: 2015-11-28T21:36:36.603Z Reads: 342

```
those boxes are perfect! great find.... i remember my countless hours of searching for the perfect pre-made boxes... walking around shopping malls looking like a box zombie... i think you nailed it with these!
```

---
## \#17 Posted by: lowGuido Posted at: 2015-11-28T23:13:11.448Z Reads: 338

```
those are some pretty nice boxes there. how are you going to wire it? battery in one box and VESC in the other?
also are you going to remove each battery for charging?
```

---
## \#18 Posted by: trbt555 Posted at: 2015-11-29T08:07:22.807Z Reads: 342

```
Yes, batteries up front, VESCs towards the drive side.
Because the lids are so easily removed, I'm keeping the batteries in the box, fixed with velcro.
I already own two chargers so I'll parallel charge 2 x 2 packs overnight.
```

---
## \#19 Posted by: trbt555 Posted at: 2015-11-29T20:07:27.312Z Reads: 358

```
Today I put the power meter in the drive-side box.
I like easy access so I didn't mount it to the lid but mounted it to the bottom of the box on a riser to bring the display up to the right level.
I wasn't happy with the look of the display in the cutout so I transplanted the original bezel:
[img]/uploads/db1493/original/2X/1/12dfac79c68847cfca24430c717edf1aecb98bcb.jpg[/img]

This week I'll be receivng my fuse and then I'll mount the boxes and wire them up.
Then comes the countdown to the November batch of Vesc...
```

---
## \#20 Posted by: treenutter Posted at: 2015-11-30T15:50:52.318Z Reads: 348

```
@trbt555 I ordered one of these lunch boxes as a replacement for my plastic screw-organizer enclosure that recently failed, thx for the inspiration! I made a flat spot on the bottom of my deck with epoxy. It also eliminates flex in that area (which you don't want, but I prefer). Are you going to line the interior of the box with anything so that it doesn't facilitate shorts? You mentioned some rubber bushings around the bolts but it also looks like there is a layer of black rubber\silicone between the deck and the boxes; is that a full sheet of rubber?
```

---
## \#21 Posted by: trbt555 Posted at: 2015-11-30T16:34:15.521Z Reads: 353

```
@treenutter No, I don't have anything like silicone inbetween, it just looks that way in the picture.

I'm using plain rubber bushings with a metal washer in them like these:
[img]/uploads/db1493/original/2X/a/a73575646fb4ffc6351df86415c263a0db3781c6.jpg[/img]

Here is a potato-quality close-up of how the box is mounted:
[img]/uploads/db1493/original/2X/d/dde4a2f5092a50904df395412f25ca31d9d1685f.jpg[/img]

No need to line the interior to prevent shorts, the boxes are plastic. 
I've found a way to avoid having M5 bolt threads protruding into the boxes too. 
I'll post pictures of that later, I'm short on time at the moment.
```

---
## \#22 Posted by: treenutter Posted at: 2015-11-30T18:24:13.735Z Reads: 340

```
thx @trbt555 I thought that they were metal ha!
```

---
## \#23 Posted by: hexakopter Posted at: 2015-12-01T12:08:07.044Z Reads: 337

```
I really like that design of the board, thumbs up.

The boxes are a good finding, but have the question if the dimensions "255 x 170 x 33" from the website are the inside of the box? Because than there will also 3 Multistar 5200mAh 4s Lipos fit and there is some space for the Vesc and the Turnigy wattmeter, so with an single motor one box is maybe enough.
```

---
## \#24 Posted by: trbt555 Posted at: 2015-12-01T12:42:07.769Z Reads: 341

```
I currently have 4 x 5200mAh 4S Multistars in one box and there is very little room left for much else:
http://www.electric-skateboard.builders/uploads/db1493/original/2X/6/6cc10ddf48d5c81b64120e7f8a946296010883f4.jpg
```

---
## \#25 Posted by: hexakopter Posted at: 2015-12-01T13:09:26.831Z Reads: 325

```
Sure you have 4 x 4s? So that would be a 16s Lipo together?

I think you are using 4 x 3s. :smiley: The 3s are 142 x 49 x 22 and the 4s 142x49x29.
```

---
## \#26 Posted by: trbt555 Posted at: 2015-12-01T19:06:17.003Z Reads: 328

```
@hexakopter Yes you're right I wasn't paying attention when I posted...
I measured the boxes up for you.
Inside dimensions are approx. 233x163x30mm.
```

---
## \#27 Posted by: trbt555 Posted at: 2015-12-01T19:07:05.581Z Reads: 333

```
Finally wired up the battery box.
Now waiting for the VESC's and motors...
[img]/uploads/db1493/original/2X/6/64129b61d2d20f06a745fd148f3989bf7bf32b3b.jpg[/img]
```

---
## \#28 Posted by: hexakopter Posted at: 2015-12-01T21:58:44.381Z Reads: 329

```
Thanks a lot for measuring it. So the 29mm high 4s Lipos maybe also work when it is possible to put the XT60s between them.

I am very new to eSkateboards and you are there first person who will use a wattmeter. The idea is great and a wattmeter is also on the way to me. :smiley: But on an electrical point of view I am not sure if it will work with the regen of the VESC. I am not sure if the current in the opposite direction will maybe destroy the wattmeter? I really don't know. Do you or any other person has tested that?
When the consumed mA are not displayed correctly, because the energy going back in to the Lipos that would not be a problem for me, but when it will destroy something that would be bad.
```

---
## \#29 Posted by: trbt555 Posted at: 2015-12-01T22:30:16.517Z Reads: 328

```
Yes, been thinkg about that too.
I'm certainly not the first to use a wattmeter.
This guy is also running VESCs with a wattmeter: [thread][1]

If I'm not mistaken regen braking can be turned off/disabled in the VESC if necessary.


  [1]: https://endless-sphere.com/forums/viewtopic.php?f=35&t=71511
```

---
## \#30 Posted by: onloop Posted at: 2015-12-01T23:38:06.272Z Reads: 326

```
[quote="trbt555, post:29, topic:524"]
If I'm not mistaken regen braking can be turned off/disabled in the VESC if necessary
[/quote]

you can turn it off but you won't have any brakes at all.
```

---
## \#31 Posted by: onloop Posted at: 2015-12-02T00:00:22.137Z Reads: 332

```
My personal option is that a permanently attached/ built-in watt meter is mostly useless.

there are a few reasons why I say this;
1. they only show real time data when your riding
2. they display only the peak/max data once stopped.

so if you want to know how much power you are using/outputting for any given moment you need to be looking at the screen whilst riding, waiting for the info to scroll through, which is very unsafe! ALSO, as most people mount them beneath the board you can't actually see the real time data which is what I believe is the most important.

I want to know how many amps I'm pulling on the flat vs hills vs coasting along a light decline etc - it doesn't offer that info when mounted roadside.

When mounted roadside basically you need to get off the board to see any data, it can show peak watts & ah / wh consumed etc. Which is useful info for testing a drive train or new motors/ But really that is not data you need on a daily basis. When you think about it you really only need to know how much battery you have remaining. 

permanent watt meters fall into the bling category.

Save the money & space.
```

---
## \#32 Posted by: trbt555 Posted at: 2015-12-02T07:04:49.895Z Reads: 314

```
So if i set negative battery current limit to zero, I lose all braking ?
Won't be doing that then....
```

---
## \#33 Posted by: onloop Posted at: 2015-12-02T07:14:12.501Z Reads: 304

```
correct. regen braking is the only type of braking it does.
```

---
## \#34 Posted by: hexakopter Posted at: 2015-12-02T19:59:07.847Z Reads: 312

```
[quote="trbt555, post:29, topic:524"]
I'm certainly not the first to use a wattmeter.This guy is also running VESCs with a wattmeter: thread
[/quote]


Sorry for the misunderstanding, but I mean you are the first person "I saw" using a wattmeter. Thanks for the link, I will ask him how the regen is working with the wattmeter.
```

---
## \#35 Posted by: trbt555 Posted at: 2015-12-21T09:10:35.003Z Reads: 303

```
Woohoo, I just paid an obscene amount of import duties to get my r-specs and vescs thru customs and now delivery is slotted for tomorrow.
Impressively short delivery time from the other side of the globe.
Feels like christmas !
I'll be sure to post progress soon.
```

---
## \#36 Posted by: kai Posted at: 2015-12-21T13:57:58.212Z Reads: 298

```
Where do you live bro? I had to pay 11 usd on my space cell. Didnt get a bill on my vesc.
```

---
## \#37 Posted by: trbt555 Posted at: 2015-12-21T14:17:30.169Z Reads: 311

```
In Belgium. It was like 25% of the total value.
Belgium is well known for its chocolate and high taxes ;-)
```

---
## \#38 Posted by: kai Posted at: 2015-12-21T14:49:49.236Z Reads: 312

```
wow! 25% damn bro! that is some high tax
```

---
## \#39 Posted by: cmatson Posted at: 2015-12-21T14:51:53.503Z Reads: 323

```
[quote="trbt555, post:37, topic:524"]
Belgium is well known for its chocolate and high taxes :wink:
[/quote]

Belgium waffles? real or stereotype?
```

---
## \#40 Posted by: trbt555 Posted at: 2015-12-21T15:20:17.147Z Reads: 325

```
Waffles are for tourists.
```

---
## \#41 Posted by: trbt555 Posted at: 2015-12-23T05:58:30.122Z Reads: 328

```
I finally made some progress on the drive-side box.
I mounted the VESCs on standoffs. The nuts on the motor side of the VESC were scary close to the phase wires, so I put some heat shrink over them.
(Those M2.5 nuts are damn tiny !)
Same thing for the PPM pins.
I had to shorten the battery wires on each VESC in order to tame the spaghetti monster somewhat.
<img src="/uploads/db1493/original/2X/1/17e4f7426ca78b65b0a5d1fea3e824bd32c161a4.jpeg" width="375" height="500">
 
Tomorrow I'll tackle the mechanical side and mount the motors on the board and maybe hook everything up for a bench test.
```

---
## \#42 Posted by: locktight Posted at: 2015-12-23T11:20:13.144Z Reads: 315

```
Your battery wires are going to end up being pretty long with the spegetti and the wire connecting your 2 boxes. The vesc come with 3 beefy capacitors to deal with this however your wires are so long I think youre pushing the limit. You should probably shorten your spegetti monster a bit to cope with this. Good luck with the rest of your build.
```

---
## \#43 Posted by: trbt555 Posted at: 2015-12-25T20:35:55.160Z Reads: 319

```
Finally found the time to put the drivetrain together.
Belt alignment seems to be acceptable, will have to see how it goes once I can spin the wheels with the motors.
These Enertion R-SPEC motors are a thing of beauty.
<img src="/uploads/db1493/original/2X/e/e0ec1f6d8755fe0309eba6204ee8ecd6ade93523.jpg" width="666" height="500"><img src="/uploads/db1493/original/2X/a/a6485d87612c35ba69fac28eba40a591c99670eb.JPG" width="666" height="500">

Note to self: don't forget threadlocker on all bolts before first ride ;-)

I also managed to hook up the Nunchuck RX to a longer set of wires so I can put it on the other side of the box.
I put the RX back into its little case to give it some protection. I'll probably hot-glue or double-side-tape the RX into the box somewhere.
<img src="/uploads/db1493/original/2X/1/156b025e1108ba15eabe7779e9421069a55fa43b.JPG" width="666" height="500">

I powered up the VESCs for the first time today. Updated the firmware using the 2.5 BLDC tool for OSX without a problem.
Configured them as master/slave.
I tested the Nunchuck connection to the master VESC, all seems to be OK.

Is there any way to 'listen in' to the CANbus communication to see if the VESCs are talking without having to power up the motors ?

In the next few days all will be coming together.
```

---
## \#44 Posted by: trbt555 Posted at: 2015-12-25T20:55:17.273Z Reads: 308

```
I just took a second look at the BLDC tool and managed to answer my own question: In the realtime data tab you can listenin to the CAN data coming from a slave by clicking CAN Fwd and entering the slave ID:
<img src="/uploads/db1493/original/2X/5/5507ed1800c4955142da770ac6b122e4c53450ec.jpg" width="434" height="500">
I got realtime data from my slave VESC so all is looking good for a bench test under real power soon.

Another note to self: set input voltage shutoff to correct value before test ride.
```

---
## \#45 Posted by: NIK Posted at: 2015-12-25T21:11:02.755Z Reads: 278

```
Hi, could you post pictures of both your ESCs connection? pretty please :smile:
```

---
## \#46 Posted by: NIK Posted at: 2015-12-25T21:11:34.328Z Reads: 275

```
and your power supply wiring.
```

---
## \#47 Posted by: trbt555 Posted at: 2015-12-26T09:43:09.339Z Reads: 292

```
Hi @NIK, I don't have access to my board at the moment but if you scroll up you'll find a picture of the drive-side box containing the VESCs.
The battery leads come into bullet connectors, from which I run a wire to each VESC so thats 2 wires per bullet connector, soldered on.
The CANbus connection is just a set of connecting wires between the two middle pins on the 4-pin connectors.
I'm not sure this answers your question, feel free to ask.
I'll post a picture of the finished box later today after I've finished my post-christmas chores ;-)
```

---
## \#48 Posted by: trbt555 Posted at: 2015-12-26T16:41:23.191Z Reads: 297

```
Here's a picture of the finished drive side:
<img src="/uploads/db1493/original/2X/2/22587f04ecd88b8b7920df8758478fac113e78a8.jpg" width="666" height="500">
```

---
## \#49 Posted by: NIK Posted at: 2015-12-26T16:59:26.884Z Reads: 295

```
That is super clear wiring pictures. Thanks, dude and merry Christmas :smile:
```

---
## \#50 Posted by: trbt555 Posted at: 2015-12-27T18:57:50.880Z Reads: 305

```
I didn't let having [only one VESC][1] VESC stop me from doing my first test ride today.
I left the unused motor on the board but removed the belt.
I was quite surprised to find only one motor was sufficient to drag my 90kg ass up some hills.
I can't wait to find out what 2 motors will do !

I added a tie-wrap around my battery box to make sure I wouldn't spill my cells on the pavement on my first ride:
<img src="/uploads/db1493/original/2X/9/90a5d1b7d6551688c676ab469329cff4249690b3.jpg" width="500" height="500">

Weather was great for the time of year, and carving on the 90mm flywheels was buttery soft:
https://www.youtube.com/watch?v=vC15-rRvIT0

Some stats:
Distance covered: 10.8km
Average speed: 18.23kph
Max speed: 39kph (I had the ERPM limited, this was downhill)

Peak current: 23.27 A
Peak power: 1114.6W
Battery charge used: 2139mAh

Start voltage: 49,87V
End voltage: 46,11V

I'm not happy with the range of these Multistar 5200mAh batteries, it appears their capacity spec is inflated, I have only been able to draw rougly half the charge of what was specified.
Towards the end of my ride I could clearly feel the batteries increasingly not being able to cope with the hills, which was a bit of a disappointment. I might go for a second set of Zippy Flightmax cells after all.

I was very pleased with the Nunchuck connection, no dropouts at all. Pretty impressive range too. At one point I had my youngest daughter riding the board with me on the stick and at about 10-12m distance I would typically lose the connection.

  [1]: http://www.electric-skateboard.builders/t/enertion-vesc-failure-please-help/812/6
```

---
## \#51 Posted by: lowGuido Posted at: 2015-12-27T20:34:02.448Z Reads: 285

```
Excellent build.
Im really looking forward to your dual motor stats.

A lot of people are surprised by single motor power but there's this myth of dual motor being the only way floating around here.
```

---
## \#52 Posted by: psychotiller Posted at: 2015-12-27T22:17:49.760Z Reads: 283

```
We've never needed 2 motors to climb hills. I weigh 200lbs and haven't had an issue with speed or hills from day one. 63mm motors, 150a car escs @ 6s and 15mm belts has always worked well. The dual motor hype started with boosted. Twin 63's @ 12s is overkill.
```

---
## \#53 Posted by: trbt555 Posted at: 2015-12-28T15:35:38.227Z Reads: 286

```
Second test ride today.
This time on flat ground (23m climb) and pretty steady speed using the cruise control

Distance: 9.36km
Avg speed: 18.3kph
Peak power: 1035W
Peak current: 22,5A
Charge used: 2019mAh
End voltage: 45,9V

Max speed on this run was 30,5kph, which corresponds nicely to the theoretical speed I calculated using a max ERPM of 30000 (which corresponds to approx. 4286 mechanical rpm on a 14pole motor) I had set in the VESC to protect me from myself :smile: 

The batteries suck, they should be giving me double this range. It was only 12°C but I don't think it's the temperature. I think I got what I paid for.

No nunchuck dropouts.

I did manage to trip the VESC hard (ie not soft) twice, each time it happened when I tried to overtake a cyclist and accelerated hard. 
I have no idea why this happened. Any ideas ?
```

---
## \#54 Posted by: Jeff Posted at: 2015-12-28T16:42:03.992Z Reads: 273

```
Hi trbt555, 

It looks like you are using 12S, so shouldn't you be able to safety run on voltages from 50.4 to 38.4 (assuming starting at 4.2V per cell and ending at 3.2V per cell)? It looks to me that you should have quite a bit of capacity left if your end voltage is 45.9V.

I experienced similar behavior with my now dead VESCs. I pushed them hard, they cutout, and never came back. Ended up faulting the DRV chip on one and a temp sensor on another. I am not sure if this is an issue with that batch of VESCs or what. I have one coming from @chaka with heat sinks that I will try out next.
```

---
## \#55 Posted by: trbt555 Posted at: 2015-12-28T17:18:06.824Z Reads: 274

```
OMG @Jeff you're right I don't know how I came up with 3,7V per cell !?
Thanks for the wake-up call.
I had somehow set my cutoff voltage and hadn't given it any further thought.
Apparently I've been leaving half the capacity in the battery.

I retract my earlier statements regarding the Multistars pending further testing.

On the issue of tripping the VESC: I'll see if I can log someting on my next ride but it does seem similar to what I saw on my bad VESC: push the stick and the VESC just shuts down and reboots.
```

---
## \#56 Posted by: chaka Posted at: 2015-12-28T17:50:19.614Z Reads: 269

```
You were most likely tripping the low voltage cuttoff if you had it set at 44.4v. The voltage will sag under high current use. One way to combat voltage sag is by adding more capacity.
```

---
## \#57 Posted by: trbt555 Posted at: 2015-12-28T20:28:20.617Z Reads: 265

```
Yep, probably the Multistars not being able to cope.
Am I correct that I could counteract this by limiting the battery current in the VESC ?
```

---
## \#58 Posted by: chaka Posted at: 2015-12-28T20:44:33.450Z Reads: 264

```
Yes, adjusting your max current settings will help. You may not need to once you adjust your low voltage cutoff.
```

---
## \#59 Posted by: treenutter Posted at: 2015-12-29T03:08:46.718Z Reads: 268

```
[quote="trbt555, post:53, topic:524"]
I did manage to trip the VESC hard (ie not soft) twice
[/quote]


@trbt555 Thanks for these updates; I appreciate the testing and the feedback. When you say that you tripped your VESC what did that feel like? What was the result? I'm thinking back to a few times I thought that I lost controller signal with a nunchunk, and I think that they were all during hard acceleration and before I fully configured VESC for my setup. If you were accelerating hard and the VESC reboots, did you get tossed?
```

---
## \#60 Posted by: trbt555 Posted at: 2015-12-29T08:19:09.292Z Reads: 271

```
I think @chaka could be right, because my low voltage cutoff was set so high, I was probably tripping it by demanding too much from the batteries.
I don't think it was the nunchuck.

What did it feel like ? I hit the stick to overtake a cyclist and all of a sudden I'm no longer on the board but running. It just cut off all power.

I'm actually very happy with how the nunchuck/VESC control feels. Very precise, braking is just right. @onloop made it very easy by putting default r-spec settings in the VESC.

On the mechanical side, My board seems to have a few rattles that are bothering me, I'll need to straighten those out too.
I've owned Flywheels before, but these ones tend to "creak" like a new shoe when rolling. I hope this is only part of the run-in process.
```

---
## \#61 Posted by: trbt555 Posted at: 2015-12-29T17:43:35.573Z Reads: 286

```
OK, now this is getting seriously fun !

Third test today on flat terrain with these modified settings:
Batt max: 30A
Battery cutoff start: 39,6V
Battery cutoff end: 38,4V
Max ERPM: 40000

Stats:
Distance: 21,38km
Avg speed: 20,35kph
Top speed: 37,5kph
Charge used: 4850mAh

No more cut-offs when accelerating.
No nunchuck dropouts either.
Me happy :smile:

I tried hitting 40kph but got speed wobble because I had my trucks way too loose so I backed off.
I'm pretty sure that within a few rides 40kph will not feel fast at all.

Towards the end of my ride the VESC unexpectedly cut off the power twice but my wattmeter was still showing 44V by the time I turned the board over to look.
The wattmeter was also reading a peak power of 4125W, which is impossible.
I think it can't cope well with the regenerative braking. It may fail soon.
I was probably hitting the lower cutoff voltage so I kept off the stick and rode the last few hundred meters at snail pace. Because you know, pushing sucks ;-)

So, the batteries ain't as bad as I first thought. I'd say acceptable for the price.
Anyways, my Zippy's arrived today so if the weather keeps up I'll give those a try later this week to see how they compare.

I hit a few rough patches with some loose gravel, the Flywheels just ate that gravel up. 
The R-SPEC's on the other hand, got pummeled:
<img src="/uploads/db1493/original/2X/1/17cda6db9b285deb582574d61983af2ebc0b3215.JPG" width="500" height="500">
But hey, a good tool wears signs of use well ;-)

I removed the unused motor though. No use dragging it around for nothing.
I hope my VESCs from @chaka come soon, dual drive will be insane.

I also started an offensive against rattle.
I found one of these dampening mats at the local hardware store and put some in my control box, to prevent wires rattling.
I also added some thin dampening material to keep the wattmeter from rattling against the lid:
<img src="/uploads/db1493/original/2X/1/1e8c3f7ea89d4b075ba2ecf8f530e4bbce0f7a11.JPG" width="666" height="500">
```

---
## \#62 Posted by: trbt555 Posted at: 2016-01-02T16:47:12.793Z Reads: 275

```
My Zippy Flightmax Lipo&#39;s arrived but the weather was bad and I was bored so I decided to see if I could take an objective approach to setting the low voltage cutoff and whether or not I would need different settings for different Lipo packs.
So I had some good clean geeky fun with my Arduino and did a discharge test.
I set up the Arduino to measure the pack voltage over the balance plug while I discharged the Lipo over a 35W halogen bulb. I had the Arduino send a timestamp and the measured value over the serial port to my PC, from where I could import data into Excel. 
I had a cell voltage monitor/alarm set up at 3,6V so I could leave the setup alone until stuff started to get interesting.
The 35W bulb drew a current of approx 2,8A. Unfortunately I didn't have anything more powerful, it would have been fun to see the effect of a larger discharge current, especially a current close to the max discharge rating.

My setup:
<img src="/uploads/db1493/original/2X/7/7df4d552e0046c6403f0ae0bbc1a06f182277e1c.jpg" width="666" height="500">
The results:
<img src="/uploads/db1493/original/2X/d/d4dcd54a8a7563253d5fb0cfa60cd9525c0d83d2.PNG" width="690" height="449">

Some observations:

 - 3,6V per cell will be a good cutoff limit for both packs. Under 3,6V the voltage drops VERY fast. It took both Lipo's about 15 min. to reach 3,0V coming from 3,6V at approx 2,5A, imagine how fast the voltage drops when you're drawing 10 times that current.
 - Both curves show a small dent at 4,0V, I don't know what is going on there, it could have been someting in my setup.
 - The Multistar takes 13% longer to discharge to 3,6V while it only has 4% more capacity, while the current in both tests was identical. I don't know how accurate my test was but one thing for sure, range with the Zippy's will be shorter.

If I ever decide to repeat this kind of test, I'll put my wattmeter in the circuit as well and maybe even have Arduino monitor and log individual cell voltages, and have it shut off automatically at 3,0V

Now I'm waiting for the weather to clear so I can go out and do a real-life test.
I'm also brooding on the idea of having my Arduino log values from the VESC's over CANbus and store them on an SD card, while also logging accelerometer data, which would give me useful data to analyse after a ride.
```

---
## \#63 Posted by: trbt555 Posted at: 2016-01-08T17:10:59.060Z Reads: 254

```
I had a quick ride after work on the Zippy's, on flat terrain.
Distance 17km / 10,5miles
Avg speed 24kph / 15mph
End voltage: 3,6V per cell
They definitely don't get me as far as the Multistars, so contrary to my earlier conclusions, for a mellow riding style on flat terrain the Multistars really give bang for buck.
I hope the weather stays OK so I can try the Zippy's on some hills.
```

---
## \#64 Posted by: chaka Posted at: 2016-01-08T17:38:27.189Z Reads: 258

```
Temperature plays a huge role in how much range you get out of your pack. As the temps drop you not get as much range. Something to keep in mind whilst comparing different brands.
```

---
## \#65 Posted by: trbt555 Posted at: 2016-01-08T17:58:01.038Z Reads: 251

```
Yeah I know from my RC days. Temperatures were similar to my other rides.
But what I really would need to do is run the Multistars empty and switch to the Zippy's on the same ride. 
Only, I can't find a route long enough :smile:
```

---
## \#66 Posted by: massy Posted at: 2016-01-12T22:08:46.028Z Reads: 250

```
I think I can top you! Bought stuff for around 2600 SEK and 826 SEK import duties, that's almost 32%... 

25% sales tax + 2.6% customs and always 100 SEK in processing costs :'(

Build looks really good, gonna build a quite flexy one quite soon too. I feel like the board flex will be my greatest challenge. Backup plan is to just get a stiff board lol.
```

---
## \#67 Posted by: trbt555 Posted at: 2016-01-13T21:11:16.181Z Reads: 257

```
Due to the bad weather and no daylight after hours I've been working on a Lipo display/alarm.
It's a small 128x64 pixel OLED display which will be visible on the top of my deck so I can keep an eye on things.
Got the code running and the hardware sorted on the test bench. I'll be able to display live data from the vesc as soon as I've sorted getting it back over CANbus. Don't hold your breath though. I have a day job ;-)
<img src="/uploads/db1493/original/2X/d/db6ab16afa3c51e886d7aaab98dbbb49f4b4e338.jpg" width="666" height="500">
```

---
## \#68 Posted by: laurnts Posted at: 2016-01-27T17:37:53.840Z Reads: 253

```
I am using the same box as well. It's from Rosti Mepal! I was doubting about the thickness, but apparently its really the perfect size.
```

---
## \#69 Posted by: laurnts Posted at: 2016-01-27T17:39:25.302Z Reads: 250

```
This is a Rosti Mepal Flat Bread Lunch Box made in the Netherlands.
Materials is ABS.
https://www.rostimepalshop.nl/to-go/lunchbox-take-a-break/lunchbox-take-a-break-flat-silver.html
```

---
## \#70 Posted by: hexakopter Posted at: 2016-01-31T14:19:32.522Z Reads: 246

```
My build comes closer and I also want to use these boxes. Should one buy them over the internet or can one buy them in some shops located in the Netherlands?
Did you buy them from your link or in a local store?
```

---
## \#71 Posted by: laurnts Posted at: 2016-01-31T14:29:47.473Z Reads: 246

```
I have bought them both in local stores and online. Sometimes it's slightly cheaper in the local stores, but normally they didn't have the same colors for two pieces or more. So last time I decided to get them online from the link I've posted.

[quote="laurnts, post:69, topic:524, full:true"]
This is a Rosti Mepal Flat Bread Lunch Box made in the Netherlands.Materials is ABS.https://www.rostimepalshop.nl/to-go/lunchbox-take-a-break/lunchbox-take-a-break-flat-silver.html
[/quote]

And I have it black on my build by spray painting it.
```

---
## \#72 Posted by: trbt555 Posted at: 2016-01-31T15:23:08.454Z Reads: 228

```
I got mine in a local store around the corner. They're literally eveywhere.
```

---
## \#73 Posted by: hexakopter Posted at: 2016-01-31T16:07:08.990Z Reads: 231

```
Ok, thank you both. Will have a look then next time.

@trbt555 Could you tell me what local shop it was? Vaals doesn't have that many. :smile:
```

---
## \#74 Posted by: treenutter Posted at: 2016-02-02T21:46:47.853Z Reads: 239

```
I bought two of these as well. Perfect fit for 2 4s 5000MAH batteries, a VESC, and receiver. My winter project is to to paint it and get it installed. It's very slim, and appears very durable.
```

---
## \#75 Posted by: laurnts Posted at: 2016-02-02T22:29:08.334Z Reads: 248

```
Thats great! Btw I used t fit 2 3s 5000mah battery, 100A ESC, 2 Rocker switch, RX receiver & telemetry, 1 10000 micro farad capacitor, a fan and a SBEC lol. Thats like mega tight fit!

This is my version 3 build before, but somehow 5000mah just seems to be too short of a distance.
<img src="/uploads/db1493/original/2X/2/2752d6d09332db6ba06a2698d87965934f0d2dc9.jpg" width="464" height="500">
```

---
## \#76 Posted by: treenutter Posted at: 2016-02-03T16:06:54.942Z Reads: 241

```
@laurnts Yes that is a snug fit, but I like it! I prefer to have everything enclosed in a small unit with minimal wasted space. Have to keep an eye out for shorts though :smile:
```

---
## \#77 Posted by: trbt555 Posted at: 2016-02-25T13:31:38.545Z Reads: 246

```
Been making some progress on my DIY battery status display.
I finally found the time to draw a housing in Sketchup and have it printed via 3Dhubs.com, which by the way is awesome.
<img src="/uploads/db1493/original/2X/8/84b4a082a0f2904a962b653c37a853fa03c50afc.JPG" width="579" height="386">

Soldered a JST connector to the OLED display, and fixed it in place with some hot-snot:
<img src="/uploads/db1493/original/2X/5/51060edad6f8dd6cf1936e03b8905161c5dbbe91.JPG" width="686" height="500">

Finished product after I pimped it with some carbon-vinyl:
<img src="/uploads/db1493/original/2X/3/35838ba6a70f040652209abd4e7cf3485a8aa376.JPG" width="598" height="422">

Next steps will be migrating the prototyped Arduino Uno setup to a dedicated Arduino Nano board and (re)testing it on my board.
```

---
## \#78 Posted by: treenutter Posted at: 2016-02-25T14:08:41.534Z Reads: 231

```
@laurnts FWIW I have two 4S 5000mAh Lipos in mine and I get about an hour of ride time, Zippy compacts help to reduce some of the size.
```

---
## \#79 Posted by: treenutter Posted at: 2016-02-25T14:09:05.313Z Reads: 234

```
@trbt555 This is really cool!
```

---
## \#80 Posted by: trbt555 Posted at: 2016-03-11T16:34:59.920Z Reads: 235

```
I finally got a repaired high outputVESC back from @chaka so I'm back in business with my dual setup.
I made some changes to the tail shape of the deck in order to gain some clearance between the motors and the pavement:
<img src="/uploads/db1493/original/2X/4/4765d43864437e64ab58e5df64c93fe941eaad42.jpg" width="666" height="500">

Now I need to add some griptape over the mounting bolts fo the boxes and add my on-board display and I'm at my final config.
<img src="/uploads/db1493/original/2X/8/817abe3ffb2383ce6904561cc0adca3c7273f406.jpg" width="666" height="500">

I took the dual setup for a spin around the neighbourhood, this thing is a beast.
```

---
## \#81 Posted by: trbt555 Posted at: 2016-03-13T16:42:28.239Z Reads: 231

```
After a sunny weekend and a lot of riding my dual setup on a hilly route with lots of acelleration/braking some observations:

42A peak current draw, 1900W peak power
Approx 50 min run time, average 18km.

 - Insane acceleration, even uphill, great braking =  safer when lots of
   pedestrians are around.
 - More weight in the back: easier to break out into a standup-slide when carving hard.
 - More drag when in idle, coasting or downhilling doens't feel as natural.
 - More noise.

I liked the whine of a single motor setup, I'm not sure about the dual. The whine is just too loud, it tends to draw too much attention. (Is there anyone out there running dual R-specs in FOC mode without issues ?)
I'm not sure whether or not a dual is worth it compared to the single, I guess it depends on the type of riding I'm doing.
```

---
## \#82 Posted by: Iceni Posted at: 2016-03-13T18:40:49.498Z Reads: 230

```
I got my dual r-specs running fine with FOC, did a 40 minute run yesterday without a hitch.
Though it's the first real run I've made with an eboard ever, so I don't really have anything to compare it to.
I might switch it over to bldc mode just for comparison sometime.
```

---
## \#83 Posted by: matt Posted at: 2016-04-06T14:24:12.098Z Reads: 217

```
here's what i did with my loaded dervish, used two diy battery packs made from ncr18650bd (which i built for my fixed wing drones) - range is incredible with these 520wh batteries. 

https://www.youtube.com/watch?v=anB4oZ5n1Mw
```

---
## \#84 Posted by: trbt555 Posted at: 2016-04-06T16:22:14.627Z Reads: 216

```
Dude that is some slick video editing you did there. Great job !
I also like your maker-space.
Are you inspired by Casey Neistat by any chance ?

Massive batteries by the way, no ploblems hitting the pavement with flex ?
```

---
## \#85 Posted by: Ulfberht Posted at: 2016-04-06T22:42:17.362Z Reads: 204

```
@trbt555 I really like your build. Any updates on your build. Thoughts? Observations? Anything you would do differently?
```

---
## \#86 Posted by: matt Posted at: 2016-04-06T22:45:53.506Z Reads: 211

```
[quote="trbt555, post:84, topic:524, full:true"]
Dude that is some slick video editing you did there. Great job !
I also like your maker-space.
Are you inspired by Casey Neistat by any chance ?

Massive batteries by the way, no ploblems hitting the pavement with flex ?
[/quote]

surprisingly no, never touched the concrete even once. i made stiff wooden cases for the batteries though which takes away some of the flex. more about that in the upcoming part2 (soon hopefully).

the video style: definitely inspired by neistat. the workspace not so, had this long before i ever heard of casey ;)
```

---
## \#87 Posted by: NIK Posted at: 2016-04-07T08:51:54.944Z Reads: 206

```
Awesome editing video. and good explanation too.You just missed out the binding process, but that is really small matter. I really like the kegel wheels. We want more, more! XD
```

---
## \#88 Posted by: trbt555 Posted at: 2018-11-10T12:11:34.590Z Reads: 43

```
Ok guys, I’m getting out of the game, and selling my complete setup above, including components, spare parts etc.
Europe only. Contact me if you’re interested.
```

---
## \#89 Posted by: Grozniy Posted at: 2018-11-10T13:04:28.921Z Reads: 41

```
could you post all components that you're selling?
```

---
## \#90 Posted by: briman05 Posted at: 2018-11-10T13:34:42.387Z Reads: 41

```
You should probably make a new thread in the parts section
```

---
