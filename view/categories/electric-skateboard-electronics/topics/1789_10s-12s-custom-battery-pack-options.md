# 10s-12s Custom Battery Pack Options

### Replies: 99 Views: 19925

## \#1 Posted by: AbrownMN Posted at: 2016-03-13T01:25:16.477Z Reads: 968

```
Hey there guys, I am in the process of putting together a dual hub motor build. I am stuck on which battery setup to get, and not getting much feedback on my build thread. Right now it's between just getting a prebuilt 10s2p like Jason's SPACE Cell or Torqueboards pack. Or building my own Lipo/8650/26650 battery pack to fit the setup I am going for just right. I want it to be slim, I don't mind if it's long, but i'd like the batteries to be around 1.0-1.2 in (30mm) or less in thickness. The size of the SPACE cell looks about right, but If i can get away with a few  less goodies, make it thinner and save some money I will put in the effort. The main thing holding me back from just buying one of these packs is a concern voiced by Lever that I may experience some cutoff with these cells on his dual hub motors in high acceleration. He is also working on a new pack I guess, so maybe it's best to wait for that? Unless there is a custom, thin 12s pack that I am not finding? I will buy it immediately, so if you're selling let me know!
```

---
## \#2 Posted by: delta_19 Posted at: 2016-03-13T02:12:29.992Z Reads: 862

```
i would go the 18650 route do to it being the safest, lipos can explode and really cant take any damage. 18650's are in a metal can that can take some damage in both physical and electrical situations. also cells like samsung dont explode or shoot fire no matter what you do to them. 

right now im building my own 18650 battery using battery sleds used in vapes because they can take the high current.

this lets me recharge them on 18650 cell chargers like the nitecore d4 and i can remove any cell i want at anytime to check to make sure its still good.
little more labour intensive but gives you piece of mind.
```

---
## \#3 Posted by: AbrownMN Posted at: 2016-03-13T04:18:32.933Z Reads: 834

```
Right on, thanks for the info. I was watching some videos on those Samsung cell tests when I was trying to get my bearings on all the differences, and best suppliers. They look pretty redundantly safe.

So you're going to take out like 30 some cells individually every time you charge, or will you have some balance charger solution for when they're all installed in the pack as well?
```

---
## \#4 Posted by: delta_19 Posted at: 2016-03-13T04:24:11.113Z Reads: 798

```
im gonna get a 6 bay charger and just charge them 6 at a time, shouldnt take that long.
```

---
## \#5 Posted by: AbrownMN Posted at: 2016-03-13T04:27:08.585Z Reads: 776

```
I'd buy 5 of them :smile: Are you building a 10s or 12s pack? How are you planning on putting it together? I'd be interested in seeing some rough dimensions.
```

---
## \#6 Posted by: delta_19 Posted at: 2016-03-13T04:34:43.937Z Reads: 751

```
10s4p

its gonna be using these sleds 
http://www.brimstonevapeco.com/product-p/slim-dual-18650.htm

im gonna solder solid copper to each contact and put it all in to a box under my board. size wise it will be shorter then the space cell because no bms.
```

---
## \#7 Posted by: lowGuido Posted at: 2016-03-13T14:50:44.031Z Reads: 723

```
I am contemplating a similar Dilemma myself.
I have 12 10000mah cells sitting on my desk in front of me and I'm wondering if I should make a 10S or 12S battery?
```

---
## \#8 Posted by: AbrownMN Posted at: 2016-03-13T15:49:31.590Z Reads: 699

```
Make a 12s! We need more people figuring out the best possible configurations to keep them sized to the board. I would love to see a little writeup.
```

---
## \#9 Posted by: AbrownMN Posted at: 2016-03-13T15:50:04.510Z Reads: 689

```
Is BMS not necessary with that configuration?
```

---
## \#10 Posted by: Glenn Posted at: 2016-03-13T17:27:12.944Z Reads: 699

```
I've been building my packs(18650) with no bms,and they seem to be working just fine. I'm guessing they don't get the full charge but must be close to full. The last 8s3p set up cost me just over $60, and some time.<img src="/uploads/db1493/original/2X/a/a75f9161c9b30e860239d7235fe0f5ad5173c32b.jpeg" width="375" height="500"><img src="/uploads/db1493/original/2X/a/a0402dd8f5873a5d5ddef692c22891702e191cf5.jpeg" width="375" height="500"><img src="/uploads/db1493/original/2X/4/4fdb076a2414b797fcb5266d752e9c03dd662720.jpeg" width="375" height="500">
```

---
## \#11 Posted by: Glenn Posted at: 2016-03-13T17:37:29.338Z Reads: 658

```
My first build was 6s2p using 18650's that was six months ago is still working. It has about a 4 mile range with a top speed on 22mph. The packs were made with used batteries that I took out of my cordless drill that is about 3-4 yrs old. I believe all batteries were Samsung. I've been using a smart charger that I got on line that was specifically used for lithiun ion batteries.
```

---
## \#12 Posted by: delta_19 Posted at: 2016-03-13T17:53:46.538Z Reads: 654

```
a bms is never necessary but it is a nice safety feature. as long as you have balance leads and watch your voltage on the ride your safe.
```

---
## \#13 Posted by: Hummie Posted at: 2016-03-13T18:33:45.856Z Reads: 655

```
Where did you guys read that the Samsung are safer? I can't find any info saying that.  Some have a high discharge rate but can't find anything that says they are less likely to burn up than other li-ion when abused :over charged, over discharged, or banged.

Why seal the cells up so there's no way to check and balance them!?  Bulk charging without knowing what the cells voltages are is asking for trouble and really frowned on. Even if you had some gaps to get some prongs around each cell you could at least check them periodically and do some balancing with a modified phone charger or some resistors to discharge.  Otherwise if you're charging to full capacity at 4.2...danger.  Maybe at least only charge to 4.15 or 4.10. Some people would freak if they saw unmonitored cells like that.
I'm building a huge 48 cell 12s pack without a bms or balance leads but plan to still balance in the ways I mentioned above. Also relying on the esc low voltage cut-off. And with such a huge pack I'll likely only charge to 4.1 and it will last much longer
```

---
## \#14 Posted by: delta_19 Posted at: 2016-03-13T18:45:35.549Z Reads: 616

```
im going by samsungs in house test and just general reviews.

and no one runs it where they cant balance, any 18650 battery made here is made with a bms or balance leads.
```

---
## \#15 Posted by: Hummie Posted at: 2016-03-13T18:47:33.087Z Reads: 622

```
I can't find those Samsung safety claims. 

The guy above is going without anything to monitor
```

---
## \#16 Posted by: delta_19 Posted at: 2016-03-13T18:49:43.661Z Reads: 616

```
https://www.powerstream.com/p/INR18650-25R-datasheet.pdf

its on the datasheet for the cells
```

---
## \#17 Posted by: Hummie Posted at: 2016-03-13T19:19:51.650Z Reads: 632

```
Here's a sheet for the Lg hg2 cells. The tests are on the last page. They're similar and showing doing just as well.  I've never heard of a li-ion cell for sale that was considered safer.  

http://www.lenovo.com/social_responsibility/us/en/LGC-CY151.pdf

But after looking at both these...they're safer than I though.
```

---
## \#18 Posted by: lowGuido Posted at: 2016-03-13T20:02:11.244Z Reads: 634

```
I think that regardless of the brand, all lithium batteries should be considered dangerous and treated with respect.
```

---
## \#19 Posted by: chaka Posted at: 2016-03-15T14:25:44.582Z Reads: 649

```
If you are using the VESC, divide 8600 by your motor KV and that will give you the max voltage you should use. Of course this isn't some golden rule just a general guide.

@AbrownMN If you are going to power hubs you will want some amperage for initial take off and acceleration unless you will be installing a VESC. The VESC can make a weak pack work by limiting the current draw but, in my opinion, it is a big compromise. Go as big as you can with your battery pack and you will not need to put the VESC into "nanny mode". 
<img src="/uploads/db1493/original/2X/a/a1d1c049fb451517f10d4d64082c588b9cf7addc.jpg" width="506" height="500">
10s7p
```

---
## \#20 Posted by: torqueboards Posted at: 2016-03-15T14:40:08.398Z Reads: 610

```
Board looks nice Chaka.. I want one :)
```

---
## \#21 Posted by: AbrownMN Posted at: 2016-03-15T15:53:09.168Z Reads: 603

```
Damn @chaka..that board is awesome....I went with a 12s3p pack from torqueboards (30a-60a I think?). So I should be able to power the dual's with that no problem, right? I also am going dual VESC so as you mentioned that should help. Any other advice you can give is greatly appreciated. I haven't been able to find the exact KV of the Carvon's..I should probably call on @leVer...
```

---
## \#22 Posted by: mccloed Posted at: 2016-03-15T17:26:56.834Z Reads: 588

```
The Carvon Hub Motors are 149kv.
```

---
## \#23 Posted by: torqueboards Posted at: 2016-03-15T17:37:46.987Z Reads: 582

```
@AbrownMN - 30a cont/80a peak
```

---
## \#24 Posted by: AbrownMN Posted at: 2016-03-15T21:05:17.001Z Reads: 575

```
Thanks Guys! @torqueboards @mccloed
```

---
## \#25 Posted by: Hummie Posted at: 2016-03-16T18:48:32.470Z Reads: 578

```
8600 divide by the motor kv giving the voltage you can use with the vesc!?!  that seems really high.  I did read vedder's thing about an optimum e-rpm but I didn't understand it to mean the voltage usable.  With 100kv motors that would allow me to use 86 volts!.  that sounds way off.  I heard from him that 12s would be fine so 44 volts or maybe call it 50.

86 volts?  maybe I'm misunderstanding you.

what's the highest voltage youve ran the vesc?


Are these the biggest capacitance with low esr:
http://www.digikey.com/product-search/en/capacitors/aluminum-capacitors/131081?k=Rubycon+ZLH&pv13=126&pv63=491&FV=fff40002%2Cfff80009&mnonly=0&newproducts=0&ColumnSort=63&page=1&quantity=0&ptm=0&fid=0&pageSize=25
```

---
## \#26 Posted by: Hummie Posted at: 2016-03-16T18:49:22.750Z Reads: 543

```
what cells are they?
```

---
## \#27 Posted by: AbrownMN Posted at: 2016-03-16T19:01:10.428Z Reads: 541

```
What woodworking tool did you use to cut that slight channel around the outside edge? A router? What sort of bit did you have in there?
```

---
## \#28 Posted by: torqueboards Posted at: 2016-03-16T19:01:12.905Z Reads: 527

```
@Hummie The cells are LG HE4.
```

---
## \#29 Posted by: Hummie Posted at: 2016-03-17T05:07:28.444Z Reads: 528

```
Looks more like 60amp continuous and 105 burst  with 3p for your pack torque
```

---
## \#30 Posted by: kaywerks Posted at: 2016-03-17T05:08:57.922Z Reads: 532

```
Why LG HE4 vs Panasonic NCR18650B ?
I know the HE4 have 10A cont. Discharge but Panasonic have much higher 3400 mah and 8a cont. 
You wouldn't be pulling 30a cont and 80a burst?
```

---
## \#31 Posted by: Hummie Posted at: 2016-03-17T05:13:51.580Z Reads: 515

```
He4 have 20 amp continuous

The Panasonic are 6.8amp continuous.
```

---
## \#32 Posted by: torqueboards Posted at: 2016-03-17T05:15:43.466Z Reads: 510

```
@Hummie - Yeah, so far I haven't needed any higher than that. Bigger BMS/more costly and don't seem a need.
```

---
## \#33 Posted by: Hummie Posted at: 2016-03-17T05:18:24.235Z Reads: 504

```
Oo so the bms is the limit
```

---
## \#34 Posted by: NNGG Posted at: 2016-03-17T05:18:27.836Z Reads: 491

```
Still dont understand why not just bypass all of this and get some cheap Lipos....
```

---
## \#35 Posted by: Hummie Posted at: 2016-03-17T05:20:04.718Z Reads: 500

```
Last many more cycles. Less likely to burn up and don't have to think about it. Less physically vulnerable.   More energy density.
```

---
## \#36 Posted by: NNGG Posted at: 2016-03-17T05:21:01.873Z Reads: 493

```
Do the extra cycles offset the extra cost?
```

---
## \#37 Posted by: lowGuido Posted at: 2016-03-17T05:21:10.018Z Reads: 499

```
I have just bought a pack of cheap multistar lipos and ripped them all apart. I'm going to solder them all together again soon.

where does every one get that big heat shrink from??
```

---
## \#38 Posted by: NNGG Posted at: 2016-03-17T05:21:51.923Z Reads: 493

```
ebay/ hobbyking, They are just different millimeters
```

---
## \#39 Posted by: Hummie Posted at: 2016-03-17T05:22:09.030Z Reads: 503

```
I think so.  The cycles are many more.  Piece of mind.  

I just got the multistar as well actually.  Great deal. Slim.  Going even slimmer!! The 3s is the slimmest I've found
```

---
## \#40 Posted by: NNGG Posted at: 2016-03-17T05:23:26.799Z Reads: 505

```
How many more....like 3X, 5X, 10X?
```

---
## \#41 Posted by: torqueboards Posted at: 2016-03-17T05:28:33.674Z Reads: 479

```
Don't get me wrong.. Can't go wrong with LiPo's especially with HobbyKing's most recent sales. Cheap and great source of power, not too costly to replace. But some people want a more convenience factor.

IMO If you don't mind the LiPo's and charging in parallel. Go LiPo's all the way. Don't bother with a custom pack. But some people just don't like having to deal with the LiPo's. Zippy Flightmax 6S1P 25C for $31.12 that's a steal.. x3 sets (6) batteries = $186.72. It's a great deal. @LowGuido - I wouldn't get the Multistar packs 6s5.2ah $27.99 as they don't pack as much of a punch vs the Flightmax. If the Flightmax is on sale it's worth the 3 bucks difference.

Multistar sucks :( my 12S feels weak sauce...
```

---
## \#42 Posted by: NNGG Posted at: 2016-03-17T05:30:28.802Z Reads: 459

```
Thats why you read the Hobbyking racing quad battery reviews. :D soo happy I didnt bite on multistar deals when I have the zippy option
```

---
## \#43 Posted by: lowGuido Posted at: 2016-03-17T05:30:40.439Z Reads: 460

```
too late already bought and chopped. oh well.. for science.

for what its worth I got them mad cheap.
```

---
## \#44 Posted by: Hummie Posted at: 2016-03-17T05:31:07.190Z Reads: 449

```
Wow how the world turns...on es I was talking crap on the multistar low c rating while you talked them up and here we are now reversed.

Actually tried to cancel the order but seems they never charged me.  Can't cancel free!
```

---
## \#45 Posted by: NNGG Posted at: 2016-03-17T05:32:49.126Z Reads: 437

```
lol I still agree that li-ions are the future, but I will buy the lipos now and use them for a good 3 years before switching
```

---
## \#46 Posted by: Hummie Posted at: 2016-03-17T05:33:40.958Z Reads: 431

```
I'm into the li-ion as I'm lately obsessed on making a compression pack using clear rubber

It's a hobby.
```

---
## \#47 Posted by: lowGuido Posted at: 2016-03-17T05:34:23.984Z Reads: 422

```
where do you get that stuff?
the compression wrap
```

---
## \#48 Posted by: Hummie Posted at: 2016-03-17T05:37:43.866Z Reads: 426

```
I've got tons of liquid polyurethane.  Clear 70 duro. Tomorrow I make the pattern for the mold!!

Copper is in the mail on route and the 48 cells sit here waiting. I can talk up a storm..first


U just want shrink wrap though right?
```

---
## \#49 Posted by: lowGuido Posted at: 2016-03-17T05:52:25.692Z Reads: 409

```
yeah just the shrink wrap that batteries are usualy wrapped in.
```

---
## \#50 Posted by: Hummie Posted at: 2016-03-17T05:59:24.036Z Reads: 412

```
Hobbyking has like 100 sizes.  Some are hard and light and others rubbery and heavier
```

---
## \#51 Posted by: torqueboards Posted at: 2016-03-17T06:20:49.592Z Reads: 417

```
[quote="Hummie, post:44, topic:1789, full:true"]
Wow how the world turns...on es I was talking crap on the multistar low c rating while you talked them up and here we are now reversed.

Actually tried to cancel the order but seems they never charged me.  Can't cancel free!
[/quote]

@Hummie LOL tell me about it right...I think it was ok at first a bit.. but jus not enough..
```

---
## \#52 Posted by: lowGuido Posted at: 2016-03-17T06:28:20.680Z Reads: 391

```
[quote="Hummie, post:39, topic:1789"]
Great deal. Slim.  Going even slimmer!! The 3s is the slimmest I've found
[/quote]
how slim are we talking?
```

---
## \#53 Posted by: chaka Posted at: 2016-03-17T06:28:45.754Z Reads: 407

```
@kaywerks The he4 have 20 amp discharge but they also have a very low resistance as a result. To me it seems the lower the resistance the greater the punch. Could be a placebo effect? So many factors at play on these builds it can be hard to tell sometimes. I can say honestly that the panasonics or any other low discharge will do fine in an 80 cell pack, anything smaller and you want to jump up to a 10 or 20 amp discharge cell. This is assuming you are going to ride like a savage and full throttle hills. Ride like a civilized citizen and you can drop it much much lower.

@AbrownMN I used a rabbiting router bit from diablo. Nice bit but it is still a difficult cut. You have to follow up with a rabbit plane and chisel on some of the transitions.

@Hummie The 8600rpm rule was something Vedder had mentioned regarding anything beyond this resulting in a reduction in efficiency. I have not used more than 12s on the vesc yet.
```

---
## \#54 Posted by: Hummie Posted at: 2016-03-17T06:33:10.542Z Reads: 392

```
But Vedder didn't mean u can use more than 12s I'm pretty sure

The multistar 3s are 2cm thick.  The hobbyking battery finder tool seems legit with the dimension variables 

Who can answer my parallel vs series battery question? Chaka u ever do inductance measurements with that many cells?
```

---
## \#55 Posted by: chaka Posted at: 2016-03-17T06:45:41.987Z Reads: 382

```
I do measure individual cells but not the whole pack. It might be a good baseline to gauge loss in capacity over time?
```

---
## \#56 Posted by: Hummie Posted at: 2016-03-17T06:47:41.591Z Reads: 404

```
The inductance of the pack I doubt would change.  I'm wondering how 18650 cell packs do...have to add more capacitors I'm pretty sure
```

---
## \#57 Posted by: chaka Posted at: 2016-03-17T07:08:38.123Z Reads: 425

```
I was thinking resistance, sorry.  They do fine with 3x680uf caps
```

---
## \#58 Posted by: whitepony Posted at: 2016-03-17T08:48:17.661Z Reads: 455

```
for hub motors you'd probably want a battery that can deliver higher currents compared a battery for a belt drive setup. if you want to go down the DIY 18650 route, Id go for high power medium capacity cells like the LG HG2 - I made a 10S4P pack from those cells myself and its holding up very well. sadly the cells are quite expensive compared to others (for a reason I guess).

In the end id always use as many cells as possible to share the load. for my mountain touring board Im currently building a 750Wh 10S6P battery with high capacity medium discharge rating cells sold on the endless sphere forum (sanyo ncr18650GA) -> https://endless-sphere.com/forums/viewtopic.php?f=31&t=61608 

the 10S3P from enertion is a pretty cool product with fairly high discharge ratings, but imo its a little small - at least for my touring desires. a colleague of mine has that one and when his BMS is cutting off his power, im still at healthy 36V and ready to go for another 10km. due to the fairly large (and convenient) electronic package of the space cell, it has the exact same dimension as a 10S4P 18650 DIY battery without any electronics. dont think you can go much smaller/slimmer in the electronic department than my tesseract build:

<img src='/uploads/db1493/original/2X/7/7486ddf89b32cb8b08c8557312d9620d619d5388.jpg'>
```

---
## \#59 Posted by: lox897 Posted at: 2016-03-17T10:11:45.625Z Reads: 439

```
Finally @whitepony is on esk8. I was wondering when you would join here. You are awesome at making packs.

EDIT: Why are you using those Sanyos? On the info page that the guy linked it says they have 10 amp continuous discharge? I thought you were going with the Sony VTC5?
```

---
## \#60 Posted by: whitepony Posted at: 2016-03-17T10:24:46.606Z Reads: 434

```
always depends on the currents you are aiming for. with a massive 10S6P battery, I got 60A continuous current from 6x10A cells (and even larger motor phase currents) - thats more than enough to have a lot of fun! ;)

at the same time, the 18650GA have a 10% larger capacity for half the price! ;)
```

---
## \#61 Posted by: Tarzan Posted at: 2016-03-17T11:00:42.776Z Reads: 404

```
Yes nice to see you here. Have read a lot of your post on ES and will build a cap spot welder like yours when it comes to the battery point of my build.
```

---
## \#62 Posted by: lowGuido Posted at: 2016-03-19T00:02:27.616Z Reads: 391

```
I'm just soldering the balance leads onto my custom 12S lipo now.
actually technically I'm making two 6S packs in series so that I can charge them easier.
```

---
## \#63 Posted by: kaywerks Posted at: 2016-03-19T12:21:54.559Z Reads: 395

```
Where are y'all buying these LG's at ? I'd love some for testing.
@chaka
@torqueboards
```

---
## \#64 Posted by: chaka Posted at: 2016-03-19T14:10:35.644Z Reads: 400

```
There are lots of distributors in HK if you are looking for quantity otherwise check ebay or maybe a distributor on endless sphere.
```

---
## \#65 Posted by: delta_19 Posted at: 2016-03-19T19:53:28.975Z Reads: 408

```
So I made a thing.....
https://youtu.be/OKv0Kb0v8o4
```

---
## \#66 Posted by: Hummie Posted at: 2016-03-19T20:01:05.210Z Reads: 399

```
Nice. So ur not a hot girl.  There are none here 

Are they connected soley pressed in to sleds or are they solder/welded?
```

---
## \#67 Posted by: NNGG Posted at: 2016-03-19T21:21:28.447Z Reads: 389

```
How much did the 40 18650's cost?
```

---
## \#68 Posted by: lowGuido Posted at: 2016-03-19T21:25:45.494Z Reads: 381

```
[quote="Hummie, post:66, topic:1789"]
So ur not a hot girl.
[/quote]

LOL, there are no girls on this forum.

maybe people put girls as their avatar so people talk to them :P
```

---
## \#69 Posted by: delta_19 Posted at: 2016-03-19T21:52:26.275Z Reads: 379

```
just pushed in to the sleds.

and the 48 18650s that i ordered cost 233 usd and sleds another 100 but, now when the batteries are at their cycle limit i just spend 233 more instead of 350.
```

---
## \#70 Posted by: Hummie Posted at: 2016-03-19T23:14:50.769Z Reads: 386

```
Speaking of sexual allure what do you think I should name my website?  I've got skatehubmotors.com and pervomotors.com

Skatehubmotors is straight forward
Pervomotors...would be a site you'd have to say you were over 18 and then it would be filled with antique porn from 1900s which are legal to reprint.  
And then I also like boostedkilla.com. 

I just spent 120 on a 3D printed sled for 24 cells that's being made now.  I'll make a mold with it and end up potting 48 cells in 70 during clear rubber.  No bms and just access to each cell through small holes for monitoring.  Using cocnut oil to fill the pressure release valve on cells and melt it out.  

Stunned how light the (48) 18650s are.  Energy density equals light weight I guess. 

I'm having a great time.  Thank you everyone.
```

---
## \#71 Posted by: NNGG Posted at: 2016-03-20T00:53:06.926Z Reads: 370

```
We like.... NEED a weird esk8 porno site to get more traffic
```

---
## \#72 Posted by: lowGuido Posted at: 2016-03-20T02:38:25.829Z Reads: 382

```
Pics of my custom lipo pack in my build thread.
http://www.electric-skateboard.builders/t/skate-a-tron-4000-superleggera-carbon-deck-12s-dual-hub-motor-vesc/1531/15
```

---
## \#73 Posted by: delta_19 Posted at: 2016-03-20T02:56:23.184Z Reads: 377

```
battery hour on the forums today
```

---
## \#74 Posted by: mostwanted Posted at: 2016-03-20T08:25:12.189Z Reads: 387

```
@chaka !   10s7p   ~     70cells ? ? ? ?
are you COMPLETELY INSANE  ? ? ? ?
you want to beat NGV's  record ? ? ? ?
wanna beat their 100km  record ? ? ? ?

in the discussion of power packs ,
i got this from aliexpress . no i didnt buy it . now i got my own local supplier for 18650 packs 36V  40cells .
anyway this supplier is making $$$ in aliexpress by the looks of it . he also offers a complete sensored dual hub with dual escs and remote minus the 22.2V cell .

honest to God ~ i'm lured by that sensored dual hubs .

<img src="/uploads/db1493/original/2X/e/efcd1c078bf9eca63be9e92f5b88931d817dee4d.jpg" width="640" height="361">
<img src="/uploads/db1493/original/2X/3/31c3f2c86af224de8b5ee9385dc16a8709adde4b.png" width="281" height="500">
```

---
## \#75 Posted by: chaka Posted at: 2016-03-20T15:53:36.071Z Reads: 362

```
I am not really into setting records @mostwanted. It is the range I am after, anything less is just disappointing after riding with this many cells. The bms is limited to 90 amps, about 3300 watts. I usually only need to charge a system like this once every three days. And when you do need to charge, it is a simple plug and play operation

The board in that photo is for a customer who has been patiently waiting for a long time while I work all the bugs out of my initial design. 

I honestly think 70 cells is the minimum for a serious rider. I am building a smaller board for my daughter and it will have about 40 cells. I think it will be fine for her due the the low rider weight but I think it will deplete much too quickly for my tastes.
```

---
## \#76 Posted by: AbrownMN Posted at: 2016-03-20T20:06:32.964Z Reads: 354

```
Hmm, how about Eskee8ers.com?
```

---
## \#77 Posted by: delta_19 Posted at: 2016-03-20T20:39:11.605Z Reads: 342

```
going by TB's calculation im getting 63KM range..... sweet baby Jesus.
```

---
## \#78 Posted by: torqueboards Posted at: 2016-03-20T21:46:11.282Z Reads: 339

```
@delta_19 The calculation doesn't calculate losses due to external factors. For the most part it's accurate but not always accurate. More of just a base line.
```

---
## \#79 Posted by: delta_19 Posted at: 2016-03-21T00:28:10.860Z Reads: 347

```
still give or take 7KM he could still get from my base to the nearest city and back.
```

---
## \#80 Posted by: mostwanted Posted at: 2016-03-21T11:50:26.269Z Reads: 371

```
i'm 47yrs old this year , dont think i can stand & balance myself for a long distance of 10km . 

usually people will crowd inside a feeder bus , me ? i ride my sweet ride to the nearest train station without having to cramp inside the sardin packed bus . once the train reach my work place , again i ride my sweet ride to work without having to put up with smelly armpits in a crowded  feeder bus .

70 cells is equivalent to 2 times s.p.a.c.e  cell (30cells) with bonus 10 cells . your customer  must've have strong muscular legs to withstand 30 km or more  commute .

what do you think of this ?  it is an 18650  li ion , 40 cells , made in china . no particular brand . but it is sold in local store for just SGD $280 .  i was thinking of stripping it and re assembling it flat out .  batt pack comes standard with brick charger and built~in BMS .
this batt pack is meant for ebikes . the ones famously known as SUV Ebikes .
this local company also offers the same price if i wanted it to be custom made flat . all 40 cells . just that it is not a popular brand we all knew .


<img src="/uploads/db1493/original/2X/9/93b9b189a51df2ad0dafd8bddbb2ccd97b0da7c8.png" width="666" height="500">
```

---
## \#81 Posted by: chaka Posted at: 2016-03-21T13:55:43.816Z Reads: 355

```
I don't touch those no name brands. They are usually unprotected cells and can be very dangerous if they are discharged heavily. If you are not deterred by my recommendation at least make sure they used vented cells. The unvented cells can become projectiles if they build up pressure.
```

---
## \#82 Posted by: BigAl Posted at: 2016-03-21T14:17:52.644Z Reads: 366

```
Since we're all showing our privates :blush: here's what I put together this weekend.


[URL=http://s276.photobucket.com/user/BigAlinmiami/media/1E76AAA4-B8FD-44FE-B3B2-BB00FFE9A277_zpsn0t7mi3f.jpg.html][img]/uploads/db1493/original/2X/2/2feeda31721d3e23ad9aa2da9977be7013bb6c07.jpg[/img][/URL]


[URL=http://s276.photobucket.com/user/BigAlinmiami/media/A35F72EA-5FF1-486D-A0A0-3CB4EB93EC0E_zpsaewjt3eu.jpg.html][img]/uploads/db1493/original/2X/6/678878e68d6e9f8df113af6802af2df0d97179db.jpg[/img][/URL]

Obviously the only things missing are the switch and VESCs.
I know some of you guys like a whole lot more cells but this is for my son who ways 85lbs.  I figure with the lower combined weight, this should last roughly what my board last with the 10s3p.

Al...
```

---
## \#83 Posted by: psychotiller Posted at: 2016-03-21T16:12:24.819Z Reads: 354

```
Looks good! Let us know how those Hub motors spin up at 4s.
```

---
## \#84 Posted by: BigAl Posted at: 2016-03-21T16:27:11.551Z Reads: 352

```
Actually, it's tough to tell from those pics but it's going to be 10s2p.

Al...
```

---
## \#85 Posted by: longhairedboy Posted at: 2016-03-21T16:43:07.588Z Reads: 370

```
i took this 16Ah 6S2P multistar pack and flattened it out, keeping it 6S because my objective was to rebuild my old 6S system into a rat board on a Black Metal edition Scarlet deck i've been using as a push board for a while. 

<img src="/uploads/db1493/original/2X/7/74cead48d8231663e246f64d5da88a2d286fbd97.jpeg" width="666" height="500">

<img src="/uploads/db1493/original/2X/4/477ed901dfb9710e51790e89e3410939922068e1.jpeg" width="666" height="500">

<img src="/uploads/db1493/original/2X/a/ae3d624ae5c5d4465bc56b74e3b1a4ff383001cf.jpeg" width="666" height="500">

I could easily rewire it for 12S with proper balance leads and buy a BMS for it and go that route after installing a pair of VESCs, but I have no idea what a set of NTM propdrive 5060 270Kvs would do on 12S, i'd likely want larger, lower kv motors. All of that is beside the point though. 

The point is you can have a simple plug-in-the-wall 8Ah 12S pack (roughly 350 watt hours) for under $100 if you're willing to repack off the shelf lipos and add a BMS for another $60 or so.  So around $160ish  total.
```

---
## \#86 Posted by: lowGuido Posted at: 2016-03-21T17:16:43.554Z Reads: 363

```
I really like the flat pouch lipo's
I know everyone is leaning towards the tube cells but you can never get as flat as a pouch pack.
and they are dirt cheap and don't need a special spot welder, just a good iron.

http://www.electric-skateboard.builders/uploads/db1493/original/2X/f/f0e11f4419ee8fcee0c4a1d555e1979ae3b477bb.jpg
```

---
## \#87 Posted by: longhairedboy Posted at: 2016-03-21T17:44:56.017Z Reads: 364

```
yeah with some good silver bearing solder and not that bullshit lead free shit and a nice 80 watt or higher soldering iron you can repack all day with those easy to solder tabs. Silver bearing solder has a lower flow temp so its less heat on the tab for less amount of time, and on a nice soldering iron its just really quick, so there's less of a threat to the cells from the heat. 

when i get into the 5Ah 26650s i've been eyeballing i'm going to order them with tabs to make soldering them easier. I plan on making a ridiculous 12S pack one of these days out of those. 

One day when i make custom packs to sell with BMSs and chargers i'll think about spot welding, but not now. IT would be a fun project building one out of microwave parts though.
```

---
## \#88 Posted by: torqueboards Posted at: 2016-03-21T17:59:26.956Z Reads: 351

```
Multistar doesn't pack enough punch though :( Feel like I borrowed grandma's batteries.
```

---
## \#89 Posted by: lowGuido Posted at: 2016-03-21T18:01:32.299Z Reads: 348

```
Yeah i'll see how they go.
they can't be THAT bad can they?
```

---
## \#90 Posted by: torqueboards Posted at: 2016-03-21T18:06:39.582Z Reads: 352

```
[quote="lowGuido, post:89, topic:1789"]
they can't be THAT bad can they?
[/quote]

ohhh... they are bad... unless you can turn them off (on/off switch or disconnect).. say buh bye to your packs :frowning:

I learned the hard way. Never again...

Get one cell .5-.8v away from the others... It's literally a gone'er.. Unless you want to try re-charging that one cell like everytime..
```

---
## \#91 Posted by: lowGuido Posted at: 2016-03-21T18:09:42.604Z Reads: 336

```
well like I said. I have them now so I'm gonna use them.
time will tell.
```

---
## \#92 Posted by: torqueboards Posted at: 2016-03-21T18:10:39.844Z Reads: 335

```
Let us know your results..
```

---
## \#93 Posted by: psychotiller Posted at: 2016-03-21T19:09:20.710Z Reads: 324

```
I have a couple of those packs and ran 8s with a single 245 bigfoot. No issues on the runs I took.
```

---
## \#94 Posted by: longhairedboy Posted at: 2016-03-22T16:22:07.175Z Reads: 327

```
@torqueboards sounds like 10C isn't enough for you, although i have to admit that i'm also not feeling the umph i used to on my original 10ah custom pack that this replaced. unfortunately there's a ton of other variables in my case, i basically rebuilt the entire board on a different deck with new boxes and everything, and the pack is heavier, and i can't tell if i think its slower because it is slower or because i had previously been tearing around on a 10S li-ion system with dual 6355s on VESCs which would skew anyone's perception of what "fast" is.
```

---
## \#95 Posted by: torqueboards Posted at: 2016-03-22T16:38:26.449Z Reads: 330

```
@longhairedboy Yeah, I was testing Turnigy pack (2) 6S vs Multistar (2) 6S.

I couldn't punch it harder enough and seemed like it lacked power. It was at full charge too. I didn't think much of it until I ended up realizing it was a Multistar pack. oh welps.. last time I buy the multistar packs for myself.
```

---
## \#96 Posted by: longhairedboy Posted at: 2016-03-22T16:55:13.621Z Reads: 347

```
yeah.. the more i think about it.. the more i realize i was entirely too comfortable on that throttle... in the past a comfortable glide was about half throttle and full throttle was kind of scary. But i spent about 18-20 miles at three quarter throttle and never once felt the fear. 

Clearly i'm going to need to gather more evidence this weekend. This time with an app that will tell me how far and fast i was actually going.
```

---
## \#97 Posted by: laurnts Posted at: 2016-04-06T00:57:03.760Z Reads: 354

```
I have to say the C rating from the multistarpack is too low, they lack the punch. I have 4 packs of 3S 5000mah 25C Zippy lipo, when I have them in 6S 10AH I have more punch compared to 6S 5AH. What I mean is that I could feel difference when I have my packs at 50c (having them in parallels). Therefore I could safely say that making battery in parallels increase C rating as parallels setup split the current draw between batteries, maximizing C rating output. Also having them not discharging close to the maximum C rating increases life cycle.

So with the case of Lipo ie: having 6S 10AH could be better than 12S 5AH.
Because it splits the current draw each, cooler, more punch and improve life cycle.

Since I have experienced the power of higher C in batteries, I try to avoid having only 25c / 30c rating packs combo.
```

---
## \#98 Posted by: Papo Posted at: 2017-06-08T22:52:50.766Z Reads: 191

```
you can use water bottle coke bottles when it shrinks it is like a plastic case
https://www.youtube.com/watch?v=ITGw4qqiMwY&t=5s

https://www.youtube.com/watch?v=Ltcw69bD_Wk
```

---
## \#99 Posted by: nenecossais Posted at: 2018-01-11T12:43:59.067Z Reads: 104

```
What do you think about Aliexpress Power pack, https://fr.aliexpress.com/item/Hot-sale-36V-Lithium-battery-36V-20AH-Electric-Bike-battery-36-V-25ah-1000W-Scooter-Battery/32825976769.html?spm=a2g0w.10010108.1000013.16.7cd09253cb3hB9&traffic_analysisId=recommend_2088_8_90158_iswistore&scm=1007.13339.90158.0&pvid=3f3612a7-b650-4933-a5b4-36fae58a3a7d&tpp=1
```

---
