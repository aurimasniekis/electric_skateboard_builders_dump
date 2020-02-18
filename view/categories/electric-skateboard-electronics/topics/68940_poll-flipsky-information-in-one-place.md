# POLL: Flipsky information in one place

### Replies: 183 Views: 5641

## \#1 Posted by: brenternet Posted at: 2018-09-23T10:53:42.596Z Reads: 547

```
It's evident now that a significant amount of people have bought items from Flipsky and we've had some great communication from both users here, unofficial representatives and Flipsky themselves on how things are going but it's all quite spread out at the moment and lots of people using this stuff have not reported anything at all because they are just out riding with working parts. 

Let's collate and see how it's going? Vote on what you bought and how it went, explain in a reply if you don't mind but a vote will do to get an overall impression.

A quick note on this. It's clear that Flipsky give a damn about our feedback and are working on parts we actually need, filling the middle ground in cost. The point of this post is not to rip into them if issues are common, it's to help them improve the product. We all want cheap, well built parts don't we?

**4.20 DUAL**
[poll name=poll1 type=regular public=true]
* Working well on FOC
* Working well on BDLC
* Had problems with 11s 12s 13s 
* Dead on arrival or early issues
[/poll]

**4.20 SINGLE**
[poll name=poll2 type=regular public=true]
* Working well on FOC
* Working well on BDLC
* Had problems with 11s 12s 13s 
* Dead on arrival or early issues
[/poll]

**4.20 MINI**
[poll name=poll3 type=regular public=true]
* Working well on FOC
* Working well on BDLC
* Had problems with 11s 12s 13s 
* Dead on arrival or early issues
[/poll]

**6.6 DUAL**
[poll name=poll4 type=regular public=true]
* Working well on FOC
* Working well on BDLC
* Had problems with 11s 12s 13s 
* Dead on arrival or early issues
[/poll]

**6.6 SINGLE**
[poll name=poll5 type=regular public=true]
* Working well on FOC
* Working well on BDLC
* Had problems with 11s 12s 13s 
* Dead on arrival or early issues
[/poll]

**MOTORS**
[poll name=poll6 type=regular public=true]
* Working well
* Loose magnets
* Solder balls inside can
* Vibrations or loud noise under load
* Dead on arrival or other problems
[/poll]
```

---
## \#2 Posted by: Wraith Posted at: 2018-09-23T11:41:50.302Z Reads: 456

```
Maybe it may be worth adding in the versions with and without heatsink and the alu case as well for the 6.6 single vescs?
```

---
## \#3 Posted by: Octave Posted at: 2018-09-23T11:51:24.859Z Reads: 440

```
Maybe add the 4.12 version and their anti spark to get all their products.
```

---
## \#4 Posted by: martijntje42 Posted at: 2018-09-23T12:13:12.327Z Reads: 428

```
getting in some motors and an anti spark tomorrow, and 2 vesc 4.12 later this week. I will open everything up and take a look.
```

---
## \#5 Posted by: Benjamin899 Posted at: 2018-09-23T12:19:44.915Z Reads: 404

```
4.20 is the mini, i think you mean 4.12 single insead of 4.20 single.
```

---
## \#6 Posted by: brenternet Posted at: 2018-09-23T12:20:24.336Z Reads: 380

```
Yeah you're right but I can't edit the poll after it has begun. I'll ask a mod for help later when I'm back at my pc
```

---
## \#7 Posted by: Lumaci Posted at: 2018-09-23T12:33:51.697Z Reads: 375

```
I would also sort it out so its their 6354 and their 6374 since it seems like there has only been talked about problems on the 6374.
```

---
## \#8 Posted by: Riako Posted at: 2018-09-23T12:35:50.931Z Reads: 362

```
Thanks, good idea this thread!

I haven't the answer I want for 4.20 Mini and dual
(working on smooth flat ride 10s bldc, but when I push to much the trigger uphill I got OVER CURRENT and over intensity when braking, I will try if FOC is better now)...

(my click on mini is an error !) :sweat_smile:
```

---
## \#9 Posted by: Jasonkimberson Posted at: 2018-09-23T16:12:56.811Z Reads: 352

```
great thread, would be cool to see more results
```

---
## \#10 Posted by: mmaner Posted at: 2018-09-23T16:18:18.332Z Reads: 358

```
I'm currently testing the FlioSky Dual FSESC 4.2 with a 10s4p 30q battery pack using the following config. 

Motor Current Max: 30A
Motor Current Max Brake: -30A
Battery Current Max: 50A
Battery Current Max Regen: -40A

I'm still trying some stuff out with the config and gearing, but so far I'm impressed. 27mph max at this point, which is the limit if my current gearing.

_Edit: added battery pack to description_
```

---
## \#11 Posted by: brenternet Posted at: 2018-09-23T16:20:52.963Z Reads: 340

```
Is that on 10s Mike?
```

---
## \#12 Posted by: mmaner Posted at: 2018-09-23T16:21:16.453Z Reads: 334

```
Yes sir, 10s4p 30q pack.  Added that to my initial post.
```

---
## \#13 Posted by: BruSkater Posted at: 2018-09-23T16:40:03.323Z Reads: 327

```
FOC or BLDC? I don't know much of esc conffig, but isn't the batt regen too high for liion?
```

---
## \#14 Posted by: mmaner Posted at: 2018-09-23T16:43:36.428Z Reads: 329

```
BLDC, I'll try FOC after I run through all the options on BLDC. 

[quote="BruSkater, post:13, topic:68940"]
isn’t the batt regen too high for liion?
[/quote]

Not to my knowledge, 20a per group, 4 groups in parallel.  I'm using half of that.
```

---
## \#15 Posted by: Benjamin899 Posted at: 2018-09-23T16:46:49.737Z Reads: 319

```
Liion doesnt equal liion. 30q actually can take 4A continous and they can handle a short burst, safety>battery.
```

---
## \#16 Posted by: BruSkater Posted at: 2018-09-23T16:52:07.689Z Reads: 319

```
Then shouldn't max regen be set at 16?
```

---
## \#17 Posted by: Hummie Posted at: 2018-09-23T17:01:56.949Z Reads: 322

```
If u follow the peak continuous charge rate as ur guide yes  but we do a lot of “burst” braking
```

---
## \#18 Posted by: Riako Posted at: 2018-09-23T20:58:45.621Z Reads: 323

```
thanks for your parameters Mike !
I don't know why ... I don't try putting more on batt than motor amps get ...
I will try this too !!.. Maybe it will help mine.
```

---
## \#19 Posted by: Benjamin899 Posted at: 2018-09-23T21:29:03.211Z Reads: 321

```
careful with battery current. depends if your battery can derliver it without taking damage.
```

---
## \#20 Posted by: Riako Posted at: 2018-09-23T21:38:35.423Z Reads: 318

```
;) yes, thanks Ben, well point !
It should > 10s 5Ah 45C Graphene (extra small, compact and powerfull, was runing them on my light setup mtb last summer)
```

---
## \#21 Posted by: brenternet Posted at: 2018-09-25T06:44:33.074Z Reads: 294

```
My 4.20 dual arrives today. I should get it all plumbed in and get time on it this afternoon
```

---
## \#22 Posted by: dareno Posted at: 2018-09-25T07:49:48.838Z Reads: 296

```
This is dependent on the motors you're using really and I expect those settings are split between two motors.
```

---
## \#23 Posted by: Riako Posted at: 2018-09-25T13:36:28.272Z Reads: 308

```
Just try with 30A batt max on the Dual4.20, keeping all my motor parameter at 20A.
Trying full throttle a bit uphill but all of that at low speed regarding all the issues already happened... 
No faults here, I pull full trigger most time, accelerate braking etc 
Just made a short record ride at lunch break, this is with the new setup : 
https://metr.at/r/IUwr5
 20A Motor Max -20A Motor min 30 Amps Batt Max -15A Batt min 10s bldc sensoreless (little dual 5065 140kv)
old setup : 
https://metr.at/r/3VaFV
will do a longuer ride tonight, and at the end pushing a bit more.
:v:

Edit: looking to the end of the new test (1st metr window) got the same reccord has when I got faults Over Intensity when braking hard in long downhill ... Now I go more easy on the brake but it -35A motor current and just after that +56A !? And Im downhill trying to stop me front of home so Im not re-accelerating here ...

Plus I can see 56.4 max motor current with a setup at +20A/motor for motor max, ?
```

---
## \#24 Posted by: mmaner Posted at: 2018-09-25T13:40:12.084Z Reads: 281

```
I have found that 30 motor amps and 50 battery amps is the magic spot.  speed, torque...all is reasonably responsive.  I wouldn't put these in a racing board, but for an inexpensive mid-range VESC these are the way to go.
```

---
## \#25 Posted by: Riako Posted at: 2018-09-25T13:50:37.345Z Reads: 283

```
Cool Mike ! Still in bldc ? 
Yes, true that it could handle cool cruise ride, but I'm a bit skeptic when you suddenly need more and play hard with the throttle, I'm sure I could if I would make faults still happened but knowing this ... I will ride it like a cruise board. 
Hope the next version will be perfect, even if it's not 12s, but we need it perfectly safe and handle at list 30A perfectly :innocent:

So, I'm still trying to figure at what will be the good parameter and safe parameter here with better torque, for my board setup ?
Tonight I will make it at 30 motor max and 35 batt max (as my motor are rated for 34 amps).
And after my classic 5km test ring around the house I will try to set all FOC ...
```

---
## \#26 Posted by: mmaner Posted at: 2018-09-25T13:56:22.394Z Reads: 277

```
Yeah, still in BLDC.  Im having some issues getting a good FOC detection but I think its my motors.  Im going to try it in another deck with known goof FOC detections and see what happens.
```

---
## \#27 Posted by: Blasto Posted at: 2018-09-25T14:58:47.224Z Reads: 273

```
[quote="mmaner, post:24, topic:68940, full:true"]
I have found that 30 motor amps and 50 battery amps is the magic spot. speed, torque…all is reasonably responsive. I wouldn’t put these in a racing board, but for an inexpensive mid-range VESC these are the way to go.
[/quote]

I don't understand how bad hardware design can be justified by using sub-par settings. There's obviously a problem, using low settings is only masking the issue.
```

---
## \#28 Posted by: mmaner Posted at: 2018-09-25T15:00:16.674Z Reads: 265

```
I dont think its a bad hardware design.  It was designed to be a mid-level speed controller, it does that well.  Its better than the eBay/Chinese proprietary ESC's by a lot, yet cheaper than dual FocBox's.  I don't see what your issue is.
```

---
## \#29 Posted by: DAddYE Posted at: 2018-09-25T15:48:53.432Z Reads: 256

```
Like TB vescs and others on the same price range (or even higher) are better. There is always a trade-off.
```

---
## \#30 Posted by: mixedcreation Posted at: 2018-09-25T16:00:44.156Z Reads: 264

```
Running a single 6374 with the Flip6.6 & 10s3p 30q setup.  

MM= 60A
MB= -50A/-60A
BM= 40A
BR= -12

Max 30mph, mostly cruise at 20-24mph.  Running this setup for the past 2 months.  Hasn't been an issue besides an extremely hot NC summer day going up a decent hill.  Weather was around 95, with 70% humidity.  Grade hill was around 15%.  

Besides that one time during that extremely hot day, it hasn't hiccuped at all.  Very impressed with how it has been going.  Wish I had a dual setup to test it on my dual 6374 or even my dual 6355 setup.
```

---
## \#31 Posted by: Riako Posted at: 2018-09-25T18:58:57.901Z Reads: 268

```
Ok e-riders :slightly_smiling_face:
[Tonight ride](https://amadridefr.files.wordpress.com/2018/09/screenshot_20180925-205437.jpg?w=240) was with this setup : 
https://amadridefr.files.wordpress.com/2018/09/screenshot_20180925-190245.jpg?w=240
Work almost perfect, but on 3 hard long braking, I got the throttle/brake cut ... just like that ... I got to re-arm it to make it work again ... weird and it does report faults just once with a Over Current...
https://metr.at/r/ZvL4k
Apart of that got a bit more torque maybe, but it's still really wick ... Got some full throttle time always :smile: 
I hurry to get my custom motor mount, when I will pass in Quattro mode it should help them a lot !
```

---
## \#32 Posted by: linsus Posted at: 2018-09-26T13:02:32.278Z Reads: 257

```
Hi folks.

@Hummie reached out and said flipsky was looking for some help/tips and also wanted to know where to donate and what not. So i put them in contact with BV. Here is the official response from BV (yes he exists) regarding the flipsky dual;

"Hi,

I had a quick look at the document with the feedback, and users seem to have both overcurrent and drv faults. To me it sounds like there are layout problems with the power stage and/or the current sensing signal path. Making the power stage right is quite tricky, and the vesc4 still had some issues after all revisions. I also made some designs before the V4 that didn't work well at all, that I never published. The VESC6 is the first layout where I got the power stage right, making it run extremely well even on the most demanding setups.

Also, using only two shunts is a lot more challenging for getting the signal path right, as the sampling interval gets very short in the worst case during high modulation. Personally I won't make new design with only two shunts any more, as three shunts is much more stable and gives a significantly more linear and smoother acceleration. For new designs that focus on low cost, I would recommend something like the DRV8305 with three low-side shunt amplifiers. Three phase shunts with external amps such as the INA240 as the VESC6 has is better of course, but three low side shunts are still far better than only two shunts.

If you want to, I can have a quick look at your gerber files and see if there are any obvious problems."

So thats status so far. Just thought that everyone should be on the same page.

cheers.
```

---
## \#33 Posted by: brenternet Posted at: 2018-09-26T13:17:11.591Z Reads: 246

```
Mr Vedder continues to be a hero. A quiet hero.
```

---
## \#34 Posted by: BruSkater Posted at: 2018-09-30T15:33:05.221Z Reads: 245

```
Still good results Mike? Have you tried upping the motor amps?
```

---
## \#35 Posted by: mmaner Posted at: 2018-09-30T15:36:09.593Z Reads: 249

```
Actually just rode it. Using 30a motor max and 50a battery max per motor, no cutouts & no errors. 

https://metr.at/m/vb8l
```

---
## \#36 Posted by: BruSkater Posted at: 2018-09-30T15:51:03.612Z Reads: 244

```
But why are you only at 30 for motor max? You found that it is enough for your needs or you had trouble with higher amps?
```

---
## \#37 Posted by: mmaner Posted at: 2018-09-30T16:07:14.178Z Reads: 242

```
Over 30 I get cutouts.
```

---
## \#38 Posted by: Hummie Posted at: 2018-09-30T16:20:01.946Z Reads: 244

```
It’s probably not as bad at 30 motor amps with a pulley but I like 100!

Maybe I missed something above but the 6.6 on the other hand is showing totally capable and the few that broke in the last group buy (all by the same person and his suspect motor) flipsky told him to send them back for repairs.   

Doing another group buy for the 6.6 only.
```

---
## \#39 Posted by: Komamtb Posted at: 2018-09-30T16:31:05.969Z Reads: 247

```
Dual 6.6, was working great on 12s, but poped a few chips just being put aside on a table.
```

---
## \#40 Posted by: Hummie Posted at: 2018-09-30T16:40:15.009Z Reads: 247

```
Maybe a strong conformal coating on them is worth doing
```

---
## \#41 Posted by: Riako Posted at: 2018-09-30T17:42:16.875Z Reads: 250

```
Another ride tonight, and at this end would like to provoke some faults,.. and I pretty good to this  :blush: 

Friday night (+22/-22 A Motor 30 batt max and -15 batt min), cruising cool : 
https://metr.at/r/qpm1H
Saturday evening same parameters, riding still cool : 
https://metr.at/r/BQNM7

Tonight I start with the same again : 
https://metr.at/r/5wKVM

And when I want to play a bit harder at the end, trying +-25A Motor and 35A batt max, applying full throttle uphill, I cunt around 8 faults over current ... : 
https://metr.at/r/5nWnZ

So whats should be my next test :smile: !?
```

---
## \#42 Posted by: Okami Posted at: 2018-09-30T18:25:28.836Z Reads: 221

```
Hm i saw 55 motor amps in your logs and thats when it seems to cutout..

Luckly i dont have many hills around my place but will see what results i get after i hook it up (still havent managed that yet)
```

---
## \#43 Posted by: Riako Posted at: 2018-09-30T18:40:52.724Z Reads: 225

```
Yes, and you could see 7 other at the ends of the ride when I try to reproduce that, uphill or on flat almost from start.
I will run them hard again tomorrow at again 22A/motor so almost 45A max, but with still 35Amps batt max, and then go low to 30a and see if it faults as easy as I made it happen at the end ...

All that is cool, test and see the limit of overcurrent, but if you need an urgent braking you still could have Over intensity ... this will be a board exclusively for me now and for cruise mode !
Still got this drop from 0 to +40a motor when I'm braking ... is it normal ? (after the braking all the over intensity is drop to the motor ?) Look at the end of the last ride
```

---
## \#44 Posted by: Riako Posted at: 2018-10-01T21:25:49.091Z Reads: 228

```
Ok run them today like I say at 22A Motor and 30A batt, I can still make it Over intensity if I really play with the throttle in uphill but somethimes it handle more without problem and sudently, FAULTS !.. 
https://metr.at/r/N9pxP
```

---
## \#45 Posted by: BruSkater Posted at: 2018-10-01T21:28:44.672Z Reads: 217

```
Have you contacted Flipsky about this? Are they going to do something about this issue? They should since they advertise 50A continuos per esc...
```

---
## \#46 Posted by: Riako Posted at: 2018-10-01T21:35:15.678Z Reads: 217

```
Yes, they're replacing my mini's actually, I'm waiting them with new caps and then same for this dual I guess.
loading ...
Its a chance that the season is almost ended for esk8, and I will be back on my eMTB under VESC6 at 70Amps Motor& batt cause all of this is a lot of frustration :smile:
```

---
## \#47 Posted by: Riako Posted at: 2018-10-01T21:37:49.043Z Reads: 212

```
we are so far from that ... and they was supposed to be 12s and why not foc !..
I had planned all my setup with 12s ratio etc (got 16A 30C of graphene for this) ... and I was locked at 10s 5Ah (just what I got in stock ^^) no sensor, no foc ... no luck
```

---
## \#48 Posted by: Okami Posted at: 2018-10-02T10:14:20.908Z Reads: 214

```
Mh it starts to sound really messed up now..

Will see whenever Flipsky will pay attention and what action they will take
```

---
## \#49 Posted by: Hummie Posted at: 2018-10-02T16:51:52.501Z Reads: 215

```
But the 6.6 is showing well.  Almost no one with a problem with it. ...and with the group buy at 125$ it’s a great deal.  It uses three sensing shunts not just two as the 4 uses
```

---
## \#50 Posted by: M.Hboards Posted at: 2018-10-03T23:39:13.412Z Reads: 212

```
@mmaner would you change any of these settings if you were running a 10s3p pack instead of a 4p?
```

---
## \#51 Posted by: mmaner Posted at: 2018-10-04T00:08:39.493Z Reads: 219

```
yeah, Id make battery current 35 or 40a.
```

---
## \#52 Posted by: mtuan293 Posted at: 2018-10-04T17:07:54.157Z Reads: 227

```
Behold...Hall of DRV_FAULTS for 4.20 dual. Running **10s**2p Samsung 20R pack, FOC with 5055 270kv motors from DIYeboard kit. Tried on both stock and Ackmaniac's, the only difference is on stock you have to release the throttle to gain control back, while on Ack's it can reset itself.
Settings on each VESC:
Motor: 80 / -80
Battery: 20 / -5

![image|281x500](upload://xThW7MLq2dsbl3GqMmz9pSLpVUJ.jpeg) ![image|281x500](upload://91ro4VvoCHBGys76rPsJ168EyYv.jpeg) 

![image|281x500](upload://82Wn0dkO4o9Ts8iRE89YifixPXi.jpeg) ![image|281x500](upload://w7AlE8ImiCFYCTRdDD7cpfOLv2P.jpeg) 

![image|281x500](upload://zJAQiSicUl0Q7wWZac9OtZVvzDH.jpeg) ![image|281x500](upload://3VQsURcrZbXHChO91sLgfaEgIWl.jpeg)
```

---
## \#53 Posted by: Hummie Posted at: 2018-10-04T17:39:13.041Z Reads: 206

```
why's it show duty cycle at almost 0 on all of them but showing youre at higher erpm?
```

---
## \#54 Posted by: mtuan293 Posted at: 2018-10-04T17:42:17.497Z Reads: 209

```
[quote="Hummie, post:53, topic:68940, full:true"]
why’s it show duty cycle at almost 0 on all of them but showing youre at higher erpm?
[/quote]

I guess that's when the cutout happens so duty cycle is 0?
```

---
## \#55 Posted by: brenternet Posted at: 2018-10-04T17:42:24.437Z Reads: 217

```
My findings:

Dual 6.6 is flawless but too big for the board I want it in so it will go in my Hummie build at some point in the near future.

Dual 4.20 is pretty disappointing, 10s5p 30q's on dual 6355's with @mmaner settings, on both FOC and BLDC I'm getting cut outs, specifically when braking, even just coming to a complete stop from slow it will get almost there and then cut out at the last second. I'm going to replace it with two focboxes and bench it.

Single 4.12 (not the mini) runs better than the dual, on BLDC with similar settings to a focbox it ran well. I didn't try FOC, I don't think it was built for that at all, I bought them for £36 each ffs :smiley:
```

---
## \#56 Posted by: Hummie Posted at: 2018-10-04T17:47:04.092Z Reads: 217

```
for weeks or months now been showing the 6.6 as good and solid (group buy is on!) and the 4.2 as problems with cutouts or faults.  

  but I thought duty cycle and erpm would be hand in hand always based on speed you were going
```

---
## \#57 Posted by: Benjamin899 Posted at: 2018-10-04T17:48:28.860Z Reads: 220

```
cant comment on 6.6 and 4.20 but my 4.12 works fine up till now.
```

---
## \#58 Posted by: mtuan293 Posted at: 2018-10-05T06:59:55.989Z Reads: 222

```
So the 4.20 dual is trash now? Damn... I was expecting too much for this....Been waiting over a month for it to arrive (thanks @Hummie, maybe if you hadn't made me wait that long, I would have felt better lol)
```

---
## \#59 Posted by: akira Posted at: 2018-10-05T07:09:31.116Z Reads: 218

```
I would like to get the schematics of the modified vesc versions from flipsky. They have to publish it because of the gpl licence of the vesc. 
The decision not to publish it is a violation of the licence and an inaceptable denial of respect for Ben, the vesc developer.
That s th information I would like.
```

---
## \#60 Posted by: Benjamin899 Posted at: 2018-10-05T11:42:16.641Z Reads: 215

```
yeah i will wait for further clearification otherwise i will go back to established brands.
```

---
## \#61 Posted by: Lumaci Posted at: 2018-10-05T12:01:10.290Z Reads: 212

```
Its not trash, its cheap so it needs to be handled like a cheap vesc.

Run it at around 30A per unit max, dont try to pull to many amps of it and it should be fine from the looks of it.
```

---
## \#62 Posted by: mtuan293 Posted at: 2018-10-05T15:39:13.252Z Reads: 207

```
Hmm... their 4.12 is cheap too. @brenternet confirmed that it can run well. I still have their 4.12s, let me put them back in and see how they go compared to this 4.20.
```

---
## \#63 Posted by: Riako Posted at: 2018-10-05T20:16:46.211Z Reads: 209

```
even at 20A batt and motor max it faults ...
I made many tests with the metr.pro and even with low setup, and cruising easily you could be confronted to overcurrent or intensity ... 
And yes sometimes it goes all good during 2 or 3 rides. But be really careful don't ride this to much confident.
Edit : Dual 4.20
```

---
## \#64 Posted by: Benjamin899 Posted at: 2018-10-05T20:45:08.180Z Reads: 219

```
damn, well i was riding with my flipsky 4.12 today and i have Battery 35A and Motor 80A, no faults
Here a Screenshot. ![vescmonitor|281x500](upload://j2TPM3LaxiowqBUBA7ja9W9tHlo.png)
```

---
## \#65 Posted by: DAddYE Posted at: 2018-10-06T01:04:13.871Z Reads: 214

```
30/30a and I get 2/3 faults with ease. Do you guys think if I cut the battery max cutoff is going to help?

https://metr.at/r/eJnOT
```

---
## \#66 Posted by: Benjamin899 Posted at: 2018-10-06T10:06:09.315Z Reads: 211

```
dunno, but you always got one when you got close to the 30a battery max. which is weird. how much can your battery give?
```

---
## \#67 Posted by: Kug3lis Posted at: 2018-10-06T10:13:39.719Z Reads: 207

```
One thing I suspect is that their passive components suck and fck up reading or etc, if voltage is jumping the same way current readings will jump too..
```

---
## \#68 Posted by: brenternet Posted at: 2018-10-06T10:49:49.660Z Reads: 208

```
Messed around some more with the dual 4.20 yesterday, dropped to Motor 25 -25, Battery 40 -40 and only had one fault in a 2 hour ride. Unfortunately it was going down a pretty nasty hill and I was even being extra careful - not good enough. If I lived on the absolute flats with no hills to deal with it would be fine for a small chuck around board but I just don't trust it.

Not to mention that it had no balls at all configured that way.. hill climbing on a single focbox was similar to dual with this.
```

---
## \#69 Posted by: DAddYE Posted at: 2018-10-06T11:18:51.537Z Reads: 202

```
I’ve set 30A battery max -7 battery regen.
```

---
## \#70 Posted by: Hummie Posted at: 2018-10-06T15:54:18.644Z Reads: 203

```
To confirm u guys with the cutouts from overcurrent are using the 4.2 right and not the 6.6?
```

---
## \#71 Posted by: brenternet Posted at: 2018-10-06T16:02:23.465Z Reads: 200

```
Yes. 6.6 is flawless for me
```

---
## \#72 Posted by: DAddYE Posted at: 2018-10-06T18:05:16.352Z Reads: 203

```
Yup. That’s my case.
```

---
## \#73 Posted by: Riako Posted at: 2018-10-07T01:17:52.572Z Reads: 199

```
Yes, exactly, Dual and mini.
EDIT :blush: 4.20
```

---
## \#74 Posted by: DAddYE Posted at: 2018-10-07T02:01:09.056Z Reads: 207

```
It seems that the 4.20 works great on 10s. Wonder why. 

Have anyone tried to limit the wattage and the battery cutoff and see if helps?
```

---
## \#75 Posted by: Ixf Posted at: 2018-10-07T02:04:15.521Z Reads: 208

```
6.6 dual. 12s lipo
Theres no good hills around where I live... so i did the next best thing... I put on bigger tires :p to stress the vesc.
Managed to max out the motor 80amps and 34amps on battery.  Didn't skip a beat.  Now if the voltage reading will actually be steady.. it would be perfect... Can't complain I guess.. its cheaper then 2 focboxes
 ![image|690x282](upload://xZ7RDeVSz55VP5uA8rmLU9AlYM7.png)
```

---
## \#76 Posted by: brenternet Posted at: 2018-10-07T06:50:51.988Z Reads: 210

```
It does not work for me on 10s.
```

---
## \#77 Posted by: Riako Posted at: 2018-10-07T09:18:33.483Z Reads: 211

```
Same doesn't work great at all on 10s too.
```

---
## \#78 Posted by: Pmac Posted at: 2018-10-08T04:51:43.476Z Reads: 211

```
I finally set up my 4.2 dual in FOC and it runs well.

I need to adjust my setting though as something happened yesterday.

I was accelerating up a hill and the board all of a sudden slammed the brakes on me kicked me off and as i was still holding the throttle the board went up the curb.  Did a barrel role and just got some road rash on my elbow which was lucky.  I need to check what i have done as I am also unable to connect to the flipsky bluetooth module through Ack firmware.  So I'm sure i fudged something up.

That brings my count of falling off to 2 times and i probably have only done maybe 150km of riding, so not a great start.  Better than the first fall though.  Bent my knee sideways and was on crutches for 6 weeks.
```

---
## \#79 Posted by: Benjamin899 Posted at: 2018-10-08T07:09:25.275Z Reads: 206

```
Sounds Like overcurrent or  voltage cutoff. Happened to me too this Weekend. Battery was already down to 20% and i went full throttle and bamm cutoff flored me. Got some nasty rashes on my knee because my Pads slipped Up.
```

---
## \#80 Posted by: Pmac Posted at: 2018-10-08T10:18:08.013Z Reads: 206

```
I'm hoping it wasn't voltage cut off as that would mean i have some crazy voltage sag going on as I was at just under 70%.
```

---
## \#81 Posted by: dspx Posted at: 2018-10-08T13:27:11.450Z Reads: 202

```
Jesus, is the 4.2 Dual a death trap? I haven't even set mine up yet (planned to run on 10s with hub motors/CarvON) - but at this point, do I even want to?
```

---
## \#82 Posted by: brenternet Posted at: 2018-10-08T13:30:03.707Z Reads: 208

```
It's not a death trap haha. Don't panic. It's just a bit lame
```

---
## \#83 Posted by: visnu777 Posted at: 2018-10-08T13:44:27.169Z Reads: 212

```
Today I did a first speed test with the 2x FSESC 4.12 @ 12s on unsensored FOC and it worked as it should. I made it to 52kph which is the calculated limit I could get, 43000 erpm.
```

---
## \#84 Posted by: Riako Posted at: 2018-10-08T16:46:40.966Z Reads: 215

```
Some questions, processor of **FSESC6.6** :slight_smile:

**Wow did you set your ESC in your case ?**??
They're even more complicated to integrate or fix them in your enclosure !? 
What do you think? Do you have some pics ? :mag: ideas ??:bulb:

Thanks a lot for your help :blush:
```

---
## \#85 Posted by: Static Posted at: 2018-10-08T19:09:25.835Z Reads: 208

```
I asked this too. Not really an easy way to mount these, especially if you want any kind of cooling. 

When I tested them i just used lots of foam in the enclosure. We need a good 3D printable design to secure them
```

---
## \#86 Posted by: brenternet Posted at: 2018-10-08T19:32:25.084Z Reads: 202

```
3m sticky back hardcore velcro. It won't come loose and gives good vibration dampening. It's pretty easy to solve this issue.
```

---
## \#87 Posted by: Pmac Posted at: 2018-10-08T21:50:47.582Z Reads: 221

```
No, it's not a death trap.  If this was due to battery cutoff than  its an issue with the batteries.  or my setting on the battery cutoff being too high.

I'm pretty sure there are setting with what the vesc should do in the instance of a battery cut off so you should be able to adjust it so it doesn't brake.

I am still a total newb so I am trying to learn as much as possible.

Cheers,
Patrick
```

---
## \#88 Posted by: Riako Posted at: 2018-10-09T01:35:58.297Z Reads: 223

```
Thanks! Yeah on a lot of vesc, v6, focbox or escape ... but here with the 6.6, I'm a bit annoy... 
Where did you put it for the hardcore fix on the FSESC6.6 ? on the heatsink? yes, it should old enough, but I would like to let the heatsink out of the case..
Do you have a photo ? :) plzzz

@Static, I think I will try to do that (plus velcro if I find a way to ensure more) ;)

Edit: I'm talking about the 1st single with PSA and the xt90 ...
https://cdn.shopify.com/s/files/1/0011/4039/1996/products/DSC05342_360x.JPG?v=1536542345
```

---
## \#89 Posted by: Pmac Posted at: 2018-10-09T12:30:46.995Z Reads: 215

```
Hi All,

just wanted to say that the flipsky bluetooth module will only work with the VESC Tool on Android.  May work with other apps on iOS but I have no way of testing this.

Cheers,
```

---
## \#90 Posted by: Bor.inc Posted at: 2018-10-09T19:39:15.682Z Reads: 205

```
Guys maybe you can help, what is more a more reliable/ better setup:
dual tb vesc 4.12 or the dual 4.2 fesc
```

---
## \#91 Posted by: visnu777 Posted at: 2018-10-09T19:49:40.053Z Reads: 206

```
Try 2x FSESC 4.12, they have a great price/value ratio. You'll get 2 of them for the price of one tb ESC and so far they seem to be good quality. I'm running 2of them at 10s and 12s in FOC without any issues,from the tb ESC I heard/read no good so far.
```

---
## \#92 Posted by: brenternet Posted at: 2018-10-09T20:27:44.392Z Reads: 199

```
[quote="visnu777, post:91, topic:68940"]
Try 2x FSESC 4.12
[/quote]

I'd do this personally.
```

---
## \#93 Posted by: Bor.inc Posted at: 2018-10-09T20:37:28.815Z Reads: 196

```
serious? @visnu777 @brenternet
I thought tb is a bit more reliable because they are longer on the market but I guess not, the only thing is that I already have a tb vesc so I think it will be easier for me to buy an extra tb instead of buying 2 fesc 4.12's and selling my tb
```

---
## \#94 Posted by: brenternet Posted at: 2018-10-09T20:47:31.320Z Reads: 199

```
I get what you are saying though but there's multiple people running these fesc 4.12's on 12s foc and I bought one on ebay from a seller by offering $47.

$100 for a tb vesc that is designed for BLDC or two new 4.12's for a very similar price that appear to perform better? Seems like a no brainer to me haha. Sell your spare tb vesc and get better results for half the money.
```

---
## \#95 Posted by: Bor.inc Posted at: 2018-10-09T20:50:58.572Z Reads: 199

```
Ah thanks for the advice, now we can go on topic again haha
```

---
## \#96 Posted by: brenternet Posted at: 2018-10-09T20:51:44.858Z Reads: 197

```
We're definitely still on topic here with this discussion.
```

---
## \#97 Posted by: Benjamin899 Posted at: 2018-10-09T21:05:56.465Z Reads: 199

```
i use my fsesc 4.12 with a focbox in a dual setup, so you actually don't need to buy 2, just one.
```

---
## \#98 Posted by: Bor.inc Posted at: 2018-10-09T21:07:09.381Z Reads: 198

```
ooff thats another level, I have always wondered if using to different vescs together would work
```

---
## \#99 Posted by: Benjamin899 Posted at: 2018-10-09T21:10:41.955Z Reads: 198

```
yeah, but i run them over Split PPM, since i don't want to risk damage over CAN, but then again someone said that it doesnt matter....there is a real advantage to a dual setup over CAN, changing setups over bluethooth on the fly is rly something. For example when the battery goes below 50% you can switch to a more conservative setting to avaid strain or cutoffs.
```

---
## \#100 Posted by: brenternet Posted at: 2018-10-09T21:28:11.308Z Reads: 204

```
What sort of settings are you running them together on out of interest?
```

---
## \#101 Posted by: Benjamin899 Posted at: 2018-10-09T21:42:32.627Z Reads: 204

```
old setup 
Motor 60/-60
Battery 35/-12

until i had a nasty cutoff. i was already running on my last 20% and hitting the throttle must have strained the battery too much and i rushed through my slow cutoff directly to the hard cutoff and i lost balance. Funny to watch my log. It went from 33v to 30V and then in about 1-2seconds down to 26v. 

new setup
Motor 60/-60
Battery 25/-12
```

---
## \#102 Posted by: Bor.inc Posted at: 2018-10-09T21:43:10.116Z Reads: 198

```
And what is the difference between the fesc mini and the fesc 4.12 other than the dimensions, has the 4.12 better performance?
```

---
## \#103 Posted by: Benjamin899 Posted at: 2018-10-09T21:45:33.465Z Reads: 201

```
4.12 is still based on the the classic shematic as far as i know, the 4.20 is an "improvment". post nr.32 explains it.
It is not a bad product but it doesnt handle current as well as the old 4.12.
```

---
## \#104 Posted by: Riako Posted at: 2018-10-09T23:39:41.356Z Reads: 209

```
Personally, getting the 4.20 dual and mini ... I'm changing them too for fsesc 4.12 like _brenternet_.
Making an AWD setup, I prefer to go with 4.12, it's more stable IMO. 

Just another ride to go "quickly" to the post office and don't know why ... I start with a fault... It really doesn't prevent, even with more than a month of the ride now, I set low parameter for them, go easy on the throttle and ride cool but this thing still has not reassuring faults : 
https://metr.at/r/ogOs2

I would love so much this dualFSESC4.20 handling like the old 4.12 !!!...
```

---
## \#105 Posted by: brenternet Posted at: 2018-10-10T11:21:53.013Z Reads: 202

```
@longhairedboy did you pursue any further with the 4.20 dual in the end or just bench it? I know you spoke to them about cut outs and they accused your battery. Did that go any further?

They're pretty much accepting it's limitations now are aren't making excuses. I'm asking for a solution though so let's see how the customer service works out.
```

---
## \#106 Posted by: Riako Posted at: 2018-10-10T12:11:26.044Z Reads: 203

```
I guess we got no solution for them ... Even with better and bigger caps, it didn't handle it well ... HW issue :persevere:
```

---
## \#107 Posted by: Riako Posted at: 2018-10-10T12:12:07.102Z Reads: 212

```
[quote="Static, post:85, topic:68940"]
We need a good 3D printable design to secure them
[/quote]
I try to work on it yesterday :blush: a slim fit inside, locked with silicon glue to prevent vibration?
https://amadridefr.files.wordpress.com/2018/10/escsf_2018-oct-09_02-46-48am-000_customizedview3583755963.png

* Want to keep the heatsink direct on top for air flow (will have fun with silicon or so I guess)
* Need another stage (2nd), below the "holding" space (1st stage), to pass sensor uart ppm wires etc.
* it sizes actually 165 x 84 x 22 mm

https://amadridefr.files.wordpress.com/2018/10/sdfghn51b.jpg
If you have any advice e-riders, please don't hesitate :v: ;)
```

---
## \#108 Posted by: longhairedboy Posted at: 2018-10-10T14:37:43.213Z Reads: 200

```
i told them it was a manufacturing defect and binned it. I can't ride on it reliably and they didn't seem keen on fixing the issue. So i don't know what happens next.
```

---
## \#109 Posted by: AreaKruzer Posted at: 2018-10-10T14:43:27.928Z Reads: 201

```
That's quite a bummer though
```

---
## \#110 Posted by: DAddYE Posted at: 2018-10-10T14:48:51.417Z Reads: 196

```
Got mine replaced. No much question asked.
```

---
## \#111 Posted by: Riako Posted at: 2018-10-10T22:35:36.569Z Reads: 199

```
If someone want to have a look ;) 
https://www.thingiverse.com/thing:3148179
```

---
## \#112 Posted by: mtuan293 Posted at: 2018-10-11T19:07:39.562Z Reads: 203

```
[quote="mtuan293, post:52, topic:68940"]
Behold…Hall of DRV_FAULTS for 4.20 dual.
[/quote]

So I’m back here to report to you guys. I changed it to BLDC mode and **no more cutouts**. I guess this is still the nature of VESC 4 having issues running FOC.

[quote="linsus, post:32, topic:68940"]
Here is the official response from BV (yes he exists) regarding the flipsky dual;

"the vesc4 still had some issues after all revisions. I also made some designs before the V4 that didn’t work well at all, that I never published. The VESC6 is the first layout where I got the power stage right, making it run extremely well even on the most demanding setups."
[/quote]

[quote="visnu777, post:91, topic:68940, full:true"]
Try 2x FSESC 4.12, they have a great price/value ratio. You’ll get 2 of them for the price of one tb ESC and so far they seem to be good quality. I’m running 2of them at 10s and 12s in FOC without any issues,from the tb ESC I heard/read no good so far.
[/quote]
@Kug3lis sorry for dragging you into another flipsky post haha. What do you think? Does cheaper mean worse in this case?
```

---
## \#113 Posted by: Flashgod224 Posted at: 2018-10-14T12:33:33.271Z Reads: 198

```
I have been running the 4.20 dual from Flipsky for a bout 4 weeks now.

Firstly I started with BLDC 36/15t,10s5p 30Qs on 110mm wheels using their 6354 motors. I could not believe all the over-current faults I got on startup, it was VERY disappointing. 

Then I went to use sensored hybrid and it was better but over-current faults do still tend to happen. After this I went over to using FOC in which 99% of the problems disappeared but I also dropped down to 97mm wheels. The big issue is hard acceleration and breaking when you need more power within the instances thus getting the blessed cutout. Re-arming the throttle is the quick fix, but I definitely think that a higher gear ratio would be best for this dual VESC and adding a very generous throttle curve. I don't think it's best to handle this vesc at higher speed than 45ish km/h.

I only run my 110mm wheels when I go on my local race track to hit 55km/h which is fine because I am very gentle on the throttle.
```

---
## \#114 Posted by: Okami Posted at: 2018-10-14T12:45:23.233Z Reads: 194

```
@Flashgod224 what settings u ended up using?
```

---
## \#115 Posted by: nuttyjeff Posted at: 2018-10-14T12:46:36.740Z Reads: 194

```
The FESC 6.6 seems to be the ESC to go for flipsky. The voltage readings are pretty much fucked though.
```

---
## \#116 Posted by: Flashgod224 Posted at: 2018-10-14T12:48:01.254Z Reads: 195

```
I bypass BMS fyi, so if I remember correctly @Okami 
45
-45
35
-18
```

---
## \#117 Posted by: Benjamin899 Posted at: 2018-10-14T12:56:46.732Z Reads: 204

```
thats something i can't wrap my head around. why did they not notice this
```

---
## \#118 Posted by: SkaterBoy58 Posted at: 2018-10-14T23:15:17.039Z Reads: 211

```
No QC or real life testing
```

---
## \#119 Posted by: brenternet Posted at: 2018-10-17T22:23:27.533Z Reads: 211

```
So the polls here and general forum posts are pretty clear now. Please correct me if I am wrong so that I can adjust this for future buyers.

Motors are 50/50 and not recommended due to epoxy and magnet issues. Especially the 6374
4.20 dual appears to just about work on 10s and lower BDLC on moderate settings
4.12 single is decent with reasonable settings, even on FOC.
4.20 mini single isn't worth buying over the 4.12 single
6.6 single works well, decent settings, FOC
6.6 dual works well, decent settings, FOC

Flipsky do support the products, they are aware of the issues and are actively trying to resolve them at a manufacturing level.

Refunds, replacements and communication is happening, if a little slow some times.

As with everything at this price point a solid visual inspection is needed before plugging in.

Looks like the real winners here are the 4.12 single in my opinion, the 6.6's will give you great results on top end boards but bang for your buck on a mid range build that 4.12 is a beast at ~$55 with a aluminium case at ~$30 on eBay.

Comments or corrections?
```

---
## \#120 Posted by: nuttyjeff Posted at: 2018-10-18T00:29:43.228Z Reads: 208

```
I think the motors that have the most problems are the 6355s, bot the 6374s?
```

---
## \#121 Posted by: brenternet Posted at: 2018-10-18T01:14:47.234Z Reads: 210

```
Can anyone confirm this please?
```

---
## \#122 Posted by: Flashgod224 Posted at: 2018-10-18T01:20:54.568Z Reads: 212

```
I am running the 6354 motors, no issues.
```

---
## \#123 Posted by: brenternet Posted at: 2018-10-25T18:50:37.343Z Reads: 216

```
Looks like they've taken to stocking the same set that diyeboard sell?

https://flipsky.net/collections/new-accessories/products/copy-of-bldc-belt-motor-6374-190kv-3250w

diyeboard:

* (2) N5055 Motor Mounted (Black, 270KV, 1400W/Motor)
* (1) 7.25'' Rear Truck with two 83*52mm PU wheels mounted(Black/Red)
* (2) Motor Mount (Black)
* (2) 35T Drive Wheel Pulley (HTD5)  13mm width
* (2) 13T Motor Pulley (HTD5)  13mm width
* (2) 250-5M High Torque Timing Belt (HTD5)  12mm width

Flipsky:

* 2* N5055 Motor Mounted (Black/Red, 270KV, 1200W)
* 2* Bolt On Motor Mount (Black)
* 2* 7.25'' Truck (Black)
* 2* 35T Drive Wheel Pulley (HTD5)  13mm width
* 2* 13T Motor Pulley (HTD5)  13mm width
* 2* 250-5M High Torque Timing Belt (HTD5)  12mm width
* 4* Wheels:  83mm*56mm 83a Longboard Wheels

They list 1200w vs 1400w at diyeboard but these are the same product right? 

I wonder if they know these trucks routinely snap in half.

@BarbaraZ care to comment?
```

---
## \#124 Posted by: Scream Posted at: 2018-10-26T00:47:37.044Z Reads: 209

```
I’m going to purchase the 6354 motors for my build. I read somewhere on this forum that the loose magnet issue with the 6374 motors was probably due to the cans swelling with heat, rather than the type of glue used. Perhaps it’s feasible that this issue doesn’t affect the 6354 motors as smaller surface area of can = less swelling?

The solder ball issue is obviously still concerning, but it sounded like maybe they’re addressing this going forward. I haven’t read of any actual problems this has caused with flipsky motors... but there’s obviously potential for significant issues if the solder balls were to short the windings.
```

---
## \#125 Posted by: Riako Posted at: 2018-11-30T03:56:46.750Z Reads: 196

```
Some news for the dual 4.20 Plus 10s max 30A/motor
https://cdn.shopify.com/s/files/1/0011/4039/1996/products/01_d4f45a48-32ae-41e2-869d-05ad206a4471_1800x1800.jpg?v=1543545669
https://flipsky.net/collections/electronic-products/products/dual-fsesc4-20-100a-plus-based-on-vesc-with-anodized-aluminum-heatsink
```

---
## \#126 Posted by: BruSkater Posted at: 2018-11-30T04:27:36.921Z Reads: 192

```
@mmaner is there any point in setting 50a on battery if motors are only taking 30a max? Shouldn't be the same to set bat at 30a?
```

---
## \#127 Posted by: mmaner Posted at: 2018-11-30T04:29:13.978Z Reads: 199

```
It's let's the battery drain as fast as the ESC can demand. At least in theory. I haven't really tested accross multiple boards.
```

---
## \#128 Posted by: Gamer43 Posted at: 2018-11-30T06:53:32.628Z Reads: 201

```
I would just like to add that I've been running two (singles) mini FSESC 4.20s on delta-wound (reterminated) 8-in hoverboard hub motors in sensored FOC, and I've had little issues with them over 50 miles. 10s lipo (super cells from jehu garcia's listing on ebay, these things REALLY pack the power).  
The only problem I've had is that they can't handle prolonged stall conditions and instant flooring and braking. Throws a DRV fault. Positive ramping time solved the latter, not attacking 50% grades solved the former.
I got up to 22 mph before almost cracking my head open. (The board could have easily done 25+mph, and I was being an idiot).

From the DRV8302 datasheet, DRV faults are thrown during overcurrent, overvoltage and undervoltage conditions on gate drive and power supply. In the schematics, overcurrent protection is disabled (but can still trigger at extreme VDS thresholds, I actually need to check if Flipsky might have actually implemented a divider for OC_ADJ). Considering the same caps are used on the 6.6, it is likely not a power supply UV or OV fault. The only difference between the 4.20 and 4.12 is the choice of MOSFETs and bypass capacitor placement (which, I would think, are both better on the 4.20, but the 4.12 uses larger capacitors to compensate). The 4.20 mini uses only one set of NTMFS5C628NLT1G MOSFETs, so my best guess as to why the faults are occurring are either the large slew rates (because the gate charge on these fets is REALLY good) causing a overvoltage or undervoltage event, or that the MOSFET body diodes are actually saturating during dead-time. I am thinking this because in VESC tool, the DRV faults were thrown around 40A during low speed, high torque demand conditions, this means current slew rate is very high. In the NTMFS5C628NLT1G's datasheet, the graph for body diode forward voltage cuts off at 40A. This is just a hunch, but many signs are pointing that it is some aspect with the MOSFETs that are triggering the DRV faults people are seeing.

Taking a closer look at the 4.20 mini, the PCB is reasonably well designed; components are neatly laid out and bypass capacitors are placed where they are needed and the tracks minimize parasitics. It just seems like a piece of junk because it really can't handle many of the heavy loads some of the users here have tested it with. Honestly, I think it would be perfect for lighter builds (like 5065 or 6355 single motor with max speed of 15-20 mph). It only has one set of MOSFETs that have twice the RDSon of the FETS on the 4.12 and are rated for half the current (but they have one-tenth the gate charge, so they are ideal for FOC, actually). 

For heavier builds (like climbing hills from a standstill or any kind of racing), the 4.20 is definitely not suited for the task. For lighter and/or cost-effective builds, I think it would fit right in. It is more compact than the 4.12 and generates less heat in FOC because of the (MUCH) lower switching losses. 

I would actually recommend FSESC over TB ESCs, my friend ordered two VESCs from DIYEletricSkateboard and one of the VESCs literally died on his second use when configuring it for FOC (the DRV 8302 gate driver circuit failed). I then tried a pair of TB VESCs with my motors; there was quite a bit of cogging during tuning and start-up and they also couldn't handle stall conditions. Motors ran much more smoothly with the FSESCs. 

If my hunch is correct, then using hot air rework to replace the mosfets with something like the NTMFS5C604NLT1G might solve the DRV fault issues. But, those MOSFETs are twice as expensive and have 2.5 times the gate charge.
```

---
## \#129 Posted by: mtuan293 Posted at: 2018-11-30T07:32:30.962Z Reads: 186

```
Thanks for the input. I run my setup using 5055 270kv motors, with battery current max of 20A in 10s. Everything works fine in BLDC.
In FOC if I hard throttle or hard braking, then DRV_fault happens, and it cuts off for a second. However if I ease on the throttle, I can still climb steep hills here in SLC.
Now I’m scared to run in FOC because it once cut off on me when I had to brake because I was close to people. 
I actually tried changing the time to cut off from 500ms to 0ms in the advanced settings section of vesc tool, but still didn’t work, just didn’t report any DRV_fault, but still cut off.
```

---
## \#130 Posted by: Gamer43 Posted at: 2018-11-30T08:11:17.024Z Reads: 188

```
Just curious, how fully charged were your batteries when you attempted this? I noticed I can sometimes trigger overvoltage (triggered on MCU firmware, not DRV) faults if I send too much charging current, this is usually if I have a BMS installed on the battery as I'm guessing the BMS is cutting off the motor controller because one (or more) of the cells can't handle the charging current.

Also, your motors are reasonably high speed, so you are not losing much from not running FOC. 

Longer ramping time and/or more gradual throttle curve should reduce the number of cutouts as it is very large changes in current that trigger the DRV faults the most. 

I can understand the situation, you want to stop, but put just too much throttle and the ESC cuts out from the rapid change in current, which is why the 4.20 should be used with lower speed and lighter builds. You also have to play around with the braking to make sure you have enough to stop on a dime but not to trigger a fault. I got it to cut out a couple times by slamming the brakes while going downhill, luckily I have a handbrake just for that situation, haha (but it really wasn't needed as I was able to reset the motor controllers and ease up on the brake).
```

---
## \#131 Posted by: mtuan293 Posted at: 2018-11-30T18:20:16.633Z Reads: 180

```
I’ve bypassed the discharge on my BMS, so now the 4.20 can directly draw/charge the 10s pack. It happens across all voltages, from 40V down to 30V. 

I think you’re right, like drastical change in current can throw DRV fault.

Well yeah the motor can still reset, but like in some emergency situation, you’d want it to keep braking instead of releasing the brake for a split second. It actually threw me off balance when I tried to brake, leaned backwards, then suddenly cut out so board kept moving forward, then I fell.
```

---
## \#132 Posted by: BruSkater Posted at: 2018-11-30T18:45:29.862Z Reads: 174

```
So I used @mmaner 's config with @rey8801' smad hubs using the vesc tool. With no load works perfect, but applying a little resistance the motor starts clogging... Any idea of what could be happening? Is there another setting I should look for? I used the vesc tool wizard
```

---
## \#133 Posted by: mmaner Posted at: 2018-11-30T18:52:48.193Z Reads: 174

```
Post screen shots if your config, specifically the BLDC portion.
```

---
## \#134 Posted by: BruSkater Posted at: 2018-11-30T18:55:24.206Z Reads: 171

```
Sure will do later when I am at home! I am using FOC though, is that a problem?
```

---
## \#135 Posted by: mmaner Posted at: 2018-11-30T18:55:44.261Z Reads: 172

```
Definitely.
```

---
## \#136 Posted by: Kug3lis Posted at: 2018-11-30T18:58:03.116Z Reads: 178

```
I was mentioning this all in the beginning that those cheaped ass capacitors will cause some issues.

I suggest someone with skills replace ceramic ones next to current shunts with decent real ceramic capacitors and replace those electrolytes with real stuff at least 2 x 680uF (1360uF)/63V for each side.
```

---
## \#137 Posted by: Kug3lis Posted at: 2018-11-30T18:59:05.357Z Reads: 177

```
If that fixes issues than it's pretty good deal because the caps would be like under 10£
```

---
## \#138 Posted by: BruSkater Posted at: 2018-11-30T18:59:40.631Z Reads: 176

```
Is definitely a problem? I thought it was OK on FOC
```

---
## \#139 Posted by: mmaner Posted at: 2018-11-30T19:29:00.421Z Reads: 173

```
not on low KV motors
```

---
## \#140 Posted by: BruSkater Posted at: 2018-11-30T19:34:00.246Z Reads: 174

```
I'll try BLDC and report back!
```

---
## \#141 Posted by: DAddYE Posted at: 2018-11-30T21:30:34.216Z Reads: 173

```
[quote="Kug3lis, post:136, topic:68940"]
I suggest someone with skills replace ceramic ones next to current shunts with decent real ceramic capacitors and replace those electrolytes with real stuff at least 2 x 680uF (1360uF)/63V for each side.
[/quote]

I should be able to do that. The only annoying thing will be removing the glue :frowning:

Do you have any link with authentic/ quality one for  the US market?
```

---
## \#142 Posted by: BruSkater Posted at: 2018-11-30T23:42:09.887Z Reads: 174

```
@mmaner here are the BLDC screenshots. Havent tested it with load yet, but using my hand it would seem that it will be the same.... I'll assemble it now

![BLDC%201|690x478](upload://osp82f35ZrluIdJypbXv3ph9e2n.png) ![BLDC%202|690x477](upload://k4PVdwmxMAGMaTbXtkxVeylbR9Y.png) ![BLDC%204|690x477](upload://ikWCIiKrkiqWbNICss8WrNI7ftv.png) ![BLDC%203|690x478](upload://q7oekAwe8UVszwmbEOBQnfnwCfu.png)
```

---
## \#143 Posted by: mmaner Posted at: 2018-11-30T23:48:54.654Z Reads: 163

```
Get screen shots of the General tab and take it off Hybrid mode, put it in BLDC mode.  Once you get it running in BLDC you can experiment with FOC, but always get a board up and running in BLDC to rule out amperage and voltage issues.
```

---
## \#144 Posted by: BruSkater Posted at: 2018-11-30T23:55:15.522Z Reads: 176

```
IOt is already in BLDC, and same story, I can easily stop motor wuth my hand, and brakes suck. Here are the general screenshots.... Ima take Hybrid off now, should I go sensorless?![General%201|690x478](upload://h18pHoBbWJjE8lynf0U7rglODuB.png) ![General%205|690x480](upload://bm7Ji3pZcfSeGl6xz8Q4K6RC6U1.png) ![General%203|690x479](upload://707PCHnscgwi3HQEpkZy16B7k5C.png) ![General%202|690x475](upload://1etJmGBbzZetLZDzVLT5uU8c59a.png) ![General%204|690x477](upload://ey1JMHvUi9VjYy56RTZKsIjzEBW.png)
```

---
## \#145 Posted by: mmaner Posted at: 2018-12-01T00:09:37.294Z Reads: 167

```
Yeah, sensorless to start.
```

---
## \#146 Posted by: BruSkater Posted at: 2018-12-01T00:12:07.864Z Reads: 166

```
I did that, is very weak. Doesnt even take off and keeps coggin.... if I push it starts moving and keeps on
```

---
## \#147 Posted by: mmaner Posted at: 2018-12-01T00:12:36.250Z Reads: 168

```
I don't see anything wrong with your setting but I'm looking on my phone. My feeling is that you have a sensor issue. Set it to sensorless and disconnect them then try bldc detection.
```

---
## \#148 Posted by: BruSkater Posted at: 2018-12-01T00:35:08.954Z Reads: 172

```
Setting done, still the same... Here is a video. As a reference I am not able to hold the wheel like that on a Wowgo 2s.

https://youtu.be/vdaboXMo_x4
```

---
## \#149 Posted by: BruSkater Posted at: 2018-12-01T01:23:44.781Z Reads: 171

```
I realized it is just a startup problem.... is there a way to push more current in startup?
```

---
## \#151 Posted by: mmaner Posted at: 2018-12-01T02:00:51.362Z Reads: 171

```
You can increase the startup boost. Have you tried a different motor?
```

---
## \#152 Posted by: BruSkater Posted at: 2018-12-01T02:35:02.981Z Reads: 172

```
Nope, don't have another motor. How to increase startup boost?
```

---
## \#153 Posted by: mmaner Posted at: 2018-12-01T02:50:07.363Z Reads: 172

```
I'll have to look at the VESC tool, don't remember if the top of my head. I'll get back with you in an hour or so.
```

---
## \#154 Posted by: Benjamin899 Posted at: 2018-12-01T15:15:12.229Z Reads: 170

```
When you do the Motor detection you can increase Duty at start ect to make the cogging go away. It should a do a smooth start up and clear smooth stop.
```

---
## \#155 Posted by: Gamer43 Posted at: 2018-12-01T22:00:19.808Z Reads: 173

```
[quote="mtuan293, post:131, topic:68940, full:true"]
I’ve bypassed the discharge on my BMS, so now the 4.20 can directly draw/charge the 10s pack. It happens across all voltages, from 40V down to 30V.

I think you’re right, like drastical change in current can throw DRV fault.

Well yeah the motor can still reset, but like in some emergency situation, you’d want it to keep braking instead of releasing the brake for a split second. It actually threw me off balance when I tried to brake, leaned backwards, then suddenly cut out so board kept moving forward, then I fell.
[/quote]

Ouch, I'm sorry to hear that
The cut-outs during braking will be problematic. I was able to prevent cut-outs on mine using longer positive ramping time and experimenting with the settings, but they ended up being less than ideal for stopping on a dime.

@DAddYE
These look like they'll meet the necessary specifications: 750uF, 31 mohm ESR; two of them will be more than enough.
https://www.digikey.com/product-detail/en/nichicon/UBY1K751MHL/493-17770-ND/9452704
$3 each is not that bad, (except for shipping, argh).
Aside from being twice as long, they should have the same form factor as the existing electrolytic capacitors on the FSESC 4.20.
I don't think the ceramic caps need to be replaced; if there were a problem with them, the ESC would cog on most motors in FOC. 
Looking at the some of the larger ceramic bypass caps, it's hard to tell at first, but they are REALLY tall, and really big.
```

---
## \#157 Posted by: Benjamin899 Posted at: 2018-12-17T13:26:32.656Z Reads: 157

```
then you clearly didnt read this thread.
```

---
## \#158 Posted by: Gamer43 Posted at: 2018-12-18T05:40:27.587Z Reads: 158

```
SOME INSIGHT ON DRV FAULTS

Ok, so I switched out the stock MOSFETs (NTMFS5C628NL) with TPW1R306PL,L1Q.
https://www.digikey.com/product-detail/en/toshiba-semiconductor-and-storage/TPW1R306PLL1Q/TPW1R306PLL1QCT-ND/6188444
It has half the RDSon and twice the gate charge; it is basically equivalent to two NTMFS5C628NL in one package with an exposed topside source pad. 

I was wrong, faults are still occurring; HOWEVER, the nature of the faults did change. 
The current the VESC measures during a fault doubled from 40 filtered, 60 abs to 75-80 filtered, 120 abs.
I tested with an unloaded (and damaged) 6374 TorqueBoards motor from DIYElectric Skateboard.
I could not get the ESC to throw a fault in "current no reverse with brake" but I could get it to throw fault in "current" control mode and instantly going full forward to full reverse.

Pausing for a second in the center would avoid a fault altogether. 

ALSO! before, it would fault on my hoverboard hub motors in the same way; with the new MOSFETS, I can't get the thing to throw a fault. 

+- 60A motor and batt current, although the most it would pull in unloaded condition was 20A motor.

Here's a picture of the dodgy rework.
![20181217_221147%5B1%5D|375x500](upload://ethfjaqkIDjs3WneTT813DGj2ra.jpeg)  

I also doubled checked, the OC_ADJ pin is indeed tied to DVDD, but the change in measured current at fault tells me the DRV8302 is throwing its overcurrent protection fault.......
I doubt it's the DC decoupling capacitors, the VESC reports nominal voltage during fault condition.
I also can't find the GVDD caps, but there appears to be a 47uf ceramic cap on the 3.3v rail. 
But it can't be gate undervoltage since those faults would be throw at random times or all the time; these seem to happen when current changes extremely quickly.

DRV8302 throws faults in three conditions, gate undervoltage/overvoltage, overtemperature, and overcurrent.
Overcurrent protection is done by measure Vds across all actively driven transistors. 
I wish I had a digital oscilloscope, because then I would jerry-rig some probe points and plot the nFAULT signal against GVDD, phase A, and other relevant signals. 

At this point, the significance differences between the FSESC 4.20 and 6.6 is the 6.6 uses discrete highside current sense amplifiers and an SPI enabled DRV8301 instead of the DRV8302. 

Since the embedded lowside current sense amps in the DRV8302 are essentially independent of the main gate driver IC, the only significant difference that would cause the 4.20 to throw DRV faults and not the 6.6 is the DRV chip. 

I might try swapping out the DRV8302 for a different one from Arrow or Digikey, but that will be a real pain in the ass since I don't have a hot air station and only a heat gun. The ground plane in the 4.20 is absolutely huge and I would have to heat gun the thing to both remove and solder in a new one, without any thermal reliefs on the exposed ground pad. Chances are if I try this I'm going to lose passive components or possibly even ruin the STM32 chip.

I'll see if I can ask Flipsky from which electronics distributor they get their DRV8302 from.

EDIT: on second thought, I read on the TI forums that long gate drive traces can cause fault conditions, I need to reexamine the traces to see if this is a possibility.
```

---
## \#159 Posted by: Gamer43 Posted at: 2018-12-31T23:01:47.000Z Reads: 150

```
I apologize for the double post, but I discovered something interesting and would like to share it with you guys.

I now have two FSESC 4.20, one with stock MOSFETs, one with TPW1R306PL,L1Q.

The stock ESC I can get to fault everytime regardless of what VESC settings I try with my TB 6374 motor on the bench.

However, the ESC with the new MOSFETs, I couldn't get it to fault at all on the bench using these settings

+- 40A on everything.

50khz switching frequency (don't try this on a VESC with phase shunts, you'll brick it because the algorithm isn't fast enough).
![2018-12-31%20(1)|690x431](upload://eyfDqxTwNAebClm0rTSZPMYjCRS.png) 
![2018-12-31%20(4)|690x431](upload://A3OFZnPI7CPJT8LpC38Nw0I245K.png) 
![2018-12-31%20(3)|690x431](upload://4lu4nVC3HAubfRIjtsgBUPIZZTK.png) ![2018-12-31|690x431](upload://l3yKHoBxgDFYNg8arxmGgvMYK6F.png) ![2018-12-31%20(2)|690x431](upload://tBkeihyvCmYoZkdQadUXA4b3A6V.png) 


ALSO, on the FSESC 4.20 with the new MOSFETs, I couldn't get it to fault at all in sensorless mode on the bench; however, low speed startup and braking where much slower.

Testing was done at 6S with lipos that can supply 200A.

Looks like some hot air rework and a little crazy VESC settings is what will get the FSESC 4.20 to stop throwing faults xD. (at least, on the bench)

I noticed the faults generally occur at around 20% duty cycle, or right around when senorless mode is supposed to kick in.

My best guess as to what is happening, is during transitions into sensorless mode, the phase angle that the observer calculates is significantly different than the phase angle the VESC was previously using prior to the transition, this happens in both open loop and sensored mode, with the difference being larger at higher RPMs. The result (and because of some quirks in the FOC algorithm) results in a very large (and very brief) current spike in one or more of the phases.
This, in combination with the the very high slew rate (and lower saturation current) of the MOSFETs, I'm guessing is causing a glitch on the phases and triggering the DRV8302 fault.
And this is why you don't see this on 4.12 hardware, since the IRFS7530 has a slew rate ten times slower than the NTMFS5C628NL
```

---
## \#160 Posted by: brenternet Posted at: 2018-12-31T23:29:30.967Z Reads: 146

```
This is great troubleshooting. @BarbaraZ

They've got a new model on the way and hopefully they've managed to isolate these issues
```

---
## \#161 Posted by: kalebludlow Posted at: 2019-01-02T08:55:58.570Z Reads: 146

```
Hey @BarbaraZ I bought a FSESC6.6 during the buy one get one free promotional period, but when the package arrived there was no second unit. Facebook customer service have been unhelpful
```

---
## \#162 Posted by: brenternet Posted at: 2019-01-02T09:42:27.488Z Reads: 148

```
Message them on Facebook. Make your first message as clear as possible.

Name, address, order number, order date. Then the issue as simple and clear as possible.

Just make it really easy for them to help you.
```

---
## \#163 Posted by: kalebludlow Posted at: 2019-01-02T10:05:28.677Z Reads: 146

```
Already have. All they told me was that the free one was shipped with the paid one, which it wasn't.![Screenshot_20190102-210429|236x500](upload://wnQJoLXYxOPmfeBCtGhuasMwpM4.jpeg) 
What they said seemed kinda ambiguous, and leaving me on read doesn't help the situation
```

---
## \#164 Posted by: brenternet Posted at: 2019-01-02T10:09:16.835Z Reads: 143

```
Give it 24hrs haha, they will reply.

The free one might have been shipped separately as well, the convoluted shipping subsidies on mainland China are complicated and it could cost them less to send separately. Just speculation
```

---
## \#165 Posted by: Winfly Posted at: 2019-01-18T10:54:30.446Z Reads: 133

```
Just wondering. What's the max setting ppl have on 4.12? Looking to run 12s on them on a fun 
project. @visnu777 @brenternet 

Also did anyone extra 4.12 from their holiday sale? Or where to get them for cheap?
```

---
## \#166 Posted by: brenternet Posted at: 2019-01-18T11:01:03.849Z Reads: 135

```
My 4.12's are just sitting in a box here but I've not heard of anyone running into issues on 12s FOC with them. I'm sure someone has done it and will read this.
```

---
## \#167 Posted by: visnu777 Posted at: 2019-01-18T14:50:16.074Z Reads: 135

```
I have an internal 10s and an external 2s battery, most of the time I use only the internal one. 12s worked though, without issues.
```

---
## \#168 Posted by: kalebludlow Posted at: 2019-01-18T23:11:23.553Z Reads: 137

```
Cheap FS4.12 https://www.ebay.com.au/itm/FLIPSKY-FSVESC-V4-50A-SK8-ESC-w-5V-1-5A-BEC-for-Electric-Skateboard-RC-Car/132649495953

I use 35A batt max as I get thermal throttling after a while if I go higher than that, but I don't have any sort of heatsink on them
```

---
## \#169 Posted by: mishrasubhransu Posted at: 2019-01-19T13:54:38.054Z Reads: 134

```
What's the use of the 3.3v and 5v switch on the FSESC 6.6?
```

---
## \#170 Posted by: DeathCookies Posted at: 2019-01-19T14:54:19.508Z Reads: 133

```
Some Motor Sensors work in 3,3v and others on 5v. The switch Changes this voltage for the Motor Sensors
```

---
## \#171 Posted by: mishrasubhransu Posted at: 2019-01-31T15:53:04.764Z Reads: 123

```
Has anyone designed a heatsink for fs 6.6 single that can be mounted through the enclosure. For better heat dissipation while being splash resistant.
```

---
## \#172 Posted by: Bardakon Posted at: 2019-02-02T19:32:50.102Z Reads: 122

```
how did you connected the 4.12 together?
```

---
## \#173 Posted by: brenternet Posted at: 2019-02-02T19:45:54.511Z Reads: 127

```
Split PPM personally but you can CANBUS them if you want like any vesc.
```

---
## \#174 Posted by: red Posted at: 2019-02-21T17:50:15.055Z Reads: 108

```
hi im just got the 4.20 and im looking to put the firware on it.
what option did people pick in  hard ware?
```

---
## \#175 Posted by: Benjamin899 Posted at: 2019-02-25T16:10:39.590Z Reads: 105

```
Anyone got a complete BOM for the FSESC 4.12?
```

---
## \#176 Posted by: kchxaz Posted at: 2019-05-02T20:35:16.853Z Reads: 80

```
As of April '19, Flipsky is lacking (extremely important information in my opinion) information on the dual FSESC 6.6 (not the "plus" version) web page. It does not support 4WD. I found this out the hard way and purchased two, since that's what you need for 4WD, to the tune of about $600 and when they arrived I couldn't figure out how to seet up 4WD so I contacted Flipsky and they informed me that you need to buy the plus version. I was furious, I had been messaging him back and forth previous to that about this very thing so he knew what me goal was yet neglected to tell me this important fact. When I called him on it I was ignored. So now my board is a fail and I'm out $600. I had read many reviews by forum members, was even suggested NOT to go with a Flipsky ESC, but I wanted to prove the naysayers wrong - and I'm a cheap ass.  And look what happened? 

I would not recommend buying anything from that jackoff ever.

To be fair as far as two wheel setup goes, the FSESC works well, so far as I can tell. Still, the fact that Flipsky doesn't support his product is reason enough for me to never buy from him again in the future.
```

---
## \#177 Posted by: brenternet Posted at: 2019-05-02T21:20:16.344Z Reads: 79

```
Flipsky isn't a person. The esc's work well.

You had a bad experience, that's unfortunate but I'm not sure the turborage is worth it. Sell your $600 esc's for $550 and buy the plus ones. Problem solved.
```

---
## \#178 Posted by: RedBaron Posted at: 2019-05-02T21:26:49.994Z Reads: 80

```
Or you can just canbus them together. I've seen a picture of how to make it work somewhere here on the forums. Then split ppm them and presto it works. Just takes some know how is all.
```

---
## \#179 Posted by: kalebludlow Posted at: 2019-05-02T22:31:05.831Z Reads: 77

```
Yeah the issue with everything you've said here is that it is 100% possible to run 4WD with these ESCs. Just because you aren't capable of doing so doesn't mean that 'Mr Flipsky' is in the wrong. You were also told to not buy Flipsky, and you did anyway. You dug this hole, you get yourself out
```

---
## \#180 Posted by: Pmac Posted at: 2019-05-02T23:43:34.046Z Reads: 75

```
Hi Kerry,

You are incorrect.  You can run 4WD with 2x Dual FSESC 6.6.

There is no port for the CAN but you can solder 2 wires and get the port.

Here is an image from flipsky I received when I asked them about it.

I hope this helps.

![46444573_2048271948563802_4675679029683027968_n|690x321](upload://qm0SAYRmZZTkFMi1SGsgjMWNQCB.jpeg)
```

---
## \#181 Posted by: kchxaz Posted at: 2019-05-03T00:21:43.729Z Reads: 76

```
Pmac,

Thank you for the _contsructive_ criticism and having class, something a few members of the forum lack completely taking cheap jabs and repeating the obvious - whatever. I appreciate you taking the time to respond with something helpful.

I'm not sure I follow with the diagram though. Is it saying to solder the two opposing "pin" looking things on the can switch from each FSESC?

And I truly don't mean this to sound rude or challenging but there's no other way to ask it: Why would the person at Flipsky tell me that the FSESC 6.6 can't run 4WD when they clearly provided you with a "how to" to make that happen? How recent is your information? Thanks!
```

---
## \#182 Posted by: brenternet Posted at: 2019-05-03T00:32:42.316Z Reads: 75

```
The spot exists on the board but to make this esc as inexpensive as possible they didn't solder the port on. For at least some of their CS team it's likely easier to just tell people it's not possible.

 The only post here relating to your issues that lacks class is your initial one.
```

---
## \#183 Posted by: Pmac Posted at: 2019-05-03T01:24:17.404Z Reads: 71

```
Hi Kerry,

That info was from 19/11/2018.  It may have been a different person responding now who may not be aware.

When it comes to CAN wiring they are all wired in parallel to each other.

The switch on the ESC is for the CAN so you can connect and disconnect the CAN depending on whether you want the pair to communicate or not (there are use cases where you want them to be independent but still require 2).

here is another image they sent me.

![46463184_233150697586651_4966375387077541888_n|640x480](upload://oRtRWal09wkJO7nmJvfcT15ePKe.jpeg)
```

---
## \#184 Posted by: danieloath Posted at: 2019-05-03T02:14:36.978Z Reads: 69

```
If you create a poll on their Antisparks, that should assist with informing choices. I had 2 Antisparks. First one was DOA and the replacement refused to turn off after one ride.
```

---
## \#185 Posted by: kchxaz Posted at: 2019-05-03T21:17:26.890Z Reads: 59

```
Brent - thank you for the background, that makes more sense. Doesn't help with my issue but it explains the why.

I had a negative experience with Flipsky that ended up costing me a grip of money and I'm entitled to my opinion based off of those facts, which I believe is what the point of this post is about. 

But thanks for the background on the ESC situation.

Pmac, that was well before I got the information that I heard. And thank you for the pics. If this works I owe you a beer!
```

---
