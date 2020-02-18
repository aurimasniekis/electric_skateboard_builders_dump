# VESC DRV8302 Failures and Repair Options

### Replies: 177 Views: 18450

## \#1 Posted by: longhairedboy Posted at: 2016-06-03T18:46:04.846Z Reads: 933

```
Mine had bad DRVs. Word on the street is a lot of them had DRVs that failed as a result of bad or malfunctioning capacitors or other power related issues. You find a guy who can and is willing to simply replace components on all these "bad" VESCs laying around and you've probably got another boutique business opportunity. If somebody was to buy up all these bad vescs from people and just replace the parts on them that don't check out then they could probably make a killing. 

I've tried to find a local shop to replace those chips on mine and so far no one seems to want to return calls or emails or they don't see it as being worth the effort or whatever. I have the chips, its not like they have to do anything but replace it. I'd probably be willing to pay $30 or $40 to get them fixed, maybe more. I'd never use them in a customer build, but i'd sure as hell use them in my own personal ones.
```

---
## \#2 Posted by: Jinra Posted at: 2016-06-03T18:47:55.412Z Reads: 842

```
I think @jacobbloy has this service, but it's hardly local for us :)
```

---
## \#3 Posted by: makepeace Posted at: 2016-06-03T19:26:20.524Z Reads: 828

```
It seems like a good idea to repair all of these broken products like motors and VESCs etc, but in practice it doesn't really work that well. There is much risk in fault-finding and repair. It only really works if you're doing it for yourself because you can't afford not to otherwise.
```

---
## \#4 Posted by: longhairedboy Posted at: 2016-06-03T19:42:16.512Z Reads: 807

```
i suppose that's true. I just wish it wasn't because i have two dead VESCs in a bin just laying there with fried DRVs, and two brand new DRVs just laying there... and as hard as i try.. i can't replace them with the powers of my rage. It just pisses me off.
```

---
## \#5 Posted by: Karmannghiagirl Posted at: 2016-06-03T19:43:00.253Z Reads: 777

```
Psssssssssttttt.... 

hi :slight_smile:


Seriously though, I've spent way too much money recently to be jumping into anything right now. but paycheck after next i might invest in a hot air reflow station and try my hand at VESC repair.
```

---
## \#6 Posted by: longhairedboy Posted at: 2016-06-03T19:47:15.517Z Reads: 748

```
if you are trying to lure me into a long term online friendship its working. I will hang on to them for now and when you get your station set up maybe you could use my VESC and parts to try it out?
```

---
## \#7 Posted by: Karmannghiagirl Posted at: 2016-06-03T19:50:10.270Z Reads: 726

```
sounds good to me :smiley:

BTW if anyone else is interested, once i get setup I'll probably put up a thread about it with prices and everything. if all goes well it will probably be around $30-40 per vesc (including return shipping)
```

---
## \#8 Posted by: makepeace Posted at: 2016-06-03T20:03:45.878Z Reads: 717

```
A caveat from some time I spent working for an engineering machine repair company: one of their clients had a CNC machine that used a very normal PSU for it's computer. It fried, and they replaced it for about $250 (the supply specced was quite special). I fucked around with the broken supply for about an hour and found that 1 resistor had blown. I asked them if I could have it and replaced the resistor for a couple of cents. That worked out well. Another example, my dad bought a vintage broken audio amp and asked if I could have a look at it. I spent about 10 hours fault finding and replacing components and it's still not working. Long and the short is you need to consider the cost/benefit. It works sometimes, but most times it's a really bad idea unless you're willing to commit personal time to fixing it.
```

---
## \#9 Posted by: treenutter Posted at: 2016-06-03T20:20:17.404Z Reads: 703

```
@longhairedboy @Karmannghiagirl @makepeace [When my VESC recently fried](http://www.electric-skateboard.builders/t/another-drv8302-fault-i-win-the-esk8-darwin-award/3908) I ping'd the usual suspects for repair options... no takers.

I called a bunch of local electronics shops...the ones that were willing to do it$65 not including the price of the new chips. Pfffftttt!!!

So what does a stubborn DIY'er do? I did some reading and some research and ordered the tools to do DRV repairs myself. Check out what arrived today:

<img src="/uploads/db1493/original/2X/2/2ad262a035c23c9e58cb0350f98699392cc7381d.jpeg" width="375" height="500">

<img src="/uploads/db1493/original/2X/d/d7721f50acdae0d3ad7dd65151114ab1037a318e.jpeg" width="375" height="500">

If repairing mine goes well, I might offer some zero-warranty repairs. More to follow!
```

---
## \#10 Posted by: Jinra Posted at: 2016-06-03T20:23:14.075Z Reads: 678

```
Make sure you watch this!

https://www.youtube.com/watch?v=3NN7UGWYmBY
```

---
## \#11 Posted by: DougM Posted at: 2016-06-03T21:13:25.578Z Reads: 671

```
Just remember there's a center pad on the bottom of that chip - you can't just hot-air the pins and expect it to come up.  Your better bet is an IR rework station so you can preheat the board, then hit the chip with IR to bring it up.  Ditto to put it down.  But you have to be careful not to move the components on the bottom, *and* not melt the connectors.  Kind of a tricky dance, which is why I'm hoping to pay @Karmannghiagirl to do it :-)

something like this:

[T862++](http://www.ebay.com/itm/T862-BGA-INFRARED-REWORK-STATION-SOLDERING-WELDER-SMT-SMD-IRDA-MACHINE-USA-/321917196792?hash=item4af3c299f8:g:mO4AAOSwd4tT7bA6)

they're amazingly cheap now.  When I bought mine it was $700.  

DougM
```

---
## \#12 Posted by: treenutter Posted at: 2016-06-03T21:31:53.813Z Reads: 651

```
Thanks @DougM! An infrared station seems optimal. I believe that we can use hot air to heat the whole chip (from the bottom and then on top) to remove the chip and replace it.

That's how this guy did it:

https://www.youtube.com/watch?v=qeWzP2YahNc

Is this process worse in some way that I don't understand?
```

---
## \#13 Posted by: makepeace Posted at: 2016-06-03T22:01:52.060Z Reads: 643

```
I think the splitting of this thread was a little bit unnecessary and destructive to the original conversation. The content was derived from and pertains to the original thread and conversation, and is clearly thereto relevant. The poster regarding the repairs of VESCs had already committed to starting a new thread about that.
```

---
## \#14 Posted by: Karmannghiagirl Posted at: 2016-06-04T00:04:52.969Z Reads: 620

```
i disagree, i think it was good to split this out, the other thread was started to talk about customer service, not vesc repair.
```

---
## \#15 Posted by: seanpain4 Posted at: 2016-06-04T00:58:14.338Z Reads: 619

```
Remember to use tons of flux! It is extremely helpful.

Just clean it up afterwards though
```

---
## \#16 Posted by: JohnnyMeduse Posted at: 2016-06-04T01:53:56.875Z Reads: 614

```
It seems to be something really hard to do ... I wish there was somebody who can do it in less than 2 minute  :stuck_out_tongue_winking_eye:
https://www.youtube.com/watch?v=opdrL_02VL8
```

---
## \#17 Posted by: chipoi84 Posted at: 2016-06-04T02:15:37.994Z Reads: 602

```
It's looks pretty hard at first, but it is definitely doable if you have at least a heat gun, flux, solder paste, tweezer and kapton tape to shield the other components (mostly the jst connectors so they don't melt). Also I recommend replacing the eight 10uf capacitors on the pcb and the three 680uf 63v on the capacitor board if you have the earlier batch (4.10 or earlier) of the Enertion's vescs. These components seem noticeably smaller than the vesc from Chaka.
```

---
## \#18 Posted by: treenutter Posted at: 2016-06-04T11:09:18.893Z Reads: 584

```
@JohnnyMeduse this is a great demo of the removal. For the replacement I think that solder paste would need to be applied to the pins, then heated, then checked for bridges. My point is that the video just shows one step, right?
```

---
## \#19 Posted by: JohnnyMeduse Posted at: 2016-06-04T13:29:36.932Z Reads: 593

```
Not really, you still have more than enough solder on all the pads for the new DRV (in the video, I was doing the demo with a scrap board, so I juste put the old DRV back). And removing the leftover short should not be that long, when you have more than enough experience. :wink:
https://youtu.be/jwKptzHP9HU
```

---
## \#20 Posted by: chaka Posted at: 2016-06-04T14:27:16.856Z Reads: 575

```
It is always a good idea to preheat the whole board with hot air for about a minute or two before getting into it and heating the chip. If you go at it too quickly it can cause heat expansion stress on the pcb.
```

---
## \#21 Posted by: treenutter Posted at: 2016-06-04T14:37:44.287Z Reads: 558

```
Thanks for these vids @JohnnyMeduse! The liquid in the clear plastic bottle is flux, correct? (asking for those who might only use flux paste)
```

---
## \#22 Posted by: JohnnyMeduse Posted at: 2016-06-04T14:57:34.276Z Reads: 561

```
@chaka Yes it is always a good idea to reheat the board, but because the Vesc is a pretty small pcb it won't really create stress on other component, also the board heat pretty well there not enough heat dissipation, to give problem with juste the heat gun. @treenutter Yes, this is liquid NO CLEAN FLUX.
```

---
## \#23 Posted by: treenutter Posted at: 2016-06-05T19:21:07.721Z Reads: 567

```
I managed to get the DRV8302 chip off of my VESC last night without too much trouble. I tried using flux paste, 2.5mm solder wick, and a small-tipped iron to clean up the board and it didn't work very well. I still had bridges left over from the removal of the DRV8302. I also tried to remove it with hot air, but it caused more damage than anything (I melted a part of the jst connector and accidentally displaced one of the small caps).

I've got some liquid no-clean flux on the way, with a needle-tipped bottle to apply it accurately. I've also ordered some kapton tape (Thanks @chipoi84) to protect things while I'm in there.

I have a 3rd hand tool w magnifying glass, and at 10x and 60x loupes. But those still didn't seem ideal for magnification. Is there some obvious thing I'm missing here to clearly see what's going on?

<img src="/uploads/db1493/original/2X/4/453955065b955620e311151fe15e693b311d7319.jpeg" width="375" height="500">

<img src="/uploads/db1493/original/2X/4/480d490ec2a5ab32da2bfa097823d532fcec2c70.jpeg" width="375" height="500">
```

---
## \#24 Posted by: JohnnyMeduse Posted at: 2016-06-05T19:34:25.364Z Reads: 524

```
If I may give you a word of advise, always use a Tips that is larger, like 1.5mm, the larger the tips the more solder it will absorb on the wick, also put a bit a flux on it. Also use the same motion on each pad when you clean it. And the two short you see a normal, they are par of the circuit.
```

---
## \#25 Posted by: treenutter Posted at: 2016-06-05T19:53:37.564Z Reads: 525

```
@JohnnyMeduse thanks I'm always happy to get advice! I'll try a wider tip while using the solder wick (waiting for the liquid flux).

THANK YOU for confirming that those two shorts are normal; I thought I was going crazy trying to remove them.

The strange thing about this DRV error is that once I removed the chip I didn't see any evidence that the DRV8302 was damaged; no holes, not burnt spots, etc. At first I thought those shorts might have been caused by overheating or bad soldering at the factory.
```

---
## \#26 Posted by: JohnnyMeduse Posted at: 2016-06-05T19:58:14.135Z Reads: 515

```
I have change a few of them, with this king of problem, and never see any mark or damage, it more likely to be a internal failure. The problem seem to happened when you go over 70000 rpm. I have de same kind of problem with MCU who are internally short. That the beauty of electronic it alway a new adventure :stuck_out_tongue_winking_eye:
```

---
## \#27 Posted by: DeathCookies Posted at: 2016-06-06T09:03:12.870Z Reads: 507

```
Here in germany is one company that will swap a DRV for 50€ included a new chip excluded the shipping. A lot of money but if you cannot swap it yourself it is the best way to go...
```

---
## \#28 Posted by: treenutter Posted at: 2016-06-10T01:52:40.979Z Reads: 522

```
@JohnnyMeduse @chipoi84 the liquid flux works like a charm! How did I get this far without it? I found that dousing the solder wick with it made a huge difference. I was able to clean off all of the old solder on the board. 

<img src="/uploads/db1493/original/2X/6/61c802333cfb4be7d91f95ee0aef85f29ecf9610.jpeg" width="375" height="500">

Any tips on how to clean up the other residues left on the board?

Another challenge is keeping the chip in place and lined up while I apply the hot air. I don't want to use too much solder paste, but too little makes the chip slide around like a hockey puck!
```

---
## \#29 Posted by: JohnnyMeduse Posted at: 2016-06-10T02:56:34.397Z Reads: 509

```
You can put a little bit of Isopropyl Alcohol and brush it, or just brush it without the alcohol (if you don't have any). I suggest using a wooden Brush (because the are made for this purpose, the one in the picture is from MG Chemical).

<img src="/uploads/db1493/original/2X/1/1d7339d0d2de07f48b3bc577a20fc8aed890ee1a.jpg" width="375" height="500">
```

---
## \#31 Posted by: treenutter Posted at: 2016-06-10T14:25:56.586Z Reads: 476

```
Thanks @JohnnyMeduse! Any tips on lining up the DRV and keeping it in place? I feel like it jumps around on the board and I can't keep it steady!
```

---
## \#32 Posted by: DougM Posted at: 2016-06-10T15:22:04.669Z Reads: 478

```
If you/'re talking about soldering the chip [edit] with a soldering pencil [/edit] do the following:

Place the chip on the pads aligned as close as you can get.  Hold it in place with one finger and using your soldering iron, tack down one pin in one corner.  Now pick any other corner, re-align the chip and tack down the pin on that corner.

flux and solder all pins.

DougM
```

---
## \#33 Posted by: treenutter Posted at: 2016-06-10T15:26:04.313Z Reads: 466

```
Thanks @DougM. That sounds like a good strategy! I've been trying to line it up evenly and then hit it all with hot air at once, and that hasn't worked. I almost got there once, and then I accidentally tapped the chip with the hot air gun!

I'll try tacking down a few pins with my iron first (maybe 4 of them?) and then I'll use solder paste, flux,  and hot air to get the rest.
```

---
## \#34 Posted by: DougM Posted at: 2016-06-10T15:39:20.053Z Reads: 463

```
Hot air is tricky - the airflow has to be low enough not to blow the chip off the pad because the pins you tacked will re-melt.  This is a skill I never developed :slight_smile:

Tacking down the 4 corner pins seems like a good strategy.

DougM
```

---
## \#35 Posted by: treenutter Posted at: 2016-06-10T20:18:39.371Z Reads: 454

```
@DougM I think I need to use hot air  to get the pad under the DRV to make contact, but of course I have to do that without melting everything else! Kapton tape is helping for sure!
```

---
## \#36 Posted by: hexakopter Posted at: 2016-06-10T20:21:37.362Z Reads: 467

```
And don't forget to save the jst socket from the hot air. The plastic is melting quickly.
```

---
## \#37 Posted by: DougM Posted at: 2016-06-10T21:31:13.941Z Reads: 480

```
@treenutter - Yes, getting the pad underneath soldered correctly is critical.  pre-heating the whole board helps with this.  

I've never tried this but you can get hot air rework nozzles like these

<img src="/uploads/db1493/original/2X/8/873a0b540fc3dadaae80c31416437679b338ba62.png" width="565" height="500">

that allow you to localize to a single chip.

DougM
```

---
## \#38 Posted by: chipoi84 Posted at: 2016-06-10T21:48:20.428Z Reads: 458

```
I use a regular big old heat gun, and it works fine. Just make sure to heat the entire board carefully first, before apply the heat on the drv chip. Also, it would help to use solder wick to clean and make sure the solder pads for the drv chip is even first. If you have one of those soldering helping hand, it would help a lot to keep the entire pcb even, preventing the components from moving around. When I heated my drv, sometimes it would move perfectly into the correct position by itself due to the pull of the solder paste.  If not, I would hold the heat gun in one hand, and adjust the chip using a tweezer with the other hand.
```

---
## \#39 Posted by: sl33py Posted at: 2016-06-10T22:26:04.209Z Reads: 455

```
i've helped replace two dead DRV's now - with a reduction tip on the hot air to focus the hot air just where you want it, and ability to turn the air flow down so you aren't blowing other components off their pads when they also melt.

Some kapton tape as a barrier definitely can help if you just surround the DRV chip to deflect hot air from the other components.
```

---
## \#40 Posted by: squad Posted at: 2016-06-10T23:41:50.746Z Reads: 483

```
I thought it was impossible to remove drv chip without fancy soldering equipment... BUT after I realized that FOC fu**ed up also my second VESC on mountainboard (which I thought was ok), decided to give myself a try and remove that little fu**er. I used: laser thermometer (for controlling temp of pcb during preheating), heat gun (used for preheating board from bottom), gas solder iron (with removed tip, it blows narrow stream of hot air, used for final heating drv chip), flux and obviously tweezers. Here is effect:

http://i.imgur.com/lAgqXAS.jpg
http://i.imgur.com/LjvdPbv.jpg

Two new DRV8302 chips are on their way, should be here on monday.
```

---
## \#41 Posted by: treenutter Posted at: 2016-06-11T02:09:30.445Z Reads: 492

```
Thx @hexakopter, that's good advice but I've already demolished the jst connector! I'll have to replace it.  

@DougM I'd never seen those before thanks!

@chipoi84 so far I've been taping the pcb to a metal surface but a jig would be a lot better. Yes, I'll be sure to clean the pad before I mount the chip. I think I've been skimping with the solder paste. 

@sl33py I've got kapton tape all over now, it's saved me a few times already!
```

---
## \#42 Posted by: Jinra Posted at: 2016-06-11T04:23:23.428Z Reads: 493

```
You can also try the drag soldering method to get the DRV chip on :)

https://www.youtube.com/watch?v=wUyetZ5RtPs
```

---
## \#43 Posted by: c4Lvin Posted at: 2016-06-15T05:02:21.696Z Reads: 484

```
would anyone of you have want to take the challenge to fix my VESC?
```

---
## \#44 Posted by: Jinra Posted at: 2016-06-15T05:11:03.268Z Reads: 481

```
Where do you live?
```

---
## \#45 Posted by: c4Lvin Posted at: 2016-06-15T05:11:31.181Z Reads: 473

```
Southern California here!
```

---
## \#46 Posted by: chipoi84 Posted at: 2016-06-15T05:12:55.623Z Reads: 473

```
What city?
```

---
## \#47 Posted by: c4Lvin Posted at: 2016-06-15T05:13:38.863Z Reads: 465

```
Inland Empire!
```

---
## \#48 Posted by: chipoi84 Posted at: 2016-06-15T05:21:52.237Z Reads: 470

```
If nobody else takes you up on it, I'll do it. Can't really guaranteed anything, so you are going to have to take a leap of faith here. I am not a professional, but I have done this a few times before. Also, I'm in Anaheim, so you probably have to ship it to me. I'll charge you the cost for the drv chip plus the cost of the return shipping, so probably around $15.
```

---
## \#49 Posted by: c4Lvin Posted at: 2016-06-15T05:24:22.262Z Reads: 471

```
I can personally deliver it to you if you want? I'll be in Yorba Linda tomorrow anyways. PM if you want. Thank you.
```

---
## \#50 Posted by: Skitzor Posted at: 2016-07-11T11:48:35.583Z Reads: 450

```
So I've ordered a new DRV chip for € 9,50. I have a soldering station 0-400*C and a weller pryopen on gas which can heat till 650*C. Do you think I'll be able to melt the solder with this and replace the chip ? I've done this before in playstations and stuff, just want some good advice from the community. Even if I need to order a special soldering tip or something. Help me out here.
```

---
## \#51 Posted by: sl33py Posted at: 2016-07-11T19:43:21.959Z Reads: 446

```
@Skitzor Does your solder station have hot air?  I have one w/ hot air, and the small reducer tips to focus the air just where i want it.  The tricks i learned helping with the last 2 that failed, were to warm up the whole board slowly, and then just focus the heat on the DRV chip itself w/ lots of flux to help.  Once you remove the bad chip - clean up the old solder (solder wick), place new solder paste on and heat until it liquifies and secures the new DRV.

You need to be able to adjust the airflow - if you heat it up w/ lots of air it can melt and blow other components off their pads.  So lower airflow and reduction tip to focus the air just where you need it. And like mentioned above you can use some of teh Kapton tape to protect/block the air from other small components so they don't blow off.

I have a handfull of chips on the way to have as spares.  One dead VESC ready to replace...  Looking forward to getting this skill dialed in.  Hopefully not needed frequently, but love my VESC's and good to be able to repair myself when/if one fails.
```

---
## \#52 Posted by: Skitzor Posted at: 2016-07-11T19:52:09.743Z Reads: 436

```
Hi @sl33py, thanks for the tips, appreciate it !
The pryopen has a hot air feature built in (I didnt mention that in above post, but was talking about hot air, not a soldering tip on the pryopen)
What's the reason behind warming up the whole pcb? so it doens't break while the heat is expanding the DRV- area?
I've ordered a flux pen too to clean up the whole residue after I get the chip out.
I'm understanding the whole operation, but what should I do, if I have the new DRV on there and 2 legs are sharing solder?
Can I just remove it with a desoldering pump ?
```

---
## \#53 Posted by: sl33py Posted at: 2016-07-11T20:01:11.511Z Reads: 425

```
those with more expertise may have better description of the steps, but here's what i helped do last time:

heat the whole pcb gently - not to the point solder re-flows, but still pretty hot.  (reduces stress and less likely to burn the chip iirc)

Instead of mechanically removing the DRV chip (solder is under it as well as legs), heat it w/ the reduced hot-air tips until the solder re-flows.  Once molten - use tweezers to remove the bad DRV chip(anti static super fine tip help).

Then use your wick to clean the pads and inspect.  Once looking good - add solder paste to the pads and heat until it flows and secures DRV.  Check your pins - clean up any bridging w/ wick, then test.

Hey experts - anything to add or correct if i'm way off base?

Edit - adding lots of liquid flux to the chip to both protect it and help transfer heat better - both removing and replacing it.  Kinda messy amounts were what buddy showed me.
```

---
## \#54 Posted by: treenutter Posted at: 2016-07-11T20:09:31.999Z Reads: 402

```
[quote="sl33py, post:53, topic:4201"]
Then use your wick to clean the pads and inspect
[/quote]

Great description @sl33py !

@Skitzor more tips:  I found that soaking the solder wick with liquid flux helps a lot, make sure to have some. Also, be mindful of the size of the needle that comes with your solder paste; the first one I tried was way too thick and I ended up with lots more solder than I needed. You only need a very thin line of it for this repair.

I also suggest having a very bright light and good magnification, which really make the process easier. I got a 10x loupe so that I could closely inspect the legs of the chip to make sure there were no shorts.
```

---
## \#55 Posted by: sl33py Posted at: 2016-07-11T22:40:57.874Z Reads: 392

```
Thanks man!  I'll have to look for some smaller needle for my solder paste as well.  When i want to look especially _geek chic_ i wear my:
https://www.amazon.com/gp/product/B00VL22OEG

Nothing says a _**man of distinction**_ like headset magnification...  But seriously awesome for hands free and light exactly where you need it.
```

---
## \#56 Posted by: treenutter Posted at: 2016-07-11T23:44:20.628Z Reads: 411

```
[quote="sl33py, post:55, topic:4201"]
Nothing says a man of distinction like headset magnification..
[/quote]


@sl33py LOL that is dead sexy! I freaked my wife out once when I came out of the basement with a respirator over my face

<img src="/uploads/db1493/original/2X/e/e64949401a178648eb45e17fdfeb0dae72e66fec.jpeg" width="158" height="173">
```

---
## \#57 Posted by: Skitzor Posted at: 2016-07-14T17:39:09.698Z Reads: 416

```
Well, Rip Vesc :D everything went fine untill the second bottom left pad kept sticking to my solder wick, so no more connection on that leg. Or do you think I could still try to use it without the one leg if it isn't an important one...

<img src="/uploads/db1493/original/2X/0/082da14add7ad808af994199d76b3a67be4c418c.jpeg" width="666" height="500">
```

---
## \#58 Posted by: chaka Posted at: 2016-07-14T18:21:04.136Z Reads: 404

```
Those last 2 legs are are not connected to any circuit. The VESC is still viable. :ok_hand:
```

---
## \#59 Posted by: Skitzor Posted at: 2016-07-14T19:10:15.693Z Reads: 404

```
I'm too stressed atm from this whole operation. I can see copper coming to the surface between legs 1-7 . I'm going to keep this vesc for spare parts and will not risk adding a DRV chip and losing that too. 

It's kinda murphy's law all the way, I was practising on another pcb with the same kind of chips, removed 3, resoldered 3 without problems, started on the vesc and everything went a'wall.
```

---
## \#60 Posted by: mishrasubhransu Posted at: 2016-07-14T19:20:15.650Z Reads: 426

```
I have access to a hot air rework station and also happen to be kinda good at smd soldering. I am definitely interested in bringing the broken VESCs back from the dead, but don't have any :disappointed:  I can probably ask people for a couple, but since I am relatively new here, I don't really know if it is rude to ask people if they have broken VESCs that they are willing to part with, in exchange for some $ ? 

PS: Any broken VESC, not just the one with the DRV problem.
```

---
## \#61 Posted by: Nordle Posted at: 2016-07-20T20:50:52.497Z Reads: 430

```
Someone who can change my drv in EU?
```

---
## \#62 Posted by: MidnightOne Posted at: 2016-07-20T21:17:38.831Z Reads: 435

```
Best piece of advice: don't be afraid to do it if you really need to, especially if you've built the rest of your skate yourself.

For example: I replaced the Atmega chip (TQFP32 package) on an arduino mini clone with an industrial heat gun (a really bad choice for smd rework, but it had to do) a while ago. Not to say it was economically feasible too (the chip costed me the same as a new clone), but what will you do if you need it really quick and you don't have the right tool at hand. It was an interesting experience.
<img src="/uploads/db1493/original/2X/4/48aeaf7f6ea97961e535a3b38d41ad32ddfc9bc0.jpg" width="669" height="500">

PS: Watch Louis Rossmann videos on smd rework, they're a gem:
https://www.youtube.com/channel/UCl2mFZoRqjw_ELax4Yisf6w
He also has very good input on apple business tactics and business in general.
```

---
## \#63 Posted by: Nordle Posted at: 2016-07-20T21:24:30.765Z Reads: 415

```
Thank you, i think you are right. I should give this a try!
```

---
## \#64 Posted by: shred Posted at: 2016-07-21T14:37:35.307Z Reads: 417

```
would be a great skill, that's for sure! wish you luck! 

If you change your mind you could check with these guys:
http://www.lp-electronic.com/vesc/
```

---
## \#65 Posted by: Skitzor Posted at: 2016-07-29T11:57:30.447Z Reads: 415

```
@chaka, I'm going to need another opinion from you.
I've just repaired my dual setup with an interim vesc I've ordered from esk8.de.
Now after my second 1h run. At the very end the belt from my right motor broke. I was only doing 10km/h but wasn't able to brake. The right motor and vesc are fine, but the left one doesn't get power trough.

Took a look at the drv chip (2nd enertion vesc, not the new one) it isn't burned yet (cross-fingers) but I see legs with joined solder. Could this be the reason. I'll hook em up to bdlc once I get home to see if it connects and I can see errors.
<img src="/uploads/db1493/original/2X/f/fd35358fdd0eec61b4791afc24e0f0700726bcc8.jpeg" width="375" height="500">
And is there a way to protect the vesc from doing this?
```

---
## \#66 Posted by: lox897 Posted at: 2016-07-29T12:22:06.052Z Reads: 385

```
A few of the pins need to be connected. I don't think that is the problem.
```

---
## \#67 Posted by: chaka Posted at: 2016-07-29T13:38:20.791Z Reads: 377

```
Could just be a canbus issue. Let me know what happens when you power it and connect to the bldc-tool.
```

---
## \#68 Posted by: Skitzor Posted at: 2016-07-29T14:38:46.645Z Reads: 382

```
There's been 2 hours between the test's I've made. Left motor wouldn't do anything.
Now I am at home. No error codes, motor runs again.
So I guess it could've been a canbus issue. How do you explain this? how can I resolve it?
```

---
## \#69 Posted by: chaka Posted at: 2016-07-29T14:46:40.181Z Reads: 380

```
I haven't had any issues on the latest hardware/firmware using 4 pin jst-ph connectors. Make sure the connectors you are using have positive contact, should feel some resistance when pushing them on the pins.
```

---
## \#70 Posted by: Skitzor Posted at: 2016-07-29T15:03:22.372Z Reads: 387

```
I'm running FW2.18 on both vescs. In the vesc FAQ it states not to connect 5v and ground cause of grounding issues. Enertion Vesc has it soldered on, on the second I use the 2 middle pins with a connector so it's easy to go from single to dual drive.
```

---
## \#71 Posted by: chaka Posted at: 2016-07-29T18:43:16.237Z Reads: 388

```
Yes, you do not use the 5v or gnd. If you connection is good then you may want to check the slave vesc for faults.
```

---
## \#72 Posted by: Jinra Posted at: 2016-07-29T18:47:41.867Z Reads: 400

```
Can you link me to this? I wasn't aware you're not supposed to use the 5v pin on the can bus
```

---
## \#73 Posted by: tim_felbinger Posted at: 2016-11-16T06:59:57.220Z Reads: 345

```
Hello all,

I too will be joining the 'Replace your DRV8302 chip' club...

Luckily I am in college at Georgia Tech and we have a workshop with professional rework equipment.

I noticed that my VESC seems to have also lost it's C26 capacitor, can anyone tell me what exactly that does?

Replacement parts have been ordered from Mouser based on the BOM on the VESC GitHub.

After the board stopped working (I was running FOC mode with long wires) I tried to plug the vesc in again for power and it short-circuited and blew the DIY electric skateboards power switch I had on the board and vaporized the nickel strip attaching the positive wire to the battery. 

Based on this, I am a bit hesitant to try the VESC again, even after I fix it. 

So a few questions:
1) What does the C26 capacitor do?
2) I see that some legs of the DRV are fused, it that the issue?
3) Is there anything else that looks abnormal about the VESC?
4) Anything else that could have lead to the short
5) Can the VESC be powered from a lab bench power supply? (Because those have short circuit protection and more importantly wont cause fires)
```

---
## \#74 Posted by: JohnnyMeduse Posted at: 2016-11-16T13:40:24.209Z Reads: 346

```
[quote="tim_felbinger, post:73, topic:4201"]
I noticed that my VESC seems to have also lost it's C26 capacitor
[/quote]


C26 is mostly use for adding capacity over FOC option, without it you will most likely burn the drv, also if you bought your VESC from DiyElectricSkateboard it is normal they use the BOM for the 4.10 version, witch don't have the c26 capacitor.

The drv have two set of pin that are short, you can always refer to the schematic available on vedder web site. 

and yes you can power it using a bench power supply.

And if you need someone to replace you drv, maybe I can help you.

http://www.electric-skateboard.builders/t/johnny-vesc-repair-services/11267
```

---
## \#75 Posted by: tim_felbinger Posted at: 2016-11-16T16:47:14.461Z Reads: 334

```
So if I add the c26 capacitor and do a c18 mod with a 4.7 capacitor I should be much better off running FOC?

Because I'm on a college campus and occasionally ride through buildings and need a quiet board, my plan is to run dual VESC setup in FOC mode, but the way my board is laid out means I will have about 40cm of wiring between battery and VESC. 

I am currently using 12gauge flat wire, should I double up on that? 

Also, can I combine the capacitor boards of the 2 vescs into one larger capacitor board and then pass wires from there to both vescs? (Cheaper and easier than buying different capacitors if it works)
```

---
## \#76 Posted by: JohnnyMeduse Posted at: 2016-11-17T03:19:14.486Z Reads: 343

```
Just adding C26 will help. The mod with the 4,7uF is a bit more complex and dosen't require to change c18. 

Also, yes you can combine the 2 capacitor board into one, but I highly suggest that you change the capacitor for bigger one, but I can be done. 

http://www.electric-skateboard.builders/t/the-troll-enertion-cf-deck-dual-tbs-6355-sensor-10s-build-completed/1491

For the flat wire I'm not a expert but If can double it, it should be better.
```

---
## \#77 Posted by: tim_felbinger Posted at: 2016-11-18T16:49:22.572Z Reads: 350

```
Thanks. Very nice dual VESC holder concept. 

Which capacitors would you recommend? As in what is the biggest capacitor pair that I can use?

Also, my build thread is up now: http://www.electric-skateboard.builders/t/boosted-pro-loaded-vanguard-rear-dual-6355-sensored-18650-10s2p-with-bms-dual-vesc-in-foc-custom-kydex-enclosure/13236

Here are also some pictures of my burned VESC. You can see the burned DRV and missing C26. Parts have come in from mouser, and I will attempt the repair after my thanksgiving break.

<img src="/uploads/db1493/original/3X/2/3/230129abef2bf729b7d59754039242f407ca1b08.jpg" width="690" height="388"><img src="/uploads/db1493/original/3X/3/d/3d340370bd033d72cd338aa494c1ec19ce45c0d9.jpg" width="690" height="388">
```

---
## \#78 Posted by: JohnnyMeduse Posted at: 2016-11-18T18:04:56.691Z Reads: 324

```
In is setup @Blasto have use 2 x 2200uF instead of 6 x 680uF witch give approximately the same capacity.
```

---
## \#79 Posted by: tim_felbinger Posted at: 2016-11-18T23:07:48.096Z Reads: 324

```
Cool. I think I will go with either 2 or 3 or those to make sure that FOC works reliably. 

Also, I have decided that I will braid 3 strands of the 12amg flat wire together and then inlay and epoxy it into the board a bit. That should give me plenty of capacity to push through the wires.
```

---
## \#80 Posted by: rtasca Posted at: 2016-11-19T21:19:02.819Z Reads: 340

```
OMG, joined the club

8s BLDC, nothing fancy.

I think it was while pushing the board unpowered. :frowning: I noticed it suddenly locked the motor.


 

The following faults were registered since start:

Fault            : FAULT_CODE_DRV8302
Current          : -0.9
Current filtered : 0.8
Voltage          : 30.32
Duty             : 0.02
RPM              : 72.2
Tacho            : 8
Cycles running   : 3
TIM duty         : 792
TIM val samp     : 421
TIM current samp : 23542
TIM top          : 46242
Comm step        : 3
Temperature      : 25.85
```

---
## \#81 Posted by: JohnnyMeduse Posted at: 2016-11-19T21:33:23.489Z Reads: 342

```
I you feel any resistance, it's probably the motor who's burn (shorted phase)

And also maybe burn the drv
```

---
## \#82 Posted by: rtasca Posted at: 2016-11-19T21:39:38.597Z Reads: 330

```
the motor runs free, it locked while pushing the board unpowered, but then freed again. Its not a deal with other ESCS ive dealt with but IDK if this could have caused the damage.
```

---
## \#83 Posted by: JohnnyMeduse Posted at: 2016-11-19T21:45:55.812Z Reads: 323

```
Ok if the motor run free when unplug... it's maybe one of the mosfet who's shorted... because there no protection against overvoltage, wich can damage the gate of a mosfet.
```

---
## \#84 Posted by: rtasca Posted at: 2016-11-19T21:57:12.645Z Reads: 329

```
It runs free plugged in too. Can the FETs cause DRV faults?
```

---
## \#85 Posted by: JohnnyMeduse Posted at: 2016-11-19T22:02:40.463Z Reads: 332

```
No if it runnig free when plug, it's probably the drv, sorry 😧
```

---
## \#86 Posted by: rtasca Posted at: 2016-11-19T22:41:05.810Z Reads: 316

```
Now it's not giving any more DRV faults, only Under Voltage Fault, motor stutters a bit but doesnt turn. Ordered 3 DRV chips, lets have a go.
```

---
## \#87 Posted by: rtasca Posted at: 2016-11-19T23:03:07.407Z Reads: 319

```
Now I get this Fault            : FAULT_CODE_UNDER_VOLTAGE
Current          : 61.5
Current filtered : 63.1
Voltage          : 7.18
Duty             : 0.28
RPM              : 449.4
Tacho            : 196
Cycles running   : 633
TIM duty         : 3520
TIM val samp     : 1688
TIM current samp : 7977
TIM top          : 12578
Comm step        : 6
Temperature      : 22.90
```

---
## \#88 Posted by: Jinra Posted at: 2016-11-19T23:03:29.681Z Reads: 301

```
yea 7 is definitely undervoltage. Check your cells!
```

---
## \#89 Posted by: rtasca Posted at: 2016-11-19T23:06:44.816Z Reads: 307

```
Cells are good. When I just got it, I could do detection on this motor with a current limited supply no problem. Its sounds fishy that the current goes so high. Something is causing the voltage to drop drastically. The motor spins erratically on KB control. I wanted to try reflashing the FW. maybe, who knows... Funny the DRV faults went away for good.
```

---
## \#90 Posted by: Jinra Posted at: 2016-11-19T23:08:02.320Z Reads: 310

```
It could still be the DRV being broken. Maybe it's not providing the correct voltage which leads to the undervolt error.
```

---
## \#91 Posted by: rtasca Posted at: 2016-11-19T23:34:39.383Z Reads: 309

```
Fumbling around I can  make the motor spin, detection still wont work. The behaviour is very erratic, different from when it arrived... 

stranger things....
```

---
## \#92 Posted by: rtasca Posted at: 2016-11-19T23:55:33.066Z Reads: 312

```
Look what I found:  http://vedder.se/forums/viewtopic.php?f=7&t=487&p=2944#p2939
```

---
## \#93 Posted by: Eboosted Posted at: 2016-12-28T18:02:37.721Z Reads: 299

```
Where are you guys getting your DRV8302 from?
```

---
## \#94 Posted by: raxell Posted at: 2016-12-28T18:46:28.356Z Reads: 304

```
http://www.electric-skateboard.builders/t/vesc-where-to-buy-drv8302-chip/8047
```

---
## \#95 Posted by: rtasca Posted at: 2016-12-29T14:04:45.880Z Reads: 302

```
I have replaced my DRV but it still behaves the same way. Looks like some commutation problem. 

Getting the ABS MAX CURRENT ERRORS. all the time. Motor only stutters.

I have checked the FETS for shorts ( between D and S ) and between G and S... nothing weird. Thinking about removing them for testing on bench. 


Out of ideas here... maybe next is tracing the gates to the DRV..

so frustrating...
```

---
## \#96 Posted by: JohnnyMeduse Posted at: 2016-12-29T14:22:18.037Z Reads: 293

```
Sound like a broken motor...
```

---
## \#97 Posted by: rtasca Posted at: 2016-12-29T14:23:42.300Z Reads: 297

```
No sir, it spins like a boss with my Castle Phoenix 80 HV.
```

---
## \#98 Posted by: JohnnyMeduse Posted at: 2016-12-29T14:49:08.006Z Reads: 303

```
Well regular esc are less sensible than VESC... are you running sensor or sensorless ?
```

---
## \#99 Posted by: chaka Posted at: 2016-12-29T15:23:44.095Z Reads: 313

```
Check all the resistors and caps near the FETs. If your motor cogs without drv errors than you probably have a a poor solder joint somewhere. Look for cold joints and reflow with flux.

http://cromwell-intl.com/radio/nc2030-qrp-transceiver/pictures/qrp-005-009-cropped.jpg
```

---
## \#100 Posted by: rtasca Posted at: 2016-12-30T13:24:46.323Z Reads: 320

```
did so.
reflowed the fets too...
Reflowed the shunts that could be causing the overcurrent issue, no go.
Gonna check cont to the DRV gate driver pin.

It looks clearly that a phase is out of order. 

Not giving up, not yet hahaha
```

---
## \#101 Posted by: JohnnyMeduse Posted at: 2016-12-30T15:51:44.990Z Reads: 332

```
check your shunt... I suggest to reflow them as well, but check them before.
```

---
## \#102 Posted by: mclightning Posted at: 2016-12-30T18:57:23.256Z Reads: 333

```
I think I just killed my VESC completely :frowning: 
I bought a new DRV8302 chip and soldered it. But it just doesn't turn on anymore.

We must note somewhere, this repair work is extremely advanced. I have been involved in electronics hobbies for 6 years now. I have never done SMD before let alone this chip with GND pin underneath the chip.

If you are not experienced and have absolutely right equipment, don't try. Just don't. Buy a new one. 

I feel very upset spending extra to fix it rather than just buying a new one. I spent 70-80 euro on equipment & material and screwed it up completely.

EDIT : IT WORKED! :D I can't believe it. It works. https://www.instagram.com/p/BOp-QMWDTST/
```

---
## \#103 Posted by: Blasto Posted at: 2016-12-30T21:16:07.328Z Reads: 313

```
Good job man, it can be tricky
```

---
## \#104 Posted by: mclightning Posted at: 2016-12-30T21:31:11.188Z Reads: 315

```
Do you have any advice on how to test it to verify the fix?

I connected to BLDC tool, it shows everything fine. No error/fault.
I ran motor from BLDC tool, it seems to spin fine.
Except it did not power on by USB alone. I had to connect Lipo then it is detected on USB.

Solder pads came off for pins 4 , 5  completely.
Solder pads came off HALF for pins 6, 55, 20. But I probed their pathway and they still have connection.
I bridged pin 21 with a thin cable.
```

---
## \#105 Posted by: PXSS Posted at: 2016-12-30T22:15:43.410Z Reads: 311

```
SMD isn't too bad once you get the hang of it...
That's when you can really get crazy with pcb design. 
Glad you fixed it!

Don't you need at least 12v to power it?
I was under the impression that you always had to have it powered and not only usb
```

---
## \#106 Posted by: Blasto Posted at: 2016-12-30T22:30:05.650Z Reads: 312

```
The vesc will not power on w only the usb.

If you are able to run the motor detection, time to test it under stress, slap it in your board
```

---
## \#107 Posted by: mclightning Posted at: 2016-12-31T00:00:10.987Z Reads: 309

```
Great to hear!

Switched to FOC, did motor test (r&l test), stress test riding -> All OK, no problem.

This was most challenging soldering I have ever done.  I cant believe I did it :D
```

---
## \#108 Posted by: rtasca Posted at: 2017-01-02T13:14:48.539Z Reads: 302

```
yes, did that already. 

maybe some FET is not switching ON? can they be tested without desoldering?
```

---
## \#109 Posted by: Moja Posted at: 2017-01-10T16:53:49.299Z Reads: 306

```
I has a small amount of water get into my enclosure, I've cleaned and dried everything. When I power up the VESC the DRV chip gets really hot, and the red led blinks once on startup. I can still drive the Motor but under any load it cuts out and reboots the VESC. 
Any advice? Or is the DRV chip cooked.
In 2 years I think I've blown 7 VESCs with DRV chip problems, so fucking over it, why are they so unstable? Any more of this and I'm outa here, I'll just somehow put 4 years of e-boarding, all the money I've shelled out and the thrills I've had behind me :/
```

---
## \#110 Posted by: Aggdaddy Posted at: 2017-01-10T17:22:51.150Z Reads: 291

```
It seems like most of the problems with vescs is with the drv8302 chip.  How hard would it be to build a socket for the chip, so that those of us without equipment could replace it ourselves?
```

---
## \#111 Posted by: Pantologist Posted at: 2017-01-10T17:41:34.451Z Reads: 294

```
Sounds like a good idea except I that wouldn't last with all the vibrations.
```

---
## \#112 Posted by: JohnnyMeduse Posted at: 2017-01-10T19:31:15.617Z Reads: 288

```
Don't want to burst you bubble, but the drv isn't a thru-hole component, it also need a really good connection over the ground pad at the bottom, wich you won't have in a socket... also it will need double the seize of the actual vesc to get all the connection right
```

---
## \#113 Posted by: JohnnyMeduse Posted at: 2017-01-10T19:32:29.597Z Reads: 288

```
[quote="Moja, post:109, topic:4201"]
I've cleaned
[/quote]

What did you use to clean it... ?
```

---
## \#114 Posted by: Aggdaddy Posted at: 2017-01-10T19:52:33.086Z Reads: 289

```
Why would you be "busting my bubble"?  From the posts I have read, it would seem that many issues revolve around replacing that particular chip.  It would help if it was easier to replace.   

Just throwing ideas out there.  I only know of soldering wires.  I have very little experience with soldering chips on board.  So, if that isn't feasible,  what else could be done to make this vesc easier to repair or less likely to fail due to drv8302 failure.
```

---
## \#115 Posted by: JohnnyMeduse Posted at: 2017-01-10T20:12:20.241Z Reads: 278

```
Well, first option is to buy better quality vesc, second is always be carefull, double check your soldering and make sure that every cable is properly isolate before injecting any power, third double check your parameter inside the bldc tool and never forget to run a motor detection.... and dont use foc unless you have been use to the vesc before. Finaly, Always be cautious... VESC are open source controller, and not a product that was made for a easy use, it is a procduct that is still in developement.
```

---
## \#116 Posted by: Moja Posted at: 2017-01-11T12:59:23.500Z Reads: 270

```
A toothbrush with a small amount of WD40 on it to avoid any corrosion
```

---
## \#117 Posted by: TarzanHBK Posted at: 2017-01-11T13:11:45.507Z Reads: 274

```
sorry but you should´ve learned from that point and buy vescs from good vendors with good known quality and guaranty!
I would have thrown everything over from the, lets say, 3. Vesc? :smiley:
```

---
## \#118 Posted by: JohnnyMeduse Posted at: 2017-01-11T13:48:46.968Z Reads: 285

```
OK, WD40 might be one of the worst thing you can use to clean electronic, because it leave some highly conductive oily residue, that will resistance over all the pcb making it over heat and create over current at some point. It is a long shoot but if clean it using product that a specially made for cleaning electronic (like isopropyl alcohol, flux remover), you might be able to save it (just stop using it until further notice).
```

---
## \#119 Posted by: SORRENTINO Posted at: 2017-01-13T14:02:48.192Z Reads: 280

```
Good solution to making a DRV easier to replace it having the DRV on a separate pcb and that connects to the main pcb say like the chip on an arduino uno. Could that not be possible?
```

---
## \#120 Posted by: JohnA Posted at: 2017-02-09T19:44:59.618Z Reads: 278

```
Would it help save the DRV if you use a 4.7uf Cap instead of the BOM's 2.2 uf in C26? Like @chaka's C18 upgrade? I'm asking because I bought 2 vesc's from TB and want to fill that c26 gap so Foc is less risky.
```

---
## \#121 Posted by: JohnnyMeduse Posted at: 2017-02-09T20:00:26.774Z Reads: 286

```
Yep, you can... If I remember correctly the choice for 2.2uF was made partially for cost reduction.... so 4,7uF should work just fine
```

---
## \#122 Posted by: JohnA Posted at: 2017-02-09T20:03:56.272Z Reads: 297

```
<img src="/uploads/db1493/original/3X/9/2/92bdcddbaeed599d92349ae827ef2f356fce3bde.JPG" width="375" height="500"> On my vesc the c18 and c26 are bridged together, will this be an issue? Should I just add a 4.7uf cap to the c26 side?
```

---
## \#123 Posted by: JohnnyMeduse Posted at: 2017-02-09T20:07:18.576Z Reads: 286

```
C18 and c26 are place in parallel. 😉 Yep, just add the cap and it should be fine
```

---
## \#124 Posted by: michichopf Posted at: 2017-04-26T15:35:08.687Z Reads: 271

```
question, I have a blown DRV. Its an old vesc (orignial raptor 1 version, dont know which one exactly).
I somehow think buying new vesc(s) will be cheaper than to buy all the tools I would need. (given I would even be able to fix it).

Thoughts, Ideas ?
```

---
## \#125 Posted by: Rions Posted at: 2017-05-13T06:46:47.059Z Reads: 253

```
Hi there ,did you end up finding someone to repair the vesc drv problem?if so where and how much please,?
```

---
## \#126 Posted by: treenutter Posted at: 2017-05-13T12:13:43.121Z Reads: 253

```
@Rions I fixed mine myself but I believe @JohnnyMeduse repairs them for a fair price.
```

---
## \#127 Posted by: OskarCastrone Posted at: 2017-05-13T18:11:35.324Z Reads: 263

```
Hey guys
I am unsure if my my DRV chip is fried... There is no sign of any melted plastic or burn marks on the chip but when booting up the VESC, the LEDs flashes red 3 times. I also get an error saying DRV8302. The wierd thing is, this VESC is completely new and would actually make a successful motor detection. After motor detection the motor studdered and would not spin freely. I then connected another motor and same thing - the motor studders. 
Then I switched to yet a other motor and now the VESC will not respond at all - besides the error code "DRV8302" and flashing red 3 times. 
Is this a software problem or is it a blown DRV?
```

---
## \#128 Posted by: Acidfie Posted at: 2017-05-22T18:31:33.987Z Reads: 253

```
Hello there guys,

i have a little problem with my VESC. It once worked until i fucked up the DRV with the current ramp step bug for OS X.

I could connect it but the red led flashed 3 times when i wanted to start the motor detection. So i went to my university and had the DRV replaced with a SMC rework station, but since i did this, it cant be connected to my laptop. "NO FIRMWARE READ RESPONSE".

I tried it with a lab-current source with 15V, nothing. No flashing 3x Red LED at power up/connecting to power. no amps drawn. nothing.

So i checked the voltage at the tc2117. with gnd and 1. pin nothing. 2. pin 0,17V and 3. pin only 1V. 

C31 and C33 had no short. So do i need to reflash the firmware or is the exposed pad on the drv8302 not soldered correct on the board? 

are there anymore things that could be with the board?

best regards, robin
```

---
## \#129 Posted by: hexakopter Posted at: 2017-06-05T21:24:06.208Z Reads: 244

```
Sounds like your DRV isn't soldered correctly. It should output the 5V (build in step down) that goes to the LDO for the 3.3V for the STM32. I have heard that it is possible to also destroy other components when the DRV is soldered without the ground pad connected.
```

---
## \#130 Posted by: JdogAwesome Posted at: 2017-08-09T03:38:28.981Z Reads: 237

```
Hey guys digging up this old thread, but I could use some help on repairing a VESC. Pretty much a friend gave me a VESC that had a blown DRV (burn mark on the top of it) and I have been attempting to fix it. Originally I replaced the DRV modules as well as 2 of the MOSFET's that had a drain to source short which was causing the VESC to dead short when given power. Anyways now the VESC is mostly working, I can connect with BLDC Ackmaniacs software and configure it through there, though when I try to start a motor detection it moves the motor slightly but says it failed. When I check for faults it gives me two of them, the classic DRV8302 fault as well as a couple under voltage faults. I also replaced 3 of the gate resistors because they were burnt as well. And lastly this is the second DRV I put on this board, the first one I thought was badly soldered somewhere that I couldn't see so I just removed it and started over. With this one know the motor at least moves slightly though im still getting these errors. Anyways if anybody has any advise that would be much appreciated. Pics below.
P.S. The 2 MOSFET's with the silver marks in the middle are the ones I replaced.

Edit: Just replaced R51 as it was burnt as well like the gate resistors. Now when I run a motor detection I only get under voltage errors and no DRV errors so thats an improvment, I guess.
<img src="/uploads/db1493/original/3X/3/4/344853ac849f1b33b0efabab1c09391ce1d8a573.jpg" width="690" height="389"><img src="/uploads/db1493/original/3X/b/7/b7cffbfd092c80f715ca78658076b757920f375f.jpg" width="690" height="389">
<img src="/uploads/db1493/original/3X/6/0/600f64c971df8e63d8b22bea16a34fb517545af7.JPG" width="690" height="388">
<img src="/uploads/db1493/original/3X/7/8/78b9adc9574925d80178cab961eb8a697a700fdc.JPG" width="690" height="388">
```

---
## \#131 Posted by: JohnnyMeduse Posted at: 2017-08-09T20:40:44.893Z Reads: 230

```
Can you take a picture of the soldering o. The two shunt 

<img src="/uploads/db1493/original/3X/a/1/a1aa59ca9abe951779f814ee01f53a22a3edfccf.JPG" width="690" height="389">
```

---
## \#132 Posted by: JdogAwesome Posted at: 2017-08-09T20:44:49.933Z Reads: 237

```
Hey Johnny thanks for the reply! Here are some more closeups of the shunts. The soldering around them seems ok to me.
<img src="/uploads/db1493/original/3X/9/4/9447daa7ee7d30355b85064b9ef4f8f56dcd0ab9.jpg" width="690" height="389"><img src="/uploads/db1493/original/3X/6/8/686f9a2efffa10b81799c130e996249cc5ac2703.jpg" width="690" height="389"><img src="/uploads/db1493/original/3X/d/0/d0bbe3b6c6ade04354d361ead9c42f81493f58ce.jpg" width="690" height="389">
```

---
## \#133 Posted by: JohnnyMeduse Posted at: 2017-08-09T20:45:47.084Z Reads: 224

```
Missing the front 😉
```

---
## \#134 Posted by: JdogAwesome Posted at: 2017-08-09T20:47:34.444Z Reads: 235

```
Heres a pic from the front 

<img src="/uploads/db1493/original/3X/b/9/b9683ca14d083b6e4d4b2c1c5733529270a456ac.jpg" width="690" height="389">
```

---
## \#135 Posted by: JohnnyMeduse Posted at: 2017-08-09T20:56:12.056Z Reads: 238

```
[quote="JdogAwesome, post:130, topic:4201"]
I only get under voltage errors and no DRV errors so thats an improvment, I guess.
[/quote]

How do you power your vesc and what are the parameters
```

---
## \#136 Posted by: JdogAwesome Posted at: 2017-08-09T21:03:01.528Z Reads: 238

```
Powering it with a lab bench CC/CV PSU limited to 3A at 25V when motor testing which is more than enough. My VESC settings are below. 
<img src="/uploads/db1493/original/3X/4/2/42f05b75343a325f3248f02a7ccab0fa85c5daa9.png" width="690" height="370">
```

---
## \#137 Posted by: JohnnyMeduse Posted at: 2017-08-09T21:10:59.343Z Reads: 224

```
Can you tel me what is the Voltage on the real time data tab (don't forget to activate the real time data)
```

---
## \#138 Posted by: JdogAwesome Posted at: 2017-08-09T21:42:09.776Z Reads: 238

```
well for me when I go to the Realtime Data tab the voltage is under the bottom of the screen so I cant see it there. However when I type "volt" into the terminal it reads the correct 25V so its not a problem there. Pic below is what I mean
<img src="/uploads/db1493/original/3X/3/1/31c8a2b7bdec3c98f4976cfe67aeb4eba1446e9e.png" width="690" height="370">
```

---
## \#139 Posted by: JohnnyMeduse Posted at: 2017-08-09T22:18:53.929Z Reads: 227

```
Ok, I wanted to check if R3 and  R4 where ok, since you've had undervoltage error.

So I now do beleive that the UnderVoltage error you have are False Undervoltage, It is probably a problem over the DRV, so I can suggest you to recheck for short on the drv, make sure R48 to R51 are at 100ohms, R28-R29-R34-R35-R42-R43 are at 4,7ohms, and the shunt are perfectly solder (in doubt resolder them).
```

---
## \#140 Posted by: JdogAwesome Posted at: 2017-08-09T22:39:08.493Z Reads: 233

```
Yeah all those resistor values are correct, DRV looks fine no shorts. Im starting to think theres a trace or via thats burnt or shorted and is impossible to fix. I think im going to just buy a new VESC. Thanks for the help anyways.
```

---
## \#141 Posted by: hornet90 Posted at: 2017-08-11T12:39:10.664Z Reads: 242

```
Hey do u have any with dvr fault i have a guy here in ireland who has changed chips for me befor
He wants to give it ago cost for u will be just shipping to me
Ill send it back to u for testing
```

---
## \#142 Posted by: scepterr Posted at: 2017-08-13T22:11:04.272Z Reads: 244

```
@JohnnyMeduse hopefully you know, whats the part # for this diode(D4), my fume extractor ate it while I was moving it out of the way to replace all the caps lol <img src="/uploads/db1493/original/3X/2/1/21ffe92dbce2931dd72ac3c72fc90f1d4f266720.jpg" width="497" height="500">
```

---
## \#143 Posted by: JohnnyMeduse Posted at: 2017-08-13T22:34:03.011Z Reads: 241

```
It's a Shottky 60V 2A 771-PMEG6020ER-115 (parts number on mouser)
```

---
## \#144 Posted by: scepterr Posted at: 2017-08-13T22:58:51.087Z Reads: 241

```
Awesome thanks

While I'm ordering parts is there anything I should/could upgrade?
```

---
## \#145 Posted by: perication Posted at: 2017-09-01T08:26:30.048Z Reads: 242

```
Hello,

I have purchased one enertion vesc controller 4.12 version and after setup with 2 lipos 24V, motor has worked one or two spins and then fault DRV8302 has appeard in the pc tool. Temperature of the Mosfet is 29 degrees and the range of voltage is fine too. Can you help me if I'm missing anything important?
```

---
## \#146 Posted by: Deckoz Posted at: 2017-09-01T10:52:13.843Z Reads: 240

```
If I'm not mistaken...these are the ollin ESC upgrades for reliability. I'm sure you can find this info on vedders forum.. 

C1,C8,C9,C39,C40,C43,C44,C49 10uF 50V replaced with 4.7uF 100V

C37,C51 15uF 100v replaced with 22uF 100v

C24,C10,C11,C12,C13,C14,C16,C17,C18,C20,C23,C26,C31,C35,C41,C52,C401 2.2uF 16v replaced with 4.7uf 16v
```

---
## \#147 Posted by: scepterr Posted at: 2017-09-02T03:38:39.557Z Reads: 240

```
Yep got all those, went for the high temp tolerant versions too, don't know if it'll help but it can't hurt :wink:
```

---
## \#148 Posted by: TheCheat Posted at: 2017-09-06T15:14:25.879Z Reads: 236

```
I fried both my VESCs while testing out FOC on my mountainboard. Anybody in San Diego willing to help repair them? If not, what re my options?
```

---
## \#149 Posted by: TarzanHBK Posted at: 2017-09-06T21:46:52.544Z Reads: 234

```
send them to @JohnnyMeduse
```

---
## \#150 Posted by: ugothakd Posted at: 2017-09-11T12:36:28.520Z Reads: 214

```
You can do it yourself too. Drv chips are about $6, order 3 or four and have it. A hot air reflow station is $50 ish on eBay and will serve you useful in many other hobbies. I've never soldered till I replaced my drv and it wasn't horrible
```

---
## \#151 Posted by: vishal_tejwani Posted at: 2017-10-26T20:10:50.705Z Reads: 192

```
finally someone knowing Louis on forum just watching his videos would give soldering practice
```

---
## \#152 Posted by: Eboosted Posted at: 2017-12-15T06:37:37.492Z Reads: 182

```
@JohnnyMeduse how much temp are you ussing to remove the chip from the board?
```

---
## \#153 Posted by: JohnnyMeduse Posted at: 2017-12-15T06:48:42.198Z Reads: 182

```
Around 240C... but if it is lead free it could take up to two minutes to really liquify the tin, using small circle around the chip.
```

---
## \#154 Posted by: proto Posted at: 2017-12-15T07:02:06.068Z Reads: 186

```
Please let me know if you are still willing to do this! I have a bad DRV8302 chip in my brand new torque boards VESC (firm 4.18). I am heading up to LA and would gladly be willing to drop it off along with double what you quoted! Sorry if this isn't a PM, I signed up for the first time after being a long time lurker just to message you. The VESC still operates for the most part.
```

---
## \#155 Posted by: rocka Posted at: 2018-02-07T01:14:38.814Z Reads: 177

```
what temp did you use?
```

---
## \#156 Posted by: JohnnyMeduse Posted at: 2018-02-07T05:44:38.826Z Reads: 171

```
Around 240deg Celsius
```

---
## \#157 Posted by: banjaxxed Posted at: 2018-02-21T14:42:26.631Z Reads: 175

```
I was hoping not to have to visit the DRV8302 failure threads but here I am.

Pair of new VESCs from @Karen_Vanda had them in a box since delivered and just tried to power them up together (over can and powered at same time)

Only one motor spins, the other gives the DRV error fault :frowning:
So seems like I've had success replacing the thermocouple chip on my 3d printer just now & I want to jump straight to the advanced lessons of esk8 soldering.

Tools
Hakko with which I've become very attached to
A butane powered soldering torch Iroda Solderpro 120, which could be used as a heat gun since it has a torch tip
Infrared thermometer with location laser
Amtech flux RMA-223
Cored solder

Would it be a lot easier to use the torch and get some solder paste?

I've seen a couple of vids and this one seemed to meet success even though to me looks done ham-fistedly
Pros and cons of each method? Do I need solder paste? I have zero smd soldering experience

https://www.youtube.com/watch?v=A_OV0sXtbrY
 

https://www.youtube.com/watch?v=qeWzP2YahNc

https://www.youtube.com/watch?v=opdrL_02VL8
```

---
## \#158 Posted by: banjaxxed Posted at: 2018-02-21T18:31:32.063Z Reads: 165

```
@Karen_Vanda how'a my warranty?😂
![IMG_8538|666x500](upload://gOKHO0ZGLQTt539PGByWt3yluNS.JPG)

Nb. Plastic does not like my improv heat gun
```

---
## \#159 Posted by: banjaxxed Posted at: 2018-02-21T18:48:14.763Z Reads: 163

```
Better pic is this ok to mount a new chip? See any damage apart from the pin port holders?
![IMG_8542|666x500](upload://dUDU6dPyVN99PJNqhBicvGG3Kso.JPG)
```

---
## \#160 Posted by: b264 Posted at: 2018-02-21T18:50:27.921Z Reads: 154

```
Take the plastic off by pulling it over the pins before soldering
```

---
## \#161 Posted by: banjaxxed Posted at: 2018-02-21T18:55:34.220Z Reads: 155

```
that would be the next one, I'll get there thanks for the advice
```

---
## \#162 Posted by: PXSS Posted at: 2018-02-21T19:24:15.485Z Reads: 158

```
I would not use a butane torch as a heat gun. You will ruin the components with the open flame if not possibly the pcb.

Buy one on amazon for like $30
```

---
## \#163 Posted by: banjaxxed Posted at: 2018-02-21T20:08:15.603Z Reads: 158

```
It's a butane powered soldering iron, there is no flame

https://www.maplin.ie/p/pro-iroda-solderpro-120w-gas-soldering-iron-kit-n15ar
```

---
## \#164 Posted by: SOICDIP Posted at: 2018-02-21T20:12:37.087Z Reads: 161

```
[quote="banjaxxed, post:163, topic:4201"]
It’s a butane powered soldering iron, there is no flame
[/quote]

The downside is that you don't know the temperature of the hot air. It may be too hot or too cool. It's unlikely that you'll damage components, but just be mindful of that.
```

---
## \#165 Posted by: banjaxxed Posted at: 2018-02-21T20:19:21.464Z Reads: 160

```
Yeah I tried holding the temp meter and soldering torch but too difficult so I switched to a regular iron after the ground pad was hot enough and did the legs that way.

Couple of drv8302 on the way, I am considering getting solder paste for the new chip it just looks so much easier, plus I don't think you can do the ground with a heat gun of some kind, presumably you can't apply the tip of a soldering iron directly to the chip?
```

---
## \#166 Posted by: zepton Posted at: 2018-04-27T01:14:18.090Z Reads: 132

```
I just got a DRV8302 fault when I switched my board to 9S (I just plugged in the batteries on the bench I didn't ride it. It works perfectly fine with 6S, and when I switched back from 9S to 6S it worked as usual...anyone else have this issue?
```

---
## \#167 Posted by: Deckoz Posted at: 2018-04-27T01:28:52.040Z Reads: 132

```
Settings please @zepton

Post screenshots
```

---
## \#168 Posted by: zepton Posted at: 2018-04-27T01:51:05.950Z Reads: 150

```
I am using ackmaniac's modified 2.54 firmware...are there any settings that I have to adjust when I increase the voltage?

![03 PM|690x418](upload://5cImvvenuoUhHDAwqBb4G2MptZL.png)![08 PM|690x418](upload://pAKJ7qB22miFUkkoIpEIgNVse3U.png)![22 PM|690x418](upload://cX3LBR0KhZObYtD1f5qkJ4qIQSF.png)![20 PM|690x418](upload://nYx2PzRiNfnluXOcHIpvGVPf4gw.png)![29 PM|690x418](upload://yvb8zCUK0bEmHDCVP27TUBl2z26.png)![25 PM|690x418](upload://bRtQ5Ucqt6a3D2TiMtND4zbFWZO.png)![11 PM|690x418](upload://k2jmrPJ6Akp8LiUgHDTTPFrHTLP.png)![33 PM|690x418](upload://gRzo2kTLgBfFkzMYh9ZdAfFa3G.png)![35 PM|690x418](upload://uRYeGQs7zxoYywj7xp3VJCsMkNc.png)![45 PM|690x418](upload://rW7DH3l06oAEHSvFl6TqWsJRfix.png)![38 PM|690x418](upload://bDhAJsNFBp0cT0QOaUUc8aKBwht.png)
```

---
## \#169 Posted by: gstpierre Posted at: 2018-04-30T13:25:32.712Z Reads: 128

```
From what I've heard around here, never change your max input voltage. The vesc gets unhappy when it's changed from 57v. Also your ERPM is way too high, focbox limit is around 100k, and you have double that in your last screenshot.
```

---
## \#170 Posted by: Martinsp Posted at: 2018-04-30T13:43:33.400Z Reads: 134

```
In your case what @gstpierre would not do much, it seems like you are using 6S battery so the max voltage will be 25.2 +some during braking. The +some depends on how hard you brake, on 6S you will not get near 50V anyway so if it means you would have to disassemble your board, it is not worth the hustle. You will not brake it with having it 50 instead of 57 on 6S.

But generally speaking he is correct, no you should not change the max input voltage from the default 57V.

[quote="gstpierre, post:169, topic:4201"]
Also your ERPM is way too high, focbox limit is around 100k, and you have double that in your last screenshot.
[/quote]
if you are talking about the nunchuk settings, it should not matter either since he is using "PPm and UART" control
His erpm are limited in the motor config tab to 60k and -100k but keep in mind he is not using reverse. Having these values set to below 60k in both + and - will protect your VESC but it is a good idea to have tha erpm limited in the ppm "soft rpm limit" setting to a little lower than 60k. I use start at 57k and end at 58k on my daily with 10S and 245kv without problems.
```

---
## \#171 Posted by: zepton Posted at: 2018-04-30T14:27:12.840Z Reads: 131

```
Good to know. What is the difference between the ERPM setting in the PPM window versus the motor window versus the BLDC window? And my max ERPM at 9S would be 50,803 (4.2 volts* 9 cells* 192kv * 7 poles)  =  50,803. Since this number is a lot lower than my settings would it even make a difference? (my ERPM at 6S is 33,868)

When I bench tested my board at 9S, as soon as I tried using my throttle the Vesc blinked red and I got the fault, but it still worked when I went back to 6S. I am a little worried to try 9S again in case my Vesc actually breaks.
```

---
## \#172 Posted by: Martinsp Posted at: 2018-04-30T14:45:51.637Z Reads: 139

```
In that case, I would uncheck the "limit erpm with negative torque" because having that checked would brake rapidly when you reach the set erpm. The soft erpm limit as the name implies will limit the erpm just as well but it wont lock the motor but will increase braking force as necessary to limit the erpm when there is "external" force spining the motor for example going down hill. You will not reach 60k on your setup even with 9S because calculated is with no load, with load you will be lower than the calculated value. It is better to set the soft erpm limit regardless, just to make sure you dont break stuff in case.

Faults like yours that occurs at 6S usually are just a warning before total damage. But that is not always the case, I have had a drv fault when bench testing my vesc two years ago, it was intermittent on 10S and after some help from forum members I got it running and it worked for a year, then my board fell into a river which... well... did not survive :D So I would just keep riding on 6S if you are not getting faults or weird behavior that would make it unsafe in any way and see. If you are getting faults or want to upgrade the setup to higher voltage you will most likely have to replace the chip :/ 

Or maybe if you want to try it you can save your configuration that you have right now, upload fresh firmware, read default config, set up motor detection and soft erpm limit to say 55k end and start to 51k and test your setup on the bench try to reproduce what happened when you had the fault last time. This will either work and reveal that there was some fault either with settings or with maybe corrupt firmware, or it will give you the fault and in that case it would mean that it is the chips fault. I cant guarantee that it will not destroy the chip during testing, but as of right now it seems like the chip may fail eventually on its own anyway... you will have to decide for yourself, depending on time or budget to fix the vesc in a bad case or other stuff
```

---
## \#173 Posted by: gstpierre Posted at: 2018-04-30T17:32:40.333Z Reads: 133

```
Listen to this guy^^^
He's a big shot round these parts, I'm the guy who keeps blowing up his vescs. Thankfully I'm learning thanks to guys like him.
```

---
## \#174 Posted by: Lambjr088 Posted at: 2018-07-30T16:50:23.721Z Reads: 105

```
So i have been searching but it seems I cant find any drv8302 chips. Any one know if they r back in stock? Ive check but nothing maybe a different site
```

---
## \#175 Posted by: xilw3r Posted at: 2018-08-02T05:49:42.558Z Reads: 97

```
They are available on mouser and farnell at the moment.
```

---
## \#176 Posted by: luis99945 Posted at: 2018-11-22T20:40:16.516Z Reads: 62

```
I have a drv fried tb vesc I can sale it for 30usd
```

---
## \#177 Posted by: SkateYS Posted at: 2019-01-09T22:56:09.230Z Reads: 53

```
Hi, any tips for replacing drv?? I attempted twice but both failed LOL.
```

---
## \#178 Posted by: akhlut Posted at: 2019-01-09T23:07:31.720Z Reads: 50

```
call the wizard!

@JohnnyMeduse
```

---
