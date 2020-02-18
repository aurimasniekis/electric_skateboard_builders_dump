# 4 motor build max torque/top speed/range

### Replies: 431 Views: 10130

## \#1 Posted by: Sirshaunsta Posted at: 2017-11-30T13:49:37.283Z Reads: 515

```
Hey guys, planning to build a 4 motor board for added torque without sacrificing speed up steep hills, I have ordered 4 - sk3 190kv motors, 12 - 5s 20c 5000mah lipos to be assembled into a 10s 30 000mah with 4 - focbox speed controllers with 3 - y harness adapters to sync them.  A 2.4 wireless controller, led voltage display panel. 60 v capable on off switch.  218 mm v2 trucks with 63mm motor mounts. 15mm bands at 16/36 gearing. 90mm wheels also looking at 100mm. Looking for any input on my build to help this come to life. In total I've spent roughly 2500 CANADIAN so far.
```

---
## \#2 Posted by: PredatorBoards Posted at: 2017-11-30T14:49:44.322Z Reads: 484

```
I appreciate the ambition, but 2 6374 motors is already considered overkill. 4 motors is just straight up inefficient (double the drivetrain loss, double the coasting drag) and extremely heavy. We are talking about adding an extra 4lbs of weight here. When you begin carrying your board (for transport, police officer telling you to get off, no ride zones, going up stairs, etc.) you're going to wish you could shave off a single pound. I own a dual 6374 board, and that shit is already heavy as is.
```

---
## \#3 Posted by: Acido Posted at: 2017-11-30T14:55:59.570Z Reads: 457

```
BUT then it can have a double purpose, not just a skate, but also a dumbbell
```

---
## \#4 Posted by: Quezacotl Posted at: 2017-11-30T14:58:12.608Z Reads: 459

```
I presume you are going to switch the power with only a switch, since you mentioned the 60V capable switch. I strongly recommend of using an anti-spark circuit with the switch. Here is one if you want to make it yourself:
https://endless-sphere.com/forums/viewtopic.php?f=3&t=40142&start=100

But yea, your board is going to get heavy.  You could even make two overpowered boards from those supplies :D
```

---
## \#5 Posted by: PredatorBoards Posted at: 2017-11-30T16:25:54.689Z Reads: 449

```
https://www.amazon.com/gp/aw/d/B01F76VJT2/ref=mp_s_a_1_3?ie=UTF8&qid=1512059618&sr=8-3&pi=AC_SX236_SY340_QL65&keywords=waterproof+circuit+breaker&dpPl=1&dpID=419q%2BD8u6%2BL&ref=plSrch

Cheaper and better. Reset lever to turn on. Step on the button to open the circuit. I put one on top of my board(above front trucks), so when I need to shut off the board, I literally just stomp on the switch.

<img src="/uploads/db1493/original/3X/1/9/19ea8fb68c4eb47c9e8d69b33cb51535e1f1158c.JPG" width="375" height="500"><img src="/uploads/db1493/original/3X/6/b/6bd3e38075b063706a757648c0f064f8b236bddb.JPG" width="375" height="500">
```

---
## \#6 Posted by: krloz Posted at: 2017-11-30T16:37:50.621Z Reads: 432

```
Where the f*** are you going to fit 12x 5s 5a batteries???
Omg I want to see this board so hard
I'm sure you can put together a pretty overpowered jeep with that list
```

---
## \#7 Posted by: Quezacotl Posted at: 2017-11-30T21:21:01.921Z Reads: 420

```
Interesting. Bit bulky, but good for kill switch. For how long have you been using this?
```

---
## \#8 Posted by: evoheyax Posted at: 2017-11-30T22:17:27.705Z Reads: 416

```
[quote="PredatorBoards, post:2, topic:39765"]
4 motors is just straight up inefficient
[/quote]

Been debated, and yet, still no definitive answer. Using more mores means smaller magnetic fields in each motor. Depending on how much torque your demanding, you could be over saturating your stators by generating too large of a magnetic field for the motor, which is the biggest inefficiency. If 4 motors means you don't hit this point, then you could achieve better efficiency with 4 motors rather then 2.

Everyone thinks 4wd is super inefficient, yet hummie did 5 miles on my board, and only used about 1/4th of my 8ah battery. Defiantly could have done 20 miles, which is normal for a battery this size.
```

---
## \#9 Posted by: BigBoyToys Posted at: 2017-11-30T22:38:39.231Z Reads: 399

```
@evoheyax  Yeah, thats about 17whr/mile which is solid efficiency imo. My 4wd V3 board did 13.5 whr/mile  on a leisurely 10mile beach cruise. Ive yet to see any 4wd belt boards efficiency numbers though. @Pychotiller Just finished one, maybe we can throw a BT module on it and get some numbers for comparison?

I have a 4wd spur gear set up on pneumatics and have been doing some efficiency testing as well. Lowest Ive gotten it so far is down to 35whr/mile over a charge cycle and thats with similar riding style to what yeilded 13.5 on the carvon DD's.
```

---
## \#10 Posted by: evoheyax Posted at: 2017-11-30T22:48:50.734Z Reads: 389

```
The problem is theres so many factors in range though. For me, I get 40 Wh per mile on the same board that hummie gets 17 Wh per mile on.

Until someone finally makes the e-skate dyno, and set up all boards to the same battery, same esc's, and best settings for the each motor, then we won't know what motors are really the most efficient. I'd love to know though...

In my case, I run them at higher speeds for longer time (so more drag) and probably as a result, I heat them up a bit more. Not too high, but I'm probably losing a few miles just due to the extra heat I generate by riding at higher speeds. Then many more from drag, and even more from my weight. It's all kinda a guessing game at this point.
```

---
## \#11 Posted by: BigBoyToys Posted at: 2017-11-30T23:31:11.444Z Reads: 368

```
For exact comparisons between riders sure, but for basic comparison purposes it seems easy enough. Like when comparing two of my boards for example. Same rider, same riding style, same distance and location, its really pretty obvious which board is more efficient when one averages half the consumption of the other over the same distance.
```

---
## \#12 Posted by: PredatorBoards Posted at: 2017-12-01T03:05:37.736Z Reads: 346

```
Works for as long as you don't drop the entire board on the switch. They're pretty durable as is.
```

---
## \#13 Posted by: Sirshaunsta Posted at: 2017-12-01T07:43:04.278Z Reads: 333

```
So this switch is an on off breaker?
```

---
## \#14 Posted by: Sirshaunsta Posted at: 2017-12-01T07:44:41.294Z Reads: 323

```
How did you assemble the vescs? Using 3 y harness 1 to both rear another to fronts and third to connect the 4 into one receiver?
```

---
## \#15 Posted by: Sirshaunsta Posted at: 2017-12-01T07:48:13.970Z Reads: 320

```
I literally won't have to carry this where I live. I'm in a small town of ontario canada
```

---
## \#16 Posted by: Sirshaunsta Posted at: 2017-12-01T08:42:08.043Z Reads: 326

```
As far as efficiency, my motors will have less resistance each requiring less power to perform with loads. And at 1200wh 10s 37v battery I don't think I'm worried even if I dropped to 8 batteries I'd have 800wh 10s 37v
```

---
## \#17 Posted by: psychotiller Posted at: 2017-12-01T09:00:42.070Z Reads: 333

```
[quote="BigBoyToys, post:9, topic:39765"]
@Pychotiller Just finished one, maybe we can throw a BT module on it and get some numbers for comparison?
[/quote]



We have one I can put in there. Matt and I will get it set up.
```

---
## \#18 Posted by: scepterr Posted at: 2017-12-01T09:04:13.069Z Reads: 326

```
I would love to see a comparison between 4wd and 2wd with the unused motors taken off in fwd and rwd configurations
```

---
## \#19 Posted by: Sirshaunsta Posted at: 2017-12-01T12:51:00.866Z Reads: 326

```
I believe the displaced load will act like the difference of 2 and 4d in a car, more traction and lower power consumption/heat in each motor for the same tasks, allowing the ability to gear down from 2.25 to 1 (16/36) to 1.875 to 1 (16/30)  and still allow for improved torque during climbs over a standard 2wd. If the upgrade from 1 to 2 motors results in more torque doubling that should theoretically only continue to improve it allowing less energy and friction/stress in motors to accomplish the same things. Also the added motors will provide better breaking as there are 4 breaks instead of 2 for high speeds.
```

---
## \#20 Posted by: Sirshaunsta Posted at: 2017-12-01T12:55:34.193Z Reads: 325

```
So now I'm fighting with the ideas of connecting a single 10s 5000mah 20c to each motor/vesc individually to protect from overloading the wires to receiver, I realize this lowers my total available mah to 20 000 but wonder if anyone has some advice, am I safe running the 30 000 to all 4 vescs or should i divert the power individually. Will doing so effect wiring my receiver to 4 vescs in parallel?
```

---
## \#21 Posted by: BigBoyToys Posted at: 2017-12-01T16:09:10.391Z Reads: 281

```
Ive done that before but I use 4 separate receivers on one remote now.
```

---
## \#22 Posted by: Sirshaunsta Posted at: 2017-12-01T16:10:06.828Z Reads: 277

```
And how did you manage to make that work my friend? Controller and receiver names? Can multiple receiver work on same frequency and PAIR to a single frequency remote?
```

---
## \#23 Posted by: E1Allen Posted at: 2017-12-01T16:27:23.174Z Reads: 269

```
Multiple RX paired to one remote.  You could split batteries front and back.
```

---
## \#24 Posted by: Sirshaunsta Posted at: 2017-12-01T16:37:40.224Z Reads: 280

```
This is what I've been wondering, so I can connect 2 or even 4 of the same make receivers on a single frequency to one remote if I bind them all in same mode at separate times and then hook up the batteries as either a pair (2, 1 to front vescs with y cable between both wheels 1 to both on back) or a set (4, 1 going to each vesc/wheel) this is what you're saying right?
```

---
## \#25 Posted by: BigBoyToys Posted at: 2017-12-01T16:40:31.392Z Reads: 272

```
The Flysky GT2B remote can pair to multiple receivers. The receivers are available on amazon and eBay for less than $8 each. Just repeat the pairing procedure  for each additional receiver.
```

---
## \#26 Posted by: E1Allen Posted at: 2017-12-01T17:20:44.151Z Reads: 260

```
And you can y cable two ESC . Easier if they are close
```

---
## \#27 Posted by: Sirshaunsta Posted at: 2017-12-01T17:21:53.917Z Reads: 269

```
Yes I also see on hobby king the hk gt2 has spare receivers on 3 channels, would buying 4 receivers and a remote make it possible to pair the 4 to the one remote? Or 1 extra receiver and y cable them bother to 2 esc each, then both  receiver to 1 remote
```

---
## \#28 Posted by: BigBoyToys Posted at: 2017-12-01T17:34:42.486Z Reads: 260

```
Either works, I just prefer them to be all separate as a sort of failsafe.
```

---
## \#29 Posted by: Sirshaunsta Posted at: 2017-12-01T21:53:06.885Z Reads: 264

```
Quick question guys can I use the 20 tooth 15 mm motor sprocket from diyboards with 12 mm bands seeing as the wheel pulley is 12 mm I figure it won't have much effect or will I need to cut the pulley 2mm and glue it back?
```

---
## \#30 Posted by: Sirshaunsta Posted at: 2017-12-03T20:47:35.900Z Reads: 265

```
Update guys, gonna have all four using 15mm bands and pulleys with a 20/36 gear ratio of 1.8 running on 10 s(37v) . 190kv motorsx4  all capable of 7030 rpm given the battery, with weight I predict about 1 to 2000 rpm will be lost even dividing my 155 lbs to 4 motors hoping for only 1000 or less :)  this with a 97mm wheelbase puts my predicted speed with my bodyweight to be between 50 and 55km/hr hoping to never get it fast as the 70 Km max theoretic speed unweighted
```

---
## \#31 Posted by: Sirshaunsta Posted at: 2017-12-05T07:39:44.687Z Reads: 242

```
Neighbour gas a 3d printer, will be asking him to make me 32t drivewheels that match a 97mm flywheel. The increase in top speed should be about 5mph from 36t
```

---
## \#32 Posted by: E1Allen Posted at: 2017-12-05T16:20:19.060Z Reads: 240

```
I don't think you will need to cut the pulley.  Once the belts start spinning they find a sweet spot to sit.  Just make sure when you spin the wheel the direction of travel the belt lines up flush with the drive wheel pulley.
```

---
## \#33 Posted by: mmaner Posted at: 2017-12-05T17:01:36.373Z Reads: 225

```
If you guys are having trouble with belt lateral travel it's most likely because the clamp is not at a perfect right angle to the axle.  You can get that perfect angle with a [micrometer](https://www.harborfreight.com/6-in-digital-caliper-with-sae-and-metric-fractional-readings-62569.html) and a combo square ([combo square 1](https://www.harborfreight.com/6-in-heavy-duty-combination-square-69362.html) - [combo square 2](https://www.harborfreight.com/12-in-combination-square-set-62968.html)).
```

---
## \#34 Posted by: Sirshaunsta Posted at: 2017-12-05T22:50:38.741Z Reads: 220

```
Alright thanks guys, I've actually opted for the 15mm belts from diy so I'm gonna be running 20 tooth motor and 36 Wheel but after it's assembled if I find it has too much torqu I might get a custom 32 tooth 3d printer, any comments? I'm not sure if the piece will be strong enough to withstand the force applied. Please let me know what you think
```

---
## \#35 Posted by: Sirshaunsta Posted at: 2017-12-05T22:51:26.636Z Reads: 216

```
Does anyone have specs on the rpm difference with a load on a 190kv with 10s power? Theoretical top speed is 7030 rpm I assume a single motor would lower to about 5000 with 155lbs plus board being 180lbs
```

---
## \#36 Posted by: BigBoyToys Posted at: 2017-12-05T22:58:46.263Z Reads: 222

```
Try this?

http://calc.esk8.today/
```

---
## \#37 Posted by: Sirshaunsta Posted at: 2017-12-05T23:03:36.293Z Reads: 223

```
You're awesome, how do I figure the watt hours used and the number of poles for this chart though I haven't read either spec in motor description
```

---
## \#38 Posted by: Sirshaunsta Posted at: 2017-12-05T23:08:36.387Z Reads: 235

```
Holy shit, putting a 10s2p 10 000mah battery to my motor it says I'll hit a max speed of 60kpm LOADED, 70 no load. Will this be increased by having multiple motors to distribute the weight resistance?
```

---
## \#39 Posted by: BigBoyToys Posted at: 2017-12-05T23:09:10.831Z Reads: 235

```
Those are only needed for range and erpm calculations so you can just estimate. Most motors have 14 poles
```

---
## \#40 Posted by: E1Allen Posted at: 2017-12-05T23:28:54.552Z Reads: 252

```
<img src="/uploads/db1493/original/3X/8/8/88d150a46c852038c239b5f34c5ae8c1ad58f8e3.PNG" width="281" height="500"><img src="/uploads/db1493/original/3X/2/5/25fcad5bd5f59adae881749eefdb8aaf9338d44b.PNG" width="281" height="500">
```

---
## \#41 Posted by: E1Allen Posted at: 2017-12-05T23:34:22.472Z Reads: 236

```
<img src="/uploads/db1493/original/3X/e/6/e6033a3c036cb55ae3c77a1668f3bab59cab4665.jpg" width="281" height="500">
```

---
## \#42 Posted by: Sirshaunsta Posted at: 2017-12-06T02:14:25.654Z Reads: 216

```
Would you mind sharing the link for that program or posting for me what 20/36 would be? I estimate 55 or 56 Km weighted
```

---
## \#43 Posted by: E1Allen Posted at: 2017-12-06T02:48:21.175Z Reads: 231

```
<img src="/uploads/db1493/original/3X/f/b/fbb0ea72233f5c94523e28f3d658eb6066af1571.PNG" width="281" height="500">

http://calc.esk8.it/#{"batt-type-lipo":1,"batt-cells":10,"motor-kv":190,"system-efficiency":83,"motor-pulley-teeth":20,"wheel-pulley-teeth":36,"wheel-size":97}|
```

---
## \#44 Posted by: Sirshaunsta Posted at: 2017-12-06T04:50:33.885Z Reads: 201

```
Thanks so much
```

---
## \#45 Posted by: pat.speed Posted at: 2017-12-06T04:59:39.147Z Reads: 202

```
Hah and that wasn't even with a fully charged battery. Use this and imput the batteries as 13s lifepo4 that will get you pretty close to 10s full charge voltage


http://calc.esk8.it
```

---
## \#46 Posted by: Sirshaunsta Posted at: 2017-12-07T10:38:42.059Z Reads: 187

```
But I'm running 10s lipo what's the point of going off number with a different count and type of cell?
```

---
## \#47 Posted by: pat.speed Posted at: 2017-12-07T10:44:20.371Z Reads: 194

```
Because a 10s lipo is 42v when fully charged. But if you only input 10s the calculator will calculate the speed based off the cells nominal voltage which is 37v. This means you are not getting the true reading of your maximum speed because increasing voltage also increases speed. I know this may seem stupid but once you realise what I mean you will understand. The thing is though you will only be able to achieve this speed when your board is fully charged, so during the ride the top Speed will start to drop off to the nominal voltage speed and then even lower depending how low you discharge your batteries
```

---
## \#48 Posted by: pat.speed Posted at: 2017-12-07T10:45:44.562Z Reads: 185

```
The reason I used a different cell count and and completely different cell is because that combination gets as close to 42v as you can in the calculator
```

---
## \#49 Posted by: Sirshaunsta Posted at: 2017-12-07T10:48:06.076Z Reads: 195

```
Ok, actually that all does make sense, you're saying the calculator is giving an estimate of continuous usage on avg battery power to not let people down when they're at 60% and wonder if they can still hit good speed that way they know how fast they can go most of the ride? And really cause the 2 5s battery said 18.5 v each adding those only makes 37. Can you explain what I'm missing?
```

---
## \#50 Posted by: pat.speed Posted at: 2017-12-07T10:53:37.477Z Reads: 188

```
Those two batteries are 18.5volts when half charged when they are fully charged they will be at 21volts. Which gives the full 42v. Also liion nominal voltage is 3.6 per cell where as lipo is 3.7
```

---
## \#51 Posted by: Sirshaunsta Posted at: 2017-12-07T10:54:54.598Z Reads: 183

```
Oh ok, this is all news to me I knew the voltage ratings but didn't know those stats were for  half charged battery, so I'm running 42 v not 37 you say? Cool
```

---
## \#52 Posted by: pat.speed Posted at: 2017-12-07T10:56:13.708Z Reads: 174

```
Well yes when fully charged it will be 42v. It is a little confusing at the start because for some reason the manufacturers label them as there half charged voltage
```

---
## \#53 Posted by: Sirshaunsta Posted at: 2017-12-07T10:57:55.827Z Reads: 166

```
I wonder if that's because most people would treat it like a car "gas in tank so it'll still go" not realizing as they drain the battery their power becomes significantly lower
```

---
## \#54 Posted by: pat.speed Posted at: 2017-12-07T10:59:05.867Z Reads: 165

```
Hmm yes that may well be the reason
```

---
## \#55 Posted by: Sirshaunsta Posted at: 2017-12-07T10:59:12.685Z Reads: 170

```
So with a fully charged 10s2p 20c battery I can expect results from 40 to 42 v spec sheet?
```

---
## \#56 Posted by: pat.speed Posted at: 2017-12-07T11:01:44.486Z Reads: 173

```
Yes. It will just start to drop off as your ride goes on. I think that is what you meant
```

---
## \#57 Posted by: Sirshaunsta Posted at: 2017-12-07T11:02:21.811Z Reads: 188

```
I'm running 8,  5s 5000mah 20c making 2, 10s2p 10 000mah 20c's  then running one 10 s to each set of motors being 2 190kv 6364's yes 4 TOTAL MOTORS lol
```

---
## \#58 Posted by: Sirshaunsta Posted at: 2017-12-07T11:03:54.965Z Reads: 188

```
Using that app I should go over 60 to 70km/hr that's fucking nuts, 97mm wheels 20/36 (1.8) ratio
```

---
## \#59 Posted by: pat.speed Posted at: 2017-12-07T11:05:13.940Z Reads: 192

```
Yes just make sure to be wearing proper safety gear at those speeds. Are you coming from downhill?
```

---
## \#60 Posted by: Sirshaunsta Posted at: 2017-12-07T11:08:16.534Z Reads: 188

```
I live about 20 Km out of town and it's riddled with hills both incline and decline on my way, so i will be hitting ups and downs with this. And I plan for a motorcycle suit lol but may end up gearing back to 20/40 or even 16/40 if the speeds too much and then I'll never worry about a hill we know that ahaha
```

---
## \#61 Posted by: Sirshaunsta Posted at: 2017-12-07T11:09:06.735Z Reads: 157

```
Elevation from town to my house is over 100ft spread across 18km but really only 7 of it is hills
```

---
## \#62 Posted by: pat.speed Posted at: 2017-12-07T11:10:38.740Z Reads: 162

```
That's a decent climb! Good luck with you build and keep us updated it's looking good so far
```

---
## \#63 Posted by: Sirshaunsta Posted at: 2017-12-07T11:11:55.491Z Reads: 179

```
Will do, I'll be uploading some pics as soon as my parts start arriving, already got the deck I'm gonna use
```

---
## \#64 Posted by: Sirshaunsta Posted at: 2017-12-07T11:12:51.432Z Reads: 199

```
<img src="/uploads/db1493/original/3X/3/a/3a4bafffc585d2c8515a6779e768d5727cd67534.jpg" width="374" height="500">
```

---
## \#65 Posted by: Sirshaunsta Posted at: 2017-12-07T11:13:22.973Z Reads: 198

```
<img src="/uploads/db1493/original/3X/9/9/99dfed8c11a5e5e032a20b1b3e7fa7b3e0491cf6.jpg" width="374" height="500">
```

---
## \#66 Posted by: Sirshaunsta Posted at: 2017-12-08T02:36:52.284Z Reads: 201

```
Got all these in mail today :)
<img src="/uploads/db1493/original/3X/8/c/8c20c7432dc87959ddd4a7ba08040ec801fbebbe.jpg" width="375" height="500"><img src="/uploads/db1493/original/3X/5/8/58443b97cf685994e6f8efd60d5cb13cd8ac5a47.jpg" width="374" height="500"><img src="/uploads/db1493/original/3X/5/2/521e5c7cb150907412667d1ba73f10c4ac9013d5.jpg" width="374" height="500">
```

---
## \#67 Posted by: E1Allen Posted at: 2017-12-10T03:09:47.984Z Reads: 189

```
And the build begins. Gonna be plenty of torque.
```

---
## \#68 Posted by: faithfulpuppy Posted at: 2017-12-10T03:15:50.690Z Reads: 188

```
oh boy it's goin down
```

---
## \#69 Posted by: Sirshaunsta Posted at: 2017-12-18T01:39:31.827Z Reads: 189

```
<img src="/uploads/db1493/original/3X/8/4/8424d4e26e4bbca008fa04e8c481931313e297a7.jpg" width="374" height="500">
```

---
## \#70 Posted by: Sirshaunsta Posted at: 2017-12-18T01:40:02.361Z Reads: 189

```
<img src="/uploads/db1493/original/3X/c/a/cad76813351b0f215660d1d0fc6a66a336d5eec7.jpg" width="374" height="500"> 97m
```

---
## \#71 Posted by: Sirshaunsta Posted at: 2017-12-19T21:06:58.824Z Reads: 188

```
Just an update on parts I've received for the build, still waiting to order motor mounts and wide axle 218mm from diy. Also wondering if anyone can help with a question, do I need to reconnect my wires with xt90 plugs in place of the current xt60 that are on the batteries in order to wire them in series and parallel? Or would I be better off making a 60 to 90 adaptor for each battery to keep charging simple? I don't want to overload the wires and not sure if my 10s 6p 30 000mah will do that? Though I plan to split it into 2 half being 10s 3p 15000mah to each end, thus two batteries each powering 2 motors per end. Also I've found a man nearby that has a 3d printer i plan to ask to make me custom sprockets 20 tooth motor and 30 tooth wheel. Lemme know what you guys think of this Canadian fuckery;) <img src="/uploads/db1493/original/3X/0/a/0a08f2b6d986cc0c847903f9ae3a3fc64b1faa21.jpg" width="374" height="500">
```

---
## \#72 Posted by: Sirshaunsta Posted at: 2017-12-19T21:08:12.617Z Reads: 190

```
<img src="/uploads/db1493/original/3X/b/c/bcad9cc2447506fa8d86aa7fc543824be02363d2.jpg" width="666" height="500">
```

---
## \#73 Posted by: yelnats8j Posted at: 2017-12-19T22:39:35.088Z Reads: 188

```
where are all those batteries gonna go on that deck and why would anyone do this. 
looks its gonna be a beast good luck.
```

---
## \#74 Posted by: pat.speed Posted at: 2017-12-19T22:59:32.734Z Reads: 178

```
He's gonna need some big assed risers
```

---
## \#75 Posted by: Jreamer Posted at: 2017-12-19T23:01:02.971Z Reads: 179

```
Just stick them in the middle like mountain boards.
```

---
## \#76 Posted by: pat.speed Posted at: 2017-12-19T23:03:54.099Z Reads: 181

```
Yep, just not as stealthy
```

---
## \#77 Posted by: yelnats8j Posted at: 2017-12-19T23:11:38.753Z Reads: 185

```
Two of these stacked might just barely be enough.:joy:

https://www.amazon.com/Longboard-Riser-Truck-Risers-Black/dp/B00B2Q4PK2

now just need some long ass hardware.
```

---
## \#78 Posted by: pat.speed Posted at: 2017-12-19T23:12:34.610Z Reads: 181

```
Haha he might as well get two bricks and use those
```

---
## \#79 Posted by: louwii Posted at: 2017-12-20T01:37:14.341Z Reads: 176

```
I would replace the connectors with XT90, giving the power you'll pull from the batteries, I think it's safer (bigger connectors = less resistance = less heat). That's if you're good at soldering though.

And as the others said, good luck with the batteries ! I can't believe you're gonna put all of them on one board.
```

---
## \#80 Posted by: Battosaii Posted at: 2017-12-20T02:20:45.785Z Reads: 183

```
[quote="pat.speed, post:45, topic:39765"]
http://calc.esk8.it
[/quote]

hmmm if thats true My weighted top speed should be 49mph with my new set up but its currently untested. I have found the esk8 calculator to be quite accurate with my previous 10s set up it would have not been correct if i put like it had a full charge because when you are accelerating hard your voltage sags.
```

---
## \#81 Posted by: Sirshaunsta Posted at: 2017-12-20T02:24:31.870Z Reads: 171

```
That was the plan, here I'll show what it will look like when I put it together give 5 mins
```

---
## \#82 Posted by: pat.speed Posted at: 2017-12-20T02:27:04.735Z Reads: 168

```
Yes I guess it would sag slightly but it depends what batteries you are using. I have found that it was perfectly accurate for me when setting it to full charge voltage and 85% efficiency
```

---
## \#83 Posted by: Sirshaunsta Posted at: 2017-12-20T02:45:46.229Z Reads: 178

```
Now keep in mind I'm ordering 218mm whereas these a 160 or 170mm. Also plan to re-drill the truck holes 1 cm closer to the end of the board on each side to make room for motors facing inside during turns.  12 batteries in middle between feet not underneath.
```

---
## \#84 Posted by: Sirshaunsta Posted at: 2017-12-20T02:48:04.863Z Reads: 190

```
<img src="/uploads/db1493/original/3X/8/4/84a7a9c9df1f8d55c29e33d0ed455dd146905e37.jpg" width="666" height="500"><img src="/uploads/db1493/original/3X/f/6/f67e15c9f5524513dbac2874fa344835aad2f183.jpg" width="666" height="500"><img src="/uploads/db1493/original/3X/e/6/e67966348a49ceffff0884811ebf88694eeec7a6.jpg" width="666" height="500"><img src="/uploads/db1493/original/3X/e/1/e1ee3c6ad39943e4d0b793e9db1fe484f432458c.jpg" width="666" height="500"><img src="/uploads/db1493/original/3X/6/2/629a1ca3fbcf4a1ca3f18fc93cb55dc8d583a94e.jpg" width="374" height="500">
```

---
## \#85 Posted by: Sirshaunsta Posted at: 2017-12-20T02:50:17.965Z Reads: 182

```
<img src="/uploads/db1493/original/3X/6/f/6f71a005488313449cd627657e9fdc63c18bf750.jpg" width="666" height="500">
That's a full size bic lighter of clearance, just for the dummy who kept going on about risers. Read the build and you'd know I'm on 97mm wheels...
```

---
## \#86 Posted by: GrecoMan Posted at: 2017-12-20T02:52:49.533Z Reads: 177

```
he’s right about the risers... your gonna need em
```

---
## \#87 Posted by: Sirshaunsta Posted at: 2017-12-20T02:53:14.725Z Reads: 176

```
You really think so?
```

---
## \#88 Posted by: yelnats8j Posted at: 2017-12-20T02:54:01.294Z Reads: 175

```
For sure if u want to be able to go over any bumps.
```

---
## \#89 Posted by: GrecoMan Posted at: 2017-12-20T02:54:13.600Z Reads: 175

```
yea. those batteries with an enclosure will yield a very small amount of clearance. i’d say probably about 1/2” and avoid speed bumps and curbs.
```

---
## \#90 Posted by: Sirshaunsta Posted at: 2017-12-20T02:54:43.000Z Reads: 169

```
No guys, the batteries are going on top of the board not under
```

---
## \#91 Posted by: yelnats8j Posted at: 2017-12-20T02:55:29.889Z Reads: 162

```
that's a ton of batteries to put on top of a board.
```

---
## \#92 Posted by: Sirshaunsta Posted at: 2017-12-20T02:57:45.584Z Reads: 162

```
Yes I know, it will look hulky and be heavy, roughly 25lbs completed.  But I live in a small town, so police won't be much of a problem neither will no ride zones... My town has a bylaw stating longboard MUST be ridden on the street not sidewalk and that's normal  leg powered boards
```

---
## \#93 Posted by: Sirshaunsta Posted at: 2017-12-20T02:59:32.793Z Reads: 165

```
But like I said I don't see the use for risers though a 1/8 Or 1/4 might be nice just for cushion and to allow me to position the motors higher from the ground
```

---
## \#94 Posted by: yelnats8j Posted at: 2017-12-20T02:59:50.098Z Reads: 169

```
I don't know if anyone has done this but what if you mounted some on top and some on the bottom could make it look a little cleaner.
```

---
## \#95 Posted by: GrecoMan Posted at: 2017-12-20T03:01:58.074Z Reads: 172

```
oooohhh i’m tracking now, i personally think it’ll look weird with that huge mound of batteries ontop but it’s your build not mine
```

---
## \#96 Posted by: Sirshaunsta Posted at: 2017-12-20T03:05:54.604Z Reads: 166

```
I thought about that, but the batteries are 40mm thick and i have about 60mm after i step on ,  so with only 1 layer of batteries underneath I'd be left with 20mm of clearance and that's no good for me
```

---
## \#97 Posted by: yelnats8j Posted at: 2017-12-20T03:08:14.731Z Reads: 165

```
Yeah, that's not that much clearance.  what are you looking at right now for an enclosure to hold it all?
```

---
## \#98 Posted by: Sirshaunsta Posted at: 2017-12-20T03:09:33.018Z Reads: 166

```
Yes I agree it won't look as sleek as many other boards, but this is of course my first build,  and I'm using lipos, later on I may look at making my own 10s cell from li ion batteries but for now this was easier. Plus the whole point of putting them in the center is for equal weight distribution which goes with why I picked the drop deck(lower center of gravity while riding) I wanted to build this board so it would be very stable at high speeds and when accelerating
```

---
## \#99 Posted by: Sirshaunsta Posted at: 2017-12-20T03:11:50.664Z Reads: 165

```
To be quite honest I haven't thought much about an enclosure yet, as I'm still waiting for enertion to send my my 4 focbox, and then diy for the 218mm trucks and motor mount setups( also 4) so I've just been piecing things together as I get the parts also still waiting for another kill switch another volt display and my 6 plug charging boards
```

---
## \#100 Posted by: yelnats8j Posted at: 2017-12-20T03:15:34.790Z Reads: 161

```
You should start looking for an enclosure because finding one that can hold all those batteries is gonna take some time. what are the dimensions on all those batteries stacked like that.
```

---
## \#101 Posted by: Sirshaunsta Posted at: 2017-12-20T03:25:40.967Z Reads: 157

```
115×205×165 if I insulate them it may add 5 to 15mm on each dimension
```

---
## \#102 Posted by: Sirshaunsta Posted at: 2017-12-20T03:32:36.889Z Reads: 158

```
Tbh I was thinking of making one myself with kydex by making a wood block the same size as the batteries then molding it over the block
```

---
## \#103 Posted by: mmaner Posted at: 2017-12-20T03:38:28.626Z Reads: 171

```
[quote="GrecoMan, post:95, topic:39765"]
personally think it’ll look weird with that huge mound of batteries ontop
[/quote]

I've been sitting on a MBS Comp 95 build for 4 months for that exact reason. It's 80% complete but I hate the idea of batteries on he top.
```

---
## \#104 Posted by: Sirshaunsta Posted at: 2017-12-20T03:45:19.070Z Reads: 165

```
For me it's not a huge deal, it makes it look sorta like a street version of trampa board to me and I think they're sick. If I could get my hands on 107mm wheels I'd be ecstatic
```

---
## \#105 Posted by: Sirshaunsta Posted at: 2017-12-20T03:58:52.348Z Reads: 158

```
So as it stands by board had 60mm clearance and motors will have about 35 or 45 I expect after mounting
```

---
## \#106 Posted by: telnoi Posted at: 2017-12-20T13:47:14.135Z Reads: 157

```
People are too concerned with looks. Especially with a mountain board, I would never consider putting packs under a board...unless you don't really use the board for the intended purpose/just for show.

It should work, be reliable and not burst into flames when you hit a few rocks.

If you  need it lower profile you can think about just going with swappable packs. Carry the rest in a backpack.
```

---
## \#107 Posted by: mmaner Posted at: 2017-12-20T13:55:28.938Z Reads: 152

```
[quote="telnoi, post:106, topic:39765"]
People are too concerned with looks.
[/quote]

I disagree, there's some ugly ass boards around 😀.  I'm just looking for a better way that a box in top.
```

---
## \#108 Posted by: telnoi Posted at: 2017-12-20T14:01:49.493Z Reads: 152

```
If the ugly board goes faster and is still going at the end of the trip as opposed to the bottom mounted disaster with a split case and electronics hanging out, I'd go with the "ugly" board.

Different regions, different terrains, different solutions required.
```

---
## \#109 Posted by: mmaner Posted at: 2017-12-20T14:04:08.539Z Reads: 159

```
Did, can you read?  I said I'm looking for a better way.   Why don't you go build a few boards and then come back.
```

---
## \#110 Posted by: telnoi Posted at: 2017-12-20T14:08:11.639Z Reads: 166

```
Yup, my reading skills are over 9000. No need to build multiple boards to understand space limitations.

Looking forward to your upcoming solution and how it will solve that issue of having an ugly bulge (thinking TARDIS, you know..it's bigger on the inside).
```

---
## \#111 Posted by: GrecoMan Posted at: 2017-12-20T14:08:51.690Z Reads: 179

```
that’s what i thought too. duct taped sketchy looking batteries to my board and called it a day. it worked but cmon... it you go into any public place with something that looks like a sophisticated bomb you will get kicked out. I know from experience. Just go the extra mile and make something that you feel like you can show off while working well

if you don’t know what i’m talking about, my board went from this:
<img src="/uploads/db1493/original/3X/5/a/5a6b8c7d710481c75fa260e9d718f2e7e49f0562.jpeg" width="375" height="500">

to this:
<img src="/uploads/db1493/original/3X/0/5/05da0bfadd8853aa70a3412e2a8925b2e47dc7b2.jpeg" width="374" height="500">

both worked, but I feel 200% more comfortable taking v2 into any sort of public place
```

---
## \#112 Posted by: telnoi Posted at: 2017-12-20T14:29:40.294Z Reads: 172

```
I'm sure he won't use ductape :smile:
```

---
## \#113 Posted by: Sirshaunsta Posted at: 2017-12-20T16:57:41.090Z Reads: 178

```
For everyone concerned about size of batteries, the lipos are my first attempt. In future I intend to build a lithium cell myself using these I found online, 3.7v 9800mah singles my idea was 10 is series and 3 packs in series ×2. So 60 cells to make 2 10s 3p 29 400 mah. Giving almost 30ah to each end of the board. Thoughts?<img src="/uploads/db1493/original/3X/e/8/e8900b6f878e707551f79c5c9fc2e407faa4b43c.jpg" width="281" height="500">
```

---
## \#114 Posted by: Sirshaunsta Posted at: 2017-12-20T16:58:31.594Z Reads: 160

```
And no NEVER duct tape. Ill find a much nicer way to secure and enclose them
```

---
## \#115 Posted by: pylotope Posted at: 2017-12-20T17:08:13.881Z Reads: 164

```
[quote="Sirshaunsta, post:113, topic:39765"]
In future...
[/quote]

I too dream of the future when we have 9800mAh 18650 cells.
```

---
## \#116 Posted by: FredrikHems Posted at: 2017-12-20T17:14:08.831Z Reads: 166

```
Don't buy that cells. They are AS fake AS u can Get em. They usually only have a capacity of something around 500mah
```

---
## \#117 Posted by: Sirshaunsta Posted at: 2017-12-20T17:26:25.887Z Reads: 161

```
Thanks boys I was skeptical but didn't know for sure.
```

---
## \#118 Posted by: Sirshaunsta Posted at: 2017-12-20T18:00:34.162Z Reads: 157

```
Will be ordering the trucks and mounts this weekend when I get paid, then it's a waiting game as it's been about a month since I ordered my focboxs. Still waiting for those
```

---
## \#119 Posted by: GrecoMan Posted at: 2017-12-20T21:17:59.841Z Reads: 157

```
highest 18650 cell right now (usable for esk8) is the 30q from samsung, around 3000mah
```

---
## \#120 Posted by: pat.speed Posted at: 2017-12-20T21:57:44.175Z Reads: 159

```
So far I think the highest capacity 18650 is 3450 or something but it only has 10a discharge☹️ Although with a 10s10p that's 100 amps of power👍
```

---
## \#121 Posted by: Sirshaunsta Posted at: 2017-12-21T03:37:10.605Z Reads: 161

```
My 20c 5s batteries each deliver 100 amps and with between 8 and 16 of them I think I'll be good ;P
```

---
## \#122 Posted by: Cobber Posted at: 2017-12-21T06:16:20.957Z Reads: 174

```
[quote="mmaner, post:103, topic:39765"]
I've been sitting on a MBS Comp 95 build for 4 months for that exact reason. It's 80% complete but I hate the idea of batteries on he top.
[/quote]

Have you seen eboosted's trampa enclosure? that might fit and is pre-curved?
http://www.electric-skateboard.builders/t/eboosted-enclosures-thread/38073/28?u=cobber

http://www.electric-skateboard.builders/uploads/db1493/optimized/3X/2/3/234244af1c1fda722a3db88e7c4226173ff960a8_1_690x388.jpg
```

---
## \#123 Posted by: Sirshaunsta Posted at: 2017-12-21T07:03:55.408Z Reads: 167

```
My batteries as it stands form a 115×155×160mm I might end up taking a layer of 40mm off the 115 and make 4 10s4p battery packs or add 40 63mm to make 2 giant 10s8p. The 4 would serve me as 1 pack feed front and another to rear with a backup for both, whereas the 2 giants would go 1 to each end continuously
```

---
## \#124 Posted by: Sirshaunsta Posted at: 2017-12-21T07:06:47.241Z Reads: 159

```
I might also just use the 12 batteries I have to make 2 10s 4p packs and 2 10s 2p packs a small and a large for different riding distances and for the ability to swap during rides
```

---
## \#125 Posted by: pat.speed Posted at: 2017-12-21T09:11:09.868Z Reads: 156

```
Why don't you have one lot of batteries in an enclosure below the board. Then have a xt90 poking through the deck in the middle so if you want you can add extra batteries in parallel between your feet for mad range
```

---
## \#126 Posted by: mmaner Posted at: 2017-12-21T12:54:18.222Z Reads: 158

```
[quote="Cobber, post:122, topic:39765"]
Have you seen eboosted's trampa enclosure?
[/quote]

I have and it's awesome but the compartments require a battery built in sections and I all ready have a pack I'd like to use.
```

---
## \#127 Posted by: Sirshaunsta Posted at: 2017-12-21T14:44:54.202Z Reads: 155

```
To me that would be very silly to put my batteries under the board at all because of the clearance . I put them on top for practicality not aesthetics. Idc if I have a big box on top of the board as long as it functions and is protected from rocks n curbs
```

---
## \#128 Posted by: Sirshaunsta Posted at: 2017-12-21T16:33:18.839Z Reads: 158

```
And honestly with the 16 5s 5ah 20c batteries I plan to use, there's really no point in trying to space them out under the board, I will have MAD range though with 2 separate 10s 20ah 20c batteries(I believe the c rating does not change by wiring series or parallel it is a consistent level of current draw per battery nomatter the amount I use) so each pack should take me roughly 66km with weight according to my calculator. At this point I'm not sure if running them separate will double my range between the 4 motors or if I should make it a single 10s 8p 40ah 20c and use some of y harness to connect the single battery to 4 focbox followed by 4 motors
```

---
## \#129 Posted by: Sirshaunsta Posted at: 2017-12-21T16:41:16.791Z Reads: 155

```
That's 740wh each battery, and each battery powers 2 motors bro as 1 battery it'd be 1480 wh
```

---
## \#130 Posted by: FredrikHems Posted at: 2017-12-21T16:59:20.529Z Reads: 158

```
To be honest, I am freaking jealous about you batteries. :joy: About the c -rating. This is the c number (in your case 20) multiplied with the Ah rating. so if you decide to make two batteries who have a capacity of 20Ah each, each battery can deliver 400A each (20Ah*20). If you decide to build one who have a capacity of 40Ah, that one battery can deliver 800 fucking amps. (40Ah*20). This is far more than you will ever need, so you will have veeeery little voltage sag, which is positive. 
In fact, that battery have the ability to deliver enough amps to a damn tesla.
```

---
## \#131 Posted by: Sirshaunsta Posted at: 2017-12-21T17:03:00.519Z Reads: 173

```
2 batteries<img src="/uploads/db1493/original/3X/8/a/8acf1ae1b4a44abe70790a30d8bcf76741ada1df.png" width="281" height="500"><img src="/uploads/db1493/original/3X/3/4/34f445f943fa256a5deb7844d6a301fec33d0ab8.png" width="281" height="500">
1 battery 
<img src="/uploads/db1493/original/3X/8/f/8f9b49bb71d15ad42b31b3d37d08ebed687f1182.png" width="281" height="500"><img src="/uploads/db1493/original/3X/3/9/3973db872266e121438ca7071256ea3bfcf9cabf.png" width="281" height="500">
```

---
## \#132 Posted by: Sirshaunsta Posted at: 2017-12-21T17:04:57.668Z Reads: 153

```
Also I plan to run 20/30 gearing for those top speeds on 97mm. Got a guy Wil 3d printer and gonna ask him to make me the sprockets
```

---
## \#133 Posted by: FredrikHems Posted at: 2017-12-21T17:35:42.560Z Reads: 156

```
20/30? Thats a really heavy gearing, and your setup will most likely be very inefficient. 
You will get an estimated top speed of almost 90km/h.. Do you really want this? I would say aim for 50-60km/h max, and you will still have plenty of torque
```

---
## \#134 Posted by: Sirshaunsta Posted at: 2017-12-21T17:41:09.370Z Reads: 148

```
1.5 instead of 2.25 seemed nice to mme ;P I was also thinking 18/32 for 1.78 or 20/36 for 1.83 ratio which id still hit 65 to 70kmph but have some reserve torque to climb hills
```

---
## \#135 Posted by: Sirshaunsta Posted at: 2017-12-21T17:42:04.704Z Reads: 147

```
I want to have a top speed of atleast 60 even if i only hit it a handful of times but im sure the way i ride ill hit it many times
```

---
## \#136 Posted by: FredrikHems Posted at: 2017-12-21T18:40:44.366Z Reads: 148

```
Dang. U´r crazy. You you have any kind of experience of riding non-electric longboard from before?
```

---
## \#137 Posted by: Sirshaunsta Posted at: 2017-12-21T19:19:01.958Z Reads: 153

```
Tonnes, I literally ride my board to and from town everyday in the summer which is about 13 k in and 13 k out with hills, a few of the hills are quite steep to the point I kept up with ongoing traffic going down, speed limit 60kmph the last 5 yrs
```

---
## \#138 Posted by: Sirshaunsta Posted at: 2017-12-21T19:24:48.131Z Reads: 176

```
First board
<img src="/uploads/db1493/original/3X/b/6/b6d049cd15af595c84649d15898e82ee6fd67d6d.jpg" width="374" height="500">
<img src="/uploads/db1493/original/3X/2/7/27a0e02be43a550af7c1a49cc616994aa2d6e560.jpg" width="374" height="500">
 2nd board
<img src="/uploads/db1493/original/3X/1/7/174a16ab0719088f6fcefea1921257a55207a0d0.jpg" width="374" height="500">
<img src="/uploads/db1493/original/3X/e/3/e32c92c1131b806e713e45092de16c963de608c2.jpg" width="374" height="500">
 Electric boardboard
<img src="/uploads/db1493/original/3X/3/d/3d78131febcb990333c8b31c590715c852d7fa98.jpg" width="374" height="500">
<img src="/uploads/db1493/original/3X/7/d/7d3851e76e2cfc1732f37692293f77ebaf0b2add.jpg" width="374" height="500">
```

---
## \#139 Posted by: Sirshaunsta Posted at: 2017-12-21T19:37:29.366Z Reads: 163

```
^^ look up ^^
```

---
## \#140 Posted by: FredrikHems Posted at: 2017-12-21T19:38:43.731Z Reads: 156

```
Aha. Good that you have alot of experience!
```

---
## \#141 Posted by: Sirshaunsta Posted at: 2017-12-21T19:39:37.604Z Reads: 149

```
Yeah dude and the scratches on that board/trucks aren't from wipeputs or rocks, it's from the skate park where I do grinds and such. I've also jumped quite a few times
```

---
## \#142 Posted by: Sirshaunsta Posted at: 2017-12-21T19:39:53.770Z Reads: 148

```
Idk why it didn't tag you
```

---
## \#143 Posted by: Sirshaunsta Posted at: 2017-12-21T20:59:36.792Z Reads: 146

```
So I just put in the order for trucks and xt90 y harness for parallel and series. Waiting still to order mounts and belts
```

---
## \#144 Posted by: Sirshaunsta Posted at: 2017-12-21T21:00:18.346Z Reads: 144

```
Now the only part I haven't ordered is mounts n belts, also bought ceramic bones super redz for the 97mm wheels
```

---
## \#145 Posted by: pat.speed Posted at: 2017-12-21T21:09:42.213Z Reads: 142

```
I suggest you go for the 18/32 gear ratio for more torque since you said there are hills
```

---
## \#146 Posted by: Sirshaunsta Posted at: 2017-12-21T21:12:56.446Z Reads: 143

```
Yes some quite steep too @pat.speed
```

---
## \#147 Posted by: Sirshaunsta Posted at: 2017-12-21T21:17:06.313Z Reads: 148

```
Though i figure using 4 motors would mean I could  use 4x the torque but in real world I allowed for tolerance and assume 3x instead which still should allow plenty more torque with the 18/32 gearing with an optimal top speed and still fit the belt size of the order as aposed to 16/36
```

---
## \#148 Posted by: Sirshaunsta Posted at: 2017-12-21T21:22:53.397Z Reads: 141

```
I may just get both the 18/32  and the 20/30 made for me and see which works best for my local terrain and commute
```

---
## \#149 Posted by: Kug3lis Posted at: 2017-12-21T21:25:01.376Z Reads: 143

```
I dont suggest to use 3d printed gears in applications higher than 30km/h... They will be so badly balanced that it will behave more like vibrator than a puley...
```

---
## \#150 Posted by: Sirshaunsta Posted at: 2017-12-21T21:26:34.261Z Reads: 138

```
Really? I though 3d would be the way to go there being light and sturdy, i don't think it's that much weaker than the plastic diy uses is it?
```

---
## \#151 Posted by: pat.speed Posted at: 2017-12-21T21:26:35.526Z Reads: 135

```
Yeah. Or try and keep the same wheel pulley and just change the motor pulley that way it will be much quicker to snap gear ratios. You could also have an uneven board where you have a 15:40 on the rear and 20/32 on the front. Then lots of torque and speed😊
```

---
## \#152 Posted by: Kug3lis Posted at: 2017-12-21T21:27:43.333Z Reads: 131

```
U dont want to have different speeds on wheels...
```

---
## \#153 Posted by: Sirshaunsta Posted at: 2017-12-21T21:28:13.245Z Reads: 130

```
Nice thought but applying different gearings between ends will make the board imbalanced and cause the lower gear to overheat when the high speed comes
```

---
## \#154 Posted by: pat.speed Posted at: 2017-12-21T21:28:30.164Z Reads: 132

```
Actually @lowGuido has tested this and so have others and it seems to work perfectly fine
```

---
## \#155 Posted by: Sirshaunsta Posted at: 2017-12-21T21:28:59.717Z Reads: 135

```
At full speed? For over 50km?
```

---
## \#156 Posted by: Kug3lis Posted at: 2017-12-21T21:29:22.473Z Reads: 144

```
Plastic is either injected molded, or milled. 3d printed is additive creation, which just spits out plastic.

@pat.speed I am just saying you don't want to have different speed trust me...
```

---
## \#157 Posted by: pat.speed Posted at: 2017-12-21T21:30:44.684Z Reads: 143

```
Yes because once the slower geared motors reach there max they just spin faster and faster until they reach the same speed as the other motor.
```

---
## \#158 Posted by: Kug3lis Posted at: 2017-12-21T21:31:31.564Z Reads: 147

```
It works but not the way it should, the slower wheels gets pushed faster which makes stress on ESC if you use VESC you can blow DRV easily. Plus if motor reaches its configuration peak it can get damaged as it will start generating more current as it can handle...
```

---
## \#159 Posted by: pat.speed Posted at: 2017-12-21T21:31:54.912Z Reads: 144

```
Why not? The board will be at the same speed until the slowest motor reach their max speed. Once that happens the faster ones kick in kinda like turbo
```

---
## \#160 Posted by: pat.speed Posted at: 2017-12-21T21:32:37.711Z Reads: 143

```
Oh yes I forgot about erpm my bad
```

---
## \#161 Posted by: Kug3lis Posted at: 2017-12-21T21:33:14.563Z Reads: 136

```
From speed 1 it will be different speed on wheels, then the slower motors will begin to work as generators instead of pushing
```

---
## \#162 Posted by: Sirshaunsta Posted at: 2017-12-21T21:34:18.441Z Reads: 130

```
No my friend, over turning the high torque motors will result in possible overload on vesc as stated
```

---
## \#163 Posted by: pat.speed Posted at: 2017-12-21T21:34:53.523Z Reads: 135

```
Yes I guess they would. I think lowguido must have been using car escs to not hit the erpm because one of his motors were 400kv
```

---
## \#164 Posted by: pat.speed Posted at: 2017-12-21T21:35:19.768Z Reads: 140

```
Overheat on Vesc yes, over heat on motors no
```

---
## \#165 Posted by: Cobber Posted at: 2017-12-21T21:35:26.536Z Reads: 150

```
just going to leave this here...

https://www.electric-skateboard.builders/t/uneven-dual-rear-drive/113

it has all been discussed
```

---
## \#166 Posted by: Sirshaunsta Posted at: 2017-12-21T21:35:32.484Z Reads: 141

```
200+amp esc I wanna see this
```

---
## \#167 Posted by: pat.speed Posted at: 2017-12-21T21:38:31.638Z Reads: 148

```
Thank you @Cobber the thread explains it a lot better👍
```

---
## \#168 Posted by: Sirshaunsta Posted at: 2017-12-21T21:41:04.099Z Reads: 140

```
I've planned this buld from start to eliminate as much heat as possible on each part from displacing load to 4 motors to multiple high amp escs(focbox) less than max volt battery (10s) and plenty battery amp delivery 200 available to each motor which each max at 75) so I will never heat up batteries or vesc or motor
```

---
## \#169 Posted by: pat.speed Posted at: 2017-12-21T21:44:44.270Z Reads: 141

```
[quote="Sirshaunsta, post:153, topic:39765"]
cause the lower gear to overheat when the high speed comes
[/quote]

Huh? Um... I though it wasn't going to overheat
```

---
## \#170 Posted by: Sirshaunsta Posted at: 2017-12-21T21:46:37.272Z Reads: 134

```
Your idea would overheat I am using 4 identical gearings @pat.speed
```

---
## \#171 Posted by: pat.speed Posted at: 2017-12-21T22:05:46.324Z Reads: 126

```
Read the thread the cobber posted again. He only used two motors and neither overheated
```

---
## \#172 Posted by: Sirshaunsta Posted at: 2017-12-21T22:10:48.602Z Reads: 132

```
I like the link but I'd rather keep the torque in each end balanced to minimize problems, as I said before I designed this to be balanced from end to end every detail
```

---
## \#173 Posted by: Sirshaunsta Posted at: 2017-12-21T22:17:31.150Z Reads: 131

```
Having the torque of 4 190kv I believe I'll be able to gear for 60+kmph without losing speed or traction on hills
```

---
## \#174 Posted by: Kug3lis Posted at: 2017-12-21T22:19:30.489Z Reads: 130

```
Please invest some time in physics or related stuff because your leading people the wrong way ;)
```

---
## \#175 Posted by: pat.speed Posted at: 2017-12-21T22:27:51.257Z Reads: 132

```
I'm planning to do so once I finish school, evidence > physics 👍
```

---
## \#176 Posted by: Kug3lis Posted at: 2017-12-21T22:30:11.459Z Reads: 137

```
U know how many tests cases are needed to make something a proof? For simple example ask any mechanic what would happen if car front/rear wheels are driven at different speed :) They will tell you from practice
```

---
## \#177 Posted by: Kug3lis Posted at: 2017-12-21T22:31:38.571Z Reads: 132

```
Plus the evidence is just that he rides, you don't know anything else, maybe his motor already is dead or something else.
```

---
## \#178 Posted by: Sirshaunsta Posted at: 2017-12-21T22:32:32.747Z Reads: 134

```
This is why I want equal power distribution, it's no different from a high performance car? They use the same torque and hp at each wheel
```

---
## \#179 Posted by: Kug3lis Posted at: 2017-12-21T22:34:13.170Z Reads: 134

```
That's what diff does ;)
```

---
## \#180 Posted by: Sirshaunsta Posted at: 2017-12-21T22:36:32.355Z Reads: 135

```
He means Differential driveshaft for the idiots out there
```

---
## \#181 Posted by: Sirshaunsta Posted at: 2017-12-21T23:01:34.210Z Reads: 132

```
I'll update my build photos when more parts arrive, for now I'm waiting on 4 focbox, some wires, and trucks  after the weekend mounts will be ordered to complete the build, I will keep everyone in the loop
```

---
## \#182 Posted by: Orin635 Posted at: 2017-12-21T23:05:02.838Z Reads: 133

```
If you don't mind me asking
how much in total are you spending on this build?
```

---
## \#183 Posted by: Sirshaunsta Posted at: 2017-12-21T23:20:18.641Z Reads: 133

```
Well, alot :P 400- motors, 800-esc, 60-wheels, 60-bearings, 50-contoller/receivers, 750-batteries, 100-board, 175-wires, 75-voltmeter and killswitch/antispark) 900-motormounts/belts/pulleys, 45-special 20t motor pulley, 80-lights, etc. Roughly 3800 Canadian or 2750ish american so far with another 200 Canadian to spend on batteries for 16 instead of 12 so 4 thousand Canadian or 3 thousand American
```

---
## \#185 Posted by: Sirshaunsta Posted at: 2017-12-21T23:22:00.381Z Reads: 138

```
Including tax and shipping
```

---
## \#186 Posted by: caustin Posted at: 2017-12-21T23:33:18.234Z Reads: 148

```
You might benefit from a few of the folks who have recently built high end (equipment, price, speed, etc) commenting on your build specs.  Looks like a beast but caveat some concern on 20/30 gearing, not sure if AWD will compensate torque loss when you hit a hill of stature lol.

@BigBoyToys
@psychotiller
@longhairedboy
@etc (lol)
```

---
## \#187 Posted by: caustin Posted at: 2017-12-21T23:34:06.049Z Reads: 136

```
oops sorry @evoheyax and everyone else I left off the ping list lol
```

---
## \#188 Posted by: Sirshaunsta Posted at: 2017-12-21T23:35:41.451Z Reads: 132

```
I may just end up going 20/36 If I can't find a reliable wheel pulley as some say it may be unusable from a 3d printer.
```

---
## \#189 Posted by: Sirshaunsta Posted at: 2017-12-21T23:40:17.647Z Reads: 136

```
It would still allow me 65kmph top speed
```

---
## \#190 Posted by: Orin635 Posted at: 2017-12-21T23:40:31.200Z Reads: 134

```
Wow. Why are you spending 900 on pulleys system. I could build 3 of my builds for that price😂
```

---
## \#191 Posted by: Kug3lis Posted at: 2017-12-21T23:43:03.187Z Reads: 128

```
One thing I doubt is the you will not have enough torque to reach that speed...
```

---
## \#192 Posted by: Sirshaunsta Posted at: 2017-12-21T23:44:23.483Z Reads: 130

```
The motor mounts at 299 american per set with 15mm belts making 900 Canadian after shipping
```

---
## \#193 Posted by: Sirshaunsta Posted at: 2017-12-21T23:46:17.731Z Reads: 131

```
Im not sure either but thats what the calculator says for single drive and im using 4wd so i figure any max calc it has will be achieveable
```

---
## \#194 Posted by: Kug3lis Posted at: 2017-12-21T23:47:34.210Z Reads: 134

```
Calculators don't count torque... Its not even mention usually in motor page...
```

---
## \#195 Posted by: Kug3lis Posted at: 2017-12-21T23:47:52.665Z Reads: 131

```
Those speeds are best-case scenarios at 100% efficiency
```

---
## \#196 Posted by: Sirshaunsta Posted at: 2017-12-21T23:50:03.034Z Reads: 159

```
<img src="/uploads/db1493/original/3X/b/f/bf5b872beaa3b56bc6a124ab58beb45838b12be4.png" width="281" height="500">
<img src="/uploads/db1493/original/3X/9/5/95fba2b56596cb8283abee3fa107a64adb4a04cf.png" width="281" height="500">
<img src="/uploads/db1493/original/3X/f/7/f7a2a0e2e5a642153b6af97ef6ba00282b8fe139.png" width="281" height="500">
```

---
## \#197 Posted by: scepterr Posted at: 2017-12-21T23:50:36.860Z Reads: 137

```
http://calc.esk8.today/advanced/
This gives max hill grade %
```

---
## \#198 Posted by: Kug3lis Posted at: 2017-12-21T23:51:13.619Z Reads: 136

```
but they dont count motor torque...
```

---
## \#199 Posted by: Orin635 Posted at: 2017-12-21T23:51:49.657Z Reads: 143

```
Wow that's alot. I can't  wait to see the finished build. I'm also in middle of making my board but it's been stopped because I can only work on the board in school and it's Christmas break but your board sounds amazing
```

---
## \#200 Posted by: BigBoyToys Posted at: 2017-12-22T00:20:19.586Z Reads: 151

```
45mph theoretical top speed sounds about right to me. 

Youll have ample torque with 4wd but youll need to run pretty high motor amp settings. One of my 4wd's hub boards is geared for over 40mph and has way more than enough torque.

It takes me about 4000w to hold speeds above 45mph, so don't think youll be able to get much faster than 45mph without hitting the thermal backoff of the FOC box's anyway. They seem to start getting hot at sustained power levels above 1000W each for me.
```

---
## \#201 Posted by: Sirshaunsta Posted at: 2017-12-22T14:17:25.002Z Reads: 147

```
Thank you, yes in total my board should be capable of 2450×4 watts  so over 12 hp idk how much torque that adds up to yet
```

---
## \#202 Posted by: MoeStooge Posted at: 2017-12-22T15:16:51.543Z Reads: 145

```
<img src="/uploads/db1493/original/3X/0/c/0c9715a90e146cafba647a800c7bbc756eb88758.jpg" width="328" height="500">
```

---
## \#203 Posted by: Kug3lis Posted at: 2017-12-22T16:00:27.157Z Reads: 133

```
Again, power is not linear ;)
```

---
## \#204 Posted by: Sirshaunsta Posted at: 2017-12-22T17:40:53.930Z Reads: 133

```
My motors are rated up to 2450 watts each×4 I believe and 75 amps×4, focbox handle 120amps×4, batteries I'm using handle 800 amps total. I DOUBT I'll ever run into heat through lack of ability. Though motors maaay get warm during rigorous use I think that's about it
```

---
## \#205 Posted by: MoeStooge Posted at: 2017-12-22T17:59:58.334Z Reads: 137

```
Put it on a Dyno if you want real #s otherwise  be ok with people who work in the world of approximates.
```

---
## \#206 Posted by: Kug3lis Posted at: 2017-12-22T18:28:28.115Z Reads: 146

```
It's not even approximated... You took car torque calculator for the petrol engine and used it for the electric motor, then the highest power is only at low RPM side to make it move which is the complete opposite of car engine...

Here is basic graph of brushless motor

<img src="/uploads/db1493/original/3X/1/4/14de9a26c84bbc9708011c5591652bb5e7eb1c41.png" width="400" height="251">
```

---
## \#207 Posted by: BigBoyToys Posted at: 2017-12-22T19:23:24.168Z Reads: 142

```
Why would the calculator he used matter? The math is the same by definition.

Torque = (hp × 5252)/rpm.

The only concern I have is that in order for the calculator to yield the correct torque calculation, the rpm entered would need to correspond to motor speed at which the entered HP number occured.
```

---
## \#208 Posted by: MoeStooge Posted at: 2017-12-22T19:40:39.446Z Reads: 145

```
True: will do It this way for fun... <img src="/uploads/db1493/original/3X/0/f/0fc1e54bd825de4dd78f360a37a89061514bed71.jpg" width="400" height="500"> <img src="/uploads/db1493/original/3X/5/d/5d1b916b0c986a3f501f2ddbebb984b9ada11a58.jpg" width="626" height="500">. Hey it's approximately the same.  Close enough for horse shoes and hand grenades. You can spend all the time ya want, getting as close as ya want with long math but once again that's what a Dyno is for. Approximates will let ya know the area you are standing in so you can move forward without crying about the math.  Life and death I will choose math first. But not with this..
```

---
## \#209 Posted by: Kug3lis Posted at: 2017-12-22T19:53:42.499Z Reads: 138

```
If taking into consideration most common power graph of outrunner brushless motor you will have this amount of torque ;)

<img src="/uploads/db1493/original/3X/2/4/241ae1bef9cd0075dcae7386b8611916b78fe44a.png" width="618" height="298">
```

---
## \#210 Posted by: MoeStooge Posted at: 2017-12-22T20:53:39.416Z Reads: 134

```
<img src="/uploads/db1493/original/3X/4/d/4d5f86506a5d73d8212848706562b6306b1449e3.jpg" width="690" height="208"> so what your saying here is if you take a 10hp motor and attatch a 1 ft lever to it and at the end of the fulcrum I will see 21.5 lbs of pull?  I can't  play horse shoes or hand grenades with this. Ok now your gonna shorten from 1 foot to the radius on a pinion, now ratio that to your gear,  now to your wheel size, . With that wheel torque it Should climb the side of a building.
```

---
## \#211 Posted by: Kug3lis Posted at: 2017-12-22T21:02:41.151Z Reads: 126

```
It's just a torque, you forgot a whole system of other forces, gravity, friction and etc... It's best case scenario at 100% efficiency.
```

---
## \#212 Posted by: Sirshaunsta Posted at: 2017-12-22T22:06:11.918Z Reads: 138

```
Where are you guys getting the 9.8kw spec from I'm honestly curious cause I don't know, the calculator I used said roughly 750watts in a brushless made 1 hp, so having 2450 in each motor×4 adds to 9400 watts giving me about 12 or 13 hp ROUGHLY
 <img src="/uploads/db1493/original/3X/a/a/aadfe32d8a221aacf40d50c8aa5ed63328d4caba.png" width="281" height="500">
```

---
## \#213 Posted by: FredrikHems Posted at: 2017-12-22T22:34:25.195Z Reads: 123

```
What? Didnt you buy the 6374 192kv motors?
```

---
## \#214 Posted by: pat.speed Posted at: 2017-12-22T22:37:50.708Z Reads: 124

```
Guys you need to remember that he will only get as many watts to his motors as his focboxes can handle, which is about 40/50amps cont at 42v is around 2100 watts per focbox
```

---
## \#215 Posted by: Sirshaunsta Posted at: 2017-12-22T23:12:11.055Z Reads: 122

```
No I got the 190s
```

---
## \#216 Posted by: Sirshaunsta Posted at: 2017-12-22T23:12:33.049Z Reads: 123

```
Focbox are rated for 120amp are they not?
```

---
## \#217 Posted by: pat.speed Posted at: 2017-12-22T23:14:18.464Z Reads: 125

```
120amps pulses for a few seconds. Enertion claims 60 amps constantly but I doubt that more like 40 /50 amps
```

---
## \#218 Posted by: Sirshaunsta Posted at: 2017-12-22T23:14:53.767Z Reads: 145

```
I see you are right <img src="/uploads/db1493/original/3X/5/c/5c7ccd0bb75151a521fef73a8aba1303aa8f65cc.png" width="281" height="500">
```

---
## \#219 Posted by: Sirshaunsta Posted at: 2017-12-22T23:15:57.438Z Reads: 145

```
Here's hoping I only need to draw 40 or 50 amps per motor to achieve my speed goals
```

---
## \#220 Posted by: BigBoyToys Posted at: 2017-12-23T01:10:20.401Z Reads: 148

```
Probably less than 30A each. You can watch my total amp draw on the data overlay in this video at various speeds upto 49mph to get an idea. This is riding a 4wd hub motor board with a 265lb rider.

https://youtu.be/0PNWIaXaFvw
```

---
## \#221 Posted by: Sirshaunsta Posted at: 2017-12-23T01:33:49.277Z Reads: 149

```
Thank you, I am 155 plus whatever I'm carrying maybe up to 20lbs to 175 max with a 20-30lb board closer to 25, so my 4 190kv motors are propelling 200lbs with 10s
```

---
## \#222 Posted by: Sirshaunsta Posted at: 2017-12-23T01:34:19.948Z Reads: 137

```
Look up I hate the tagging in this
```

---
## \#223 Posted by: Sirshaunsta Posted at: 2017-12-23T01:38:18.213Z Reads: 134

```
4 190s I don't think I'll have any lack of torque lugging my ass to high weighted tops speeds as suggested in calculators before of over 60kmph without fail
```

---
## \#224 Posted by: BigBoyToys Posted at: 2017-12-23T01:46:23.489Z Reads: 129

```
Agreed, you'll have plenty 👌
```

---
## \#225 Posted by: Sirshaunsta Posted at: 2017-12-23T05:52:40.368Z Reads: 131

```
My gearing will also be  
Either 16/36 as norm or I will use 3d printed 18/32
```

---
## \#226 Posted by: FredrikHems Posted at: 2017-12-23T09:52:15.402Z Reads: 127

```
Dont go for 3D printed motor pulleys. They will not last long, unless you use a really tought material.
```

---
## \#227 Posted by: pat.speed Posted at: 2017-12-23T11:30:00.978Z Reads: 131

```
Why not keep the same wheel pulley (36t)  and just change the motor pulley between a 16t and 20t depending on the speed you want. It gives pretty much the same gear ratios
```

---
## \#228 Posted by: Sirshaunsta Posted at: 2017-12-23T11:30:04.608Z Reads: 130

```
Like what material?
```

---
## \#229 Posted by: Sirshaunsta Posted at: 2017-12-23T11:30:45.620Z Reads: 123

```
That was my plan but I need to find a 12mm 20tooth and diy only has 15mm
```

---
## \#230 Posted by: pat.speed Posted at: 2017-12-23T11:50:27.875Z Reads: 125

```
You can run a 12mm belt on a 15mm pulley there will just be a bit of extra room. I am running a 10mm belt on a ~20mm belt and I just wrapped some tape around the extra bit of space to keep the belt in the right spot
```

---
## \#231 Posted by: GrecoMan Posted at: 2017-12-23T13:29:38.107Z Reads: 123

```
steel

10chars
```

---
## \#232 Posted by: FredrikHems Posted at: 2017-12-23T14:53:40.663Z Reads: 123

```
It may work with polycarbonate, Acetal or similar, but its better in the long run to Get a steel one
```

---
## \#233 Posted by: Sirshaunsta Posted at: 2017-12-23T18:43:10.699Z Reads: 122

```
Does it depend on the printer if they are able to make it with the specific material? How much would it cost roughly for 4 18tooth 12mm motor pulleys and 4 32 tooth 12mm wheel pulleys roughly (just for materials)? Does anyone know?
```

---
## \#234 Posted by: Sirshaunsta Posted at: 2017-12-23T19:25:47.638Z Reads: 127

```
Or can anyone help put me in contact with somebody able to make these parts as needed to perform with my needs?
```

---
## \#235 Posted by: FredrikHems Posted at: 2017-12-23T19:37:39.236Z Reads: 130

```
If i were you i would have bought steel motor pulleys from here : https://eskating.eu/product/custom-htd-5m-12-to-20-teeth-steel-motor-pulley-in-91215-width-2x/ 

A 16t for example. And istead Go for 3D printed wheel pulleys. These can be made from alot more common materiale like ABS, PETG, nylon and more!
```

---
## \#236 Posted by: Sirshaunsta Posted at: 2017-12-23T21:15:51.163Z Reads: 128

```
So if I just went 16/30 Would this work well with a 3d printed wheel pulley. Will it still fit in the belt/mount[quote="FredrikHems, post:235, topic:39765, full:true"]
If i were you i would have bought steel motor pulleys from here : https://eskating.eu/product/custom-htd-5m-12-to-20-teeth-steel-motor-pulley-in-91215-width-2x/ 

A 16t for example. And istead Go for 3D printed wheel pulleys. These can be made from alot more common materiale like ABS, PETG, nylon and more!
[/quote]
```

---
## \#237 Posted by: Sirshaunsta Posted at: 2017-12-23T21:18:44.265Z Reads: 121

```
Or even 16/28?
```

---
## \#238 Posted by: FredrikHems Posted at: 2017-12-23T21:20:28.083Z Reads: 127

```
The belt lenght will totally depend on What mount you will use, and How much you can adjust the tension. What mount will you be using? An adjustable odler may be a good idea, as you can use the same belt lenght on both gear setups
```

---
## \#239 Posted by: Sirshaunsta Posted at: 2017-12-23T21:22:18.084Z Reads: 127

```
Using 4 single mount kits from diy (63mm)
```

---
## \#240 Posted by: FredrikHems Posted at: 2017-12-23T21:30:42.522Z Reads: 122

```
Well, They are pretty udjustable, so Thats good. But you may still need to use 2 different belt lenghts for the different gear ratios
```

---
## \#241 Posted by: Sirshaunsta Posted at: 2017-12-24T05:58:59.000Z Reads: 118

```
Different belts? I won't be able to adjust the current one to proper tension?
```

---
## \#242 Posted by: Sirshaunsta Posted at: 2017-12-24T08:01:14.590Z Reads: 110

```
Dropping 6 teeth is too much for same belt?
```

---
## \#243 Posted by: scepterr Posted at: 2017-12-24T08:05:18.656Z Reads: 111

```
Depends how adjustable the CTC is
```

---
## \#244 Posted by: Sirshaunsta Posted at: 2017-12-24T08:21:08.744Z Reads: 116

```
Ctc? I dont know the term yet
```

---
## \#245 Posted by: scepterr Posted at: 2017-12-24T08:22:59.554Z Reads: 121

```
Center to center distance of axle and motor shaft
```

---
## \#246 Posted by: FredrikHems Posted at: 2017-12-24T09:32:47.156Z Reads: 132

```
Since you Go down 6t, which is queit alot, you may still need to have a shorter / longer belt. But its really not that big of a deal. Belts arnt really expensive
```

---
## \#247 Posted by: Sirshaunsta Posted at: 2017-12-24T20:49:51.743Z Reads: 134

```
Ok thank you, if I do need new belts that's fine but I want a ratio under 2.00
```

---
## \#248 Posted by: Sirshaunsta Posted at: 2017-12-27T19:41:36.731Z Reads: 134

```
<img src="/uploads/db1493/original/3X/7/7/77961d16f328c4e063029472398d5d2b391e379d.jpg" width="374" height="500">
Wiring setup for 1 of my 10s4p 20 000mah batteries
```

---
## \#249 Posted by: Cobber Posted at: 2017-12-28T07:20:14.314Z Reads: 127

```
that is a lot of xt90 connectors dude.
keep an eye on them, check their operating temperatures regularly. If they start heating up, either re-solder or replace them ;)
```

---
## \#250 Posted by: pat.speed Posted at: 2017-12-28T07:24:09.375Z Reads: 124

```
At least 6 of those connectors could be removed by soldering the wires too
```

---
## \#251 Posted by: Sirshaunsta Posted at: 2017-12-28T07:29:33.793Z Reads: 125

```
I might look into that
```

---
## \#252 Posted by: pat.speed Posted at: 2017-12-28T07:32:00.825Z Reads: 126

```
Should help to keep resistance lower and thus amps. But I doubt a noticeable difference. Heat might be a bit lower too
```

---
## \#253 Posted by: Sirshaunsta Posted at: 2017-12-28T23:05:40.960Z Reads: 138

```
<img src="/uploads/db1493/original/3X/e/9/e9370f1034f0e2984226cc1147c224f302742f6e.jpg" width="374" height="500"><img src="/uploads/db1493/original/3X/f/0/f0f82cdbe2bed8b654d5e514d70dc1eb97d1f019.jpg" width="374" height="500">
 So these connections  won't be good enough? @Cobber
```

---
## \#254 Posted by: Cobber Posted at: 2017-12-29T02:54:46.804Z Reads: 132

```
If the wire-xt connector solder is good & they are pushed together tightly they are rated to 90A. Sometimes pre-bought ones have cold soldered joints or they can just get loose (not typical of a xt90, but something that can happen to any connector).
& regardless of the above a connector will have more resistance than a copper wire. I am not saying it will not work. I am not saying you have to change it, just be aware of the limitations or inherent weakness in your build so you can mitigate the risk.

ie. 
[quote="Cobber, post:249, topic:39765"]
keep an eye on them, check their operating temperatures regularly. If they start heating up, either re-solder or replace them :wink:
[/quote]
```

---
## \#255 Posted by: Sirshaunsta Posted at: 2017-12-29T03:06:24.008Z Reads: 128

```
Ok thank you, so I will likely switch from my 1 or 2 battery pack idea to a 4pack idea where I have 4 10s 10 000mah 20c batteries, each going to a separate motor to allow up to 90 amps to each motor even if they're rated for 65/75 this should help keep everything cool? @Cobber and lower resistance given that it will look like this
```

---
## \#256 Posted by: Sirshaunsta Posted at: 2017-12-29T03:08:13.400Z Reads: 134

```
<img src="/uploads/db1493/original/3X/4/1/41ae11d5b3176b78f5419184ff691be8bd8b44ca.jpg" width="374" height="500"> @Cobber
```

---
## \#257 Posted by: jamiex Posted at: 2017-12-29T03:08:39.788Z Reads: 130

```
this thing is going to be insane!
```

---
## \#258 Posted by: Sirshaunsta Posted at: 2017-12-29T03:09:53.597Z Reads: 130

```
Dude this board will climb hills over 40degrees (90% gradiant) @jamiex AT FULL THROTTLE(50-70KPH)
```

---
## \#259 Posted by: Sirshaunsta Posted at: 2017-12-30T11:27:04.370Z Reads: 123

```
Wait. @Cobber I know you mentioned that the xt90s are only safe up to 90 amps, having 4 motors would I not lower the amp draw to each motor enough to allow 1 pack to power all 4 or atleast just 2 packs for 4 motors?  Because when I put the specs in my calc making 4 small packs greatly lowers my range and I'd like to think it's simple as x4 the range of 1 pack, but I'm not sure about that ?
```

---
## \#260 Posted by: Sirshaunsta Posted at: 2017-12-30T11:28:19.202Z Reads: 121

```
As a single pack it says 132 km range as 4 packs each gets 33 km. So simply my question is, will 4 separate packs give me the same range as 1 large one when powering 4 motors simultaneously
```

---
## \#261 Posted by: Sirshaunsta Posted at: 2017-12-30T11:40:47.284Z Reads: 119

```
Using a dual setup do I want the overhang or no? @FredrikHems
```

---
## \#262 Posted by: FredrikHems Posted at: 2017-12-30T13:03:14.203Z Reads: 110

```
What do you mean with the "overhang"?
```

---
## \#263 Posted by: Sirshaunsta Posted at: 2017-12-30T13:05:09.625Z Reads: 107

```
The link you gave me earlier has the option for "overhang" @FredrikHems
```

---
## \#264 Posted by: GrecoMan Posted at: 2017-12-30T13:05:39.645Z Reads: 110

```
overhang, 2 flanges, 15mm wise keyway (for future)
```

---
## \#265 Posted by: Sirshaunsta Posted at: 2017-12-30T13:06:40.301Z Reads: 112

```
So the overhang just means the belts will be further from the motor and take up more space in hanger? @GrecoMan
```

---
## \#266 Posted by: GrecoMan Posted at: 2017-12-30T13:08:11.810Z Reads: 113

```
no, overhang just means you don’t have to rely on setscrews in the teeth only. with overhang allows the belt to be closer to motor mount than without
```

---
## \#267 Posted by: Sirshaunsta Posted at: 2017-12-30T13:08:56.690Z Reads: 109

```
Ok, would your recommend me using the overhang then? @GrecoMan
```

---
## \#268 Posted by: GrecoMan Posted at: 2017-12-30T13:09:50.318Z Reads: 110

```
yes.  you actually flip the pulley around so the overhang is facing towards the wheel. side with no overhang faces the motor mount.

what mounts are you using?
```

---
## \#269 Posted by: Sirshaunsta Posted at: 2017-12-30T13:11:10.937Z Reads: 106

```
Perfect you just cleared all my confusion, so using overhang I will have more space to position my motors and more reliability using extra screws @GrecoMan
```

---
## \#270 Posted by: GrecoMan Posted at: 2017-12-30T13:12:54.175Z Reads: 106

```
yup. it allows for the motor mount to be closer to the wheel pulley. less torsional stress on the motor shaft then if the belt was 10mm away from the motor mount.  general rule of thumb is motor mount should be 3-4mm away from wheel pulley.
```

---
## \#271 Posted by: Sirshaunsta Posted at: 2017-12-30T13:14:42.888Z Reads: 105

```
Perfect, I'll most likely be going 18/32 then cause a steel motor pulley and another guy gave me a link for 32 34 36 and 38 tooth wheel pulleys
```

---
## \#272 Posted by: Sirshaunsta Posted at: 2017-12-30T13:15:37.684Z Reads: 108

```
It's about 125 150 extra bucks but worth it i think after all said an done going from 16 36 to 18 32
```

---
## \#273 Posted by: GrecoMan Posted at: 2017-12-30T13:15:43.997Z Reads: 104

```
go for a steel motor pulley. 16t
aluminum wheel pulleys from @JLabs, 32-44t
```

---
## \#274 Posted by: Sirshaunsta Posted at: 2017-12-30T13:17:33.688Z Reads: 107

```
So I shouldn't use an 18 motor pulley? I only upped the tooth there because I'm lowering my wheel teeth and want the belt to still fit and be comfy in the mount
```

---
## \#275 Posted by: GrecoMan Posted at: 2017-12-30T13:19:39.262Z Reads: 102

```
what belt are you using?
```

---
## \#276 Posted by: Sirshaunsta Posted at: 2017-12-30T13:20:29.407Z Reads: 101

```
Standard 12mm that comes with the single mount kits from diy. @GrecoMan
```

---
## \#277 Posted by: GrecoMan Posted at: 2017-12-30T13:20:52.311Z Reads: 106

```
but what length...
```

---
## \#278 Posted by: Sirshaunsta Posted at: 2017-12-30T13:21:48.941Z Reads: 121

```
It doesn't say <img src="/uploads/db1493/original/3X/0/f/0ff7c25132271c88d2f9b81def612fe648c553ba.png" width="281" height="500">
```

---
## \#279 Posted by: Sirshaunsta Posted at: 2017-12-30T13:25:24.575Z Reads: 112

```
But looking at the other kit for the whole setup with trucks n wheels they used 265mm. So I'd assume they're using 265mm
```

---
## \#280 Posted by: GrecoMan Posted at: 2017-12-30T13:26:08.608Z Reads: 109

```
my question is why are you buying a mech kit and throwing away the pulleys...

just buy the mounts and get belts and pulleys from @JLabs and eskating.eu
```

---
## \#281 Posted by: Sirshaunsta Posted at: 2017-12-30T13:26:13.917Z Reads: 121

```
<img src="/uploads/db1493/original/3X/7/e/7ed50dc597e36de6cab3a13a95f38c5d4c146e20.png" width="281" height="500">
```

---
## \#282 Posted by: Sirshaunsta Posted at: 2017-12-30T13:27:01.313Z Reads: 105

```
Actually that sounds like a much simpler idea and save me some cash
```

---
## \#283 Posted by: Sirshaunsta Posted at: 2017-12-30T13:30:14.665Z Reads: 108

```
Now in your experience would dropping 2 or 4 teeth mean I should get a smaller belt or should i not worry about that unless I take off like 6? @GrecoMan
```

---
## \#284 Posted by: GrecoMan Posted at: 2017-12-30T13:39:58.591Z Reads: 107

```
I use the same belts for 12/36 and 16/36.
```

---
## \#285 Posted by: Sirshaunsta Posted at: 2017-12-30T13:42:51.619Z Reads: 102

```
I'm so glad there's people like you on here to help me out, can't wait till it's my turn @GrecoMan
```

---
## \#286 Posted by: Sirshaunsta Posted at: 2017-12-30T14:17:19.794Z Reads: 107

```
Ohh got another brain teaser here @GrecoMan my calc says 42% but i dont know if that means for single or dual drive, also by adding motors would that limit double or go up by half? Whats the math there?
```

---
## \#287 Posted by: Sirshaunsta Posted at: 2017-12-30T14:19:45.257Z Reads: 106

```
http://calc.esk8.today/advanced/ that's what I've been using with 190 kv at 10s 2p 18/32 97mm wheels 80kg rider and 20kg board just to be safe if I carry a bag sometimes but we both know I actually have 8p I'm just splitting it between 4 motors @GrecoMan
```

---
## \#288 Posted by: Sirshaunsta Posted at: 2017-12-31T05:37:33.171Z Reads: 100

```
Eh dude? Yourself or anyone got some help here? @E1Allen @GrecoMan @PredatorBoards @Cobber @psychotiller
```

---
## \#289 Posted by: E1Allen Posted at: 2017-12-31T05:39:55.646Z Reads: 104

```
What's the 42%?
```

---
## \#290 Posted by: psychotiller Posted at: 2017-12-31T05:47:39.497Z Reads: 114

```
Whenever you change your gearing:

Dropping a tooth (a tooth in 5mm htd is 5mm of space.) You'll most likely need a belt that is 5mm smaller. a 285belt will need to be a 280

Raising a tooth would be reverse 285 would need to be 290

If you have 3m htd the increments will be 3mm.

Not sure what your 42% means....
```

---
## \#291 Posted by: E1Allen Posted at: 2017-12-31T05:53:43.665Z Reads: 116

```
I think it's the hill climb grade. I just checked it's the only thing with percent. since the calculator doesn't list number of motors I would guess it's one.  Either way with your board at that gearing I doubt there is a hill you couldn't climb.
```

---
## \#292 Posted by: Sirshaunsta Posted at: 2017-12-31T06:05:53.484Z Reads: 112

```
Ok guys and yes 42 % hill grade max per motor and 70km-ish top speed
```

---
## \#293 Posted by: Sirshaunsta Posted at: 2017-12-31T06:06:58.157Z Reads: 113

```
Thank you , so if I were using a 18 32 setup instead of 1636 id need a belt 10mm shorter than the 1636?
```

---
## \#294 Posted by: psychotiller Posted at: 2017-12-31T06:18:35.428Z Reads: 109

```
Most likely yes
```

---
## \#295 Posted by: Sirshaunsta Posted at: 2017-12-31T06:20:35.616Z Reads: 105

```
Ok, the site says they use a 265 for 1636 on diy mounts, so I'll order 255mm, shorter belt means more torque and less slip as well from what I've learned, correct?
```

---
## \#296 Posted by: psychotiller Posted at: 2017-12-31T06:23:43.632Z Reads: 108

```
Gearing is the only thing that affects torque. Belt length isn't a factor. 16/36 would be torquier than 18/32
```

---
## \#297 Posted by: Sirshaunsta Posted at: 2017-12-31T07:24:03.158Z Reads: 105

```
Yes I agree 2.25-1 is more torque than 1.78-1 but I read and I can't remember where that a shorter belt was better. @psychotiller
```

---
## \#298 Posted by: Cobber Posted at: 2017-12-31T07:52:31.817Z Reads: 114

```
sorry dude, crazy times...
a longer belt can actually be better if it means you have more teeth in mesh...
lets consider that "best" is more complicated than any one thing ;)

i'll drop a longer post next week dude
```

---
## \#299 Posted by: Colson003 Posted at: 2017-12-31T07:56:15.508Z Reads: 110

```
Maybe a shorter belt is less likey to... "stretch" :wink:
```

---
## \#300 Posted by: Sirshaunsta Posted at: 2017-12-31T08:01:14.340Z Reads: 113

```
Like the only way a longer belts better is if I use tensioners on one or both sided of each mount to cradle the pulleys instead of just wrap over the outside... guess I just answered part of my question
```

---
## \#301 Posted by: E1Allen Posted at: 2017-12-31T18:22:37.543Z Reads: 130

```
@psychotiller is right. Gear ratio is what affects torque. <img src="/uploads/db1493/original/3X/c/5/c52d9f86f2f5006bd63eb28c4432f58f94ddb45f.JPG" width="375" height="500"><img src="/uploads/db1493/original/3X/e/2/e2d7ff147589313e4d07b05d1e39f16417f95294.JPG" width="375" height="500">

However, on setups built for high torque the drive system has to be capable of handling that torque. More teeth doesn't give you more torque.  More teeth will connected to the gears will give you access to that torque you have available.   Because belts are more flexible than say a chain when you demand more torque than the teeth can hold they skip over the teeth.  But you don't want to make the belt tight because that puts more stress on the bearings.  
But since you're on a monster quad build... Unless you're pulling a car I don't think you will be able to stand on the board if you do max acceleration from a standstill.
```

---
## \#302 Posted by: Sirshaunsta Posted at: 2017-12-31T19:53:46.537Z Reads: 119

```
Ok I'm loving these tips right now,  in a video I saw somebody explain how to set acceleration curve on vesc, at .010 for a really gradual start, should that be what I go for or should i use something even lower?
```

---
## \#303 Posted by: GrecoMan Posted at: 2017-12-31T20:01:12.889Z Reads: 112

```
keep it at .01.
```

---
## \#304 Posted by: Sirshaunsta Posted at: 2017-12-31T20:37:44.358Z Reads: 111

```
Ok thank you I will
```

---
## \#305 Posted by: Sirshaunsta Posted at: 2018-01-09T08:22:42.439Z Reads: 111

```
Well ... i got in contact with enertion... gonna take another fucking 2 or 3 weeks to send out the parts I orders OVER A MONTH AGO ... SO 5 OR 6 more weeks to receive my focboxs. I will NEVER order from them again
```

---
## \#306 Posted by: wmj259 Posted at: 2018-01-09T20:11:05.399Z Reads: 112

```
Enertion is currently making a business relocation event. Please be patient.
```

---
## \#307 Posted by: Sirshaunsta Posted at: 2018-01-10T04:20:18.730Z Reads: 113

```
I think I've been patient, I ordered 4 focbox... that's roughly 800 dollars I shelled out plus shipping costs(1000 total roughly). Relocating was their first excuse then when I asked later, their excuse is faulty parts... apparently they got a bad batch and while I like that they do qc and make sure to send out a good product, I think taking close to 2 full months just to send out those 4 items is absolutely ridiculous... @wmj259 i ordered them early so I could build the board over winter and have it ready for spring. Not start building in spring... if I knew it would take 3 months to get my parts ahead of time I wouldn't be so upset.
```

---
## \#308 Posted by: caustin Posted at: 2018-01-10T05:11:38.714Z Reads: 105

```
Did you order the focboxes on the Cyber Monday sale Enertion held?
```

---
## \#309 Posted by: hornet90 Posted at: 2018-01-10T06:19:38.534Z Reads: 104

```
If I was ordering parts from them I would give it 8 to 12 weeks...
```

---
## \#310 Posted by: Sirshaunsta Posted at: 2018-01-10T08:04:17.921Z Reads: 103

```
If the cyber Monday is when they drop to 200$ I ordered 2 then and 2 at regular price cause I didn't realize the sale was weekly or I would have waited to get the other 2
```

---
## \#311 Posted by: Sirshaunsta Posted at: 2018-01-10T08:04:48.715Z Reads: 105

```
That seems about right with what I've seen so far
```

---
## \#312 Posted by: Sirshaunsta Posted at: 2018-01-23T03:28:25.346Z Reads: 100

```
Hey guys, been a little while, I've been rattling some thoughts in my head and need some advice, I'm running 10s using 2 5s in series, now my amp ability of the battery is 200cont. , the 2 vesc that will be connected will each draw up to 120 a for burst and 60 cont. My batteries all have xt60 connectors though, which if I'm not mistaken can only tolerate a max cont. A of 60 before failing. Will this come into play if I end up drawing 120 a cont. By powering both vesc at the same time? Will my batteries and connectors be fine or do I need to replace the xt60s on my 5s to xt90s?
```

---
## \#313 Posted by: scepterr Posted at: 2018-01-23T03:30:44.571Z Reads: 100

```
You should definitely upgrade to xt90 at least
Even close to 60A using xt60 will generate heat and resistance
```

---
## \#314 Posted by: Sirshaunsta Posted at: 2018-01-23T03:32:23.712Z Reads: 95

```
Can I get anything higher like 120s? I've only seen 30 60 and 90 @scepterr
```

---
## \#315 Posted by: scepterr Posted at: 2018-01-23T03:33:20.115Z Reads: 92

```
Yep the AS150
```

---
## \#316 Posted by: Deckoz Posted at: 2018-01-23T03:33:38.072Z Reads: 92

```
I'm obviously reading old posts

But if you want different gearing. Do short gearing up front with one way bearings. And tall gears in the rear.

Problem solved.
```

---
## \#317 Posted by: Sirshaunsta Posted at: 2018-01-23T03:36:49.447Z Reads: 94

```
Does this mean I'll need new wiring or would I be able to just replace all my connectors?
```

---
## \#318 Posted by: scepterr Posted at: 2018-01-23T03:37:05.913Z Reads: 90

```
You can just replace
Assuming wire gauge is already thick enough, 10AWG atleast
```

---
## \#319 Posted by: Sirshaunsta Posted at: 2018-01-23T03:37:35.604Z Reads: 90

```
You're awesome, last question for ya, where would I buy the 150s?
```

---
## \#320 Posted by: scepterr Posted at: 2018-01-23T03:37:54.186Z Reads: 87

```
Amazon, Amazon everything 😉
```

---
## \#321 Posted by: Sirshaunsta Posted at: 2018-01-23T03:38:45.646Z Reads: 90

```
Ok perfect, And I'd be leaving the existing wire on batteries used for 60s, and my connectors are all xt90s (series and parrallel) @scepterr
```

---
## \#322 Posted by: scepterr Posted at: 2018-01-23T03:40:24.355Z Reads: 88

```
What wire gauge do you have coming from the battery now?
```

---
## \#323 Posted by: Sirshaunsta Posted at: 2018-01-23T03:42:06.098Z Reads: 99

```
These right?![Screenshot_20180122-224141|281x500](upload://642zGh44jPiHGBRXm9DGDW95ZNw.jpg)
```

---
## \#324 Posted by: Sirshaunsta Posted at: 2018-01-23T03:43:11.936Z Reads: 95

```
12awg good to 200degrees c
```

---
## \#325 Posted by: scepterr Posted at: 2018-01-23T03:43:39.167Z Reads: 91

```
Yeah but 12 isn't good for 100A+
It's like 85-90A max, 10AWG is 140A
```

---
## \#326 Posted by: Sirshaunsta Posted at: 2018-01-23T03:46:28.979Z Reads: 91

```
Yeah my connectors all have 10 awg but the batteries use 12
```

---
## \#327 Posted by: scepterr Posted at: 2018-01-23T03:47:00.809Z Reads: 86

```
Kinda defeats using all that 10 😋
```

---
## \#328 Posted by: Sirshaunsta Posted at: 2018-01-23T03:47:34.646Z Reads: 90

```
Now I will have 3 bundles in parallel made of 2 in series each, will that effect any of this? @scepterr yes 6 5s making 1 10s ;)
```

---
## \#329 Posted by: scepterr Posted at: 2018-01-23T03:49:34.555Z Reads: 88

```
No that's all fine, just make sure you're not losing power to heat in any connections
```

---
## \#330 Posted by: Sirshaunsta Posted at: 2018-01-23T03:50:25.899Z Reads: 90

```
So really I just have to test it out, see if I get any heat And go from there?
```

---
## \#331 Posted by: scepterr Posted at: 2018-01-23T03:51:47.779Z Reads: 90

```
Yeah, also look for voltage sag during high current load and check right after an extended high current run, like at the top of a hill
```

---
## \#332 Posted by: Sirshaunsta Posted at: 2018-01-23T03:51:59.522Z Reads: 84

```
I am tempted to add 10awg to my batteries but idk if I trust myself to soder to the lipo directly
```

---
## \#333 Posted by: scepterr Posted at: 2018-01-23T03:52:31.860Z Reads: 82

```
It's just if you have 12awg coming off the battery, there's no need to go above an xt90
```

---
## \#334 Posted by: Sirshaunsta Posted at: 2018-01-23T03:52:49.093Z Reads: 81

```
So check my meters to see if voltage drops while bursting speed?
```

---
## \#335 Posted by: scepterr Posted at: 2018-01-23T03:53:39.943Z Reads: 81

```
Better to log using Bluetooth and an app, you won't see it on meters

For this test you need to be pulling 90-100+A total battery to see impact
```

---
## \#336 Posted by: Sirshaunsta Posted at: 2018-01-23T03:55:58.281Z Reads: 78

```
Ok, so I would be able to sync my vesc to phone during ride to get specs?
```

---
## \#337 Posted by: scepterr Posted at: 2018-01-23T03:56:39.451Z Reads: 85

```
Yeah, and then be able to see full ride stats
```

---
## \#338 Posted by: Sirshaunsta Posted at: 2018-01-23T03:58:59.058Z Reads: 87

```
Thats sick, so how would i tell voltage sag from those stats? Or will it be kinda staring me right in the face and kinda hard to miss?
```

---
## \#339 Posted by: scepterr Posted at: 2018-01-23T04:00:03.582Z Reads: 88

```
The voltage drop would go from even to sharp under a consistent load in the chart
```

---
## \#340 Posted by: GrecoMan Posted at: 2018-01-23T04:01:25.324Z Reads: 84

```
I can get you a bluetooth module for $18 shipped 😉
```

---
## \#341 Posted by: Sirshaunsta Posted at: 2018-01-23T04:01:39.175Z Reads: 83

```
Ok ok so when I'm accelerating It should stay pretty consistent but if there's sag it will look significantly wit?
```

---
## \#342 Posted by: Sirshaunsta Posted at: 2018-01-23T04:02:26.478Z Reads: 79

```
And is that something I plug in to the board or is it a program?
```

---
## \#343 Posted by: GrecoMan Posted at: 2018-01-23T04:02:43.517Z Reads: 79

```
when your going at a constant speed it’ll look constant.

when you’re accelerating or braking the voltage will spike up or down accordingly
```

---
## \#344 Posted by: scepterr Posted at: 2018-01-23T04:02:56.462Z Reads: 81

```
Right the voltage should decrease but pretty steadily and without huge jumps down and up
```

---
## \#345 Posted by: GrecoMan Posted at: 2018-01-23T04:03:02.469Z Reads: 82

```
little module you plug into the vesc to connect to the phone
```

---
## \#346 Posted by: Sirshaunsta Posted at: 2018-01-23T04:04:39.435Z Reads: 79

```
How would it go up and down ? Isn't sag where you lose power quicker? I'm still fairly new here
```

---
## \#347 Posted by: Sirshaunsta Posted at: 2018-01-23T04:05:15.237Z Reads: 72

```
I will definitely be interested in that when I'm closer to finishing the build
```

---
## \#348 Posted by: scepterr Posted at: 2018-01-23T04:06:00.345Z Reads: 77

```
Sag is when the voltage drops because current is too high for a connection or the battery itself to handle which causes a slow down which decreases the current and allows the voltage to "jump up"
If the sag is severe enough it'll throw an overcurrent fault because at the moment the voltage drops the vescs try to compensate by pulling more current and usually at the point you have to stop
```

---
## \#349 Posted by: Sirshaunsta Posted at: 2018-01-23T04:08:18.540Z Reads: 75

```
Ooh k so it's like I'm pulling current pulling current but I'm pulling too much so I start pulling less and the difference shows the battery as having more power left to use?
```

---
## \#350 Posted by: scepterr Posted at: 2018-01-23T04:09:11.783Z Reads: 75

```
I'm not exactly clear on what you said there 🤔
```

---
## \#351 Posted by: Sirshaunsta Posted at: 2018-01-23T04:13:35.332Z Reads: 73

```
Nvm I had to re read your last. So it causes the voltage to increase instead of decrease as norm because the connection can't support the necessary amps needed so instead of big power normal current it's less power higher/faster current
```

---
## \#352 Posted by: scepterr Posted at: 2018-01-23T04:14:47.761Z Reads: 75

```
The other way, voltage decreases faster than its supposed to because current is too high
```

---
## \#353 Posted by: Sirshaunsta Posted at: 2018-01-23T04:17:05.796Z Reads: 76

```
But you said there could be jumps down and up? So the voltage goes down(speed of delivery) and amps go up(power delivered)? But the decline of v and incline of amp would be noticeably greater?
```

---
## \#354 Posted by: scepterr Posted at: 2018-01-23T04:19:53.425Z Reads: 74

```
Bingo 👍 .
.
```

---
## \#355 Posted by: Sirshaunsta Posted at: 2018-01-23T04:22:49.436Z Reads: 72

```
Ok I think I'm getting it, so would this occur when I'm cruising or only when I'm holding the throttle? Both?
```

---
## \#356 Posted by: scepterr Posted at: 2018-01-23T04:23:08.915Z Reads: 76

```
Only during sustained high current
```

---
## \#357 Posted by: Sirshaunsta Posted at: 2018-01-23T04:25:28.396Z Reads: 76

```
Ok but when drawing higher current wouldn't it deplete the battery faster than low current anyways? So this just means if I have sag that it will eat my battery faster than it should or just draw more amps than it should ?
```

---
## \#358 Posted by: scepterr Posted at: 2018-01-23T04:26:59.366Z Reads: 81

```
It's just drawing more amps than it should and yes technically decrease range because you would be losing energy in heat at the physical cause of the sag, whether it be a wire, connector, solder joint or the battery itself
```

---
## \#359 Posted by: Sirshaunsta Posted at: 2018-01-23T04:29:50.955Z Reads: 75

```
Ok, then I think upgrading all my wires(battery and connectors) might be a good investment.  I'm running 4 motors so I shouldn't be drawing too many amps to push my 155lbs but I'd rather be safe than sorry when I've spent roughly 4g on the build so far
```

---
## \#360 Posted by: scepterr Posted at: 2018-01-23T04:31:32.111Z Reads: 73

```
Right you can get away with not drawing a lot but you can also do like 35mph+ going uphill which would draw plenty of current 😉
```

---
## \#361 Posted by: Sirshaunsta Posted at: 2018-01-23T04:31:50.418Z Reads: 73

```
Like I seen most people drawing 30 and 40 amps for cont. High current on duals so I figure probably 15 to 30 amps per motor adding to max of 60 ish per battery as I'm running 2 10s batteries
```

---
## \#362 Posted by: scepterr Posted at: 2018-01-23T04:32:54.833Z Reads: 71

```
Yeah you really have to intend to use high current to use high current...if that makes sense...lol
Under most conditions an appropriate setup won't need to draw crazy amps
```

---
## \#363 Posted by: Sirshaunsta Posted at: 2018-01-23T04:34:30.505Z Reads: 68

```
Thats what I was hoping for, I'm using 4 sk3 190s and 12 possibly 16 5s 5ah batteries  so I'll have plenty of torque so no power loss there pushing me up hills, I just don't want to run into heat problems when I'm hitting 40mph with my gearing setup of 18/32
```

---
## \#364 Posted by: Sirshaunsta Posted at: 2018-01-23T04:38:30.674Z Reads: 68

```
So thats 2 10s 15 or 20ah batteries each powering 2 focbox and 2 sk3 190 @scepterr
```

---
## \#365 Posted by: scepterr Posted at: 2018-01-23T04:40:31.196Z Reads: 72

```
Definitely go 10AWG if you want to take advantage of all that 😉
```

---
## \#366 Posted by: Sirshaunsta Posted at: 2018-01-23T04:42:12.418Z Reads: 77

```
Then I only need to change my battery wires, I just REALLY HOPE I don't fuck the batteries up @scepterr
```

---
## \#367 Posted by: Sirshaunsta Posted at: 2018-01-23T04:44:06.171Z Reads: 78

```
So given what you know now about my build would you say the xt90s will be sufficient for  everything or should i still bump up to 150s? With the 10awg @scepterr
```

---
## \#368 Posted by: scepterr Posted at: 2018-01-23T04:45:55.698Z Reads: 83

```
If you're powering each pair of vescs independently than xt90 to each pair will be fine, if all 4 are drawing from a single source then AS150
```

---
## \#369 Posted by: Sirshaunsta Posted at: 2018-01-23T04:46:51.078Z Reads: 87

```
That was exactly my plan was 1 power source to each end of the board. 1 batt to 2 vesc
```

---
## \#370 Posted by: Sirshaunsta Posted at: 2018-01-23T04:49:38.240Z Reads: 89

```
I'll still see about switching to 10awg on batteries though , thanks alot for your help @scepterr
```

---
## \#371 Posted by: Sirshaunsta Posted at: 2018-01-23T05:53:07.396Z Reads: 89

```
Can anybody tell me why I have so much slide on my trucks here? They're the 218mm from diy. And these are 97mm flywheel I have a spacer and bones ceramic bearings so I don't know why there's so much play?![1516686686025739193566|374x500](upload://h2fPwGSDpVkSEuPk7CTuSEijtkr.jpg)![15166867130731128425490|374x500](upload://dgQaIkGcPG4f2JxK538SmYaJfsK.jpg)  ![1516686587690331543091|374x500](upload://hxzOCuCkBN6pmNFb0t1Ypt14vtp.jpg)
```

---
## \#372 Posted by: scepterr Posted at: 2018-01-23T05:53:48.839Z Reads: 85

```
Lol you need a lot more spacers
```

---
## \#373 Posted by: Sirshaunsta Posted at: 2018-01-23T05:54:43.827Z Reads: 84

```
So I'm supposed to put spacers between my wheel and the hangar?
```

---
## \#374 Posted by: scepterr Posted at: 2018-01-23T05:55:30.246Z Reads: 90

```
Yep, if you have more wheel bearing spacers that'll work
![IMG_20180123_005556|666x499](upload://f8Rect0HocWR3HVqa2s1jqpmLar.jpg)
![IMG_20180123_005609|666x499](upload://x4YtRHqrk7T4PvBV2lpR5pEq2GX.jpg)
```

---
## \#375 Posted by: Sirshaunsta Posted at: 2018-01-23T05:58:56.247Z Reads: 93

```
I do actually, so like this?![1516686974165924229015|374x500](upload://yV0NT5bPp7bo8arbFmeP1rzlGCK.jpg)![1516687033762354884844|374x500](upload://5lBhQGVTW7EA9st2S6z1kQUhUeV.jpg)
```

---
## \#376 Posted by: scepterr Posted at: 2018-01-23T05:59:54.671Z Reads: 87

```
Yeah you just need more on the nut side or maybe not if you tighten the nut
```

---
## \#377 Posted by: Sirshaunsta Posted at: 2018-01-23T06:00:53.480Z Reads: 87

```
Yeah, I don't want my bearings riding on threads, I'll have to grab my other 4 spacers or a bunch of washers, SHIT I forgot I threw out my old spacers... oh no I found some more new ones
```

---
## \#378 Posted by: Sirshaunsta Posted at: 2018-01-23T06:04:01.180Z Reads: 86

```
But that doesn't work, will everything work just as good if I take out the 2 washers and just use a spacer on each side? @scepterr
```

---
## \#379 Posted by: scepterr Posted at: 2018-01-23T06:05:14.361Z Reads: 90

```
It'll work however you fill the gap, spacer,washer just needs to take up space
```

---
## \#380 Posted by: Sirshaunsta Posted at: 2018-01-23T06:07:19.815Z Reads: 96

```
Nvm 2 spacers is too much ![15166875863821511316980|374x500](upload://6Fo8lymg3gana43LleSVYNOv2yF.jpg)
```

---
## \#381 Posted by: scepterr Posted at: 2018-01-23T06:08:27.668Z Reads: 90

```
Can you cut one in half?
```

---
## \#382 Posted by: Sirshaunsta Posted at: 2018-01-23T06:16:31.108Z Reads: 94

```
Possibly if I take it to work as I work in a shop that works strictly with aluminium, but idk if we have anything to handle such a small piece and still be precise. @scepterr
```

---
## \#383 Posted by: Sirshaunsta Posted at: 2018-01-23T06:20:24.925Z Reads: 102

```
Little update of how the board is looking, need 4 more batteries, drive system, motor mounts. Focbox and rest of wiring is on way already in mail.![15166882837091854911666|374x500](upload://roCdokTeokJh6knPx7zscUih0D3.jpg)![15166883854242026489234|374x500](upload://36lYQBXCiTiNl7HOp0fNJAqBbIS.jpg)
```

---
## \#384 Posted by: Sirshaunsta Posted at: 2018-01-25T18:09:00.113Z Reads: 92

```
So I just did some thinking, if I go from 2 separate batteries of 10s20ah to 4 10s10ah batteries I should eliminate our wire issue and save alot of work, because the 5s5ah batts can handle 92.5a so can the wire, having the draw split by a y cable I can output up to 185a from xt60s(battery) to the xt90 and the vesc. Drawing from both batteries in parallel should mean I halve the draw from each right? So if my motor is demanding 120a for a burst it's 60 from each cell which is the max of the connectors limit (used only on bursts) and for continued draw of up to 50a per motor I will only draw 25a per Battery. So I will stay well supported and have very little to no heat /energy loss or v-sag. My only wonder is would this lower my range or leave it the same, in theory I have the same amount of batteries but the calc I use says a single battery bank gives long range aposed to 4 separate smaller ones even if the v and ah are the same. You got any ideas @GrecoMan also I can set a max amp input of 100 on the vesc right? So it would never draw more than 50a from each battery cell?
```

---
## \#385 Posted by: wmj259 Posted at: 2018-01-25T18:19:46.463Z Reads: 88

```
That is a lot of Series adapters.
```

---
## \#386 Posted by: Sirshaunsta Posted at: 2018-01-25T18:51:16.593Z Reads: 92

```
16 5s5a batteries, 4 to each motor @wmj259 so really only 3 on each pack/motor. 2 series and one parallel
```

---
## \#387 Posted by: Sirshaunsta Posted at: 2018-01-25T21:13:42.606Z Reads: 92

```
I'm figuring at sustained high speeds I'll only draw somewhere between 15 and 25 amps  per motor
```

---
## \#388 Posted by: pat.speed Posted at: 2018-01-25T22:12:27.693Z Reads: 90

```
Plz be careful connecting all those batteries with that harness, one wrong connection and you'll have yourself a bigger bomb than Kim Jong Un
```

---
## \#389 Posted by: Sirshaunsta Posted at: 2018-01-25T22:31:42.220Z Reads: 90

```
I know, it's a bit nerve racking but If all works well I'll have one of the most powerful boards made(at least that I've seen) @pat.speed
```

---
## \#390 Posted by: pat.speed Posted at: 2018-01-25T22:39:40.532Z Reads: 84

```
Have you bought balance lead adapters yet? And are you going to use a bms or hobbycharger
```

---
## \#391 Posted by: Sirshaunsta Posted at: 2018-01-25T22:41:12.534Z Reads: 86

```
Balance leads? So I need harness for the white blocks on my batteries to go to vesc too? And hobby balance charger no bms. But running 10s or 37.5v at 45 amp continuous if be almost 7000w
```

---
## \#392 Posted by: pat.speed Posted at: 2018-01-25T22:42:01.307Z Reads: 88

```
No to go to the bms or charger
```

---
## \#393 Posted by: Sirshaunsta Posted at: 2018-01-25T22:43:00.067Z Reads: 91

```
If you scroll up you'll see I bought multiple balance chargers with split boards so I can balance charge up to 18 batteries at once. I'll only be charging 16 tho @pat.speed
```

---
## \#394 Posted by: Sirshaunsta Posted at: 2018-01-25T22:44:27.359Z Reads: 95

```
![15169202190571993845159|374x500](upload://vmX2XpsTEkRcLOY4BPVffyfrEla.jpg) ×3
```

---
## \#395 Posted by: pat.speed Posted at: 2018-01-25T22:45:16.096Z Reads: 90

```
Ahhh ok sorry I missed that
```

---
## \#396 Posted by: Sirshaunsta Posted at: 2018-01-25T22:46:22.871Z Reads: 87

```
No worries dude
```

---
## \#397 Posted by: BoostedBuilder Posted at: 2018-01-25T22:50:47.595Z Reads: 88

```
Man, I'm really interested, why do you have bearings that are more expensive than your wheels? If you can afford ceramics, why not go ABEC11 route with wheels?
```

---
## \#398 Posted by: Sirshaunsta Posted at: 2018-01-25T22:50:50.005Z Reads: 87

```
But yeah I have a potential of 9750w but that's drawing 65 amps per motor at 37.5v which I'll never do. Well except on bursts ;)
```

---
## \#399 Posted by: Sirshaunsta Posted at: 2018-01-25T22:51:27.729Z Reads: 84

```
All the abecs were out of stock I'm still hoping to find some 107mms those are simple 97mm from Amazon I think
```

---
## \#400 Posted by: BoostedBuilder Posted at: 2018-01-25T22:54:31.655Z Reads: 80

```
I got you bro:  [107's](https://www.muirskate.com/longboard/wheels/72661/107mm-abec-11-super-fly-longboard-skateboard-wheels) and [97's](https://www.muirskate.com/longboard/wheels/2166/97mm-abec-11-flywheels-wheels)
```

---
## \#401 Posted by: Sirshaunsta Posted at: 2018-01-25T22:55:39.774Z Reads: 82

```
I fucking love you right now dude @BoostedBuilder
```

---
## \#402 Posted by: BoostedBuilder Posted at: 2018-01-25T22:58:06.431Z Reads: 81

```
Enjoy them : )
Just don't kill yourself, please! Your build looks crazy!
```

---
## \#403 Posted by: Sirshaunsta Posted at: 2018-01-25T23:01:44.601Z Reads: 81

```
With those at an 18 34 gearing I'd hit 67 kmph and have a hill gradient of 42% on each motor (I have 4) so I'll have shit tonnes of torque and never a problem with hills @BoostedBuilder at full battery over 72 kmh/45mh
```

---
## \#404 Posted by: Bor.inc Posted at: 2018-01-25T23:07:28.228Z Reads: 80

```
Im so interested in this project, how is the progress? when do you think it is working?
```

---
## \#405 Posted by: Sirshaunsta Posted at: 2018-01-25T23:13:15.505Z Reads: 84

```
I am in the assembly stage still for now unfortunately, but i am hoping for between April and May to be finished, only because of extensive shipping wait times. So far as you can see if you scroll through, I have 4/4 motors 12/16 batteries 2/2recievers 2/4 voltmeter 4/4antispark 3/3multi-balance chargers 1/1extended trucks 1/1 remote. So I'm waiting for 4/4 focbox 4/16 batteries 4/4motormounts 4/4 belts 4/4 wheel and motor pulleys as well as some more in series and parallel xt90 adaptors. @Bor.inc once I receive the rest of my items it's really a matter of maybe 30 minutes
```

---
## \#406 Posted by: Sirshaunsta Posted at: 2018-01-25T23:16:55.930Z Reads: 83

```
@Bor.inc  I currently have 2 sets of bones ceramic bearings and 1 set of 97mm fly wheels but I'm very soon grabbing 107s thanks to @BoostedBuilder though I will prolly kick myself for spending 200+ Canadian on 4 wheels for 10 extra mm it's really not much in contrast to the overall cost of this build ;P I did just find another store carrying them for 177 Canadian tho so I might just keep looking and see if they drop in price over time
```

---
## \#407 Posted by: lrdesigns Posted at: 2018-01-26T00:41:31.730Z Reads: 84

```
[quote="Sirshaunsta, post:375, topic:39765"]
I do actually, so like this?
[/quote]

Just make sure the **thread of the axle comes past the end of the nut**, or it could come off while ridding. Its happened to me before. :scream: luckily only a rear wheel and just grinded to a stop. 

On mine the nut had many on/off cycles and the nylock part was worn out. 

The axles are extra long so you can run many different setups, gives flexibility of wheel / pulley / alignment.

You can use an old bearing as a spacer in a pinch.
```

---
## \#408 Posted by: Sirshaunsta Posted at: 2018-01-26T00:48:11.723Z Reads: 87

```
I've ended up doing this ![1516927426223988078851|374x500](upload://oiFjVgiSFAVpwAOYI36xHzjfCyY.jpg)![15169274693402128376926|374x500](upload://7GqUXtbI6L7Ry6Groj673cLTUDP.jpg) added a spacer and 3 washers to inside of hanger before wheel and 1 washer to outside to give me the maximum wheel base distance(handling) so the threads literally start in line with the end of my bearings and then the washer and nut secure it all, the bearings are completely on flat smooth hangar and at the furthest possible point of the trucks @lrdesigns
```

---
## \#409 Posted by: Sirshaunsta Posted at: 2018-01-26T00:50:24.164Z Reads: 88

```
I literally have 8.5 inches between each wheel![15169277942891033758699|374x500](upload://s6pheDatUv7IIzeJvvfrYdp8XUN.jpg) @lrdesigns
```

---
## \#410 Posted by: Sirshaunsta Posted at: 2018-01-27T01:10:51.592Z Reads: 89

```
Can anyone tell me why focbox has xt60 connectors? Shouldn't they have xt90?![1517015406040555671621|374x500](upload://jaoGqWP5amuqLFk9SfbwKaKQiT6.jpg)![15170153570291958974845|374x500](upload://bwK9MU0fO4tyThvyWUwEO1jCaHn.jpg)
```

---
## \#411 Posted by: Sirshaunsta Posted at: 2018-01-27T01:13:14.170Z Reads: 85

```
Would it be very hard for me to replace the 12awg and xt60 with 10awg xt90?
```

---
## \#412 Posted by: louwii Posted at: 2018-01-27T01:32:00.907Z Reads: 88

```
I think you can keep 12AWG and just replace the XT90.
I build my board with 12AWG only and XT90s.
```

---
## \#413 Posted by: Sirshaunsta Posted at: 2018-01-27T02:18:05.112Z Reads: 84

```
Yes but are you running 10s? @louwii
```

---
## \#414 Posted by: louwii Posted at: 2018-01-27T02:20:56.756Z Reads: 89

```
I am, yes.
I believe 12AWG is fine for 12S too (I think Focboxes wouldn't come with it otherwise). 10AWG would be safer for sure.
```

---
## \#415 Posted by: Sirshaunsta Posted at: 2018-01-27T02:46:04.167Z Reads: 86

```
So 12 awg and xt60 can actually handle loads of 42v and 120amp bursts? And up to 60 amps constant draw? @louwii
```

---
## \#416 Posted by: louwii Posted at: 2018-01-27T02:57:29.574Z Reads: 83

```
42V at 60A is 2520W, that's not something you will have to handle constantly, especially if the load is split in 4 different motors.
```

---
## \#417 Posted by: Sirshaunsta Posted at: 2018-01-27T03:02:58.526Z Reads: 81

```
True and my motors are only rated to 2450watt each so more like 42 and 55amp but still is that really able to be handled by 12 awg and xt60s?
```

---
## \#418 Posted by: louwii Posted at: 2018-01-27T03:14:23.351Z Reads: 82

```
Yes.
XT60 are rated for 60 amps

Found a voltage drop calculator there for wiring, you'll see that it's almost nothing for 12AWG at 48V 60A for 20cm of wire.
https://www.powerstream.com/Wire_Size.htm

Given the short wires we're dealing with on an esk8, 12AWG is fine.
```

---
## \#419 Posted by: Sirshaunsta Posted at: 2018-01-27T03:53:47.201Z Reads: 82

```
But the short times it goes over 60 for takeoff as an example, that won't chance ruining anything? Even with possible 120amp draw (hard accelerating from stop up a steep incline
```

---
## \#420 Posted by: Sirshaunsta Posted at: 2018-01-27T03:55:47.994Z Reads: 83

```
That link says max amp for 12 gauge is 41 amps
```

---
## \#421 Posted by: louwii Posted at: 2018-01-27T04:01:55.971Z Reads: 84

```
That applies to whatever that company is making and how long their wires are.

If you feel safer using 10AWG, you should probably use that then. You'll be the one riding your board, if you feel reassured with 10AWG, then use 10AWG :slight_smile: I don't want you fear that your board will catch fire because of 12AWG wires ;)
And 10AWG is fine with XT90.
```

---
## \#422 Posted by: Sirshaunsta Posted at: 2018-01-27T04:06:04.906Z Reads: 76

```
I think that's what I'll do, gonna be fun. I see differing xt90 vids but none of 10awg to focbox, maybe I'll be the first
```

---
## \#423 Posted by: Sirshaunsta Posted at: 2018-01-27T04:07:24.269Z Reads: 76

```
That's an American site tho dude are you sure the unit isn't inches?
```

---
## \#424 Posted by: louwii Posted at: 2018-01-27T04:10:06.847Z Reads: 76

```
For the calculator ? It's in feet, I put 0.6 feet which is roughly 20cm
```

---
## \#425 Posted by: E1Allen Posted at: 2018-01-27T04:17:33.774Z Reads: 82

```
Why are you changing out the xt60 on FocBox ?only to make it easier if you are running all xt90.?
```

---
## \#426 Posted by: Sirshaunsta Posted at: 2018-01-27T04:51:07.382Z Reads: 84

```
Because I already bought the xt90s why would I throw them away and but a bunch of 60s when I can buy 4 90s @E1Allen
```

---
## \#427 Posted by: Sirshaunsta Posted at: 2018-01-27T04:52:40.769Z Reads: 85

```
Now what if my batteries are in the middle of my board and need to transfer the power a total of just over 1 foot to reach vesc because of series and parallel adaptors +battery placement
```

---
## \#428 Posted by: E1Allen Posted at: 2018-01-27T06:11:08.514Z Reads: 89

```
I used five feet of cable between battery and vesc while I was testing with the wattmeter in between. I think you will be alright
```

---
## \#429 Posted by: Sirshaunsta Posted at: 2018-02-12T10:18:49.096Z Reads: 85

```
Well I've decided to just re order my battery harness using xt60s . Makes sense when the max I'll ever pull is 60amps per motor and will save weight size and a headache seeing as I'm making 4 harness's
```

---
## \#430 Posted by: GrecoMan Posted at: 2018-02-12T14:29:01.754Z Reads: 83

```
solder as much as humanly possible, connectors are no bueno
```

---
## \#431 Posted by: Stielz Posted at: 2018-09-06T04:06:01.773Z Reads: 53

```
What a  beast, how did this work out?
```

---
## \#432 Posted by: B_in_tha_OZ Posted at: 2019-04-05T06:58:55.677Z Reads: 19

```
I’m interested to see how this board worked out as well. Did it ever get finished? Hopefully you didn’t wipe out on the first test ride
```

---
