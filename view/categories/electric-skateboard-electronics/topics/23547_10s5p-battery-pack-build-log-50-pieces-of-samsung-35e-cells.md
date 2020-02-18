# 10S5P Battery Pack build log. 50 pieces of Samsung 35E cells

### Replies: 47 Views: 7822

## \#1 Posted by: SimosMCmuffin Posted at: 2017-05-20T15:09:00.401Z Reads: 616

```
Turns out you can't remove polls, so this poll will stay here.

[poll]
* Yes, I'm interested in a battery build log
* No, I'm not interested in how you build your battery packs
[/poll]


----------

## **Part 1, Planning and prep work**
You have decided to build your own battery pack and your new, precious and expensive cells have arrived from the supplier. If you didn't already figure out what kind of battery setup you're building, this is the time to do it, before starting to solder or weld anything together. There is also prep work that needs to be done to ensure safe and long lasting pack build.

_How will the pack be fixed in place?_ In my case I'm going to use my current board's execution style where the pack is friction locked in it's place inside the milled space with the help of some vibration absorbing foam tape. So when the bottom piece is bolted on, the milled inside space is high enough to allow the cells to actually move freely, but when the foam tape is added it squeezes the cells gently in place.
<img src="/uploads/db1493/original/3X/e/7/e759bfd0e2bb02b1cdf28876a090e42138882f15.jpg" width="602" height="499">

I'm going to change the layout of the cells a little bit from the earlier pack, which was shown above. I'm rotating the cells 90 degrees and stack them this way instead. The below picture is from a prototype deck, which wouldn't have been able to fit the 10S5P configuration I now plan on doing.
<img src="/uploads/db1493/original/3X/b/d/bddc6a4103d8592229b63aef7c1fcd5abaae80f0.jpg" width="690" height="226">

So I redesigned the deck so it would be able to fit a 10S5P and sent the new CAD-files for milling
<img src="/uploads/db1493/original/3X/f/e/fe6f8a76a5cb30f6c816ff5c05b4c42a7a4dfeda.jpg" width="690" height="336">

And here's the overall connection layout minus the balancing leads.
<img src="/uploads/db1493/original/3X/5/6/5623e5a5da91c7d6f380de281c255ea656e37d8c.jpg" width="690" height="388">

The cells are 50 pieces of Samsung's INR18650-35E, 3450 mAh, 10 A. Bought from Nkon for 3.11€ ea VAT free with company VAT number. Shipping was about 16€.
<img src="/uploads/db1493/original/3X/2/7/270aa30db0a2568f34bda671a6f9961b9c375c3b.jpg" width="690" height="231">
<img src="/uploads/db1493/original/3X/f/c/fce9a87ce6fc0e42f4835742f06b7b580946f167.jpg" width="638" height="500">


----------


_How will you assemble the battery pack?_ I re-thinked the assembly process after my first battery pack and came up with a quite neat and simple plan to build it.

1st, I weld up 10 pieces of 5 parallel packs.
<img src="/uploads/db1493/original/3X/9/d/9dd40aa450bf508b5df29511361978081c5c3f6f.jpg" width="458" height="499">

Then I connect the parallel packs in series with a couple short parallel tabs for better current carrying. I also will most likely add the balancing leads at this point.
<img src="/uploads/db1493/original/3X/9/e/9e815b2492438e276212cc00f05c4974fe3d3f19.jpg" width="481" height="499">

Then I will just fold out the pack into it's flat form, which will then fit into the board.
<img src="/uploads/db1493/original/3X/9/9/99dd67ec01e0782914a2db0a18c51a0877d39f0a.jpg" width="690" height="304">

The bends in the image are over emphasized for better illustration purpose. Once I have the pack folded out I will add some kapton tape to secure it mechanically better together.
<img src="/uploads/db1493/original/3X/d/5/d5f0d831cd7231b38326b0cf3678902c31374f5c.jpg" width="690" height="287">

----------


**Now that's the planning done, now the prep**
Before welding the parallel packs, care must be taken to ensure that all the cells that are to be connected in parallel have roughly the same voltage each. Otherwise you might connect for example, couple cells at 4.00 V with a one that is 3.50 V and that will cause a high current from the 4.00 V cells to flow into the 3.50 V one to even out the voltages and that might cook the cells due to the current. Worst case is that you have a fire.

In this case all the cells were around 4.13±0.02 V. I then did a final topping charge to the cells and got them all 4.19±0.01 V
<img src="/uploads/db1493/original/3X/e/8/e811132e78f8155d7dad4ef883ea32fe2aa30459.jpg" width="690" height="389">

If they do differ then they should be charged with a charger to full voltage to even them out. Like I did earlier, before measuring the cell voltages. This setup is my solar panel charger, which is charging the car battery, which to the Li-Ion charger is connected to. Green energy folks right there.
<img src="/uploads/db1493/original/3X/e/4/e4084402535931002efc48479c8093499651ea86.jpg" width="690" height="389">

I also now like to add an extra protection to the positive end of the cell to protect from short circuits caused by excess tab temperatures, which could possibly melt the plasticy protective ring around the positive terminal and short it into the negative terminal shell.

DANGER CLOSE! The positive tab is surrounded by the negative terminal shell and should be protected from accidental short circuits! (Image from batterybro.com)
<img src="/uploads/db1493/original/3X/d/e/de722c0dcd246664ed7be1b20d880cde97c124cb.jpg" width="668" height="500">

These adhesive cardboard ring add a little bit of thickness, but are much more resistant against mechanical and thermal stress. If you're planning on soldering your pack together, I strongly recommend these, as the longer heat exposure will start melting the plastic ones. These were bought on ebay.
<img src="/uploads/db1493/original/3X/0/7/07866c98763f6b727fab4af55218e1df537b1506.jpg" width="690" height="391">

**So to review the planning and prepping:**

* Figure out your pack configuration: 10S5P, 8S3P, 12S4P etc.

* Figure out how you're going to attach the pack onto your board

* Think through how you're going to assemble the pack. Tab connections, balancing leads

* Charge your cells to same voltage before starting to weld or solder

* Add extra protection to the positive terminal to protect from accidental short circuit to the negative outer shell, if necessary

----------


## **Part 2, Welding and assembly** (Unfinished and on hold, check post #6 for info)
We have our action plan together and our prep has our cells at the same voltage and the positive terminals are protected. It's time to start welding! well... almost.

<img src="/uploads/db1493/original/3X/2/a/2a00148b9d1de9ca8752674a5fe54fd8e431a1fe.jpg" width="689" height="324">

First we need to start testing and dialing in our welding settings. I usually start with the shortest pulse length and do a test weld and try to pull the nickel tab off of the battery and if it comes off easily, I up the power.

<img src="/uploads/db1493/original/3X/c/c/cc442c7a3eb31bb53c9113f0b19305d14129970f.jpg" width="690" height="338">

Turns out this legitimate pure nickel strip at this thickness (0.2 mm) is pretty dang good conductor, because I had to test all the way to max pulse length the welder could put out and only there were the tabs starting to stick well.
<img src="/uploads/db1493/original/3X/6/8/6897d70316886ae956de5a5c85a281592630910e.jpg" width="629" height="417">

After testing out the correct pulse settings for the weld, I measure out the needed tab length for the parallel packs and cut them with plain household scissors, because the nickel tab is pretty soft, but I wouldn't recommend using maybe the best scissors in the house still... I also snipped off the sharp corners for a little bit cleaner look.
<img src="/uploads/db1493/original/3X/2/3/23374bb03e8953e05d1c6b1a742bc2aa6d5b8be5.jpg" width="690" height="389">

I have 3D-printed a holder for the cells while I'm welding them that holds them in a straight line and I then add a rubber band to pull them together to make straight and tight packs.
<img src="/uploads/db1493/original/3X/8/a/8af86bb1ed6b95a41ce2a3c7b83065b8c3e389d8.jpg" width="689" height="248">

First parallel pack done!
<img src="/uploads/db1493/original/3X/e/0/e0c27fe8009caf492e701e2c254e96373a390ddf.jpg" width="690" height="439">

Halfway done.
<img src="/uploads/db1493/original/3X/0/8/08e11e1c6ac35abe60383eded7cafcc5307e2473.jpg" width="690" height="184">

All 10 parallel packs done!
<img src="/uploads/db1493/original/3X/3/6/369501be75a668c535141055761dbaa381ae9efe.jpg" width="614" height="500">
```

---
## \#2 Posted by: Okami Posted at: 2017-05-20T17:42:00.166Z Reads: 535

```
Tell something about your spotwelder too! I think seeing first hand spot welding experience is a rewarding thing! So just go on..

I think we got only a few documented cases about spotwelders on this forum.. :D
```

---
## \#3 Posted by: SimosMCmuffin Posted at: 2017-05-20T18:41:50.820Z Reads: 539

```
I'll start the build tomorrow, based on these encouraging results:
<img src="/uploads/db1493/original/3X/b/f/bfe59130c413729a6442c193beafcac007790fc4.jpg" width="642" height="176">


----------


My battery welder uses a car battery with a DIY double pulse electronic switch with a foot switch.
<img src="/uploads/db1493/original/3X/4/c/4ce2636b0ceb07d89674da568b8dc92bcedacbc3.jpg" width="690" height="389">

The idea is based on this welder that I saw in a hackaday article. I needed to start welding my first pack together quickly so I didn't bother ordering the custom pcb and parts, but rather compensated with a perfboard and components right off my shelf.
http://hackaday.com/2016/03/22/arduino-nano-runs-battery-spot-welder/

The controller gives an adjustable double pulse with the longer pulse being between 1-20 milliseconds and the first short pulse being only a tenth of that. I admit that it is not very aesthetically pleasing, but it was made with a pragmatic purpose to get building the battery pack.

I'm planning on designing a proper capacitive discharge welder with proper designed PCBs and an enclosure and a way to set the pulse length. I've been eyeing up the idea based on this design, but I'm most likely going to do some things differently. I just don't think the car battery based solution is very good for a long term use, as I feel like the battery slowly degrades over use.
http://www.zeva.com.au/Projects/SpotWelderV2/
```

---
## \#4 Posted by: Okami Posted at: 2017-05-20T18:44:21.324Z Reads: 500

```
well.. as long as it performs as it should, no problem ;)

Yeh I saw some earlier prototypes too of some of these arduino driven welders.. the circuitry is a bit crazy if you got to do everything with wires and want to make it compact :D
```

---
## \#5 Posted by: SimosMCmuffin Posted at: 2017-05-21T11:46:37.716Z Reads: 487

```
First part of the build log posted.
```

---
## \#6 Posted by: SimosMCmuffin Posted at: 2017-05-22T09:09:23.671Z Reads: 488

```
**Update on the build**. I can't finish it with my current welder because it doesn't have enough power to weld the tab-on-tab connections which are needed for connecting the parallel packs in series. This is because the new legitimately pure and quite thick nickel tabs conduct electricity so well, that they don't heat up to their melting point with the car battery welder. Against the battery terminals themselves it worked, but I had to crank pulse length to the max to make a decent weld.

<img src="/uploads/db1493/original/3X/f/e/fe6412acffb3781fdd2b67102aef429a4f555f4b.jpg" width="690" height="449">

I'm going to have to build a capacitive discharge welder to finish this build and that will take some time and this build will stay on hiatus meanwhile. If you have questions or anything related to this topic we can of course discuss about them here.

If you're wondering about capacitive or dual pulse welding here's a couple links on the subject:
http://www.spotweldingconsultants.com/capacitive-discharge-welders/dual-pulse.htm
http://www.powerstream.com/spot-welder.htm

And I'm going to build something based on this project:
http://www.zeva.com.au/Projects/SpotWelderV2/
```

---
## \#7 Posted by: Maxid Posted at: 2017-05-22T09:23:07.993Z Reads: 455

```
what thickness do the nickel strips have? I did not have any problems to weld nickel on nickel with my 0.15 strips from nkon and the arduino car battery welder (at a pulselength of ~14ms if I remember correctly).
The endless-sphere topic on it even had people weld copper with it!
```

---
## \#8 Posted by: SimosMCmuffin Posted at: 2017-05-22T09:30:40.306Z Reads: 459

```
It's 0.2 mm thickness and the problem comes when I'm trying to weld the tabs onto other tabs.

So I have a pancake of:
Electrodes
Series tab
Parallel tab
Battery terminal

It just can't heat up the contact points enough to weld the tabs onto one another.
```

---
## \#9 Posted by: Maxid Posted at: 2017-05-22T09:33:22.925Z Reads: 456

```
are you welding this pancake at once or layer by layer? I did mine layer by layer up to 3 on my series connections to allow for higher currents. I also added points with solder on the top most strip before welding it to the battery to be able to put some additional copper wire on top without heating the battery up too much.
```

---
## \#10 Posted by: SimosMCmuffin Posted at: 2017-05-22T09:48:54.281Z Reads: 473

```
I just updated the build log on the first post how it has progressed, but at the last image you can see the current situation. So when I'm adding the tabs to connect the parallel packs in series I can't get them to stick, they just don't weld well enough and come off too easily.

Actually here's a picture of the problem weld.
<img src="/uploads/db1493/original/3X/1/d/1dd88ec8b6cd7df7002ee97bc67aa36108e5e4b5.jpg" width="690" height="389">

So when adding the short series connection tabs, they are the problem at the moment.

@Maxid btw, can you post a picture of your electrodes you're using on your welder? Just interested in the tip shape.
```

---
## \#11 Posted by: Maxid Posted at: 2017-05-22T09:59:23.691Z Reads: 461

```
[quote="SimosMCmuffin, post:10, topic:23547, full:true"]
@Maxid btw, can you post a picture of your electrodes you're using on your welder? Just interested in the tip shape.
[/quote]

Sorry I don't have it around currently. I just used 16mm solid copper wire from home depot and filed it to be pointy
```

---
## \#12 Posted by: SimosMCmuffin Posted at: 2017-05-22T10:01:27.778Z Reads: 456

```
<img src="/uploads/db1493/original/3X/8/4/8410f56b6a109e1584f28a836b290ccc44bde05c.jpg" width="690" height="266">

Something like this?
```

---
## \#13 Posted by: Maxid Posted at: 2017-05-22T10:02:15.824Z Reads: 449

```
yeah - however I filed it on all sides to have a round shape with a pointy tip - like a pencil. From what i heard the pointier the better as the current heats that point up even more than a "large" surface.
```

---
## \#14 Posted by: SimosMCmuffin Posted at: 2017-05-22T10:03:26.689Z Reads: 443

```
Ok, I filed the pointy bit to be on the edge, so I can get them closer together when welding.
```

---
## \#15 Posted by: TarzanHBK Posted at: 2017-05-22T10:45:29.078Z Reads: 450

```
I see you´re using a 55Ah battery. That was my problem too. Got a new bigass 700A battery, tried again and now i´m able to weld at least 5 layers of 0,15mm nickelstrips with only 14ms timer :slight_smile: 
The other difference is the spotwelder itself. You´re using a different one.
@Maxid and I are using the arduino Spotwelder:
http://www.instructables.com/id/DIY-Arduino-Battery-Spot-Welder/
```

---
## \#16 Posted by: SimosMCmuffin Posted at: 2017-05-22T11:04:58.455Z Reads: 434

```
My welder electronically is an equivalent to the arduino one, although not as cleanly executed.  I might still go with the capacitive discharge welder, because then I don't need to lug around a big battery to weld, but I can use a small and lighter power supply to charge the capacitors back after a welding pulse. It has also the added benefit of being able to give higher current pulses.
```

---
## \#17 Posted by: TarzanHBK Posted at: 2017-05-22T11:09:54.390Z Reads: 428

```
alright! keep us updated :slight_smile:
```

---
## \#18 Posted by: SimosMCmuffin Posted at: 2017-05-22T17:57:50.317Z Reads: 437

```
I guess I'll update the progress on the new welder here. Anywhoo, the capacitor and MOSFET board design is pretty much done and I also did small 3D-model of the system in blender to figure out any immediate problems with it, but so far it seems pretty good. I sourced ebay for copper bus bar and decided to go with 10x10 mm size bar that I'm going to drill through some holes and then fasten them with screws onto the cap boards for minimum impedance.
<img src="/uploads/db1493/original/3X/a/3/a3795cc747db768d5ae3696ec971bc314a973a7b.jpg" width="671" height="500">

PCB layout looks as such.
<img src="/uploads/db1493/original/3X/f/e/feef6eba33797db39be779e8a438f01289144357.jpg" width="474" height="500">

I plan on putting 4 of these PCB-modules on the first version of the welder.
24 pcs of 47000µF 16V El.caps https://www.digikey.fi/products/en?keywords=565-2620-ND
16 pcs of IRLS3034-7 MOSFETs https://www.digikey.fi/products/en?keywords=IRLS3034TRL7PPCT-ND
```

---
## \#19 Posted by: Maxid Posted at: 2017-05-22T18:02:31.112Z Reads: 416

```
Caps for 100€ - wow. Wouldn't an audio cap have been cheaper? @whitepony uses one and seems to get pretty good results. Looking forward to your results.
```

---
## \#20 Posted by: SimosMCmuffin Posted at: 2017-05-22T18:14:29.842Z Reads: 420

```
I'll wait for @whitepony  to give a reply and tell about his experience with his welder and if he has had any power problems with it. He can also tell his thoughts on this welder build of mine.

I checked out a couple of car audio capacitors' ESR ratings, which were around 1.5 mOhm and with 24 of these caps in parallel they would have around 0.6 mOhm, enabling for higher current spikes, plus I think this design has a very good low impedance connections to it.

If he hasn't had any problems with it, I can just replace the car battery with the car audio cap and it should then be able to provide plenty of amperage.
```

---
## \#21 Posted by: SimosMCmuffin Posted at: 2017-05-22T18:20:09.554Z Reads: 415

```
Btw, do your welding cables start heating up after a dozen welds? Mine are ~7 AWG and they do start getting progressively hotter with the welds. The below IR picture is from after about 2 dozen closely done welds.

<img src="/uploads/db1493/original/3X/f/e/feca384beee09d4fa4805d20465930d05a7994b3.png" width="281" height="500">
```

---
## \#22 Posted by: TarzanHBK Posted at: 2017-05-22T18:26:50.422Z Reads: 400

```
I´m using 8 awg and they are getting warm after 10 welds and hot after about 20 welds when I´m fast
```

---
## \#23 Posted by: Maxid Posted at: 2017-05-22T18:28:35.906Z Reads: 403

```
yeah they get noticeable warmer but not hot.

@The_Dude has exactly the setup you proposed: car cap with timed mosfet switch instead of a car battery. Seems to work well: https://www.electric-skateboard.builders/t/dude-hubs-in-depth-dual-hubmotor-build/21519/55?u=maxid
https://www.electric-skateboard.builders/uploads/db1493/optimized/3X/8/8/8821dd89b27ab0e0b89511d008f39cdd470e36a7_1_666x500.JPG
```

---
## \#24 Posted by: whitepony Posted at: 2017-05-22T18:31:04.007Z Reads: 393

```
Im not a spot welding expert, but my audio cap works very well and it was a very cheap spot welder in total: https://endless-sphere.com/forums/viewtopic.php?f=35&t=70435&hilit=evolve+at#p1062504

not perfect, but I got pretty fast with batteries by now - would say I made about 10 batteries in total. my welding spots seem less pronounced & deep than others, but when I tried to separate the nickel strip from a cell, I tore off the strip and the nickel at the weld spots was still on the cell.

btw, my discharge wires are 25mm^2 (!!) and my copper rods are 5mm thick and they get quite warm to the touch after fast welding.
```

---
## \#25 Posted by: fedestanco Posted at: 2017-05-22T19:04:47.915Z Reads: 377

```
How would a setup like this perform compared to a sunkko 709?
```

---
## \#26 Posted by: SimosMCmuffin Posted at: 2017-05-22T19:46:44.885Z Reads: 380

```
@Maxid @whitepony @TarzanHBK
Now the question is whether a 1 Farad cap is going to be enough, because that I can go get immediately in a local shop. Otherwise I'll have to order it and wait for it to arrive and I'd like to get this pack welded together ASAP.
```

---
## \#27 Posted by: Okami Posted at: 2017-05-22T21:06:52.824Z Reads: 384

```
[quote="SimosMCmuffin, post:26, topic:23547"]
Now the question is whether a 1 Farad cap is going to be enough
[/quote]
im interested in this too. Get more info, please share it here, maybe :)
```

---
## \#28 Posted by: SimosMCmuffin Posted at: 2017-05-22T21:09:05.333Z Reads: 380

```
Well I just ordered a 1 Farad cap from UK for 14 £ with shipping so at least if it doesn't work at all, I'm not making a too big of a dent in my pocket and if it does work I can order a second one to connect in parallel :wink:
```

---
## \#29 Posted by: Sander Posted at: 2017-07-14T22:55:16.841Z Reads: 344

```
Any Update? :(
```

---
## \#30 Posted by: SimosMCmuffin Posted at: 2017-08-03T15:02:03.597Z Reads: 362

```
Update.

This process has been a b***h and a half, if I'd have to sum it up. Not going smoothly at all.

_**So what's been going on?**_

Well, I ordered the cheap car audio cap from ebay, waited a couple of weeks and was starting to wonder why the item had not been shipped. I go check the order on ebay and discover that the seller account I ordered the cap from has been terminated. Ok? I contact ebay support about not receiving the item and that the seller account doesn't exist no more, so I can't contact the seller anymore. Couple backs-and-forths with the support and they cancel the order and refund. Ok, wasted a lot of time there...

I go and find another audio cap that's the same model, but more expensive, but whatever I just want to get this project rolling forward and I order it. It finally arrives couple weeks later, so at this point I have already lost a month of time. I make it part of the system and replace the car battery with it. I test it. Nope, nothing, barely making a dent in the strip. Well just what the cuck man? When I give the welding pulse the voltage just crashes back to zero on the cap. I test the thick strips more, but they just don't weld, they simply don't heat up enough to get welded. Then starts the other part of this delay. I go to test the strip one more time and just by touching the welding anode and cathode on the strip causes suddenly sparks to fly. Wut?... It also turns out that I had borked up my grounding on the welder, which left the logic side partly floating and caused one the gates on the mosfets to basically fail, so it short circuited the mosfet internally (Or that's what I  post-mortem believe to have happened). Shooooot.... And I tried to see if I could get the mosfet desoldered, but with the large gauge wire soldered to the back of the board, it just sucked away the heat and I decided to just start designing a new one instead.

So then I spend a couple weeks designing a couple different PCBs for my different projects and sent them to manufacturing. 3 weeks later I got the new boards. Now I've gotten the new board assembled and just did a couple test welds with only the audio cap. Nope, still nothing. Well, s**t. I hook up the car battery in parallel with the audio cap. On max pulse length of 16 ms, there is a little bit of welding going on, but not something I'd trust to put under any sort of vibration. Hmmm.... what to do?.... Increase the length of pulse ofc. Crank it up to 64 ms and oh yes, we are welding boys.

Then I started to wonder why in world do I need such a long pulse length? Well, TLDR: The car battery is not stronk enough. Picture below of my oscilloscope attached to the terminals of the car battery.

<img src="/uploads/db1493/original/3X/f/5/f5efc940b8a73524ae931db45c2109893ad7738f.jpg" width="690" height="389">
<img src="/uploads/db1493/original/3X/1/f/1fd42f05ec8aec1de44d4f725b3a65fdc56e7f6b.jpg" width="690" height="389">

So the battery floats at about 12.6 Volts, then comes the first short pulse and the voltage dips to 8 V it then bounces back up during the short pause and then when the main welding pulse comes it dips back down to 8 V, so what does this mean?

These strips are goooood man. They conduct well so they don't heat up as much relative to the current and they sink the heat very well, due to them being 0.2 mm thick. The car battery simply can't provide the strong current pulse, because the voltage dips down, meaning the welding current also dips down, meaning that I have to use a loong pulse to get the contact points to actually heat up to welding temp. I guess I'll have to invest in a beefier battery at some point as @TarzanHBK 
[quote="TarzanHBK, post:15, topic:23547"]
I see you´re using a 55Ah battery. That was my problem too. Got a new bigass 700A battery, tried again and now i´m able to weld at least 5 layers of 0,15mm nickelstrips with only 14ms timer :slight_smile: 
The other difference is the spotwelder itself. You´re using a different one
[/quote]

The spot welder itself has no problems, barely heats up. I guess I'll try to finish this pack finally this weekend!

EDIT: Ok, I need another battery, because it still can't weld 2 strips on top of each other...
```

---
## \#31 Posted by: TarzanHBK Posted at: 2017-08-04T06:16:50.763Z Reads: 332

```
yep, it´s like our lipo batteries with to low c rating ;)
The poor car battery is simply not strong enough. You could use 2 or 3 of them in parallel or get a bigger one.
```

---
## \#32 Posted by: SimosMCmuffin Posted at: 2017-08-04T14:03:44.980Z Reads: 330

```
This thing pumps out some real angry pixies!

<img src="/uploads/db1493/original/3X/8/b/8b4c7bb39047a9a4ea83f47cb19299ab6a0e3f67.jpg" width="690" height="389">

The red lead jumps when I pulse the thing and I can now actually weld the strip on top of each other.
```

---
## \#33 Posted by: TarzanHBK Posted at: 2017-08-04T15:25:56.146Z Reads: 327

```
Nice :slight_smile:
Always funny when cables are jumping around because of high current :clap:
```

---
## \#35 Posted by: SimosMCmuffin Posted at: 2017-08-07T10:22:50.514Z Reads: 328

```
I can't edit the original post anymore to add the rest of the build log, so I'll just have to add it here.

**Continuing**
Time to add the parallel tabs... finally. I first finish 4 easy identical packs, which will then be assembled into a bigger pack.
<img src="/uploads/db1493/original/3X/5/6/5644a2a1983bb5b3a4c8557ad149ae1e355c1f2c.jpg" width="690" height="423">

Now here's the both halves of the pack done. There are also parallel tabs on the bottom to complete the circuit.
<img src="/uploads/db1493/original/3X/3/d/3d5f38c5101ebf76c1c9c11d8f95068ee7155451.jpg" width="651" height="500">

**Time to prepare the balance leads**
Now comes the interesting part of the build, which I don't think anyone here has done it like this before. First we need some small nickel strips. I cut the pieces in half lengthwise.
<img src="/uploads/db1493/original/3X/e/c/ec359247d80a2d53c818dac68d471be03ea9883d.jpg" width="690" height="350">

Now we can solder the balance lead on to the strip.
<img src="/uploads/db1493/original/3X/b/8/b8009ee463835f330ecc6905c714068233a9540d.jpg" width="689" height="308">

Money.
<img src="/uploads/db1493/original/3X/e/1/e18ecdf90869b5c427df087638c9653aeb23f253.jpg" width="690" height="372">

And then finish the leads by heatshrinking the ends for a neater look.
<img src="/uploads/db1493/original/3X/5/4/549ec2530f947fb352ba8f56276c7d8193dd7635.jpg" width="690" height="491">

Now I can weld the rest of the pack and I can just weld the balance leads onto the strips. No soldering iron anywhere near the pack at any point.
<img src="/uploads/db1493/original/3X/7/3/739ba3c9d9185c541bdb0c539a342feb38c7ff9e.jpg" width="690" height="389">

I then folded the pack out just like shown in the original post's planning stage.
<img src="/uploads/db1493/original/3X/5/4/5435c4decc066533662c2bfdb4c9652f525af3fa.jpg" width="690" height="354">

Close-up.
<img src="/uploads/db1493/original/3X/b/5/b5279034fae9bcb66b247a9234a13afd88657320.jpg" width="690" height="389">

I then routed the balance leads to the front of the pack and taped everything together to add some rigidity.
<img src="/uploads/db1493/original/3X/9/3/938a723e0885b54bf962a2cf9beee2c8b4eb6927.jpg" width="690" height="353">

It fits so snuggly into the board. Although it should, because I designed the board from the beginning for this battery pack.
<img src="/uploads/db1493/original/3X/a/6/a6d034412b42d3a9b318abd48067410d095ad092.jpg" width="690" height="389">

I'm most likely going to go with a XT60 power connector, which will plug into my own BMS module. I have XT90-S loop key, so I don't have to worry about the in-rush currents.

**Summary and afterthoughts:**
I think I'll have to admit that I used too thick of a nickel strip. The 0.2 mm thickness is just overkill for the currents I spec'd this battery for. Mind you this is genuine pure nickel that I tested and verified. I'm still not 100% happy with the welds and their penetration. They could be better, but would require a complete rework on the pack, so I plan on going with what I have now and seeing if it survives. If the welds come undone, I'll rebuild the whole pack with thinner strip (0.1 or 0.15 mm).

The most challenging part of the build was in the assembly stage after I had folded the pack out and needed to route the balance leads to the front. Problem was flipping the whole pack neatly onto it's pack, while it did not have all the tape giving it some structural support. Ideally at the point you see in the last picture, would be to shrink the whole pack with a _big_ PVC heatshrink sleeve to give it a neater look and give more mechanical support to the pack. I do believe that the strips will stay connected as long as there isn't any rotational or twisting motion applied to them.
```

---
## \#36 Posted by: SimosMCmuffin Posted at: 2017-08-28T21:32:56.735Z Reads: 309

```
Figured out in part why the car audio capacitor did jack squat for the spot welds.

Being bored in the evening, I decided to strip the capacitor down to the cap itself. So I removed the voltage display module and removed the PVC shell with the "1 Farad - 1000 Watt audio capacitor" text on it. We'll see about that...

<img src="/uploads/db1493/original/3X/9/c/9c3c162fa188f7244ea05884bb554047e5b3ddc0.jpg" width="690" height="389">

I decided to test the real capacitance of the capacitor by doing a RC time constant measurement https://en.wikipedia.org/wiki/RC_time_constant

I set my power supply for 10 Volts and connected a 10 Ohm resistor in series to the capacitor, So if the cap really has 1 Farad capacitance, the voltage should rise to 6.3 Volts in 10 seconds...

<img src="/uploads/db1493/original/3X/c/7/c760ab338d47e7a39aa006e0141f330ca7fee1c8.jpg" width="690" height="389">

Except it only took 2 seconds...

THIS FRICKIN' THING IS ONLY 0.2 FARAD CAPACITANCE!!! NO WONDER IT DIDN'T DO ANYTHING TO THE WELDS!

http://i0.kym-cdn.com/photos/images/newsfeed/000/072/009/reaction_image_1185.png

Color me semi peeved off....
```

---
## \#37 Posted by: SimosMCmuffin Posted at: 2017-08-29T13:15:37.121Z Reads: 298

```
But wait! There's more!

Decided to cork this POS open to see what is inside...

So I mangled the end of it open.

<img src="/uploads/db1493/original/3X/f/f/ff14ea83492830e46f573ad90f5c9e874270e27a.jpg" width="577" height="500">

That looks like... cement?...

<img src="/uploads/db1493/original/3X/7/9/797aadda5a9cdd83e06813198149ec4af515d553.jpg" width="519" height="500">

Oh, it **IS** cement. I can now guess where this is going...

<img src="/uploads/db1493/original/3X/2/2/22d01e0efbe39e6276dc578e9e316a9eca0b574a.jpg" width="690" height="389">

Did two long cuts length wise on both sides to start cracking it open. Hmm... those look like normal small caps...

<img src="/uploads/db1493/original/3X/2/1/210778c089648520586f3fa0bd83c531f77dd457.jpg" width="690" height="389">

MotherF****!

<img src="/uploads/db1493/original/3X/2/a/2a9b1720a4aefa43e944d220d6c4e4e5de167245.jpg" width="690" height="389">

With a god dang cement puck at the other end!

<img src="/uploads/db1493/original/3X/4/f/4f3749e5eeb028ee9cab77d6b0ee22217f39dc4f.jpg" width="566" height="500">

I already wish I could shove this up the arse of the chinese bastard who made this scam...

<img src="/uploads/db1493/original/3X/7/d/7dafe7109625dee5f9da753c5fa89e5647bcb85f.jpg" width="690" height="389">

Welp, it's a fake confirmed. So maybe a closer look at these el.caps explain why the measured capacitance was only 0.2 Farads from the promised 1 Farad one...

<img src="/uploads/db1493/original/3X/5/2/529f9ceab54745c12109382189b74a2546999308.jpg" width="690" height="389">

16 V 10000 µF caps.

<img src="/uploads/db1493/original/3X/e/d/ed6ed43e6004bcac13fd16a654e65e692881370d.jpg" width="690" height="389">

And there's twenty of them... Well, THERE'S MY GOD DANG 0.2 FARADS OF CAPACITANCE ALRIGHT!

@Okami @whitepony @Maxid @TarzanHBK    

http://www.dailydogmemes.com/bamb-thumb.jpg
```

---
## \#38 Posted by: Maxid Posted at: 2017-08-29T13:43:06.759Z Reads: 286

```
wow - reminds me of these:
<img src="/uploads/db1493/original/3X/7/b/7b976d93a6d0b9d83681be86124f633343088b2f.jpg" width="375" height="500">

Glad you at least got some welds done
```

---
## \#39 Posted by: darkkevind Posted at: 2017-08-29T13:48:24.656Z Reads: 279

```
WTH is that supposed to be? A powerbank?
```

---
## \#40 Posted by: SimosMCmuffin Posted at: 2017-08-29T13:50:16.343Z Reads: 280

```
Either a "high-capacity" usb storage device or a power bank.
```

---
## \#41 Posted by: Maxid Posted at: 2017-08-29T13:59:44.464Z Reads: 281

```
these are chinese usb drives that are obviously sold with much higher capacity as they actually have just like @SimosMCmuffin said.
```

---
## \#42 Posted by: darkkevind Posted at: 2017-08-29T14:03:06.851Z Reads: 277

```
Ahhhh! Hahahahaha! Now I see....! Portable drives that are actually just USB sticks.... Amazing...


Hmmm.... get rich quick scheme, update.... :smirk: :+1:
```

---
## \#43 Posted by: Ronny_CTS Posted at: 2017-08-29T15:05:03.650Z Reads: 264

```
HAHAHA...that cement "cracks" me up...
```

---
## \#44 Posted by: SirDiff Posted at: 2017-08-29T15:43:56.668Z Reads: 265

```
Have you tried opening the smaller caps? RUSSIAN DOLL EFFECT
```

---
## \#45 Posted by: SimosMCmuffin Posted at: 2017-08-29T16:21:50.456Z Reads: 269

```
Jokes aside. The tested capacitance was pretty much exactly what the smaller caps were put together 20x10000µF = 0.2 F, so no reason to suspect further bamboozling
```

---
## \#46 Posted by: TarzanHBK Posted at: 2017-08-30T06:18:14.032Z Reads: 252

```
lol these bastards :sweat_smile:
I wonder how a chinese company sits in their team meeting and goes like: 
"What should we copy and fuck up from the western people next guys?"
- "Let´s build some cement-capacitors to reach the weight of the real one!"
:monkey:
```

---
## \#47 Posted by: scepterr Posted at: 2017-08-30T06:19:49.334Z Reads: 258

```
This is a proven practice for them with 18650 and other cells<img src="/uploads/db1493/original/3X/e/8/e8318516ebcf8fbbfa789c29975d9b024f09bb75.jpg" width="164" height="250">
```

---
## \#48 Posted by: Marsen Posted at: 2018-08-17T07:24:46.640Z Reads: 119

```
Amazing what people do to make a buck. 
I was looking at getting some large capacitors for a Power Factor correction device. Will be very careful where I get them from after seeing this.
```

---
