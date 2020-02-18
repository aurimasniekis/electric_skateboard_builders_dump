# DIY Boosted Board &#124; Custom Deck &#124; Paris Trucks &#124; SK3 192 kv &#124; Custom Mount &#124; 10S2P &#124; VESC

### Replies: 29 Views: 6935

## \#1 Posted by: mschil2440 Posted at: 2016-05-17T23:49:27.236Z Reads: 535

```
Hello All,

If you couldn't tell by the build title, my plan is to make a board copying the design of the Boosted Board. This will be my first e-board build and I have done a decent amount of research and reading on this forum. The only parts i've bought so far are paris trucks and Orangatang wheels (same as the boosted board).

<img src="/uploads/db1493/original/2X/7/767a36845c111b021557badf1700bc1d6e762955.jpg" width="690" height="388">

As for the rest of my plan: 

**Battery**: 6 x [5000 mAh 2S 20C lipos] wired together as 2 6S packs in series to function as a 12S. As for charging, I plan on charing them as 2 6S packs. I'm also hoping I can install a battery screen reader thing to show me how much juice is left.

**Motor**: Turnigy Aerodrive SK3 - 6364-190kv Brushless Outrunner Motor. Not much else to say about this, haven't seen any bad reviews on Turnigy thus far...

**VESC**: from Enertion, originally planned on a car ESC but this is the same price and I've read a lot about it on this site.

**Transmitter**: HK-GT2B. Planning on eventually modifying the case to make it smaller once my board is fully functional.

**Board**: I am making my own deck (2nd time) copying the boosted design

**Gears**: After using the gear ratio calculators I'm going with a 15 tooth motor wheel and a 36 tooth drive wheel. And following some users tips, an Enertion timing belt.

My plan is to first assemble a dirty board to make sure all the mechanical and electrical parts work well. Then I want to make the final board as slim as possible (thats why I chose 2 cell lips).

I will continually update this build thread as my parts start arriving and as the board gets put together. 

Feedback is **GREATLY** appreciated! Anything at all, I would like to know what you think!

Thanks,
Matt
```

---
## \#2 Posted by: Chris_KP Posted at: 2016-05-18T00:14:53.062Z Reads: 502

```
You should have bought kegles instead of in heat wheels because you will have to drill through them and build a jig instead of having the holes already there.
```

---
## \#3 Posted by: barajabali Posted at: 2016-05-18T00:28:18.002Z Reads: 503

```
If you want to make a true copy of bb 

Use 26650 batteries 
Dual drive higher kv sensored
Vanguard flex 3 (black grip tape)


Just my input if you're actually wanting to make a copy
```

---
## \#4 Posted by: Mrmoonlight Posted at: 2016-05-18T05:08:43.975Z Reads: 465

```
Boosted uses Caliber trucks too. Since they're square-ish, you can attach a motor mount without having to deal with welding.
```

---
## \#5 Posted by: mschil2440 Posted at: 2016-05-18T21:36:17.701Z Reads: 457

```
@Chris_KP I considered kegles but I just love the look of the in-heats. I'm hoping drilling through the wheels isn't a huge deal with the use of a drill press.

@barajabali I am currently siding with lipos because I have no experience with 26650 batteries and it just seems like a lot could go wrong with finding working cells and soldering packs. As well as I want to make a slim board different from the way Boosted laid out their enclosures. I am making my own board to save money. Here's my blueprint...
<img src="/uploads/db1493/original/2X/7/73b07025d847467774ea643e70c759edbad73e2b.jpg" width="353" height="500">

@Mrmoonlight I wish I would have noticed that before I bought the paris trucks... I'll make due, there is a local place that can weld for me.
```

---
## \#6 Posted by: barajabali Posted at: 2016-05-18T21:37:30.295Z Reads: 406

```
This could be your chance to learn how to make battery packs it's really easy once you start
```

---
## \#7 Posted by: mschil2440 Posted at: 2016-05-18T21:38:26.891Z Reads: 393

```
Where do you suggest buying/ finding them from?
```

---
## \#8 Posted by: barajabali Posted at: 2016-05-18T21:40:41.376Z Reads: 401

```
We did a group buy for 18650 battery's from liion whole sale .com or something like that. They sell 26650 too
```

---
## \#9 Posted by: Jinra Posted at: 2016-05-18T22:10:39.434Z Reads: 390

```
If you're in the states you can easily find Samsung 25R Li-ion 18650 cells for $5 each. A123 makes some high power 26650 LiFePo4 cells too, but they're twice the price.
```

---
## \#10 Posted by: longhairedboy Posted at: 2016-05-18T22:48:23.809Z Reads: 386

```
[quote="Jinra, post:9, topic:3427"]
Samsung 25R Li-ion 18650 cells for $5 each
[/quote]

those are my favs right now. mmm mmm good.
```

---
## \#11 Posted by: mschil2440 Posted at: 2016-05-18T23:49:05.085Z Reads: 375

```
How are 18650 cells labeled? Compared to lipos... I was looking to have a 12S lipo 5000mAh 20C
```

---
## \#12 Posted by: Jinra Posted at: 2016-05-18T23:55:10.382Z Reads: 377

```
If you're asking how to get comparable specs as that lipo, you'll need 12 cells (thus the 12S) in series and probably 2 in parallel to reach 5amp hours. This probably won't reach 20C but should have enough amp output for most boards, especially at 12S.
```

---
## \#13 Posted by: Chris_KP Posted at: 2016-05-19T01:15:23.793Z Reads: 361

```
Ok if you have any question on drilling wheels ill be happy to help :slight_smile:
```

---
## \#14 Posted by: Kaly Posted at: 2016-05-19T18:12:52.971Z Reads: 356

```
[quote="mschil2440, post:5, topic:3427"]
Here's my blueprint...
[/quote]

You want to move the battery as close as you can to the front truck, the flexing in the middle of the deck will damage your lipos.
```

---
## \#15 Posted by: mschil2440 Posted at: 2016-05-23T00:45:48.778Z Reads: 333

```
Very close to switching to 18650 cells vs Lipo. Only thing holding me back is connecting the cells. From what I've seen and read everyone uses spot wielding. I don't own a spot welder. Is it to dangerous to solder the cells together? Or does that create too much heat?
```

---
## \#16 Posted by: mschil2440 Posted at: 2016-05-23T00:54:59.525Z Reads: 379

```
Just finished clamping down the board blank with a concave press. Used 4 x 1/8 in plys of baltic birch and used spray adhesive to temporarily secure the board blueprint.
<img src="/uploads/db1493/original/2X/4/4dd4032dabd038dc4d326628d2bcb4475e4fbedd.jpg" width="281" height="500">
<img src="/uploads/db1493/original/2X/5/54a7eb45cd15628b3b24fbecd69077c772de77c8.jpg" width="690" height="388">
<img src="/uploads/db1493/original/2X/0/065a434a74e0493dd619f2ac83ed9a50f6d4e13f.jpg" width="281" height="500">
```

---
## \#17 Posted by: mschil2440 Posted at: 2016-05-29T18:48:17.089Z Reads: 370

```
Finished cutting out the board with a jig saw and cleaned up the edges with a sanding block and a belt sander. Batteries also arrived. I changed my original plan from 12S to 10S with 5 x 2S 5000mAh LiPos. Waiting for the BMS to arrive and I will jump into soldering the packs to the board and making a temporary quick n' dirty enclosure. Almost every other component I need to buy is on backorder and has been for a month. Also kind of upset VESC price on exertion went up $30. I have a feeling this build is going to hold a lot of waiting for parts to restock and arrive.
<img src="/uploads/db1493/original/2X/a/ab9cf7ffb903458071de252a6fe2e584db7fc053.jpg" width="690" height="388">
<img src="/uploads/db1493/original/2X/1/19255f35b17a7683dc4285b84782a0d684108078.jpg" width="690" height="388">
<img src="/uploads/db1493/original/2X/b/bda3009212f6a5c957f7873f034d24f5b7e75831.jpg" width="690" height="388">
```

---
## \#18 Posted by: mschil2440 Posted at: 2016-06-03T15:13:39.405Z Reads: 350

```
Just received most of my battery pack components. Finished soldering all the balance leads to the BMS plug. Just need to connect the main power wires in series to create a 10S pack. Please don't judge me on the tape job, only temporary to hold everything together and not stress any wires!!!

<img src="/uploads/db1493/original/2X/8/8eddf3f960bd956718767a518397475c2ec48cf0.jpg" width="690" height="388"><img src="/uploads/db1493/original/2X/8/8454c8efd2b762812823c6a9bde00fca53e2d0b3.jpg" width="690" height="388">
```

---
## \#19 Posted by: mschil2440 Posted at: 2016-06-03T15:15:12.615Z Reads: 344

```
HELP NEEDED:

I want to wire in a voltage reader or a "fuel tank" display and an anti-spark circuit to allow the use of a simple low current switch. Does anyone have any nice diagrams or insite they could share?

Thanks
```

---
## \#20 Posted by: Maxid Posted at: 2016-06-03T16:38:53.130Z Reads: 352

```
This should work. This way the voltemeter will not be connected when the AS is "off" and thus not drain your battery

<img src="/uploads/db1493/original/2X/6/68bb9636641b2a656faadae39d6db28b698ae5d2.PNG" width="690" height="292">
```

---
## \#21 Posted by: ajaynagra Posted at: 2016-10-16T17:32:40.299Z Reads: 247

```
Did you finish this build?
```

---
## \#22 Posted by: mschil2440 Posted at: 2017-06-28T11:52:59.376Z Reads: 172

```
Been a very long time since last update. I believe everything is finished on my board. HOWEVER, I cannot get my controller from torqueboards to pair with the receiver... I've done everything on the instructions but cannot get the initial pairing complete. If anyone knows how to troubleshoot, help would be appreciated.
```

---
## \#23 Posted by: mschil2440 Posted at: 2017-07-10T11:43:45.429Z Reads: 162

```
I was finally able to pair my mini 2.4 ghz transmitter to the receiver thanks to this video:
 https://www.youtube.com/watch?v=ywUfqtKF8Zg&t=28s

I find it kind of funny how this has been the issue holding up my eboard build for the past year. The instructions that came with the remote do not explain how to pair the receiver and if it wasn't for this video I would have bought another transmitter. 

With that, it marks the "end" of the electronics build for my DIY Boosted Board. I say "end" because I can guarantee something will break, need replaced or need upgraded very soon but until then we can pretend it is finished.

Now time for my favorite part, making it look **_PRETTY!!_:hammer:**
```

---
## \#24 Posted by: Decdog Posted at: 2017-07-10T19:05:35.608Z Reads: 152

```
Pics? 
Tenchars
```

---
## \#25 Posted by: mschil2440 Posted at: 2017-07-11T15:01:19.419Z Reads: 152

```
Pictures of the completed electronics. I plan on trimming some wires and replacing plug connections with soldered connections. I also want to eventually wire in a voltmeter "Fuel Gage" and a anti-spark circuit with a nice looking toggle switch. 
<img src="/uploads/db1493/original/3X/b/3/b3c10409bbee907fbe6eebb6cdde26f4ad1c7cff.JPG" width="666" height="500"><img src="/uploads/db1493/original/3X/3/f/3f41810820459611058350bd733271ac736498ff.JPG" width="666" height="500"><img src="/uploads/db1493/original/3X/3/3/3336aaf2175a52f6e64b2a596123510a8a08044e.JPG" width="666" height="500"><img src="/uploads/db1493/original/3X/9/0/90549611b150fe8228c1f31b3e57853f7af3c8d4.JPG" width="666" height="500">
I held everything down with some duct tape for a quick test ride and it was awesome. The motor struggled a bit trying to start motionless, but with one push, it had no problem accelerating. Haven't taken it even close to top speed so that is still unknown. 

My plan for beautifying the board deviates a little from the actual boosted design. I want to countersink as much of the battery brick as possible and cover it with a smooth sloping lid. The Tupperware container in the pictures fit the batteries perfect but did not have room for the VESC. Still tossing around the idea of making a carbon fiber cover, if anyone has any tips or suggestions shoot away.
```

---
## \#26 Posted by: mschil2440 Posted at: 2017-07-14T17:49:04.733Z Reads: 130

```
VERY HELPFUL SOLDERING TIP:
I was struggling big time trying to solder thick gauge battery wire before learning this tip.

First, spread out the strands of wire for the 2 wires I am going to solder together
<img src="/uploads/db1493/original/3X/6/6/66a3c35d2f6a2cb3febed3e7305fd329e56cf8ac.jpg" width="666" height="500">

Next, combine the 2 wires head on, interweaving as many strands as possible and squeeze the combo together.
<img src="/uploads/db1493/original/3X/f/7/f7cc85b500e2f4153ddfc8e7641744e56ae16817.jpg" width="666" height="499">

After that, use a thin wire pulled from a separate wire to wrap around the bundle creating a very strong joint.
<img src="/uploads/db1493/original/3X/f/7/f710e17df7f2a85d2425fbb27718966dbdfe0f5b.jpg" width="666" height="500">

Finally, simply solder the connection like every other solder joint.
```

---
## \#27 Posted by: Smorto Posted at: 2017-07-15T01:08:33.486Z Reads: 120

```
You can also twist the 2 wires together after your push them together. Then wrap the thing wire around and you will have a very good joint.
```

---
## \#28 Posted by: mschil2440 Posted at: 2017-08-08T16:12:25.281Z Reads: 106

```
HELP PLEASE:
So my board was up and running for a few days. I was hesitant about taking it too far because the battery had still never been charged. On my last ride, the motor slowed way down and I had to push to get home. I assumed it was because the battery had finally died. After charging the battery, I plugged everything in to go for another ride, but the motor wouldn't run. The battery is confirmed charged and my remote paired successfully. The VESC started blinking a pink/red light. I read that that could be due to a short in the motor wires and decided to check it out in the BLDC tool. I am not very experienced in this tool so I started watching some intro videos, but I can't even get the BLDC tool to recognized my VESC. It displays, "serial port error: 2"

Does anyone know how to solver error 2, or know what the blinking red light means?

Thanks,
Matt
```

---
## \#29 Posted by: darkkevind Posted at: 2017-08-08T19:10:37.739Z Reads: 95

```
Best place is https://eu.nkon.nl/rechargeable/18650-size.html
```

---
