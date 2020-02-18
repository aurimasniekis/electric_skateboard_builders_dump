# Focbox - stuttering when accelerating from slow speeds in FOC mode?

### Replies: 77 Views: 2876

## \#1 Posted by: cliofreak Posted at: 2018-05-24T23:31:06.086Z Reads: 411

```
So, Im very very disappointed.

Ive got a 10s4p (currently 9s4p due to a bad pack - still aint figured out what killed it. Been riding on it anyway with no major issue untill now).
Single 6374, 200kV, 15T42T gearing, 100 MBS Wheels

Focbox overheated and cut power after just 6.5 miles riding. I was hammering along at 18 - 22 mph but no major hill till mile 6 and then the board just crawled to a stop.

Anyone else getting this? I think these 100mm MBS wheels are just too big and heavy. 
Motor was very warm. Truck was warm and acted like a heatsink. Enclosure felt a bit warm, meaning battery was probs warm too.

Here is metr data: https://metr.at/r/VUaMV
```

---
## \#2 Posted by: mmaner Posted at: 2018-05-25T00:38:54.062Z Reads: 391

```
You've got a battery problem, not a FocBox problem. At least you didn't have a FocBox problem, you might now if you battery was throwing garbage.
```

---
## \#3 Posted by: cliofreak Posted at: 2018-05-25T00:53:06.334Z Reads: 385

```
Ive ordered 4 new 30Qs to replace the bad pack. I still dont know why the pack went dead.

What causes that?
Bad BMS? (only using it for charging)
Leaving on charger too long (Overnight - did it once coz forgot about it)?
```

---
## \#4 Posted by: mmaner Posted at: 2018-05-25T00:55:48.799Z Reads: 375

```
All kinds of things...BMS, bad cells, bad weld, shorted balance wire, intermittent switch short, bad charger, etc. It's impossible to tell without tearing the back down, which would be my next move.
```

---
## \#5 Posted by: cliofreak Posted at: 2018-05-25T00:58:47.210Z Reads: 362

```
Ive already done that and found a middle pack to be completely dead. Found no burn marks. No bad welds. No shorts. Just a pack in the middle that had zero V.
```

---
## \#6 Posted by: mmaner Posted at: 2018-05-25T01:00:26.530Z Reads: 346

```
I would replace the BMS at least.
```

---
## \#7 Posted by: b264 Posted at: 2018-05-25T01:00:30.752Z Reads: 340

```
Are the balance wires on the BMS in the correct order?  Are two of them swapped?
```

---
## \#8 Posted by: cliofreak Posted at: 2018-05-25T01:01:22.425Z Reads: 335

```
It has been fine for about 200 miles. This is a new issue.
```

---
## \#10 Posted by: mccloed Posted at: 2018-05-25T02:31:51.050Z Reads: 326

```
If you have your focbox’s set for 10s then your hitting the low voltage cutoff, is what it sounds like to me. I’ve had BMS’s kill cells. Namely the cheap white BMS’s. Maybe set your focbox’s for 9s, if you haven’t already.
```

---
## \#11 Posted by: lrdesigns Posted at: 2018-05-25T03:05:54.815Z Reads: 320

```
[quote="mccloed, post:10, topic:56672"]
Maybe set your focbox’s for 9s, if you haven’t already.
[/quote]

This :point_up_2:t3: Voltage goes down to 30.8v at 5:35:12

The focbox is hitting 84c so it may throttle just a little at that temp but no cutoff. 

Some focboxes came with a plastic film over the thermal transfer pads, might be worth checking that also.
```

---
## \#12 Posted by: cliofreak Posted at: 2018-05-25T10:06:36.189Z Reads: 303

```
Thanks, Ill set it to 9s till my new cells and BMS come. 84c seems high though. Maybe ive just never checked Focbox temp after 6 steady miles.
```

---
## \#13 Posted by: cliofreak Posted at: 2018-05-25T13:15:10.474Z Reads: 297

```
So, I reprogrammed the Focbox and set to 9s. I put conservative settings on it.

The motor stuttered and shut off/on under medium load.
I stopped after 200mtrs and the motor was too hot to hold hand on and the VESC was already close to 80deg C.

Im sure having a 10s4p with a dead pack in there and calling it a 9s in settings cant be good!?
I know the next step is new BMS and new pack of 4 18650s. Ugh... rewiring that will be a pain. 

I just really really really hope that the Focbox isn't screwed because of dud battery.
```

---
## \#14 Posted by: Mathias Posted at: 2018-05-25T19:57:00.079Z Reads: 275

```
I'm pretty sure you are looking at two separate problems here. Overheating should not cut, but only reduce the power. There is a battery issue. But this doesn't explain the extreme heat of the FOCBOX or the motor. Please post your settings. The last time I saw someone with this issue, the problem was that he had set the motor to "sensored" instead of "hybrid".
```

---
## \#15 Posted by: cliofreak Posted at: 2018-05-25T21:04:46.844Z Reads: 268

```
Yeah, I have mine set to 'sensored'. I've never heard of anyone setting it to 'hybrid'! Is that a thing if you're running a sensored motor?

Its weird... before I changed settings to 9s (due to the bad pack in the 10s obviously) it didnt 'cut' the motor. It was more like real voltage sag like I used to get from the old 4.x Vesc when going up hill with the big wheels on. It was still hot but I only checked it after 6 miles (when it started sagging). I'd never noticed any heat before when powering off before.

Now that ive changed to 9s in settings, its fine if rolling gradually on flat but if I jam on power it 'cuts' and almost throws you forward... and it gets crazy hot in a short time.

Bad charger? Bad Focbox? Bad settings? Bad BMS? Bad Cells? 

There is an argument for all of these. For example, when I plug in my charger to my other 10s2p build, it stays green, rather than red even when there is only 50% charge and it refuses to begin charging straight away. It eventually works. 
I do recall a time when I shorted the charger by testing the polarity on its tip with a multimeter. This was when I was building and wiring the 10s2p board (8 months after the 10s4p... that had no issues prior to this event... I think. Issues certainly began in the same week or two of this event). Could a briefly shorted charger (that still works, eventually) cause a bad pack, therefore a bad Focbox, therefore an overheating motor, therefore a sagging/cutting. Jeez. What a head melt!!
```

---
## \#16 Posted by: Mathias Posted at: 2018-05-25T21:13:57.444Z Reads: 248

```
[quote="cliofreak, post:15, topic:56672"]
Yeah, I have mine set to ‘sensored’. I’ve never heard of anyone setting it to ‘hybrid’! Is that a thing if you’re running a sensored motor?
[/quote]

"Sensored" is definitely never the right choice for eskate. What you want is hybrid. This means the VESC uses sensored for increased startup torque and then switches to sensorless at high ERPM. This is the way it should be. This will certainly cause overheating motor and FOCBOX. From the telemetry you posted, it looks like riding that should barely heat the motor or the FOCBOX at all, if everything is configured correctly. 
The hard cutoff that you fell could be the motor overheating. I don't know what's the result of that. But the FOCBOX overheating causes a soft cutoff, meaning a gradual reduction of power. 

So please switch to hybrid mode. But it definitely seems like there is some funny-business going on with you battery - even if this is unrelated to your heat issue. Check your balance cables, the individual cell voltages, your charger etc...
```

---
## \#17 Posted by: cliofreak Posted at: 2018-05-25T21:25:44.882Z Reads: 240

```
Thanks man! 
I'll change to hybrid (I dont even recall that option!). Makes sense, what youre saying although it didn't cause any issue before... unless thats whats caused the problems now! I've done a few hundreds miles on sensored with no apparent issue. 

I've ordered new cells and a BMS. I'll be rebuilding the battery anyway to rewire the BMS so I should be checking everything. Till then, I guess I'll just park it up. Don't wana mess anything up further!.
```

---
## \#18 Posted by: Mathias Posted at: 2018-05-25T21:35:48.170Z Reads: 246

```
[quote="cliofreak, post:17, topic:56672"]
I’ll change to hybrid (I dont even recall that option!). Makes sense, what youre saying although it didn’t cause any issue before… unless thats whats caused the problems now! I’ve done a few hundreds miles on sensored with no apparent issue.
[/quote]
Well it for sure also caused way more heat than it should before, and therefore wasted a lot of battery power. You probably just didn't overheat the motor yet. Once you fixed up your battery, have a try in hybrid. The power and the range should be a day and night difference for high speed/high power riding!
```

---
## \#19 Posted by: dareno Posted at: 2018-05-26T08:07:59.154Z Reads: 239

```
Hey, sorry to hijack your conversation but that really sounds like a great innovation,hybrid mode.  I used to experience a flat spot of acceleration with sensored motors as opposed to unsensored.  It was smoother yes but felt less powerful so i unplugged the sensors and adjusted the programming to suit but still experienced a little cogging.  more power but cogging.  i'm just about to start programming my dual focboxes and am using 200kv 6374 motors and as i understand it the hybrid will allow smooth take off but then let go to achieve full motor revolution at top end.  Is this the case?
Thanks for the heads up!!
```

---
## \#20 Posted by: Mathias Posted at: 2018-05-26T15:27:23.285Z Reads: 230

```
Yes, that's exactly the point of hybrid mode. Unsensored is more efficient at high ERPM, and sensored mode has good torque at stand-still. Hybrid is meant to give you the best from both worlds. Sensored mode is NEVER a good choice on an eskate!
```

---
## \#21 Posted by: cliofreak Posted at: 2018-05-27T00:02:54.306Z Reads: 224

```
How do you even setup hybrid mode? I had a look on Vesc Tool and I dont see it as an option!
```

---
## \#22 Posted by: mmaner Posted at: 2018-05-27T00:18:35.062Z Reads: 211

```
Select FOC on the Motor tab, then Hybrid on the BLDC tab.
```

---
## \#23 Posted by: mmaner Posted at: 2018-05-27T00:20:05.802Z Reads: 215

```
[quote="Mathias, post:20, topic:56672"]
Sensored mode is NEVER a good choice on an eskate!
[/quote]

Just off the top of my head...a short board cruiser built for carves & people slalom, not high speed, would definitely benefit from sensored FOC.
```

---
## \#24 Posted by: Mathias Posted at: 2018-05-27T01:39:23.584Z Reads: 215

```
[quote="mmaner, post:22, topic:56672, full:true"]
Select FOC on the Motor tab, then Hybrid on the BLDC tab.
[/quote]

That's not hybrid mode. That's going to use FOC and completely ignore your BLDC settings. Hybrid mode means hybrid between sensored BLDC and unsensored BLDC mode. I was under the impression @cliofreak is using BLDC mode, not FOC?

[quote="mmaner, post:23, topic:56672"]
Just off the top of my head…a short board cruiser built for carves & people slalom, not high speed, would definitely benefit from sensored FOC.
[/quote]
Doesn't matter if you are using FOC or BLDC. After takeoff, sensors should be switched off. There's no benefit from the sensors after that. All it does is waste energy and produce extra heat. 
"Sensored FOC" in that sense doesn't even exist. It's always sensorless or hybrid, unless you set the switching frequency so high, that it doesn't happen. But that's would be a pretty bad idea.
```

---
## \#25 Posted by: Mathias Posted at: 2018-05-27T01:42:58.308Z Reads: 199

```
[quote="cliofreak, post:21, topic:56672, full:true"]
How do you even setup hybrid mode? I had a look on Vesc Tool and I dont see it as an option!
[/quote]
Motor settings -> Motor type -> BLDC
and
Motor settings -> BLDC -> Sensor Mode -> Hybrid
```

---
## \#26 Posted by: mmaner Posted at: 2018-05-27T01:47:11.035Z Reads: 195

```
I'm not gonna argue with you, but your wrong.  Maybe do a few build then come back either some experience.
```

---
## \#27 Posted by: mmaner Posted at: 2018-05-27T01:47:38.139Z Reads: 191

```
I just pulled that out off the top of my head, thanks for looking it up.
```

---
## \#28 Posted by: Mathias Posted at: 2018-05-27T02:01:23.317Z Reads: 190

```
Sensor mode for BLDC:
![image|613x140](upload://uHAT7Naz0mQw6HkGTtAP9FwsE1m.png)
Sensorless ERPM for FOC (always enabled, no switching to "pure sensored FOC mode"):
![image|613x140](upload://ywFyYHYLJuESJ5y5J657kKqpl7U.png)
```

---
## \#29 Posted by: cliofreak Posted at: 2018-05-27T10:01:34.777Z Reads: 186

```
Ok I’m confused...

So I’m running FOC. Can I have FOC hybrid as a thing!? 
I can’t stand the coggy, noisey BLDC.
```

---
## \#30 Posted by: Mathias Posted at: 2018-05-27T16:31:03.224Z Reads: 186

```
Ah, I see! When I read about your heat issue I thought you you might be running sensored BLDC, which would explain the problem. If you're running FOC then sensored is fine. As I said: FOC has no pure sensored mode like BLDC. It always uses unsensored above the "Sensorless ERPM for FOC" value (unless you changed the default settings) similar to hybrid BLDC. So this is not the problem.

Your cut-outs will probably be solved once you fix your battery. But it's still weird that your motor gets this hot. Maybe post your settings or try the motor detection again. You have a big motor. Maybe you have to increase the current for the detection. Also probably removing the belt for the detection makes it more accurate.
```

---
## \#31 Posted by: cliofreak Posted at: 2018-05-27T16:44:40.989Z Reads: 180

```
Ive a new BMS and cells coming Tues hopefully. I'll know more when that batt is fixed!
```

---
## \#32 Posted by: Mathias Posted at: 2018-05-27T17:00:26.794Z Reads: 177

```
Cool! Post some updates how it goes. Good luck, man!
```

---
## \#33 Posted by: cliofreak Posted at: 2018-05-31T15:00:32.572Z Reads: 185

```
OK, so I replace the bad pack (What a nightmare... it'd be easier starting from scratch.)
Good news is that its now charging to 100% and I've got 42V. I checked the BMS and I think its fine. I thing the error was that there was a break in one of the nickle strips. If a pack dies again, I'll know that its the BMS for sure.

So bad news...
Im getting a real stutter and shut off on the motor when I try to apply any torque from start off. If I gently take off or push start and gradually climb speed its ok and when its up and running (15mph +) I can hold throttle down fully but from slow speeds its useless. 
This setup used to have a savage torque. It'd launch off the line very strongly (10s4p, 15T42T gearing).

With the bad pack I was topping out at 21mph. Now Im hitting 28mph.

So, any ideas why I can't apply torque at very low speeds!?

I did a mile loop of a park: https://metr.at/r/Q2oPc

SETTINGS:

![IMG_1298|230x500](upload://4vusG17fCvot1vR7D3xOUl45nFX.jpg)![IMG_1297|230x500](upload://443aDdz0dhW6asMVB84nuE4cAzN.jpg)![IMG_1300|230x500](upload://wagdkQJ8lApF7y1pFfmaGSVQxhv.jpg)![IMG_1301|230x500](upload://h0NNFxsKEXkICnXwYju5JKncTdx.jpg)![IMG_1296|230x500](upload://gqPkmUZGinro2mQeWPfYtx5rmIx.jpg)![IMG_1299|230x500](upload://vWICvAKdgoOErWUD7qjEzPZk0fT.jpg)![IMG_1294|230x500](upload://gSnRjTYwi8uWqifHTwy3VPBXtVQ.jpg)![IMG_1295|230x500](upload://zgzgTcNLfHXT8g9LOE5coqKbS5U.jpg)![IMG_1291|230x500](upload://yyKTo64rX9JV2FKb5kWwGvrJ4Ew.jpg)![IMG_1293|230x500](upload://nrtIKuYm64AVRFTRwJMsjmdTx9E.jpg)![IMG_1292|230x500](upload://34vzC8gKzg7QPWf6KCPIpI9AuEN.jpg)![IMG_1290|230x500](upload://6qoUXZEeELDGInjn7jpwO39uQVB.jpg)
```

---
## \#34 Posted by: Mathias Posted at: 2018-05-31T16:33:34.706Z Reads: 167

```
Sensored FOC switches to unsensored at 2500 ERPM, which is something like 1-2 mph for you, so literally as soon as you are barely rolling. If you everything runs fine after you kick once it is probably a sensor problem. You can try doing the FOC sensor detection again, but it sure looks like you did it already. You have a big motor, so you should make sure that the motor easily spins during hall sensor detection. Maybe try to set the current for detection to 10 or 15 A instead of 5. Removing the belt won't hurt either. 

If that doesn't fix it, you could test unsensored FOC. I'm not familiar with that app, what's that? Metr? It doesn't say in your screenshots which is FOC sensor mode but it should be where it says "Sensor mode: Hall", not "hybrid". The hybrid one must be BLDC sensor mode. Anyway, if unsensored FOC improves your startup there is definitely something wrong with your sensors.
```

---
## \#35 Posted by: cliofreak Posted at: 2018-05-31T16:47:04.171Z Reads: 165

```
Yeah, I think its time to try BLDC at least just to try out a different mode. Its not really a 1-2 mile an hour issue. It'll start in FOC no probs but only if I feather the throttle up to 15mph or so. I used to be able to slam on the throttle with exactly the same setup. However, throttle slamming, or indeed even half throttle chokes it up and kinda cuts out/stutters.
```

---
## \#36 Posted by: Mathias Posted at: 2018-05-31T17:01:42.718Z Reads: 161

```
OK, then it's not a sensor thing. This sounds like something went wrong with the motor detection. Try re-doing it for BLDC and FOC. No belts. Increase the current for detection to 10 or 15 A, see if you get the same results as for 5 A.
```

---
## \#37 Posted by: fraannk Posted at: 2018-06-01T09:29:27.502Z Reads: 158

```
Late to the discussion, but did you check that the phase wires have a solid connection? My friend had the same problem, and when he got up to speed, the vibrations at that exact moment made one of the phases stutter, and when he then stopped, there was no problem (unless he wiggled the wires) :)
```

---
## \#38 Posted by: cliofreak Posted at: 2018-06-03T01:21:57.577Z Reads: 153

```
Hey, 
yeah this could be the issue but it seems to happen only on full load. Ive had stuttering motors in the past due to bad connections. This seems different.
```

---
## \#39 Posted by: cliofreak Posted at: 2018-06-18T17:27:08.784Z Reads: 154

```
Just getting around to setting this up again. Ive tried to set it up in FOC and it seems to go OK but then has the same stutter issue when I try to accelerate hard.
However, when I try BLDC mode, it fails on the hall sensor test (bad detection). It also fails when I remove the hall sensor cable and select 'no hall sensors'. It spins up ok etc but fails and judders at the end of the short test. Bad motor!? Its an Alien Power System motor. 6374 200kv
```

---
## \#40 Posted by: onepunchboard Posted at: 2018-06-18T17:34:40.097Z Reads: 151

```
up the duty cycle slowly up to 0.10 and see if it detect. low kv want more voltage for detection
```

---
## \#41 Posted by: cliofreak Posted at: 2018-06-18T22:14:57.886Z Reads: 156

```
So, I upped the duty cycle (even though Ive never had to do that before with this same setup) and it did detect hall sensors on BLDC mode (at 0.09 D). This mean BLDC works ok.

So, I tried to get FOC running again. I did the same thing and when detecting and setting up in VESC Tool, I ran it at 0.05 Duty first and it all went green as usual but when riding it it stutters an cuts off when accellerating hard from zero mph. I redid the VESC TOOL at 0.09 D in FOC mode and it made no difference. ???? Im lost. 

Hall Sensors appear to be working but in FOC mode it stutters on full acceleration from zero mpg. I even checked the belt to see if it was slipping. Thats the kinda feeling it has but its not slipping (as its ok in BLDC mode). Any other thoughts please!?
```

---
## \#42 Posted by: lrdesigns Posted at: 2018-06-19T02:35:56.180Z Reads: 152

```
This might be a shot in the dark but is your receiver or its wires close to the phase wires going to the motor? 

I had an issue with my board once where if I accelerate up a steep hill it would cut out a little, My receiver wires wrapped over the phase wires and when there was a large amp flow it would make the receiver cut out. Rearranged the layout then it was all good.
```

---
## \#43 Posted by: cliofreak Posted at: 2018-06-19T10:33:31.692Z Reads: 147

```
TBH I dont think its the issue in this case. Its more of a sensor wire issue or a bad FOC mode. 
Im wondering if I should try to reinstall the firmware? My gut feeling says there is a motor issue but so often, software makes you think you have a hardware issue!
```

---
## \#44 Posted by: Zyb Posted at: 2018-06-19T11:50:10.860Z Reads: 143

```
i think we have exactly the same problem. bldc motor detection fails at default values but when i up the duty cycle to around 0.09 detection is successful. no problems with normal acceleration from a dead stop but if i hammer the throttle when im cruising at lets say 15kph it makes a massive stutter. with fairly quick acceleration theres no problem what so ever but if i push it too hard i feel its coming :D no problems with braking. this happens both in FOC and BLDC. ive sent my motor for replacement due to another problem but i ll see if the new one makes the same thing. i can narrow down the problem by using another focbox i have and making another phase wire extensions. so motor, cables and focbox is what i can swap other than that i dunno whats wrong with it.
edit: forgot to mention i did a motor detection in bldc tool and detection was successful every time i did it but when i upgraded the fw so i can use it with vesc tool detection failed with default parameters. sadly i did not test it on the road to tell if bldc tool vs vesc tool makes any difference. because on the bench theres no problem with hard acceleration it only happens when theres a load
```

---
## \#45 Posted by: cliofreak Posted at: 2018-06-19T15:43:32.706Z Reads: 134

```
Yip, sounds spot on to me. Same issue! Mine is fine to smash throttle after about 10mph but anything below it stutters and shuts of till i release trigger and reapply gently.
Keep me informed and ill do the same to you!
```

---
## \#46 Posted by: Zyb Posted at: 2018-06-19T15:56:44.839Z Reads: 137

```
All right, my new motor is on it’s way to me I ll report back. When I get it I won’t change anything to see if the motor was the problem and go on from there. I’m suspecting it was a tiny strand touching inside the motor or I have a cold solder joint in my extensions but that’s highly unlikely as I inspected each one of them when I was making them.
```

---
## \#47 Posted by: cliofreak Posted at: 2018-06-19T15:57:10.859Z Reads: 133

```
I should also add that on the bench, even with belt on, its completly fine to smash the throttle. I've even tried holding the wheel with a towel to simulate load and its fine. Its clearly not enough load to replicate the issue.
```

---
## \#48 Posted by: Zyb Posted at: 2018-06-19T15:57:48.623Z Reads: 133

```
Lol I tried exactly the same thing same result
```

---
## \#49 Posted by: Mathias Posted at: 2018-06-19T16:53:19.740Z Reads: 134

```
[quote="cliofreak, post:43, topic:56672"]
TBH I dont think its the issue in this case. Its more of a sensor wire issue or a bad FOC mode.
[/quote]
@lrdesigns has a point. 10-15 mph is too high to be sensor related, the motor detection worked fine, and you guys don't get a fault code. The only other thing that I can think of that can cause this crap without throwing a fault is the receiver.  
The fact that the problem's gone after a certain speed suggests that it happens at high motor current or fast changes of the motor current. After a certain speed, the battery current becomes the bottle neck instead of the motor current. 

Rearranging is one way to improve it, but a ferrite ring around the PPM cables is also a good idea.
```

---
## \#50 Posted by: Zyb Posted at: 2018-06-19T17:26:05.060Z Reads: 129

```
I have another receiver also got a gt2b remote going to use it’s receiver too see if that makes any difference. Expecting the new motor next week so I can test these options
```

---
## \#51 Posted by: cliofreak Posted at: 2018-06-19T18:18:31.774Z Reads: 127

```
Yeah, I could try moving receiver but I know it’s pretty far from phase wires... I think. 
The issue isn’t at 10-15 mph, it’s at speeds lower than that. 0-10 mph where if you squeeze trigger gradually, you could get to 25mph no issue but if you squeeze hard from 0mph it jumps to 2 or 3 mph then stutters and stalls. 
If you squeeze hard at 15 it’s got no issues.
```

---
## \#52 Posted by: Mathias Posted at: 2018-06-19T18:33:13.103Z Reads: 128

```
[quote="cliofreak, post:51, topic:56672"]
The issue isn’t at 10-15 mph, it’s at speeds lower than that. 0-10 mph where if you squeeze trigger gradually, you could get to 25mph no issue but if you squeeze hard from 0mph it jumps to 2 or 3 mph then stutters and stalls.
If you squeeze hard at 15 it’s got no issues.
[/quote]

That's my point. Squeezing hard at low speeds means high motor current. At high speed the battery max limits the motor current, which would explain why the problem goes away at high speeds.
```

---
## \#53 Posted by: cliofreak Posted at: 2018-06-20T08:49:22.601Z Reads: 126

```
UPDATE:

So, I moved the reciever and placed it far from any major current and it made no difference unfortunately.

It also got me thinking about my description of the error in more detail...
It actually stutters from very little throttle from the get go. 1 or 2 mph its ok then around 3mph it just fails, stutters and you have to release throttle and start again, teasing it up to around 10mph where its got enough momemtum to allow full throttle (or indeed where its past the sensors use). 

It feels like a car engine thats being flooded with petrol, causing misfires. You have to tease it with power till you get momentum, then its fine. Any other ideas welcome. I have a feeling, if I had another sensored motor to test, it'd be fine. I only have a non sensored Hobbyking 6374 SK3 150KV and its not worth swapping over.
```

---
## \#54 Posted by: cliofreak Posted at: 2018-06-21T21:46:10.648Z Reads: 118

```
Ok,
What would allow a motor, battery and FOCBOX all to work perfectly when using BLDC mode but stutter when accellerating from very slow speeds in FOC mode??

You'd say sensors... right!?
But sensors pass the hall sensor test in BLDC mode and give all green in FOC mode in Vesc Tool.  
Stumped!
```

---
## \#55 Posted by: lrdesigns Posted at: 2018-06-22T06:46:13.151Z Reads: 113

```
Can you try FOC mode with sensored turned off in vesc tool and unplugged?
```

---
## \#56 Posted by: cliofreak Posted at: 2018-06-22T08:32:47.291Z Reads: 117

```
Ive quickly tried FOC mode 'sensorless' and it was no different. I used Perimetr (iPhone app) to load a pre-saved version I had so I have now tried what you suggested however, I didnt open the enclosure and remove the sensor plug. I dunno if that would have made a difference!?

Anyway, unfortunatly the problem continues.
```

---
## \#57 Posted by: lrdesigns Posted at: 2018-06-22T08:48:30.956Z Reads: 119

```
Yeah un-plugging the sensors shouldn't make a difference, its just nice to be 100% sure you have illiminated a potentiality issue. 

So weird, it seems like a sensor issue as it goes away after you pic up speed and get into the sensor-less speed range. 

So you fixed the battery, and is the over heating issue also gone? Maybe change your tittle to focbox slow speed stuttering in FOC mode. 

But it works in BLDC mode just fine? 

This leads me to 3 possible causes, bad sensors, bad motor or software issue. 

If it works in BLDC there seems like there is no reason not to work in FOC except for a software issue. This might be a pain in the a** but maybe erase all settings and try a different firmware?????
```

---
## \#58 Posted by: cliofreak Posted at: 2018-06-22T08:52:43.379Z Reads: 113

```
Yeah, I was thinking reinstall the firmware. Cant bear the thought of going through it all again haha.
BLDC is fine. No overheating (well, in the relativly short test run of a mile or two). I'll get a good run on it today in BLDC and see if its actually not overheating.
```

---
## \#59 Posted by: cliofreak Posted at: 2018-06-26T22:29:59.294Z Reads: 117

```
Update,

So, Im back to only charging to 60%. That means Ive blown another connection and a set of 4 18650s are most likley doomed... another £20 wasted never mind the rebuilding effort. The nickel strips I'm using are relativley thick and posed no issue before I was having other issues. 

The motor gets warm in BLDC mode when ridden for a mile or two. It also becomes very hard to move (Its pretty impossible to roll the board when not applying power to motor - after a mile or two or riding). Focbox is hitting 83deg C after just a couple of miles. 

So, heres my guess...

The motor is to blame for everything. The FOCbox overheats because the motor is 'sticking' and requires extra strain to turn. The nickel strips are breaking like a fuse, due to the extra constant amps its needing to draw to turn the bad motor.

I dunno. My Metr app didnt save the data today so I cant see the stats but it felt like the last time its was only charging to 60% and nobody on here mentioned anything about the stats of the motor the last time I shared that data.

I know Ive got the amps set high for the battry but at 80A I dont think its excessive. Maybe I just need to rebuild batt and double up on all strips.

Still, doenst explain the cogging in FOC even when battery was mended last time.
```

---
## \#60 Posted by: Sender Posted at: 2018-06-26T22:51:07.485Z Reads: 116

```
Are you sure FOC is working properly? Mine was good for 40 miles then the sensor board went out on me....also, where are you? 

 It is getting hot as hell here in alabama and when I was riding harder, my temps would climb into thermal throttling range pretty quickly.  @deckoz also mentioned some demagnatization on the motors at these higher temps.  Even magnets swapping poles causing lock up.  

Obviously not your battery problem, but something to think about in these warm summer months.
```

---
## \#61 Posted by: cliofreak Posted at: 2018-06-26T23:01:07.963Z Reads: 117

```
Cheer,
Nah Im in Ireland and although this week is in the 80s, its abnormally hot.

This has been going on a while and its been pretty crap weather untill this week.
Id hate to think the FOCBOX is potentially bad. I guess I'll fix battery (AGAIN!) and then swop out the Alien Power Sys motor Ive in there and put in the SK3 150kv I've got sitting in a box. If the same issues happen again, it'll be the foxbox.
```

---
## \#62 Posted by: wafflejock Posted at: 2018-06-26T23:24:44.537Z Reads: 116

```
Would be curious how often you're pulling anything near 80A would really be good to get some metr data to see how long it's staying at high amps.  Personally would be concerned about the nickel strips burning up and taking cells with them (chain reaction).  Think while things are acting weird till you replace motor or get more data on why the nickel strips are failing would reduce that max amperage.  Also I'm a small guy on flat land but I never pull that many amps (single drive 6374 149kv turnigy sk3, 10S) https://metr.at/r/GLCvO
```

---
## \#63 Posted by: cliofreak Posted at: 2018-06-26T23:57:07.074Z Reads: 120

```
Well, here is some data from last time it saved properly. During this run, the board got really slow near the end and it was the last time FOC mode was working correctly. I then fixed the battery (was only charging to 60% and had a break in nickle and bad pack). When I rebult it all, FOC mode was stuttering hense this thread. As you can see at the beginning of this run, its only at 37.8 on full charge (10s4p). So, the break in nickle happened in a previous run. I didn't notice it as it kept running ok on what was essentially 9s.

https://metr.at/r/GMV4s
```

---
## \#64 Posted by: sofu Posted at: 2018-06-27T00:02:05.539Z Reads: 118

```
Could it be a shorted motor? I've heard of similar issues but on a hub motor... (Motor barely turning, cogging, super hot to touch, focbox extremely hot. I'm not an expert!)
```

---
## \#65 Posted by: cliofreak Posted at: 2018-06-27T00:04:14.895Z Reads: 120

```
I dunno. Motor works to an extent. Dunno if shorted motor would work at all.
```

---
## \#66 Posted by: sofu Posted at: 2018-06-27T00:05:23.381Z Reads: 124

```
The shorted one also worked to an extent... it would just burn through battery like nothing else...
```

---
## \#67 Posted by: Sender Posted at: 2018-06-27T00:43:36.973Z Reads: 118

```
How did short?
```

---
## \#68 Posted by: sofu Posted at: 2018-06-27T01:12:31.914Z Reads: 115

```
As far as I understand, something inside the motor broke and shorted. It wasn't anything you can fix externally
```

---
## \#69 Posted by: cliofreak Posted at: 2018-06-28T22:47:28.073Z Reads: 109

```
So, Ive repaired the battery today. What a pain!! Like surgery.
Anyway, its now fixed and charging to 100%. 
Interesting... there was no break in the nickel. It didnt blow! I'm going to now blame the BMS for the dead pack. I was gonna replace it last time I has a bad pack but because I thought I saw a break in the nickel, I  blamed that and didn't replace the BMS.

So, BMS is replaced. We'll see if it holds out.

I still have stutter in FOC mode and BLDC is totally fine.
Here is a metr stat from today in BLDC mode. All mostly flatish ground in 28C deg heat. Motor was quite warm at the end.

Anyone see any issues that might hint at the warm motor and the FOC stutter?

https://metr.at/r/7Qtg7

![IMG_1710|666x500](upload://wVclFuaz0r8IHnu4GB4bIVoaMlb.jpg)![IMG_1711|666x500](upload://3yvzMIVO8CYBcIRmUCgQ8BHdJsv.jpg)
```

---
## \#70 Posted by: lrdesigns Posted at: 2018-06-29T01:06:04.594Z Reads: 102

```
Does your motor have a temp sensor? Because I can see it in the graph. The graphs look fairly normal to me, maybe your just to heavy for a single, or too much of a speed junkie for this setup. 

The focbox does get pretty close to 80c near the end. 

Why it only stutters in foc suggests the issue is in the foxbox.
```

---
## \#71 Posted by: cliofreak Posted at: 2018-06-29T01:24:22.607Z Reads: 101

```
Yeah, I'm about 160lb. Maybe I just need a double setup. I have a Maytech vesc in another build that I might put in this for an hour to see if FOC works ok with my current motor. It has different size bullets connectors so I'll have to make adapter cables.

Its so hard to keep track of my setups and figure out when it all went wrong...

15/36T with Maytech Vesc (83mm, 90mm and 100mm wheels)
15/42T with FOCBOX (83mm, 90mm, and 100mm wheels) 


Flat smooth park ground, my fav was 15/42T with FOCBOX 83mm wheels. HUGE torque but maxed out at 20 mph.

Truth is, the best by a mile on various surfaces is 15/42T with FOCBOX 100mm MBS. Very acceptable torque and still 25mph. It just hammers over sticks and stones with ease and very little vibration. I just wish I had FOC mode working again!
```

---
## \#72 Posted by: Zyb Posted at: 2018-07-04T15:26:13.765Z Reads: 96

```
I experience a stutter at hard acceleration aswell. So far swapped motors, focboxes, made a second set of phase wire extensions, tried foc - bldc, vesc tool, bldc tool. Nothing makes a difference. Battery seems to be fine as it charges normally. Motor turns without a problem and it’s smooth. Using 30qs and supower bms as well as an anti spark switch. These are the ones left to change but I feel like I won’t bother anymore it’s not a major issue.
```

---
## \#73 Posted by: cliofreak Posted at: 2018-07-05T11:31:11.377Z Reads: 83

```
Sounds like a PITA. Yeah, mine is currently fine in BLDC mode. If I knew a simple fix to get FOC working again I would do it but Im fed up trying now.
```

---
## \#74 Posted by: Benjamin899 Posted at: 2018-07-05T11:36:50.059Z Reads: 82

```
those batteries look weird. i havnt' seen such markings till now, the others look normal. source legit?
Also is your motor with or without sensors?
```

---
## \#75 Posted by: cliofreak Posted at: 2018-07-05T11:43:20.894Z Reads: 83

```
The source for those 30Qs was www.18650.uk
The kinda white marks on them is glue residue.
The motor is sensored, yes.
```

---
## \#76 Posted by: Zyb Posted at: 2018-07-05T11:57:21.876Z Reads: 82

```
For my second build I will use different motor, bms, battery brand, simple xt90 anti spark, motor mount etc and see if the problem persists :slight_smile:
```

---
## \#77 Posted by: banjaxxed Posted at: 2018-07-14T13:03:44.128Z Reads: 75

```
Try swapping the remote and receiver?
```

---
## \#78 Posted by: Airwolf Posted at: 2019-11-03T16:46:36.005Z Reads: 12

```
Hey Guys,

I had the problem where if you try to pull the throttle trigger hard from a stop or a really slow roll then it stutters. 

Here's how I fixed it: 

STEP#1: I went in to the FOCBOX UI, went to "Remote Config" > "Advanced Throttle Config" > "Positive Throttle Ramping Time" > (Increase from 0.30 to 0.55 seconds.)

STEP#2: I went in to the FOCBOX UI, went to "Remote Config" > "Advanced Throttle Config" > "Negative Throttle Ramping Time" > (Increase from 0.10 to 0.25 seconds.)

STEP#3: While You are in the FOCBOX UI, "Remote Config" > "Advanced Throttle Config" menu, try setting your "Traction Control" = (Disabled). 

I think STEP's #1 and #2 will solve your problem, but Step #3 is how I have mine so might want to try your Traction control setting to Disabled also.

*Like I mentioned, changing the Positive and negative throttle ramping time fixed my off the line stuttering problem. My thinking at the time had been, if I am at a standstill or moving slow, and I try to hammer the throttle, the board will be unable to achieve the acceleration that I am specifying with the throttle in the time allowed for that acceleratin to be achieved as specified by the positive ramping time. So I gave the acceleration a little more time to achieve the setpoint input from the throttle. I.E. 0.55 seconds instead of 0.30 as comes default on Focbox. this means the current to the motor will be applied a little more slowly also. 

However, to the rider, the difference between 0.30 seconds and 0.55 seconds isnt much. But to the controls, it means almost twice as much time to complete the change from a stop to the acceleration set point being specified by the Throttle Trigger.  So try that. Might even go out to 0.60 seconds on the Positive Throttle Ramp to see if the stuttering is reduced. 

Or, if all else fails, apply the throttle a bit more gradually from a slow speed. 

Have a nice day.
```

---
