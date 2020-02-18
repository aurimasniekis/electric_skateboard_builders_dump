# Pneumatic setup: Psychotiller SixShooter wheels / Treenutter Mas deck / 2x Torqueboards 190kv 6355 motors / 10s4p battery with 30Q cells

### Replies: 47 Views: 3146

## \#1 Posted by: sash Posted at: 2018-01-02T22:53:06.882Z Reads: 395

```
Here is my pneumatic setup, which will be very similar to @mmaner's build.  (The main difference is that I am going to build a bigger 10s4p battery pack.)

Parts:

@psychotiller's 6x2 SixShooter wheels
2x @psychotiller's  Ripba motor mounts
195mm Paris trucks (V2, 50 degrees)
Red Ember (@treenutter) Caldera deck 
  Edit: Decided to use Red Ember (@treenutter) Mas dec
2x 190kv 6355 Torqueboards motors & 16T motor pulleys
2x VESC (either Focbox or Axle VESC)
10S4P battery pack with 30Q cells
XT90S antispark key
BMS (have not decided which one)
Enclosure (possibly space cell, need to decide)

Gear ratio: 16/60


More details:

(1)  I've already got @psychotiller's wheels & motor mounts.  The delivery was super fast.   The parts look gorgeous.  They seem to be high quality and precision made.  Also they are quite light.

(2)  @treenutter says that he has a queue of people who preordered decks, and he can start working on my deck only in a month or so.  I guess I have to wait for it.

(3)   I've used Torqueboards motors before and they work fine.

(4)  Battery:  I am going to build a 10S4P pack myself using 30Q cells.  I've got an Arduino spot welder, and last year I've built a battery pack for my Loaded Vanguard.  It was a lot of fun to spot weld the cells.

(5)  VESC:  I have a pair of new Axle VESCs, which I could use.  I also like Enertion's Focbox (aka VESC-X).   The latter has a heatsink, a protective case, and a form factor which makes them easier to fit into the enclosure.   I've successfully used Focbox's but I have not used Axle VESC's.

Does anybody have comments on reliability of Focbox vs Axle VESC?   Are they pretty much comparable?

(6)   I would like to minimize the number of electronic components in my board.  My theory is that the less electronic components the board has, the smaller the chance that a component fails while riding.

This means that 

(a) I'll use XT90S plug instead of electronic antispark switch.
(b) I will NOT use a fuse.
(c) I will NOT use a BMS for discharge.

I think that these choices are better for safety.  Maybe in this setup there is a higher chance to burn VESC. (One needs to be extra careful not to short circuit anything.)   But my safety is more important than VESC.
Any comments or opinions about it?

(7)   Enclosure.   I might use a space cell enclosure.   But I am also considering the fiberglass 12S enclosure from @Eboosted http://www.electric-skateboard.builders/t/loaded-vanguard-and-never-summer-reaper-enclosures-for-sale/17137/112

 Does anybody know how well it would fit the Caldera deck?


(8)   BMS.   I'll be using a BMS only for charging the battery.  But I need to decide which one.   

People here say good things about Bestech or Battery Support BMS.  But they are huge, and will not fit into the enclosure.

In my Vanguard build I used this cheap $10 BMS (suggested by @Eboosted):

https://www.ebay.com/itm/Max-40A-Balance-Battery-Protection-Board-BMS-PCB-For-36V-10S-10Packs-Li-ion-Cell-/311862435323?epid=508180040&amp;hash=item489c731dfb:g:yXoAAOSwX61ZCgP~

@Eboosted says that they work fine for him.  I have mixed feelings about it.  The first one stopped working after a  week.  I've ordered a new one, which seems to work Ok so far.   Also it took very long time for it to arrive from China.

To tell the truth,  I've been mostly using my Vanguard board without a BMS.   I was using a 10S balance changer to charge it.   I kind of like this solution, because I can easily monitor the cells.  But I needed to open the enclosure every time when I charged the board, which was a pain.

So I need to either

(a)  Find a small and relatively reliable BMS (for charging only), or

(b)  Find a clean and waterproof way to make charging port and balance connectors for charging with a balance charger without opening the enclosure.

Has anybody found a good solution to (b)?

Do you have other suggestions for a small BMS (for charge only setup)?

Actually, Enertion's space cell battery uses a BMS which is even smaller than the one linked above (and probably costs below $10).   It should be easier to fit in the enclosure.

Do you know what BMS the space cell uses and where to get it?


Any other comments and suggestions?
```

---
## \#2 Posted by: atenner Posted at: 2018-01-03T00:38:19.172Z Reads: 340

```
You could use a couple of these : 

https://rover.ebay.com/rover/0/0/0?mpre=https%3A%2F%2Fwww.ebay.co.uk%2Fulk%2Fitm%2F132279467307

gx16 connectors, cant seem to find a 10pin one :( 

And the metal waterproof cap is good:

https://rover.ebay.com/rover/0/0/0?mpre=https%3A%2F%2Fwww.ebay.co.uk%2Fulk%2Fitm%2F192085661998

you can get them with a rubber link instead of the chain
```

---
## \#3 Posted by: atenner Posted at: 2018-01-03T00:39:56.956Z Reads: 327

```
<img src="/uploads/db1493/original/3X/0/2/02a321d97309ed140819b98f7188ae5b63e79bd6.jpeg" width="690" height="388">
```

---
## \#4 Posted by: Pedrodemio Posted at: 2018-01-03T01:15:17.316Z Reads: 311

```
[quote="sash, post:1, topic:42596"]
(b) I will NOT use a fuse.
[/quote]

Nice build, but stupid logic, don’t skip the fuse, in case of problems it can at least increase the chances of saving your board, you, your house or more important the ones you love, people vastly underestimate the amount of energy stored in the battery’s we use and the damage they can make
```

---
## \#5 Posted by: mmaner Posted at: 2018-01-03T02:11:27.386Z Reads: 292

```
[quote="sash, post:1, topic:42596"]
a clean and waterproof way to make charging port and balance connectors for charging with a balance charger without opening the enclosure.
[/quote]

I would use a 15 pin VGA connector, female on the board side. Mine has been a great board, you will live it 😊.
```

---
## \#6 Posted by: sash Posted at: 2018-01-03T03:17:21.000Z Reads: 295

```
I was thinking a lot about a fuse for my previous build, but finally decided not to use it.  Let me explain why.   

With XT90S plug, when the board in not in use (the plug is unplugged) the battery is totally disconnected from the board.   It is as safe as storing your battery separate from the board in a fireproof container.  The fuse will do nothing because it is simply not in the circuit.

Now if the XT90S plug is plugged in and you are riding the board...  Imagine that you are going really fast and the board suddenly becomes uncontrollable.    This can happen if

(a)  Your VESC burns
(b)  Your fuse burns.

If you have no fuse, then (b) is impossible.   So your chances of survival are higher.

To see that this is not an imaginary possibility, but this really happens, check out what @Jinra wrote here: 

http://www.electric-skateboard.builders/t/what-fuse-do-you-use/6457/41

This convinced me not to use a fuse.
```

---
## \#7 Posted by: GrecoMan Posted at: 2018-01-03T03:18:17.477Z Reads: 272

```
i’d just use a fuse for charging.
```

---
## \#8 Posted by: sash Posted at: 2018-01-03T03:23:53.691Z Reads: 270

```
Agree.  Fuse for charging makes sense.
```

---
## \#9 Posted by: mmaner Posted at: 2018-01-03T03:35:28.036Z Reads: 269

```
I don't use a fuse either as a general rule.  I have a 60a on my 6s build, but that's just in case of thermal runaway.  Prolly won't help that either. I'd rather burn up a vesc that have my board lock up at 25mph.
```

---
## \#10 Posted by: sash Posted at: 2018-01-03T03:40:01.741Z Reads: 262

```
I have the same logic.
```

---
## \#11 Posted by: sash Posted at: 2018-01-03T04:08:54.932Z Reads: 249

```
Thanks.  I'll check out these connectors.
```

---
## \#12 Posted by: sash Posted at: 2018-01-03T05:57:22.029Z Reads: 260

```
Thanks for the pointer about a VGA connector.  I'll give it a thought.  I did some search and found that people typically use a VGA connector in 6S builds.  But I think that it will work equally well in a 10S build.

I might use the following ports for charging:

XT60 connector for the main battery leads + 
VGA connector for balance leads.

One can probably connect all leads to a single VGA connector.   But I feel that a single VGA connector may not be able to handle higher amps (say, if I want to fast charge the battery at 6 amps).    Balance leads don't use a lot of amps, so VGA should be enough for them.  So XT60 + VGA seems like a solid charging solution.  

A quick question:  Is there a waterproof cover for a VGA connector?
```

---
## \#13 Posted by: sash Posted at: 2018-01-03T06:34:47.764Z Reads: 236

```
Here is an 11 pin GX20-11 aviation plug that might work for balance wires

https://www.ebay.com/p/4-X-Aviation-Plug-20mm-11-Pins-Gx20-11-Male-Female-Panel-Metal-Wire-Connector/1366196583?iid=231636267408

It is circular, so it is easier to mount it on the enclosure than a VGA connector.
```

---
## \#14 Posted by: sash Posted at: 2018-01-03T22:25:43.070Z Reads: 246

```
More thoughts on BMS vs no BMS....

I think that the most versatile solution for charging is to use no BMS module integrated in the board but to make a balance port in the enclosure (using a VGA or an Aviation plug connector). 

Pros:  I can easily monitor the cells, charge, discharge at any current (slow charge, fast charge) etc., using a 10S balance charger.

Cons:  (1)  A 10S balance charger is expensive. (But I already have it.)

(2)  The balance charger is bulkier and heavier than a small laptop-style power brick.  It is harder to put it in a backpack and charge the board at work, etc.

(3)  Instead of plugging in 1 plug, I need to plug in 2 plugs.  This is really not a big deal.


Solution to 1 and 2.   Take a small power brick and hot glue to it a cheap BMS.    This will make a small portable balance charger.   Basically, it will be charging through a BMS, but the BMS will not be inside the board but inside the charger.

Does anybody use this charging method?
```

---
## \#15 Posted by: davidbonde Posted at: 2018-01-11T09:18:00.236Z Reads: 197

```
The 195mm paris truck will handle the pneumatic no problem?
```

---
## \#16 Posted by: mmaner Posted at: 2018-01-11T14:07:33.517Z Reads: 201

```
[quote="davidbonde, post:15, topic:42596, full:true"]
The 195mm paris truck will handle the pneumatic no problem?
[/quote]

Yes, Ive don it, no issues.  Just pay attention to clearance on your deck, make sure you dont have any wheel bite.
```

---
## \#17 Posted by: sash Posted at: 2018-01-11T15:35:28.869Z Reads: 205

```
[quote="mmaner, post:16, topic:42596"]
Yes, Ive don it, no issues.
[/quote]

I've just got Paris 195 trucks.   Going to work on attaching Psychotiller motor mounts soon.  The difference in diameters of trucks and mounts is very small, less than 1/2 mm I think.  It might be enough just to sand the hanger a little bit.

Did you use sandpaper or a file for this? 

Also, did you use any riser pads with Paris trucks to avoid wheel bite?
```

---
## \#18 Posted by: Deckoz Posted at: 2018-01-11T15:39:34.198Z Reads: 207

```
@psychotiller
Hey man what tires are these? And will they fit superstars?

I'd like to try pneumatics on superstars before I purchase another set of hubs... Just the trampa 6.5s aren't out yet..7 is to big...6 would be preferable...
```

---
## \#19 Posted by: psychotiller Posted at: 2018-01-11T17:13:52.312Z Reads: 194

```
They won't fit superstar hubs. They are 6x2
```

---
## \#20 Posted by: mmaner Posted at: 2018-01-11T19:53:41.111Z Reads: 211

```
[quote="sash, post:17, topic:42596"]
Did you use sandpaper or a file for this?

Also, did you use any riser pads with Paris trucks to avoid wheel bite?
[/quote]

I used an end-mill to shape mine, but you could do it with a drill press and a little elbow grease.  

Measure the depth of the mount and mark that measurement with a sharpie or better yet a scratch awl on the hanger, all the way around.  Wrap the threaded end of the axle in paper, a lot of paper, then tape over it with electrical tape, a lot of tape.  This is to keep from damaging the threads.

Then chuck the axle into a drill press with as much pressure as needed but not too much, you just want it to hold not deform the axle.  Use some heavy grit sandpaper, like 50 grit or something, and wrap it around the place you want to shape and turn on the press.  You will want to stop a lot and measure the diameter until it is correct, you want it to be tight.  

If you find the sandpaper you are using is taking it down quick get to something close to the diameter you want then switch to a higher grit.
```

---
## \#21 Posted by: sash Posted at: 2018-01-12T05:03:29.848Z Reads: 175

```
Thanks a lot for the tips!  I might start with a higher grit, like 100, just to extend the pleasure of sanding the hanger.
```

---
## \#22 Posted by: sash Posted at: 2018-01-14T06:26:10.958Z Reads: 195

```
@treenutter  @psychotiller

I am tempted by the flexible Mas deck from @treenutter.  So I am trying to decide if I go the Caldera or the Mas route.   

The main challenge with Mas deck is fitting 10s4p battery into max 8.5'' x 8.5'' enclosure.   This might be tight, but can probably be done with careful planning.  I am thinking about this battery design: 
http://www.electric-skateboard.builders/t/loaded-vanguard-and-never-summer-reaper-enclosures-for-sale/17137/68
This way I can use the same battery as for my Vanguard build.

A few questions:

Has anybody done a similar build with the Mas deck?

Has anybody made a 8.5'' x 8.5'' enclosure for 10s4p battery? 

Can I drop mount the SixShooter wheels on the Mas deck without wheelbite?
```

---
## \#23 Posted by: psychotiller Posted at: 2018-01-14T08:54:31.198Z Reads: 177

```
I know the Sixshooters will work on the mas deck
```

---
## \#24 Posted by: treenutter Posted at: 2018-01-15T00:48:23.405Z Reads: 181

```
[quote="sash, post:22, topic:42596"]
Has anybody done a similar build with the Mas deck?
[/quote]

Not yet.

[quote="sash, post:22, topic:42596"]
Can I drop mount the SixShooter wheels on the Mas deck without wheelbite?
[/quote]

I believe so, but I need to test it. I’ve been planning to build up Mas with a similar setup (drop-through mounting and sixshooters). This is a part of the reason that it has such deep wheel cutouts.

@sash While the intent of the details in the middle is to increase flex at the center, I'm not sure how much that is true, especially if I render this in 9-ply. Most of the flex in comes from the narrow tails at either end. What I'm saying is that it you might be able to use a standard 10s4p pack and enclosure.
```

---
## \#25 Posted by: davidbonde Posted at: 2018-01-15T07:50:30.543Z Reads: 174

```
Mas deck? picture! :)
```

---
## \#26 Posted by: treenutter Posted at: 2018-01-15T17:15:14.264Z Reads: 185

```
[quote="davidbonde, post:25, topic:42596"]
Mas deck? picture! :slight_smile:
[/quote]

@davidbonde this is "mas"
 
![IMG_6677|500x500](upload://dhqxLujgpTyYwwtXguZIsFTMMCo.JPG)

![FullSizeRender|500x500](upload://vXnV0giiv8ILUlyEEouDKewUX99.jpg)
```

---
## \#27 Posted by: davidbonde Posted at: 2018-01-15T17:42:07.478Z Reads: 169

```
Cool - that looks like a looow ride!
```

---
## \#28 Posted by: treenutter Posted at: 2018-01-15T17:48:51.843Z Reads: 169

```
[quote="davidbonde, post:27, topic:42596, full:true"]
Cool - that looks like a looow ride!
[/quote]

It is low! 1" drop and drop-through mounting. But with 6" pneumatics (i.e. @psychotiller's 6shooters) it has perfect ground clearance.
```

---
## \#29 Posted by: mmaner Posted at: 2018-01-15T19:12:57.576Z Reads: 159

```
You need to make a top mount version of this deck.  Would be epic....
```

---
## \#30 Posted by: treenutter Posted at: 2018-01-15T19:34:48.970Z Reads: 158

```
[quote="mmaner, post:29, topic:42596, full:true"]
You need to make a top mount version of this deck.  Would be epic…
[/quote]

I can do that... someone order one :slight_smile:
```

---
## \#31 Posted by: sash Posted at: 2018-01-17T18:19:28.508Z Reads: 159

```
While I am waiting for a deck, I am trying to decide about electric components.   I want a simple and bullet-proof design with minimal number of components that can fail.   I read a lot of horror stories about batteries catching fire, so I want to be sure that everything is 100% safe.

I need some expert advise, especially from expert battery builders.

Here are my thoughts:

5.5 x 2.1 jack + VGA port for charging with an external balance charger.   This way I can easily monitor the cells every time I charge.

5-7 amp fuse for charging.   Should I put it on the positive battery lead?

I read that thin balance wires fuse out themselves if there is a short.   But it is better if they fuse out outside of the battery pack.   So I am thinking about using thinner balance wires for a connection between the battery pack and VGA port.  How about 24 awg silicone wires inside the battery pack and 26 - 28 awg silicone wires for connecting the battery to VGA port?  Does it make sense? 

In my first battery build (10S4P with 30Q cells) I used a lot of hot glue and also paper rings on the positive sides of 18650 cells.   Now I am reading that this may not be good because hot glue and paper rings can catch fire.   I also used hot glue to cover nickel strips, and to fix balance wires and battery leads, to make sure that they are not rubbing against anything.   I was using this battery for some time without issues (sometimes riding up pretty steep and long hills).  But now I am a bit worried that I used hot glue.   Should I be worried?    What are safer alternatives to hot glue and paper rings?

I am still debating about using a fuse for battery discharge.   There are pros and cons to it, from safety perspective.   If I use it, I'll go with a 60+ Amp fuse.   I guess without a fuse, there is a higher chance to burn VESC (which is fine with me).    But is it possible that VESC short out the battery and cause fire?   Did anybody have battery fire because of it?

I'll solder wires (instead of using connectors) everywhere where it is possible.   I'll solder can bus  wires directly to VESCs as well as the wires connecting VESC with remote receiver.   In my Vanguard I was using can bus and servo cables secured with tape.   But after riding some bumpy road these wires got loose and the board started to act very strange and dangerous (like suddenly accelerating instead of braking or vise versa).    After I soldered everything and secured it by hot glue, I never had this problem.    I think that servo cables and can bus connectors are not safe.   Why are people using them?

The only connectors that I'll use are XT60 for connecting the battery to VESCs and bullet connectors for phase wires connecting VESCs to motors.   Even with these connectors, one needs to add extra protection to make sure that they don't come loose.    On another occasion after I rode some bumpy road on my Vanguard, one of the motors started to rotate in the opposite direction.   This happened because one bullet connector on a phase wire got loose.   So I used pliers to bend the prongs of bullet connectors a little bit to make sure that they are really tight and can never get loose - this solved the problem.
```

---
## \#32 Posted by: Deckoz Posted at: 2018-01-20T13:07:49.094Z Reads: 143

```
[quote="psychotiller, post:19, topic:42596, full:true"]
They won’t fit superstar hubs. They are 6x2
[/quote]

Hey man are you positive about this? Superstars/hypas are 50mm... 2" tires have 50.8mm beads. A few mm  shouldn't make them not fit? The inner diameter of the bead looks the same... 

I think I need to order to know for science...
```

---
## \#33 Posted by: Darklinks Posted at: 2018-01-20T16:40:59.303Z Reads: 151

```
Dam wish I saw this post before ordering them I have a pair on the way today waiting on the post man to deliver them and I have superstar hubs. Well see what happens
```

---
## \#34 Posted by: sash Posted at: 2018-01-25T23:54:48.293Z Reads: 161

```
Today was the circumcision day.   

![IMG_20180125_183543502|374x500](upload://rKuhplPB4GWyJ6PQTIDPFklbbDS.jpg)

![IMG_20180125_183534484|374x500](upload://1Kk6UGeThn9ZzitaJ9tWkJ8Jd4r.jpg)

If you want to use @psychotiller's SixShooters with @torqueboards motors, be aware: The shafts of TB motors are too long for SixShooters.  You need to cut off 6mm from the shafts.   

Dremel is your friend:

https://www.youtube.com/watch?v=uSWoDYxt3t8
```

---
## \#35 Posted by: mmaner Posted at: 2018-01-26T00:06:49.071Z Reads: 151

```
Couldn't you move the mounts inside 6mm instead?
```

---
## \#36 Posted by: sash Posted at: 2018-01-26T00:21:28.121Z Reads: 149

```
[quote="mmaner, post:35, topic:42596, full:true"]
Couldn’t you move the mounts inside 6mm instead?
[/quote]

@mmaner   Is it how you did it in your build?   I could not figure out how to move Ripba mounts inside, because they sit in fixed position.  Another option I was thinking about was to add 6mm plate between motors and motor mounts, but I decided that cutting motor shafts was easier than making this plate.

I am curious how you move Ripba motor mounts inside.  Did you cut 6mm from the hanger?
```

---
## \#37 Posted by: psychotiller Posted at: 2018-01-26T00:23:07.566Z Reads: 156

```
It's not the SixShooters really...It's that the Ripba mounts are a fixed positition. With other motors, that's not an issue.
```

---
## \#38 Posted by: mmaner Posted at: 2018-01-26T00:30:22.152Z Reads: 158

```
I see what you are saying now.  Mine is using hanger clamps, not the cups.  Im using 177mm SUrf Rodz TKPs with 6374 TB Motors.  WIth my mounts as far out as they can possibly be, I still only have about 3mm between the motors.  Also, Im using 25mm pulleys and belts, so the shaft was actually a little short.

![image|690x356](upload://anEyM7VgD1jQeACH7AzKwRV0eAo.jpg)

I have a couple of builds that use the cups but they have BKB motors.
```

---
## \#39 Posted by: sash Posted at: 2018-01-26T00:33:52.655Z Reads: 157

```
Actually, one of the features of TB motors advertised on the website is "Extra long motor shafts".   I guess for pneumatic wheels this feature is rather a (minor) annoyance.
```

---
## \#40 Posted by: sash Posted at: 2018-01-26T00:39:22.596Z Reads: 156

```
I see.   I guess for 25mm belts "Extra long motor shafts" of TB motors is a helpful feature.   But for 15mm belts they are too long.
```

---
## \#41 Posted by: psychotiller Posted at: 2018-01-26T00:45:18.526Z Reads: 144

```
Build's looking good though! Get to riding!!
```

---
## \#42 Posted by: sash Posted at: 2018-01-26T00:54:13.461Z Reads: 139

```
I can't wait until I get to riding.    Waiting for @treenutter's deck.  Also 30Q 18650 cells are on the way.
```

---
## \#43 Posted by: psychotiller Posted at: 2018-01-26T00:55:44.047Z Reads: 137

```
Wait, I'm waiting on Treenutter decks too...Hmmm
```

---
## \#44 Posted by: sash Posted at: 2018-01-26T00:57:52.714Z Reads: 137

```
Loaded Icarus deck that I have on pictures is a mock up.  I really love this deck, but unfortunately it has wheelbite with SixShooters.
```

---
## \#45 Posted by: treenutter Posted at: 2018-01-26T03:39:27.061Z Reads: 139

```
@sash @psychotiller I never miss an order! Steez is imminent.
```

---
## \#46 Posted by: sash Posted at: 2018-03-02T03:48:10.742Z Reads: 122

```
Some pics:

![IMG_20180301_223314129|666x500](upload://emGgtIHk19EqI4AHUFZkQ4TBYy2.jpg)

Side by side with Loaded Vanguard


![IMG_20180301_223338409|374x500](upload://jMO7a6qi4mpayXNBf2tD9CF9IEK.jpg)

![IMG_20180301_223522692|666x500](upload://99gYvQ6JEKqUZwdjvD2cYDYfsvj.jpg)

Enough clearance for motors?
```

---
## \#47 Posted by: psychotiller Posted at: 2018-03-02T04:11:13.699Z Reads: 118

```
Looks good to me!
```

---
