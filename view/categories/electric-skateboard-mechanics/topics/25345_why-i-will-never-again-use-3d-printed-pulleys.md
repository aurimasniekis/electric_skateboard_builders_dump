# Why I will never again use 3D printed pulleys

### Replies: 57 Views: 7290

## \#1 Posted by: michaeld33 Posted at: 2017-06-14T04:08:56.978Z Reads: 637

```
Although at first using a 3D printer pulley sounded like a good idea to me, considering many pulleys are made out of thermoplastics like ABS and Nylon, I was under the misguided conception that these parts would conform to the tolerance and temperature standards of an electric skateboard. After 5 to 10 minutes of riding, the pulley had been absolutely destroyed, resulting in something that looks like this: 

<img src="/uploads/db1493/original/3X/7/7/77186dbc9a70bc6cdccd2eb4986943f5656fae5c.JPG" width="375" height="500"><img src="/uploads/db1493/original/3X/e/a/eaafc50ce86f52d35b0ae34d0427310986989bea.JPG" width="375" height="500">

Now, I'm not bashing @JuniorPotato93, being the grandmaster of 3D pulley design, but it does raise some serious considerations when building a board, along with the potential riding dangers, seeing as how this occurred while riding down the street at 30 mph. I looked down while riding to find a melted pulley which was hot to the touch and significantly pliable. I would have dismissed this most likely if the board had continued to function, but it took only 30 seconds more for the second pulley to melt and get pulled off as well. For this reason, I don't see the benefit of using a 3D printer to make a pulley for an electric skateboard, or for any high-speed application for that matter.
```

---
## \#2 Posted by: Boardnamics Posted at: 2017-06-14T04:14:57.733Z Reads: 614

```
What type of plastic did you use to print the spur? I have printed my own custom modeled spur with the help of an scad template creator. It allows the teeth to be customized with a decimal value to ensure a perfect fit. Took me about 3 printed spurs to get the shape just right. I had one PLA printed spur that delaminated probably from a rock jamming it. Yours looks like it melted apart, so the fit was probably not proper causing excess friction and failure.
I printed mine in PETG and it has held up 50 miles so far. It is all about fine tuning the tooth profile to fit.
```

---
## \#3 Posted by: michaeld33 Posted at: 2017-06-14T04:22:01.341Z Reads: 603

```
It was printed using PLA, the other using PETG, I was interested in testing the difference between the two, unfortunately, it seems that it was a friction problem, enough so that the belt actually felt HOT, which was very concerning. I ordered metal gears for the wheels which should improve the durability, I believe that 3D printed mounts can be durable, considering 3D printed polycarbonate can be shot out of a shotgun and it seems to hold up pretty well, it's the tolerance issues that resulted in my near 30mph accident, when the pulley got ripped out. That being said, I still believe that 3D printed pulleys work better as a temporary solution rather than a finished product.
```

---
## \#4 Posted by: PXSS Posted at: 2017-06-14T04:25:39.513Z Reads: 590

```
There's something wrong with your system. It should not run that hot. If there is that much friction, switching to metal pulleys won't help. Your belt will fail next. You need to fix whatever is causing the extra friction
```

---
## \#5 Posted by: Just_esk8in Posted at: 2017-06-14T04:29:54.194Z Reads: 586

```
Has anyone tried 3D printing with tough resin from formlabs? I just made some I believe I used junior potatoes design off of thingiverse I have not tried with my weight on them yet but they seem very promising I just spun the motor with them attached. 
<img src="/uploads/db1493/original/3X/9/9/994ab4ba7c5ea7acbadf7bd31fe300e1f0c014c5.jpeg" width="375" height="500">
Just a pic of the setup not the pulleys
```

---
## \#6 Posted by: michaeld33 Posted at: 2017-06-14T04:29:59.966Z Reads: 541

```
I determined the problem was that that pulley was getting rubbed against the edge of a screw, a problem which I fixed by sanding down the edge of the pulley, but I guess the while the board was under load, it managed to brush up against the screw and create some heat, although I can not be assured that the metal mount will work better, the smaller gear on the metal pulley should prevent it from creating friction.
```

---
## \#7 Posted by: Boardnamics Posted at: 2017-06-14T04:31:53.279Z Reads: 531

```
If the belt feels hot, it means either it is rubbing on something, or the belt/tooth mesh is poor. It could also be too high of a tension. On my $200 poor teenager board, I run barely any tension at all on a htd5m 15mm belt and I never get any skips. If I run more tension, everything gets this "bind" feeling and the belt gets to about 150f no load. If you want higher tolerances, print slower. With gears especially, you have to print very slow, about 25mm/s or under for most printers unless it's one of those super speed deltas. Any faster with my setup, and the teeth started looking really bad.
```

---
## \#8 Posted by: michaeld33 Posted at: 2017-06-14T04:31:55.574Z Reads: 505

```
I have a smaller resin printer which is designed for making small parts around 5 cm in diameter, but this is definitely something I'd love to try.... Maybe it's time to invest in an SLA. I would imagine the UV cure properties allow it to hold up to better temperatures, along with the better tolerances and layer adhesion.
Very cool. Let me know how it goes.
```

---
## \#9 Posted by: Just_esk8in Posted at: 2017-06-14T04:34:41.596Z Reads: 489

```
I will make sure to let you know if it's worth it or not.
```

---
## \#10 Posted by: michaeld33 Posted at: 2017-06-14T04:35:36.369Z Reads: 472

```
The gear was printed on a well tuned Makerbot which I ran calibration on before I printed. It's definately friction created by the screw, but my point isn't the source of the heat, rather the stability of the gear at high speed and how easily they melted.

Regarding your bind issue, THAT sounds concerning to me, have you figured out the source of it? The belt should spin freely both directions, especially a tight belt.
```

---
## \#11 Posted by: psychotiller Posted at: 2017-06-14T04:40:14.959Z Reads: 442

```
Nylon is the way to go. Also, aside from the screw rubbing. Having your belts too tight will cause over heating as well.
```

---
## \#12 Posted by: michaeld33 Posted at: 2017-06-14T04:45:06.762Z Reads: 455

```
I've got some nylon kicking around in the back shelf, my main concern with nylon is that it absorbs water from the air which can cause some issues while printing. Some people like to stick the spool of filament in the oven to help dry it out a little, but I prefer not to put my plastics where my food goes. For now, I just keep it in a bag with some silica gel which hopefully will keep it pretty dried out. In the future, I'd be interested in doing a comparison of different materials for 3D printing pulleys if anyone would be interested I would be happy to throw together a video or something, and I'll post my settings for those interested.
```

---
## \#13 Posted by: michaeld33 Posted at: 2017-06-14T04:47:17.887Z Reads: 424

```
While that's logical, I also would think that a loose belt is also capable of skipping and creating fiction on the teeth as well, I think it's about finding the neutral zone where it works just right.
```

---
## \#14 Posted by: Boardnamics Posted at: 2017-06-14T04:47:27.248Z Reads: 420

```
Not really sure, as of now I am not even going to bother checking because like I said, I have had no belt slippage before. There is sort of a relationship between the torque deliverable, width of the belt, and tension that I have found. With a wider belt, you need more tension in general which is more frictional loss but it has a higher capability. I have a relatively low powered board so I don't really need a 15mm wide belt anyways, so I am able to run it on such a low tension with no issues at all.
```

---
## \#15 Posted by: michaeld33 Posted at: 2017-06-14T04:51:52.919Z Reads: 424

```
What's your top speed? 

If it's 10+ mph I just don't understand how you can experience zero slippage while riding using a loose belt, but I guess if it ain't broke then don't fix it. Lol

 My belt slips sometimes even when it's on tight.
```

---
## \#16 Posted by: lrdesigns Posted at: 2017-06-14T04:51:55.895Z Reads: 441

```
I have, been about two weeks on this pulley. Previously I was using PCmax filament by polymaker printed on an ultimaker. They lasted a several months. I expect these to last longer as there is no delamination issues and the tooth profile is much more precise. 

Also I would never us PLA for a pulley, it gets soft at too low of a temp. Minimum is ABS in my opinion. 
<img src="/uploads/db1493/original/3X/5/0/5021cc7a3fb5af4c57d676a7adc94973c8851e4f.jpg" width="666" height="500"><img src="/uploads/db1493/original/3X/3/a/3ab4c2aa40fd407ce79231698e73a20d2bc0f506.jpg" width="666" height="500">
```

---
## \#17 Posted by: michaeld33 Posted at: 2017-06-14T04:53:38.743Z Reads: 422

```
That is awesome, are those made on a formlabs as well? Now I need to try one of these bad boys!
```

---
## \#18 Posted by: lrdesigns Posted at: 2017-06-14T04:54:59.966Z Reads: 418

```
Yeah on a form 2. Print time was about 8 hours per piece though. Plus cleaning and post curing in a UV oven.
```

---
## \#19 Posted by: Boardnamics Posted at: 2017-06-14T04:59:33.872Z Reads: 420

```
My top speed with my 12t pulley 31t printed spur is about 17mph flat ground. I am soon switching it out for a 10t but the chinese seller took 2 weeks to package it due to a chinese boat parade :frowning: 5mm pitch 15mm wide is pretty overkill and yeah somehow I get no slipping. The belt is loose enough to be able to slide on the pinion with no effort.
```

---
## \#20 Posted by: michaeld33 Posted at: 2017-06-14T12:31:07.699Z Reads: 391

```
Word ok. If you modify the pulley and try a tighter belt let me know how that affects the riding. Very interesting.
```

---
## \#21 Posted by: JLabs Posted at: 2017-06-14T12:57:57.607Z Reads: 345

```
I would edit your first post so it dosnt give newcomers the wrong idea. I have used 3d printed pulleys countless times and this appears to be user error. So maybe you can say what not to do to help people not have your problem (PLA & friction)
```

---
## \#22 Posted by: mmaner Posted at: 2017-06-14T13:23:10.768Z Reads: 344

```
Me too, I've been using 3D printed ABS wheel pulleys for months on multiple boards, never seen anything like that.
```

---
## \#23 Posted by: 2-alex-2 Posted at: 2017-06-14T13:29:30.410Z Reads: 349

```
Yea I print my own with no issues. Did you use bolts to hold it in place as well or did you only rely on just the 3D print to hold in place.
```

---
## \#24 Posted by: mwkeefer Posted at: 2017-06-14T15:51:54.429Z Reads: 357

```
Michael, I've used printed pulley from ABS, Nylon and some other more esoteric materials available in spools of filament.

A few quick suggestions... Reprint your part at 25% infill (I was on the phone with Mike C while I was reading this so I know your setup) and instead of using it, smooth it with a heatless humidifier and isopropyl alcohol (put the print on an old 33 turn table or motorized lazy Susan to ensure mist is evenly distributed... that will remove the print lines, and artifacts - finally.... get some plaster of Paris and some "Magic Clay" aka play dough and google creating a mold for casting resin with POP and Magic Clay, then call your local auto parts supplier (not pep boys or royal auto a part supplier and get some gear resin mix (google again) and after the mold dries (shit print at 3% over size to account for resin shrinkage and curing...

Now mix the resin and pour the mold, 4 hours later you can free the part and 24 hours later you can use it... same shit as epoxy rules so, if you can fire the resin then the temperature and length of firing to cure the resin will directly effect it's tensile strength, hardness and temperature stability for automotive environment (under hood in summer motor running, car not) which TRUST ME BRO, will never, ever fail you.

Or find someone with a small foundary and have them smelt some 6061 aluminum bar stock filets down, remove the slag (I personally smelt at 1800F which is about 600F above the melting point of aluminum and lets me expose and remove any impurities in the alloy before pouring it into a voided mold made with PLA and burned out in the microwave for 10 minutes till the PLA vaporizes leaving behind the perfect mold to pour the aluminum into to cast your parts (hint, hint... I can smelt and cast stainless in my forge)

Hope this helps you bud, send me a msg if you have any questoins or want clarification...  I could alternatively throw them in one of my print beds and make a few materials to be tested from filament spools I have on hand which are known to produce survivable parts with a decent service life.

-Mike
```

---
## \#25 Posted by: mwkeefer Posted at: 2017-06-14T15:55:32.188Z Reads: 313

```
PLA filaments for me tend to melt and become extrudable at a lower temperature than ABS  (around 180°C to 220°C) and is actually harder than ABS,  also has a glass transition temperature between 60-65 °C, so is potentially a very useful material. **It does exhibit higher friction than ABS**

Combined with your belts and eRPM (and the ambient heat) yea, you way exceeded the intended use of ABS... 

-Mike
```

---
## \#26 Posted by: mmaner Posted at: 2017-06-14T15:58:17.902Z Reads: 318

```
???  
[quote="mwkeefer, post:25, topic:25345"]
Combined with your belts and eRPM (and the ambient heat) yea, you way exceeded the intended use of ABS...
[/quote]

That doesn't make sense, as you dont know what belts I use or what the ERPM is on my board(s)...Am I missing something?
```

---
## \#27 Posted by: Achmed20 Posted at: 2017-06-14T16:41:37.546Z Reads: 313

```
my large pulley is printed in PETG, 100km so far, about 45min of contious usage, not signs of wear at all
my small one is ABS, same usage, no usage at all.

tbh, i think you scrwed something up somwhere/somehow.
```

---
## \#28 Posted by: mwkeefer Posted at: 2017-06-14T17:13:14.572Z Reads: 310

```
Yes,  you're right there was a misprint I was saying you way over did it for PLA filament objects :slight_smile:

  Sorry guys I'm on my way to Manhattan or I'm gonna meet up with a couple of guys from the threads including with a little Kaly.nyc and pick up a sweet trampa build...

 Sad but true I'm just leaving Philadelphia I had to make a pitstop I have one iPad Pro three cell phones within my line of sight and yes I'm using them all as I drive difficult because I'm so damn excited  ( and to be perfectly honest a little bit anxious I haven't been in New York since 911 )

 But I seriously,  you printed 50% and fill in PLA material and  because PLA is harder and has more friction or generates more friction then its counterpart ABS and also cause it's nonflexible which is why it generates more friction, it melted Aka "Indian rope burn"  please don't take me the wrong way I don't mean disrespect I'm not messing with you I have so many failures before I succeed in fact I one time printed a chain ring out of PLA now this was just for filament and I managed to crack like eight or nine of the teeth just putting the chain on it ;)

 I wish I had seen this thread before I left my house in the burbs a Philly auto brought some filament and I are giving it to you or give it to Mike to give to you for better results than the PLA stuff
```

---
## \#29 Posted by: mmaner Posted at: 2017-06-14T17:25:49.651Z Reads: 284

```
I got confused because you replied to the wrong person :).  I print mine with ABS 100% infill. It was @michaeld33 that had the melting issue.
```

---
## \#30 Posted by: Chicagojoshua Posted at: 2017-06-23T02:25:18.067Z Reads: 266

```
I have over 800 miles on ABS and Nylon pulleys. You probably have some real cheap filament.
```

---
## \#31 Posted by: TheFluffiest Posted at: 2018-02-24T08:47:38.060Z Reads: 216

```
I'm having problems getting my nylon pulley to stay on the motor. How do you mount your 3d printed pulleys?
```

---
## \#32 Posted by: e.board_solutions Posted at: 2018-02-24T09:00:02.050Z Reads: 213

```
You mean the wheel pulley? Do you have a picture?
```

---
## \#33 Posted by: TheFluffiest Posted at: 2018-02-24T09:06:45.960Z Reads: 210

```
No, I mean the motor pulley. It keeps falling off the shaft. No problems with teeth or anything, it just won't stay on the shaft.
```

---
## \#34 Posted by: e.board_solutions Posted at: 2018-02-24T09:08:17.677Z Reads: 215

```
3D printed pulleys for motor is not commonly used, do you have a picture?
```

---
## \#35 Posted by: TheFluffiest Posted at: 2018-02-24T09:33:39.936Z Reads: 214

```
I don't currently, I just finished the printing a new motor mount. It's only temporary until I can afford metal ones. I've heard people be successful, but only with nylon or polycarbonate. I will hopefully upload a photo tomorrow
```

---
## \#36 Posted by: e.board_solutions Posted at: 2018-02-24T09:42:48.209Z Reads: 218

```
You use HTD5? 8mm axle? Where are you from? 
Maybe [this](https://www.aliexpress.com/item/Durable-HTD5M-5M-Aluminum-Timing-Belt-Drive-Pulley-15-Teeth-8mm-Hole-16mm-Width-Stepper-Motor/32830484749.html?ws_ab_test=searchweb0_0,searchweb201602_5_10152_10151_10065_10344_10068_10342_10343_10340_10341_10084_10083_10618_10630_10304_10307_10302_5711211_5722315_10313_10059_10534_100031_10103_10627_10626_10624_10623_10622_10621_10620_10142_5711312-10152,searchweb201603_1,ppcSwitch_5&algo_expid=89f02687-3a50-482b-b7d1-ceaa110403bd-4&algo_pvid=89f02687-3a50-482b-b7d1-ceaa110403bd&priceBeautifyAB=0) could work?
```

---
## \#37 Posted by: banjaxxed Posted at: 2018-02-24T23:09:17.260Z Reads: 214

```
Put a grub screw or two in and use some thread lock, some just run with threadlock if need 24h to cure properly. POM/nylon/petg may have a chance to not strip teeth for a while, better to use an extra tooth like 16T to help spread the load a bit more.

You sure you can't spring for $5 for alloy gear
```

---
## \#38 Posted by: FredrikHems Posted at: 2018-02-24T23:14:20.594Z Reads: 213

```
[quote="banjaxxed, post:37, topic:25345"]
$5
[/quote]

Bro, you are getting ripped of with that 
ridiculous price! 

I got some aluminium ones for $2!
```

---
## \#39 Posted by: GrecoMan Posted at: 2018-02-24T23:22:54.816Z Reads: 205

```
threadlock dissolves plastic
```

---
## \#40 Posted by: banjaxxed Posted at: 2018-02-24T23:30:37.587Z Reads: 200

```
I'm including shipping, ah and yes threadlock will eat plastic true
```

---
## \#41 Posted by: FredrikHems Posted at: 2018-02-24T23:31:59.875Z Reads: 189

```
Haha. I was just kidding :grin: :joy:
```

---
## \#42 Posted by: TheFluffiest Posted at: 2018-02-24T23:46:27.784Z Reads: 184

```
It is already a 16t, and I haven't had much success with getting a grub screw to stay in. I will very soon, I just want to ride now :joy: Where are you getting that pulley? I need a htd5m 15mm wide 14-16t 6mm bore, and I have had lots of problems finding that with fast shipping
```

---
## \#43 Posted by: GrecoMan Posted at: 2018-02-25T00:06:28.453Z Reads: 180

```
6mm bore? who the hell uses motors with 6mm shafts anymore?
```

---
## \#44 Posted by: TheFluffiest Posted at: 2018-02-25T02:53:37.972Z Reads: 181

```
Someone who got dual sk3 5055 :joy: I didn't realize they were 6mm bore, otherwise I would have found something else. Dual, less torque-y motors is why I think 3d printed motor pulleys won't be a problem
```

---
## \#45 Posted by: GrecoMan Posted at: 2018-02-25T02:54:55.740Z Reads: 178

```
are you in the US?
```

---
## \#46 Posted by: TheFluffiest Posted at: 2018-02-25T03:30:18.850Z Reads: 173

```
Yes. I can find them, the problem is inexpensive, fast shipping
```

---
## \#47 Posted by: GrecoMan Posted at: 2018-02-25T03:33:36.910Z Reads: 174

```
i might be able to dig up 2 tomorrow. i’ll let you know, if I can find them, you just owe me $2.50 shipping :)
```

---
## \#48 Posted by: stormboard1 Posted at: 2018-02-25T05:36:48.611Z Reads: 171

```
How dju get aluminium one for 2 dollars link or didn’t happen 😂
```

---
## \#49 Posted by: GrecoMan Posted at: 2018-02-25T13:41:07.690Z Reads: 167

```
https://m.ebay.com/itm/HTD5M-15-Aluminum-Timing-Belt-Pulley-15-Teeth-8mm-Bore-16mm-Width-Stepper-Motor/302418153225?epid=1339404249&hash=item466986cf09:g:z-UAAOSwl~tZlPDt
```

---
## \#50 Posted by: TheFluffiest Posted at: 2018-02-26T08:45:31.822Z Reads: 164

```
Wait really? That is awesome, thank you so much!
```

---
## \#51 Posted by: notepad Posted at: 2018-02-26T22:14:09.089Z Reads: 157

```
I have only skim read the post so I might be repeating myself here.

That melt pattern is definitely that of PLA.  the average belt temperature of an Esk8 is 42C which is enough to slightly soffern the material, which will lead to deformation and more heat- so on and so on.

ABS is decent but can shrink a bit which will cause a slight melt pattern on the tread which will rehardern after melting.    PETG and NY are the best and I have been using dual PETG 40T gears for about 300Km with no problems.

If you do want bulletproof,  get them printed in an impact resistant resin.
```

---
## \#52 Posted by: TheFluffiest Posted at: 2018-02-27T06:56:47.914Z Reads: 151

```
Did you manage to find them?
```

---
## \#53 Posted by: TheFluffiest Posted at: 2018-02-27T06:58:39.962Z Reads: 147

```
Successfulling using 3d printed motor pulleys as of today. Printed in Taulmann Bridge Nylon with 7 perimeters, 50% infill, .2mm layer height. Went pretty fast, stopped hard, very little slippage. Highly recommend using nylon, it is made for this sort of purpose
```

---
## \#54 Posted by: GrecoMan Posted at: 2018-02-27T11:57:17.087Z Reads: 137

```
i was only able to find one.
```

---
## \#55 Posted by: banjaxxed Posted at: 2018-02-27T12:49:59.258Z Reads: 138

```
He's using printed MOTOR pulleys, less teeth more strain
```

---
## \#56 Posted by: riva_00 Posted at: 2018-02-27T14:14:06.012Z Reads: 131

```
I'm considering using PETG for the motor pulley, 18~20 teeth. I'm not sure if that'll survive but i'll be testing with plenty of armor. Hoping the high tooth count will help.

I have a 60~72 tooth wheel pulley printed in ABS and it works fine.
```

---
## \#57 Posted by: TheFluffiest Posted at: 2018-02-27T16:37:54.092Z Reads: 124

```
It's all good, the nylon is actually working really well! Thanks anyways, this community is awesome!
```

---
