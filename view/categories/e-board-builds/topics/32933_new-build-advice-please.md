# New Build - Advice, Please!

### Replies: 65 Views: 2925

## \#1 Posted by: buckhr Posted at: 2017-09-12T03:53:03.688Z Reads: 276

```
Hi All!  First time builder here, looking for some confirmation components before I buy.  I'm going relatively budget, trying to get this first board running as a starter board and eventually working into more complex builds.  Im wanting to use this board as a mountainboard, or at least be able to handle the stiff transitions here in Indiana and do some light offroading. 
 Im open to modifying the suspension and board later as necessary to achieve more cushion and ride comfort.  Here are the components I've already got and/or considering buying:

Board: hand-me-down longboard from a friend, seems completely wooden and relatively heavy for my set up but worth it for $0 and where Im at.  :)  Also came with Paris trucks and bushings.  I added "1 polyurethane risers to the trucks to account for the added wheel diameter (described below).

Wheels: 113mm from [this thread](http://www.electric-skateboard.builders/t/anyone-tried-to-use-these-rubber-offroad-wheels/30947/36).  I have them mounted and have realized they are definitely too hard for a true mountainboard ride, but they are sufficient for now and I may drill holes through them later in an attempt to get more cushion.  Ultimately, if I stick with this board long term Ill replace the wheels with something more robust.

Pics of board as it sits currently:
[Pic 1](https://photos.app.goo.gl/sFf0Fujz6l9aRyJA2)
[Pic 2](https://photos.app.goo.gl/woxdow7EAdcPVYu32)
[Pic 3](https://photos.app.goo.gl/Zfhf04XmtsT2GDjP2)

Drivetrain mounts: I decided on [this kit from Ebay](http://www.ebay.com/itm/Electric-Skateboard-Longboard-Kit-Pulleys-And-Motor-Mount-for-80mm-Wheel-OS914/371996513753) after using the RC Calc app to determine ultimate drive ratio and top speed based on some assumptions about battery and motor (below).  The teeth are 16T and 48T, though the pitch angle is not mentioned.  Since we're talking a 4x reduction and a relatively large motor gear, I figured this will be sufficient and cost effective.

Motor: Im wanting to start with a dual motor setup, so Im intending to go lower on KV.  Im thinking [two of the 190kv Turnigy motors from Hobby King](https://hobbyking.com/en_us/turnigy-aerodrive-sk3-6364-190kv-brushless-outrunner-motor.html?___store=en_us) should be good, but interested in feedback on KV, Turnigy, and Hobby King.

Battery: With two motors, and wanting decent range, I am thinking 10S based on further reading and using the RC Calc at 48V.  Possibly [this battery](http://www.ebay.com/itm/ZIPPY-COMPACT-4000mAh-10S-37V-25C-35C-LIPO-BATTERY-HXT-4MM-QUAD-HELI-EBIKE-MULTI-/272813733688?hash=item3f84f73738:g:4n0AAOSwrRlZmh8C)?  Open to ideas or feedback on upgrading to 12S?

VESC: It seems like there's a lot of options and not a lot of quality feedback on what VESC to use.  Im thinking 2x of [these Maybach-based VESCs from Ebay](http://www.ebay.com/itm/302200711613).  Thoughts?

[RC Calc pic](https://photos.app.goo.gl/mjKLdpInDjOalRva2)

Ive got [this Watt Meter from Amazon](https://www.amazon.com/gp/product/B06Y5DDK6N/).  

What else do I need?  What am I missing?

Thanks so much in advance!
```

---
## \#2 Posted by: thisguyhere Posted at: 2017-09-12T04:19:39.836Z Reads: 241

```
forget where but remember seeing someone complaining about slippage with those 3mm pitched pulley / belts. overall that drive kit doesn't seem to be very good but they are cheap. 

basic tooling wise you'll need a solder station, I use the hakko 888. 

those cheap vescs should be ok as long as you bldc, not foc. 

as for those wheels you'll probably have to drill holes to make the pulley fit, not sure
```

---
## \#3 Posted by: cwazy1 Posted at: 2017-09-12T05:04:51.460Z Reads: 222

```
if the maytech's are $100 each, why not just get TB's VESC? at least that way you'll have a real american company who is active on the forums backing the product.
```

---
## \#4 Posted by: marcmt88 Posted at: 2017-09-12T05:24:20.195Z Reads: 204

```
Don't think paris truck can accommodate dual 190Kv turnigy motors.  Take a look at my dual 6374s mounted on TorqueBoards 218mm truck:

<img src="/uploads/db1493/original/3X/7/c/7c6867bf586112f6a931a6f2a0448d1246599d47.JPG" width="666" height="500">
```

---
## \#5 Posted by: buckhr Posted at: 2017-09-12T16:06:23.506Z Reads: 186

```
I cant actually tell if these are 3mm or 5mm pitched - do you see that somewhere?  Maybe Im missing it...

Ive got soldering stuff from other projects, but good call out thanks!

Sorry, newbie question: what is bldc vs foc?

Yes, definitely going to modify the wheels for the pulley.  

Thanks for the reply!!
```

---
## \#6 Posted by: buckhr Posted at: 2017-09-12T16:06:41.022Z Reads: 169

```
Do you have a link to TB's VESCs?
```

---
## \#7 Posted by: Zimbombe Posted at: 2017-09-12T16:19:28.894Z Reads: 168

```
I've seen some of these motor mounts broke in 2 pieces in some threads, maybe not the best choice.

I've bought this one which is also not top notch quality but at least looks more stable to me. But check if it can hold your motor and suits your trucks.

Electric Skateboard Belt Motor Mount Bracket Pulley Screws For 83/90/97MM Wheel
https://banggood.app.link/JDkAxjOTnG
```

---
## \#8 Posted by: buckhr Posted at: 2017-09-12T16:21:05.921Z Reads: 165

```
Thats a great call out, I hadnt yet thought about clearances between the motors.  Im not sure exactly how to measure the length of the trucks; they are either ~186mm or ~254mm depending on where you measure from:

[Measured from threads](https://photos.app.goo.gl/KF98W8BrzBTEqd5p2)
[Measured from shaft start](https://photos.app.goo.gl/9p9OptlhZNAhUz1F2)

Just eyballing it, you're right that there isnt going to be enough room to mount the motors symmetrically as you have.  I do have quite a bit of ground clearance though, so Im thinking Ill either stagger them or mount them on opposite sides of the truck.  Does that sound reasonable to you?

What is the difference between your 6374s and the 6364s I linked?  Reading the product descriptions, it seems like the 6374s can handle 10S - 12S, where the 6364s can only handle 10S.  Is that the only difference?

Thanks for the reply!
```

---
## \#9 Posted by: buckhr Posted at: 2017-09-12T16:30:13.252Z Reads: 150

```
Thanks for the recommendation!  Ill give these a consideration.  In first glance I like the fact that the ones you have a  19mm bracket hole for the trucks vs the 18mm hole in the ones I have; my trucks are _slightly_ over 18mm, which means Ill need to shave/file them down slightly to fit my current brackets.  Ill have to do that anyway though, because the Paris trucks are pretty heavily chamfered from the axle to the mount meaning Ill need to clear some of the metal out anyway.  I also like that the ones you linked come with a mounting bracket for the wheel gear on the opposite side of the wheel vs the ones I have do not have this.  The final drive ratio with 12/36T vs 16/48T would be just fine as well.

I dont like the price though... :frowning: plus the fact that I already bought these.
```

---
## \#10 Posted by: marcmt88 Posted at: 2017-09-12T16:36:04.716Z Reads: 139

```
6374s has a length of 74mm vs 6364s of 64mm.  63xx designates the diameter of 63mm.
```

---
## \#11 Posted by: cwazy1 Posted at: 2017-09-12T17:04:31.926Z Reads: 135

```
diy-electric-skateboard-kits-parts/vesc-the-best-electric-skateboard-esc/
```

---
## \#12 Posted by: thisguyhere Posted at: 2017-09-12T17:31:57.273Z Reads: 140

```
[quote="buckhr, post:5, topic:32933]
I cant actually tell if these are 3mm or 5mm pitched - do you see that somewhere?  Maybe Im missing it...
[/quote]

in the ebay post, product photos, that 3m designation indicates pitch depth.

[quote="buckhr, post:5, topic:32933]
Sorry, newbie question: what is bldc vs foc?
[/quote]

a search will get you your answer:

http://www.electric-skateboard.builders/t/vesc-faq-what-is-foc-field-oriented-control/419

[quote="buckhr, post:5, topic:32933]
Yes, definitely going to modify the wheels for the pulley.  
[/quote]

i'd recommend against this.  unless you have a drill press for perfect angles, just get abec core wheels so things just fit together without having to modify things by hand.
```

---
## \#13 Posted by: buckhr Posted at: 2017-09-12T19:48:29.408Z Reads: 120

```
Sweet, thanks for the info, that makes sense.
```

---
## \#14 Posted by: buckhr Posted at: 2017-09-12T19:48:44.643Z Reads: 117

```
Thanks!  Ill probably get these instead ;)
```

---
## \#15 Posted by: buckhr Posted at: 2017-09-12T19:54:40.151Z Reads: 123

```
[quote="thisguyhere, post:12, topic:32933, full:true"]
in the ebay post, product photos, that 3m designation indicates pitch depth.
[/quote]

Thanks, I see it on the belt now.  

[quote]

a search will get you your answer:

http://www.electric-skateboard.builders/t/vesc-faq-what-is-foc-field-oriented-control/419
[/quote]

Of course, the search feature... so obvious, yet so noob.  Thanks!

[quote]
i'd recommend against this.  unless you have a drill press for perfect angles, just get abec core wheels so things just fit together without having to modify things by hand.
[/quote]

I do indeed have a drill press, so Ill be using it.
```

---
## \#16 Posted by: cwazy1 Posted at: 2017-09-12T20:11:35.665Z Reads: 110

```
yeah definitely, TB VESC is 2 subversions ahead of maytech's 4.10. I still wouldn't do FOC, instead just stick with BLDC.
```

---
## \#17 Posted by: buckhr Posted at: 2017-09-13T14:18:37.795Z Reads: 105

```
[quote="cwazy1, post:16, topic:32933, full:true"]
yeah definitely, TB VESC is 2 subversions ahead of maytech's 4.10. I still wouldn't do FOC, instead just stick with BLDC.
[/quote]

I just ordered two of TB's ESCs... the money pit gets deeper!
```

---
## \#18 Posted by: cwazy1 Posted at: 2017-09-13T17:40:16.833Z Reads: 102

```
Just wait until you start breaking parts and frying chips.. I thought I was going to stop at 1100$ for my single build. Then the second motor, then fried a drv, etc. etc. fuck this hobby.
```

---
## \#19 Posted by: buckhr Posted at: 2017-09-13T19:04:39.790Z Reads: 109

```
[quote="cwazy1, post:18, topic:32933, full:true"]
Just wait until you start breaking parts and frying chips.. I thought I was going to stop at 1100$ for my single build. Then the second motor, then fried a drv, etc. etc. fuck this hobby.
[/quote]

Yes, I already decided on different wheels instead of the ones Ive bought and paid for.  These look more promising: http://www.diyeboard.com/6-15050mm-70a-allterrain-offroad-skateboard-wheels-p-568.html.  Id be better off financially just buying the entire board from them at this point, but its about the experience, right?  RIGHT?  :slight_smile:
```

---
## \#20 Posted by: cwazy1 Posted at: 2017-09-13T19:35:15.274Z Reads: 104

```
You'll have to let me know how you like those wheels... They're really quite appealing now that they're made with 8mm axles. I wonder if it will be as soft as pneumatics.
```

---
## \#21 Posted by: buckhr Posted at: 2017-11-13T22:38:43.561Z Reads: 86

```
So, after a long ordeal with the manufacturer, I swapped the wheels out for regular 10" pneumatics.  The 8" rubber wheels were nice enough on visual inspection, but I never got to use them for a number of reasons and moved on.
```

---
## \#22 Posted by: buckhr Posted at: 2017-11-13T22:44:25.903Z Reads: 92

```
I need some more help please!  I ordered a number of parts from www.diyeboard.com - good guys to work with, they helped swap some parts around with other customers in the US instead of paying for expensive shipping to China! - including this battery which came with charger: http://www.diyeboard.com/10s5p-18650-lithium-battery-pack-36v-10ah-360wh-p-460.html

However, I cant figure out how to connect the battery to the charger?  I see the connectors are different, but Im totally unsure how to wire them up together.  Ive searched and found info on building a loop key for charging, which I think I can do, but that is only part of the problem.  Any help?

Also, Ive read somewhere that I shouldn't program the VESC with the 10S battery, and need something with less amps... is that right?  I bought two of the Torque VESCs which according to the product description come pre-booted and dont need the initial startup amp protections, but what about using the 10S battery for programming as well?

Thanks!
```

---
## \#23 Posted by: mmaner Posted at: 2017-11-13T23:02:48.076Z Reads: 83

```
I would assume the open connector is for the power switch, but it may be the charge port.  Either way, you can solder one into the XT60 connector.
```

---
## \#24 Posted by: buckhr Posted at: 2017-11-16T21:01:58.985Z Reads: 91

```
Thanks!  Im sure the connector is for the charge port, but Im not sure what you mean by "solder one into the XT60 connector" - is there a diagram somewhere that describes this?

Here's my connector on the charger: https://photos.app.goo.gl/0NWFU0cxKnl0wOEd2
```

---
## \#25 Posted by: mmaner Posted at: 2017-11-16T23:45:48.971Z Reads: 91

```
You need to get the female side for that charger and solder it onto the charge leads on the battery pack.  Its probably a 5.5x2.1mm socket.

https://www.ebay.com/itm/10X-Waterproof-5-5-x2-1mm-DC-Socket-Power-Jack-Plug-Female-Mount-Connector-Best/111889160001?ssPageName=STRK%3AMEBIDX%3AIT&_trksid=p2060353.m2749.l2649

You can use this diagram for reference maybe.  
<img src="/uploads/db1493/original/3X/1/6/165e3937454525d36d984803b5984bb83a34c11d.jpg" width="687" height="500">
```

---
## \#26 Posted by: buckhr Posted at: 2018-02-14T14:39:53.548Z Reads: 79

```
Update: Ive got the electronics sorted out and the VESC connected to the BLDC tool.  It was a PITA figuring out how to get the BLDC tool to work in Windows, and I made a small post on how to do it in the FAQ section here: [link](http://www.electric-skateboard.builders/t/new-vesc-user-read-this-complete-walktrough-of-the-vesc/2980/154)

Motors I used, 2x of http://www.diyeboard.com/180kv-n6354-outrunner-motor-2000w-for-diy-electric-skateboard-p-540.html
Battery http://www.diyeboard.com/10s5p-18650-lithium-battery-pack-36v-10ah-360wh-p-460.html

I can make the motors move, but they are moving a bit erratically.  It seems like there isnt enough power getting to the motors, as the board will move without me standing on it but if I stand on it there isnt enough torque to move my weight.  

Here's my VESC settings:
![image|690x407](upload://jTyFJTvoYfcjLKEihYIt2JdpOrI.png)
![image|690x407](upload://nQqUpsr5A0rewFTrHzgfC6DwjDO.png)

Is there something blatantly incorrect in these settings?  Any help appreciated!
```

---
## \#27 Posted by: buckhr Posted at: 2018-02-14T15:12:49.724Z Reads: 68

```
Im concerned about the erpm settings given my motor KV, but I dont quite know what to do with them.
```

---
## \#28 Posted by: TarzanHBK Posted at: 2018-02-14T15:32:18.359Z Reads: 67

```
set it to 60k max. Your motors are not the best to work with 10s.. they are too high
```

---
## \#29 Posted by: buckhr Posted at: 2018-02-14T15:41:07.901Z Reads: 67

```
thanks for the advice!  Ill set the max erpm to 60k.  Do you have advice on the min erpm?

Yeah, I realize now that the 270kv motors were too high, but it's what Ive got for now.  I can upgrade to 12s later.  What are the downsides of running higher KV motors on 10s?  Can I mitigate the risks with VESC settings?
```

---
## \#30 Posted by: buckhr Posted at: 2018-02-14T15:53:29.337Z Reads: 64

```
ACK, I posted the wrong motors... these are the ones I have: http://www.diyeboard.com/180kv-n6354-outrunner-motor-2000w-for-diy-electric-skateboard-p-540.html (180KV).  I had originally ordered the 270kv motors but returned them because of this reason.
```

---
## \#31 Posted by: ZackoryCramer Posted at: 2018-02-15T00:26:26.093Z Reads: 58

```
[quote="buckhr, post:1, topic:32933"]
Possibly this battery?  Open to ideas or feedback on upgrading to 12S?
[/quote]

Cough _use sam. 30Q_ Cough
Uh you would want those in parallel which would then give you ~18miles(9 miles is just not enough). Use 12s if you want higher speed potential. And remember more packs = more range. Arrangements don't matter.
```

---
## \#32 Posted by: buckhr Posted at: 2018-02-15T01:08:15.211Z Reads: 59

```
> Cough use sam. 30Q Cough

Sorry, but Im not sure what this means?

I also went with the 10S battery already, so no need to revisit that decision for now :slight_smile:
```

---
## \#33 Posted by: ZackoryCramer Posted at: 2018-02-15T01:13:06.198Z Reads: 52

```
Samsung 30Q's are 18650 lion cells. Compared to lipos', they have lower capacity degradation, safer, and cheaper(for the long run). The only draw back is voltage sag which can be remedied by using bigger parallel blocks. If you ever need to replace your lipos' think 18650 packs first. :wink:
```

---
## \#34 Posted by: buckhr Posted at: 2018-02-15T01:55:41.202Z Reads: 54

```
Thanks, but Im still confused: the battery I bought is made of 50 cells of 18650s: http://www.diyeboard.com/10s5p-18650-lithium-battery-pack-36v-10ah-360wh-p-460.html

I dont actually know how many cell packs that is though, and it's not listed on their site.  Ive asked but yet to receive a response
```

---
## \#35 Posted by: buckhr Posted at: 2018-02-15T02:53:26.708Z Reads: 58

```
Im getting closer, but struggling with the VESC set up.  I am able to spin both motors when the board is not under load (when Im not standing on it), but when I do stand on it the motors feel like they are "shuttering" for lack of a better term.

Also, my realtime data graph looks like this:

![image|690x397](upload://AiuW6cBeG5k7APWVeUeee8k5STJ.png)

I feel like this is abnormal - anyone have an idea what settings are incorrect which are causing this behavior?

Thanks!
```

---
## \#36 Posted by: bsancken Posted at: 2018-02-15T03:20:29.881Z Reads: 53

```
You mean you just stand on the board and expect it to go? You gotta give it a push in the right direction, otherwise you'll expirence cogging
```

---
## \#37 Posted by: buckhr Posted at: 2018-02-15T03:23:59.459Z Reads: 50

```
Oh damn, no way.  I just assumed... sigh.  I have limited space in my current workroom so Im not able to do that in here, which is why I didnt think of it.  Ill have to take it outside and give a try, strapping down the components for now until I build an enclosure.

Any thoughts on the graph data?
```

---
## \#38 Posted by: buckhr Posted at: 2018-02-15T03:27:07.307Z Reads: 50

```
Yeah, that worked alright... a little nudge and the board went flying out from under me and left me on my ass!  It seems like its going 0 - 100 instantly
```

---
## \#39 Posted by: bsancken Posted at: 2018-02-15T03:45:21.354Z Reads: 47

```
Yup, its an art to get goin slowly! From my understanding you need to make it a sensored motor to get the cogging to atleast be mitigated. I have sensors I need to put on this weekend to try that out. Basically wothout the sensors, it doesn't know that the motor issn't spinning so it doesn't ramp up the power to get you initially moving.
```

---
## \#40 Posted by: buckhr Posted at: 2018-02-15T04:47:25.174Z Reads: 47

```
Annnnd I think I somehow just fried a VESC... isnt responding to power like the other one or as it was a few minutes ago... shit.
```

---
## \#41 Posted by: b264 Posted at: 2018-02-15T04:49:02.530Z Reads: 49

```
[quote="buckhr, post:29, topic:32933"]
Yeah, I realize now that the 270kv motors were too high, but it’s what Ive got for now.  I can upgrade to 12s later.  What are the downsides of running higher KV motors on 10s?  Can I mitigate the risks with VESC settings?
[/quote]

No, you need to go down to 8S
```

---
## \#42 Posted by: b264 Posted at: 2018-02-15T04:50:29.089Z Reads: 51

```
[quote="bsancken, post:36, topic:32933, full:true"]
You mean you just stand on the board and expect it to go? You gotta give it a push in the right direction, otherwise you’ll expirence cogging
[/quote]

You can do that if it's a sensored motor and you're in BLDC hybrid mode
```

---
## \#43 Posted by: buckhr Posted at: 2018-02-15T05:03:26.680Z Reads: 47

```
Yeah, I posted that I have 180kv motors, not 270kv.  My bad!
```

---
## \#44 Posted by: buckhr Posted at: 2018-02-15T05:35:33.883Z Reads: 52

```
Where did you get the sensors?  Are they compatible with any motor?
```

---
## \#45 Posted by: ZackoryCramer Posted at: 2018-02-15T05:53:11.701Z Reads: 53

```
Sensors are supposed to come with the motor. You can install hall sensors by yourself if you know what you're doing. :thinking:
```

---
## \#46 Posted by: ZackoryCramer Posted at: 2018-02-15T05:59:37.891Z Reads: 58

```
Post a picture of the fault code if any, then you can tell what's going on.
![Capture2|690x410](upload://l8Sc9K09hk3wIeEJVEDNTIXRhY.PNG)
```

---
## \#47 Posted by: buckhr Posted at: 2018-02-15T06:38:49.245Z Reads: 57

```
No fault codes, it won't even power on
```

---
## \#48 Posted by: ZackoryCramer Posted at: 2018-02-15T06:41:54.530Z Reads: 59

```
Did you connect the Vesc using the xt90? Do the leds light up? You can go to the diyesk8 website and ask them directly.
```

---
## \#49 Posted by: b264 Posted at: 2018-02-15T06:42:00.769Z Reads: 55

```
Measure the voltage on the input wires, what's it say
```

---
## \#50 Posted by: buckhr Posted at: 2018-02-15T07:07:08.862Z Reads: 55

```
LEDs do not light up anymore :frowning:
```

---
## \#51 Posted by: buckhr Posted at: 2018-02-15T07:07:59.433Z Reads: 52

```
Input from the battery?  That's not the problem, the other vesc still works. Maybe I'm misunderstanding
```

---
## \#52 Posted by: pat.speed Posted at: 2018-02-15T11:09:04.896Z Reads: 48

```
I think he is testing to make sure that Vesc is getting power
```

---
## \#53 Posted by: bsancken Posted at: 2018-02-15T18:43:21.112Z Reads: 46

```
Not to get off topic, but these are the sensors if OP ends up going that route..

@ZackoryCramer @buckhr http://e0designs.com/products/hall-effect-sensor-board/
```

---
## \#54 Posted by: Acido Posted at: 2018-02-15T19:28:18.381Z Reads: 48

```
I have it, its not so good...
```

---
## \#55 Posted by: buckhr Posted at: 2018-02-22T05:12:24.360Z Reads: 39

```
I believe that Ive burned my canbus on one VESC, but the other is still functional so I ordered a new one and it arrived today.  I went to hook up the connections and no variation of settings in BLDC tool worked to get the 2nd motor moving.  I can move both motors independently, but cant move both at the same time using canbus.

So I tried the split ppm approach.  This seems to work at times, but I just took the board out for the first test ride (!) down the street and when I returned I noticed only one of the motors was moving.  I reset the config, double checked and rebooted the VESC to the non-working motor and it started moving again.  

However, now one motor seems to move/continue spinning slight more than the other.  It's almost like one motor is experience more resistance (mechanical or electrical, Im not sure which yet) and starts later / stops sooner than the other.  Im not sure yet, but it seem like this mismatch of motor rotation may have caused one  to stop working altogether in my short (~500 ft) ride down the street and back.

Any ideas?
```

---
## \#56 Posted by: mmaner Posted at: 2018-02-22T05:15:46.088Z Reads: 36

```
2 motors will never rotate at the same speed without a load.  Too many factors, belt drag, voltage delivery, wheel and pulley weights, etc. You have to test with a load on it to get practical results. 

Have you set the IDs on the VESC's so that can bus can operate correctly. There's a few guides on how to do this, hit up the search bar. I'd link them for you but just got home from.work, late night, tired...
```

---
## \#57 Posted by: buckhr Posted at: 2018-02-22T05:18:58.678Z Reads: 38

```
Here's a video of the behavior: https://www.youtube.com/watch?v=s4U-tZBbZOs

Yes, Ive followed directions on the various threads on setting IDs, setting the "send over can" settings, etc. and still no luck :frowning:  I had it working prior to (stupidly) frying the canbus on at least one VESC...
```

---
## \#58 Posted by: mmaner Posted at: 2018-02-22T05:21:38.916Z Reads: 36

```
Sounds like you've got more than canbus issues if split ppm is also giving you trouble. I'd check your wiring with a multimeter for resistance and continuity.
```

---
## \#59 Posted by: buckhr Posted at: 2018-02-22T05:23:38.626Z Reads: 34

```
one thing that is odd: I have a loop key, but whjenever I plug it in there is a visible spark/pop in the connector.  is that normal?
```

---
## \#60 Posted by: mmaner Posted at: 2018-02-22T05:24:32.165Z Reads: 35

```
Nope, a xt90-s shouldn't spark. Does it have the green stripe?
```

---
## \#61 Posted by: buckhr Posted at: 2018-02-22T05:24:55.668Z Reads: 36

```
Im using xt60s because that is what came on the battery.
```

---
## \#62 Posted by: mmaner Posted at: 2018-02-22T05:26:41.739Z Reads: 37

```
You need an anti-spark, quick before you turn shit up 😀
```

---
## \#63 Posted by: buckhr Posted at: 2018-02-22T07:06:35.379Z Reads: 35

```
I'm on it, already ordered a set of xt90 antispark connectors from Amazon.
```

---
## \#64 Posted by: buckhr Posted at: 2018-02-23T07:03:23.109Z Reads: 34

```
I'm up and running on split y ppm for now. Im going to take another stab at can fwd set up this weekend, resetting everything to default to see if I can it working again. 

There is so wobble in the drivetrain that I need to sort out as well. 

Vid for those interested: https://youtu.be/luGAGlFkE5g
```

---
## \#65 Posted by: b264 Posted at: 2018-02-23T07:11:33.587Z Reads: 33

```
Make sure you always plug in the anti-spark XT90 all the way, and not just almost all the way.  Otherwise you will burn up the resistor.
```

---
