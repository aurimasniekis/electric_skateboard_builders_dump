# High speed (40-50 mph) build! I need advice/help please

### Replies: 177 Views: 9346

## \#1 Posted by: KeivanM Posted at: 2017-10-24T19:11:34.310Z Reads: 635

```
Okay so I am trying to build a longboard that will have a maximum speed of 40-50 mph & go a range of 12 miles or above. 

I am 17 years old, 145 pounds and am very decent at longboarding at high speeds. This isn’t my first electric longboard and have gone up to 30 before and I am craving that 40-50 mph range. 

I want to plan this build out first and was thinking of these components 


PARTS: 

Motors (2 of them): 
http://alienpowersystem.com/shop/brushless-motors/aps-6384s-sensored-outrunner-brushless-motor-200kv-4000w/


VESC (2 of them):
collections/featured-items/products/torque-esc-vesc-bldc-electronic-speed-controller

Battery(4 of these, 2 in series and 2 in parallel to double both the (s) and (mAh)): 
https://hobbyking.com/en_us/multistar-high-capacity-6s-5200mah-multi-rotor-lipo-pack.html

Deck: I’m not sure, any recommendations? 

Wheels: Any flywheels at or above 97mm 

Trucks: I’m not sure for this

 These are the parts so far, what I need help/ advice on is, what gear ratio do I use for the motor and where can I get a motor mount and also if what I have will get me to go 40-50 MPH, any suggestions would be SUPER helpful since it’s my first time actually building a electric longboard from scratch!!! 


Thanks :)


Also ps my budget is 800-1100 usd
```

---
## \#2 Posted by: Jedi Posted at: 2017-10-24T19:19:57.863Z Reads: 586

```
Use this: http://calc.esk8.it

Need for speed huh? I would try this motor: https://m.banggood.com/Racerstar-6368-BRD6368-280KV-6-12S-Brushless-Motor-For-Balancing-Scooter-p-1117657.html

It's got a higher kv rating for more speed, you may want to gear it down to a 12-14 tooth motor pulley. It's also got a 10mm shaft, so you'll need a motor pulley with 10mm bore. Eskating.eu has some custom pulleys available. With 10s or 12s you should be able to hit 40+ mph.
```

---
## \#3 Posted by: GrecoMan Posted at: 2017-10-24T19:35:35.071Z Reads: 581

```
most you’d be able to go on 280kv is 6s...
erpm limits 

i recommend a setup along the lines of 190kv with 12s geared like 15/25 for 40mph
```

---
## \#4 Posted by: pennyboard Posted at: 2017-10-24T19:48:52.605Z Reads: 570

```
For batteries those are a good choice and motors seem good. The problem is gearing. Basically with the components you have, you'd have to run somewhere around 18/36T gearing in order to be able to hit 50 mph. I don't know of any E-sk8 vendor that sells motor gears larger than 16T. Check SDPSI.com (http://www.sdp-si.com/products/Timing-Belt-Pulleys/index.php)
I've gotten a few motor gears from there and they've been great so far.

I'd recommend getting the motor mounts, and wheel gears and belts from the same site you got the VESC from. Get caliber 2 trucks to fit the motor mounts off amazon for $35. (Good price considering they are legit caliber trucks and not fakes).

For deck, get something as stiff as possible. Pretty much any longboard deck will do, just make sure its really stiff to avoid speed wobbles (I'm sure you know this as you said you're already a long boarder)
```

---
## \#5 Posted by: willpark16 Posted at: 2017-10-24T19:50:59.960Z Reads: 518

```
Go li ion lipos are boring
```

---
## \#6 Posted by: willpark16 Posted at: 2017-10-24T19:51:58.807Z Reads: 518

```
Please wear proper gear when attempting these speeds last thing we need is someone getting killed or seriously injured and new laws coming in
```

---
## \#7 Posted by: pennyboard Posted at: 2017-10-24T19:53:13.376Z Reads: 516

```
Boring? That's not the word I would use :joy:

<img src="/uploads/db1493/original/3X/6/9/691c248b6fa3f757d145ed74e9f39cf7bd64a180.png" width="690" height="463">
```

---
## \#8 Posted by: pennyboard Posted at: 2017-10-24T19:54:48.764Z Reads: 512

```
But honestly for a board like this, lipos seem the way to go. He wants to stay within budget and he'll need to pull a lot Amps to hit 50 mph, and lipos are better suited for that.
```

---
## \#9 Posted by: willpark16 Posted at: 2017-10-24T19:58:04.729Z Reads: 502

```
1100 dollars means it's possible he should have bought my raptor slayer that's supposed to go 66mph theoretically
```

---
## \#10 Posted by: pennyboard Posted at: 2017-10-24T20:00:41.851Z Reads: 495

```
Okay, you've now peaked my interest, where is is for sale, and how do I get more information on it?
```

---
## \#11 Posted by: willpark16 Posted at: 2017-10-24T20:05:31.485Z Reads: 485

```
Just missed it it ended up going to some guy in New York who's gonna try racing it
```

---
## \#12 Posted by: Brycehoosiers Posted at: 2017-10-24T20:55:20.318Z Reads: 468

```
Torque boards sells 18t motor pulleys
```

---
## \#13 Posted by: Orin635 Posted at: 2017-10-24T20:56:36.019Z Reads: 463

```
Could you get like a 1:2 ratio (1 on the wheel, 2 on the motor) idk if  this would be possible but its an idea
```

---
## \#14 Posted by: Cobber Posted at: 2017-10-24T21:46:12.965Z Reads: 461

```
I wouldn't use a cheap 10C rated lipo... look for something at least 20C or higher discharge. Cheap batteries are often over rated.
I don't know how many times we have to go though this... yawn!

If you want :punch: go lipo for the leaky membrane and it's capacity to deliver big amps on demand
If you want a fecking huge battery go li-ion
```

---
## \#15 Posted by: BigBoyToys Posted at: 2017-10-24T23:50:14.577Z Reads: 443

```
I think youll be lucky to get past 40mph on a belt drive with out risk of your speed your controller blowing due to excessive erpm unless you are using a ridiculously tall gear ratio <2:1. If you are willing to sacrifice the the torque, efficiency and motor heat to get to those speeds Id highly recommend using  an FOC box at least. Better yet consider the VESC 6 (over double the erpm limit of the 4.12 VESCs) with an even higher KV motor so you can keep you gear ratio lower. 

Then of course there's always other options that involve crossing over to the darkside 😉, but we wont talk about those here.
```

---
## \#16 Posted by: pennyboard Posted at: 2017-10-25T01:26:08.663Z Reads: 426

```
I think hitting 50 mph with 2:1 ratio is definitely possible, and arguably the easiest way to hit 50 mph. 

I agree with everything else @BigBoyToys says though. After all, he knows all about those high speed builds
```

---
## \#17 Posted by: JdogAwesome Posted at: 2017-10-25T01:55:37.148Z Reads: 433

```
Normally I wouldn't recommend car ESC like the X-Car Beast one from Hobby King though if this board is meant solely for speed, it's probably gonna be the only way to go due to the ERPM limits of the VESC. Also I would definitely recommend 20C minimum if your going with foil pouch LiPos.
```

---
## \#18 Posted by: BigBoyToys Posted at: 2017-10-25T02:05:12.484Z Reads: 428

```
Maybe it is easy and ive just never seen anybody try it, idk. Im not a high speed belt drive specialist, Ive only thought about the basics involved. To keep under 60k erpm and still hit 50mph you're gonna need under a 2:1 gear ratio even with 107mm super flys. So maybe a 17/32 ratio and hope you can hit 85% theoretical max?

Id actually really love to see this done so I can compare it to my 49mph board in terms of efficiency, start up torque and time to reach top speed :).
```

---
## \#19 Posted by: PXSS Posted at: 2017-10-25T02:16:35.727Z Reads: 425

```
245kV motor
107mm wheels
GR 2:1
12S pack
Max speed under 60k erpm = 53.7mph

Lets say you lose 20% efficiency, you're looking at 42.9mph. 

I would spend my money on dual motors (sk3 6364s) 150 and escs 200. Then 250 for a large ass lipo and bms. 170 for abec 11s. 30 on remote. 100 on motor mounts, gears and belts. Finally 150 on deck and trucks. 50 on enclosure. $1100 build.
```

---
## \#20 Posted by: KeivanM Posted at: 2017-10-26T03:27:46.524Z Reads: 391

```
Okay so should I use 200 KV Motors with 18t/16t and 97 mm wheels with a 12s and VESC?
```

---
## \#21 Posted by: KeivanM Posted at: 2017-10-26T03:28:24.343Z Reads: 361

```
What should I end up using then in terms of kv Motor and ratio and ESC?
```

---
## \#22 Posted by: scepterr Posted at: 2017-10-26T03:32:38.472Z Reads: 354

```
I would seriously consider precision cnc trucks vs cast for 40-50mph
I'm fine with spending $30-$40 in bolts for a 50mph build but not the trucks...
```

---
## \#23 Posted by: pennyboard Posted at: 2017-10-26T03:33:44.361Z Reads: 348

```
Since you're using 12s, don't use more than 190kv motors, or you risk exceeding the vesc's ERPM limit and blowing the vesc. 

For esc, use a vesc. I have one from torque boards and it got a single motor build up to 32 mph, so I imagine with 2 of those vescs running dual motors, the vescs would be able to handle the power required to get to 50 mph and not blow up. If you have room in the budget though, get FOCbox vescs or ollin vescs. The quality on those, particularly on ollin's, is a big step up from torque boards.

Assuming you use 97 mm flywheels, a 20 tooth or 22 tooth pulley on the motors and a 36 tooth pulley on the wheels should get you above 40 mph, maybe even above 50 mph, depending on efficiency, power from your motors, and drag.
```

---
## \#24 Posted by: pennyboard Posted at: 2017-10-26T03:35:16.447Z Reads: 323

```
I'd think $35 caliber 2 trucks would be fine. I've never heard of them breaking, and I'm assuming he's going to be wearing proper safety gear at those speeds even if they do break. But its far more likely he'll fall off than the trucks break.
```

---
## \#25 Posted by: scepterr Posted at: 2017-10-26T03:35:57.547Z Reads: 314

```
It's not about them breaking it's about the precision and tolerances in a CNC truck vs cast

Personally at 30mph I don't find the caliber 2 "stable" , there's definitely some quirkiness that starts to show
```

---
## \#26 Posted by: pennyboard Posted at: 2017-10-26T03:37:57.908Z Reads: 314

```
Why would that make a difference? once the motors are mounted and wheels are rolling I don't see how tolerances matter other than breaking.
I'm not a traditional long boarder so maybe there's something I don't know here, but I've got my fake, chinese caliber 2's well past 30mph and they felt fine

edit: I can see how worse tolerances could lead to wobbles, but I've never experienced any of that.
```

---
## \#27 Posted by: scepterr Posted at: 2017-10-26T03:39:29.001Z Reads: 315

```
There's wiggle where any 2 parts join
You might not even realize until you ride some precision trucks on the same setup
Things that seemed "normal" , vanish and your like huh...
I've found it most evident in high speed cornering
```

---
## \#28 Posted by: mmaner Posted at: 2017-10-26T03:41:54.259Z Reads: 317

```
[quote="pennyboard, post:24, topic:36381"]
caliber 2 trucks would be fine. I've never heard of them breaking
[/quote]

I'll buy you a beer sometime and tell you a story about a caliber 2 axle that came loose inside the hanger at 25mph.  I peed a little 😀.
```

---
## \#29 Posted by: pennyboard Posted at: 2017-10-26T03:41:55.922Z Reads: 302

```
Hmm, yeah that makes sense I suppose. Deffinetly peaked my interest in trying out new trucks. What would you recommend as good precision trucks?
```

---
## \#30 Posted by: pennyboard Posted at: 2017-10-26T03:42:33.977Z Reads: 303

```
I'll deffinetly take you up on that....once I reach the drinking age :joy:
```

---
## \#31 Posted by: scepterr Posted at: 2017-10-26T03:42:54.755Z Reads: 295

```
@psychotiller or @trampa (not sure if there are cnc longboard trucks) on here
Ronin are also great
```

---
## \#32 Posted by: Mikenopolis Posted at: 2017-10-26T03:44:50.666Z Reads: 275

```
Tsk tsk. Offering alcohol to a minor. Hahaha
```

---
## \#33 Posted by: mmaner Posted at: 2017-10-26T03:45:18.022Z Reads: 279

```
I didn't know, I swear officer 😀.
```

---
## \#34 Posted by: scepterr Posted at: 2017-10-26T03:45:35.550Z Reads: 288

```
It was root beer...right...
```

---
## \#35 Posted by: Mikenopolis Posted at: 2017-10-26T03:47:01.665Z Reads: 285

```
Totally understandable. @pennyboard was wearing a lot of makeup and looks older
```

---
## \#36 Posted by: pennyboard Posted at: 2017-10-26T03:49:34.790Z Reads: 287

```
*casually puts on fake mustache*
```

---
## \#37 Posted by: zpoole27 Posted at: 2017-10-26T03:49:35.971Z Reads: 290

```
Most of this can be mitigated by using proper pivot cups, quality bushings, bushing inserts, and sleeved washers. 

These are the main things people don't focus on enough, but are immensely suprised in the gains you get from quality pivot cups on ANY truck. That's where every brand seems to cut corners.
```

---
## \#38 Posted by: scepterr Posted at: 2017-10-26T03:50:33.504Z Reads: 288

```
Yah, I've spent more than the price of the caliber trucks replacing all the parts I can lol
```

---
## \#39 Posted by: dickyho Posted at: 2017-10-26T03:50:55.850Z Reads: 290

```
Wow,  50mph=80km/h.  that would be very very danger for eboard!!!   remenber insurance youself first......, but dont drink before drive, otherwise will not got coverd.

in that speed, the motor will sucking a lot of power, I suppose a 30C battery would be better.  and 5200mah LIPOis too less, will drain very soon.

big wheels are certainly.   High KV motor would be better, maybe 400KV.    and full ceramic bearings is needed, because metal bearings alway produce heat in high speed, will melt the wheel sometimes.

I once have a 5065 400KV board can hit 55km/h.
```

---
## \#40 Posted by: pennyboard Posted at: 2017-10-26T03:51:05.038Z Reads: 284

```
Come to think of it, I rode one of psychotiller's board and was amazed at how refined and smooth it felt. Probably due to the massive flywheels on it, but I'm sure the trucks played a role as well.
```

---
## \#41 Posted by: pennyboard Posted at: 2017-10-26T03:52:04.063Z Reads: 272

```
400kv running on 12s voltage is almost guaranteed to blow the VESC
```

---
## \#42 Posted by: BigBoyToys Posted at: 2017-10-26T03:53:07.592Z Reads: 265

```
Dickyho must use vesc6's too 😉
```

---
## \#43 Posted by: dickyho Posted at: 2017-10-26T03:53:26.965Z Reads: 271

```
I was use normal 150A RC ESC , it lasted a long time on that board....
```

---
## \#44 Posted by: pennyboard Posted at: 2017-10-26T03:54:00.368Z Reads: 271

```
I stand corrected. How'd they perform?
```

---
## \#45 Posted by: dickyho Posted at: 2017-10-26T03:56:59.263Z Reads: 273

```
I think the RC ESCs are good, just control will not smoothly as VESC, and no regen braking.  and  braking always will do damage to the ESC....
```

---
## \#46 Posted by: jrpwit Posted at: 2017-10-26T04:18:49.897Z Reads: 267

```
Those lips are only 10c that's weak!
```

---
## \#47 Posted by: BigBoyToys Posted at: 2017-10-26T04:26:09.542Z Reads: 269

```
Yeah maybe a bit higher 200-245 as suggested by PXSS
```

---
## \#48 Posted by: KeivanM Posted at: 2017-10-26T11:38:10.550Z Reads: 282

```
after Reading all these comment, should I get these parts? 18/36 gr

So far these are the parts I am planning to get 


MOTORS(2x):https://hobbyking.com/en_us/turnigy-aerodrive-sk3-6364-213kv-brushless-outrunner-motor.html


VESC(2x):collections/featured-items/products/torque-esc-vesc-bldc-electronic-speed-controller


BATTERY(2x):https://hobbyking.com/en_us/zippy-compact-6200mah-6s-40c-lipo-pack-xt90-1.html


WHEELS(1x): https://www.ebay.com/i/263173335334?chn=ps&dispItem=1&ul_ref=http%253A%252F%252Frover.ebay.com%252Frover%252F1%252F711-117182-37290-0%252F2%253Fmpre%253Dhttps%25253A%25252F%25252Fwww.ebay.com%25252Fi%25252F263173335334%25253Fchn%25253Dps%252526dispItem%25253D1%2526itemid%253D263173335334%2526targetid%253D376529821623%2526device%253Dm%2526adtype%253Dpla%2526googleloc%253D9007580%2526poi%253D%2526campaignid%253D936467927%2526adgroupid%253D47513584075%2526rlsatarget%253Dpla-376529821623%2526abcId%253D1129666%2526merchantid%253D8562084%2526gclid%253DCjwKCAjw7MDPBRAFEiwAppdF9EQiFavHmVCJM8GKFNNL3LkRtxegKPA9uDWTd9QRjWfQ7aL43OKbZhoCjKUQAvD_BwE%2526srcrot%253D711-117182-37290-0%2526rvr_id%253D1345486352683


TRUCKS(1x): https://www.amazon.com/gp/aw/d/B00J5J6B0U/ref=mp_s_a_1_4?ie=UTF8&qid=1508951815&sr=8-4&pi=AC_SX236_SY340_QL65&keywords=caliber%2B2%2Btrucks&dpPl=1&dpID=31gL0kYlgVL&ref=plSrch&th=1&psc=1 


GEARS(combo): 

- for motor : collections/motor-pulleys/products/18t-htd5-12mm-motor-pulley
- for wheel : collections/drive-wheel-pulleys/products/36t-abec11-drive-wheel-pulley-only

MOTOR MOUNTS(2x):products/single-bolt-on-motor-mount-set-only-black

DECK:(1x): http://www.skateshred.com/index.php/wholesale-blank-longboard-decks/36-x-9-5-downhill-kicktail-canadian-maple-cmdh36-461.html

Controller & Receiver(1x): collections/remote-controller/products/torqueboards-2-4ghz-mini-remote-controller
```

---
## \#49 Posted by: KeivanM Posted at: 2017-10-27T16:06:49.795Z Reads: 251

```
So do you think I can get it to 40 plus while using 213 KV, 12 s, and the 18/36 ratio?
```

---
## \#50 Posted by: Jedi Posted at: 2017-10-27T16:37:45.688Z Reads: 255

```
Yes, but what's the point. If your not going to break the Guinness record (59.55 mph) then why even try. Go big. Shoot for 70 mph. You can do it. You're a legend.
```

---
## \#51 Posted by: KeivanM Posted at: 2017-10-27T22:32:12.773Z Reads: 248

```
Okay, so how do I achieve 70 mph???
```

---
## \#52 Posted by: KeivanM Posted at: 2017-10-27T22:32:24.648Z Reads: 256

```
How should I approach going 70 mph
```

---
## \#53 Posted by: GrecoMan Posted at: 2017-10-27T22:38:17.872Z Reads: 263

```
please don't try to go 70mph.

if you haven't read enough to know that 213kv with 12s will blow your vesc. also, how are you going to combat speed wobbles? how are you gonna accelerate that much?
```

---
## \#54 Posted by: Youssless Posted at: 2017-10-27T23:00:50.252Z Reads: 266

```
You should be able to hit 45+mph according to the calc but I do worry about safety and, as @GrecoMan mentioned, your knowledge and experience since you should know that 213KV at 12S will exceed the 60k erpm limit and will blow your VESCs. 

I highly recommend getting your setup with a 190KV motor and smaller motor pulley (15 is good). Once you've all the safety equipment and have ridden loads (like 500miles) in different situations and know the limits of your brakes, how your board handles, speed wobbles and how to position yourself on your board to reduce drag and gain more control AND done loads more reading THEN, MAYBE, consider getting a bigger motor pulley to go at faster speeds on very empty places but still with someone who can call the ambulance should, God forbid, anything go wrong and you crap your pants.

Hope thoughts above are useful.
```

---
## \#55 Posted by: KeivanM Posted at: 2017-10-28T02:12:36.688Z Reads: 254

```
Okay I’ll go with the 190 KV motor, using 12s, would this be a problem since the motor says 10s on the website?
```

---
## \#56 Posted by: BigBoyToys Posted at: 2017-10-28T03:00:37.666Z Reads: 258

```
It will only exceed the erpm limit while free reving without load and only on a full charge. The loaded erpm will be well below the limit. Also, consider the voltage sag occurring under that sorta load and youll see he'll be even further below the limit. The FOC box has also been spotted on video exceeding 60k erpm without having issue. (Ive seen video of an FOC box at 100k erpm). A 200+ kv and using a 60K erpm limit in the vesc is gonna be your best bet to keep the lowest gearing possible.
```

---
## \#57 Posted by: Youssless Posted at: 2017-10-28T08:06:47.711Z Reads: 244

```
Thanks for the insight, I guess I shouldn't be so rigid with numbers.
```

---
## \#58 Posted by: BigBoyToys Posted at: 2017-10-28T08:27:34.278Z Reads: 244

```
Error on the side of caution is a good thing, but since breaking 50mph seems like a tall order to me I think he'll have to push the envelop a bit. Especially if henwants it to still be ridable at low speeds. I agree with you on your comments about safety for sure. 40+ on a skateboard feels super intense, hoping on a brand new build and blasting up to high speed is a terrible Idea lol.  I rubbed right through a full leather jacket going down on my eboard at 41mph.
```

---
## \#59 Posted by: pat.speed Posted at: 2017-10-28T10:02:12.116Z Reads: 247

```
Obviously he's going to use the skateboard stabilisers 😂
```

---
## \#60 Posted by: KeivanM Posted at: 2017-10-28T14:13:48.139Z Reads: 251

```
Okay so if I use a VESC from the diyelectricskate site, I should be using 12s and a 213 and I don’t blow the VESC? Also the gear ratio I’m gonna keep is 18/36 to get that high speed, do you think the breaking and regenerative breaking will be fine? I’m gonna use 2 6s 6200 mah, 40C batteries connected in series & a dual XT90 connector to connect the VESCS
```

---
## \#61 Posted by: KeivanM Posted at: 2017-10-28T19:09:36.839Z Reads: 237

```
So I am using a 12s battery(2 6s, 6200mAh 40C in series), a 18/32 gear ratio, and a VESC from diyelectricskateboards. What my question is what motor should I choose.

hobbyking.com1

Turnigy Aerodrive SK3 - 6364-213KV Brushless Outrunner Motor

Turnigy Aerodrive SK3 - 6364-213kv Brushless Outrunner Motor

OR

hobbyking.com2

Turnigy Aerodrive SK3 - 6374-192KV Brushless Outrunner Motor

Turnigy Aerodrive SK3 - 6374-192kv Brushless Outrunner Motor
I am aware of the 60,000 ERPM limit recommendation and I used calc.esk8.it and both choices are very close to that limit.

My goal with this board Im building is to go as fast as possible, so I am not sure which motor to choose, because one says it takes 10s and one says 12s and im not sure what the W or T or A mean for each motor and what that will do to speed, acceleration, range and so on.

Sorry if im bothering you with my question btw
```

---
## \#62 Posted by: PXSS Posted at: 2017-10-28T19:36:22.867Z Reads: 223

```
To add to what @BigBoyToys said. There is also an erpm limit setting. You can simply set it to 60k erpm snd you won't exceed it, even with a 300kv and 12s. 

As long as you have the correct settings, you should be fine.
```

---
## \#63 Posted by: Rob69de Posted at: 2017-10-28T19:42:07.167Z Reads: 222

```
Most if not all electric motors, the KV is lower than advertised
```

---
## \#64 Posted by: BigBoyToys Posted at: 2017-10-28T19:50:32.311Z Reads: 220

```
Good point!
```

---
## \#65 Posted by: KeivanM Posted at: 2017-10-29T00:37:20.162Z Reads: 215

```
ok! thanks
```

---
## \#66 Posted by: pat.speed Posted at: 2017-10-29T01:12:20.363Z Reads: 213

```
Yes but the motor will just never reach its max speed
```

---
## \#67 Posted by: PXSS Posted at: 2017-10-29T01:13:11.017Z Reads: 211

```
So? It doesn't need to
```

---
## \#68 Posted by: pat.speed Posted at: 2017-10-29T01:14:12.240Z Reads: 217

```
Yes I know that. But you might as well choose a lower kv motor that is running at its max speed when it's near 60k. That way it will produce more torque
```

---
## \#69 Posted by: pennyboard Posted at: 2017-10-29T01:45:17.897Z Reads: 224

```
If you want to break 70mph, you're going to need 2 things. 

1) A LOT of power. Air resistance starts to be a factor at 40+ mph, so at 70 mph, you'll need some serious power to overcome it. I'd recommend 4 wheel drive with 2500 watts per motor At Minimum. To be safe, I'd say run 2 motors per wheel, that are about 2500 to 3500 watts each, which should put you in the neighborhood of 25 to 35 horsepower, depending on exactly which motor you go with. The other reason you need a lot of power is...

2) a Tall gear ratio. As in get 8 inch pneumatic wheels and instead of running 60 teeth gears on them like most people do, run normal 36 Tooth gears on them, and then on the motor run somewhere around 15 or 16 tooth gears. The tall wheels will greatly reduce your torque in exchange for top speed, which is why you need all the power from your motors. 

All in all, it'd cost roughly 5-10k USD to create a build that would reliably break 70 mph. Not worth it in my opinion unless it's your life dream, or you just have extra money sitting around.
```

---
## \#70 Posted by: PXSS Posted at: 2017-10-29T02:42:00.027Z Reads: 221

```
Scenario 1:
190kv at 12s:
Fully charged: 50.4v = 67k erpm
Nominal: 43.2v = 57.5k erpm
Empty: 30c = 39.9k erpm

Scenario 2:
240kv at 12s:
Fully charged: 50.4V = 84.6k erpm
Nominal: 72.6k erpm
Empty: 50.4k erpm

---

If both configurations are limited to 60k erpm:
Lets say the battery voltage sags 3.6v under load, which isn't crazy, scenario 1 can only reach 60k erpm if the battery is fully charged. Once the battery is at 90%, it can no longer do 60k erpm. Scenario 2 can reach 60k erpm even if the battery is under 50% charged. Therefore it can maintain that top speed for way longer than scenario 1. 

---

Now on to torque:

For any power condition:
A set voltage and current, scenario 1 will be slower but have more torque while scenario 2 will be faster and have less torque. 

If the rider is looking for a board that accelerates hard and is powerful at low speeds, I agree that a low kv would be better but for a setup that is meant to go up to 50mph, he'll need the higher kv.
```

---
## \#71 Posted by: pat.speed Posted at: 2017-10-29T03:33:05.403Z Reads: 199

```
Hmm yes ok I see your point on the higher kv motor. For me personally though I would choose the lower one so that I have more torque. Also I'm not sure a 240kv motor would be powerful enough to get him moving with the sort of gearing he is going to need. Dual would be a must for this build. I just calculated it and he is going to need a 1.7:1 gear ratio and 97mm wheels to achieve nearly 50mph
```

---
## \#72 Posted by: KeivanM Posted at: 2017-10-29T03:51:51.941Z Reads: 199

```
YOU ARE A GOD ! Thank you for your incredible explanation, I’m going to go with the 245 KV SK3 motor from hobby king And that 12s and the VESC!! I’ll be buying those parts soon, thanks again :)))
```

---
## \#73 Posted by: KeivanM Posted at: 2017-10-29T03:52:08.574Z Reads: 197

```
What gear ratio would be best?
```

---
## \#74 Posted by: PXSS Posted at: 2017-10-29T08:12:00.650Z Reads: 187

```
I don't think he'll have issues getting up to speed with dual 6374s. 

@KeivanM 
I would personally go with 107mm wheels and 2:1gr for a max theoretical of 53.7mph. So 45ish after losses. So 18/36?
```

---
## \#75 Posted by: scepterr Posted at: 2017-10-29T10:12:16.561Z Reads: 184

```
I would certainly go with an upgraded vesc like the ollin vesc or vesc6. I wouldn't use a standard vesc4, especially from a vendor with an unknown track record with vescs.

*I would not want to experience the "speed boost' at  30-50mph*
```

---
## \#76 Posted by: pshaw Posted at: 2017-10-30T02:44:32.358Z Reads: 195

```
[quote="scepterr, post:75, topic:36381, full:true"]
I would certainly go with an upgraded vesc like the ollin vesc or vesc6. I wouldn't use a standard vesc4, especially from a vendor with an unknown track record with vescs.

*I would not want to experience the "speed boost' at  30-50mph*
[/quote]

speaking of speed boosts my buddy had a vesc then switched to a focbox and said it went away. But if I recall I thought this was a hardware issue of noise on the current sensor. Both escs share the more of less the same hardware. Can anyone back this up?
```

---
## \#78 Posted by: KeivanM Posted at: 2017-10-30T04:31:32.598Z Reads: 181

```
Can’t I just set the limit to 60k? On the Vesc & it won’t blow or get all jacked up , right?
```

---
## \#79 Posted by: scepterr Posted at: 2017-10-30T04:39:26.440Z Reads: 183

```
That setting isn't meant to correct an over limit configuration, it's there incase you go over
```

---
## \#80 Posted by: willpark16 Posted at: 2017-10-30T15:15:26.732Z Reads: 185

```
I'm suprised people are endorsing this idea, 70mph is much too fast for someone who doesn't understand the electronics taking them that fast not to mention a minor. Speeds like this should only be attempted in the safest of environments. This is a good way to get boards banned
```

---
## \#81 Posted by: michichopf Posted at: 2017-10-30T15:31:52.673Z Reads: 195

```
absolutely agree. Furthermore even if he goes trough with it he is literally pushing alot of boundaries, meaning alot COULD go wrong. I think between me starting taking freeriding and downhill seriously until I hit 60mph were years. Years in which I went riding 2-3 times a week, with proper instructers and teachers who were world champions nontheless. 

They were all about balls to the wall fast but with safety and brain. Got burned into me that whenever I want to push my limits you need to be able to do everything on that speed you want to beat. Coleman, toeside, drift, speedcheck, full stop etc. So you are even able to react when shit goes south. Speed is fun, pushing boundaries is thrilling but I already lost a beatiful human being this year to his willigness to take risks where caution would have been advised. Going over you own limit is super dangerous. (You dont need 70mp/h to kill yourself, 40 is plenty when you loose your laine and go outline into a car....

Other thing is, going speed even close to 60/70mp/h needs so much set up. Pefect conditions, super familiar with the road and its conditions. Then porper hardware, from the wheels, trucks and board. So if you would ask me, would you want to go 60mp/h+ on 97mm or even 107mm wheels ? Hell no. On stock caliber 50 ? Jesus no. On a set up that wheigs close to 10-14KG ? nononono. 
Then come things like having race leathers with all the protection, a full face, gloves, closed of road, safety nets, medics on point, you in your best shape.

Considering just for fun or as a free time vehicle ? ludacris. That would be worthy of a Darwin Award if anything would happen and where to be discussed between Worldcup riders....
```

---
## \#82 Posted by: KeivanM Posted at: 2017-10-30T18:52:57.035Z Reads: 174

```
What do you mean? So if my ERPM is 78k, and I set the limit to 60k on my VESC, will it stay under 60k or go to the 78k? Because if it does then it’ll blow my VESCS
```

---
## \#83 Posted by: maxhost4 Posted at: 2017-10-30T21:25:59.426Z Reads: 180

```
Before I throw my 2 cents in here, I'm gonna agree wholeheartedly with @willpark16 - If you're really gonna try this, eliminate ALL dangerous variables. I don't want to hear about this project on the news cause your board gave out on you. 

That being said, I appreciate projects that seems insane on the first pass. Here are some tips I can think of that are gonna make this safe/more achievable.
1. If possible, test ride your deck/trucks at a higher speed before strapping the motors on. Familiarity on a deck will be huge when you actually try it.
2. You're going to want your center of gravity to be as low as possible. If possible, mount all your electronics/batteries on top of the deck and run your motors outside your deck. Lower deck=more stability.
3. Look at what downhill boarders use whenever they make their speed runs. Those guys are used to hitting high speeds. They know their stuff, especially when it comes to truck/wheel setup.
4. Soft wheels are ideal. You don't wanna slide at 40mph.
5. From what I've read, you're going to want smaller (75mm-ish) wheels for high speed. You'll have to get clever with your gearing/motor choice but it will keep you safe when you actually try going for it.
6.Make your wheelbase as long and as wide as you can without losing maneuverability. 
7.Make sure you configure your VESC so that if something happens, your motors don't lock up on you. 
8. Don't do this alone. If something (anything) goes south, you want people ready to make sure you'll be okay.

Overall, be smart, do your research, and don't take any unnecessary risks. I'm excited to see how this comes together. Ask questions- better to find out you're wrong now than when you're on the road. Good luck man.
```

---
## \#84 Posted by: KeivanM Posted at: 2017-10-31T00:06:58.400Z Reads: 169

```
yeah im not really trying to go 70 mph, they were just joking, im aiming for 40mph
```

---
## \#85 Posted by: KeivanM Posted at: 2017-10-31T01:09:30.358Z Reads: 166

```
dont worry im actually aiming for around 40 max under safe conditions
```

---
## \#86 Posted by: KeivanM Posted at: 2017-10-31T01:09:51.699Z Reads: 165

```
what do you mean by the "speed boost" on your FOCBOX??
```

---
## \#87 Posted by: willpark16 Posted at: 2017-10-31T01:17:12.703Z Reads: 166

```
40 is much more realistic stay off the city steets with it though aim for open road full throttle. Build around your battery which for this would need to be 10 or 12s
```

---
## \#88 Posted by: chuttney1 Posted at: 2017-10-31T01:37:02.662Z Reads: 168

```
No one should attempt to go 50 mph or higher unless you have adequate protection like wearing motorcycle gear at this point. Dress for the slide, not style. You probably break both your legs and maybe a clavicle in the fall of your board.
```

---
## \#89 Posted by: KeivanM Posted at: 2017-10-31T03:19:50.861Z Reads: 172

```
okay i will do that, should i buy 2 lipos and connects them in series or should i buy lithium ion, OR should i make my own lithium ion pack with singular cells?
```

---
## \#90 Posted by: KeivanM Posted at: 2017-10-31T03:20:05.212Z Reads: 168

```
yeah, im not trying to die ahahahhah
```

---
## \#91 Posted by: willpark16 Posted at: 2017-10-31T03:22:39.636Z Reads: 167

```
Lithium ion is good for the long run and can be much safer/easier
```

---
## \#92 Posted by: mmaner Posted at: 2017-10-31T03:24:23.823Z Reads: 164

```
From.my personal experience, and I actively run lipo and li-ion, a well made 10s4p 30q pack is as good as high C lipos.  Li-ion is a lot more expensive but it supports more charge cycles so it equals out. 

Mathematically lipos have more available amp delivery but the loss after substantial charge cycles is substantial.  After 15'ish builds I would NOT consider running a lipo build at 10s or greater without a BMS so the price point gets even closer.
```

---
## \#93 Posted by: KeivanM Posted at: 2017-10-31T03:24:27.610Z Reads: 157

```
okay, can you point me in the right direction where i can find info about adding a on/off switch, and an easy charging method for recharging the battery and not having to worry about it overcharging and being dangerous?
```

---
## \#94 Posted by: KeivanM Posted at: 2017-10-31T03:25:48.763Z Reads: 156

```
okay thanks for that info, i think im going to go with lithium ion due to the charging management and safety
```

---
## \#95 Posted by: mmaner Posted at: 2017-10-31T03:26:31.344Z Reads: 154

```
The simplest solution is a Bestech BMS which has a power switch.   It's good for lipo or li-ion, although you will want to get the cutoffs programmed differently when you order the BMS, based on the chemistry you choose.
```

---
## \#96 Posted by: willpark16 Posted at: 2017-10-31T03:26:31.600Z Reads: 146

```
Well first are you going to build it or buy it
```

---
## \#97 Posted by: KeivanM Posted at: 2017-10-31T03:28:17.410Z Reads: 162

```
either way works to be honest
```

---
## \#98 Posted by: KeivanM Posted at: 2017-10-31T03:28:25.198Z Reads: 167

```
okay ill keep that in mind
```

---
## \#99 Posted by: willpark16 Posted at: 2017-10-31T03:30:46.547Z Reads: 162

```
I'd say but if you have no experience in building because it will usually be more expensive to build it yourself than buy it if you don't have the tools
```

---
## \#100 Posted by: mmaner Posted at: 2017-10-31T03:31:01.961Z Reads: 165

```
Talk to @Namasaki, he knows more about Bestech BMS's then sooner i know.
```

---
## \#101 Posted by: KeivanM Posted at: 2017-10-31T03:32:35.483Z Reads: 165

```
okay, if i buy a premade lithium ion pack, am i able to still add on a bms, switch, and charger port?
```

---
## \#102 Posted by: willpark16 Posted at: 2017-10-31T03:32:58.329Z Reads: 149

```
All that comes with a properly assembled battery pack
```

---
## \#103 Posted by: KeivanM Posted at: 2017-10-31T03:33:19.956Z Reads: 149

```
okay i will do that
```

---
## \#104 Posted by: KeivanM Posted at: 2017-10-31T03:34:40.072Z Reads: 151

```
ok thanks perfect
```

---
## \#105 Posted by: pat.speed Posted at: 2017-10-31T04:47:40.420Z Reads: 148

```
@willpark16 actually builds batteries if I remember
```

---
## \#106 Posted by: willpark16 Posted at: 2017-10-31T04:57:21.318Z Reads: 151

```
Thanks pat and yea I do depending on what your looking for and the time frame I can probably help you out
```

---
## \#107 Posted by: racidon Posted at: 2017-10-31T05:16:16.387Z Reads: 153

```
@KeivanM it might be worth mentioning (may have already, I skimmed most of the thread) that riding a barebones board at those speeds is completely different to riding an electric board at those kinds of speeds. 
I'd suggest making sure you **_break-in_** your board first to make sure any issues are ironed out at lower speeds, rather than at full speed.
Also take note of the temperature your VESC/ESC hits when doing this too, because having it overheat at 40mph and cutting power on you could shock you enough to loose balance.
Speedwobbles shouldn't be a problem if you're proficient enough at riding a board at high speeds. 
I'd also agree with @BigBoyToys original suggestion, I get that Hubs get a lot of hate at times, but Top speed is definitely where they win
However if you really want to go with belt, I'd suggest a large wheel, and if you're not used to riding a board at those speeds then I'd suggest going with pneumatic instead of thane.
```

---
## \#108 Posted by: BigBoyToys Posted at: 2017-10-31T05:56:10.898Z Reads: 153

```
Have you found pneumatics to be more stable at high speed?
```

---
## \#109 Posted by: chaka Posted at: 2017-10-31T14:13:04.355Z Reads: 154

```
>  I get that Hubs get a lot of hate at times, but Top speed is definitely where they win

How do you come to that conclusion? I can easily reach 40 to 45 mph on a dual belt drive. Can go faster if I change my ratio.
```

---
## \#110 Posted by: KeivanM Posted at: 2017-10-31T14:52:03.618Z Reads: 154

```
so do you sell these lithium ion batteries that you make? how much if you do? Im looking for a 12s battery that can take me about 12 miles or more on one charge.
```

---
## \#111 Posted by: KeivanM Posted at: 2017-10-31T14:52:21.467Z Reads: 152

```
okay thank you for that advice ill take this into consideration!
```

---
## \#112 Posted by: racidon Posted at: 2017-10-31T21:55:42.126Z Reads: 152

```
[quote="chaka, post:109, topic:36381, full:true"]
>  I get that Hubs get a lot of hate at times, but Top speed is definitely where they win

How do you come to that conclusion? I can easily reach 40 to 45 mph on a dual belt drive. Can go faster if I change my ratio.
[/quote]

A 1:1 gear ratio will always reach a higher speed with the equal motor. Obviously if  you can't get the torque to reach the speeds you're screwed. Also obviously if you really wanted you could go a 2:1 ratio on a belt, but that would be pretty rediculous.  I also wasn't saying belt can't reach those speeds, fastest I've gone on one of my belt systems is 80 something km/h and I tend to average 60 on my trampa as a top speed.

[quote="BigBoyToys, post:108, topic:36381, full:true"]
Have you found pneumatics to be more stable at high speed?
[/quote]

**_stable_**.. I wouldn't say more so either direction, but more forgiving yes, I can hit some pretty horrid debris or potholes with the pneumatics where as thane can result in some pretty scary situations at those speeds, or dead stops if I'm going too slow xD
```

---
## \#113 Posted by: chaka Posted at: 2017-10-31T22:15:05.038Z Reads: 142

```
You average 60km/h on a trampa!? whats your top speed?:laughing: They get squirrely at 30km/h, you must have superhuman ankles!
```

---
## \#114 Posted by: racidon Posted at: 2017-10-31T22:23:25.363Z Reads: 152

```
[quote="chaka, post:113, topic:36381, full:true"]
You average 60km/h on a trampa!? whats your top speed?:laughing: They get squirrely at 30km/h, you must have superhuman ankles!
[/quote]

As my top speed I tend to get 60km/h on average. I average about 40-50 on my long rides. I don't find an issue with them, I feel a lot more _comfortable_ on a trampa versus a longboard, but that's mostly to laziness as I find there's less effort to keep stable at those speeds on the trampa.
```

---
## \#115 Posted by: chaka Posted at: 2017-10-31T22:29:45.692Z Reads: 153

```
No offence, but I need to see it to believe it. Never seen someone ride a trampa over 25mph with any amount of confidence. Are you running stock geometry?
```

---
## \#116 Posted by: racidon Posted at: 2017-10-31T22:31:53.337Z Reads: 152

```
[quote="chaka, post:115, topic:36381, full:true"]
No offence, but I need to see it to believe it. Never seen someone ride a trampa over 25mph with any amount of confidence. Are you running stock geometry?
[/quote]

Sadly not, I've been pretty slack lately with it. I got a real case sorted and then I never really bothered with much more as I need to go down to bunnings to get a few things :slight_smile:
I'll happily organise it at some point for you.
```

---
## \#118 Posted by: pshaw Posted at: 2017-11-01T01:13:45.080Z Reads: 145

```
[quote="chaka, post:115, topic:36381, full:true"]
No offence, but I need to see it to believe it. Never seen someone ride a trampa over 25mph with any amount of confidence. Are you running stock geometry?
[/quote]

I hit ~30mph all the time on my street carver. It's seen 35mph maybe 2 dozen times. Nothing ever seemed super sketchy about it. And my trucks are really loose too.
```

---
## \#119 Posted by: chaka Posted at: 2017-11-01T03:38:28.313Z Reads: 150

```
Again, I need to see it to believe it. To date all I have seen is super sketchy handling on those trampa builds. . Don't get me wrong, they seem great up to 20 mph but it is the last thing I would want to be riding at 35 mph. Definitely wouldn't recommend it for a speed build.
```

---
## \#120 Posted by: pshaw Posted at: 2017-11-02T02:22:52.460Z Reads: 160

```
[quote="chaka, post:119, topic:36381, full:true"]
Again, I need to see it to believe it. To date all I have seen is super sketchy handling on those trampa builds. . Don't get me wrong, they seem great up to 20 mph but it is the last thing I would want to be riding at 35 mph. Definitely wouldn't recommend it for a speed build.
[/quote]

Haha if I'm comfortable on this at 30+ i guess I should really try a dedicated speed board then huh :stuck_out_tongue:
```

---
## \#121 Posted by: Schulerbible Posted at: 2017-11-03T06:10:27.883Z Reads: 167

```
What's the setup you are running to reach such a high top speed?
```

---
## \#122 Posted by: BigBoyToys Posted at: 2017-11-03T09:12:21.203Z Reads: 170

```
My experience so far with Trampa builds is similar. They arent stable above 25mph. My buddy has a 16ply 4wd and hits 30mph+ regularly but definitely looks wiggly at those speeds.
```

---
## \#123 Posted by: Deckoz Posted at: 2017-11-05T22:24:43.723Z Reads: 169

```
Pshaw hits those speeds often...and is just fine...me on the other hand. I never wanna ride a trampa again lol

From yesterday going 30+ on the trampa...the wobbs are real on tramps for featherweight riders lol...
<img src="/uploads/db1493/original/3X/e/d/ed0805fdc9b263686051bb3953d68180173fdb69.jpeg" width="295" height="500">

Where as in the vanguard I hit those speeds no problem... <3 flex hate stiff decks.
```

---
## \#124 Posted by: pshaw Posted at: 2017-11-05T23:10:33.561Z Reads: 167

```
^ :frowning:
```

---
## \#125 Posted by: racidon Posted at: 2017-11-08T00:45:23.598Z Reads: 163

```
Pretty much this: http://www.electric-skateboard.builders/t/e-toxx-directdrive-vs-trampa-vesc6-vs-leopard-8072-170kv-vs-nowind/30822

Except I'm using a belt setup rather than direct drive
```

---
## \#126 Posted by: Dameshh Posted at: 2017-11-21T09:54:17.865Z Reads: 150

```
Hi Keivan, I’m also a 17 year old looking to go fast with an electric longboard. I read through literally every reply and comment but I have a hard time understanding what the gear ratios and power supply have to be for the board to go fast and far. I also want to build a board that goes around 40-50 mph. I’m wondering what did you eventually order. What gears, motors, vescs, and power supply. And since this reply is like 20 days late, did you already get the stuff in and build it?
```

---
## \#127 Posted by: KeivanM Posted at: 2017-11-21T12:22:45.644Z Reads: 145

```
I haven't gotten the stuff yet because ill get paid mid December, I'm planning on getting the 245kv motor from hobby king, making my own lithium ion battery, 36 inch downhill deck, dual motors, dual VESCS, and dual motor mounts on caliber ii trucks

For gear ratios, I'm not really sure about that, but you can ask someone smarter on this thread than me. 

Hope this helps, its cool to see someone else try and go this fast too.
```

---
## \#128 Posted by: GrecoMan Posted at: 2017-11-21T12:40:19.060Z Reads: 139

```
have you ever ridden a normal longboard at 40mph?
```

---
## \#129 Posted by: Jreamer Posted at: 2017-11-21T12:55:46.018Z Reads: 146

```
Fast seems fun till you get the wobbles at 30.
```

---
## \#130 Posted by: Vanarian Posted at: 2017-11-21T13:47:06.818Z Reads: 151

```
Hey since you haven't gotten anything yet, lemme throw some ideas too :wink: You got a nice budget so nice parts is possible (don't know your location though so prices may vary).

- About your 2x VESCs, get a DirectFET version (vesc6, FOCBOX or Chaka's version) ; with the 6 you should not get a problem crossing 60k erpm if I recall (need to confirm this, sorry if this was said before). It is expensive but you can always wait for me and other to report on @stewii hw6.4 offering, about how it performs compared to Trampa's ones.

- For batteries, well if you do the pack yourself you can pack a punch for not too big price. Maybe try Samsung 30Q cells because it is a 20A 3000mAh cell with decent voltage sag, despite manufacturer's rating it performs better and cooler than both 25R and VTC6 or HG2 for example. A ballpark is 150ish € is price for bare 10S4P of 30Q, with group buy you can make it down to 120ish. 10s4p is ~450wh, that's very conservative 20-25km street use.

- About trucks, I recall somebody here praising Ronin trucks. Miles better than Caliber trucks was what he said.

- I'm sold on direct drives and hub motors. Or Jenso style drive. Look at @BigBoyToys 4wd setup, the beast is fast!

- @psychotiller makes sick enclosures for electronics.

It's not your first e-board so I'll keep it short to these suggestions, but 1000usd should allow for a nice setup damn !
```

---
## \#131 Posted by: Exiledd_Top Posted at: 2017-11-21T14:33:31.063Z Reads: 146

```
This "going fast " is like buying sports car we want the fastest out there but soon to realize this is to much and just cruise and never go fast. You have yet to actually go 30 or even 40 .Also it's going to be hard to hit 40and up with nonhub and direct drives
```

---
## \#132 Posted by: BigBoyToys Posted at: 2017-11-21T17:21:33.531Z Reads: 147

```
[quote="Exiledd_Top, post:131, topic:36381"]
This "going fast " is like buying sports car we want the fastest out there but soon to realize this is to much and just cruise and never go fast.
[/quote]

Id say this is generally true but my 4wd Carvon breaks 40mph, acceletates well and is the most efficient board I have. Cant say anything negative about it besides it was expensive to build lol.
```

---
## \#133 Posted by: Acido Posted at: 2017-11-21T17:58:00.607Z Reads: 143

```
My advice for you is to save up some money for the doctors before you go out and ride this thing
```

---
## \#134 Posted by: Dameshh Posted at: 2017-11-21T19:12:41.858Z Reads: 141

```
Surprisingly yes. Me and my friends are a bit crazy. They would drag me behind their car going 50 mph down a smooth road on a regular non-electric longboard.
```

---
## \#135 Posted by: GrecoMan Posted at: 2017-11-21T19:13:51.333Z Reads: 141

```
sounds like you need new friends :joy:
```

---
## \#136 Posted by: Dameshh Posted at: 2017-11-21T19:15:16.169Z Reads: 141

```
Lmao. But I kind of get used to the speed wobbles and learned how to control them
```

---
## \#137 Posted by: Exiledd_Top Posted at: 2017-11-21T19:17:39.018Z Reads: 146

```
When the vesc blows up and your screwed and get badly injured don't come blaming any brand here in esk8 just saying that now.
```

---
## \#138 Posted by: Dameshh Posted at: 2017-11-21T19:19:11.101Z Reads: 148

```
Nah I won’t do that
```

---
## \#139 Posted by: michichopf Posted at: 2017-11-21T20:26:08.108Z Reads: 163

```
Hard to believe but I give you the benefit of the doubt.¨
Anyway, you should feel super comfotable at 50mp/h. Comfortable in a sense that you can take sweepers both sides, hold your side in turns, being able to speedcheck, drift and slide coleman and toeside. EVEN then it is still super risky to go 50 with a 30lbs piece of wood. 

Further down you make a remark that is truely scary for me:"Lmao. But I kind of **get used to the speed wobbles** and learned how to control them" 

If you are getting wobbles so often that you are trying to controle them... I am afraid for your safety honestly. Wobbles aren't an oh shit moment or a difficulty you have to overcome. It is a deadly, silen't killer. No joke. Most deaths in longboarding are because of wobbles. Itmeans a rider is either sloppy or going over his own limits and it kills them. 14 poeple in the USA alone last year to be exact. If you fall even at 60mp/h but it is controlled and on your terms it is mostly harmless. BUT if you fall out of a wobble, with all that momentum, rotations, and katapult like propulsion shit gets nasty or like I said above deadly.

I seriously urge you to go out there. ( with porper safety gear) spend a year figuring out speeds of 30-40. Controling it, living it knowing how big your apex is at that speed. How lonnng a full stop takes on what kinnd of wheel (duro, contact patch, size). Not trying to be a dick or anything, if at all take it as an invitation be get your skill on par with your ambitions.

I am planing a crazy fast build as well (4wd even). I wanted that for ever. But I said to myslef. It toock you so many hours, of painful falls, endles walking up the same parts of a road, just to figure out how fast I can take corners. Basically it toock me 1 whole year to feel at home at 50 (not my first year skating, my first year understanding and learning what 50 means). This was a few years ago and still today as soon as my eyes start to hurt, i feel the pressure in my ears I know I am close to 55/60 and shit gets real. Muscle memory kicks in, you have to plan your ride ahead suddenly, try to read the road etc. etc.

The beauty of downhill or high speed skating in generall is to have that burst of adrenalin, that moment when your mind shuts off, everything goes quiet. You are no longer thinking, just instintively gliding over this beautiful planet. But going home, being able to tell the tale and do it all over again that's what it is about.

Some motivationn for the nnnescessary skillset fur such an endevour:

[many close calls thanks to skill](https://www.youtube.com/watch?v=9jNFRviMkxo&t=59s)

All the luck inn your project man, but stay safe !!
```

---
## \#140 Posted by: KeivanM Posted at: 2017-11-22T16:46:14.312Z Reads: 146

```
Okay I’ll keep that in mind, thanks for the advice!
```

---
## \#141 Posted by: notepad Posted at: 2017-11-22T18:04:18.711Z Reads: 144

```
Just going to leave this here. take from it what you will.

http://www.electric-skateboard.builders/t/motor-choice-for-fast-longboard/36722/36?u=notepad
```

---
## \#142 Posted by: KeivanM Posted at: 2017-11-22T22:00:37.285Z Reads: 145

```
okay thanks!
```

---
## \#143 Posted by: KeivanM Posted at: 2017-11-22T22:01:20.268Z Reads: 144

```
Does anyone know if dual SK3 192 KV motors will fit on caliber ii trucks with Diyelectricskateboard motor clamps without any problems?
```

---
## \#144 Posted by: notepad Posted at: 2017-11-22T22:21:38.922Z Reads: 141

```
nope, they are too large,  If they fit I would havent had to get new longer trucks to go dual
```

---
## \#145 Posted by: Dameshh Posted at: 2017-11-25T01:36:31.258Z Reads: 149

```
what if i use dual 270kv alien motor on a 18 to 36 gear ratio with 10s lipo and a set of focboxes. would i blow the focboxes? how fast do you think i would go?
```

---
## \#146 Posted by: BigBoyToys Posted at: 2017-11-25T09:04:28.453Z Reads: 157

```
I think the FOC box can take it but its beyond the manufactures recommend KV range if you are gonna push 12S voltage so its at your own risk.
```

---
## \#147 Posted by: LEE Posted at: 2018-07-30T11:28:44.400Z Reads: 134

```
I am planning to make a 45 mph board with Samsung 40T 10s5p or 12s4p.
6374Motor 190KV 2WD and 5065Motor 220KV 4 WD.
Which is more efficient?
The deck is scheduled for Landyachtz EVO, belt drive 2WD, gear drive 4WD.
4WD needs money. It is good if it can achieve the target speed without problem even with 2wd.
36V150A, 43V120A, I think the power is sufficient.
```

---
## \#148 Posted by: Blitz Posted at: 2018-07-30T11:40:29.494Z Reads: 131

```
Dual 6374 12s4p , Is a popular choice here for speed board's,
buying 2 more Esc's and 2 more pulley kit's cost's more, so... 2wd is more effeienct on your wallet thats all i can say :D 

Maybe 13s4p if you wanna crank it to 45mph, @Deckoz would know more about this.
```

---
## \#149 Posted by: LEE Posted at: 2018-07-30T12:01:32.067Z Reads: 127

```
Is it difficult at 45 mph with a torque board belt drive with a gear ratio of 36:15?
It seems to be theoretically achievable if the gear ratio is 2:1.
It seems that @Deckoz changed to a gear drive.
```

---
## \#150 Posted by: E1Allen Posted at: 2018-07-30T12:46:37.122Z Reads: 125

```
Mine goes 38mph at that gear ration on 107mm with 12s6p
```

---
## \#151 Posted by: LEE Posted at: 2018-07-30T13:23:12.399Z Reads: 126

```
For example, if you can change to 32:16, is it possible to achieve 45 mph?
```

---
## \#152 Posted by: Battosaii Posted at: 2018-07-30T13:48:15.261Z Reads: 127

```
I've gotten 44mph top speed at full battery on a 12s4p 16t 36t set up.
```

---
## \#153 Posted by: sk8l8r Posted at: 2018-07-30T13:59:04.194Z Reads: 124

```
going to be interesting to see how that compares to my 13s5p 16t 36t
```

---
## \#154 Posted by: E1Allen Posted at: 2018-07-30T14:01:31.958Z Reads: 126

```
I guess I didn't mention I cutoff my charge voltage to 4.15, but a full battery still only got me 38 on 15/36
```

---
## \#155 Posted by: tonycamaro427 Posted at: 2018-07-30T22:49:19.066Z Reads: 117

```
there is a board from "next board" that used 12 lipo and made it to the 60mph range look him up it shows specs of the board and video
```

---
## \#156 Posted by: tonycamaro427 Posted at: 2018-07-30T22:53:16.653Z Reads: 116

```
 use motorcycle gear for safety .  I have gone 50mph on a downhill board with no motor and have been towed by a car  to that speed too.  its a lot faster then you think,.  I had to use stabilizers on the trucks
```

---
## \#157 Posted by: tonycamaro427 Posted at: 2018-07-30T22:59:16.959Z Reads: 115

```
BTW down hill boards still have the record 81mph on speed over electric at by almost 20mph    not for long
```

---
## \#159 Posted by: Cobber Posted at: 2018-09-07T16:25:50.247Z Reads: 105

```
[quote="tonycamaro427, post:156, topic:36381"]
I have gone 50mph on a downhill board... I had to use stabilizers on the trucks
[/quote]

stabilizers :smile: :rofl:
they have quite the reputation here, tell us more?

[quote="tonycamaro427, post:157, topic:36381, full:true"]
BTW down hill boards still have the record 81mph on speed over electric at by almost 20mph not for long
[/quote]

No & No dude, guys are going faster than that on both.
```

---
## \#160 Posted by: Kug3lis Posted at: 2018-09-07T16:47:10.789Z Reads: 106

```
[quote="Cobber, post:159, topic:36381"]
No &amp; No dude, guys are going faster than that on both.
[/quote]

I think I saw a video on youtube with a dude on longboard going downhill through the tunnel at 91mph like for sure I even remember that he used evo deck then I was doing research about evo decks :D
```

---
## \#161 Posted by: Wraith Posted at: 2018-09-07T16:53:39.874Z Reads: 108

```
Evo decks are just soo good for those speeds. Makes me want one now too especially with more builders using the deck :smile:
```

---
## \#162 Posted by: skatardude10 Posted at: 2018-09-07T17:57:34.859Z Reads: 107

```
A couple of us use stabilizers on our trucks...

![20180704_231923|675x500](upload://wiUHYeHJ8PKMnUEYxxG7DLEndcg.jpg)

Mine works great, since getting it setup right I haven't had a single wobble or hint of instability... Having the extra layer of stability physically bolted to your board is really indispensable for me when riding at high speeds next to traffic. Sure, learn to be stable on your board, learn to be comfortable, learn to deal  with wobbles without  it first, setup your bushings correctly, wedge properly, all these things are great and 100% necessary. After that's all said and done though, the best thing imo to top it all off is having that reassurance (almost a guarantee) that your board is even more so *far less likely* to do anything crazy under your feet at the worst possible moment.
```

---
## \#163 Posted by: b264 Posted at: 2018-09-07T18:05:54.753Z Reads: 108

```
[quote="skatardude10, post:162, topic:36381"]
A couple of us use stabilizers on our trucks
[/quote]

You should make a new thread about truck stabilizers :slight_smile:
```

---
## \#164 Posted by: skatardude10 Posted at: 2018-09-07T18:07:13.032Z Reads: 105

```
There are threads out there... 

I'd advocate everyone at least try it, but not everyone has the means to so I'm just a very very silent advocate for it outside the couple threads I've posted about it in.
```

---
## \#165 Posted by: Cobber Posted at: 2018-09-07T18:09:29.412Z Reads: 104

```
on his dh board dude... :thinking:
```

---
## \#166 Posted by: Deckoz Posted at: 2018-09-07T18:09:44.822Z Reads: 105

```
No offense. But all I see is

To much riser, washers instead of cups and likely too soft of bushings.. but hey I'm not here to judge
```

---
## \#167 Posted by: skatardude10 Posted at: 2018-09-07T18:16:43.236Z Reads: 106

```
No offense taken ☺️ the tall risers negate the drop on the deck itself, putting it on par (maybe a tad taller) than just top mounting a flat deck. Tried precision cups- too much rebound for the rear and I use the keys to keep the hanger aligned center with the kingpin. Those were the hardest WFB chubbies I could get.
```

---
## \#168 Posted by: skatardude10 Posted at: 2018-09-07T18:31:13.031Z Reads: 102

```
My DH boards became my Eskates and Eskate is now my downhill.... Dunno if this is even relevant. Honestly I just hopped into the discussion reading your comment about stabilizers without reading into any context 😀 forgive me if I am off base or taking this the wrong way.
```

---
## \#169 Posted by: Cobber Posted at: 2018-09-07T18:38:47.365Z Reads: 106

```
i'll let you catch up dude ;)

https://www.electric-skateboard.builders/t/stabilised-skateboard-truck-anti-speed-wobble-tech-advice-from-a-moron/24902
```

---
## \#170 Posted by: b264 Posted at: 2018-09-07T20:04:59.010Z Reads: 99

```
LoL @Cobber  I saw that thread and am intentionally ignoring it
```

---
## \#171 Posted by: skatardude10 Posted at: 2018-09-08T01:06:03.430Z Reads: 94

```
Omfg okay yes thanks, I remember reading that. Ah, what. Springs are stabilizers? Rhetorical question... Thanks for filling me in and reminding me 😋😎
```

---
## \#172 Posted by: tonycamaro427 Posted at: 2018-09-15T15:45:42.261Z Reads: 85

```
![thZIU0LYTJ|270x202](upload://ia1dhey0Dyw1fbVBR7AmIhrDTnN.jpg)![Electric_Skateboard_Gnarboards_Trail_Rider_07|316x235](upload://jzEnszEMoy3I4v8VGjV3WZk7Ei6.gif)![20180724_193722|375x500](upload://8wPwRJthca19i0obxYzY8Qq1Dnh.jpg)![20180726_175150|375x500](upload://wfyjffvx0beyE2n4vwLb5gWqkaO.jpg)
```

---
## \#173 Posted by: tonycamaro427 Posted at: 2018-09-15T15:51:27.654Z Reads: 82

```
![b98ac534835b15cf93adf67d142f4972|600x391](upload://MGzYMMrn0JkPaxvLneXWAzmRC1.jpg)
```

---
## \#174 Posted by: tonycamaro427 Posted at: 2018-09-15T15:54:54.649Z Reads: 82

```
if these were Massive hub motors, made properly in AWD all wheel drive should solve the power issue![Wholesale-High-Quality-Ecorider-Off-Road-Four-Wheels-Electric-Skateboard-with-Bluetooth_2|500x500](upload://lzyXVToHfS5JOj5O2JUApufFIzL.jpg)
```

---
## \#175 Posted by: Cobber Posted at: 2018-09-15T16:01:35.383Z Reads: 80

```
At this point I see so much wrong, springs, elastic bands...
All this has been discussed before please do some research.

& with that I'm out guys, please don't encourage others to try...
```

---
## \#176 Posted by: Sebike Posted at: 2018-09-15T16:11:10.562Z Reads: 80

```
OMG they're back...!!

https://youtu.be/Zy8yZ2hu7fo?t=1m26s
```

---
## \#177 Posted by: tonycamaro427 Posted at: 2018-09-15T16:28:29.283Z Reads: 78

```
The top two will be the direction I predict it will go.  These already work and have been proven on motorcycles & bicycles. The stable shock that is.
```

---
## \#178 Posted by: tonycamaro427 Posted at: 2018-09-15T16:32:06.691Z Reads: 77

```
Gnarboard which is a $6000 USD is the one that is already in production,  it does work and is being sold currently.   Most will never be able to buy the board he makes them in very limited production.
```

---
## \#179 Posted by: tonycamaro427 Posted at: 2018-09-15T16:50:19.336Z Reads: 78

```
What is needed is independent suspension, yet still be able to lean the board to steer.
```

---
## \#180 Posted by: tonycamaro427 Posted at: 2018-09-17T19:18:33.149Z Reads: 62

```
![gila-board|667x500](upload://hP8zm81JI0xqU7mVJ6Z7IduCN92.jpg)
```

---
