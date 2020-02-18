# I opened up my blink s2

### Replies: 53 Views: 6740

## \#1 Posted by: florensvb Posted at: 2017-10-22T11:05:07.219Z Reads: 577

```
Hey guys,

a few weeks ago I got my Blink S2 and have already put above a 100km on it so far. Last night i rode it on super wet streets and when i got to my destination, it didn‘t turn off anymore whilst beeping in a triple pattern haha. Since Actons warranty doesnt cover damage from moisture anyways- why not open it up and see whats under the hood, right?! Thought some others might be interested to see:

<img src="/uploads/db1493/original/3X/f/4/f42ebc79e624b58b3c71da6808be5c62aa30534a.jpeg" width="349" height="500"><img src="/uploads/db1493/original/3X/c/e/ceab506fffea03a145b19aef26797221403491e3.jpeg" width="374" height="500"><img src="/uploads/db1493/original/3X/4/1/41f3ce8d1c2f4ce23700c407f3ae5ed491024e14.jpeg" width="374" height="500">

I have been just leaving it open since then, hoping that the electronics will dry. For example: When i try to turn off the lights, they just flickr hahah.. 

What made me really curious and what pushed me to make this post is: 
The battery pack has plus and minus leads coming out to the esc for discharge and on the other side as well, for the lights i believe, BUT there are NO balance leads?! How are they keeping this thing in balance? I made sure by lifting up the pack- no balance leads. Dafuq- can somebody explain please hahah? 

I think the ESC is the same chinese one they use in Meepo as well?

Also, they use XT40s!! 40?!? hahaha 

Tell me more about my board! ;)
```

---
## \#2 Posted by: Hankbull Posted at: 2017-10-22T11:19:57.138Z Reads: 535

```
Now's your chance to pull all that shit out and DIY it
```

---
## \#3 Posted by: florensvb Posted at: 2017-10-22T11:53:40.658Z Reads: 525

```
Hhaha dudes i already made my own DIYs and am in the process of making another one right now- bought the S2 before getting into this but acton took ages to ship. so it was all for the better ;)

I am trying to get wiser on the S2 though- your input would be much appreciated :)
```

---
## \#4 Posted by: florensvb Posted at: 2017-10-29T19:32:05.772Z Reads: 482

```
hey @Namasaki sorry for pulling you in to this- but i am just so curious how there can be no balance leads :) do you have a clue?
```

---
## \#5 Posted by: boards Posted at: 2017-10-29T19:40:59.567Z Reads: 468

```
Might have balance circuitry in the pack, or they just yoloing it.
```

---
## \#6 Posted by: WARMAN Posted at: 2017-10-29T21:19:49.142Z Reads: 446

```
Have you taken the shrink wrap off the battery? I'm guessing the bms must be wrapped up in there with the balance leads,and what you have in the picture with the hall sensor's leading to it is the esc!
```

---
## \#7 Posted by: Namasaki Posted at: 2017-10-29T22:26:17.309Z Reads: 430

```
[quote="boards, post:5, topic:36183"]
Might have balance circuitry in the pack
[/quote]


this would be my first guess. Maybe a very small bms used only for charging.
```

---
## \#8 Posted by: HeyMacfly Posted at: 2017-12-10T17:39:12.632Z Reads: 401

```
WTF ! That board supposed to be splash proof.
```

---
## \#9 Posted by: florensvb Posted at: 2017-12-10T21:03:39.085Z Reads: 392

```
By now i can tell you that it's definitely not! Whenever its just slightly moist on the road the board goes crazy, mainly the circuit board that controls the on/off switch. Instead of a hard dead switch they implemented some magic curcuitiry that goes mad every time it gets moist and then doesnt respond anymore! Also by now one of the hub motors seems to be broken, resulting in the board not turning on anymore. I havent had the time to check it out- i could probably temporarily unplug one hub and just drive it as a single, but anyways quality is not great ... after 350 km i have a broken hub, an on off switch that only works sometimes, the front lights are permanently gone and one of the side lights are also off. Shame. Back to DIY.
```

---
## \#10 Posted by: GhettoFab.rictation Posted at: 2017-12-14T17:35:53.627Z Reads: 358

```
Use a voltmeter to track where the power stops or shorts at. Google is your friend, also we are lol. Looks like step down converter is at the bottom and ESC is up top ( on the picture). I would undo shrink wrap then start following the volts to the short
```

---
## \#11 Posted by: harveld9 Posted at: 2017-12-22T14:46:04.674Z Reads: 338

```
I also support this one. Thanks for the recommendation.
```

---
## \#12 Posted by: Dark180 Posted at: 2018-04-12T16:21:40.985Z Reads: 321

```
Did you manage to fix it? Mine just got water damaged. I was debating on dropping the 300 to fix it but then i saw your post and that esc looks like this one http://www.diyeboard.com/v11-dual-belt-motor-sine-wave-foc-esc-speed-controller-p-522.html . I might take a stab at fixing it myself
```

---
## \#13 Posted by: Hurleyjacket17 Posted at: 2018-04-22T02:19:49.342Z Reads: 315

```
Same issue. I got it to turn back on by plugging it into power to recharge it. Went for a ride, it works like normal. Waiting to check to see if the problem repeats itself. Could be just a shitty power switch. If it happens again, I might swap it for a marine power switch for a boat. Every time you ride through water you need to grease the hubs and bearings so they don’t rust out and break at 15mph. Let me know if you found a solution I didn’t think of let me know. ![image|375x500](upload://owW7ZQlCFXfUDhLi5nWF1otbmgw.jpeg)
```

---
## \#14 Posted by: Hurleyjacket17 Posted at: 2018-04-22T04:47:55.227Z Reads: 287

```
Went to ride it to work and it was completely non responding. Took the battery off to check the power switch and noticed a button on the motherboard. Pushed it and held for 10 seconds and then hit the power button and it came to life like nothing ever happened. Must be a design flaw with the power button. That’s going to suck if I have to do that every time the side walk is wet. Either way looks like that’s the easiest fix with out modifying anything. Hope that helps someone....![image|376x499](upload://qa67IR8sCO99lwieXwcYuHwlR47.jpeg)
```

---
## \#15 Posted by: Jebe Posted at: 2018-04-22T08:55:29.937Z Reads: 267

```
thats that crappy ebay diyboard esc.
```

---
## \#16 Posted by: Hurleyjacket17 Posted at: 2018-04-22T13:34:07.051Z Reads: 254

```
You mean the ACTON Blink s2?
```

---
## \#17 Posted by: OlivierDud Posted at: 2018-04-24T14:23:45.116Z Reads: 252

```
Hey guys.

The ESC from the blink S2 is on a metal plate that you can see on those pictures. My S2 was making annoying noises under lots of vibrations and I found out it was due to that metal plate moving around and the screws that hold it not being tight enough.

When I tried the tighten the tiny nut on of those bolts, half the bolt snapped off with the nut. I'm guessing the vibrations must have been eating that bolt. 

I kinda fixed the issue slightly by putting pieces of cardboard around the metal plate, but there's still some noise going on. 

My question is, can I just put hot glue kinda everywhere around it without damaging the electronics or doing something wrong?
```

---
## \#18 Posted by: Gatwod Posted at: 2018-05-02T06:04:08.589Z Reads: 240

```
Any luck finding a receiver? I'd love to figure out how to add a different controller! Nano x?
```

---
## \#19 Posted by: 99Questions Posted at: 2018-05-18T12:43:45.567Z Reads: 220

```
Open my board ready to jump into the DIY pool. Any ideas what to do with the Battery? Options: Sell, Take apart, Trash it appropriately
```

---
## \#20 Posted by: chulander Posted at: 2018-05-19T00:16:43.804Z Reads: 204

```
my board died while riding on the wet streets after it rained. It went about a mile before suddenly stopping. I suspect the ESC is died but given I'm a noob. I have no idea which ESC to buy.

any pointers would help. thanks!
```

---
## \#21 Posted by: aigenic Posted at: 2018-05-19T19:34:32.962Z Reads: 177

```
If you have S2 ebay [ESC](https://www.ebay.com/itm/Dual-Motors-Electric-Skateboard-Longbaord-Controller-Remote-ESC-Substitute-Solid/332504878542?epid=17018333775&hash=item4d6ad5cdce:g:l18AAOSwcOFaOMXP) could work...
But if you can afford to go dual VESC way, go for it :)
```

---
## \#22 Posted by: chulander Posted at: 2018-05-22T05:27:01.217Z Reads: 170

```
thanks! I'll research more about the dual vesc but it's great to know the backup option. Appreciate the help
```

---
## \#23 Posted by: HeyMacfly Posted at: 2018-05-22T21:41:34.596Z Reads: 164

```
Any ideas how to replace dying led strip lights on S2 ? Does anyone tried to replace them ?
```

---
## \#24 Posted by: OlivierDud Posted at: 2018-05-23T20:54:07.719Z Reads: 159

```
I wish mines died. Those things are tacky as hell and I can't believe you can't turn them off manually. I placed two layers of electrical tape to mask the light.
```

---
## \#25 Posted by: Mikenopolis Posted at: 2018-05-23T20:55:25.540Z Reads: 155

```
can't you just open up the board and disconnect the LED leads
```

---
## \#26 Posted by: Exigent Posted at: 2018-05-24T05:20:15.251Z Reads: 152

```
I had the opportunity to open up a new board and found one of the PCB's retention machine screws rattling around loose inside the electronics enclosure. Wasn't very impressed with some of the soldering quality.

Checking for loose items and dodgy soldering/wiring inside high-energy density products (only where practical) has now been added on my list as one more thing to do before applying power to stuff.
```

---
## \#27 Posted by: Exigent Posted at: 2018-05-24T05:37:12.541Z Reads: 149

```
What do you mean by "dying"? What are the symptoms? Dimming? flickering? Just some of the LEDs dark/dim?
Might not be the LED strips. I found the LED strips on an old Blink belt-drive board very easy to replace, but ultimately decided to just remove them. 
If you can remove them easily, then your main issue would be matching the board-supplied voltage to the LED strip(s) you purchase or scavenge. Check the dimensions to be sure they'll fit, too. You might even be able to adhesive or hot-glue stick the new strips right on top of the old (electrically disconnected) strips for mechanical compatibility. Mouser and digikey are good electronic parts companies that have had reasonable Qty=1 prices. Of course, eBay or Amazon too. If going with White LEDs, my personal "color" preference is "cool" white or above 4000K. "Warm" white LEDs look yellowish.

That particular set of LED strips didn't take much power (total about 150mA @ 42VDC = 6W) but still...power is power and the board's battery pack was only 72 Watt-hours. So, the LEDs ate about 8-9% of the **theoretical** battery capacity for an "hour" of use (but it's actually much lower than motor Watts, so it's not really a real-world example for battery runtime). But, one had to remember to turn off the board after every use without the bright LED reminders.
```

---
## \#28 Posted by: Exigent Posted at: 2018-05-24T06:09:32.676Z Reads: 143

```
[quote="OlivierDud, post:17, topic:36183"]
My question is, can I just put hot glue kinda everywhere around it without damaging the electronics or doing something wrong?
[/quote]

You may have better solution with double-sided tape or even just a small layer of neoprene (or "foam") tape across PARTS of the shield to dampen any resonant vibration. You shouldn't have to cover the whole thing with tape. This is assuming it's not a heatsink.
```

---
## \#29 Posted by: HeyMacfly Posted at: 2018-05-24T20:20:10.226Z Reads: 131

```
Almost half of the strip led light is dim.
```

---
## \#30 Posted by: tex Posted at: 2018-05-25T20:23:41.673Z Reads: 132

```
After only 350km it's very disappointg, how much it cost new this board?
```

---
## \#31 Posted by: HeyMacfly Posted at: 2018-05-26T14:55:01.020Z Reads: 126

```
$600 for the new board.
```

---
## \#32 Posted by: florensvb Posted at: 2018-05-26T19:10:13.583Z Reads: 128

```
Hey guys sorry for the long response time haha. I am actually super happy that this thread is gaining some traction because there’s virtually no information on the internet about the s2 other than the standard commercial spec sheet. This thread is actually on the first google page when searching for stuff related to the s2 :open_mouth: 
Now that the suns out I’d love to finally give this board some attention again and fix my broken hub motor. Therefore I’ve got two questions: should I attempt to fix the damn motor or better go ahead and buy two new motors in a set? The symptoms were as follows: sometimes during accelerations it cut out, kind off like the vesc does when it tries to draw more amps than the battery has to offer, and after a few days of that repeating, the motor just completely stopped working. The board only turned on again after disconnecting the motor leads from the esc. Help me out dudes :D
```

---
## \#33 Posted by: florensvb Posted at: 2018-05-26T19:11:53.226Z Reads: 125

```
I actually ordered from Indigogo for 899 :sweat_smile:
```

---
## \#34 Posted by: HeyMacfly Posted at: 2018-05-26T22:29:11.047Z Reads: 132

```
It’s on sale right now. $599 is a good deal. I wouldn’t pay more for that board. ![image|330x500](upload://lMjeCewSMRz2YxQqYgyoYDMIpFo.jpeg)
```

---
## \#35 Posted by: ChrisJerzey Posted at: 2018-06-10T22:20:09.719Z Reads: 118

```
My wife bought me this board for my bday had the board for two weeks ran over damp street and now board won't shut off and right hub motor stopped moving help!!!! She bought it on Amazon with the three year insurance can I just return it and get a new one Acton Blink S2
```

---
## \#36 Posted by: HeyMacfly Posted at: 2018-06-10T22:29:24.145Z Reads: 117

```
Return it if you can. Mine died  and i have to pay $230 for repairs from water damage. Its a shame because right now i could fix it by myself.
```

---
## \#37 Posted by: Blitz Posted at: 2018-06-10T22:37:56.260Z Reads: 116

```
wowgo got better top speed.
And the remote is nice boosted copy the brakes never lock up, and it's just super smooth.
a lot of reviews would say that.

So why Buy a board that has lower top speed for the same price?
```

---
## \#38 Posted by: HeyMacfly Posted at: 2018-06-10T22:58:26.437Z Reads: 116

```
I bought S2 almost a year ago. I still have it. It's a good board but chinese boards are way better.
```

---
## \#39 Posted by: ChrisJerzey Posted at: 2018-06-15T21:48:49.853Z Reads: 112

```
Hi guys just wanted to update you on what was the outcome of my situation. I opted to return it to amazon directly per their 30 guarantee..... After alot of research. I am now a proud owner of a Riptide R1 it's amazing I'm so happy with it. It handles like a dream. Thanks for all your help!!! I really appreciate it.
```

---
## \#40 Posted by: HeyMacfly Posted at: 2018-07-05T14:58:35.310Z Reads: 108

```
I sold my S2. Soon I will be the proud owner of Lacroix Board.
```

---
## \#41 Posted by: Dark180 Posted at: 2018-07-05T16:10:35.560Z Reads: 96

```
woah talk about an upgrade, congrats man
```

---
## \#42 Posted by: OlivierDud Posted at: 2018-07-05T16:12:44.129Z Reads: 97

```
How much did you pay for the Lacroix?
```

---
## \#43 Posted by: HeyMacfly Posted at: 2018-07-05T16:44:56.857Z Reads: 93

```
With shipping and Sanyo 20700 battery pack: $2770
```

---
## \#44 Posted by: ElskerShadow Posted at: 2018-07-05T17:07:29.624Z Reads: 95

```
Worth it with these battery the board can easily last 10 years if properly maintained. Enjoy your board! 
@HeyMacfly
```

---
## \#45 Posted by: hempmilk Posted at: 2018-07-31T18:34:09.550Z Reads: 88

```
Where can i get parts for my board? mine wont charge.... i dont know why im very confused i think its this![image|375x500](upload://azPK1GIi8ROayXeF5M6RpArjQSU.jpeg)
```

---
## \#46 Posted by: pixelsilva Posted at: 2018-08-01T06:01:23.460Z Reads: 81

```
> @florensvb 
> 
> ![image|349x500](upload://ag8XFgMRDzg1TcRhDzRJBTdgrho.jpg)
> 
> ![image|374x500](upload://4wNkBtOOlPe4VX7fC46NacPfaPV.jpg)

No wonder why is so heavy!! Look at how much metal frame plating are inside this thing? :nut_and_bolt: :hammer_and_pick:
```

---
## \#47 Posted by: Nelson Posted at: 2018-12-14T21:31:27.860Z Reads: 60

```
![image|375x500](upload://m0abJXV0mKiU074ZIN75V6Yf89U.jpeg) 
I ripped out the cables for the side lights to disable them forever. Now what?? Do I just cover the edges of the white and black cables with electrical tape and put everything back in or what?
```

---
## \#48 Posted by: Fredisyoga Posted at: 2019-01-29T23:19:00.583Z Reads: 49

```
Just wondering if you had any luck on finding the receiver and swapping the remote for the nano x, yet? Thanks in advance! :)
```

---
## \#49 Posted by: Battosaii Posted at: 2019-01-30T01:01:34.909Z Reads: 45

```
My buddies Blink s2 didn't want to charge anymore. 

I found the culprit broken tab for the battery on the BMS.

![20190125_162048|666x500](upload://acRY5RjyETtoxPwbS4VkKrNxdOy.jpeg) 

These boards are so damn heavy. My 12s4p dual 6355 evolve build feels like it weighs less than the blink s2
```

---
## \#50 Posted by: Chalupa_Batman Posted at: 2019-06-18T00:21:11.029Z Reads: 30

```
sorry to revive an old thread.

I'm fixing my brothers s2, it will not turn off.  I'm guessing the onboard spark switch has failed.  Has anyone had a similar experience?

part of me wants to just add a loop key rather than replacing the whole esc.
```

---
## \#51 Posted by: Bulgrim Posted at: 2019-07-24T14:49:19.400Z Reads: 21

```
You didn’t have to rip them out the black and white cables are all the you need to cut if you look at the connection you could have added a switch and you can turn it on and off
```

---
## \#52 Posted by: Bulgrim Posted at: 2019-07-24T14:59:12.413Z Reads: 20

```
So I am New the e-boarding community but I have learned a lot from you guys here so long story short I ran into the battery not charging and other stuff I got the board brand new in a box from someone and only did 42k total on it when all this started happening called acton no response was disappointing but hey I really like the board so I took apart and took it to a electronic repair shop the guy helped me out and he told me that the issue might be the power connection for the battery and there is a board inside the battery so you have to cut it open and check that also here is the end result of the process. ![image|375x500](upload://yif5QkOg4SYNIRR7LZG6bQal9Wo.jpeg)
```

---
## \#53 Posted by: Bulgrim Posted at: 2019-07-24T15:05:20.902Z Reads: 19

```
I will be doing some more improvements to this board to see what I can do to make it better it’s sad that Acton cheapen  out on a really great board and won’t help people with this board but don’t worry I have something I want to do with this board in the winter to make it better I will update when it’s done but I’m the mean time I am going to enjoy the summer with this board.
```

---
