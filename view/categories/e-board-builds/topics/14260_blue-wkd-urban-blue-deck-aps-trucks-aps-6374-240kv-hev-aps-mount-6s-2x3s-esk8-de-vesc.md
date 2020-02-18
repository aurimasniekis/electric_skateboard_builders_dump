# Blue WKD &#124; Urban Blue Deck &#124; APS Trucks &#124; APS 6374 240kV HEV &#124; APS Mount &#124; 6s (2x3s) &#124; esk8.de VESC

### Replies: 18 Views: 2933

## \#1 Posted by: Neilfenstein Posted at: 2016-12-06T11:50:49.040Z Reads: 241

```
This is my first build so I will most likely need some revision before I pull the trigger on the parts purchase.

Here is the donor phase 1 board <img src="/uploads/db1493/original/3X/f/a/fa08fc15a5f0e7cbb620726b0a832e701b2d4e4f.JPG" width="375" height="500">

So here's some questions to get going, I have everything in carts on the online shops waiting to click buy, but I thought it's worth asking you experts first. 

As I state in the title I am planning to use Alien Power System parts as I can get them easily in the UK. But I am happy to be convinced otherwise!! How do these motors and mounts compare to turnigy or esk8.de motors parts interns of performance and reliability?

1) I am quite confused about the ERPM and kV / Battery Cell combos and the benefits trade offs of each however I think the price difference for the Cells from Hobby king between 2X 3s or 5s means that I can decide after I select a motor. I appreciate you should calculate ERPM and keep below a level for the VESC but is there any actual difference between a 190kV+10s or a (as per tutorial) 245kV+6s? Is it just preference? The only issue I can see is charging. I could more easily/cheaply charge a 6s config. 
1a) I would love to add BMS down the line, does this make a difference?

2) Would the esk8.de VESC or vedder VESC be better?

3) Is there any issues with the APS trucks or should I stump up the extra for Caliber 2s?

4) Is there any issues with the APS ABEC clones? I'm struggling to find EU real versions.
```

---
## \#2 Posted by: Tuomalar Posted at: 2016-12-06T12:09:12.493Z Reads: 214

```
http://www.electric-skateboard.builders/t/start-here-faq-for-diy-electric-skateboard-builders/215/14
```

---
## \#3 Posted by: NickTheDude Posted at: 2016-12-07T01:30:49.951Z Reads: 186

```
The VESC ERPM limit is 60,000. The advantage of low kV high voltage is that in order to make the same power you need less amps. Power = V * A. Amps are bad because they create heat which can potentially fry the VESC. Heat is also lost energy and therefore less efficient.

Generally it's important to allow some headroom and 190kV + 10S gives you a max ERPM of around 50k which is why it's a pretty common setup with the VESC.
```

---
## \#4 Posted by: zmoney Posted at: 2016-12-07T02:25:46.130Z Reads: 173

```
[quote="Neilfenstein, post:1, topic:14260"]
2) Would the esk8.de VESC or vedder VESC be better?
[/quote]
They are the same ESC. There are multiple vendors (including myself) that offer the VESC.
```

---
## \#5 Posted by: saul Posted at: 2016-12-07T02:34:40.127Z Reads: 166

```
[quote="zmoney, post:4, topic:14260"]
vedder VESC
[/quote]

VESC = Vedder's Electronic Speed Controller.

lol :sweat_smile:
```

---
## \#6 Posted by: zmoney Posted at: 2016-12-07T02:35:26.921Z Reads: 156

```
You quoted my quote  :joy:
```

---
## \#7 Posted by: saul Posted at: 2016-12-07T02:36:47.777Z Reads: 156

```
too lazy to scroll up and it the extra rundunancy proves the point :sunglasses:
```

---
## \#8 Posted by: Neilfenstein Posted at: 2016-12-07T19:46:45.717Z Reads: 159

```
Thanks for the replies guys.

I messed up the question, I was looking at Phoenix VESC and esk8.de but chose the esk8 one after all, order has been made :slight_smile: I like that the esk8.de VESC was complete and came with XT60 connector etc.

I went predominantly APS equipment, I don't think I was quite as clear as I could have been in my original question, I was asking if the parts are comparable to other more common parts that are harder to get/cost more in UK such as Caliber trucks and Turnigy Motors etc.

**Final parts list - Phase 1**
* APS trucks - Black
* APS ABEC Clone Wheels
* APS Mount
* APS Pulleys & belt 15mm - Motor 15T - Hub 32T & 36T (everything I read said 36T so I bought it extra) + spare belt
* APS 6374 245kv Motor
* APS Controller
* esk8.de VESC
* 2 x 3s 5500maH from Fluoreon to be wired in series for 6s
* IMAX B6AC Charger
* Various cabling etc including XT90 anti-spark for loop key.

So the reason I went Floureon was cost, I got both batteries for the price of a single Turnigy/Zippy equivelent posted for free rather than hobby king, which I couldn't figure out if there would be import cost on top. They get reasonable reviews online plus this is my first build, so try it out and see. Plus they come with XT60 connectors like the VESC so less effort.

Current thoughts on phase 1 enclosure is something like this:-
<img src="/uploads/db1493/original/3X/7/0/7032287c23102f50c699eb2a9b928880182c6d5a.png" width="487" height="362">


**Phase 2 plans (possibly 1.5 if I muck something up :slight_smile:** 
Improve distance/milage (possibly with new batteries, hence cheaper ones initially)
Add BMS and charging port electrics for easier charging
Power Switch to replace loop key
Fancy/bespoke enclosure.

Phase 2 may rely on my brothers interest so I can pass on/trade up to make the changes.

Any comments welcome. Some of my orders have dispatched so I'll take pics as stuff arrives and the build progresses :wink:
```

---
## \#9 Posted by: DreadBiscuit Posted at: 2016-12-12T15:16:31.963Z Reads: 140

```
I like your build.  I am building an eboard soon (I have all of the parts, just waiting on free time) with some AlienPowerSystem components as well (just motor and remote) - Take a look [here](http://www.electric-skateboard.builders/t/arbor-axis-maple-aps-6374-240kv-tb-vesc-8s-6ah-lipo-tb-single-mount-kit-caliber-ii-50s-abec-83mm-aps-remote/14217).  

I have noticed very few people using the APS remote (few = one so far...you make two).  Why did you choose it?  And have you gotten a chance to use it?  

I will keep you posted as to my experience with it, but if you get to it first, I'd like your feedback as well.  Good luck with your build! 

Cheers!
```

---
## \#10 Posted by: NickTheDude Posted at: 2016-12-12T16:27:34.207Z Reads: 131

```
I'd definitely reccormend increasing your voltage and using a lower kV motor. [One like this](http://alienpowersystem.com/shop/brushless-motors/alien-6374-hev-outrunner-brushless-motor-170kv-3300w/) on 10S would be perfect for the VESC. It would give you a much more powerful setup for similar cost.
```

---
## \#11 Posted by: Neilfenstein Posted at: 2016-12-12T19:06:32.659Z Reads: 124

```
Hi DreadBiscuit,

I saw your build thread as I was searching the forums for use of the Alien stuff.
I went predominantly Alien Power systems as they are UK based and hopefully should all work together. I wanted to simplify my first build where I could as I have  lot to learn. 
I went with the APS Controller as I really don't like the size of the GT2B and longer term I want to create a boosted board style thumb controller like a combo of the wiimote and the 3d printed mods done with the insides of the GT2B on this forum.

All my parts from Alien are still missing, I got a UPS shipping confirmation but it got cancelled, so I'm going to contact them later.
I only have the VESC, Batteries and donor board at the moment. I will let you know my thoughts on the Alien stuff as and when it arrives.
```

---
## \#12 Posted by: Neilfenstein Posted at: 2016-12-12T19:14:43.555Z Reads: 118

```
Hi Nick,

Thanks for the advice. I didn't have the confidence in the charging set up for 8 or 10s. So, I went the "noob guide" route for now and have ordered the 240kV motor from Alien and creating the 6s setup charging with an imax B6.

My next board or phase 2 will hopefully be 10s with BMS and simple charging solution with a matching motor 170/190kV. 

I am hoping that I will like the skate boarding and that I am keen to continue but right now I have tried to keep things simple and fairly cheap by avoiding import duty and buying things that are immediately compatible.

Thanks for the advice though.
```

---
## \#13 Posted by: Neilfenstein Posted at: 2016-12-12T19:33:44.901Z Reads: 120

```
Quick pic update on the stuff that has arrived, not much but here it is.
<img src="/uploads/db1493/original/3X/2/2/22536c1ab6afd213886e9a90d42a78ef597535c5.png" width="667" height="500">
Vesc fits in sideways nicely, may keep it this way for easy wiring to the motor.
<img src="/uploads/db1493/original/3X/4/a/4aa7697e4877c0b92e60ed9d906e8747d0f6e62c.png" width="663" height="500">
All laid out.
<img src="/uploads/db1493/original/3X/4/c/4ca447d66dad88f7f5d156dc85950d1a6e0c5846.png" width="667" height="500">
Cable connector layout, waiting on the silicon Cable to come :slight_smile: 
<img src="/uploads/db1493/original/3X/0/8/087b2d6f68c2e217b692285cfd5d247228948bdf.png" width="666" height="500">

Thats it for now

Neil.
```

---
## \#14 Posted by: Tonto2k Posted at: 2016-12-13T07:14:24.909Z Reads: 105

```
I'm interested to see how this build goes mate 👍
```

---
## \#15 Posted by: Neilfenstein Posted at: 2016-12-21T23:01:39.287Z Reads: 104

```
Hi guys,

I managed to get most of the wiring set up and mount the enclosure today. Still waiting on the bulk of the stuff trucks, wheels, mount and motor. But I'm in a position to probably just bold together and go (minus setting up the VESC:stuck_out_tongue_winking_eye:).
Parallel XT60 set up so I can connect up for charging ( sorry about the picture)
<img src="/uploads/db1493/original/3X/b/2/b2500635d0a5df34efbda909b4549adf452ae33f.png" width="450" height="500">
Wire for Loop Key
<img src="/uploads/db1493/original/3X/2/8/286415ea51ad6957c2d98282609b3671c8a408a7.png" width="631" height="434">
Final loop key
<img src="/uploads/db1493/original/3X/a/c/ac5c795e0ffda7778af3c942c3976737f5d193f1.png" width="586" height="403">
I'm a bit gutted I melted through heatshrink whilst holding with pliers during the soldering.

Here is how I decided to mount to the phase 1 enclosure.
<img src="/uploads/db1493/original/3X/a/a/aaf27f2b66246ff8f799e984fe0f4f455d57b7b5.png" width="516" height="500">
I used 16mm (5/8") countersink screws with load spreading washers. I put them through the Velcro straps which meant the straps and screws are taking the weight of the batteries rather than the enclosure. I then lined the base of the straps with the foam that the batteries were shipped with. Should hopefully protect the battery. I only show one bit here, but I doubled up.
<img src="/uploads/db1493/original/3X/7/7/77fa1cbedf410815c914a9f8ef62c43bdd0360c8.png" width="558" height="500">
Batteries in position
<img src="/uploads/db1493/original/3X/0/7/077cecc8fcf5393d322e98f0996d08e1f3e026ed.png" width="600" height="500">
Here is everything in position (except the receiver). I Also went ahead and started making a Simple Charging Plug how-to I followed ---> [MEB Charging plug](http://www.electric-skateboard.builders/t/miami-electric-boards-diy-charger-how-to/4242) 
<img src="/uploads/db1493/original/3X/7/c/7c6cd0df9b26b85c29fe2e06639d2ea5d0b4612f.png" width="690" height="414">
Here is a close up of the Loop connector and the motor cable holes. I just used HOT Glue for connector.
<img src="/uploads/db1493/original/3X/e/1/e14fbd4096d44faed3ff2d261b85e959dd80424e.png" width="690" height="485">
Here is a picture with the lid on. The box clips just miss the XT90s. hopefully enough room to squeeze the receiver in too.
<img src="/uploads/db1493/original/3X/d/0/d072d1938a61934f0dda1f9c9b666e0f48536040.png" width="690" height="363">
Here is a shot of the VESC light on :smile: 
<img src="/uploads/db1493/original/3X/e/3/e3d331af331fc0bc24de60bf5613c62f4a9c69d1.png" width="690" height="480">

So whats left to do, I am waiting on the thinner silicon cable to come in to finish the Simple charging plug which also needs a hole cut in the box, probably on the opposite side from the XT90. I am also waiting on the motor connectors to solder on the the VESC cables, once that is done I can then seal the holes and fix the VESC in the box.

I am excited for the rest of the stuff to come in. I can't wait it christmas everyday at the moment, Christmas day is just an awkward day when the post men aren't working :slight_smile:. 

In other news, my brother just bought a 3D printer so I plan on designing a new cooler looking enclosure ASAP.
```

---
## \#16 Posted by: kyo Posted at: 2016-12-22T04:25:59.644Z Reads: 86

```
Kool board !!! how do you mount the motor on the truck? weld the mount on ???
```

---
## \#17 Posted by: Neilfenstein Posted at: 2016-12-22T14:18:54.211Z Reads: 83

```
Thanks,

I am getting new trucks, these are just the originals with the donor board. I have APS trucks and mount on their way soon hopefully.
```

---
## \#18 Posted by: Neilfenstein Posted at: 2016-12-29T18:32:17.250Z Reads: 72

```
Yeah build complete!!!

I have been out for a few rides over the last couple of days :slight_smile:.

I managed to get the build complete for Christmas day so got to have a go on it after all the presents were opened and breakfast was eaten.

Its a bit weird weather here at the moment and the floor is quite damp after the morning frost has melted so my board is a bit mucky in the photos.

Here goes:-
Parts arrived Friday before Christmas eve
<img src="/uploads/db1493/original/3X/0/d/0de70fb943a927ac90b3e6a4d98a73ffbe827c32.png" width="399" height="500">
Close up of the pulleys and motor mount
<img src="/uploads/db1493/original/3X/8/c/8c814cb79d732492a9c90238941143709bad9a9a.png" width="433" height="500">
Close up of the controller, I really like it it has a smooth rubbery feel to it and is smaller than I expected.
<img src="/uploads/db1493/original/3X/c/4/c4b462942ffc0a50797d1058abdebd220cc0eba8.png" width="472" height="499">
trucks motor and pulley
<img src="/uploads/db1493/original/3X/5/e/5ef94856569fc08e17f5a1c8183719262241d24e.png" width="413" height="499">
Second short ride (near my work at lunchtime on the 27th dec) - tracked on my Garmin Fenix 3 GPS watch
<img src="/uploads/db1493/original/3X/5/b/5b026d0bc831f5cfa4bce079ae8b831c10a741bf.png" width="498" height="164">
Here is the finished board today
<img src="/uploads/db1493/original/3X/a/5/a5fc9cb3861dd8b29255f37afb0f8624c67ec60d.png" width="393" height="499">
Here is a close up of the mount and motor truck etc
<img src="/uploads/db1493/original/3X/7/a/7a1253f7ea89793e109c67170b754cfd6562acc4.png" width="443" height="500">
I made a little clip that holds the motor wires in place using a piece of heatshrink, washer and screw.
<img src="/uploads/db1493/original/3X/3/7/3740f882834062e1a446628e162b290381b51548.png" width="397" height="500">
Here is a picture of the clearance
<img src="/uploads/db1493/original/3X/e/4/e4dd1299ad6c0724ddea1b79c799cf60532d7bb7.png" width="690" height="288">
A shot with the board using the simple charging port that I added.
<img src="/uploads/db1493/original/3X/3/c/3c59911b274f483f9f9d0b93ee1a7ef161789669.png" width="673" height="500">
Finally here is my stats for my runs yesterday and today.
**Yesterday**
Speed
<img src="/uploads/db1493/original/3X/6/2/62a3e8f9c3fea53010b20452744bd51924a455ed.png" width="498" height="138">
Distance
<img src="/uploads/db1493/original/3X/4/e/4e568291ab3565c0b2b76c115c7e52d2d5415b72.png" width="497" height="222">
**Today**
Speed
<img src="/uploads/db1493/original/3X/a/e/aeb839760cecbdde5236291771bf42ed3d76eabf.png" width="496" height="135">
Distance
<img src="/uploads/db1493/original/3X/6/a/6a25e0583b3edd1156d985a1b42dbc9272656bfb.png" width="496" height="220">

I'm pretty pleased with it so far, I am a bit sketchy as high speed and I'm still learning to ride it but it is great. I don't think where I live is really made for esk8 but I'm giving it a go :slight_smile:
I'm impressed that I am on par with the esk8 calculator for speed. I have calculated my range to be about 11km but I so far have only clocked up 4.5miles (7.25km) in a single charge, but 4.5miles is roughly the distance to work so I should make it. I am nervous about trying it though as when I leave in the morning it is still a bit frosty.

Any questions let me know :wink:
```

---
