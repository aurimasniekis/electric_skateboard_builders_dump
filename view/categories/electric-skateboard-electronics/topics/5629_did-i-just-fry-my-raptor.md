# Did I just fry my Raptor?

### Replies: 57 Views: 4523

## \#1 Posted by: Adam0311 Posted at: 2016-07-06T00:28:14.827Z Reads: 276

```
I've been the proud owner of a dual Raptor for about four months. I've had no issues with it...until about a week ago, then began a sequence of events that has me fearing its fried. To best explain let me start with a quick chronology:

1.) June 26th - board randomly shuts down while riding over rough surface. Turn off/on, board fires back up, no issues rest of day.
2.) June 27th - while riding the board shuts down and won't turn back on. Power switch on space cell is very loose. Upon further investigation, it appears the battery shifted which jammed the power switch against the opening in enclosure lid causing it loosen and fail. 
3.) June 30th - thinking this would be a relatively easy fix, I order new power switch (this one http://www.ebay.com/itm/5Pcs-2-Pin-On-Off-SPST-Round-Rocker-Switch-AC-10A-125V-6A-250V-Black-/262209348826?_trksid=p2141725.m3641.l6368 ) and remove old switch and solder (I suck at soldering) in the new one. The new switch is virtually identical to old, but the prongs are a bit longer. I snip the prongs shorter so it lays flush on space cell like the old switch. Switch works, board powers up and seems fine. Only difference is the lcd screen blinks once when switched on. Test ride around block is good to go, no issues.
4.) July 3rd - 
A) riding board to breakfast, take off from stoplight with a kick push then throttle like normal, accelerate to about 15mph and suddenly the brakes (or brake) slams on, I do a poor superman imitation and earn some minor road rash. Get up, look at the board, it's off and won't turn back on. One motor seems to have heavy resistance (attached to slave VESC) while the other has normal rolling resistance. 
B) Walk home, pull space cell out and disconnect from board, turn on and it powers up like normal, plug back into board and it shuts off. Happens multiple times. Plug fast charger into space cell while battery is connected to board and get a decent size spark.
C) decide to try different battery. Plug in @torqueboards 12s battery (used with board before without problem) get a fairly big spark at xt60 connectors. 
D) pulled new space cell switch. Soldering is ugly, but seems solid. decide to seek help before I melt my board.
My questions:
Am I correct to assume there is a short somewhere in board and not battery?
Could poor soldering in power switch to battery lead to a short in board?
Are my VESCs likely fried?
Would a short in one of the motors cause this? 
Greatly appreciate any feedback.
```

---
## \#2 Posted by: sl33py Posted at: 2016-07-06T00:31:40.927Z Reads: 263

```
Ugh - suck man.  have you contacted @EnertionSupport to see steps they suggest?  They build it, they can help.  Might be worth taking some pics to show them.

Best of luck!!
```

---
## \#3 Posted by: Jinra Posted at: 2016-07-06T00:33:35.901Z Reads: 262

```
The spark is indicative of a short, while the behavior sounds like a faulty BMS. I'd do as @sl33py suggested and email Enertion Support.
```

---
## \#4 Posted by: Adam0311 Posted at: 2016-07-06T00:34:09.306Z Reads: 256

```
not yet. I'll load some pics when I get home tonight.
```

---
## \#5 Posted by: sl33py Posted at: 2016-07-06T00:37:17.771Z Reads: 248

```
i would test VESC and motors directly - eliminate all variables.

edit - spark.  Depending how big, that may be normal.  When connecting 12s without an anti spark connector they can give off quite a big spark.  Now if it's melting/slagging the connector that sounds like a short...  I'm not sure, but i thought the SPACE cell had anti-spark built in?

Take your known good DIYes 12s battery - a single VESC, and a single motor.  Can you get it to work on the bench?

Swap motors and VESC's to see if any VESC or motor doesn't work correctly.  Since the SPACE cell was your culprit **_i'd set it aside until enertion replies and you show pics to troubleshoot._**  

But i'd also be worried of damaging VESC and motors.  If a motor acts oddly on both VESC's it might be bad, but i'd also connect up BLDC tool and look for errors on VESC.  Hopefully something simple if there is an issue - something like swapping the DRV chip which is doable (not for you if you suck an soldering) vs just simply fried.

Will be following and fingers crossed it's an easy fix man!
```

---
## \#6 Posted by: Adam0311 Posted at: 2016-07-06T00:44:04.428Z Reads: 230

```
Really appreciate the feedback. I'm gong to try the BLDC tool and take some pics tonight.
```

---
## \#7 Posted by: Namasaki Posted at: 2016-07-06T02:46:09.781Z Reads: 224

```
when you disconnect the battery, did you check spin resistance of the motors again. Because if the phase wires are shorted inside or outside the motor, then it will seem like the brakes are on. I mean you can unplug the motor and touch 2 of the phase wires together and it will cause resistance like the brakes are on.
So if you have brakes when the motor is disconnect, then you have a motor short. If the brake releases when you unplug from the esc then you may have a short in the esc.
I experienced a similar situation once when I fried one of my esc's
```

---
## \#8 Posted by: Namasaki Posted at: 2016-07-06T02:48:31.450Z Reads: 219

```
You said the battery worked fine when it was disconnected from the Vesc's so I'm guessing your problem is not the switch or the battery but either the Vesc or motor or wiring in-between.
```

---
## \#9 Posted by: Skitzor Posted at: 2016-07-06T05:37:40.477Z Reads: 214

```
Yes, do the steps mentioned above, it's what I did when I had motor trouble with my dual ( space cell was fine though). 

The first gen motors don't have isolation running up to the point where they enter the coils. Riding rough surface gives vibrations and in my case stranded wires came loose and caused a short in one of my motors.

http://www.electric-skateboard.builders/t/raptor-dual-one-motor-starts-breaking-short-in-windings-solution-found/4868/16 

Take a look in this thread how I fixed the motor problem. I got a new motor in warranty from enertion which I will swap later when I get home again.

Good luck! Let us know what you found, it's handy for the knowledge base.
```

---
## \#10 Posted by: Adam0311 Posted at: 2016-07-06T05:49:36.119Z Reads: 195

```
I definitely still have resistance with the battery disconnected, but I think you're saying I need to disconnect the motor from the vesc and then check for resistance...is that right?
```

---
## \#11 Posted by: Namasaki Posted at: 2016-07-06T06:09:19.310Z Reads: 183

```
yes, disconnect the motor in question form everything and then try spinning it.
It the brakes are still on then you have a short in the motor
```

---
## \#12 Posted by: Namasaki Posted at: 2016-07-06T06:10:42.482Z Reads: 179

```
If the motor spins normally by itself but has more resistance when you connect it to the vesc, then you likely have a short on the vesc
```

---
## \#13 Posted by: Namasaki Posted at: 2016-07-06T06:11:57.109Z Reads: 176

```
Basically, touching 2 of the 3 motor wires together will cause brakes or resistance
```

---
## \#14 Posted by: Namasaki Posted at: 2016-07-06T06:14:45.424Z Reads: 175

```
When it happen to me, it was the Esc. shorted out and burned up. the motor was fine but dragging as long as it was plugged into the esc
```

---
## \#15 Posted by: Adam0311 Posted at: 2016-07-06T06:39:37.018Z Reads: 168

```
Thank you. Exactly the feedback I'm looking for.
```

---
## \#16 Posted by: Skitzor Posted at: 2016-07-06T08:10:05.067Z Reads: 167

```
I'm hoping it's not ur esc. Pushing the wires more inside the motor if it would block still while disconnected can also resolve the short. Then ur sure its inside the motor.
```

---
## \#17 Posted by: Dedbny Posted at: 2016-07-06T10:10:50.358Z Reads: 173

```
I always go simple first.  Before the spark,  I was thinking the reason was a loose connection between motor and vesc. Try and check there is proper connection at the vesc point.  Possible loose solder. Youll need to get the hot glue off to check.

Now that there is the spark something else may have been damaged. Need to break down the potential reason by elimination.  I think its back to Enertion support for help.  Ive got a dual here you could use by Im in AUS.  Hope it gets fixed first. 

On another note with the toggle type switches now being used for the battery is there any chance that you can  turn it off when riding. That would not be good.  Glad you didnt experience too much pain on that sudden brake to the shop.
```

---
## \#18 Posted by: Adam0311 Posted at: 2016-07-07T06:54:39.317Z Reads: 159

```
Quick update. Tried connecting to BLDC without success. Went ahead and removed the slave vesc side motor, no visible shorts. Plugged in space cell and turned it on...spark followed by small fire on slave vesc...good times. Pic attached. Pulled slave vesc and plugged in space cell...board fires up. So looks like master vesc and motor is good to go. Next step, get on list for a vesc. <img src="/uploads/db1493/original/2X/1/182ad0b3cc5093a115d6902e1b6241a37cf61fcb.jpeg" width="375" height="500">
```

---
## \#19 Posted by: chaka Posted at: 2016-07-07T14:13:46.061Z Reads: 154

```
i would try and find out what happened before hooking up another fresh VESC. Check the bottom side of the pcb and see if the jst pins have punctured the positve primary power cable. Pick and place manufacturers rarely, if ever, trim these and they will eventualy puncture cables if left long. I circled the GND pin in question.

<img src="/uploads/db1493/original/2X/3/3f74d91a358ed49855379a9cb7261b34eb411d81.jpeg" width="375" height="500">
```

---
## \#20 Posted by: Sboard342 Posted at: 2016-07-07T14:46:39.555Z Reads: 147

```
This knowledge is why I buy all my VESCs from Chaka.
```

---
## \#21 Posted by: elkick Posted at: 2016-07-07T15:29:23.383Z Reads: 143

```
[quote="chaka, post:19, topic:5629"]
Pick and place manufacturers rarely, if ever, trim these and they will eventualy puncture cables if left
[/quote] 
That's really important! Needs to be done with every single PCB - its always the first thing I do prior to program it with the STlink. Won't be an issue anymore with the v6, but it's  just a way of keeping things clean, so I'll do it anyway with those too.
```

---
## \#22 Posted by: Adam0311 Posted at: 2016-07-07T19:03:18.345Z Reads: 137

```
Thanks for the knowledge @chaka. Indeed the postive wire has an indention, but it doesn't look like it punched through the coating yet. I've added a couple more pics of the vesc. <img src="/uploads/db1493/original/2X/8/847d02f05ab22d54407de807d189ff3eeb4333b8.jpeg" width="387" height="500"><img src="/uploads/db1493/original/2X/9/94f70dfa2e5801e4b15860126c529e6e3893e98f.jpeg" width="375" height="500">
```

---
## \#23 Posted by: Adam0311 Posted at: 2016-07-07T19:04:38.539Z Reads: 130

```
Note the chunk missing from chip in first pic.
```

---
## \#24 Posted by: chaka Posted at: 2016-07-07T19:38:38.844Z Reads: 131

```
Usually a direct short will also burn the primary power trace withing the area I circled so you very well could have a short somewhere in your phase wires or it could be related to that broken fet. If you or a friend has a hot air station you could probably revive this unit by replacing a few fets and possibly the drv chip. You would also need to bridge the burned trace between the fets on the top side.

<img src="/uploads/db1493/original/2X/d/da546e15188f871fd75b30e519b2bc2e9ac60428.png" width="387" height="500">
```

---
## \#25 Posted by: sl33py Posted at: 2016-07-07T19:48:06.275Z Reads: 128

```
Sucks man.  I would contact enertionsupport and start there.  I definitely would not use the space cell until they confirm it should be OK.
```

---
## \#26 Posted by: Adam0311 Posted at: 2016-07-07T19:54:37.542Z Reads: 128

```
I did try other battery with same results...@torqueboards 12s...its in my earlier posts.
```

---
## \#27 Posted by: Adam0311 Posted at: 2016-07-07T20:39:49.022Z Reads: 125

```
I did your test on motor once it was disconnected. Normal spin. Hadn't thought of this test until you mentioned it, but it makes sense and gives me some comfort that the motor appears to be ok.
```

---
## \#28 Posted by: Namasaki Posted at: 2016-07-07T23:44:31.188Z Reads: 120

```
Now, with the motor disconnected, try shorting 2 phase wires together and spin the motor to see what the resistance is like.
```

---
## \#29 Posted by: Adam0311 Posted at: 2016-07-08T04:20:42.315Z Reads: 115

```
I taped two wires together and it's much heavier resistance. That's what a motor short would feel like, correct?
```

---
## \#30 Posted by: Michaelinvegas Posted at: 2016-07-08T04:21:39.531Z Reads: 115

```
Yes correct 
----
```

---
## \#31 Posted by: Adam0311 Posted at: 2016-07-08T04:21:59.568Z Reads: 113

```
Since it doesn't feel like that when the wires are separated, should mean no short in motor, correct?
```

---
## \#32 Posted by: Namasaki Posted at: 2016-07-08T04:23:18.283Z Reads: 113

```
Correct...
```

---
## \#33 Posted by: Adam0311 Posted at: 2016-07-08T04:24:55.605Z Reads: 110

```
Sorry for Barney style questions.
```

---
## \#34 Posted by: Michaelinvegas Posted at: 2016-07-08T04:28:32.534Z Reads: 108

```
Hell no...you have a problem...you want to figure it out...ask away bro
```

---
## \#35 Posted by: flatsp0t Posted at: 2016-07-08T20:23:28.789Z Reads: 108

```
Correct.

Didn´t jason say something about a no questions asked warranty for raptors?

I would go for that and ask for a replacement VESC.
This might be the fastest and safest way.
```

---
## \#36 Posted by: Xusia Posted at: 2016-07-13T02:49:16.405Z Reads: 106

```
I had a very similar issue with my board (locked up and threw me off; one motor had heavy resistance to spinning when I bench tested later) and actually got fairly hurt in the superman thingy that resulted.  I Emailed Enertion, board was sent for repair (my cost) no questions asked.  I'm currently waiting to hear back.  If you wanted it repaired under warranty, I doubt you would have any problems (except maybe the VESC, *if* you actually made that worse).
```

---
## \#37 Posted by: Adam0311 Posted at: 2016-07-13T05:10:01.334Z Reads: 100

```
I emailed enertion@support and waiting to hear back. Was yours the slave VESC or motor connected to slave VESC? It actually seems like several boards have had the same or similar problems. Another thread started by @Skitzor seems like it could be the same issue and a few other raptor owners have weighed in with similar experiences.
```

---
## \#38 Posted by: Adam0311 Posted at: 2016-07-13T05:35:39.104Z Reads: 102

```
Sorry to hear you got hurt. Being honest, the part that bothers me the most is the loss of confidence in the board. I remember accelerating, sudden lock up and then I'm sliding across Pacific Coast Highway (super busy F'ing street) on my shoulder. I didn't even have time to think about running it out....literally flew off the board. I had cars at the light I was crossing pulling over to make sure I was OK. At this point I just want to make sure the lock up doesn't repeat.
```

---
## \#39 Posted by: Xusia Posted at: 2016-07-13T06:21:36.143Z Reads: 99

```
Sounds like we had very similar experiences; the next thing I knew I half way to  a face plant.  (Lucky for me I was in a full leather suit and motorcycle helmet!)  I too have lost confidence in it.  I'm hoping I'll gain it back over time...
```

---
## \#40 Posted by: redvlx Posted at: 2016-07-13T07:37:06.602Z Reads: 98

```
It seems to me like people are going through VESC like hotcakes. I mean they aren't that cheap and the results can be fairly catastrophic when they fail so I just wonder why people rave on about how good they are. Seems most DIY builders have gone through at least 1 sometimes many more. Cant someone heavily over engineer these things to handle whatever is thrown at them or am I missing something? I feel like maybe a lot of people on this forum are ex (or current) RC enthusiasts who seem to accept that constant failure and replacement of parts is just a standard with the hobby but I know the reason I chose not to use VESC was inevitable failures and ongoing cost. Am I missing something?
```

---
## \#41 Posted by: c4Lvin Posted at: 2016-07-13T09:12:45.271Z Reads: 88

```
Can't agree with you more and could not have said it better. Someone needs to come up with a tank of an ESC. Not just for robots but ridiculous power output, input handling and SUPER RELIABLE where it doesn't short out or burn out for no specific reason. RC cars ESCs almost never short out if you don't go over their stated limits...EVER. My Team Novaks and Tekins are still running strong since the late 80s!
```

---
## \#42 Posted by: flatsp0t Posted at: 2016-07-13T09:30:28.454Z Reads: 85

```
That is what VESC version 6 will bring.
```

---
## \#43 Posted by: redvlx Posted at: 2016-07-13T09:53:09.380Z Reads: 87

```
Ok that's good to know. Don't get me wrong I'm not a hater and i want it to work as much as the next guy but they definitely aren't there yet and in their current form they seem very over rated
```

---
## \#44 Posted by: jrpwit Posted at: 2016-07-13T12:30:13.738Z Reads: 86

```
Ahm but Vedder is working on improvements for the vesc. In his upcoming version 6 vesc one will be able to have a much higher erpm without blowing their drv chip and more. Progress is coming but at the current state the vesc is a great esc especially for electric skateboards. I would call it hardly overrated cause it is made specifically for electric skateboards but needless to say it is still a work in progress.
```

---
## \#45 Posted by: redvlx Posted at: 2016-07-13T13:06:06.354Z Reads: 85

```
I don't feel you can call it great if it is not reliable and has plenty of documented failures, some explained and some still a mystery. Definitely shows a lot of promise and eventually will be great, but as you said...work in progress. No one seems to mention that you will likely burn one or two out in some way, shape or form in your travels if you go with the current VESC when they recommend them to people is all I'm saying. In saying that ill jump straight on board when the reliability issues are ironed out.
```

---
## \#46 Posted by: JohnnyMeduse Posted at: 2016-07-13T13:22:47.967Z Reads: 85

```
Sorry but it not totally true, the vesc is not the most reliable esc, but don't forget that on this web site people who talk about the Vesc are most often people with problem. You won't hear so much from the hundred and hundred of people who got their build working fine with Vesc, because their are out having fun. And also, when the vesc is program within is limit and being push, it really a great product.
```

---
## \#48 Posted by: flatsp0t Posted at: 2016-07-13T13:27:33.512Z Reads: 80

```
This plus people with good vescs dont tell it to everyone. (Running 6 of you VESCs, never had a problem, never told everybody about having no problem)
```

---
## \#49 Posted by: redvlx Posted at: 2016-07-13T13:37:46.919Z Reads: 85

```
Ok fair enough. I guess also because VESC are a lot more popular that they would naturally have a higher amount of failures due to simple ratio comparison and I can see that not many would get on to say they haven't had a break down as you say @flatsp0t. That was pretty much the info I was after @Chaka as I felt I was missing something so obviously people are running them outside of there capabilities then and suffering the consequences. That makes more sense to me that they still have a large following. Bring on the high current version 6 then!
```

---
## \#50 Posted by: onloop Posted at: 2016-07-13T15:45:53.706Z Reads: 90

```
@Adam0311 hey Adam. 

Please email support@enertionboards.com  so we can get you up and running again.
```

---
## \#53 Posted by: sl33py Posted at: 2016-07-13T17:04:58.503Z Reads: 90

```
VESC failures - not if you are getting a well made one, and not if you are sticking with what works best.

VESC is capable of FOC - but there are issues.  VESC is capable of 12s - but there are motor limitations.  If you stick to BLDC and 8-10s it's extremely reliable.  FOC will come, but think how long it took to dial in all the abilities within BLDC.

I have 4 or 5 VESC's (maybe 6 now).  I've had two fail - both my fault while bench testing/troubleshooting.  I was seeing inconsistent errors voltage related on 12s.  So while testing - hammering hard starts/stops is a sure way to fry your DRV.  So i don't do that anymore.  Since then no issues with those 2 VESCs.  I have one VESC on 8s, using old 4.7hw and firmware, going strong now for 1-1.5 years.  Untouched - just works.  Single generic 6355 200kv motor.

I got a new 4.11/4.12 VESC from a member here with a dead DRV chip already.  Have the DRV's on their way from Mouser now, plus a few spares.  I don't mind swapping a chip if i'm going to try FOC or 12s - and as part of DIY it's good practice and a skill i want to get better at (SMD soldering).

If you are that worried about a component failure - don't go bleeding edge.  Either stick to another ESC altogether, realizing it is a compromise and sacrifice some capability - wether that's FOC ability, or 12s, or tweakability/configurability, or run your VESC more conservatively - not 12s, not FOC (just yet), etc.

And don't buy cheap VESC's.  I respect enertion's dedication to giving us VESC's as cheaply as possible, and that initial batch was FUBAR (cheap "equivalent" components) - which he made right.  Since then swapping manufacturers to ensure good quality.  Similarly i wouldn't hesitate to buy from Chaka/Ollin.  I would avoid the "Maytech" VESCs like the plague...  but that's just my opinion.  My first 3 VESCs were direct from Ben.

And since i'm on my soapbox today it seems...  These are being developed by "a guy" - someone you've never met (unless you're lucky), and probably never even spoken with, besides the forums.  I have sent him close to $200 now - splitting a small 5-10$ profit on some of the anti-spark switches he helped develop (along with Fechter), and a few general donations when able to help him continue to develop these amazing ESC's.  That is likely a _fraction_ of the money he personally has invested in developing a completely new ESC.  One built and dedicated for non-RC esk8 (and other) use.  So if you want to see v6 sooner - **_put your money where your mouth is and kick in a few $ to help with the effort_**.  [/soapbox]
```

---
## \#54 Posted by: Blacksheep Posted at: 2016-07-13T17:43:29.136Z Reads: 83

```
I'm just waiting for my vesc so I can build my first board but I have 4 3s lipo and what you are saying is that 12s is bad for the vesc ?
```

---
## \#55 Posted by: chaka Posted at: 2016-07-13T18:10:08.289Z Reads: 81

```
12s is not bad for the VESC. You do need to be a little more mindful of how much regen/braking current you set in the bldc-tool so you do not end up pushing the voltage too high when riding with a fully charged pack. I have a very reliable 12s board that I ride daily. 10s is a little better since it gives you plenty of headroom with what voltage the components can handle.
```

---
## \#56 Posted by: sl33py Posted at: 2016-07-13T18:25:26.917Z Reads: 84

```
@Chaka - exactly.  12s is totally doable (if your motor is <200kv to point out the obvious), but you still need to be mindful of your settings as it is easier to damage the VESC with misuse/misconfiguration.

i would recommend 8/10s on BLDC as the most reliable i've found.  I've ran my Vanguard (GF's board) on 8s without any issues.

All that said - can't wait for v6 from Vedder!
```

---
## \#57 Posted by: Blacksheep Posted at: 2016-07-13T18:26:01.196Z Reads: 82

```
Ok thanks for explaining
```

---
## \#58 Posted by: Adam0311 Posted at: 2016-07-13T22:59:08.673Z Reads: 80

```
Thanks Jason. Email was actually sent on Monday my time. (I'm in US). Please let me know if you need any other details.
```

---
## \#60 Posted by: onloop Posted at: 2016-07-14T00:28:36.649Z Reads: 79

```
[quote="Adam0311, post:58, topic:5629"]
Email was actually sent on Monday my time.
[/quote]

we have a backlog of about 200 emails at the moment.....
```

---
## \#47 Posted by: onloop Posted at: 2016-07-14T04:39:10.158Z Reads: 31

```
6 posts were merged into an existing topic: [Are 50mm OR 63mm Motors Better on Electric Skateboards?](/t/are-50mm-or-63mm-motors-better-on-electric-skateboards/6074)
```

---
