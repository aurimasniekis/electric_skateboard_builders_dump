# Failed build 2 years ago and gave up, desperately need help on second try

### Replies: 32 Views: 483

## \#1 Posted by: ArsenalMain Posted at: 2020-01-09T02:27:46.454Z Reads: 131

```
Hello everyone, 
Two years ago, I attempted to build an electric longboard. I purchased the following: 
 218mm torque board motor mount 
https:///collections/bundle-kits/products/single-motor-mechanical-kit 
190 kV 6374 Motor 
https:///products/electric-skateboard-motor-6374-190kv
Torque ESC 
https:///products/torque-esc-bldc-electronic-speed-controller 
BMS from best tech
![BMS%20ESK8|362x500](upload://lDlXtv87BCA5mY1RjBTzGcEC2Uc.jpeg)

Luna 36V 4 Amp charger
https://lunacycle.com/36v-4amp-luna-mini-charger/

Case from psychotiller

Controller from miami electric boards. 

https://miamielectricboards.com/shop-1/handheld-electric-remote 

5 turnigy, 60C 7.4V Lipo Batteries. 

In the end, nothing worked for me and it was heartbreaking. I talked for months with Namasaki and other users for help and nothing worked for me. As i was a freshman in college when i started this process, I did not have the funds to redo the board and I was stuck with a broken, unusable electric board. At the present, I do not have an overly abundant supply of funds, but i would really like to get my board working for the last semester of college. 

My best guess is that the BMS boards fried somehow and my batteries fried as a result, or the other way around. Hence, I at least new a new set of batteries and BMS. I do not know if my VESC was fried as well, but i cant check as the board has no power. Same with the controller circuit board. 

Attached are images of my board and previous setup: 
![20200107_172350|666x500](upload://fuwaXXCW7Yg0owgvUFj4jfpvtTN.jpeg) ![20200107_172436|666x500](upload://gfgRfIxNStp0GOONrsC4EBpEMer.jpeg) ![20200107_172441|666x500](upload://zYEyMzO3F2lS0yot1cq7NVqMl6y.jpeg) ![20200107_172509|375x500](upload://qKKAOAO97swwl4acyw6iks1MVyk.jpeg) 

I have spent the last couple weeks refreshing myself on the different aspects of DIY board building and how everything works. It is at this point that I need help with getting new batteries, if I should should go lion this time instead of lipo, where I could get the best deal, etc, as well as if there is anything of my current build I should change out. 

For reference, I would like top speed of 30, with a range of 15 miles. This means I would like a minimum of 10s, prefereably >5000 mAh, with a minimum Wh of 250. 

Basically, I am still at a loss of why my board didnt work previously and am really anxious about this second time and making sure it is not a repeat. 

Thanks for making it all the way through this. I appreciate any and all help.
```

---
## \#2 Posted by: ZachTetra Posted at: 2020-01-09T02:39:41.401Z Reads: 110

```
Start with the simple things first.  Check the voltage of each individual battery (disconnect them from the board), if they are all good check the voltage going into the BMS, if that's good check the voltage coming out of the BMS

By the looks the solder joints are not up to par so maybe a connection is bad, alternatively the BMS may be cutting the connection since the cell voltages will all read as an error (non of the balance leads are connected, please be very careful with with which one goes where)

BTW you're gonna want to go to forum. since all the cool people are there too
```

---
## \#3 Posted by: PixelatedPolyeurthan Posted at: 2020-01-10T13:23:57.080Z Reads: 101

```
[quote="ZachTetra, post:2, topic:105157"]
forum. since all the cool people are there too
[/quote]

This.
please join the new forum, this one is not being paid and we don't know when it is going to go down
```

---
## \#4 Posted by: deucesdown Posted at: 2020-01-11T00:49:50.349Z Reads: 85

```
Where are you located? Maybe you need a once over with someone experienced to jump start you on how not to blow stuff up.
```

---
## \#5 Posted by: ArsenalMain Posted at: 2020-01-11T01:12:11.993Z Reads: 83

```
Mcminville Oregon. And honestly, that would be so nice. Its really f'ing hard to find answers to all the questions I have. Like there are only so many answers you can find by searching and asking. Discussing in person would be so helpful. @Skunk has actually been answering some questions I have, which helps.
```

---
## \#6 Posted by: deucesdown Posted at: 2020-01-11T01:14:41.561Z Reads: 77

```
The oregon gang is creepy. Make sure you wear protection. :) you might be able to trade favors. I hear @Skunk is moving.

BTW your parts look nice.
```

---
## \#7 Posted by: ArsenalMain Posted at: 2020-01-11T01:19:55.041Z Reads: 72

```
Appreciate it. Hopefully this time, I will work more than once :joy:
```

---
## \#8 Posted by: deucesdown Posted at: 2020-01-11T18:50:34.169Z Reads: 68

```
[quote="ZachTetra, post:2, topic:105157"]
Start with the simple things first. Check the voltage of each individual battery (disconnect them from the board),
[/quote]

Start here. If voltage is below say 3.2v per cell you may need a new pack. You'll need a multimeter. The harborfreight free with coupon one will work. The health of the packs will determine next steps.
```

---
## \#9 Posted by: ArsenalMain Posted at: 2020-01-12T02:40:01.477Z Reads: 63

```
I already know the batteries are dead honestly, I know I need to order a new set. I just don't know if I need to order new bms's, vesc, or remote/remote 2.4 receiver. I'm sure the motor still works fine, so I'm not worried about that. I just sucks cause Im not sure if I have enough to replace all 3 if it needs it.
```

---
## \#10 Posted by: deucesdown Posted at: 2020-01-12T03:30:41.147Z Reads: 63

```
That's a shame, that was a nice battery setup. I feel like, maybe a good strategy here is to get the cheapest possible battery that will move your board, because the chances of you killing it while you learn are decently high. Once you learn care and feeding of battery packs you can move on to a more $$$ pack.

I would honestly advise not hooking up BMS at first. Do a few short rides (don't drain the pack down too far, set esc cutoffs conservatively), charge the batteries carefully to like 85% while checking cell voltages manually. Like 3-4 rides. This would be a very simple system, easy to troubleshoot (if the battery was built well).

Then once all this stuff is working add the BMS.

The trick then is what battery to start/test with... @ZachTetra do you have anything horded? :slight_smile:  

Just to give some comfort, you can probably get an equivalent esc in the $50-60 range if you get lucky. If you go to the other forum, in a month or two we may have access to a focbox (single) clone for $80, called the NeoBox.

If the BMS is toast you can replace with a small charge-only one for like $20. Likely candidate is the Bestech D140, or a generic red waterproof bms from aliexpress.
```

---
## \#11 Posted by: ZachTetra Posted at: 2020-01-12T03:36:26.509Z Reads: 52

```
Sorry that happened but I got nothing good at the moment.  I'm selling a 6s 5000mah lipo, but that's nothing for this build so not at the moment...I can make a 10s up to maybe 6p Samsung 13Q in a bit though.  I'm not an expert at building packs but it would be good quality and decently safe to use (I mean I'd trust it)
```

---
## \#12 Posted by: deucesdown Posted at: 2020-01-12T03:40:52.803Z Reads: 49

```
the 6s might be great for testing, what are you looking to get? OP can resell it for a small loss when he gets his real battery. I guess there's the question of how to charge 6s without spending money...
```

---
## \#13 Posted by: ZachTetra Posted at: 2020-01-12T03:46:07.965Z Reads: 52

```
I was hoping $50 plus shipping and fees for the pack and a charger for it (no BMS), but I've just gotten someone interested on the other forum already
```

---
## \#14 Posted by: ArsenalMain Posted at: 2020-01-16T03:49:06.709Z Reads: 47

```
Yes, I agree it was an awesome battery setup. It would have been high output. And I agree that the chance I kill it is somewhat high, but ive been doing alot of research to figure out exactly what went wrong. Im thinking it was either a defective bms, or defective balance placement. I appreciate the assistance. I agree that 

[quote="deucesdown, post:10, topic:105157"]
Do a few short rides (don’t drain the pack down too far, set esc cutoffs conservatively), charge the batteries carefully to like 85% while checking cell voltages manually. Like 3-4 rides. This would be a very simple system, easy to troubleshoot (if the battery was built well).
[/quote]
this would have been a good idea in the beginning, but I overshot. And ya, I think that that is the way to go, small, charge only bms. 

On a side note, a guy on here who lives close to me has offered to help me figure out my battery situation. 

Question though that ive been looking for. What do you do to waterproof your board as much as possible?
```

---
## \#15 Posted by: ArsenalMain Posted at: 2020-01-16T05:34:06.382Z Reads: 42

```
Also, why do some people recommend a discharge only bms and other a charge only bms. Whats exactly the difference/why is one preferred over the other?
```

---
## \#16 Posted by: deucesdown Posted at: 2020-01-16T06:14:31.014Z Reads: 43

```
[quote="ArsenalMain, post:14, topic:105157"]
Question though that ive been looking for. What do you do to waterproof your board as much as possible?
[/quote]

Don't attempt this now. Get your board working for a prolonged period, then look into improvements. Basics first.

[quote="ArsenalMain, post:15, topic:105157"]
some people recommend a discharge only bms and other a charge only bms
[/quote]

charge+discharge bms:
- big, expensive
- protects output from overdischarge and overcharge
- if protection kicks in, power cuts off and sometimes sends you flying

charge only bms:
- small, inexpensive
- provides protection only for charging
- will not cut off your esc, will always have power even if it's destroying the batteries (many feel batteries/board are cheaper to replace than broken bones/joints, etc).
```

---
## \#17 Posted by: GeraldSwerdfegger Posted at: 2020-01-28T20:44:58.769Z Reads: 31

```
I'm in Portland. I'd be happy to go over it with you if you can make it up here. I've even got some extra battery packs and components sitting around that we could use to troubleshoot.
```

---
## \#18 Posted by: ArsenalMain Posted at: 2020-01-30T04:15:14.217Z Reads: 27

```
@deucesdown

I have a couple questions that I have been unable to find elsewhere in this forum or the other:

I will be riding my board almost every day to class. Should I allow my batteries to drop down to ~35v before I charge it to get a whole cycle or could I charge it daily to maintain that pre-sag feel? Or is that really bad for the batteries.

Would you recommend the ackmaniac tool or the vesc tool?

Also, correct me if I'm wrong, but a 10s5p q30 battery has a continuous output of 75 amps correct? Or a peak of 100a. And my motor is capable of 80A, and my esc is 50a and 250 continuous.

I was just looking at setting up my vesc settings. I have to base everything off of my esc then cause it's the bottleneck? So the motor max would be 80a, the motor min would be -80 (?), peak 250a, batt max 50a and bat min like -20 (?). And what's your thoughts on foc vs bdlc? Sorry, alot of stuff all at once. Just tryin to review my stuff before we get together.
```

---
## \#19 Posted by: ArsenalMain Posted at: 2020-01-30T04:16:53.066Z Reads: 28

```
And how do you think this bms would work? https://www.amazon.com/Akozon-Protection-Balance-Li-ion-Battery/dp/B07FX7DRXP
```

---
## \#20 Posted by: deucesdown Posted at: 2020-01-30T05:36:10.528Z Reads: 32

```
[quote="ArsenalMain, post:18, topic:105157"]
I will be riding my board almost every day to class. Should I allow my batteries to drop down to ~35v before I charge it to get a whole cycle or could I charge it daily to maintain that pre-sag feel? Or is that really bad for the batteries.
[/quote]

lithium ion doesn't have memory effects like ni-cad or nimh, so you can charge it whenever you like. However, lithium ion does degrade when stored full or empty. So try to top off right before you ride for maximum cycle life. You can also charge to 4.1v/cell to roughly double cycle life, but doing this will not give bms an opportunity to balance the pack, so at least once a month give it a full charge.

[quote="ArsenalMain, post:18, topic:105157"]
Would you recommend the ackmaniac tool or the vesc tool?
[/quote]

Pros and cons. vesc tool will have all the latest and greatest, and all the up-to-date support and documentation will match. On the other hand, ack's version is kind of frozen at one version, so it's very well understood, works with the ackmaniac android app, and some would argue the newer features of vesc-tool are not really significant. You can try both and decide for yourself. I prefer ack, but every day as vesc tool gets improvements, the scale shifts toward vesc tool.

[quote="ArsenalMain, post:18, topic:105157"]
10s5p q30 battery has a continuous output of 75 amps correct
[/quote]

internet wisdom is 30Q is good for 20A discharge. A 5p pack can do 100A if built correctly. But not many motor/esc combos can extract that much power. For example with settings at 50a battery per focbox in a dual drive 6374, I'm only about to pull 70a from the battery total.

[quote="ArsenalMain, post:18, topic:105157"]
I was just looking at setting up my vesc settings. I have to base everything off of my esc then cause it’s the bottleneck? So the motor max would be 80a, the motor min would be -80 (?), peak 250a, batt max 50a and bat min like -20 (?). And what’s your thoughts on foc vs bdlc? Sorry, alot of stuff all at once. Just tryin to review my stuff before we get together.
[/quote]

Start small here and work up. You can use the factory defaults I think. You're on a single 4.12 vesc. I think a safe motor max is 60a (but start at 50a). Battery max, safe is 30A. I don't think it's safe to set more than 35A (but you may want to try higher).

This is a simplification, but motor max influences torque at low speeds. battery max influences torque at high speeds. You get the smoothest control by setting both to the same number. But typically motor max is set quite a bit higher.

FOC vs BLDC, on your 4.12hw esc, do NOT use FOC. I repeat, do NOT use FOC. It has a very very good chance of frying the drv. Also do not do 12s. The reputation of torqueboards 4.12 is anything more than 10s BLDC is danger danger.

Generally, BLDC is loud and powerful, FOC is quiet and more refined (and also makes the FETs heat up more). FOC has gotten more attention from bvedder, so for example, sensor support is better in FOC. On newer good quality vesc, most people run FOC.

[quote="ArsenalMain, post:19, topic:105157, full:true"]
And how do you think this bms would work? https://www.amazon.com/Akozon-Protection-Balance-Li-ion-Battery/dp/B07FX7DRXP
[/quote]

With your story, get your board running for a few rides before thinking about BMS. :) Keep it simple, work forward in small steps. When it's time, try to search here and on the other forum, for a popular BMS.

Finally, you should hit up @GeraldSwerdfegger with his generous offer! Meet up, buy him cookies, show him what you'd do and have him teach you all the places you messed up and would blow something up. :slight_smile:
```

---
## \#21 Posted by: ArsenalMain Posted at: 2020-01-30T08:16:59.513Z Reads: 24

```
[quote="deucesdown, post:20, topic:105157"]
So try to top off right before you ride for maximum cycle life. You can also charge to 4.1v/cell to roughly double cycle life, but doing this will not give bms an opportunity to balance the pack, so at least once a month give it a full charge.
[/quote]

This sounds great. I also didn't realize that lion doesn't have the memory effect that nicad/nimh has.

[quote="deucesdown, post:20, topic:105157"]
You can try both and decide for yourself.
[/quote]
I have looked into both at this point, and considering that both have pretty easy wizards to set stuff up, there ultimately isn't much of a difference between these two correct?

[quote="deucesdown, post:20, topic:105157"]
You’re on a single 4.12 vesc. I think a safe motor max is 60a (but start at 50a). Battery max, safe is 30A. I don’t think it’s safe to set more than 35A (but you may want to try higher).
[/quote]
At least, looking at the torquboard specs for this esc and motor, the esc is rated at a 50a continuous max and a 240a peak. 
https:///products/torque-esc-bldc-electronic-speed-controller

And the motor is rated for 80a max. 
https:///collections/electric-skateboard-motors/products/electric-skateboard-motor-6374-190kv

Could I reasonably out 50a for the battery max and 50a for the motor max. In reality, the motor could take 80a, but if this is true:
[quote="deucesdown, post:20, topic:105157"]
You get the smoothest control by setting both to the same number.
[/quote]
Than could I set both to 50a? Is is the torquboard esc not really recommended to use the 50a max and keep it closer to 40a? Just considering my battery is 10s5p, then I would hate to only use 30a of the possible 100a output.

[quote="deucesdown, post:20, topic:105157"]
on your 4.12hw esc, do NOT use FOC. I repeat, do NOT use FOC. It has a very very good chance of frying the drv.
[/quote]
Thank you for this. I was considering using the foc so I'll make sure to stay clear of it for now until I get a vesc-6/x/focbox to be safe.

[quote="deucesdown, post:20, topic:105157"]
With your story,
[/quote]
Man, you don't even know the half of it 😂

[quote="deucesdown, post:20, topic:105157"]
Finally, you should hit up @GeraldSwerdfegger with his generous offer!
[/quote]
Absolutely, I'm trying to get all the help I can find and it's always nicer whne you can ask questions in person and work through solutions. Infinitely harder over a forum.

[quote="deucesdown, post:20, topic:105157"]
buy him cookies,
[/quote]
If he really helps me out, I may just have to one up that and bring him some of my homebrew.


Last couple things (for now lol):
When setting the motor min, do you set it to be equal and opposite of the motor min? And what exactly does this relate to in the actual ride? Is it the brake at high speeds?

Same question but with bat min? I've seen people recommend it anywhere from -10 to - 20. Is this the high speed break or low speed?

Do you recommend enabling reverse within the vesc or do you personally not prefer it?

Lastly, I justed wanted to thank you again for going out of your way to give me some advice. Really appreciate it. And it goes out to everyone on this thread and the two forums. I think the group that makes up this hobby are all really positive and selfless and it's been a blast being apart of it.
```

---
## \#22 Posted by: deucesdown Posted at: 2020-01-30T15:21:15.328Z Reads: 17

```
[quote="ArsenalMain, post:21, topic:105157"]
ultimately isn’t much of a difference between these two correct?
[/quote]

Ack firmware is basically an old version of vesc firmware with a few tweaks. There have been many changes, but mostly the ride is the same. The UI has been changed a lot, including the wizards I believe.

But, as we speak, last night vesc tool announced/shipped a pretty interesting new feature for sensorless start from standstill. :slight_smile:

 

[quote="ArsenalMain, post:21, topic:105157"]
rated for 80a max
[/quote]

[quote="ArsenalMain, post:21, topic:105157"]
In reality, the motor could take 80a
[/quote]

Don't pay much attention to listed specs on things like esc and motor. Look for hard won community experience.

For you especially ;) start with the safe settings, and creep up only if needed after reading a bunch. I'm purposefully trying to stay away from optimal, and complicated discussion of numbers, and generalizing some relationships, and some safe limit numbers I've read many times on the forums. Keep it simple until you have it working reliably.

You also want to focus on the low voltage cutoffs. Set them very very conservatively at first, and don't discharge your pack past say 50%. This is where many destroy their multiple hundred dollar pack in their first few excited rides.

[quote="ArsenalMain, post:21, topic:105157"]
I would hate to only use 30a of the possible 100a output.
[/quote]

You should seriously consider dual motor if you're looking at those numbers that way :) It's really hard to pull anything close to 100a from one esc, and dual gives you more than double the torque and more important, braking.

[quote="ArsenalMain, post:21, topic:105157"]
Last couple things (for now lol): When setting the motor min, do you set it to be equal and opposite of the motor min? And what exactly does this relate to in the actual ride? Is it the brake at high speeds?

Same question but with bat min? I’ve seen people recommend it anywhere from -10 to - 20. Is this the high speed break or low speed?
[/quote]

motor max/min affect low speeds, battery max/min affect high speeds. We talked about max. For battery min, typically you set it to what your pack can handle in _fast charge_ mode. Usually this isn't quite enough, and most people creep it up (technically down, as it's a negative number) until they have okay brakes. Raising this can also increase your chance of frying the vesc if you brake hard at full charge.

motor min, you can raise it until it feels good up to maybe -60 maybe even -80.

The closer motor/battery min and motor/battery max are to each other the smoother the throttle will be. But this is usually not practical, and motor settings will be quite a bit higher than battery settings.

[quote="ArsenalMain, post:21, topic:105157"]
Do you recommend enabling reverse within the vesc or do you personally not prefer it?
[/quote]

You should probably start with current (or watt) mode brake with no reverse. Play with it after everything is working well, see for yourself. Ackmaniac's android app makes it really easy to temporarily change modes on the fly.

[quote="ArsenalMain, post:21, topic:105157"]
Lastly, I justed wanted to thank you again for going out of your way to give me some advice
[/quote]

Dude all of us feel your pain! Acutely! And we're stoked to see you back on it. Wear helmet and gloves minimum especially on test rides!
```

---
## \#23 Posted by: ArsenalMain Posted at: 2020-02-02T17:51:26.856Z Reads: 13

```
[quote="deucesdown, post:22, topic:105157"]
Ackmaniac’s android app makes it really easy to temporarily change modes on the fly.
[/quote]
 Do I need an HM-10 module in orded to connect it to my ackmaniac android app?
```

---
## \#24 Posted by: itsrow Posted at: 2020-02-02T18:01:32.169Z Reads: 12

```
Yessir, and I have a LiPo 3s1p x 4 if you want some pictures for balacing connections and general setup.
```

---
## \#25 Posted by: deucesdown Posted at: 2020-02-02T22:26:08.438Z Reads: 12

```
https://buildkitboards.com/collections/accessories/products/vesc-bluetooth-adapter#

https://forum./t/us-sale-bluetooth-modules-remote/17494

I think he has a shit-ton of the enertion ones, and I believe they'll work.

[quote="itsrow, post:24, topic:105157"]
LiPo 3s1p x 4
[/quote]

This is nice but he has a TB 4.12, risky for 12s. 6s or 9s would work lol but you probably want to sell all 4 as a set.
```

---
## \#26 Posted by: itsrow Posted at: 2020-02-03T04:13:32.611Z Reads: 10

```
Standard 4.12s with at least 600UF of capacitance are alright, I've been running them for months.  They just need a little more attention and I wouldn't brother trying them in FOC or the DRVs going to give out on motor detection.
```

---
## \#27 Posted by: deucesdown Posted at: 2020-02-03T04:15:43.692Z Reads: 9

```
Dude this guy blew his whole electronics stack at least once. I don't think he should take chances in this round. The TB 4.12 is kind of notorious -- might have a strong one, but might have a weak one.
```

---
## \#28 Posted by: itsrow Posted at: 2020-02-03T04:25:46.121Z Reads: 9

```
I've heard strange stories about the TB4.12s aswell so that's fair,  I'd probably go with 3s1p 8Ah x 3 Turnigy graphenes in this situation so he can makeup for lost total power using higher amps.
```

---
## \#29 Posted by: deucesdown Posted at: 2020-02-03T04:28:28.340Z Reads: 11

```
[quote="itsrow, post:28, topic:105157"]
3s1p 8Ah x 3 Turnigy graphenes
[/quote]

IMO zippys or vanilla turnigys for this round, or a cheap china pack, until he figures out how to maintain a pack.
```

---
## \#30 Posted by: itsrow Posted at: 2020-02-03T04:30:21.919Z Reads: 11

```
I've found graphenes are pretty close to the same price as basic bitch turnigys and the cycle life just isn't there, wouldn't even bother wasting his time with them.  Zippys yeah they're good.
```

---
## \#31 Posted by: ArsenalMain Posted at: 2020-02-08T07:20:25.622Z Reads: 8

```
When I turn on my controller (Miamiboards) the light turns on but it's constantly orange and doesnt move from the lowest spot, no matter what I do. Does this mean it just isn't connected to the board (obviously because there's still no battery), or broken. I ask because I'm just trying to figure out if it's fully charged, but I have no idea.
```

---
## \#32 Posted by: ArsenalMain Posted at: 2020-02-08T07:20:40.699Z Reads: 8

```
Sorry, kinda a very specific question
```

---
