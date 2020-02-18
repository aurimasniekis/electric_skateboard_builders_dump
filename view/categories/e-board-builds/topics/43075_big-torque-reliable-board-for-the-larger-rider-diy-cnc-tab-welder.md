# BIG TORQUE - Reliable board for the larger rider + DIY CNC Tab Welder

### Replies: 133 Views: 9918

## \#1 Posted by: ducktaperules Posted at: 2018-01-07T13:40:45.065Z Reads: 901

```
Im just starting my first eskate build. Im a big guy (145kg) that wants a reliable board to commute around my small hilly English town. After having issues finding any boards from well known brands that would officially support my weight and hearing stories of axles snapping i decided to go the diy route. 

The plan is to create a cruising board with super torque. Not looking to break and land speed records here, its just got to haul my fat ass about. I am kind of aiming towards the look of the Evolve GT or some of the kaly.NYC street boards.

I started with a 6374 190kv motor from STREET WING but made sure to buy equipment that is wide enough to accommodate dual drive. I also spent a long time looking for a good deck that will have the right amount of flex for a larger guy (http://www.electric-skateboard.builders/t/heavy-duty-decks-for-large-guys/37012/30). 

I ended up buying a Trampa Ultimate Street Carver. I went for the 16 ply deck with titanium axles and king pins. I also ended up also buying the 13/37 pulley set, belt and motor mount from trampa. 

Bodged all the parts on for a quick test drive:
http://www.electric-skateboard.builders/uploads/db1493/optimized/3X/9/1/9144e962ec3ab2edd00483d757912cca7b9d759f_1_666x500.jpg

Its Fucking Solid. Turns super easy and has a little flex but feels indestructible. I dont think i could ever break it and i feel like i could really throw it about without worrying about damaging it. 

Super hype. Time for some temporary waterproofing:
https://photos.app.goo.gl/ycNk4wpbwqPIgGBF2
Yes . . . those are Chinese takeaway containers.

At the moment i dont have any proper batteries so im currently reusing some miniquad lipo's that i have laying round. these are 4s 100c 1300mah and im using 3 of these in series to run at 12s. They perform surprising well and i get about 1.7 miles on a set which is enough to get me to work and up some big hills. im sure i would get much more distance on flat ground but i dont have any to test on :unamused:.

Short video of it working :
https://photos.app.goo.gl/3uBxMSh0KlpHfTyo1
```

---
## \#2 Posted by: Bor.inc Posted at: 2018-01-07T13:56:12.958Z Reads: 778

```
whats the name of the deck? (with those sharp angled truck holders)
```

---
## \#3 Posted by: ducktaperules Posted at: 2018-01-07T14:11:49.276Z Reads: 796

```
2 months later . . .

I have been riding the board in its current state to work most every day and here are my thoughts:

1. 6374 is more than enough torque for any beginner. It takes me easily up the hills i thought i would struggle with. The problem that im having with this setup is grip. 1 wheel is not enough contact with the ground when your trying to transfer that much torque to the ground. As soon as i go over wet / moss / metal covers the wheel just spins up which causes momentary lack of power. I think its time for DUAL :grin:

2. loving the Trampa board however as im getting more confident and faster im starting to find that it is a bit loose on he turning. To combat this i added some red Trampa dampers to my next order.

3. Make sure you lock-tight the shit out of everything. lost a few of the nice trampa grub screws and a few other bolts before i realised this. Even the parts that come pre-assembled from trampa like the screws that hold the springs in the trucks, you will loose them unless you lock-tight them yourself.

4. Switching lipo's all the time and charging them on a lipo charger is becoming a ballache. Its worked well and it does the job but chargeing them is so much effort that i cant be bothered with.

Upgrade Time:
I Purchased a second 6374 motor and FOCBOX to upgrade to dual, mostly for more grip . . . . but im not going to complain about the extra power :wink:. Now that im running dual FOCBOX's i guess i should make a little more effort to waterproof everything so i got some real resealable sandwich containers to store everything in. Also added antispark xt90 and made up some stainless steel support bars to go between the motor brackets for added strength.

https://photos.app.goo.gl/VMH4rf0nttoLK9XF3

Containers were modded to allow mostly watertight connections to motors.

https://photos.app.goo.gl/4PIJAwArlHmAxCKk1

Power is insane. Have not yet been able to go full throttle and the board doesn't even notice hills any more. It accelerates me faster than i thought was possible. I dont know how any normal size rider would be able to use this much power.
```

---
## \#4 Posted by: ducktaperules Posted at: 2018-01-07T14:14:00.130Z Reads: 714

```
All Trampa decks are like this. The sharp angles are required for there trucks to work as they don't have a standard angled kingpin.
```

---
## \#5 Posted by: Bor.inc Posted at: 2018-01-07T14:29:55.820Z Reads: 698

```
but does that deck work for normal trucks too?
```

---
## \#6 Posted by: ducktaperules Posted at: 2018-01-07T14:40:00.051Z Reads: 694

```
Works with any other Mountain board or channel trucks. I have seen people fit angled risers to use normal skate/longboard trucks before
```

---
## \#7 Posted by: Bor.inc Posted at: 2018-01-07T14:56:59.628Z Reads: 681

```
ooh okay, but can normal trucks go on the deck without those angle risers? or where can i find it out on internet?
```

---
## \#8 Posted by: ducktaperules Posted at: 2018-01-07T16:24:38.968Z Reads: 696

```
Lets Talk Batteries:

I have acquired some recycled VTC4 18650 cells from a skip. The cells are pre-made into 6s1p packs which look like they will hold up well to vibration and abuse. I built a capacity tester and tested the packs to find the best ones to use. Im measuring about 38Wh per pack which seems reasonable for these cells as there theoretical max should be about 44Wh (22.2v*2000mAh). Im asuming this difference is due to the conservative battery cuttof with the BMS that is built into the packs.

I am planning on wiring these up to make 2x 6s3p packs which i can run in series to give me 12s3p total. After the capacity test i have also removed the built in BMS's as i am replacing this with a 12s 80A BESTECH BMS with anti-spark.

At the moment i cant decide about how to arrange the battery's under the board. Im planning to make a kaly@nyc style battery tray that goes underneath however due to the size of the packs im not to sure how to lay them out.

One row of Six :
https://photos.app.goo.gl/SVOSjRmcJ2inIYmx1
https://photos.app.goo.gl/rmqEB2gvOso2iOll2

Two rows of Three :
https://photos.app.goo.gl/p5ytKRozpj68p5W53
https://photos.app.goo.gl/oHUEKcJXGDmmc5t73

Im thinking the longer thinner pack will give more flex however it may be more difficult to vacuum form due to the smaller gaps and harsh edges between the packs. Also the length is concerning as i need space for 2 FOCBOX's at the back and whatever other charging ports and power switches i decide to add.

Any thoughts anyone?
```

---
## \#9 Posted by: ducktaperules Posted at: 2018-01-07T16:58:09.506Z Reads: 649

```
Started mocking up what the "One row of Six" pack might look like.

<img src="/uploads/db1493/original/3X/7/d/7d4a1950cd5d20d4ddb58d93cb0741227cacbe53.jpg" width="690" height="360">

<img src="/uploads/db1493/original/3X/f/9/f9da96563513cf0c73257136c2c09ed9a1418961.jpg" width="690" height="491">

This has 10mm between the packs but i think that it will be hard to get a good mould of this area from the vacuum former, especially if i try and use a thicker material. I could separate the packs slightly more but im concerned about weather it will even fit on the bottom of the board. Space is already very tight around the FOCBOX and BMS and i haven't left much space for other things like charging port or power switch.
```

---
## \#10 Posted by: mikenyc Posted at: 2018-01-07T17:44:06.989Z Reads: 618

```
These packs are interesting. Do you know who makes them?
```

---
## \#11 Posted by: ducktaperules Posted at: 2018-01-07T19:15:42.696Z Reads: 612

```
They are replacement packs from cordless vacuum cleaners. I guess they use quality cells so that they can produce enough current in higher power modes.
```

---
## \#12 Posted by: ducktaperules Posted at: 2018-01-07T19:25:41.007Z Reads: 640

```
I also started mocking up what the "two rows of three" pack might look like.

<img src="/uploads/db1493/original/3X/d/8/d8945fbfdba2cc4ca00c6e38e22cc320c0c3d2bf.jpg" width="690" height="373">

<img src="/uploads/db1493/original/3X/a/3/a3363d4011d7b5af4b9b83ff0da8129127bdbd8c.jpg" width="690" height="373">

I think this would be far easier to vacuum form but i wonder if it would still have enough flex.

Any thoughts?
```

---
## \#13 Posted by: ducktaperules Posted at: 2018-01-14T22:18:24.287Z Reads: 630

```
PROGRESS REPORT:

Over the last week i have been trying to recreate some of the Trampa and parts in Fusion 360 as i eventually plan on building custom cable risers and motor mounts for them. 
![testbuild2 v4-3|690x413](upload://r4zD6u3wjNg4d0XbGI4iqrPxzoC.jpg)![test build v4-1|690x413](upload://mNTgOkkNipTmz8XfpsRdGpNWhhF.jpg)

Motor mounts are Still a work in progress but the plan is to lift the motors higher giving more clearance and better access to the grub-screws that hold the mounts to the axles.

![TestBuild3 v5-mounts|690x373](upload://atTvHRLfC0AhLaouxnM5vSxQv9u.jpg)

I Also found time this weekend to finish wiring the battery packs up into 2 x 6s3p Packs that i will run in a 12s configuration.

![IMG_20180114_171132|666x500](upload://vjP2ge4aIJjNGKIAirsUUaE8bo1.jpg)

Just need to finish refining smaller details on the enclosures before i fully commit and start the CNC'ing.
```

---
## \#14 Posted by: pixelsilva Posted at: 2018-01-14T23:03:30.203Z Reads: 612

```
...this enclosure looks familiar.... :smirk:

![image|690x360](upload://dAoSsR07dbzFUy8EJOfTJvoKhqn.jpg)

![image|690x491](upload://9zLT757qzflj3fGkK0gjkDTJaeM.jpg)
```

---
## \#15 Posted by: pennyboard Posted at: 2018-01-14T23:20:21.199Z Reads: 577

```
Looks like a really great build so far. Make sure you're careful with how you route wires between enclosures, I seem to recall @Eboosted having his board catch fire in a similar set-up, but I'm not sure if they ever determined the exact cause.
```

---
## \#16 Posted by: ducktaperules Posted at: 2018-01-14T23:26:49.361Z Reads: 568

```
Why? What other enclosure is it like? I have not seen anything which is that similar other than it is segmented like almost all trampa enclosures. I would be interested to see :slight_smile:
```

---
## \#17 Posted by: ducktaperules Posted at: 2018-01-14T23:31:16.828Z Reads: 568

```
Yeah everything is going to get a good helping of hot glue to remove all unwanted cable movement and add some extra insulation. Also there will be stress relief Bends in wires between packs when fitted.
```

---
## \#18 Posted by: pennyboard Posted at: 2018-01-14T23:32:38.159Z Reads: 590

```
Here's the link to the thread
http://www.electric-skateboard.builders/t/my-trampa-caught-fire-last-weekend/35012/79
```

---
## \#19 Posted by: Pedrodemio Posted at: 2018-01-14T23:32:54.659Z Reads: 574

```
Beautiful board and nice cad work

On the new battery, how thick are the nickel strips that you are soldering to the wires? depending on how much current you plan to pull they might not be enough and get very hot or melt altogether
```

---
## \#20 Posted by: lock Posted at: 2018-01-14T23:44:12.798Z Reads: 573

```
I thought about CAD'ing up the Trampa trucks, but stopped myself once I realised how long it would have taken. Model looks great dude!
```

---
## \#21 Posted by: ducktaperules Posted at: 2018-01-14T23:45:05.462Z Reads: 545

```
I don't know how thick the nickel strips are but they are designed to handle the full 30A that each 6s1p pack can provide. I did not weld the packs myself, they came pre welded in this configuration inside the tools I salvaged them from. 3 Packs are then wired in parallel direct to the 10AWG cable. This settup should easily be good for 90A. It will connect to a 80A bestech bms. I don't think current handling will be a problem
```

---
## \#22 Posted by: E1Allen Posted at: 2018-01-14T23:54:04.777Z Reads: 546

```
Good looking board and battery use
```

---
## \#23 Posted by: pixelsilva Posted at: 2018-01-15T08:07:20.368Z Reads: 558

```
....presents some similarities with the Slick Revolution enclosure....... :point_down:

![image|690x459](upload://qAFIqhywgErR3f4lbN2VLZvC8X3.jpg)
```

---
## \#24 Posted by: ducktaperules Posted at: 2018-01-15T08:11:19.130Z Reads: 538

```
Hmmm interesting, wonder how they lay there cells out inside. Also wonder if there replacement packs would fit a Trampa board. Could be a nice solution for builders who don't have access to equipment
```

---
## \#25 Posted by: ATLesk8 Posted at: 2018-01-15T19:55:42.086Z Reads: 524

```
I've seen these around Amazon and Instagram, but I've still yet to see one in person. How do all these esk8 companies stay in business if they don't have a product to sell? Kickstarter is a sham
```

---
## \#26 Posted by: ducktaperules Posted at: 2018-01-15T20:05:21.642Z Reads: 506

```
I have a friend that has a board from this company and its not that bad. 
He has this one: https://www.slickrevolution.co.uk/dual-max-eboard-spec/
Its not as powerful as a boosted dual+ but it does the job for a lot cheaper. It feels very tall when you ride it and the lack of flex is noticeable but otherwise it looks well built.
```

---
## \#27 Posted by: pixelsilva Posted at: 2018-01-15T20:46:17.421Z Reads: 499

```
Is a british company. Perhaps their currency, the pound, and a different economy which affects them in a different way. Who knows??
```

---
## \#28 Posted by: halifax21 Posted at: 2018-01-16T00:56:24.112Z Reads: 494

```
Yeah man, I'm 127kg and i built my Trampa just because no other production ready board was useable, but now I'm switching to the mountain board deck because it's wider so my feet aren't hanging off the edges a lot and a bit longer.
```

---
## \#29 Posted by: ducktaperules Posted at: 2018-01-20T18:24:22.499Z Reads: 533

```
Update:
I have been very slow about finishing the enclosure design. I have changed my mind multiple times about how im going to layout the electronics. So that this does not hold up progress i have decided to make the battery enclosure separate to the the electronics enclosure.

Final Battery Enclosure:
![JustBatteryEnclosure v7|690x373](upload://tkbxdpSzhKKDG7KZDjq4vgqMzvL.jpg)
![JustBatteryEnclosure v7-1|690x373](upload://eZFdLQK7Jr0evDMPJuWLdF1ygmL.jpg)

Buck to CNC that will go in the vacuum former:
![JustBatteryEnclosure v7-3|690x373](upload://oZfolupEsRlfDeSRwCjQsOfnETg.jpg)

Hopefully i get time to CNC this and vacuum form this week :) then at least i can start using the battery even if im still having to charge it on a balance charger.
```

---
## \#30 Posted by: ducktaperules Posted at: 2018-01-25T18:54:10.834Z Reads: 525

```
SHITSGETTINGDONE UPDATE:

Got some CNC time and was able to get the buck made. Looks great. Super happy with it so far.

![IMG_20180124_132742|690x458](upload://s5somtW8EYpLizaAOg779ReGbL3.jpg)

Next job was to put the in the vacuum former. luckily I have a friend with some experience in doing this who offered to help me. I decided to try and use some 3mm poly-carbonate as i assumed that this would be strong and impact resistant.

![IMG_20180124_192459|689x500](upload://ggyH9XxVgnJk4Si4ybYzvFZqVmx.jpg)

So what happened? 

Basically the part got stuck on the mould. I learned 5 lessons from this:
1. Poly-carbonate is way stronger than i expected. It bends when in a flat sheet but as soon as it has shape it's super rigid.
2. You should put a small taper on every vertical surface. I thought i would be ok without tapering the sides of the packs . . . I was wrong. 
3. Take off the protective plastic. This seems to have melted in some areas basically gluing the plastic to the buck.
4. Poly-carbonate can absorb moisture, when heated this causes the bubbling you can see. To avoid this it should first be dried out in an oven. 
5. If your having issues getting the the buck and the poly-carbonate apart again then Don't **smash it on a table**. This will not help you but instead lead to incredible frustration. Furthermore you are likely to hear a large cracking sound, followed by the feeling of dread, then finally the realisation that you have broken the buck.

We had to cut the poly-carbonate off in the end. Then began a long and tedious job of repairing the damage to the buck. My friend helped me sand off all the melted plastic, glue things back together and filler the damaged areas.

![IMG_20180124_200020|690x409](upload://vCOZFmnWm1PcOe1ORLzcB6wn97I.jpg)

Ready for round 2. This time we decided to switch to 2mm PETG as this should be more flexible and hopefully be easier to remove.

![IMG_20180124_204725|666x500](upload://maudNCg8R9qAXCX4K9VRFuNb4MZ.jpg)

SUCCESS :smile:  

This time it released much easier and seems to have come out pretty good. There is a small amount of "webbing" in a few places between the battery's however i dont think it notices much and it shouldn't affect the performance so i think it will be ok. I haven't had time to tidy up the edges yet however i decided i should probably check it fits on my board before i invest to much effort into tidying it up.

![IMG_20180124_224214|666x500](upload://bcrCrpFZOUuuBelviNMlOJAjFmy.jpg)

Also the battery's look like they fit perfectly.

![IMG_20180124_223747 (1)|690x141](upload://twBKYBvYVukhPeYfFdkXN6WoulQ.jpg)

Overall im pleased with the result. Next job is to clean up the edges, Paint it from the inside & order some mounting hardware.

 PS. I have a new appreciation for how professional some of the other enclosures in the forum are.
```

---
## \#31 Posted by: MasterCho Posted at: 2018-01-25T19:07:07.565Z Reads: 490

```
Looks great!   What's the "Buck" made of?   is it durable to be CNCed as a mold?
```

---
## \#32 Posted by: ducktaperules Posted at: 2018-01-25T19:25:10.673Z Reads: 495

```
The buck is made form Ureol. Its polyurethane like Material, almost like a super high density foam. It is often used for making prototypes or models. It cuts very easy on the CNC but is very strong and gives a good finish. cuts like this https://youtu.be/yCufLWWNTiM?t=45
Just happens to be what i had scraps of avalable. 

Also "Buck" is what you call the piece you make a Fiberglas mold from. i dont know if its still the correct term for vacuum forming but im using it anyway :smile:
```

---
## \#33 Posted by: MasterCho Posted at: 2018-01-25T19:39:39.841Z Reads: 483

```
I was asking because I am thinking of CNCing a mold from the CAM program directly, I would use High Density Polyurethane but isn't commercially available the size I need or it's damned expensive. Thanks for the link  I'll look it up.

Yeah,  now I know people call it "plug or buck"
I am not even sure if I spell "mold " right   some people call it " Mould"
```

---
## \#34 Posted by: BigBrit Posted at: 2018-01-25T19:44:25.339Z Reads: 476

```
Keeping an eye on this thread, looks great!
```

---
## \#35 Posted by: ducktaperules Posted at: 2018-01-25T20:02:21.074Z Reads: 492

```
Try googling modelling board, comes in almost any size. 

The most dense stuff has a great finish and you can make molds to cast parts from. http://lcamtuf.coredump.cx/gcnc/cb-silicone.jpg

The lower density stuff is often used for large scale surface modelling
http://www.premierpatterns.com/files/cache/d9648ad2540a5a628661b81f81a7979e_f64.png
https://www.rqriley.com/images/xr3foam2-big.jpg
```

---
## \#36 Posted by: pixelsilva Posted at: 2018-01-25T22:03:45.578Z Reads: 478

```
This is what I was looking for! The shit is what I need for Kydexing my enclosure. :star_struck: :+1:
```

---
## \#37 Posted by: ArnhemAnt Posted at: 2018-01-26T03:25:14.307Z Reads: 472

```
Great for you to be able to share how your build is evolving. Love the new enclosure - very nice work man.
```

---
## \#38 Posted by: ducktaperules Posted at: 2018-02-01T20:34:51.823Z Reads: 496

```
SHITSGOINGTOGETHER UPDATE:

Holes marked and drilled . . . Check.
Battery packs fitted . . . Check.
Wiring adjusted and tidied . . . Check.

![IMG_20180130_234141|666x500](upload://rwPAmrqh3OZPPY6bJSI4xs2qFQn.jpg)

Board marked and drilled . . . Check.
Brass threaded inserts Fitted  . . . . erm . . . . uhhhhhh. . . . . . . . . Check.
EPDM Seal Cut . . . Check

![IMG_20180130_223029|666x500](upload://9qI2V5crFr1Tg7OOMyXzWVTiKOO.jpg)

Cover everything in Hot Glue so nothing Rubs . . . Check & Double Check
Kapton all loose wires down . . . Check
Get ready to awkwardly put both half's together . . . yep

![IMG_20180131_211526|690x368](upload://vhrpni56IPicIsb6Tmqrubzx8R4.jpg)

Lift . . . 
Flip . . . . . 
Bolt everything together . . . . . Check

![IMG_20180131_212532|666x500](upload://5V3CZclhWsxoldR8dd3RYSkPakR.jpg)

Finally Ready For a test ride :smile:
```

---
## \#39 Posted by: FredrikHems Posted at: 2018-02-01T20:37:46.782Z Reads: 487

```
Looking sweet! What configuration is the batteries in?
```

---
## \#40 Posted by: ducktaperules Posted at: 2018-02-01T20:43:18.527Z Reads: 492

```
They are 12s3p but unusual in that each cell in a parallel group is in a different pack.
```

---
## \#41 Posted by: ducktaperules Posted at: 2018-02-08T00:21:39.297Z Reads: 483

```
Just been thinking how awesome some trampa cable risers would be.

![riser v2-1|690x360](upload://3F7vTMt4CkXOSYkkNwvRjvsJfOg.jpg)
![riser v2|690x360](upload://8oW3hNQEUks9r8UD2JhwA4mviEJ.jpg)

Thoughts?
```

---
## \#42 Posted by: mikenyc Posted at: 2018-02-08T00:34:43.016Z Reads: 463

```
Surprised it hasn’t been done yet
```

---
## \#43 Posted by: Riako Posted at: 2018-02-08T23:41:09.482Z Reads: 454

```
Gorgeous !!!
```

---
## \#44 Posted by: lock Posted at: 2018-02-09T03:22:43.521Z Reads: 452

```
Almost did this, but I won't be routing my motor cables that way so opted against. Of course I only later realised that I still need to run the power button / battery display into the middle of the truck base plate.

You'll need longer bolts to mount the trucks, but that's hardly an issue.
```

---
## \#45 Posted by: Rob69de Posted at: 2018-02-09T18:43:13.225Z Reads: 444

```
If you made those risers with wire channels I would buy them👍
```

---
## \#46 Posted by: JonathanLau1983 Posted at: 2018-02-09T19:26:48.388Z Reads: 441

```
Those truck risers look awesome! Is the Trampa outer layer carbon fibre? Be careful!
```

---
## \#47 Posted by: ducktaperules Posted at: 2018-02-11T10:08:26.973Z Reads: 438

```
No it looks like it but its more like fibreglass. Its not conductive (i checked a lot before mounting my batteries)
```

---
## \#48 Posted by: ducktaperules Posted at: 2018-02-22T22:36:54.624Z Reads: 436

```
Currently borrowing a small desktop cnc :) 

While i finish designs for my enclosure i decided to make some random shit. This is first time i have used CAM before so im learning a lot about milling techniques and just trying to get a feel for what the machine is capable of. Im hoping to try and cut some aluminium eventually but in the mean time im using scraps of acrylic.

![IMG_20180222_221311|690x390](upload://nMLOpCnBgWg177lCIMiqdeQ6aAu.jpg)
Dual Focbox Heatsync @Kug3lis style ? 

After cutting this i realised that i should always check the cutting bits are in the correct box (this cutter was larger than i thought so all my dimensions are slightly wrong).

The CAD is based off the original heat sync and i just duplicated it. After cutting i realised that @Kug3lis design (http://www.electric-skateboard.builders/t/dual-focbox-fully-enclosed-cnc-machined-case/42321/89) is very clever and has a few small changes that would make it far easier/quicker to machine. i guess i have changes to make before trying again :grinning:
```

---
## \#49 Posted by: GrecoMan Posted at: 2018-02-22T22:41:19.404Z Reads: 413

```
can you mill aluminum?

oh wait, just read it 😜
hit me up if you want a quick project 🤟
```

---
## \#50 Posted by: ducktaperules Posted at: 2018-02-22T22:49:28.005Z Reads: 406

```
Well i think aluminium is on the edge of my machines capabilities but if im feeling brave i may give it a go. I dont want to push things to hard cause its not mine and i dont want to break it :worried: Also i only have it for a limited time and i already have a butload of things i want to make.

That said, if it goes well and proves to be useful i may buy one the same or similar. If this happens i will let you know :slight_smile:
```

---
## \#51 Posted by: FredrikHems Posted at: 2018-02-22T23:04:41.520Z Reads: 400

```
May you share the name of the CNC? :grinning:
```

---
## \#52 Posted by: topcloud Posted at: 2018-02-22T23:13:56.406Z Reads: 406

```
Extraordinarily helpful, thank you!
```

---
## \#53 Posted by: ducktaperules Posted at: 2018-02-22T23:35:41.670Z Reads: 423

```
Its a "3020T", don't know the company but its some cheep chinese machine. They can be acquired for around £300.

![IMG_20180222_213350|666x500](upload://vsPa7o15qx6xJvyoLM62qMCxFoK.jpg)
```

---
## \#54 Posted by: FredrikHems Posted at: 2018-02-22T23:44:38.630Z Reads: 422

```
That stepper looks so freakin big wtf, haha
```

---
## \#55 Posted by: ducktaperules Posted at: 2018-02-24T18:31:42.670Z Reads: 426

```
Just had some more time on the CNC. no aluminium yet but i did have some time to redesign and cut my Trampa Cable Riser :grin:

![IMG_20180224_172849|656x500](upload://lsiYJHZtChx06APqOmesbSHrqY6.jpg) 

Not the best finish ever but i guess you wont see the faces . . . right?

![IMG_20180224_172907|645x500](upload://vBzkTfmJPnjZFLHe2thjMidOd3E.jpg)

These have been cut from poly-carbonate which im hoping will make them robust and able to withstand the shock and vibration at the trucks.
```

---
## \#56 Posted by: ducktaperules Posted at: 2018-02-24T18:53:25.329Z Reads: 446

```
Also while im here, a quick update on how the enclosure is holding up . . . 

The only problem i have been having is that as the seal compresses around the screw holes it has created pressure points, causing the case to split around the screws.
 
![IMG_20180224_183821|690x235](upload://qKv3Zh8tB53BrzLt0N2k2ZitWUH.jpg)

And here is my temporary solution (so i can keep riding) :

![IMG_20180224_183904|690x206](upload://kjYGDDuZ05UOshR9lxwpKY2f70c.jpg)

This is just some 4mm acrylic strips to distribute the pressure along the length better. The wiggly bits allow for a slight amount of compression and expansion as the board flexes. seems to be holding up well so far. 

I guess in the long term i will have to mold another enclosure and make some kind of metal strips or something.
```

---
## \#57 Posted by: ducktaperules Posted at: 2018-04-19T22:40:27.325Z Reads: 432

```
BACK ON THE ROAD AGAIN:

A months or so ago I managed to get water inside my temporary electronics enclosure :frowning: 
![IMG_20180228_194856|666x500](upload://3rQBxaD1gHw6VSxEdkPr9h5QbY1.jpg)

managed to blow a DRV on a focbox. After replacing it I decided I probably shouldn't ride again until I had sorted out my enclosure situation to a more permanent solution.

The plan here was too CNC a base plate which I could mount focbox's and bms on securely.
![IMG_20180315_081942|666x500](upload://d6Mcsnb83PZKi1nr4mXuTjomSgx.jpg)

Then CNC an outer housing and EPDM seal to keep everything dry inside.
![IMG_20180323_180023|666x500](upload://xJZpoHIQx3jeLb9Y1hsfgpjMQMl.jpg)

Then when I had time I finished the Tampa riser wires.
![IMG_20180419_192101|684x500](upload://gvQVlzfldZtFSaWCb5uTiC4C6z0.jpg)

Got these mounted on my trucks.
![IMG_20180419_192401|690x436](upload://7jjuEPIoypiALkdA4AtCaUtcgaq.jpg)

Mounted the enclosure and plugged everything in. 
![IMG_20180419_221930|690x255](upload://435AkZbVThmaVG1Ix0qNoRNNTzt.jpg)

So far I'm happy with the way it's working out.

The best bit is defenatley the cable risers, the cables look so good coming out the end of the board.
![IMG_20180419_222035|666x500](upload://tCn03hH0BFCvtNLMb493ojJbsKV.jpg)

There are defenatley some things I would change next time around but I'm interested to see how well this is going to hold up to some abuse. Also it's awesome to finally have the bms on-board and not have to wire up lots of cables ever time I want to charge.
```

---
## \#59 Posted by: ducktaperules Posted at: 2018-05-02T11:01:24.826Z Reads: 398

```
[quote="ducktaperules, post:57, topic:43075"]
BACK ON THE ROAD AGAIN:
[/quote]


After a few great weeks of riding it seems that water has once again returned to my electronics :cry: 
After a very wet ride to work today one of my motors is no longer spinning. 

I have not had a chance to open it yet but it seems odd. It is the master focbox thats not driving the motor, but its still connecting to bluetooth, receiving commands from my remote, and passing them over CAN to the slave which seems to be running.
```

---
## \#60 Posted by: JonathanLau1983 Posted at: 2018-05-02T12:09:30.232Z Reads: 384

```
Might be worth thinking about using a waterproofing spray on the electronics. Think CorrosionX is one option, seen someone spray it on a quadcopter esc then run it under water with the motor.
```

---
## \#61 Posted by: Holyman92 Posted at: 2018-05-02T12:10:58.814Z Reads: 386

```
those trampa decks... are they solid carbon fiber or is there wood in there?
```

---
## \#62 Posted by: mikenyc Posted at: 2018-05-02T12:12:27.732Z Reads: 367

```
neither.

https://www.alibaba.com/showroom/basalt-fiber-fabric.html
```

---
## \#63 Posted by: JonathanLau1983 Posted at: 2018-05-02T12:13:11.540Z Reads: 370

```
No carbon at all I believe, it's glass fibre composite. Just looks like CF
```

---
## \#64 Posted by: Holyman92 Posted at: 2018-05-02T12:14:34.859Z Reads: 368

```
nice... i was thiking of doing a hybrid build using s-glass and carbon... since carbon is stiffer and s-glass is "stronger"
```

---
## \#65 Posted by: ducktaperules Posted at: 2018-05-02T12:15:31.555Z Reads: 367

```
yeah its a fiberglass like composite. unlike carbon fiber its not conductive which makes things easier.
```

---
## \#66 Posted by: ducktaperules Posted at: 2018-05-02T16:11:54.871Z Reads: 366

```
so my fault on my master focbox is weird. 

Im getting "FAULT_CODE_DRV" show up in the app but only when i try and run the motor, as soon as i stop it goes back to normal. Also "ESC Monitor" app by @Ackmaniac is showing "invalid command: can_member" followed by "Error : Unknown fault".

But the CAN seems to be working as i can control and connect the other focbox. any ideas anyone?
```

---
## \#67 Posted by: ducktaperules Posted at: 2018-06-19T16:57:04.748Z Reads: 375

```
FOCED FOCBOX . . . again.

Had another focbox fault recently. This is my third failure so far (admitted one was my own fault caused by water damage). anyways i ordered another DRV and when it arrived i opened my board to investigate.

First thing I found was that all of the hot glue / silicone round the capacitors has broken. This has resulted in one of the caps breaking both legs. 

I think our rural English countryside provide to much vibration for many eskate components.

The second thing is that it looks like one of the fets has released the magic smoke. I assumed this was going to be a DRV fault so had a replacement chip ready but unfortunatley it looks like it might not be the driver that caused the problem :frowning: 

At this point im thinking it might be a better idea to wait for the unity or a dual vesc6 than to buy another focbox. I dont seem to be having great luck with them. I dont think they can handle my current requirements and local road conditions.

I guess i will just have to ride slow on mono for the next few months :cry:
```

---
## \#68 Posted by: ducktaperules Posted at: 2018-06-26T12:31:44.046Z Reads: 380

```
Just had some time to look at this in more detail. This is what the FET damage looked like under the TIM.

![IMG_20180619_172858|666x500](upload://rTxfWmWmmXcVxrRgXBUR41G7hze.jpg)

After cleaning up I start to get some clues as to whats happened.

![IMG_20180626_110444|666x500](upload://k60RLG8nVD63AdMDuE3RSaIu029.jpg)

Looks like the PCB has corroded and copper had been exposed on some areas. Also the edge of the FET seems to be corroded here. Maybe a short between the FET housing and copper has occurred.

![IMG_20180626_110743|690x399](upload://ke2utLMgAw6pCAlcIoKy8mse8KH.jpg)

Decided to remove the fet and asses the damage.

![IMG_20180626_111536|554x500](upload://j9QmP1y97diGd76MXmItUp2CunI.jpg)

Yep, that defenatley looks done.

![IMG_20180626_111830|426x500](upload://tzADyMV0JWrolqcOB5yVVoQe37U.jpg)

The board dident look great either. So I tried again to clean it up.

![IMG_20180626_112123|514x500](upload://7KOPMSiaoCQcuSVrm4Ex5ttcchY.jpg)

This actually doesn't look too bad. It looks like the PCB has worn down to the copper in a few areas. Maybe this is caused by vibration or maybe water ingress? not 100% sure. also cant work out how to check the other FETS without removing them which i don't really want to do if i can avoid it.

So I plan to re coat the bare copper areas again some how then replace the FET. Wish me luck :)
```

---
## \#69 Posted by: ducktaperules Posted at: 2018-06-28T19:41:51.360Z Reads: 352

```
WOOOOOOOOOOOO

So today i fitted the replacement FET and rebuilt the focbox. after conecting it on the desk it seems that everything is working again. Hopefully i can get some time so to put it back in the board and try it out under some load :smile:

Also finally got round to uploading the cable riser to thingiverse if anyone else wants to make one. 
https://www.thingiverse.com/thing:2981889

Hope this is useful to some one :slight_smile:
```

---
## \#70 Posted by: Holyman92 Posted at: 2018-07-05T08:55:51.574Z Reads: 346

```
I'm currently printing something similar... it's based on the unikboard riser and it's coming along swimmingly

 ![JPEG_20180705_030115|375x500](upload://hFd2UqWVeTNgN2epFPbNfJEC1Kg.jpg)
```

---
## \#71 Posted by: pennyboard Posted at: 2018-07-18T01:58:14.277Z Reads: 329

```
Is that cable riser not aluminum, it looks it in the picture, although there's no way it is cause that would short your phase wires for sure.

Actually, come to think of it, are you sure it's not water getting in the cable riser and shorting your phase wires that's killing your focbox? I know shorted phase wires during operation will cause a dry error on any vesc
```

---
## \#72 Posted by: ducktaperules Posted at: 2018-07-19T08:26:50.536Z Reads: 325

```
The cable riser is milled from poly-carbonate. I think its the rough finish that makes it look like aluminium but if i bothered to polish it up it would be clear. its not conductive and the only other thing the wires touch is the composite deck. 


Also after looking under the fets in my focbox im 100% sure issues were caused by water ingress from somewhere.
```

---
## \#73 Posted by: JonathanLau1983 Posted at: 2018-12-04T15:01:37.923Z Reads: 281

```
@ducktaperules how have you found the truck riser with the motor wires? I'm thinking of my options at the moment and my main concern with doing it this way is the connectors are held static to the board so the connectors would potentially vibrate on the motor side a lot and break. I've heard of some members having issues with solder joints breaking at the bullets.
I might still use the riser but have the connectors outside so the cables just bend with the vibrations to hopefully not transfer them to the joints as much.
```

---
## \#74 Posted by: ducktaperules Posted at: 2018-12-05T17:44:09.182Z Reads: 271

```
its actually held up surprisingly well. I ride abusive roads and have broken 3.5 to 5.5mm bullet adaptors before but since switching to this its been very reliable. 100% one of the lowest maintenance parts of of my build :slight_smile:
```

---
## \#75 Posted by: Yerffej Posted at: 2018-12-06T03:19:58.503Z Reads: 261

```
Absolutely love this thread - It's super inspiring to see how your build progresses!
```

---
## \#76 Posted by: drone001 Posted at: 2019-01-01T23:21:58.578Z Reads: 262

```
I weight about 250 and  was thinking about a Trampa or a Lacroix I'm concerned about bottoming out on the Lacroix. How's the flex on that Trampa?
```

---
## \#77 Posted by: ducktaperules Posted at: 2019-01-02T11:33:58.129Z Reads: 266

```
I went for the 16 ply and the shorter deck type cause i was worried about the flex but tbh i think its almost a little to stiff. I have never ridden the longer deck or any of the thinner boards so i cant comment on them but you wont have any issues with ground clearance for sure. 

Looking at lacroix website it looks like they also offer different deck stiffness, with the highest one being labelled 250+ so maybe it would be fine.
```

---
## \#78 Posted by: ducktaperules Posted at: 2019-01-02T17:14:09.667Z Reads: 273

```
ITS TO LONG:
So i have been waiting for my Unity to arrive so that i can rebuild my board over winter ready for next season. it finally arrived before Christmas 
![IMG_20181219_164715|666x500](https://www.electric-skateboard.builders/uploads/db1493/optimized/3X/3/0/30c502f16f91bbd8c8bab9d81e1b2999973c529e_1_666x500.jpeg)

I actually like the orange more than i thought i would.

![IMG_20181219_164711|666x500](https://www.electric-skateboard.builders/uploads/db1493/optimized/3X/c/8/c89aa950ad8f813be4706bf233ef5704e78c87cf_1_666x500.jpeg)

In the interest of science i had to do it :smile: 

![IMG_20181219_145915|375x500](https://www.electric-skateboard.builders/uploads/db1493/optimized/3X/9/a/9ac2db0975530b89af43c19135d209b274ba68c4_1_375x500.jpeg)

Im planning my build using Fusion 360 so i spent some time rebuilding a fairly accurate model.

![unity2|690x465](https://www.electric-skateboard.builders/uploads/db1493/optimized/3X/d/6/d6d697e59efbf7e82a1b9e2b227c107346696870_1_690x465.png)

I modelled as much of the heat-syncs as i could without taking any screws out.

![unity1|690x410](https://www.electric-skateboard.builders/uploads/db1493/optimized/3X/6/b/6b4e09a4826d4295277996f1d28331ad8be34230_1_690x410.png)

no cables included yet but looks good.

![Unity(Recieved)%20v9-1|690x308](https://www.electric-skateboard.builders/uploads/db1493/optimized/3X/b/7/b7a9d555c9b1e2450c622008bf39fa29cfc2e13d_1_690x308.jpeg)

Also made the switch.

![UnitySwitch%20v2%20-1|690x308](https://www.electric-skateboard.builders/uploads/db1493/optimized/3X/0/a/0a0cc1b84b0e74ada8d5701700a39d9012dd123f_1_690x308.jpeg)

Upon inspection it looks like my batteries have not fared well over the winter so i plan to fully rebuild with the unity and a new 21700 12s3p pack and fully watertight enclosures for everything so i can ride in the rain.

I have been thinking about the enclosures for a while now and decided to have a go at mocking something up today as i had some spare time. each enclosure has a rubber seal in the top face and they lock together allowing for slight variation in the distance between pack as the board flex's.

![underpack%20size%20up%20v1|690x368](upload://wjQc1rKcD3tlEVk84uxIPgykL0x.jpeg) 

Only problem is that its way to long they once i have all 6 packs and the unity together. guess its back to the drawing board on that idea.

maybe 2 packs side by side like in my old enclosure, maybe just move mounting points to the edge instead of between the packs would be enough.

Im also considering using PC water-cooling fittings and running in cables inside the pipes to create waterproof flexible joints between the enclosures. might end up looking very sci-fi, or might just end up costing a metric fuck-tone and getting dirty easily. Not !00% sure yet.

EDIT: 
If anybody wants the unity model, All files can be downloaded here:
https://a360.co/2Ua0OTk
Hope This is usefull to someone :wink:
```

---
## \#79 Posted by: drone001 Posted at: 2019-01-02T20:01:30.620Z Reads: 239

```
thx a lot and enjoy that board bruh....
```

---
## \#80 Posted by: Newbie-1 Posted at: 2019-01-03T08:03:39.247Z Reads: 233

```
Nice work may need 1 4 trampa board
```

---
## \#81 Posted by: ducktaperules Posted at: 2019-01-12T12:07:10.590Z Reads: 241

```
[quote="ducktaperules, post:78, topic:43075"]
Upon inspection it looks like my batteries have not fared well over the winter
[/quote]

Suspicions confirmed. RIP wet cell. you have served me well.

![IMG_20190112_115025_1|666x500](upload://mMWC2r0yUpiq3tYNjwI7ypIqXpe.jpeg) 

In all seriousness tho let this be a lesson for everyone. Battery's don't like getting wet or damp. This cell has also pulled down its whole parallel group :frowning: 
I got lucky here and didn't have my house burn down but i will definitely be checking my battery's more frequently in the future.
```

---
## \#82 Posted by: Alex753 Posted at: 2019-01-12T13:11:12.530Z Reads: 227

```
Damn how do this happened ?
```

---
## \#83 Posted by: ducktaperules Posted at: 2019-01-12T13:58:46.918Z Reads: 232

```
i guess water got in one of the cracks in my battery enclosure. tbh the enclosure was never planned to be permanent anyways and and i already started planning a new battery pack. now i got some motivation to actually get it finished before spring.
```

---
## \#84 Posted by: ducktaperules Posted at: 2019-02-09T16:26:51.451Z Reads: 228

```
Just found the time and motivation to make some progress on new enclosures.

The current line of thinking is to make some custom PCB's that will mount 2 of my 6s1p packs together to make a single 12s1p modules.

![12s1pPack|690x371](upload://zgC1m1JPw99dOA62KhhYhnW2IWP.jpeg) 

As there will be large pcb's across the battery pack i have decided to use the opportunity and add some lights. each module currently contains 12 WS2812B addressable RGB Led's in a 3x4 grid.

The board will have 3 of these modules in the centre with the bms at the front and Unity at the back.

Enclosures for these components will be milled from some type of plastic and have clear Poly-carbonate lids.
Enclosures will be joined with thick neoprene gaskets allowing cable entrys to stay waterproof.

![ENC2Build%20v9|690x308](upload://mVdf7CGqU8Rq6Pw7ub5G6CbLlzC.jpeg) 

I have not yet finished the designs for the end enclosures but it looks promising so far.
```

---
## \#85 Posted by: JonathanLau1983 Posted at: 2019-02-09T22:25:19.215Z Reads: 221

```
Looking forward to see this. 
Integrated lighting is the bee's knees.
```

---
## \#86 Posted by: ducktaperules Posted at: 2019-02-11T08:42:38.587Z Reads: 219

```
Small amount more progress, everything laid out better. 

![ENC2Rebuild%20v5|690x308](upload://kj964rQr888zjc0GCplOiXlWtIr.jpeg) 

End enclosures still need trimming down to fit but it looks like the electronics will fit well :)
```

---
## \#87 Posted by: ducktaperules Posted at: 2019-02-12T22:42:15.986Z Reads: 219

```
Got some more time to work on the end enclosure boxes tonight.

![ENC2Rebuild%20v8|690x308](upload://9dgn4ozQ8LlBT1UX0L0ERogIQcz.jpeg) 

its starting to look quite bulky but i don't know that there is much that i can do about that. I guess once you have 21700 cells in protective housing (24mm) and add a PCB (3mm) then put all that in a box with a reasonable wall thickness (2mm top and bottom) there is not much you can do to keep it slim.

Its going to be a big beast thats for sure.
```

---
## \#88 Posted by: ducktaperules Posted at: 2019-02-26T19:38:36.582Z Reads: 220

```
BIG TORQUE requires BIG POWER.

Finally finished and sent the battery PCB's. 

![sentFile1|690x371](upload://zgEhleusTtlUS4WbiXyptqfBfBb.jpeg) 

PCB is 2oz copper with black silk screen. The big pads allow access to the main battery outputs whilst the smaller pads have all the battery balance points. These 12S1P modules can then be hooked in parallel to form larger battery packs on flexible boards.

![sentFile2|690x371](upload://8RQCmczrcJmRdMGU7xufvnzqCT3.jpeg) 

I decided to remove the LED's as they made the wiring complicated and reduced the width of current handling traces. I can always add strips on at a later date if i want to.

My current line of thinking around cabling between enclosures is to find low profile cables that can be passed directly under the seals between separate enclosures. i found some braided cable that looked good so i ordered some.

![IMG_20190226_191846|690x285](upload://ypjNJsGumf5ITDrpV8r4R8n3yxU.jpeg) 

This 2mm thick by 19mm wide braid is equivalent to 5AWG cable. Its probably overkill but it looks great :grinning: IMO If its worth doing, its worth overdoing. 

Also got some 22AWG ribbon cable on its way for the BMS connection points.
```

---
## \#89 Posted by: Blasto Posted at: 2019-02-26T19:45:32.193Z Reads: 207

```
Do you have the real estate to put a smt connector on the bottom side of the pcb for the sense connections? That would require elongate the pcb a bit to clear the cell holder
```

---
## \#90 Posted by: ducktaperules Posted at: 2019-02-26T19:52:47.483Z Reads: 204

```
I could do but im not sure it would give me much benefit. 
Once power is connected it will be difficult to disconnect the modules anyway plus any connection that is not soldered is a point of potential failure due to vibration.
```

---
## \#91 Posted by: Blasto Posted at: 2019-02-26T19:54:40.367Z Reads: 209

```
speaking out of experience, skinning and soldering ribbon cable is no fun at all. A connector would add a little elegance to this already badass pack

![image|376x331](upload://5LNWWbCb0L37BnSAZtjXhtxFwdE.jpeg)
```

---
## \#92 Posted by: ducktaperules Posted at: 2019-02-26T20:32:43.188Z Reads: 207

```
[quote="Blasto, post:91, topic:43075"]
skinning and soldering ribbon cable is no fun at all
[/quote]

I agree, but also to get a connector with adequate current rating they end up being huge. Due to using batteries that are already packaged im super tight on space. I considered putting connectors in the middle between the packs but then the ribbon cables would have to twist and that would require extra height. additionally the cutouts either side should allow me to heat shrink the balance wires directly to the pcb providing additional strain relief.
```

---
## \#93 Posted by: ducktaperules Posted at: 2019-02-26T23:03:11.835Z Reads: 210

```
This is how battery modules should look once assembled

![ENC2RebuildBraided%20v6-2|690x368](upload://4OOIkq2hX1xoOLdPDqizSEVO0Sd.jpeg) 

![ENC2RebuildBraided%20v6|690x368](upload://7OvQyfB5fCZoDQFaBIhwbXzLxNZ.jpeg)  

:grin::grin::grin:
```

---
## \#94 Posted by: Sn4pz Posted at: 2019-02-26T23:34:00.165Z Reads: 203

```
I hope youre running at least 7 inch tires for some decent ground clearance... Im worried about this on my build as well :thinking:

I want to find something good to put on the outside of the enclosure to give it another shell of protection...  

Looks really really nice otherwise!
```

---
## \#95 Posted by: Blasto Posted at: 2019-02-26T23:45:06.312Z Reads: 199

```
Looks dope, i see a nice application for some flex pcb’s 😇
```

---
## \#96 Posted by: ducktaperules Posted at: 2019-02-26T23:48:13.143Z Reads: 206

```
@Sn4pz, This is a concern. But i dont think there is a lot i can do to reduce the height that much.

My battery packs are 24mm thick, 2mm for PCB, 2mm for braided cable, a few mm for the outer layer of poly-carbonate, a few mm for seals and foam padding. Realistically im probably looking at around 30-35mm total enclosure height

With 90mm Gummies im currently measuring around 80mm clearance under the deck at the lowest point. hopefully 45mm clearance should be enough . . . maybe . . . . . . who knows.

Might make the switch to the 6.5" urban treads but i dont know if that will actually increase the ride height at all after i flip the hangar.
```

---
## \#97 Posted by: ducktaperules Posted at: 2019-03-04T19:07:54.324Z Reads: 204

```
Pcb's turned up and they look awesome.

![IMG_20190304_130943|690x484](upload://23oVFwu2ZsXw9MZm7wipCi2dAsw.jpeg) 

![IMG_20190304_130953|690x494](upload://wBshr5K19NXrLp4tgVbVjECEq5k.jpeg) 

![IMG_20190304_130931|690x227](upload://oaMQ8pnlNodTe8UmP61wiHSbbSB.jpeg)
```

---
## \#98 Posted by: PatRocks Posted at: 2019-03-05T06:20:19.682Z Reads: 195

```
Thanks for this write up! I'm about to do a similar process with PETG! I know this was a long time ago but... BUMP!!

The reason I'll be using PETG (vs. ABS) is that the final product is going to be a mold for vacuum infusion. Your write up was very inspiring/reassuring, and one of the only ones about petg specifically that I've found. Cheers for that! Excellent work dude. 

I had a feeling about the rigidity from geometry, thanks for confirming that too!
```

---
## \#99 Posted by: ducktaperules Posted at: 2019-03-14T22:35:33.842Z Reads: 189

```
Assembled my first 12s1p pack of 21700 cells this evening to check everything fits correctly.

![IMG_20190314_221826|690x383](upload://3QYx63Yob5Js9mcoW9leaCEEOfq.jpeg) 

![IMG_20190314_221856|656x500](upload://etJlM9YR8KHrjglulh43MriBuOx.jpeg) 

![IMG_20190314_222037|607x500](upload://qUJJQvcJi6iTOiRl1aVprgAg6yv.jpeg) 

Now I just need to get on with milling enclosures.
```

---
## \#100 Posted by: Okami Posted at: 2019-03-14T23:09:03.430Z Reads: 182

```
Looks really good. Have u at any point considered selling further these battery pcbs?

I guess they could be somewhat costly and tailored to 21700 cells but non the less look really good and capable amps wise
```

---
## \#101 Posted by: ducktaperules Posted at: 2019-04-17T20:57:24.435Z Reads: 174

```
Lots has happened so i will space this over a few posts but basically, after doing lots of cad, designing pcb's and building a test pack i found that some of my 6S1P packs were not in the condition that i though they were in. Additionally my supply if these packs has dried up so i cant get hold of enough to finish my board using this design :frowning: 

so . . . 

**PLAN B.**

looks like i am going to have to buy cells and build my own batteries after all. Lucky for me a friend has also decided to build a diy board. This means that we will get a better price on cells and can split the cost of a spot welder making it far more reasonable to buy one.

Also, BUILDING ENCLOSURES IS HARD. making reliable waterproof enclosures is really difficult and i have earned a lot of respect for the people sell these. I have gotten to the point now where i just want to be out riding. Trying to come up with my own designs has cost me to much time and effort. at least for now im willing to spend the money and buy something that is proven and works.

After looking at a lot of cells and enclosure options it seems that there are not many enclosures avalable that fit the street carver. The easy solution would be to get a hs11 deck but im not keen on the extra length or the £200 price tag. 

For 18650 cells i found the eboosted carver enclosure  https://www.eboardsperu.com/product/trampa-carver/ and the kaly.nyc enclosure https://www.kaly.nyc/product-page/battery-enclosure. Both support 12s4p and fit the carver deck.
I would of preferred to go 21700 however i was unable to find an enclosure that would house these and fit the carver.

I finally decided that the Kaly enclosure would be better because it is cheaper, comes will all the mounting hardware and i prefer they layout to the eboosted board. Additionally the fact that im splitting the costs with a friend means that shipping cost is halved.

Next decision was which cells to buy. After reading much information and looking at many graphs i decided on the popular Samsung 30Q https://eu.nkon.nl/rechargeable/18650-size/samsung-inr-18650-30q-3000mah.html . This decision was based on them having a good balance of capacity, discharge current and performance over life.
```

---
## \#102 Posted by: ducktaperules Posted at: 2019-04-17T21:11:24.735Z Reads: 172

```
First thing to arrive was Samsung 30q cells.

![IMG_20190403_224534|666x500](upload://b9kUtVRDPiULLTa07dQ4OgEFLFF.jpeg) 

100 of these for 2x 12s4p packs plus a few spares to practice on (maybe a new battery for my fat-shark goggles)

In order to facilitate gluing these together squarely i knocked up a few quick jigs which held the cells together whilst gluing. After doing a few quick tests and some reading i decided to use hot glue rather than silicone. Also made sure to squeegee the glue well down in between the cells to maximise glued surface area. Found the end of a spoon handle worked well for this.

![IMG_20190406_104130|666x500](upload://7qVK7rBhvO34JLWMoGsxvR5Rekl.jpeg)

After gluing i protected the positive terminals with these 4p fishpaper stickers(also from eu.nkon.nl)

![IMG_20190406_112018|666x500](upload://k8Rvg25JLCCUYgrqTtj6Jvg3ONW.jpeg) 

Finally a quick test fit on the board. All is looking good so far.

![IMG_20190406_112647|666x500](upload://c3gmljEhEpqAeKTp5InFWqmIRyX.jpeg)
```

---
## \#103 Posted by: ducktaperules Posted at: 2019-04-17T21:31:18.899Z Reads: 171

```
Next fun toy to arrive was the spot welder. We decided to buy a DC style diy spot welder rather than an AC Chinese style one. 

We went for the Malectrics "DIY Arduino Battery Spot Welder Kit V3.3" as i have seen quite a few people using these and having good success. we own lots of 4s miniquad battries so decided to go for the " Full Bundle for Lipo Battery". https://malectrics.eu/product/diy-arduino-battery-spot-welder-kit-v3-2-2-full-bundle-lipo-battery/

Arrived quickly from EU and was easy to assemble (once we managed to find the instructions).

![IMG_20190412_213118|666x500](upload://xoY8rzEoWFBPYHrCmVk61kIX3Ff.jpeg) 

Powered it up from a small battery to test it but soon wanted to get some more power and test the welds.

This is where we hit a problem. It only runs off 3S lipo and all my miniquad batteries are 4S. Fortunately im a hoarder and i have a stash of damaged quad batteries (knew they would be useful for something). After some lipo surgery and removing damaged cells i managed to make 3x 1400mah 3s batteries. We were able to run these in parallel with another 2x 3s batteries that i had to make up a 3s 7000mah power supply for the welder.

![IMG_20190412_213153|666x500](upload://yD87GL3i1fzyesk7yLMGGx6hYS2.jpeg) 

Initial test went well. According the the welder we were achieving pulses of around 600A. 
I do think we need to mount the probes in order to get consistent placement but other than that they seem sufficiently strong.

![IMG_20190417_222549|522x500](upload://1M5wkAXAYSHyKPMr94wWBUBnllY.jpeg)
```

---
## \#104 Posted by: ducktaperules Posted at: 2019-04-17T22:47:14.979Z Reads: 173

```
Last post for today is about our @Kaly enclosures.

As i said previously we went for the kaly enclosures because i like the layout and like that all the mounting hardware is included. Kaly boards are awesome and i think i would of considered one instead of diy if i was in US. I also like the individual cell fusing and battery PCB's that they offer as a kit. 

We ordered a pair of enclosures from kaly.nyc 2 weeks ago from US to ship to UK. We also added 2 sets of the Cell Fuse PCB kits. Unfortunately on the new site there is not option to pay extra for expedited shipping or even tracking but we ordered anyway knowing that they would arrive . . . at some point.

Finally after 2 weeks of waiting patiently i got my delivery notification today. Super stoked when i received the package. 

**THE GOOD**

Enclosure looks good. Finish is nice. Material is thicker than I expected (which is a good thing) yet it still flexes easily.

![IMG_20190417_225239|690x222](upload://qxnXTp2VmnBW6KKmlLRLGrmhbUy.jpeg) 
![IMG_20190417_225244|690x159](upload://uk3BIBqyy7CA6vpjxPQeFzReIFq.jpeg) 
![IMG_20190417_225258|690x186](upload://p1DkCOoo1sKgWdozWXxIaCKtrnU.jpeg) 

Everything fits well and there is enough space for vibration isolation around cells and electronics.

![IMG_20190417_225728|690x230](upload://bl2OPJO2vMQRJ8m45VaYHc2k8PN.jpeg) 

**THE BAD**

Firstly the enclosure is going to need modification to fit the carver deck.

![IMG_20190417_225419|690x215](upload://2JabczUVly4X3CvdXzSM5OMpfgp.jpeg) 
![IMG_20190417_225426|690x195](upload://vlUt0X1lVqx9Za0db6xgFXL7161.jpeg) 

The enclosure is described as being compatible with the Urban Carver but dont think it will be without modification. The corners will need to be substantially cut in order to fit on the deck without overhang or causing wheel bite. This concerns me as cutting this much from the corners will affect the amount of sealing around the corners and may affect the waterproofing of the enclosure. 

Also it looks like the enclosure was cut from its panel with a CNC. It surprises me that the corners are not cut to fit on the cnc whilst the profile is being routed. It would lead to a much neater job than any user will do by hand.

Second minor issue is that my battery cell pcb's are white, not back as shown on the website. Whilst This is not a deal breaker it is a shame that what you see is not what you get.

![IMG_20190417_231755|526x500](upload://eq22PLHvkPg6Leqtx5AgTlXI66b.jpeg) 

**THE BITS THAT I DONT HAVE**

My final and fairly major problem is that there is a large amount of my order missing.

Firstly the order only includes ONE enclosure and ONE cell fuse kit instead if the TWO on my order confirmation. 

Secondly the one enclosure that i did receive is missing a large number of the parts the website says it comes with. I am missing all the screws, all the threaded inserts and all the mounting plates.

Additionally the CELL fuse kit that i received it is also missing the heat shrink that is supposed to be included with it.

**What does this all mean??**

Unfortunately without the cell fuse PCB's for both builds there is not much that we can do to continue. There is not much point in trying to get one board built up as we don't have all the mounting hardware to get it finished and it means setting up the battery welder twice rather than doing all the cells in one go. 

I guess there not much we can do now except wait to hear back from @Kaly and hope that he can get this sorted out. Just sucks that we will likely have to wait another 2 weeks for things to ship from over seas again.
```

---
## \#105 Posted by: ducktaperules Posted at: 2019-04-24T22:47:14.350Z Reads: 165

```
If something is worth doing then its worth overdoing right?

![build%20v3-2|690x322](upload://qoi45DxV0THAcoww3TegthwfxtJ.jpeg) 
![build%20v3-3|690x322](upload://tym1hrOYdy2fbwmtigT0P1ybBhq.jpeg) 
![IMG_20190424_233849|666x500](upload://mFQ30hdpdBjuoeeSwUWzIy3xhJC.jpeg)
```

---
## \#106 Posted by: Shaz Posted at: 2019-04-25T15:34:33.032Z Reads: 158

```
where did you pick up the batteries?
```

---
## \#107 Posted by: ducktaperules Posted at: 2019-04-25T21:49:48.933Z Reads: 160

```
cells are from here :

[quote="ducktaperules, post:101, topic:43075"]
https://eu.nkon.nl/rechargeable/18650-size/samsung-inr-18650-30q-3000mah.html
[/quote]
```

---
## \#108 Posted by: ducktaperules Posted at: 2019-04-25T22:32:01.288Z Reads: 164

```
TAB WELDER PROGRESS.

So lots of people are asking "why bother" and to be honest the short answer is BECAUSE I CAN.

The long answer is that i need to build 2 x 12s4p packs soon and potentially another 2x 14s4p packs for some e-bike friends in the near future. Thats 52x 4p packs or 208 cells each with 3 welds on both ends.

THAT IS 1248 WELDS .

1248 times I have to hold those awkward probes int he right place and concentrate.

Sounds tedious to me so i decided to have a go at creating something to automate the process (at least partially).

This is where im at:

![IMG_20190425_223247|690x396](upload://1FzGoXoMDheQRXWgleQqak1s94S.jpeg) 

The idea here was to make something that can make my welds precise and repeatable but requires the minimal amount of effort to build.

The current design includes 2 stepper motor driven linear stages. The X axis can position cells under the welding head. The Y axis moves the weld probles away from the cells, This axis is also spring loaded so that once contact is made the lead screw can be used to apply consistent pressure to the weld head.

![IMG_20190425_223138|666x500](upload://9ldVnDaV68fqrTGAY2UIa9Ynm8I.jpeg)

 I was considering adding a another axis to allow the weld head to move up and down however it i think this would vastly increase the complexity and im only likely to need 3 positions in the z axis so i might be able to achieve this by placing spacers under the battery pack.

![IMG_20190425_223315|666x500](upload://jAEQHPQepYsvxadPnxvAh2ezTlW.jpeg) 

The linear stages are made from cheep parts from Banggood which i acquired for another project but never got round to using. The bearings seem to be ok but everything else is made of chinesium. It is designed such that dimensional tolerances (or lack thereof) should not be critical to operation. Im kind of glad i never tried to build a real CNC with these parts.

![IMG_20190425_223305|666x500](upload://1GejcnFIMdcCBzR5ZaxUkG9cmJd.jpeg) 

I still need to design a way of holding the cells and welding probes accurately in place but that is a challenge for another night . . . probably tomorrow night as im desperately trying to get it done before the rest of the kaly PCB kits and enclosures arrive.
```

---
## \#109 Posted by: ducktaperules Posted at: 2019-04-28T10:02:23.685Z Reads: 155

```
Still waiting for my replacement kaly parts. seems like the first lot went through fine but the second shipment got stuck in customs :frowning: im £35 lighter but at least they should be here monday :slight_smile:

In other news we have been making good progress on the tab welder.  Yesterday we finished mounting the lead screws and wiring up the stepper motors to a controller.

https://imgur.com/hSKekrI

you can see it running a quick 2 axis weld pattern doing 1 weld for each cell. The spring system in the top axis allows for repeatable pressure on he weld tips during welds.

https://imgur.com/Qroamdh

Additionally we decided to go all the way and add a third axis to the weld head to allow for doing all 3 welds per cell without having to adjust things. this is what the 2 upward facing steppers are for. these will eventually have small lead screws and give the weld head around 12mm of z travel which should be enough for spacing the welds.

![IMG_20190427_232439|666x500](upload://xKc2kWoXjsLKtj1FuhBB6gW8wNG.jpeg) 

I have also designed a more accurate holder for the weld tips and cells. the weld tip holder is made of 2  parts that clamp the tips in place and bolts to the z axis. Cell holder also bolts directly to the x axis.

![IMG_20190427_232505|666x500](upload://rje0iAnGLdTbfrAQsmeOxpyqX9g.jpeg) 

The cell PCB (with pre soldered nickel strips) fits snugly into the cell holder.

![IMG_20190427_232545|666x500](upload://y6p3sF9XxxlIOW9ii8Bh4HK9UW5.jpeg) 

The cells then slide into pace above this. The printed part is pre-tensioned so that cells are held accurately. Tabs will then be bent up over the front ready for welding.

![IMG_20190427_232714|666x500](upload://ko5VsP4UTRQbgs6O43TuKjVWAzs.jpeg) 

Despite basically making it up as i go along im very happy with how this is progressing so far.
```

---
## \#110 Posted by: MCCLANE Posted at: 2019-04-28T11:03:59.005Z Reads: 147

```
Woao, very very good job & step by step progress report.
```

---
## \#111 Posted by: Mudders Posted at: 2019-04-28T11:50:06.103Z Reads: 148

```
Brilliant! I did my 12s6p with the same welder, this method will ensure no burnt fingertips!
```

---
## \#112 Posted by: ducktaperules Posted at: 2019-04-28T22:59:44.039Z Reads: 153

```
Finished the hardware tonight tonight. 

![IMG_20190428_224819|563x500](upload://mYg4GxzjbxFEZov1Lecz6LR4j8d.jpeg) 

![IMG_20190428_224619|624x500](upload://6H5yZorziis542s3M82oY89hw3w.jpeg) 

![IMG_20190428_224633|666x500](upload://4CpJRAlyPWceZ4rvlHJA2mWhwav.jpeg)

Just got some electronics and software tweaks to make before I can test it out . . . Maybe tomorrow if I get time :smile:
```

---
## \#113 Posted by: mmaner Posted at: 2019-04-29T00:22:57.914Z Reads: 146

```
That's cool stuff, I'm curious how much it costs in parts of you happen to know it care to guess.
```

---
## \#114 Posted by: ducktaperules Posted at: 2019-04-29T10:17:35.537Z Reads: 148

```
I built this mostly from stuff laying or purchased for previous projects around but these are the main parts :

2 x Cheep linear axis kits - £17.85 each https://www.banggood.com/15pcs-Optical-Axis-Guide-Bearing-Housings-Aluminum-Rail-Shaft-Support-Screws-Set-CNC-Parts-p-1276180.html?rmmds=detail-left-hotproducts__3&cur_warehouse=CN 

Arduino with cnc shield & stepper drives - £7.87 https://www.banggood.com/CNC-Shield-UNO-R3-Board-4xA4988-Driver-Kit-With-Heatsink-For-Arduino-Engraver-3D-Printer-p-1082323.html?rmmds=search&cur_warehouse=CN

2x small nema17 (Zaxis) and 2xlarger nema17 (X&Yaxis) stepper motors. Seems to cost ~£10 each but i had some laying around from 3d printer projects.

All acrylic was scraps that i have collected.
only other parts are a few printed parts + screws and mounting hardware.

All in all if you had to buy everything i would guess around £100 for all the hardware + some acrylic. I used it cause i had it but i guess wood would probably do just as good a job if that is what you can get hold of.
```

---
## \#115 Posted by: banjaxxed Posted at: 2019-04-29T12:41:29.863Z Reads: 144

```
For different cell sizes would you just manually adjust the Z mount

Presumably a different set of code is required 

Variables?
Cell type, parallel group size, No. of welds, Weld pattern? Something like that

Cool beans my man

I could see this being used with the Boss welder using the foot pedal connector
```

---
## \#116 Posted by: ducktaperules Posted at: 2019-04-29T14:24:35.310Z Reads: 145

```
I guess the cell holder part could be reprinted for different size cells which would mean that z axis would not need to be adjusted much. longer x axis might be needed for more than 4P groups. 

At the moment the cell count, welds per cell and distances between welds are all adjustable for fine tuning.

Im currently using the welder foot pedal just to start the weld sequence but i may change it to  do one cell at a time depending on how much monitoring it requires when running.
```

---
## \#117 Posted by: ZachTetra Posted at: 2019-04-29T14:31:44.807Z Reads: 144

```
If you rotate the head 90 degrees so it's vertical, doing 3 side by side welds per cell will give you the 2x3 contact area without having to space it up every time, just set it down for the 12 welds
```

---
## \#118 Posted by: banjaxxed Posted at: 2019-04-29T16:42:45.859Z Reads: 144

```
Thanks it’s sweet but I use the outer holes, any chance of an accomodation for that or the fusion file in order to tweak?

![image|669x500](upload://6Ikckv2i742ay4i13FPY2x4QUeP.jpeg) 

Here’s what happens if you pull those holes through the riser from a sketch of the hole placement from a HolyPro
```

---
## \#119 Posted by: Acido Posted at: 2019-04-29T20:17:46.722Z Reads: 135

```
Im definetley interested in getting or making one  of these!

Really nice work, could you help me out a bit with the electrical part of it?

Im assuming it wouldn't be complicated to make it possible to weld 3-6p pack?
```

---
## \#120 Posted by: ducktaperules Posted at: 2019-04-29T23:15:02.346Z Reads: 134

```
@Kaly enclosures arrived today for both boards along with all the missing parts plus a few extras 😉 so I don't feel too bad about having to pay some extra customs charges. 

![IMG_20190429_231318|666x500](upload://whtiWtn4y2u5ANuhMmqu8nkCzFi.jpeg) 

![IMG_20190429_231339|666x500](upload://bXhLgm3EONZLx7jQarvGTzDhuAs.jpeg) 

Both enclosures look great and my friend and I are super excited to get building.

![IMG_20190429_232041|666x500](upload://d17z8wnngqnlDj5LUCWRIcQMAEW.jpeg) 

I was a bit worried that the LLT Bluetooth BMS and Unity might not fit side by side but it looks like there is space and maybe even a little room to spare.

![IMG_20190429_232116|666x500](upload://5x9c2bvIcL1E4D0aGQUkWRIELFU.jpeg) 

@ZachTetra that is a great idea . . . About a day to late. Unfortunately I already finished the z axis but your way makes much more sense.

@banjaxxed I'm sure it could be modified to fit all the cables between those holes. I'm away from my pc at the moment but Im happy to share the fusion files with you when I'm back at my pc in a few days if you can wait.

@Acido electronics has been quite easy. If your using that CNC shield I linked then you basically plug the steppers in and your good to go. I can share my code if needed but it's not that pretty. Doing 6p packs should be fine if you add a longer X axis travel. 

That said I haven't actually welded any cells myself yet so maybe we see if it works out first :slight_smile:
```

---
## \#121 Posted by: banjaxxed Posted at: 2019-05-01T15:53:17.830Z Reads: 124

```
thanks! that would be super-de-dooper
```

---
## \#122 Posted by: IndyPilot Posted at: 2019-05-01T17:09:27.140Z Reads: 126

```
Nice!  How fast is it at the moment?  Looks pretty decent and useable, speed wise.
```

---
## \#123 Posted by: ducktaperules Posted at: 2019-05-01T23:05:28.613Z Reads: 124

```
First weld test this evening didn't go great. All axis worked well and operated as expected but it seems like we had some problems getting the weld pressures correct. 

We had assumed that bolting down both probes and spring loading the axis would provide even pressure on both welding tips but that is not the case. Whichever tip touches first stops the other from applying sufficient pressure.

I think we need to work out a way to independently spring load each of the tips so that they are both applying the same pressure. Not 100% sure how yet but I guess we can think about it for a day or so before trying again.

@IndyPilot it's not super fast but it's not suposed to be. The goal here is tidy and repeatable. Im not expecting to save time but if it requires less concentration for a better result then I will consider it a success.
```

---
## \#124 Posted by: sharky Posted at: 2019-05-02T19:10:45.900Z Reads: 122

```
Just a wuick question regsrding the trucks are those the regular trampa ultimates or are these the mini ones?
Kr and thx
```

---
## \#125 Posted by: ducktaperules Posted at: 2019-05-02T21:00:20.037Z Reads: 121

```
these are the mini trucks
```

---
## \#126 Posted by: ducktaperules Posted at: 2019-05-03T22:08:18.275Z Reads: 126

```
New plan for interdependently holding the weld probes to evenly apply pressure on the tab

![build%20v10|690x381](upload://87cplNWgxV8fOptxDnElQMtcSes.jpeg)

Now i just got to wait for it to finish printing :slight_smile:
```

---
## \#127 Posted by: ducktaperules Posted at: 2019-05-04T00:03:44.712Z Reads: 124

```
Parts came out great but i underestimated how strong 3d printed parts are. There is no flex at all in these at all. guess i will have to thin out the cad and try again.

![IMG_20190504_001904|690x336](upload://xaG9wfe6rkfIrYMnxx5bgy3YlFX.jpeg)
```

---
## \#128 Posted by: ducktaperules Posted at: 2019-05-04T00:24:04.603Z Reads: 121

```
Attempt number 2 ready to print

![build%20v12-2|690x381](upload://4zWNMUzhRCQcY7Yk9NSevoWAoP6.jpeg)
```

---
## \#129 Posted by: banjaxxed Posted at: 2019-05-05T09:25:18.009Z Reads: 118

```
Springs?

https://www.thingiverse.com/thing:3070927

https://www.thingiverse.com/thing:3204208
```

---
## \#130 Posted by: rusins Posted at: 2019-05-10T00:57:52.163Z Reads: 104

```
https://www.electric-skateboard.builders/t/no-words-just-pictures-delete-words-2/88821/947?u=rusins

Looking good! One thing I might suggest is to not do all the welds for a cell at once, but go down the line, and then repeat for the next weld, so that each cell can cool off after each weld. (Maybe it doesn't matter though, I'm not an expert; a thermal camera would show)
```

---
## \#131 Posted by: akhlut Posted at: 2019-05-10T01:38:59.809Z Reads: 104

```
100%

Weld once per cell until cell n is reached then return to cell 1.
```

---
## \#132 Posted by: lrdesigns Posted at: 2019-05-10T01:52:17.178Z Reads: 102

```
This little robot needs its own thread. Its too cool to be part of a build thread.

The printed springs is a cool idea and simple, but the consistency of them will be way lower than coil springs. I would think after like 50 flexes the spring force will start to drop dramatically.
```

---
## \#133 Posted by: ducktaperules Posted at: 2019-05-10T09:11:42.816Z Reads: 95

```
@rusins & @akhlut
I also had this concern but i did some testing and i dont think its a problem. 

After doing a few welds it seems like the heat created by the weld is so localized that it is cooled by the surrounding metal quickly and its gone before you can even get your finger in there to feel it. doing 6 successive welds like this generated so little heat that you can barely even feel it.

@lrdesigns might split it off into its own thread at some point once i have some spare time to do a proper write up and upload the CAD.

With regards to the "printed springs" i have actually found them to be very reliable so far. The spring design is based around a "flexure" which basically exploits material flex to provide motion. Flexures are great because they can provide robust & reliable motion with very little backlash. If designed properly and you don't exceed the materials elastic limit they can be very reliable and often outlast other linear mechanisms in industrial applications. They are ideal for scenarios where you need small amounts of accurate movement.

The tab welder also uses a similar concept for the z axis, relying on the flex of a long piece of acrylic to provide relativity linear motion for moving the weld head up and down. 

There is a great video on flexures here (https://www.youtube.com/watch?v=97t7Xj_iBv0) which i recommend everyone watch if you design your own parts.

SIDE NOTE: something that i want to write down before i forget:

I have been considering some flexure based light mounts for my board that are joined to both the board and front hanger. I think it should be possible to use the board lean to steer the lights towards the direction you are riding :slight_smile:
```

---
## \#134 Posted by: lrdesigns Posted at: 2019-05-10T09:22:06.848Z Reads: 92

```
I[quote="ducktaperules, post:133, topic:43075"]
With regards to the “printed springs” i have actually found them to be very reliable so far. The spring design is based around a “flexure” which basically exploits material flex to provide motion. Flexures are great because they can provide robust &amp; reliable motion with very little backlash. If designed properly and you don’t exceed the materials elastic limit they can be very reliable and often outlast other linear mechanisms in industrial applications.
[/quote]

I agree they can be good in injection molded parts, I am just skeptical they can do the same with FDM printed parts. Maybe in SLA without any walls it might be consistent.
```

---
