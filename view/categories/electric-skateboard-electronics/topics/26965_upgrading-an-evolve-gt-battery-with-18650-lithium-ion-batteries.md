# Upgrading an Evolve GT battery with 18650 Lithium Ion batteries

### Replies: 186 Views: 21099

## \#1 Posted by: Eboosted Posted at: 2017-07-07T05:02:28.590Z Reads: 827

```
Hello guys I know there has been another topic about this already but didn't want to hijack it, besides I wanted to do a step-by-step tutorial so others could easily benefit from it.

Step 1:
Remove the 8 screws holding the battery and turn it over:
[img]http://i.imgur.com/VskA7xs.jpg[/img]
[img]http://i.imgur.com/aa1rEw2.jpg[/img]

Step 2:
Unplug the motor phase and sensor wires

Step 3:
Unplug the battery from the BMS, the original battery is a 10S made of 10 LiPo pouches.
[img]http://i.imgur.com/7kTXKY4.jpg[/img]
[img]http://i.imgur.com/1mTlX4e.jpg[/img]

Step 4:
Unplug the balancer plug from the BMS and desolder the 4 red wires from the positive lead of the battery pack
[img]http://i.imgur.com/Zi8TfgE.jpg[/img]

Step 5:
Desolder the 2 wires on the negative lead of the battery pack
[img]http://i.imgur.com/WnhBx6M.jpg[/img]

Step 6:
Get some 18650 Batteries, I used some Samsung 25RI had laying around
[img]http://i.imgur.com/VoKKvJz.jpg[/img]

Step 7:
Use cardboard isolating rings around the posituve lead of each cell in order to have an extra layer of short protection and sport weld them
[img]http://i.imgur.com/kNdRn22.jpg[/img]

Step 8:
Spot weld 4 each one of the four leads to make 5 x 2S4P
[img]http://i.imgur.com/x7r2GnC.jpg[/img]

Step 9:
Bend the pack:
[img]http://i.imgur.com/R6VQIck.jpg[/img]
[img]http://i.imgur.com/TICW9qg.jpg[/img]
[img]http://i.imgur.com/lbbmo2O.jpg[/img]
[img]http://i.imgur.com/HpLqB8i.jpg[/img]

Glue them together with hot glue silicone
[img]http://i.imgur.com/Z7QJIJa.jpg[/img]
[img]http://i.imgur.com/Y4CkMqb.jpg[/img]

Reconnect the BMS and solder the lead wires:
[img]http://i.imgur.com/RToc0hA.jpg[/img]

I run into an issue here, @longhairedboy could give me a hand?

I'm getting only 31.78v on the battery plug however if I meassure the pack directly I get 35.66, I'm not sure where the other 3.88v went! 

Meassuring from the battery plug:
[img]http://i.imgur.com/nwS7xIx.jpg[/img]

Meassuring the whole pack directly:
[img]http://i.imgur.com/RToc0hA.jpg[/img]

I took advantage of the procedure to change the faulty Evolve BMS for a the new one from them but there was 1 red wire I left unconnected because I didn't know where to solder it on the BMS, there were no instructions, maybe that's the problem.

I'll update the tutorial once I sort this out.
```

---
## \#2 Posted by: Bataleon Posted at: 2017-07-07T08:47:54.971Z Reads: 696

```
Really nice, clear pics. Thanks for sharing.
```

---
## \#3 Posted by: longhairedboy Posted at: 2017-07-07T11:49:36.875Z Reads: 685

```
The red wire should be the #10 balance lead and go to positive on the pack, IIRC. I don't have a unit in the shop at the moment but there are two coming in for this upgrade so i can take a look then. 

EDIT: I just saw your PM about having the #10 already connected. When the two come in i'll look and see where that mysterious extra wire is supposed to go. 

That's how its done though. That's how you make the flexi pack. I also add some 180mm heat shrink over each P group and let it overlap just a little onto the next one, sort of like scales. That allows it to still flex but keeps things nice and neat.
```

---
## \#4 Posted by: Smorto Posted at: 2017-07-07T17:47:42.553Z Reads: 660

```
[quote="Eboosted, post:1, topic:26965"]
Bend the pack:
[/quote]


Nice job on the pics. I am getting confused as to what you do after you bend each 2s4p pack. So you put all of them next to each other like in a few pics down, but you never sport weld each of the 2s4p packs together? What am I missing here?
```

---
## \#5 Posted by: Eboosted Posted at: 2017-07-07T18:45:24.582Z Reads: 646

```
Here are the pictures on both sides, so you can see them better, the read rings are positive terminals on each cell

[img]http://i.imgur.com/NW54UkR.jpg[/img]
[img]http://i.imgur.com/wGj4FdE.jpg[/img]
```

---
## \#6 Posted by: Smorto Posted at: 2017-07-08T01:03:41.401Z Reads: 612

```
Ahh ok. Why did you use the method of folding the pack like that when you could have done a diagram similar to this?
<img src="/uploads/db1493/original/3X/5/a/5a12f27ac9794cd173c458d6bbdffc09432d5d94.png" width="690" height="432">
```

---
## \#7 Posted by: Jinra Posted at: 2017-07-08T01:05:34.532Z Reads: 599

```
Thats exactly how I have my 10s4P pack. a possible downside to this is that if you don't have your pack 100% secure the two sides can possible come in contact and short. I kapton'd both sides and put some rubber in between to be safe, but it is a bit concerning :smile:
```

---
## \#8 Posted by: Smorto Posted at: 2017-07-08T02:45:03.208Z Reads: 600

```
Cool, I like the idea of the design that @Eboosted is using because it eliminates that risk.

One question for @Eboosted though, can you spot weld the packs together on the sides instead of using a bit of wire? I feel like spot welding them would put less heat into the cells and maybe a bit stronger?
```

---
## \#9 Posted by: Eboosted Posted at: 2017-07-08T06:45:14.191Z Reads: 598

```
@smorto that's correct, i used my method as I once had a short on my pack with your diagram, even thought I isolated the center with cardboard. 

With my layout you eliminate that risk, the only downside is that need of a long positive wire to go back to the BMS, but that wasn't a big problem, however it added a little bit of thickness to the pack, hope it closes good tomorrow. 

BTW in regards the difference on voltage before and after the BMS, I found it to be pretty normal, once you connect the BMS to the ESC the pack voltage was perfect. So don't worry if the unconnected battery has a lower voltage output. 

Step 10:
Use 180mm battery heat wrap to cover the battery
<img src="/uploads/db1493/original/3X/3/e/3e2238786a69369bb3203361a404558b43e35b9a.jpg" width="666" height="500">

Step 11:
Use a heat gun at 250 Celsius.
```

---
## \#10 Posted by: Smorto Posted at: 2017-07-08T14:40:06.271Z Reads: 569

```
Just one more thing, could you spot weld the packs on the side instead of using silicon wire like you did?
```

---
## \#11 Posted by: Eboosted Posted at: 2017-07-08T14:42:21.103Z Reads: 564

```
Spot welding them will not allow flexibility on the pack, I wouldn't suggest to spot weld them unless you have a Carbon GT deck, the Bamboo GT flexes and will stress the nickel strip in no time.
```

---
## \#12 Posted by: Smorto Posted at: 2017-07-08T14:44:21.059Z Reads: 562

```
Ahh ok, the wire is to allow for a slightly flexible pack. If I have  rigid deck though, I am fine spot welding them correct?
```

---
## \#13 Posted by: Eboosted Posted at: 2017-07-08T15:39:00.035Z Reads: 566

```
If your deck is 100% rigid I would say it'd be ok, however almost all decks even the rigid ones flex a tiny bit
```

---
## \#14 Posted by: Eboosted Posted at: 2017-07-08T17:58:11.450Z Reads: 571

```
Small video of the heat wrapping

https://youtu.be/NIIaywH3V9w
```

---
## \#15 Posted by: Smorto Posted at: 2017-07-08T18:15:02.011Z Reads: 562

```
Ok , do you have a video of how much your battery flexes?
```

---
## \#16 Posted by: Eboosted Posted at: 2017-07-09T19:30:03.564Z Reads: 567

```
I had to modify the enclosure to add 25mm of lenght in order to make room for the the 10S4P and BMS, I've seen people routing the deck to mount the BMS, but as I didn't have a wood router and I have the ability to make enclosures it was easier to just modify it. 

<img src="/uploads/db1493/original/3X/c/0/c0f222f198e287810b099ad49d39a9fa9f5e2a36.jpg" width="666" height="500">
```

---
## \#17 Posted by: davidbonde Posted at: 2017-10-04T10:13:17.002Z Reads: 537

```
I am preparing to do this myself. Eboosted do you have a diagram for this pack design short of Smorto posted of the other design? Maybe just a drawing on paper :)
```

---
## \#18 Posted by: davidbonde Posted at: 2017-10-07T09:59:18.868Z Reads: 526

```
Found one at endless-sphere:
￼<img src="/uploads/db1493/original/3X/9/a/9aa5e3aa229b9b830053f50a322ff19999ecf23b.jpg" width="690" height="175">
```

---
## \#19 Posted by: Burrito Posted at: 2017-10-10T22:06:25.901Z Reads: 522

```
Great thread! Thank you.
```

---
## \#20 Posted by: aaseb Posted at: 2017-10-20T12:03:05.881Z Reads: 541

```
Hi, I found this topic when searching about how to make your own battery for an evolve board. I want to travel to India with my board but it seems the battery is too big to take in the plane.
My conclusion was that the best option would be to buy cells in India and make another battery there.
Can anyone confirm that this is the right cell?
http://www.ebay.in/itm/3-7V-18650-Li-ion-battery-rechargeable-6-BATTERIES-5800mah-/152749404181?_trksid=p2059707.m48543.l9013
```

---
## \#21 Posted by: b264 Posted at: 2017-10-20T14:45:30.225Z Reads: 526

```
The biggest issue you will have is that for an Evolve board, you MUST use the BMS from the original battery pack or you will be stuck in ECO mode.  Evolve does not sell the BMSs.  If you break it, you'll have a hard time replacing it, if you can at all.  Definitely never discard a broken one.

So are you planning to reuse your original battery when you get back home?  Or just use this new one?  Or make yet another battery when you get home?  That could get expensive.

Also 5800mAh is really high for an 18650 lithium ion cell, which is good.  Also not sure I'd like the karma associated with using cells that say "UltraFire" on them
```

---
## \#22 Posted by: BigBoyToys Posted at: 2017-10-21T05:19:34.025Z Reads: 509

```
Those are flashlight batteries. They will not work for an eboard, they put out less than 1A each, good 18650's are rated at 20A.
```

---
## \#23 Posted by: darkkevind Posted at: 2017-10-21T07:23:24.580Z Reads: 502

```
The largest mah of any genuine 18650 cell right now is less than 4000mah so these ones are almost definitely fake.

Also, you're going to need a minimum of 2 cells in parallel (minimum! 4 preferably),  so factor that in to your cost. Each cell should put out at least 15A, so a minimum of Samsung 30q's should be used. LG HG2's would be better, Sony Konion US18650VTC6's would be better than those...
```

---
## \#24 Posted by: aaseb Posted at: 2017-10-21T10:14:41.421Z Reads: 486

```
yes the idea woud be to take the original battery apart to use the BMS and probably put it back together when I get back since I probably wont be able to fly with the new battery either.
```

---
## \#25 Posted by: aaseb Posted at: 2017-10-21T10:15:47.342Z Reads: 470

```
> Those are flashlight batteries. They will not work for an eboard, they put out less than 1A each, good 18650's are rated at 20A.

how can you tell?
```

---
## \#26 Posted by: scepterr Posted at: 2017-10-21T10:42:42.219Z Reads: 461

```
Seriously dude, Google or YouTube ultrafire
```

---
## \#27 Posted by: aaseb Posted at: 2017-10-21T13:08:50.021Z Reads: 467

```
[quote="darkkevind, post:23, topic:26965"]
Each cell should put out at least 15A
[/quote]

thanks for the tip. Is that the specs of the original battery cells? What would happen if I tried with cells that have maybe only 10A output? Would the board just be slower or would it risk burning the battery or something?
```

---
## \#28 Posted by: darkkevind Posted at: 2017-10-21T13:36:58.811Z Reads: 457

```
I'm not sure what the standard Amp draw rating on the Bamboo GT's stock battery is, but have a higher discharge rate, counteracts voltage sag, which means you can use your GT with full power for longer...

With 4 cells in parallel that can discharge 10A each, you just multiply it so that would be a max continuous discharge of 40A, which, may not be good when you're at 40-50% battery and trying to climb an incline or pull away fast, plus it stresses the battery more and they'll die quicker...
```

---
## \#29 Posted by: aaseb Posted at: 2017-10-22T14:35:47.468Z Reads: 449

```
I found the hg2 lg cells but they're pretty expensive.
I also found samsung 18650 25R which are only 2500mah but are rated 20amps and 30% cheaper
Now this is the cheapest option : samsung ICR18650-22P which are only 2200mah and rated only 10amps max but they are one third of the lg price. Even if the batteries die much faster, it might be worth trying the cheaper option.
```

---
## \#30 Posted by: darkkevind Posted at: 2017-10-22T14:54:54.212Z Reads: 451

```
Samsung 30q are probably your best option.
```

---
## \#31 Posted by: aaseb Posted at: 2017-10-22T14:58:05.002Z Reads: 434

```
I thought the LG ones were better. they are 1000rupees each
I think the samsung 30Q are above 1300
```

---
## \#32 Posted by: darkkevind Posted at: 2017-10-22T15:27:14.049Z Reads: 437

```
Well I was saying, if the LG are too expensive go with the 30q's...
```

---
## \#33 Posted by: darkkevind Posted at: 2017-10-22T16:17:23.971Z Reads: 434

```
I just put this up in the other thread about evolve battery upgrades...

If anybody needs this done in the UK I can help with the battery pack upgrade... I've just completed two and I have the correct Evolve-specific 11 pin connector for the BMS.

Pm me for more info...
```

---
## \#34 Posted by: esk8jpn Posted at: 2017-10-23T04:19:23.138Z Reads: 429

```
Hi @Eboosted

Thanks for sharing.

I think that 10S4P and BMS will not fit in the EVOLVE genuine enclosure. Even if you look at your photos, the enclosure looks as if nothing has changed.
Where did you change it?
```

---
## \#35 Posted by: Eboosted Posted at: 2017-10-23T05:26:46.378Z Reads: 421

```
Yes, the BMS won't fit a 10s4p,you need to cut the enclosure and make a fiberglass extension, otherwise you will need to use a router on the deck in order to make space for the BMS.
```

---
## \#36 Posted by: scepterr Posted at: 2017-10-23T05:42:41.677Z Reads: 441

```
Have any of you guys looked at the LG MJ1? I'm building a 14S10P split triangle ebike pack for a client with the them. 
https://www.imrbatteries.com/lg-mj1-18650-3500mah-10a-flat-top-battery/
<img src="/uploads/db1493/original/3X/1/f/1f31e2241c53a2bf538b8507344860944b2b9054.jpg" width="590" height="500">
```

---
## \#37 Posted by: Froxx Posted at: 2017-11-11T08:20:25.322Z Reads: 423

```
Hi guys, just finished a 10s4p myself, worked flawlessly. 
Assembled the cells like eboosted and lhb did. 

However after wiring everything, the board doesn’t switch on. No blinking switch, attaching the charger doesn’t work too. Charger LED stays green. 

Pack has 36V, also at B- at the BMS. P- at BMS showing 31V. 

Don’t know how to troubleshoot further, what connections to check etc. 
Any help would be much appreciated!

Thanks!
```

---
## \#38 Posted by: SkaterBoy58 Posted at: 2017-11-11T08:22:59.576Z Reads: 414

```
Can you draw a diagram showing connections? 
I have completed a similar mod to yourself with no problems
Cheers
```

---
## \#39 Posted by: Froxx Posted at: 2017-11-11T08:43:16.470Z Reads: 411

```
CWired the BMS cables according to this diagram from another build I found. Second pic shows the main cables.

Image deleted
```

---
## \#40 Posted by: Froxx Posted at: 2017-11-11T08:43:59.691Z Reads: 414

```
image deleted
```

---
## \#41 Posted by: Froxx Posted at: 2017-11-11T11:16:20.891Z Reads: 382

```
Shame on me! One balance cable was bad ... All good now!
```

---
## \#42 Posted by: SkaterBoy58 Posted at: 2017-11-11T11:24:28.371Z Reads: 390

```
No worries
Wiring all looks fine
The origin of the balance wiring diagram is a local here in Perth (Nick)
Cheers
```

---
## \#43 Posted by: khaotic Posted at: 2017-11-12T04:14:48.329Z Reads: 380

```
Where do you guys source your 30q's from in Aus?  And is there anyone here down under who is offering a similar service to Kevin or LHB?  I would do it myself but I don't have access to a tack welder.
```

---
## \#44 Posted by: ElskerShadow Posted at: 2017-11-13T07:06:43.862Z Reads: 365

```
I think kevin just send you the pack and then you have to solder the BMS andplace the battery yourself.
```

---
## \#45 Posted by: darkkevind Posted at: 2017-11-13T09:10:40.950Z Reads: 370

```
This is back to front! Please remove this diagram just in case someone else sees it and doesn't see that it's the wrong wiring diagram and fries their BMS! (Y)
```

---
## \#46 Posted by: darkkevind Posted at: 2017-11-13T09:11:24.585Z Reads: 364

```
Either that or a rubber 6mm gasket ;)
```

---
## \#47 Posted by: BelviGER Posted at: 2017-11-16T15:19:27.922Z Reads: 360

```
Could you tell me where the red wire goes?

My bms is currently not showing 10 cells and that red wire that goes to the bottom corner of the board is the one that's missing
```

---
## \#48 Posted by: longhairedboy Posted at: 2017-11-16T18:07:45.446Z Reads: 358

```
red wires go to cell pack main positve. there may be two or three red wires runnign back there depending on which batch your board came from. There's always one red balance lead, that goes to main positive. then there is the charge lead from the tiny red connector, that red wirte goes to the pack positive also. Then sometimes there is a third red wire coming from the BMS which also goes to pack positive. 

All of those wire independently go all the way to pack positive.
```

---
## \#49 Posted by: BelviGER Posted at: 2017-11-16T18:20:07.381Z Reads: 359

```
Thank you, will communicate that to my guy

And I misspoke, 4 of the cells aren't showing up when measuring at the BMS, so we are 3.7 volts low.
This is on a brand new bms

When using an old BMS that has some water damage and has problems with the data connection etc we still get the full voltage though

Very very weird
```

---
## \#50 Posted by: davidbonde Posted at: 2017-11-19T18:49:47.373Z Reads: 341

```
I am ready to put everything back together. I have made a new pack and done the board modification (bamboo GT). Do you guys use any kind of foam/neopren around the pack or between the board and pack, to take some of the vibration? Or is it not necessary?
```

---
## \#51 Posted by: Eboosted Posted at: 2017-11-20T04:03:29.491Z Reads: 346

```
Use 3M double sided tape to stick the battery to the enclosure, I'll make you life easier when putting everything back together and I'll help with vibrations
```

---
## \#52 Posted by: davidbonde Posted at: 2017-11-21T13:56:36.296Z Reads: 379

```
I have just finished doing this upgrade my self. Mainly because when I started looking in to this only LHB were just starting to offer this service. Normally I would have paid for this kind of work as I have no experience, and are in general not very good with my hands. But being on the other side of the pond from LHB, I decided to learn how to do it my self. I have spend countless hours reading, looking at pictures, and asking a questions or two now and then. I have enjoyed it! I have mainly been getting my info from these resources:

https://endless-sphere.com/forums/viewtopic.php?f=35&t=70435
https://evolveforums.com/threads/how-i-built-a-12ah-battery-for-my-bgt.1091/#post-8484 
http://www.electric-skateboard.builders/t/evolve-bamboo-gt-battery-upgrade/23706
https://endless-sphere.com/forums/viewtopic.php?f=35&t=72026
https://endless-sphere.com/forums/viewtopic.php?f=35&t=70435&start=75#p1166305

Videos: 
https://www.youtube.com/channel/UCRMrqzsrPIWvY3PINkLKs-Q/playlists

Book:
https://www.amazon.co.uk/DIY-Lithium-Batteries-Build-Battery/dp/0989906701/ref=sr_1_1?ie=UTF8&qid=1511269524&sr=8-1&keywords=how+to+build+battery

It is not the most beautiful pack out there, but it seems solid and safe enough. Let me know if you see it differently 

I have learned a great deal, and my craftsmanship getting better and better for every glueing, spot weld, solder and handling of tools I have done. So next time it will be more beautiful - but there will likely not be a next time :) But I enjoyed the journey, and think I will do other e-skate building stuff in the future. I have already some in mind and lined up. 

I have done one thing a little different than from others. The jumpers in serial between P-groupes are made longer to take away some of the stress on the wire/solderjoint when the pack flexes. But that became a small issue when trying to fit everything back together, because of extra width nearly all over. 

Battery glued in fours, and nickel prepared with solder.

<img src="/uploads/db1493/original/3X/0/1/01644e3d2a2834aa2aff851691de32890f5fb78e.JPG" width="666" height="500">

Nickel spot welded. 

<img src="/uploads/db1493/original/3X/7/3/7307ec975dadc0c857aa059033ac6ca08da9b820.JPG" width="666" height="500">

Jumpers soldered. longer jumpers to take away some of the stress. 

<img src="/uploads/db1493/original/3X/5/c/5ccc588415f9f6cfc7b106b6958d04f6210db693.JPG" width="666" height="500">

Balance wires attached. 

<img src="/uploads/db1493/original/3X/7/6/7664aa422459235fb7dd810ec54b17f4b6d3c9e5.JPG" width="666" height="500">

Taping up for insulation.

<img src="/uploads/db1493/original/3X/c/7/c7be56fa1e3f775910060040e4f88ba5594916bf.JPG" width="375" height="500">

Connecting the balance wires to the bms. 

<img src="/uploads/db1493/original/3X/1/6/16a6156cb22a96043ac6553fa75612901dbbb06c.JPG" width="666" height="500">

Heat shrink everything.

<img src="/uploads/db1493/original/3X/1/d/1d50e01e3312f7ca66060baebacc5b97deda0d4c.JPG" width="375" height="500">

Routing the deck with a hand router. This took way longer than expected, but I only missed up twice, and nothing seriously.

<img src="/uploads/db1493/original/3X/2/4/240cd80c45ea9325ed3c75dd91f77b7b9598a358.JPG" width="375" height="500">

Ready to be turned around.

<img src="/uploads/db1493/original/3X/1/8/1809b4d7b72a3d61232671b995ca21d99c6e1f6e.JPG" width="375" height="500">

Done.

<img src="/uploads/db1493/original/3X/1/2/125dc0cd4bb8df7a9e528b08c07dda9bb52b2195.JPG" width="375" height="500">

And it actually works!I Just a same that it is freezing here right now and that spring seems far way.  Will check in on the battery regularly, to see if everything holds up.
```

---
## \#53 Posted by: longhairedboy Posted at: 2017-11-21T14:15:01.480Z Reads: 337

```
[quote="BelviGER, post:49, topic:26965"]
When using an old BMS that has some water damage and has problems with the data connection etc we still get the full voltage though

Very very weird
[/quote]

I've been in plenty of situations where the voltage readings just lie about available power. 

Depending on what's actually happening, you can occasionally read a correct voltage then lose it all when the potential collapses as a load is placed on the pack. Its weird, but its all voltage and hardly any current to back it up in those cases. I suspect blown components are responsible. Shits broke, that's my professional assessment. lol
```

---
## \#54 Posted by: BelviGER Posted at: 2017-11-21T14:30:41.375Z Reads: 332

```
Haha okay

I've talked to the guy who does 18650 packs in the UK and he thought that it might be a balance wire or the terminal for the balance wire that is a bit fucked

Honestly if the pack works otherwise flawlessly, even at 9s, I don't think I care thaaaat much.

As long as the bms allows more than eco mode im probably happy, though my battery guy isn't, haha.

He would like to offer the service to everybody in Germany but obviously won't if the only experience he had was that shit is fucked.
```

---
## \#55 Posted by: longhairedboy Posted at: 2017-11-21T14:37:33.092Z Reads: 326

```
a thin or burned out wire can definitely behave in the way we're discussing. I cooked a balance lead and didn't know it and couldn't figure out the weirdness for a long time. Replacing a section of wire was all it took, but damn did it take me forever to figure that shit out when the old volt meter was telling me things that may or may not be true.
```

---
## \#56 Posted by: davidbonde Posted at: 2017-11-21T16:10:25.783Z Reads: 326

```
Does anyone know the low voltage cut off on the BGT? I know I have seen it somewhere in the tons of posts I have been reading, but can't remember where. Maybe some of you know the number?
```

---
## \#57 Posted by: Bowski Posted at: 2017-12-18T16:00:20.871Z Reads: 321

```
Hi Everybody,

I am offering this service in Germany now. We are doing 10S4P for Bamboo GT and also 10S5P for Carbon GT.

If you are interested please sent a PM or contact me via WhatsApp 015120940064
```

---
## \#58 Posted by: b264 Posted at: 2017-12-18T18:22:40.324Z Reads: 314

```
How are you doing the 10S5P?  Curious because the only reason I haven't had my CarbonGT upgraded yet is because I wanted it to be 10S5P

Specifically, where are you putting the BMS
```

---
## \#59 Posted by: mikenyc Posted at: 2017-12-25T14:48:58.712Z Reads: 303

```
I even didn’t think that the CGT could fit 10s5p. Has this been done?
```

---
## \#60 Posted by: Eboosted Posted at: 2017-12-25T15:32:22.194Z Reads: 299

```
I'm not sure but the current limit should still be restricted on the ESC so, I don't know if you could benefit from a higher discharge battery pack unless you program the ESC
```

---
## \#61 Posted by: b264 Posted at: 2017-12-25T17:50:39.355Z Reads: 293

```
[quote="mikenyc, post:59, topic:26965, full:true"]
I even didn’t think that the CGT could fit 10s5p. Has this been done?
[/quote]

@Fiori [fit 10S5P](https://www.electric-skateboard.builders/t/custom-evolve-carbon-gt-10s5p-battery-build/34045) in a CarbonGT.  Well, almost.  The BMS was mounted above the back trucks
```

---
## \#62 Posted by: Zyb Posted at: 2018-01-17T12:24:22.824Z Reads: 280

```
Thanks for sharing this, I cannot stress how valuable it is to me because I will try to swap every bit of electronics as well as battery inside of my bamboo GT. It was my first ever electric board enjoyed it a lot but it has poor quality battery and a Bms. Range dropped to 7km also sags from %100 to %50ish on hard acceleration, BMS is shot so I thought I might as well swap everything with better quality parts. Going to use 2 focboxes, Samsung 30Qs, custom made remote and supower 60A bms.
```

---
## \#63 Posted by: Eboosted Posted at: 2018-01-17T15:04:06.902Z Reads: 280

```
I couldn't change the BMS on my board, it seems my bms is also shot and evolve won't sell me a BMS on its own, they request to have the board on their facilities to perform any repair service, of course shipping my board to USA or Australia from Perú is no option at all, nearly impossible.

On the other hand if you decide to use a different bms, you will loose the ability to change modes and could be stuck on Eco mode as the BMS is the one that controls the power delivery and speed
```

---
## \#64 Posted by: Zyb Posted at: 2018-01-17T15:15:13.317Z Reads: 282

```
Yes that’s what I’m told about using a different BMS. That is the reason for changing vescs and the remote too. I may change the board, motors and drivetrain etc. in the future aswell but one step at a time that’s gonna be my first build. I wanna see how it goes, I hope I don’t blow anything up :smile: going to use precious information on this topic and the forum aswell. Thanks again for sharing.
```

---
## \#65 Posted by: mikenyc Posted at: 2018-01-17T15:15:37.183Z Reads: 286

```
sounds like you need to swap out all of the electronics.
```

---
## \#66 Posted by: Acido Posted at: 2018-01-17T17:19:36.595Z Reads: 288

```
Get an extra 20$ bestech bms is worth it
```

---
## \#67 Posted by: Zyb Posted at: 2018-01-17T17:22:30.995Z Reads: 295

```
I’m afraid already ordered, gonna try to use this old heatsink salvaged from my old graphics card. I ll see how it goes ![image|375x500](upload://eGIuqZr9NNjokAzstD1qUYVM7ad.jpg)
```

---
## \#68 Posted by: b264 Posted at: 2018-01-17T18:24:32.357Z Reads: 282

```
You need to publicly call-out Evolve on reddit and all social media channels for this.  Their image is more important to them than even their boards and frankly, this is horse shit.

"Evolve won't sell me parts to fix my broken Evolve"
```

---
## \#69 Posted by: Zyb Posted at: 2018-01-27T16:24:02.520Z Reads: 276

```
[quote="Eboosted, post:35, topic:26965, full:true"]
Yes, the BMS won't fit a 10s4p,you need to cut the enclosure and make a fiberglass extension, otherwise you will need to use a router on the deck in order to make space for the BMS.
[/quote]

 can you please elaborate the extension abit more as im at total loss about how to execute this whole process. for example what did you use with the fiberglass? epoxy resin, polyester resin or something else?
```

---
## \#70 Posted by: agent Posted at: 2018-04-05T05:22:37.321Z Reads: 255

```
Hey... I'm from India too.. Do you ride electric skateboards?
```

---
## \#71 Posted by: aaseb Posted at: 2018-04-05T06:40:35.108Z Reads: 260

```
So this is my evolve skateboard adapted Indian style.
If anyone wonders why I did this, I couldn't take the battery in the plane.
It's 3 12v batteries originally used in UPS devices.
I get a bit less range but otherwise works fine.

![IMG_20180405_115612621|281x500](upload://AvdWE0KnjKDCwPBlwvrBv6FAlvt.jpg)
```

---
## \#72 Posted by: aaseb Posted at: 2018-04-05T07:02:39.788Z Reads: 249

```
see my last post...
```

---
## \#73 Posted by: myreala Posted at: 2018-04-05T07:27:30.358Z Reads: 244

```
Damn, those are some heavy ass lead acid batteries. Not a bad setup if its temporary, although putting the batteries in the middle might have been another option.
```

---
## \#74 Posted by: aaseb Posted at: 2018-04-05T07:36:35.342Z Reads: 243

```
I had them in the middle at first and found that having them in the back made it a bit more comfortable.
It is temporary, the nice part is those batteries cost me only around 50 usd.
```

---
## \#75 Posted by: myreala Posted at: 2018-04-05T08:06:26.534Z Reads: 254

```
Nice, thats a good setup. You could have also bought one of those hover-board batteries directly shipped from china to India. Would have cost you about same but equal to size of just one of those.
```

---
## \#76 Posted by: agent Posted at: 2018-04-05T15:26:30.367Z Reads: 263

```
Awesome.. I love the Giant Wheels 8" size(I think).. and where did you get the long Hanger trucks??

Also are you from MUMBAI?

These are My 2 skateboards..
![IMG_0938|690x388](upload://kLSmQJ8ptxuoYl8atCR4s9IohKf.jpg)
This is the Skateboard..
![IMG_6333|665x500](upload://bVRx8qysEhgI3wwaASoBQBLBKJY.jpg)
These are the pics of the Longboard
![IMG_6336|375x500](upload://jdxPmtTOuE8C2uz9zy1Xj1asmOz.jpg)
![IMG_6334|665x500](upload://uye95QXEeSG75ZNq2V3ZSBvz6le.jpg)
![IMG_6494|374x500](upload://bP0pLzeNxDv2zpDiNmQTwBaTQQD.jpg)
![IMG_6335|375x500](upload://4sG2PpQ0tbn9dEwrP9QGFm2CUce.jpg)

Longboard has a 40" deck.. and Skateboard has 31" deck with kicktails.
```

---
## \#77 Posted by: PickSix24 Posted at: 2018-08-29T18:56:46.309Z Reads: 208

```
Does anyone have a good photo or drawing of where the balance leads go on the pack. I’m starting a build soon and that’s the only thing I’m unclear on. Thanks !!
```

---
## \#78 Posted by: esk8jpn Posted at: 2018-08-31T04:23:51.802Z Reads: 211

```
This is what I wrote when Bamboo GT battery modify.
![evolve_BMS|465x500](upload://totAEziBOvqWN2FCFTSWBSzPO7T.PNG)
```

---
## \#79 Posted by: PickSix24 Posted at: 2018-08-31T06:23:09.906Z Reads: 196

```
@esk8jpn thank you ! Exactly what I was looking for
```

---
## \#80 Posted by: blively Posted at: 2018-09-09T19:58:02.643Z Reads: 189

```
Hey Esk8jpn. Is your diagram correct? Shouldn't the balance leads be reversed? #10 should be #1, right?
```

---
## \#81 Posted by: esk8jpn Posted at: 2018-09-10T00:49:08.781Z Reads: 192

```
Aside from the wire number I gave, I think wire color and connection point are correct.

I made a 10S4P battery pack with LG HG2 works perfectly on my Bamboo GT.
![20180204_112209|238x500](upload://4qw88DyXtTWQ2HT20kPnCG5vXnk.jpg)
```

---
## \#82 Posted by: PickSix24 Posted at: 2018-09-10T02:09:57.621Z Reads: 190

```
Yep 👍🏻 worked for me. Just finished and tested my battery today.
```

---
## \#83 Posted by: esk8jpn Posted at: 2018-09-10T05:05:10.559Z Reads: 188

```
Congrats :tada:
```

---
## \#84 Posted by: blively Posted at: 2018-09-14T01:59:06.052Z Reads: 182

```
What thickness nickel strip are you guys using? And do you double it up on the series connections?
```

---
## \#85 Posted by: Eboosted Posted at: 2018-09-14T06:20:38.405Z Reads: 183

```
I use 12awg wire between p-groups, nickel strips won't cut it
```

---
## \#86 Posted by: blively Posted at: 2018-09-14T10:48:34.801Z Reads: 183

```
12gauge wire to make the flexible series connections but when you put two parallel groups in series you’re using nickel. What thickness nickel on those connections? Thanks
```

---
## \#87 Posted by: esk8jpn Posted at: 2018-09-14T11:16:24.345Z Reads: 177

```
I'm using 0.15mm thickness.
```

---
## \#88 Posted by: Eboosted Posted at: 2018-09-14T22:34:37.734Z Reads: 184

```
I use only one pure nickel strip 0.15mm
```

---
## \#89 Posted by: Marsen Posted at: 2018-09-14T23:36:38.808Z Reads: 185

```
0.2mm x 10mm single in positions 2, 4, 6, 8 and 10 and double in positions 1,3,5,7,9 and 11 with 4mm2 tinned flat copper braided wire for main series outer connections.![Braid|690x422](upload://fdLXFxT4f50ktBskkszU5NzWRCK.jpg)
```

---
## \#90 Posted by: Schulerbible Posted at: 2018-09-15T01:31:28.922Z Reads: 185

```
You are sure that’s enough?
```

---
## \#91 Posted by: Eboosted Posted at: 2018-09-15T02:22:21.629Z Reads: 185

```
I've been riding my board for so long at so much current, I never had issues with batteries disbalancing or a bottleneck on power, I know the P-Groups connections carry a lot more current, that's why I use silicone wire there
```

---
## \#92 Posted by: Wizeartz Posted at: 2019-02-28T00:34:46.799Z Reads: 148

```
Hey, I'm going to try tack up my own pack too, would you sell me the "specific 11 pin connector" for the BMS you refer to please and thank you? 
I'm in New Zealand, one of your colonies on the opposite side of the planet ;)
Cheers, Owen
```

---
## \#93 Posted by: Wizeartz Posted at: 2019-03-20T00:47:30.111Z Reads: 135

```
Hey guys, I'm about to follow this extremely useful guide to do my own pack, but a lot of the images are missing. Any chance of relinking them up?
What nickel strip thickness do you recommend, and what AWG rating for the link between each 4p?
Thanks very much, really looking forward to GT'ing my way to work without having to fumbling the mode back out of ECO every time I slow down. Tedious!!!!!
```

---
## \#94 Posted by: Eboosted Posted at: 2019-03-20T04:37:36.150Z Reads: 135

```
Use 99.7% pure nickel strip 0.15x8mm

Use 2 x 16awg between each pack or one 12awg
```

---
## \#95 Posted by: drone001 Posted at: 2019-03-22T01:02:09.914Z Reads: 130

```
the balance wires between packs 1 and 2 .... 3 and 4. what pack should you solder to?
```

---
## \#96 Posted by: esk8jpn Posted at: 2019-03-22T02:08:23.994Z Reads: 138

```
Hi @drone001

This thread contains the necessary information. You can go back a little, and read.
https://www.electric-skateboard.builders/t/upgrading-an-evolve-gt-battery-with-18650-lithium-ion-batteries/26965/81?u=esk8jpn
Good luck!
```

---
## \#97 Posted by: drone001 Posted at: 2019-03-22T02:31:37.225Z Reads: 137

```
beautiful...thx i needed this.
```

---
## \#98 Posted by: Wizeartz Posted at: 2019-04-17T09:59:13.034Z Reads: 140

```
![image|375x500](upload://g99NMscAsgVIodWtjx7Np8dBglq.jpeg) 
I’m trying to be a smart arse and put in an XT90 in line in case I want to swap out to another pack. I plugged it in an hit the power button and NOTHING! Does the BMS 11 pin need to be plugged in too, or have I wired this puppy wrong gents?
```

---
## \#99 Posted by: Wizeartz Posted at: 2019-04-17T23:05:17.305Z Reads: 140

```
Have I got THIS right LHB?![image|638x309](upload://4Zv0yl1waGbjJQTqfCeTgDaHg82.png)
```

---
## \#100 Posted by: Eboosted Posted at: 2019-04-18T01:03:39.365Z Reads: 140

```
Another successful Evolve upgrade. 

Working on a new enclosure for the Evolve Bamboo GT to upgrade the battery from a 10s4p to 10s5p

![20190412_103517|281x500](upload://i51xkp0osazBkYi8Euh2bRYfWPw.jpeg)
```

---
## \#101 Posted by: Bataleon Posted at: 2019-04-18T14:13:02.202Z Reads: 135

```
Looks really neat. What is battery voltage sag like at the moment with 10s4p?
```

---
## \#102 Posted by: Jaydawg56 Posted at: 2019-04-18T15:52:37.752Z Reads: 134

```
Did you mold in the end cap?  Looks like a 10S4P, but the placement of the BMS suggests that the tray was extended
```

---
## \#103 Posted by: Eboosted Posted at: 2019-04-19T00:03:49.363Z Reads: 137

```
You have a great eye my friend, yes the Evolve enclosure was extended, you can't notice it was extended though.

I'm making a custom enclosure designed for Evolve so you can mount the battery without the need of modifying the enclosure
```

---
## \#104 Posted by: Wizeartz Posted at: 2019-04-21T20:01:34.091Z Reads: 140

```
Thanks for your guidance! I made my 10S4P pack and it gave me hideous sag still, and only about 4km’s range. Suspect efest 3000mAh cells aren’t quite what I paid for, or I’ve wired something up wrong!!! Have I got this right?  ![image|638x309](upload://4Zv0yl1waGbjJQTqfCeTgDaHg82.png)
```

---
## \#105 Posted by: Jaydawg56 Posted at: 2019-04-21T20:09:49.415Z Reads: 133

```
Details? What batteries? Where’d you get them?
```

---
## \#106 Posted by: Wizeartz Posted at: 2019-04-21T23:45:53.266Z Reads: 140

```
https://captainvapour.co.nz/efest-18650-nz-3000mah-20a-battery/
used .15mm 8mm nickel strips, tacked LHB style, with 12awg silicone between P groups, and main positive/negative. ![image|375x500](upload://frC4BnqHQ1G2LWIV1zNfpZHJMMO.jpeg) ![image|375x500](upload://hLeUn5hr8ID00fyby6PaCAFOhBt.jpeg) ![image|375x500](upload://aaTWmLzucgRNaIq0BA8QnVMFeeV.jpeg) ![image|375x500](upload://kc2MqFfD3gUUSxWdfvOzCkO2rCh.jpeg)
```

---
## \#107 Posted by: Schulerbible Posted at: 2019-04-22T01:22:00.086Z Reads: 130

```
Sharp corners, no fishpaper, and fucked up welds are things that have been pointed out before .... many times. 😞
```

---
## \#108 Posted by: Wizeartz Posted at: 2019-04-22T06:57:09.421Z Reads: 135

```
Thanks for the feedback! Welds seem solid, three tacks per end of each cell. Sharp corners, sure, no insulating rings either, a fairly noob oversight, but then I AM a noob, but whilst those items risk a short, they wouldn’t restrict current would they? Can’t seem to get the R2 to show me individual voltage per P group ![image|375x500](upload://7noFbffH3UyWkpTdagrhC92u4gD.jpeg)
```

---
## \#109 Posted by: Jaydawg56 Posted at: 2019-04-22T08:07:29.160Z Reads: 133

```
It’s been a while since I used that remote, but once you get to that screen hold the top button (of the two) and double click the menu button. The posted video by evolve actually is incorrect on how to get to the individual p-group voltage screen. 

But yea, if your board works and noon battery building mistakes aside it might be the quality of cells. I say this because the first time I incorrectly hooked up the BMS air gave me a battery error and couldn’t even use the board. 

Let me know if it doesn’t work, I’ll be home later today.
```

---
## \#110 Posted by: Wizeartz Posted at: 2019-04-22T08:26:30.839Z Reads: 128

```
Hey Damon, why independently may I ask? 
Cheers, Owen
```

---
## \#111 Posted by: Wizeartz Posted at: 2019-04-22T08:46:43.839Z Reads: 134

```
Thanks Jaydawg, I got the bastard R2 to work, thanks man, brilliant. Interesting results... 
![image|375x500](upload://rZPUNv6Oqab7HKCHgFBcxvHcrEX.jpeg) 
Noticed the stock charger won’t go red for very long, and I’d of expected it to charge higher than just 37 volts. My stock sad-sacks factory pack shows 42. At least the bms is reading each P group I suppose!
```

---
## \#112 Posted by: Andy87 Posted at: 2019-04-22T08:56:24.561Z Reads: 127

```
Man sorry to say, but your pack looks super sketchy. Especially as you did this fold method you risk that the corners of your nickel can hit the isolation and short out your whole pack.

I have no experience with the evolve remote, but if it shows the individual p group voltage than your battery pack seems pretty out of balance and your bms will not be able to get that back in normal ranges.


Edit: did you as min check if all cells have the same voltage before you started to put them together?
```

---
## \#113 Posted by: Wizeartz Posted at: 2019-04-22T09:19:13.748Z Reads: 122

```
Hi Andy, thanks for your time. I followed several other build threads and I don’t recall any testing them first, probably didn’t need mentioning, common sense in retrospect! Is there a way I can balance them by desoldering the 12AWG links between the P groups and charging them up separately do you think? 
Thanks, Owen
```

---
## \#114 Posted by: Andy87 Posted at: 2019-04-22T10:23:15.504Z Reads: 130

```
You can charge the individual packs with a 4.2v power supply. You don’t need to unsolder anything, just connect the power supply right. Have a look here in the forum, there are others having the same problem. I can’t say exactly but there should be a 5v step down module you can use for it and than just connect that to a usb power supply on the one end and the other to the plus and minus of each p pack one by one
```

---
## \#115 Posted by: Jaydawg56 Posted at: 2019-04-22T11:30:18.189Z Reads: 127

```
Yep, what Andy said. You can balance the pgroups (or drain the others) whichever ends up being less work, haha.  You can charge the individual groups through the balance wires so no need to de-solder anything.  If you have a regular li-ion charger you can rig that.
```

---
## \#116 Posted by: taz Posted at: 2019-04-22T13:04:49.655Z Reads: 128

```
Do any of you guys know if the Evolve GT charge plug is a 5.5x2.1mm or 5.5x2.5mm?
```

---
## \#117 Posted by: Wizeartz Posted at: 2019-04-22T20:00:06.636Z Reads: 129

```
I don’t, but can check when I get home Taz
```

---
## \#118 Posted by: Wizeartz Posted at: 2019-04-22T20:00:24.944Z Reads: 133

```
Thanks Jaydawg!!!!
```

---
## \#119 Posted by: Wizeartz Posted at: 2019-04-22T20:08:58.415Z Reads: 134

```
Thanks Andy, I might be able to use the charger on my spot welder. I guess the BMS sees the imbalance and gives up, hence it not charging fully right? Thanks so much for your help, and Jaydawg!
```

---
## \#120 Posted by: Andy87 Posted at: 2019-04-22T20:42:30.842Z Reads: 134

```
Jap that’s probably the issue. Good luck!
```

---
## \#121 Posted by: Eboosted Posted at: 2019-04-23T02:21:40.232Z Reads: 135

```
[quote="Wizeartz, post:119, topic:26965"]
I guess the BMS sees the imbalance and gives up, hence it not charging fully right?
[/quote]

As soon as the highest p-groups reaches 4.2v it will stop charging to avoid overcharge, all other pgroups will be lower and won't reach 4.2V
```

---
## \#122 Posted by: Wizeartz Posted at: 2019-04-23T02:47:25.923Z Reads: 140

```
Thank you Eboosted! I'll charge/drain and get them within range of each other and give it another go. I'd hoped it'd be like my EV, and once peak was achieved spend time balancing the other packs to a similar level. Evolve needs to Evolve I guess ;)
```

---
## \#123 Posted by: dtaoo Posted at: 2019-04-23T06:50:31.184Z Reads: 135

```
How many layers of nickel strips you used for each group of series? Also, I’m thinking of doing a double flat stack 10s4p build with 20 cells on the bottom and 20 on the top. Somewhat is following the diagram as a guide. What do you guys think?![jpg|690x175](upload://m44WGZfavfbXcl5qtFTetiKQSJZ.jpg)
```

---
## \#124 Posted by: min Posted at: 2019-04-23T07:02:35.696Z Reads: 129

```
Thanks for sharing, Dude, so clear!
```

---
## \#125 Posted by: Wizeartz Posted at: 2019-04-23T08:05:48.054Z Reads: 131

```
Burn, baby burn!![image|375x500](upload://zONK25mgNmIrJOfMMhxi22MzJU9.jpeg)
```

---
## \#126 Posted by: Wizeartz Posted at: 2019-04-23T08:18:25.915Z Reads: 128

```
Hmmmmmm, slow...
```

---
## \#127 Posted by: davidbonde Posted at: 2019-04-23T11:01:55.430Z Reads: 127

```
I am using one layer of 10mmX0.15mm.
You should be able to stack them no problem.
```

---
## \#128 Posted by: never4getf150forums Posted at: 2019-04-23T11:06:52.036Z Reads: 128

```
2.5 my good sir
```

---
## \#129 Posted by: never4getf150forums Posted at: 2019-04-23T11:15:59.300Z Reads: 130

```
you might be able to charge this easily by unplugging the p's with different cell capacity.

for example.

unplug all except c3 + c5, let that charge up to full.

then unplug them all and plug in c2, c6, c9 , let that charge up to full.

then unplug all again, and plug in c4, c8, cA, let that charge up to full.

then plug in c1, let it charge, then c7 last.

make sure you do this with a 2a slow charger, not the 4a just to be on the safe side.
```

---
## \#130 Posted by: Jaydawg56 Posted at: 2019-04-23T11:31:47.151Z Reads: 130

```
@Wizeartz
 
Yea man, it’s a slow process. I forget sometimes you are draining a 4 or 5 in parallel when I get impatient. 

But is exactly how I did it (used a super resistor myself), balanced the 2 packs I was after, then charged the whole battery to get it where I wanted.
```

---
## \#131 Posted by: Wizeartz Posted at: 2019-04-23T19:21:47.838Z Reads: 124

```
Thanks man, that's a great idea!
```

---
## \#132 Posted by: taz Posted at: 2019-04-23T19:25:02.143Z Reads: 130

```
Are you sure?

I just measured the plug on my friend's Evolve charger with calipers and it was 2.1mm (the calipers read 2.0mm)
```

---
## \#133 Posted by: Wizeartz Posted at: 2019-04-23T19:26:46.630Z Reads: 135

```
Thanks Jaydawg, I might try using my old accucel charger and go up, instead of down. Being an EV convert I struggle to find anything but efficient shit laying around to burn energy on!
Hopefully after all this it all just works, and I'll have a good balanced pack to fly with. I'm building another pack too using VTC6 cells from Aliexpress. They all appear to be 3.9v +/- .1v  . Will use insulators I laser-cut this time too![image|375x500](upload://naixKfwje1OeILY7VYVrvGcJaeE.jpeg)
```

---
## \#134 Posted by: Jaydawg56 Posted at: 2019-04-23T19:39:32.208Z Reads: 133

```
Nice.  You are quick to pick up on the good ideas dropped here by others (experienced builders), I’ve learned from them too.  My first pack is for the carbon GT and the second is different in design for my GTX. Im a big fan of using PCBs ![image|375x500](upload://huaAYI53I8kfj8P6fb2f42L9MbT.jpeg)
```

---
## \#135 Posted by: Jaydawg56 Posted at: 2019-04-23T19:39:53.079Z Reads: 134

```
![image|375x500](upload://aJ18FtwnL4GYKCInPiQDzwXT0Yg.jpeg)
```

---
## \#136 Posted by: Wizeartz Posted at: 2019-04-23T19:58:08.580Z Reads: 132

```
Wow! That’s tidy! Your balance tabs look amazing, what have you done there, far less prone to piercing wrap/insulation than my nickel poking up at the butterfly folds!
```

---
## \#137 Posted by: Wizeartz Posted at: 2019-04-23T21:22:09.479Z Reads: 132

```
Outrageous, they LOOK like prismatic pouches, far tidier than even Evolve's factory stuff.
Love the "Positive Bus" etc. This isn't just another level, this is another planet mate, how in the heck...
```

---
## \#138 Posted by: Jaydawg56 Posted at: 2019-04-24T00:24:10.138Z Reads: 130

```
Thanks.  Next round I’ll probably use fuse wire/nickel for cell leveling fusing.  But the pcbs are pretty cheap (about $1 each) and minimizes any additional heat caused by the solder iron. On top I have tinned braided flat copper wire to make it a flexible pack. 

The PCBs  provide rigidity to each parallel pack and keeps the stress off the welds. Wrapped the pack in fish paper for added isolation 

![image|375x500](upload://tLdFlOxZAj3PwxvAngtaCH65fyy.jpeg)
```

---
## \#139 Posted by: Wizeartz Posted at: 2019-04-24T00:55:30.017Z Reads: 128

```
So slick and simple. I'd love to try it myself! Can you send me the link to the braid, fishpaper and pcbs pretty please? I didn't realise you could tack weld directly onto the pcb track.
I was just looking at see if I could design a PCB with the 11 BMS tracks incorporated into the board too. Escalated into something too complex, too quickly!!!!
```

---
## \#140 Posted by: M.Hboards Posted at: 2019-04-24T02:20:18.160Z Reads: 132

```
[quote="Wizeartz, post:139, topic:26965"]
I didn’t realise you could tack weld directly onto the pcb track.
[/quote]
You could but as @thisguyhere has pointed out to me and i have tested myself the copper layer on the pcb is very thin and a very slight pull on the tacked-on nickel will pull up the copper on the PCB therefore i tacked my nickel down and then covered it in solder like in the pics below.

![0331191655|690x328](upload://mk3eLPX8Lh8gXrM0xcEXqra2ghG.jpeg) 
![0331191701|690x328](upload://9jDIwaB9nJ4Ah6MvdAXzkVL3i4N.jpeg)
```

---
## \#141 Posted by: Wizeartz Posted at: 2019-04-24T03:00:26.345Z Reads: 133

```
That's awesome, thanks M.Hboards! Where does one get the PCB's from, Google ain't helping me find a store. Interested in seeing what braid you guys are using too. Brilliant stuff, tidy, my OCD is at peace looking at this eSK8 porn!
```

---
## \#142 Posted by: M.Hboards Posted at: 2019-04-24T03:08:27.692Z Reads: 132

```
@thisguyhere sells the pcb and nickle (and braid if you ask) that's where i got mine from. However you could get everything from China ( even the pcbs which are open source thanks to @akhlut) if your not in a rush but in my case i really wanted to finish my build quick so i ordered my pcbs, nickel and braid from @thisguyhere.
```

---
## \#143 Posted by: M.Hboards Posted at: 2019-04-24T03:11:53.931Z Reads: 135

```
If you want to see more of my battery build look here- 
https://www.electric-skateboard.builders/t/no-words-just-pictures-delete-words-2/88821/71?u=m.hboards
```

---
## \#145 Posted by: Jaydawg56 Posted at: 2019-04-25T20:43:10.742Z Reads: 138

```
Didn’t see your response, but it looks like mhboards hooked you up with the info!

Just finished my battery swap for the GTX. Gotta reassemble but that the easy and fun part, haha. 

![image|374x500](upload://gpQSthIzNbmAkLeAkNYX2pA8OMB.jpeg)
```

---
## \#146 Posted by: Wizeartz Posted at: 2019-04-25T20:57:44.599Z Reads: 132

```
Sorted everything I think JD, except the PCB’s. I see Esk8 life sells the 3p and 5p alternatives, but not the 4p :( 
That BMS wiring (yellow) is nothing short of art dude!
```

---
## \#148 Posted by: Jaydawg56 Posted at: 2019-04-25T22:12:05.426Z Reads: 132

```
Thanks.  

So another place that sells the boards (but everything included in the kit including sized nickel strips) is kaly.nyc.  A little pricey but it is a complete kit to build batteries.  Check them out as well
```

---
## \#150 Posted by: Wizeartz Posted at: 2019-04-28T20:01:49.582Z Reads: 132

```
Tried getting the boards from the same supplier thisguyhere uses, but the robot came back with this message when I uploaded the Gerber file:
![image|599x136](upload://9UOmUQRfeYbQSBZtAs7fxs5hdyn.png) 
I'm going to try to get them to FIX it manually as I've no idea how to edit the gerber file.
I used to have a CNC machine that I milled PCB with, wish I'd kept it now!
```

---
## \#151 Posted by: Wizeartz Posted at: 2019-05-01T09:04:30.812Z Reads: 122

```
Boards ordered, Peter Pan (actual name) will send me the updated gerber file when it’s done so I can share it for next time!
```

---
## \#152 Posted by: Wizeartz Posted at: 2019-05-04T23:31:00.726Z Reads: 116

```
Thanks man, but just to be sure before I overcharge C7. The board charges through the bms wires, not just measuring through them? Why can’t it balance automatically then? I thought it charged through the main pos/negative and only used the bms wires to stop charging when any pack reached 4.2v (In this case C7)
```

---
## \#153 Posted by: never4getf150forums Posted at: 2019-05-08T08:06:36.520Z Reads: 117

```
because once one pack reaches 4.2 the charging is stopped.. which is why you have to do them in groups.
```

---
## \#154 Posted by: Wizeartz Posted at: 2019-05-09T10:11:16.288Z Reads: 119

```
I only just noticed your cunning battery layout! Instead of the LHB layout, you’re running your series links along five packs, then up one, and back again. So no massively long positive feed. Genius! Wondering though, it’d be way faster to weld one 30mm wide strip of nickel along the top and bottom of each pack, bent over and tacked onto the PCB than having to cut 80 pieces of 8mm wide strip eh? Any disadvantages you think? ![image|375x500](upload://pL8Z2hDKe8vEXlDZiMuEMpssNrW.jpeg)
```

---
## \#155 Posted by: M.Hboards Posted at: 2019-05-09T17:41:32.751Z Reads: 115

```
You talking about useing the type of Nickel in the pic below? If yes I don't see any reason why it wouldn't work.

![Screenshot_2019-05-09-13-39-40~2|588x500](upload://53CAMiUDXNjjavWeOAji5niF1G6.jpeg)
```

---
## \#156 Posted by: Eboosted Posted at: 2019-05-09T22:29:19.962Z Reads: 103

```
I use that one also!
```

---
## \#157 Posted by: M.Hboards Posted at: 2019-05-09T22:32:30.992Z Reads: 101

```
@Wizeartz just make sure you get pure nickle from a reliable source.
```

---
## \#158 Posted by: Jaydawg56 Posted at: 2019-05-10T02:56:33.151Z Reads: 97

```
@Wizeartz, have any extra 4P boards? Might need to do another 10S4p real quick
```

---
## \#159 Posted by: Wizeartz Posted at: 2019-05-10T07:18:05.746Z Reads: 101

```
Hey dude, I just happen to have bought ten extra ! I’ll send them your way if you send them back when you do another order/ stock up? wizeartz@gmail.com
```

---
## \#160 Posted by: Jaydawg56 Posted at: 2019-05-10T15:16:26.162Z Reads: 99

```
Thanks for the offer, I think* thisguyhere has a few in stock so I can go that route. But, I appreciate the offer!
```

---
## \#161 Posted by: Nandox7 Posted at: 2019-05-18T21:52:50.008Z Reads: 98

```
That is beautiful!

Does it fit the GTX enclosure without any modification?
```

---
## \#162 Posted by: Jaydawg56 Posted at: 2019-05-19T00:03:20.570Z Reads: 97

```
Thanks.  But no, not entirely. 10S4P is too long so you have to stack the BMS on top of the esc.  To do that you have to route out a pocket in the wood so it’ll fit.
```

---
## \#163 Posted by: Wizeartz Posted at: 2019-05-19T20:04:04.569Z Reads: 97

```
Hey JD, I've got my nickel, and I've started tacking up the packs using 80 current, and 2 pulses on my Sunkko 788H, but when I tack onto the PCB it blows a small hole through the nickel and I can smell it's burnt. Do you wind the current back for tacking the Nickel onto the PCB mate?
Thanks in advance...
```

---
## \#164 Posted by: Jaydawg56 Posted at: 2019-05-19T23:03:36.514Z Reads: 92

```
Yea. You are gonna have to throttle it waaaay back.  Use that board as a test piece and find the right setting.  I use a boss welder and when I go nickel on steel my duration is 10mS... compared to nickel on pcb it’s only 2mS. 

Then I test how hard it is to peel it up and off.  Find the happy medium and I went with it.
```

---
## \#165 Posted by: Wizeartz Posted at: 2019-05-19T23:19:05.522Z Reads: 89

```
Star as always dude, thanks very much, I'll go scribble on my cookbook :)
```

---
## \#166 Posted by: Nandox7 Posted at: 2019-05-19T23:27:10.419Z Reads: 91

```
How deep was the pocket you had to do?
Asking as if not much an alternative would be to raise the enclosure. I use only the AT wheels so unless is to much there should still be lots of clearance to the ground.
```

---
## \#167 Posted by: Wizeartz Posted at: 2019-05-19T23:32:41.201Z Reads: 88

```
I laser cut a 6mm thick flexible plastic enclosure to pack out the enclosure as I don't want to add more flex to my deck!
```

---
## \#168 Posted by: Jaydawg56 Posted at: 2019-05-20T02:10:29.240Z Reads: 87

```
I’d have to get the caliper out but it was about a 4mm pocket.  Didn’t notice any difference really, but that could just be me.  

Plenty of options though. Some offer spacers anywhere from a 5mm to 18mm for a double stack battery.
```

---
## \#169 Posted by: Jaydawg56 Posted at: 2019-05-20T03:03:37.724Z Reads: 92

```
Yea man. It’s totally preference IMO. once I got it nailed down I did a few tests.... peeling straight up it’ll peel off...  pushing on the side of the nickel strip weld didn’t not cause the strip to shear off the PCB. 

I know it was mentioned that it can/does, but when your cells are glued to the pcb the nickel strips aren’t carrying the stress and load from flex and twisting etc. with proper insulation  and wrap I’m comfortable taking the chance. 

TL;DR... if kaly does it with 3mm strips with just two tacks then I can trust it too, haha
```

---
## \#170 Posted by: Wizeartz Posted at: 2019-05-20T03:35:28.269Z Reads: 93

```
Keen to see the GTR pack pulled apart. I was thinking the cells all siliconed together, and tacked directly with a flexible PCB would be awesome! I started this VTC "belt" like this before breaking into groups of 4 ![18650Belt|666x500](upload://n4bF2mWkiKX3ipvHxIqTqmGEk7F.jpeg)
```

---
## \#171 Posted by: Nandox7 Posted at: 2019-05-20T10:26:07.066Z Reads: 88

```
Thank you!
There was no need for a precise measurement was just to get an idea.

As I don't have a way to do a clean pocket on the board I was looking at some easier alternatives and the spacer was one of them depending on how tall it need to be.
4 to 5mm is totally feasible and I may even design one in some that help seal better the enclosure.
```

---
## \#172 Posted by: Whoknows Posted at: 2019-12-30T08:21:51.824Z Reads: 38

```
 Hi @Wizeartz how did you get one have you put it altogether and had it going?
```

---
## \#173 Posted by: Wizeartz Posted at: 2019-12-30T18:46:41.332Z Reads: 38

```
Yes I did, I’ve done 3 packs now.Almost good at it! Last pack was a 10S5P of 35e cells for my CGT. Very good output, and range now! Though it cuts out in GT mode, so I stick to fast mode. Suspect motor controller...
```

---
## \#174 Posted by: Jaydawg56 Posted at: 2019-12-31T03:51:29.849Z Reads: 38

```
Should really just ditch all the evolve electronics.  When I ride my unity equipped carbon vs my evovle GTX it just doesn’t compare.   Power is weak and I always question if it’ll cutout.
```

---
## \#175 Posted by: Wizeartz Posted at: 2019-12-31T07:37:53.684Z Reads: 37

```
I might just do that Jaydawg, I got spat off at 35km/h a month ago, my knee is shagged, haven’t walked right since. I suspect my gloved palm double pushed the power button on the R2 as I was in config mode when I picked myself up. Hate that frikkin remote, R1 is better!
```

---
## \#176 Posted by: Eboosted Posted at: 2019-12-31T14:37:13.284Z Reads: 41

```
Forget the original Evolve electronics, upgrade everything inside and enjoy a perfect board
```

---
## \#177 Posted by: Wizeartz Posted at: 2019-12-31T18:47:54.075Z Reads: 38

```
If I want to hit 50km/h or more on my CGT using AT’s, I assume I’d need to upgrade to a unity, new motors and a 12s pack?
```

---
## \#178 Posted by: Eboosted Posted at: 2019-12-31T19:39:55.141Z Reads: 41

```
You could keep the motors and just set the correct gear ratio, everything else must go.

Btw those Gullwing Sidewinders are not meant for high speed, they will wobble berzerk
```

---
## \#179 Posted by: riverside.rider Posted at: 2019-12-31T19:47:48.589Z Reads: 40

```
Or keep the evolve trucks and get some bergmeisters and ride within limits of sanity 😜
```

---
## \#180 Posted by: Whoknows Posted at: 2020-01-02T02:37:33.274Z Reads: 38

```
Which do you prefer the 30q or 35e? Were did you buy the cell from? Any chance you would consider building me a pack?
```

---
## \#181 Posted by: Eboosted Posted at: 2020-01-02T04:08:38.747Z Reads: 39

```
The 35E has only 8A of discharge, if you want a decent board  you will need a 12s12p, that's really a bad idea.

The 30Q is the best bung for the buck, the 30T are the most powerful, the 40T have the best range, the P42A are the greatest at this point and time

Hit me via PM if you need a custom battery with enclosure fue your Evolve
```

---
## \#182 Posted by: Wizeartz Posted at: 2020-01-02T19:53:59.358Z Reads: 38

```
I went with 35e as I was under the impression I’d get better range. I’ve built two packs using 30q’s in 10S4P, and one 10S5P of 35e’s. Sourced from China via Aliexpress, actual cells vary but the price is such for us in NZ it’s worth the risk. The first pack I built with 30q locally sourced which were hideously expensive, and not necessarily any better than the aliexpress items.
```

---
## \#183 Posted by: Whoknows Posted at: 2020-01-02T21:17:38.259Z Reads: 37

```
How has the real world performance turned out?
```

---
## \#184 Posted by: Eboosted Posted at: 2020-01-02T22:00:04.382Z Reads: 36

```
10s4p made of 35E with give you 32A of discharge, you might be able to move one motor, restrict the current to 30A for single motor or 15A for dual
```

---
## \#185 Posted by: Wizeartz Posted at: 2020-01-03T06:31:12.805Z Reads: 33

```
Hard to tell, as it cuts out in GT mode, but with 8” AT wheels, in Fast mode, pulling my 95kg at a consistent 35-40km/h I use about a third of my battery capacity after 8km, with minimal sag. So far I’m impressed, but will probably replace the Evolve electronics with a Focbox and see how she REALLY flies!
```

---
## \#186 Posted by: Wizeartz Posted at: 2020-01-05T21:26:53.750Z Reads: 29

```
Focbox unity ordered!
```

---
## \#187 Posted by: Jamiecgt Posted at: 2020-02-06T11:05:46.233Z Reads: 15

```
Hi, amazing tutorial thanks for uploading it. I'm just about to start building the same pack. The only thing I'm not sure of is whether the series groups should be glued together? As it would stop the flex. I've got the carbon deck so maybe it doesn't really matter anyway. I would really appreciate any advice. Thanks jamie
```

---
## \#188 Posted by: Hatman30 Posted at: 2020-02-06T15:33:03.291Z Reads: 12

```
If you’ve got a carbon u don’t need the pack to flex
```

---
## \#189 Posted by: Jamiecgt Posted at: 2020-02-06T22:34:54.427Z Reads: 11

```
Thanks, I thought as much. Does anyone know what cable to use for the long positive? 12awg?
```

---
