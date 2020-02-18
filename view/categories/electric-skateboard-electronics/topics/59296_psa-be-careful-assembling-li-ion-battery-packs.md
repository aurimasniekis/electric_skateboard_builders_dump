# PSA: Be careful assembling Li-ion Battery packs

### Replies: 104 Views: 5166

## \#1 Posted by: evoheyax Posted at: 2018-06-18T17:21:19.051Z Reads: 621

```
Batteries are the greatest enemy of electric vehicles. There's a strong agreement here that li-ion batteries are safer than lipos. And while yes, a single li-ion cell is safer vs a single lipo cell, li-ions have a weaker point. And this is the need to assemble 40-78 cells. With lipos, it's easy to solder new wires to the tab. But with li-ions, you need to assemble it with either spot welding or soldering. Spot welding is the easiest solution, but it is less effective with copper, the ideal material for keeping heat down while discharging batteries, vs nickel. This leaves two other options, soldering copper wire to the cells or solder copper stringing to the cells. I copper wire in the past, and while it worked great, it increased the 65mm width of the cells to 80mm. So I decided the new idea, solder copper stripping. Calculated the amount of copper needed in each sheet to get the same copper content as a 10 AWG wire, cut them out, cut all of the corners and rounded any sharp edges. I had the copper strips bend up over top of the each p so that when connected, there would be a flexible joint (another reason I couldn't spot weld the tradition way li-ion packs are put together). I put multiple layers of good quality 3M electric tape between the + and the - of every cell (since everything except the cap is a -). I thought I had eliminated all of the possible risks. But I had certainly missed something:

![IMG-1152|374x500](upload://efo9zooxVkEDSa8pfb2tHemKJuh.JPG)

Just some context of what you are looking at. This is my prototype Rocket Deck with 4x hummie v4 hub motors. This was a 12s4p (48 cell) 30q li-ion battery pack assembled as described above. It included a speedometer, working brake lights and head lights, as well as turn signals that are controlled via the 2nd channel (the wheel) on the mini trigger remote. It had 4x 4.12 chaka vescs, and my really big spark switch (as I like to call it, haha).

Also, in this photo, your looking at the front, the same angle as the videos below. The esc's are in the back right corner. There's 9 p's of 4 cells each on the left side and 3 p's of 4 cells each on the right side. This fire started at the 9th p of the battery pack.

2 factors that I hadn't considered.
- What if vibrations cause the copper to pierce the electrical tape and the cell's thin layer of heat shrink.
- What if the cell balancing wires (which the for the 9p pack, comes out of the top, the side closet in the photo, wraps around and goes back to the middle of right side where it is used) catches a copper strip, pierces the insulation and shorts.

I will likely never know which one is was. But In my mind, it most defiantly was one of those 2 cases.

As to the story of what happened, I was on a joy ride with a friend who was biking. I took this ride so I could put more miles on these wheels, since it has been the biggest issue with all hub motors, including hummies in the past. The wheels (and board) had been ridden over 200 miles at this point. About a mile in while in the bike lane and slowing down for a stop sign (during regen), I heard a loud hissing sound. In the past, with v1 hummie hubs, I heard a similar sound, which was I lost my wheel and I'm ridding on a metal hub now (totally ridable btw, happened at over 25 mph multiple times with out any trouble). So I jumped off almost immediately, since I was only going maybe 10 mph at the time. I realized quickly that I had all four wheels on and that the cells where in fact venting like crazy. So I pulled my phone out and started shooting some video and taking photos while I waited about 30 minutes for the fire department to arrived and finally put it out. In the mean time, one cell after another goes into thermal runaway, catches fire, and spreads to the next cell. At one point, a cell or two exploded, shooting one off like a rocket.

In the end now, about 3k was lost, motors seem to still be ok, though still not tested.

What I've learned in the process:
- Li-ion batteries are still very dangerous.
- If lipos blow up, it's likely you mishandled the cells or there was a manufacturing error when they assembled the internals of the cell (assembly error far less likely than li-ion).
- Li-ion batteries need to be assembled very carefully and monitored more carefully than lipos (as theres 3-8 times the number of points of possible failure)
- Li-ions are much better at dealing with abuses than lipos, but again, more points of failure = more likely to fail (generally speaking from an engineering standpoint)

So which is actually safer? The Answer: They are both very dangerous.

I have built 2 boards with li-ion packs and 6 more with lipos, and my 2nd li-ion pack is the first one that caught fire. **Granted, the failure was on my part, and a properly assembled li-ion pack is safer than a lipo any day of the week.** But this is a DIY forum, where many new builders ARE building their own li-ion packs from the cells bought in these group buys. So if factoring in the likely hood of an assembly error or oversight, is li-ion actually safer than lipo for DIYers who are assembling the packs themselves? Well... I'm running lipos again, haha.

**The moral of the story:** Make sure you know very well what you are doing if assembling a li-ion pack and if not, make sure to buy one from someone who does (preferably with cell level fuses, which might have save me in this case). If not, lipos are easier if you have good soldering skills, but make sure you use a bms!

Lipos are more likely to have manufacturing faults that show up later and cause a fire.
Li-ions are more likely to have an assembly error, which could lead to fire.

So if Li-ion's are properly assembled, there's an extremely low chance of fire (assuming you use the cells properly).
With lipos, there's an unknown chance of manufacturing faults that cause cells to blow up, but assembly error causing fire is much lower.

Again, which is safer? Li-ion in theory. In the DIY world though, where we try experimental shit, neither is safe. This could have been my house, my university, my work, ect..

Without further a due, the after math:

![IMG_1153|374x500](upload://hXW42baeLHZWkdyI99qSHUVS4DA.JPG)
![IMG_1171|374x500](upload://t3wVixwwNjcJ12x49L1FpitYXB4.JPG)
![IMG_1167|374x500](upload://2KXfjwl7nA54HfQJmmT6TqPEhMt.JPG)
![IMG_1178|374x500](upload://xvwEHhl3pEyWFxVDRYeEsQxxrtA.JPG)
![IMG_1162|374x500](upload://12oPp7eDvLBYV6TOqXzbEeKMWYr.JPG)

Short Edited Video:
https://www.youtube.com/watch?v=MmAq2thaCm8

Full Uncut Video:
https://youtu.be/dFxgu77Qun4

Be safe everyone!
```

---
## \#2 Posted by: onepunchboard Posted at: 2018-06-18T17:29:05.605Z Reads: 534

```
you save the motor tho lol. 

generally speaking electrical tapes are being miss used in many area. they are suppose to be temporary patch or aid with something permanent, like a rubber coating or casing.
so is the kapton tape.
```

---
## \#3 Posted by: Itsmedant Posted at: 2018-06-18T17:33:21.853Z Reads: 530

```
What type of rubber coating would you use on a battery?
```

---
## \#4 Posted by: pjotr47 Posted at: 2018-06-18T17:33:34.255Z Reads: 526

```
It hurts to see such a board on fire :sweat_smile:

Thnx for sharing it to other people so everybody know how dangerous it is.

I hope you will recover good from that lost
```

---
## \#5 Posted by: onepunchboard Posted at: 2018-06-18T17:39:03.375Z Reads: 518

```
plasti dip for wires,  but for battery like that actual rubber pad or fishpaper or card stock is needed.
```

---
## \#6 Posted by: evoheyax Posted at: 2018-06-18T17:59:34.315Z Reads: 497

```
[quote="onepunchboard, post:2, topic:59296"]
kapton tape
[/quote]

Is there a difference between kapton tape and fish paper? I thought they were the same.

I have yet to see a viable solution for a flexi-pack (not mountain board, because that makes it a bit easier) that deals with the heat of 80 or 100 amp discharge con. This was my attempt and failure.
```

---
## \#7 Posted by: trancejunkiexxl Posted at: 2018-06-18T18:04:43.511Z Reads: 485

```
This is depressing ☹ glad your ok
```

---
## \#8 Posted by: onepunchboard Posted at: 2018-06-18T18:07:12.919Z Reads: 488

```
kapton tape is for protecting components from heat. also a good insulator because it is a thin plastic. when heated they shrink and loose adhesion to the surface. which can cause short in battery.  fishpaper is thicker and denser that physically difficult for copper to penetrate. some good fishpaper has mica or wax coat that things get slide off. Also the fiber(can't recall name) doesn't burn well they sort of become dust.
and you can look into Terraskin. it's a stone paper so it resistant to heat and doesn't burn and also water proof.
```

---
## \#9 Posted by: Bjork3n Posted at: 2018-06-18T18:10:04.573Z Reads: 479

```
Sorry for your loss.... :confused:

This is my biggest fear, that my battery would burst in to flames in my apartment....
My battery from eskating 10s4p has been solid for 6 months, lets hope it stays that way.

My 10s2p battery stopped working when out riding and i found this ![59|375x500](upload://2p0pgLT3GiRxHJ5vjsxiD01GVrz.jpg)![20180512_124957|374x500](upload://tkPa7Q4JeVvhYxnGfMwT0RHteJg.jpg) 

Be careful guys...
```

---
## \#10 Posted by: sunnyD Posted at: 2018-06-18T18:12:43.328Z Reads: 460

```
oh thats rough dude. best of luck to whatever build you work on next!
```

---
## \#11 Posted by: Michaelinvegas Posted at: 2018-06-18T18:14:45.286Z Reads: 455

```
I’m glad I got a chance to ride your chariot before it became a battery bbq...

RIP
```

---
## \#12 Posted by: riva_00 Posted at: 2018-06-18T18:35:49.054Z Reads: 445

```
Sorry for your loss m8y.
I'm re-doing my battery setup so it's in modular 3d printed boxes for the Lipo's to go in, perhaps i could also house them in lipo-safe material, would only add perhaps an extra 6mm to the height, and my AT build has the ground clearance anyway....
```

---
## \#13 Posted by: onepunchboard Posted at: 2018-06-18T18:48:39.836Z Reads: 436

```
you guys really should glue the pack hard so it doesn't flex...
```

---
## \#14 Posted by: thisguyhere Posted at: 2018-06-18T18:49:31.002Z Reads: 436

```
there is inherent dangers to using these energy dense batteries regardless of how much precaution you use.  we have to assume these risks and it's your responsibility to mitigate failures as best as you can.

i mean, tesla cars, on very rare occasions, are still catching fire and they know a lot more about building batteries than we do combined.  this full [electric supercar caught fire](https://www.google.com/search?q=richard+hammond+crash+fire&source=lnms&tbm=isch&sa=X&ved=0ahUKEwjz0Nv-793bAhXJ5lQKHaCEC4MQ_AUICygC&biw=1636&bih=1011#imgrc=zjJ6q4DNnQ2oWM:) and burned to nothing when it was crashed.

as a general rule, we should be inspecting our batteries on regular intervals to ensure they're running optimally.

using clear building materials, like clear pvc shrink and kapton tape, aids in performing visual inspections.  make sure no wires are coming loose or stripping.  generous use of insulating materials, ie fish paper, foam inserts, rubber pads to isolate the pack from vibrations.  monitoring cell health by checking voltage drift at full drain and full charge may be a good idea.

but despite all that, it may still blow up and it's a reality we all have to live with.
```

---
## \#15 Posted by: Sender Posted at: 2018-06-18T18:50:28.842Z Reads: 417

```
Man it really makes me nauseous seeing this.  I tried to be careful and diligent but there is a lot of room for error.  Thats why I tried to post a lot of pictures in my build thread to get more eyes on.  I live in a loft. Whew. Makes me nervous.  Glad it wasn't in your home.  Sorry for the loss. I would cry.  😥😥😪😪😭😢😢😢
```

---
## \#16 Posted by: legend27 Posted at: 2018-06-18T18:51:43.381Z Reads: 409

```
Wow man, sorry for your loss. I hope the motors still work. But thanks for posting this to show that li-ions can be dangerous too.
```

---
## \#17 Posted by: banjaxxed Posted at: 2018-06-18T18:55:14.828Z Reads: 400

```
Wow that is quite a story thanks for sharing & sorry you lost your pride and joy, hubs salvageable?
```

---
## \#18 Posted by: evoheyax Posted at: 2018-06-18T18:57:28.335Z Reads: 400

```
They seem to be. Took them apart and they look good. Soldered new leads on them but never got around to testing them. Just so much going on in my life right now.
```

---
## \#19 Posted by: banjaxxed Posted at: 2018-06-18T19:01:03.316Z Reads: 401

```
I'm considering a small electrical extinguisher quick release mounted to the deck, it's an extra kg but this just shows you. You never know
```

---
## \#20 Posted by: Blitz Posted at: 2018-06-18T19:12:07.787Z Reads: 392

```
[quote="thisguyhere, post:14, topic:59296"]
[electric supercar caught fire](https://www.google.com/search?q=richard+hammond+crash+fire&amp;source=lnms&amp;tbm=isch&amp;sa=X&amp;ved=0ahUKEwjz0Nv-793bAhXJ5lQKHaCEC4MQ_AUICygC&amp;biw=1636&amp;bih=1011#imgrc=zjJ6q4DNnQ2oWM:) and burned to nothing when it was crashed.
[/quote]
Must not make conspiracy theories about top gear, trying to make electric cars look bad coz they sponsored by Shell (Petrolosos)
```

---
## \#21 Posted by: thisguyhere Posted at: 2018-06-18T19:14:54.650Z Reads: 364

```
that was on the grand tour, not sure if they have petrol companies as sponsors since it's mostly amazon, and some dhl sponsorship monies too.
```

---
## \#22 Posted by: Blitz Posted at: 2018-06-18T19:15:38.919Z Reads: 361

```
But the thing about conspiracy theories Is that you can just go nutz :D

Back on topic: Live and learn :( hope this doesn't happen to others.
```

---
## \#23 Posted by: onepunchboard Posted at: 2018-06-18T19:40:12.033Z Reads: 359

```
GrandTour. It's backed by Amazon. Jeremy fired TopGear.
```

---
## \#24 Posted by: ducktaperules Posted at: 2018-06-18T19:54:16.282Z Reads: 363

```
Sorry to hear you lost your board. :frowning: 

If it makes you feel any better building battery's is difficult. Just yesterday a Tesla caught fire for no reason https://www.independent.co.uk/news/world/americas/tesla-fire-mary-mccormack-us-actress-flames-los-angeles-a8402016.html the video is not that different from yours.

Maybe the community should start opening lots of products with lithium battery packs to see how we can make our diy packs more reliable.
```

---
## \#25 Posted by: evoheyax Posted at: 2018-06-18T20:06:15.151Z Reads: 364

```
Cell level fusing is an idea that chaka first brought to this community. This defiently decreases battery fire probability, but introduces another issue, which is when those fuses blow, so can your acceleration. On powerful boards like this, you would get thrown off.

This is the main reason I don't use fuses. It's a trap waiting for me to hit, and it will cause slams (as I saw happen to jinra in person the first time we met)
```

---
## \#26 Posted by: Aeroquiv Posted at: 2018-06-18T20:39:13.087Z Reads: 351

```
Damn, so sad to see things go in balls of fire... I know you're out of the industry game, but you still building another board? So far, my cell-level fuse battery pack is holding up in my Evolve, but I was so paranoid every time i charged or rode the thing. Kept imagining it would blow in the middle of the night and burn the damn house down.
```

---
## \#27 Posted by: thisguyhere Posted at: 2018-06-18T20:47:30.122Z Reads: 353

```
[quote="evoheyax, post:25, topic:59296"]
This defiently decreases battery fire probability, but introduces another issue, which is when those fuses blow, so can your acceleration
[/quote]

i think cell fuses makes sense in huge P groups, ie tesla's 6s72p, where the remaining cells in the P group can make up for the lost cell(s).  in a 12s3p tho, missing a cell in P group without it being addressed quickly will be a massive problem.
```

---
## \#28 Posted by: evoheyax Posted at: 2018-06-18T20:51:09.680Z Reads: 357

```
With the carvon v2's, because the kv was so high, I could lose reception under full throttle and recover. I can't do that hummie a lower kv lower top speed motor like the hummie v4's.
```

---
## \#29 Posted by: evoheyax Posted at: 2018-06-18T20:54:47.420Z Reads: 355

```
I'm rebuilding, but In a hole still. I'm actively applying and interviewing now though. 4x focbox or vesc6.4 is not cheap. I'm using one of hummies decks with the @psychotiller enclosure with zippy 12s (4x 3s) rewired on the tabs so they could fit and with a 12s balance plug. Everything's together except esc's.
```

---
## \#30 Posted by: aethyr Posted at: 2018-06-18T23:28:09.610Z Reads: 345

```
Did you use insulators on your cells?: ![download|225x225](upload://w9WLD5wwbtX8uJct43ebAH9t0ol.jpg)

Did you solder the copper strips onto the cells? Maybe one of the solder joints failed?
```

---
## \#31 Posted by: Benjamin899 Posted at: 2018-06-18T23:38:00.988Z Reads: 342

```
i can't rly picture the copper strips, can you post a pic?
```

---
## \#32 Posted by: lrdesigns Posted at: 2018-06-19T02:07:27.016Z Reads: 344

```
Sorry for the loss, glad no one was hurt. 

Personally I think lion is more dangerous than lipo in a skateboard due to the increased number of connections and short points compared to a lipo setup. Also if there is a fire they shoot off like little rockets while lipo's stay still. 

Vibration is a big issue with all the connections in an esk8. 

This wouldn't stop me using lion but you have to be even more careful with pack assembly. Most of the fires on this forum have been lion and happened while ridding. I only remember one lipo fire and it was due to a screw from the enclosure penetrating the lipo pouch.
```

---
## \#33 Posted by: Chase Posted at: 2018-06-19T02:27:26.250Z Reads: 347

```
Looking at this post scared the hell out of me. I built first pack and I was about to start using it until I realized I didn’t follow all the necessary precautions. For example I didn’t use fishpaper, or positive terminal insulators as shown two posts above. It kind of seems like the nickel strip I used is a little wide. Can you guys look at my first attempt at battery making and see if you think it’s safe to use? If not, is there anything I can do at this point to make it safe? I was told that once the strips have been soldered onto the positive terminals, it’s too late to add insulators. Check out the pics. Let me know if it’s unsafe or fixable. 12s4p from 30q cells.

![image|666x500](upload://qVzdmchmw1oRE6YnVLSqfrzQecd.jpeg)![image|666x500](upload://3xZZ1zpPi0LkLs1aijVbyigH1YH.jpeg)![image|666x500](upload://6z3DC4UNdYMFKDP2kZMTtpKNVwo.jpeg)
```

---
## \#34 Posted by: slick Posted at: 2018-06-19T03:26:44.248Z Reads: 331

```
ouch - sorry to see that man...
```

---
## \#35 Posted by: Eboosted Posted at: 2018-06-19T04:12:45.495Z Reads: 333

```
Brother I feel your pain, I've been there and it's not fun, o also could ever detect the main cause of my Trampa catching fire but I know what I didn't do. 

I did use the round circles around the positives leads, but I didn't use fish paper between each pack.

Did you use the circular fishpaper terminal isolators?
Did you use fish paper between the packs? 
Do you have pictures of you battery build process? 
Did you isolate the charging port? 
Did you use fish paper between the cells and balance wires? 
Did you use bullet connectors between the battery and ESCs?
Were you giving full throttle when the first cell started to vent? 
What was your technique to connect P groups? 

Sorry for all the questions hope you don't mind answering, but I understand this post has been created to prevent these kind of incidents and so are my questions. 

Wish you good luck with the next build hope you do t get discouraged by this episode
```

---
## \#36 Posted by: Kuchi Posted at: 2018-06-19T04:51:50.506Z Reads: 321

```
I was thinking about putting m batter in a lipo safe bag
```

---
## \#37 Posted by: Hummie Posted at: 2018-06-19T05:13:13.073Z Reads: 320

```
disassembling the battery would be a pain.  maybe you can get in behind all the possible edges with something.   can see if the welds are any good at the same time.  but there are long spans of horizontal nickel strip which will be very rigid.   theres a method people use with a bend which allows flex.

i also believe the lipos are ironically safer considering so many people are connecting 18650 packs having never done it before.  I think especially if you want to get decent brakes on a high kv hub motor at higher speed, and have the battery max regen be possibly set high, lipo may be the best thing
```

---
## \#38 Posted by: evoheyax Posted at: 2018-06-19T06:02:21.959Z Reads: 324

```
[quote="Eboosted, post:35, topic:59296"]
Did you use the circular fishpaper terminal isolators?
[/quote]
No

[quote="Eboosted, post:35, topic:59296"]
Did you use fish paper between the packs?
[/quote]
No

[quote="Eboosted, post:35, topic:59296"]
Do you have pictures of you battery build process?
[/quote]
Unfortunately, no

[quote="Eboosted, post:35, topic:59296"]
Did you isolate the charging port?
[/quote]

Yes, charge port was opposite corner of where the fire started.

[quote="Eboosted, post:35, topic:59296"]
Did you use fish paper between the cells and balance wires?
[/quote]

No, but the wires where no under any pressure.

[quote="Eboosted, post:35, topic:59296"]
Did you use bullet connectors between the battery and ESCs?
[/quote]

Positive yes, neg, no. Used the positive to turn the board off and on.

[quote="Eboosted, post:35, topic:59296"]
Were you giving full throttle when the first cell started to vent?
[/quote]

No, I was braking, was going maybe 20 mph, slowed down to around 10 mph and it started venting.

[quote="Eboosted, post:35, topic:59296"]
What was your technique to connect P groups?
[/quote]

I used a copper strip on top of the cells to connect the p's. This was all covered in electrical tape.

Yes,  could have taken more precautions. The last li-ion battery I built did not have any issues, besides it was larger than desired. The only difference was I used copper stripping instead of copper wire.
```

---
## \#39 Posted by: pjotr47 Posted at: 2018-06-19T06:05:04.737Z Reads: 298

```
I don’t works. Our packs are above 100wh and are to powerful for a Lipo bag
```

---
## \#40 Posted by: Eboosted Posted at: 2018-06-19T06:30:38.581Z Reads: 314

```
Lack of fish paper would easily be the culprit venting of the first cell, I guess P groups could have been rubbing against each other.

I don't think thicker strips could have caused a short as once they are spot welded they don't move at all, however the copper sheet might have cutted one negative isolation.

[quote="evoheyax, post:38, topic:59296"]
I used a copper strip on top of the cells to connect the p’s. This was all covered in electrical tape.
[/quote]

I need to understand this, I'm not sure what you mean. Did you spot weld the P groups and the folded the strip?

On the other hand, if something like this ever happens to anyone reading please go to the nearest shop, grocery store, office, building, business, etc., and ask for a fire extinguisher, no sane person would ever deny it.

In this scenario the mind just freaks out and says, sh!t there's nothing I ccan do just wait it to finish, but remember it could take 20 minutes to finish or even more, so you just take out your phone and shot a video, I know because I did it myself and then banged my head knowing there were docens of shops around.
```

---
## \#41 Posted by: SimosMCmuffin Posted at: 2018-06-19T06:44:37.038Z Reads: 311

```
I personally haven't been okay with leaving batteries charging unattended for a long time, just too paranoid about something going wrong (can't sleep peacefully) and destroying most of my stuff and possibly somebody elses. Too high risk vs reward.

New pack build has been going quite nicely though.

![IMAG1050|690x389](upload://sGQxTmO3l3MMOLlMqCERcXr0bYQ.jpg)
![IMAG1049|690x389](upload://7HfM89VlT0I3vcM61i84eWV4eyz.jpg)
![IMAG1052|600x500](upload://jcV4d41T6u0fqJgG4hRE8qSMkVm.jpg)
![IMAG1054|689x440](upload://8x73VWTmJdbulgDuMVLHyEkld6n.jpg)
![IMAG1058|690x389](upload://gtmu0FLszTed9rynsLx1ZrSjZTN.jpg)
![IMAG1055|690x309](upload://nfNRTgMcgR0nCduBiuW8e9nBEP5.jpg)
![IMAG1057|690x470](upload://xctBoExH1IjL17n4rS3AQgjw5Na.jpg)
![IMAG1064|690x389](upload://5LcKKANWLILosdM98TqzcHluk9w.jpg)
![IMAG1065|690x389](upload://2YxMu8H49XcQi7CUhSjfMfMzpUB.jpg)

I did the first submersion test with the XT90-panel connector attached to the back of the pelican case (empty insides) and found it to without any extra sealing material to not leak any air out on it's own, but after pressing the sides of the pelican case in, it did produce some air bubbles meaning that water was getting in and air was coming out. I then redid the test with some hot glue added onto the mating surface of the connector and re-heated it before bolting the connector back onto the back panel. Absolutely watertight, couldn't get any air bubbles to come out even with rigorous pressing on the case.

Going to visit a hardware store today to get some foam tape to add around the cell pack's exoskeleton to insulate it from vibration and cushion any harder hits from the pelican case. I personally started to work on this new pack with ruggedness in mind. It will most likely also house the first FlexiBMS and work as a test platform for it.

@evoheyax , live and learn, this is the mentally I have developed as an engineer. You lost one pack, improve on the next one! No bodily harm was caused to anyone, just monetary loss, so no reason to not keep going forward and learn from past mistakes.
```

---
## \#42 Posted by: Eboosted Posted at: 2018-06-19T06:50:29.562Z Reads: 299

```
BTW never use bullet connectors on batteries if they unplug they will cause a big short, it happened to me before. Use XT60 or X90s.
```

---
## \#43 Posted by: Eboosted Posted at: 2018-06-19T07:01:58.522Z Reads: 298

```
[quote="Chase, post:33, topic:59296"]
Can you guys look at my first attempt at battery making and see if you think it’s safe to use? If not, is there anything I can do at this point to make it safe?
[/quote]

If I were you I'd disassemble the all P groups by cutting the nickel strip between them in order to add fish paper between them, them stick them together with hot glue or natural cure silicone.

Remove those balance wires and put fish paper between the cells and wires, fix wires with kapton tape.

Buy 200mm heat shrink and wrap the pack together.

I'm sorry to say this but, in it's current state, your battery does not look safe to me, please remember I'm not being a jerk just want you to avoid a possible fire in the community.
```

---
## \#44 Posted by: Chase Posted at: 2018-06-19T07:15:26.053Z Reads: 297

```
So @Eboosted do you think it would be safe to reuse the cells after pulling off the nickel strip if I sand down the terminal ends of the 30q with a Drexel like in this video at 2:20

https://youtu.be/iScKCOH3eqA

What nickel strip width do you reccomend? This 12mm wide seems a bit much.
```

---
## \#45 Posted by: lrdesigns Posted at: 2018-06-19T07:31:16.798Z Reads: 297

```
This PCB is cool, where can people get that? 
![image|690x219](upload://3F51WCWiTgAdDfT6olfg507tNzX.jpg)

The pack construction and case look really nice. But no fish paper rings for the positive ends? How thick is the white plastic ring in there?
![image|398x378](upload://sN0VehFA5qA1KH0rKG7Six3Z4jj.jpg)
```

---
## \#46 Posted by: SimosMCmuffin Posted at: 2018-06-19T08:09:41.676Z Reads: 290

```


[quote="lrdesigns, post:45, topic:59296"]
This PCB is cool, where can people get that?
[/quote]

PCB is custom design by me for this specific pack. Although I don't see any reason why it wouldn't work in other packs, if the pack geometry allows for it. I can share the ready-to-order gerber .zip file if somebody wants them.

[quote="lrdesigns, post:45, topic:59296"]
But no fish paper rings for the positive ends? How thick is the white plastic ring in there?
[/quote]
The cells are fresh virgin Samsung 35Es, So they are what the manufacturer made them to be. 

Personally I don't see the need to use fishpaper with this pack, because everything has been spot welded with minimal thermal stress applied to the cell terminals, so the plastic rings insulators are completely fine.
They are very unlikely to mechanically break, because the whole pack is welded first in parallel, then in series, then bolted into the 3D-printed exoskeleton, which is then foam pad insulated and then placed into the pelican case. Very, very rigid build with vibration dampening.
Only possible way I see of having them be broken is by melting them with too high currents running in the nickel strips, but the strips are hefty 10x0.2 mm size with multiple parallel series strips to avoid hot spots and carry the current better. I don't plan on running such high discharge currents that I believe this would become an issue.
```

---
## \#47 Posted by: linsus Posted at: 2018-06-19T08:11:29.128Z Reads: 278

```
A longboard vibrates a fair amount so something is bound to get loose after awhile. I've torn down all packs I've built atleast once and saw welding spots gone loose on atleast one spot on all of them. Been Lucky enough to ever penetrate a cell tho *knocks on wood*
```

---
## \#48 Posted by: sebaszz Posted at: 2018-06-19T08:25:09.040Z Reads: 281

```
Really appreciate you story and sharing this

I'm no expert in batteries but as an electrical engineer I see a lot of dangerous battery packs created over here.

few examples
- insufficient nickel used for power distribution
- insufficient insulation or physical distance
- no mechanical strain relief between the cells
- battery packs not or improper secured
- improper soldering
- improper routing of balancing wires
- no vibration dampingen

Highly recommend for our application to use:
exoskeletons +  fuse wire
```

---
## \#49 Posted by: SolarTurtle Posted at: 2018-06-19T11:11:21.857Z Reads: 267

```
Just my two cents: The 0,15mm nickel strip is rated for 15A. So if you use it for electric skateboarding, i recommend to weld 4-5 nickel strips on the battery.
```

---
## \#50 Posted by: Cobber Posted at: 2018-06-19T11:42:10.187Z Reads: 274

```
We all have our own experience I guess Bro:

[quote="Eboosted, post:42, topic:59296, full:true"]
BTW never use bullet connectors on batteries if they unplug they will cause a big short, it happened to me before. Use XT60 or X90s.
[/quote]

XT90s are good if you will always be under 90A, I use AS150's on all my lipo batteries as the charge connectors as well as my board, and as the connector to my esc's (my default connector, but I unplug to charge with my icharger), past that I either use some 400A 6.5mm bullets I got from Europe or 8mm Castle bullets...

I expect my mountain board to pull more than 90a and I feel more secure in big over rated connectors.

I guess where I am going is I _bet_ the bullets you had problems with were not as big. 
eg. if you push my 400a 6.5mm bullets together the tolerances are so tight your going to need a serious grip to pull them apart by hand, most are going to reach for a tool. 

So I think the rule would be better or more accurate for the layman:
_at least use XT60/90 or some **solid bullets** * rated for higher current._  

*because those **_solid bullets_** have a interference fit that is very tight in order to carry the rated Ampacity

TLDR: 6.5mm-8mm bullets rated for high current are the cats whiskers :cat: the bee's knees :honeybee: and the ducks nuts :duck: !
```

---
## \#51 Posted by: pat.speed Posted at: 2018-06-19T11:51:31.936Z Reads: 262

```
What are the chances of over stressing the battery in regen? Max charge is 4a for 30q cells so that is 16a total, or 4a per Vesc, that doesn't seem like much and makes me think you must have it set higher. 

If I've got the regen wrong please correct me as I'm new to using vescs
```

---
## \#52 Posted by: Bjork3n Posted at: 2018-06-19T12:17:19.490Z Reads: 260

```
I use a total of -16A on my pack (10S4p 30q)
I think it's maximum 4A per parallel group.
```

---
## \#53 Posted by: pat.speed Posted at: 2018-06-19T12:28:20.552Z Reads: 256

```
Yes that’s pretty much what I said, the thing that’s makes me wonder is that he has 4 motors so he must only run -4a per Vesc.

 I think you mean 4a per cell, 16a per parallel group
```

---
## \#54 Posted by: evoheyax Posted at: 2018-06-19T15:00:06.564Z Reads: 259

```
[quote="Eboosted, post:40, topic:59296"]
I need to understand this, I’m not sure what you mean. Did you spot weld the P groups and the folded the strip?
[/quote]

Soldered copper strips, then folded up to on top of the battery, where they were connected to the next p. There was 2 layers of electrical tape between the cell and copper though. I used the battery heat shrink on each p so they weren't actually touching the next or previous p..Only cells in the same p could touch, which is fine.

[quote="Eboosted, post:40, topic:59296"]
On the other hand, if something like this ever happens to anyone reading please go to the nearest shop,
[/quote]

Might not work. Battery university said it might work for small lithium fires, but I think were over that threshold.

The fire department used a special extinguisher for lithium fires. It worked really well, but was not your tradition foam, looked more like a clear liquid (not water though).
```

---
## \#55 Posted by: Dyspro Posted at: 2018-06-19T15:34:33.132Z Reads: 247

```
Or throw it in the backpack.
```

---
## \#56 Posted by: banjaxxed Posted at: 2018-06-19T15:43:14.276Z Reads: 244

```
Yeah but I don't like anything in a backpack that can hurt me if I fall on it
```

---
## \#57 Posted by: aethyr Posted at: 2018-06-19T16:49:20.664Z Reads: 255

```
[quote="SolarTurtle, post:49, topic:59296, full:true"]
Just my two cents: The 0,15mm nickel strip is rated for 15A. So if you use it for electric skateboarding, i recommend to weld 4-5 nickel strips on the battery.
[/quote]

This is completely false.  0.15mmx7mm nickel is rated for about 5A continuous. Above that the nickel will heat up, leading to premature failure of the strip, or melt insulators and definitely reduce pack efficiency due to heat. I'm not trying to be a dick but simply correct the number so that others don't think that a single 0.15mm strip can handle 15A and lead to a pack fire like the OP. You definitely do want to layer 4-5 nickel strips depending on the current load you will need, so no argument here.
```

---
## \#58 Posted by: wafflejock Posted at: 2018-06-19T16:49:51.367Z Reads: 266

```
Yup regarding putting out the fire the only thing I've heard works with lithium fires really is removing the source of oxygen so it can't burn (completely covering it with sand is the best technique I've seen to contain the smoldering fire).  Still probably doesn't hurt to have an extinguisher on hand to suppress it or stop it from spreading to anything near by.  I've considered keeping a small sandbag in my backpack but lots of extra weight if it were to be enough to actually cover 2 5S 5Ah (let alone something bigger)

Regarding charging I imagine most people are just plugging in a BMS and assuming everything will be good I made my lipos removable so I don't have to worry (as much) about it when charging can put them in a lipo safe bag at the very least or if you want to go gung ho and feel really safe do something like this:
https://www.youtube.com/watch?v=gobFcNzGG9I

or buy something like this https://hobbyking.com/en_us/bat-safe-lipo-battery-charging-safe-box.html
```

---
## \#59 Posted by: evoheyax Posted at: 2018-06-19T16:54:37.678Z Reads: 256

```
[quote="aethyr, post:57, topic:59296"]
This is completely false. 0.15mmx7mm nickel is rated for about 5A continuous.
[/quote]

This is the issue with nickel stripping. It's not the best material due to the low amp ratings it can do. if it's 5a con, then I need what, 20 layers, to do 100a con safely... This is what pushed me away from them in the first place and to copper. But copper is hard to spot weld without damaging the cell also.
```

---
## \#60 Posted by: clistpdx Posted at: 2018-06-19T16:55:33.196Z Reads: 260

```
[quote="evoheyax, post:38, topic:59296"]
Did you isolate the charging port?
[/quote]

@Eboosted can you clarify what you mean by "isolate the charging port"? I'm not yet building my own packs, but trying to gain enough knowledge to someday consider it.
```

---
## \#61 Posted by: aethyr Posted at: 2018-06-19T17:01:19.257Z Reads: 253

```
Depending on the pack layout, you don't need most of the nickel to handle 100A. For example, if I'm connecting 30Qs in series and I calculate 15A continuous then my series connection between then needs to only handle 15A continuous or 3 layers of nickel.

The issue as at termination, where all your parallel cells come together at a single (-) or (+) terminal and THAT does need to handle the full pack current. I ended up crimping a 10AWG bus bar to accomplish that.
```

---
## \#62 Posted by: SolarTurtle Posted at: 2018-06-19T17:13:14.200Z Reads: 253

```
It depends on the nickel width. You can find very different statements on the current for nickel strips, some says 15A, some says 5A, some says 8A.
Can you underline your statement with a temperature measurement? I would be interested.

We are agreed that one stripe isn´t enough. And i saw pictures here with just one stripe. So it is very dangerous, because the nickel will heat up and could be a trigger for battery fire.

Best regards,
Solar
```

---
## \#63 Posted by: willumpie82 Posted at: 2018-06-20T13:18:14.750Z Reads: 246

```
It is not just the thickness, a nickel strip of 5mm wide vs 10mm is twice the current
Just calculate the surface (like we do in EU with copper wires) 5x0,15 = 0,75mm2 and take the resistance /m for the strip, this way you could calculate the resistance over the length used, following to calculate the power lost over the wire and last calc the heat-up of that. Theoretically the wire is cooled by the cells mass. So,.. it's hard to tell the exact melting point of the nickel strip. 
I would care much more about the quality/quantity of the welds. A bad weld gives much more heat-up than overloading a piece of nickel strip
```

---
## \#64 Posted by: sebaszz Posted at: 2018-06-20T14:19:14.910Z Reads: 252

```
When I first saw all the single strip versions on these forum. I couldn't believe the charts with these incredible low rating were correct.

So I took current injection tool and started inject 10-70A into different size of nickel. After these test I can confirm the table below from Endless Sphere is correct.

![Cu%2C%20Ni%2C%20Steel%20efficiency%20chart|549x500](upload://67AaXbcHal5oa69BBd33ZyGIqvU.png)

Many people have quite some luck. I think it's a combination of lower loads during the ride and the max required power is only during short amount of time. Still it's very risky to operate the nickel strips in this high current window.

12S3P - 2x 6355 motors, I used 4x 12x0.15mm (good for around 40-45A continous)
12S5P - 2x 6384 motors, I used 1x 12x1.0mm copper (overkill)

Difference in resistance between copper and nickel is incredible. That's why spotwelding works very well for nickel :zipper_mouth_face:
```

---
## \#65 Posted by: willumpie82 Posted at: 2018-06-20T14:26:22.235Z Reads: 241

```
Man, great overview! 
to add, it will get even worse with bad welds. 

now I'll consider to take my pack apart soon (used .15mm strips and set the vesc to 40A), I do monitor the cell temperature but not the strips. :open_mouth:
```

---
## \#66 Posted by: aethyr Posted at: 2018-06-20T16:14:35.593Z Reads: 231

```
Thanks for doing this. I built my pack a year ago based on this table using optimal values, ie 5A per 0.15x7mm strips. IMO, its foolish to build your pack at the bleeding edge of capability. You always want to leave a large safety margin. As I said earlier, some guy here built his 90A pack using single layer 0.15 and claimed it was fine because his pack hadn't blown up. :roll_eyes:
```

---
## \#67 Posted by: Exigent Posted at: 2018-06-26T19:11:50.759Z Reads: 210

```
A possibility you left out, while remote is still possible; a counterfeit cell(s) that didn't hold up to the energies your system placed on it. It can also take time for the counterfeit to fail. All it takes is one bad cell and the entire system is at risk.

Even quality resellers suffer from the occasional counterfeit battery/cell. Counterfeit parts happen to the military, aerospace, hospitals, etc all the time even with their quality checks. They can be very difficult to detect and cull from a supply.
```

---
## \#68 Posted by: Battosaii Posted at: 2018-06-26T19:18:03.659Z Reads: 205

```
Should you double up the strips in between the p groups, I'm building a 12s8p using 10mm wide .2 pure nickel.
```

---
## \#69 Posted by: Exigent Posted at: 2018-06-26T19:22:59.634Z Reads: 206

```
If it's mounted to the deck, you may not be able to get to it when you need it. The general advice is to not store an extinguisher right next to the possible direct source(s) of fire (like in a kitchen, you don't store the extinguisher right next to the stove).
```

---
## \#70 Posted by: strattos Posted at: 2018-06-26T19:23:33.688Z Reads: 199

```
Am I the only who uses 2 8mm or 2 7mm for parallel because its simply easier to weld? Anyone else out there doing this am I doing something wrong lol.
```

---
## \#71 Posted by: Sender Posted at: 2018-06-26T21:20:44.749Z Reads: 201

```
I did 2 10mmx .15mm strips for the parallel connections.  Next time I will probably just do one layer after talking with some people more.
```

---
## \#72 Posted by: strattos Posted at: 2018-06-26T22:46:00.801Z Reads: 194

```
Yeah there shouldn't be much current running between cells. But more nickel isn't really a bad thing Imo lower internal resistance can't be a bad thynj
```

---
## \#73 Posted by: Hummie Posted at: 2018-06-27T14:37:35.680Z Reads: 185

```
series connections take the full current and the parallel connections see very little
```

---
## \#74 Posted by: Exigent Posted at: 2018-06-27T19:02:01.940Z Reads: 191

```
**Temperatures, Insufficient Cooling, Thermal Cycling: contributors to catastrophic failure**

Something I've not seen much attention to on personal builds here, is heat-sinks and system ventilation. From what I see, most people seem to be more concerned about water-resistance than ensuring adequate cooling of electronics and the battery packs. I would think exposure to water should be the exception, and avoided wherever and whenever possible. Cooling should be a **very** high priority, especially on these high-power boards. Properly implemented heat-sinks can also significantly reduce system heat while maintaining water-resistance.

Also, do you have or have you considered any instrumentation that measures and reports the temperatures in your cell packs? Any warning alerts when temps get too high? One can also put thermal sensors at key locations of power bus elements. Real-time temperature sensing could give one minutes of warning before imminent catastrophic failures, even allowing one to avoid a failure. It can also provide data for improving future builds' ability to dissipate heat.

Edit to add:
Another important factor to consider is thermal expansion and contraction. Depending how the board is used/stored, some of the components might see VERY sudden temp changes of from say 32F to 200F (or higher with insufficient cooling). That could cause major structural dimensional changes in elements like the bus strips. In some cases it may thus be undesirable to have a completely rigid pack design that doesn't allow for the physical changes in the nickel or copper strips, or the physical stress on solder joints. Expansion and contraction could potentially even cause welds to pop or partially pop, thus causing hot spots. Temperatures cycle repeatedly as the board is used thus the damage could be cumulative and failure appear only after days, weeks, or months of use.
```

---
## \#75 Posted by: Exigent Posted at: 2018-06-29T16:32:13.034Z Reads: 180

```
[quote="Eboosted, post:40, topic:59296"]
once they are spot welded they don’t move at all
[/quote]
Has anyone performed any before-high-current (cold) and during-high-current (hot) dimensional measurements on bus strips in battery packs? Or measured separating gaps under the same conditions?

I **suspect** thermal expansion/contraction plays more of a part than some may have considered in some electrical failures. I've noticed what appear to be millimeter or less "insulating" gaps in some projects. There are not only possible changes in length and width, but also the potential for warping in the thinner strips of metal as they heat up.

I've seen this phenomenon in high power battery packs that amateur radio operators have built and then sold at amateur radio conventions or to provide backup power for repeater stations. But, I don't have practical exposure to any of these very high power skateboard battery packs.
```

---
## \#76 Posted by: Hatman30 Posted at: 2018-07-02T23:15:37.770Z Reads: 160

```
So what is the general concensus on what thickness/width of nickel to use on the parallel connections on say a 10s5p pack? For the series connections I know to use a 12awg wire but am I right in thinking a single strip of 7mm x0.15mm nickel for the parallel connection would be fine also?
```

---
## \#77 Posted by: Benjamin899 Posted at: 2018-07-02T23:18:23.886Z Reads: 155

```
well depends what amps you draw. there is chart up there
```

---
## \#78 Posted by: Chase Posted at: 2018-07-02T23:46:53.606Z Reads: 154

```
Well according to the chart, to optimally carry 60 amps I need something like at least 6 strips of nickel? That’s where my confusion arises because I haven’t seen anyone using that many layers between series.
```

---
## \#79 Posted by: Benjamin899 Posted at: 2018-07-03T00:17:32.703Z Reads: 152

```
thats why people use copper, siliconwire or some kind of copper braid soldered onto the nickelstrip. there are alot of examples. search a bit in this forum and you will find plenty.
```

---
## \#80 Posted by: wafflejock Posted at: 2018-07-03T00:23:57.559Z Reads: 159

```
Lots of good points.  One place I'd have to differ though is in the focus on waterproofing since sometimes it rains and you don't expect it or you just still want to be able to ride.  Agree on more thermal monitoring would be good but the vesc does some of that and can get that data through metr or believe using the ackmaniac firmware.  Problem is when you're riding you need to pay attention to the road and don't typically have time to monitor gauges while going.  Having thresholds with alarms/alerts in the apps would be nice if they don't already exist.  Problem with cell levelling thermal sensing is designing something flexible enough to work with all the various batteries configurations and in a way that makes it easy for battery builders or diyers to incorporate it.  Points about thermal expansion and all are good though and not things I've seen brought up often.
```

---
## \#81 Posted by: Chase Posted at: 2018-07-03T00:30:45.025Z Reads: 150

```
Definitely seen the posts, it’s just the majority of battery builds I see lack the extra material between series. I’ve seen a lot of them using like 3 nickel strips and calling it good.
```

---
## \#82 Posted by: Benjamin899 Posted at: 2018-07-03T00:35:05.862Z Reads: 149

```
well if you don't push your board and keep the amps low, why not. But the people who are actually pulling more and want to be safe do that often.
```

---
## \#83 Posted by: DougM Posted at: 2018-07-03T00:36:15.011Z Reads: 154

```
A lot of it depends on the distance you're traveling.  If you are going the 3/4" from one cel to another there's not that much resistance so the above advice might be a little pessimistic.  If you're going the length of the pack then definitely you want to go with bigger wire.
```

---
## \#84 Posted by: Schulerbible Posted at: 2018-07-03T01:35:33.728Z Reads: 155

```
What strips peeps are using in the middle of the pack? On the outside it is easy to apply some braided wire but the inside currently stops me building the pack. Still bothers me since months!!! What's the general setup for a higher amp draw?

Don't wanna end up with a pack like this. This is just not well done. Starting from the huge amount of kapton tape to no fishpaper rings and finally single spot welds on cells!!! 

![image|666x500](upload://vx9AaQ6HoHJrNgrxNd7Sh66VuCF.jpg)
```

---
## \#85 Posted by: Benjamin899 Posted at: 2018-07-03T01:48:25.920Z Reads: 147

```
if you dont want to use braided wire , just use your normal silicone wire
```

---
## \#86 Posted by: Chase Posted at: 2018-07-03T01:53:09.914Z Reads: 149

```
Yeah that was my first pack build that I ripped apart to make safe before ever using it. Definitely had more than one spot weld per cell though.
```

---
## \#87 Posted by: Hatman30 Posted at: 2018-07-03T11:23:05.738Z Reads: 139

```
I'm talking about the parallel connections, not the series connections. C my above post.
```

---
## \#88 Posted by: Hatman30 Posted at: 2018-07-03T11:24:17.564Z Reads: 139

```
for the series connections between P packs most ppl use 12awg silicon insulated copper braided wire. Or you could use a bus bar.
```

---
## \#89 Posted by: Benjamin899 Posted at: 2018-07-03T11:25:34.351Z Reads: 137

```
well i answered that already. what amps do you draw divide that by your p count and look up at the chart.
```

---
## \#90 Posted by: Hatman30 Posted at: 2018-07-03T13:10:36.336Z Reads: 131

```
But for cell level fusing fo example if ia 22awg fuse wire is used from the positive terminal to a bus bar and is rated for 24amps then at least a 0.3 x 7mm nickel strip would need to be used to group the parallel cells?
```

---
## \#91 Posted by: Benjamin899 Posted at: 2018-07-03T13:15:30.630Z Reads: 129

```
24a for a fuse wire? what are you building mate.
edit: ok since fusewire is a failsafe 24a seems ok. so no problem there.
```

---
## \#92 Posted by: Hatman30 Posted at: 2018-07-03T13:24:01.945Z Reads: 132

```
22awg is the recommended wire thickness to use for cell level fusing on Chaka's article for a 10s6p pack.
https://www.electric-skateboard.builders/t/fishpaper-and-cell-level-fusing-use-it/35026/124
```

---
## \#93 Posted by: Hatman30 Posted at: 2018-07-03T13:29:19.193Z Reads: 128

```
I would have thought though if the batt max was set to 80amps and I was running a 10s5p pack then the max amp discharge per Parallel group should be 16amps. So per cell that is 3.2amps  max  which means that using 0.15mm x 0.7 mm nickel strip (optimal under 4.7amps) for each attached to a fuse wire should be fine?
```

---
## \#94 Posted by: L3chef Posted at: 2018-07-03T13:36:16.743Z Reads: 131

```
16amp per cell. not 3.2
```

---
## \#95 Posted by: Benjamin899 Posted at: 2018-07-03T13:38:28.658Z Reads: 131

```
batteries in parallel act like one cell.
```

---
## \#96 Posted by: Hatman30 Posted at: 2018-07-03T13:41:03.618Z Reads: 129

```
But if I'm connecting a 22awg fuse wire to a nickel strip for each cell going to a bus bar then surely that individual cells max is only 3.2 (16 over 5)
![image|690x493](upload://uYFkRiSTmTNvWTckzomKWjvKdau.jpg)
```

---
## \#97 Posted by: Hatman30 Posted at: 2018-07-03T13:43:41.087Z Reads: 125

```
sorry just read the above... Cool :grinning:
```

---
## \#98 Posted by: Benjamin899 Posted at: 2018-07-03T13:45:15.491Z Reads: 123

```
why not start with something small to perfect your technique and then go to a 10s5p
```

---
## \#99 Posted by: sk8l8r Posted at: 2018-07-03T13:49:29.460Z Reads: 122

```
can I ask why your not just welding the fuse wire directly to the cell? (building a pack right now)
```

---
## \#100 Posted by: Hatman30 Posted at: 2018-07-03T13:50:30.037Z Reads: 126

```
I'd rather limit the amount of heat to the cell if possible.
```

---
## \#101 Posted by: sk8l8r Posted at: 2018-07-03T13:52:25.515Z Reads: 124

```
fair enough, I just see an extra point of failure on every cell - I assume less welds / connections is better
```

---
## \#102 Posted by: Hatman30 Posted at: 2018-07-03T13:54:40.400Z Reads: 123

```
Also using Chakas method of doubling over a piece of nickel strip provides a bit of give/flex to the fuse wire so less chance of it breaking.
```

---
## \#103 Posted by: sk8l8r Posted at: 2018-07-03T13:57:32.087Z Reads: 133

```
ah I like that idea :) 

I tested some fuse wire welded directly - was able to hold the weight of 5 cells but even small amount of movement could cause problems
```

---
## \#104 Posted by: Benjamin899 Posted at: 2018-07-03T13:59:13.943Z Reads: 133

```
i just bought N.E.S.E modules...f that welding^^
```

---
