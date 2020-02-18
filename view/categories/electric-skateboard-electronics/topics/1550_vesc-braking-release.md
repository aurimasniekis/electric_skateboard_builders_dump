# VESC Braking (release)

### Replies: 102 Views: 11957

## \#1 Posted by: dogeatgod Posted at: 2016-02-26T14:56:14.053Z Reads: 506

```
Upon braking all seems fine but then after a couple of seconds braking releases (freewheels) – This is happening regardless of speed.

Has anyone else come across this or can think of a solution?

192kv motor - 10S 8000mAh (2 x 4000mAh)
Max charge rate 5C – 4000mAh = 20A
Max Current = 80A
VESC settings:-
Motor Min (regen)    	-30
Batt Min (regen) 	-20

Increasing Motor Min (-40) braking is stronger but release still occurs.

Thanks in advance
```

---
## \#2 Posted by: thomwithah Posted at: 2016-02-26T23:52:19.450Z Reads: 468

```
I'm not an expert, but I thought I'd ask.... Are you using a BMS that protects you from overcharge? Does this always happen? Meaning when the battery is full, <90% full, and >30% full? Basically, are you sure your not hitting some overcharge protection?
```

---
## \#3 Posted by: Braylon31 Posted at: 2016-02-27T06:20:42.912Z Reads: 454

```
Yea ive heard if you use a lit of brakes on a fully charged battery you could kind of over charge your battery from the regin brakes cuasing bms to cut off batteries 

Unless your using the unreliable wii remote! Ha ha :)
```

---
## \#4 Posted by: dogeatgod Posted at: 2016-02-27T07:39:09.765Z Reads: 444

```
Not using BMS. 

Whatever is occurring is a response from the VESC.

If it's overcharge I'm not too worried as peak will be for a matter of seconds. I'll get some data next week and work out peak A under normal braking.

I'd rather protect my life stopping reliably than the life of the batteries

Thanks for replies - will post results soon.
```

---
## \#5 Posted by: dogeatgod Posted at: 2016-03-11T12:15:49.855Z Reads: 425

```
OK - I think I know what’s been going on

VESC was configured when GT2B controller was in original housing I then rehoused inners into a Badwolf enclosure.

I’d cut away part of the Badwolf trigger guard to allow for better movement, this increased the range of the brake – BLDC pulse width range is now between 0.58 and 2 – previously 1 and 2. 

I expect when braking in range of 0.58 and 1 without correct configuration caused brakes to fail.

When reconfigured to range of 0.5 and 2 the motor span when controller trigger in rest position – this, I believe, is because the new trigger movement range is biased to brake - 2/3rd brake 1/3 drive and VESC rest position is midpoint.

<img src="/uploads/db1493/original/2X/7/74071857bb36eaa8c2ffcee387f6a58dd84b0739.jpg" width="690" height="266">

Solution - install a brake stop for trigger on badwolf enclosure and return pulse width range to between 1 and 2.

If I’m an idiot and have missed something obvious please let me know.
```

---
## \#6 Posted by: treenutter Posted at: 2016-03-13T03:07:16.123Z Reads: 396

```
@dogeatgod I have the same problem occasionally when braking in FOC mode. I also use a gt2b with the badwolf mod. I'll do some tests to see if it happens only when my battery is fully charged. If it is the case that the regen from braking is exceeding one of VESC's protective thresholds, then it seems like the solution would be to modify braking force or the regen settings. 

Your solution of limiting the trigger swing might solve the issue, since you would not be able to reach the max brake. But it seems like having access to the full range of motion of the trigger would give us more precision in braking.

It's also possible that when you moved the gt2b into your badwolf case, you might have inadvertently moved the throttle trim dial. This could explain the new min and max pulsewidth settings for PPM.
```

---
## \#7 Posted by: dogeatgod Posted at: 2016-03-13T19:16:49.821Z Reads: 392

```
I used a square of medium density foam as a trigger stop, this returned range to as before, and everything is tickity-boo.

Previously cut outs occurred regardless of battery charge or incrementally increasing regen settings, up to Motor -55 / Battery -30. 

Adjustments were made to throttle trim – this kept the same pulse width range just moved pulse width band (max and min pulse width changed / range remained same)

I’ve a spare GT2B so could revert back and look for differences but as I’ve solved my issue it seems a little pointless, that is, unless others would find the information useful.

Please let me know how you get on.
```

---
## \#8 Posted by: FLATLINEcustoms Posted at: 2016-03-14T14:29:29.209Z Reads: 378

```
I just finished my build on Saturday with GT2b to BadWolf v2 case and had the brakes cut out on a hill. Kinda scary at the moment you need brakes.
```

---
## \#9 Posted by: treenutter Posted at: 2016-03-14T15:01:12.830Z Reads: 374

```
@dogeatgod I did some testing this weekend. Here's what I found: if I'm moving at a slow speed, and I push the brake trigger a little too hard, I can reliably trigger the VESC to shutdown and reboot.

The same thing happened when I was using a nunchuck, but it is less problematic and easier to control with the GT2B. But it still should be fixed!

My hypothesis is that the the amount of incoming energy from the motor during braking\regen is exceeding the threshold set in BLDC Tool, so the vesc shuts down to protect itself. I am running a pretty high reduction ratio of 14:60, so that may contribute (the motor spins faster than a typical eskate while coasting and braking). I don't think this is related to max battery capacity settings, because it happens even when the battery is half depleted. 

Anyone with more VESC experience have thoughts about this? @chaka @elkick ? I'm not exactly sure which setting should be modified, but I'm thinking it is "motor min" and "batt min" [per this thread][1] by @onloop. 

If I'm careful with the brake (i.e. I don't push it too hard) I can safely ride as it is, but it would be better to dial in the settings so that it less likely to happen. 

I'm going to try reducing the braking force to see if it plays better with the pulse width min of GT2B. Will report back.

BTW - the shutdown\restart only happens at very slow speeds or a stop. If I pushed the brake trigger at a high speed I get belt skipping or I get tossed off!


  [1]: http://www.electric-skateboard.builders/t/vesc-faq-regen-braking-configuration-bldc-tool-brake-force/353
```

---
## \#10 Posted by: trbt555 Posted at: 2016-03-14T15:06:08.774Z Reads: 340

```
Do you have the same issue in BLDC mode ?
```

---
## \#11 Posted by: dogeatgod Posted at: 2016-03-14T15:07:26.955Z Reads: 342

```
There may be something out of kilter with your VESC settings or controller set up – if you can share your set up (motor/battery), VESC battery/motor regen information and min/max pulse width for RC that would be useful.
Hopefully it will be an easy fix, like mine.
```

---
## \#12 Posted by: treenutter Posted at: 2016-03-14T15:08:48.409Z Reads: 329

```
@trbt555 good question; I will test it again, but I don't recall experiencing this in BLDC mode. However, I don't want to switch away from FOC mode. I love the smooth starts and the quiet operation.
```

---
## \#13 Posted by: treenutter Posted at: 2016-03-14T15:11:11.048Z Reads: 315

```
You're in the right place @FLATLINEcustoms, we're trying to figure this out as well!
```

---
## \#14 Posted by: elkick Posted at: 2016-03-14T15:15:35.030Z Reads: 309

```
Are you on 2.16? If not, give it a try, FOC motor detection seems to be better now. Also, is breaking on -20? What's happening when you go lower?
```

---
## \#15 Posted by: trbt555 Posted at: 2016-03-14T15:28:10.177Z Reads: 302

```
Just imagine how easy this kind of troubleshooting will get once @jacobbloy finishes the Android BLDC app !
```

---
## \#16 Posted by: treenutter Posted at: 2016-03-14T15:29:46.540Z Reads: 307

```
Thanks @elkick I'm on 2.15, so I'll apply the new firmware and try again. I haven't modified the breaking force from default yet; that might be the fix! I'll let everyone know. 

As a side note; I feel like a useful addition to BLDC Tool would be inputs for battery voltage and capacity that would work with the PPM or nunchuck inputs to help users figure out whether cutoff thresholds should be modified. It doesn't seem like it would be very hard to add, and it would be a major help as people start using VESC in higher volume. You only need to experience one cutoff to know that it is pants-shittingly scary to have your ESC reboot unexpectedly. Who is friends with Vedder? @jacobbloy don't you work with him directly? Maybe we can share this idea?
```

---
## \#17 Posted by: trbt555 Posted at: 2016-03-14T15:40:03.861Z Reads: 293

```
There's a "feature request" section on Vedder's forum.
```

---
## \#18 Posted by: dogeatgod Posted at: 2016-03-14T16:08:48.947Z Reads: 306

```
@treenutter thank you for update.

When you push the brake trigger too hard do you mean quickly or to extremity of trigger movement?

How quickly does the VESC reset? If I took the brake off and reapplied, braking kicked back in, a delay of a second or so onlyfor trigger movement, if I pushed movement too far braking would drop out again. 

I’m running 14:44 – just for information.

“If I'm careful with the brake (i.e. I don't push it too hard) I can safely ride as it is, but it would be better to dial in the settings so that it less likely to happen.” – when emergency braking is required it’s tricky to remain careful with the brake. I almost went under a car when riding with my braking issue, something went askew between brain, careful and trigger finger.

Reducing motor min made braking stronger but problem remained. I didn’t take batt min as far as I could but the incremental reduction that was made didn't make a difference.

“BTW - the shutdown\restart only happens at very slow speeds or a stop. If I pushed the brake trigger at a high speed I get belt skipping or I get tossed off!” – just to be clear ‘tossed off’ means being thrown from the board? Or is this a form of extreme boarding.
```

---
## \#19 Posted by: treenutter Posted at: 2016-03-14T17:30:48.976Z Reads: 298

```
@elkick just for total clarity; when people say "lower" with the negative brake force values, everyone means that we are going further from zero, right?

Example: moving from -20 to -30 would mean LESS brake force.
```

---
## \#20 Posted by: elkick Posted at: 2016-03-14T18:01:50.790Z Reads: 298

```
With less I meant -15 or so. -30 will apply more.
```

---
## \#21 Posted by: treenutter Posted at: 2016-03-14T18:06:23.118Z Reads: 293

```
@dogeatgod 

[quote="dogeatgod, post:18, topic:1550"]
When you push the brake trigger too hard do you mean quickly or to extremity of trigger movement?
[/quote]

It could be either. I really notice it at slow speed when i push the trigger too far. I think of "hard" braking as a combination of trigger extremity and trigger movement speed. So, braking too hard can force a reboot, and braking too fast can also do it.
```

---
## \#22 Posted by: treenutter Posted at: 2016-03-14T18:07:17.861Z Reads: 281

```
[quote="dogeatgod, post:18, topic:1550"]
How quickly does the VESC reset?
[/quote]


It takes about 1-2 seconds to reboot and then come back to life. Not very long, but long enough that it can cause trouble during a ride!
```

---
## \#23 Posted by: treenutter Posted at: 2016-03-14T18:10:02.774Z Reads: 266

```
[quote="dogeatgod, post:18, topic:1550"]
ust to be clear ‘tossed off’ means being thrown from the board? Or is this a form of extreme boarding.
[/quote]

I mean that the board might stop\reduce speed while my body is still accelerating, so I fall off of it. This was more due to my own bad riding... I was getting used to the braking and applied it too hard.
```

---
## \#24 Posted by: treenutter Posted at: 2016-03-14T18:11:24.824Z Reads: 251

```
Thanks @elkick that's very helpful! I'll try -15 after I update to 2.16.
```

---
## \#25 Posted by: dogeatgod Posted at: 2016-03-14T18:59:26.322Z Reads: 257

```

[quote="treenutter, post:22, topic:1550, full:true"]
[quote="dogeatgod, post:18, topic:1550"]
How quickly does the VESC reset?
[/quote]


It takes about 1-2 seconds to reboot and then come back to life. Not very long, but long enough that it can cause trouble during a ride!
[/quote]

Sounds like this is what was happening to me
```

---
## \#26 Posted by: elkick Posted at: 2016-03-14T19:07:39.722Z Reads: 255

```
[quote="treenutter, post:22, topic:1550"]
It takes about 1-2 seconds to reboot and then come back to life.
[/quote]
Yeah, and during the reboot period it's a very bad idea to play around with the trigger! If the VESC's coming back it continues exactly where your trigger is: if you're on full throttle in this very moment (or full break) it will exactly apply that! 

And believe me, that's beyond your skating skills! Happened to me today and was no fun trying to outsmart physical laws. :wink:
```

---
## \#27 Posted by: trbt555 Posted at: 2016-03-14T19:13:01.164Z Reads: 255

```
LOL.
As you probably realize by now, skaters are constantly nursing road rash on one body part or other 😎
```

---
## \#28 Posted by: RogerD Posted at: 2016-03-14T19:30:17.629Z Reads: 257

```
I wish my board could toss me off.
```

---
## \#29 Posted by: treenutter Posted at: 2016-03-14T20:00:23.256Z Reads: 260

```
@elkick @trbt555 @dogeatgod  Here's something interesting. [Mellow advertises that  their braking system][1] "still works when you are fully charged. Whereas the brakes of a lot of the existing rides actually switch off at that point. Take that for a killer feature."

Holy shit! They are right about that! I'm almost tempted to just turn off regen braking. That would solve the problem for sure. 

<img src='/uploads/db1493/original/2X/9/902cb67ab9e1e2fd9bf11f25dd587880701b4a1e.jpg'>

  [1]: http://www.mellowboards.com/mellow-the-first-electric-drive-that-fits-under-any-skateboard/
```

---
## \#30 Posted by: elkick Posted at: 2016-03-14T20:15:38.766Z Reads: 251

```
Well, they are asking a good uplift for that feature compared with our standard costs, if they remain with those 1.600€ per kit. I don't trust their distance claims though. And they are located in my home town, how comes that I never see them testing their stuff? Would like to compare their sets with mine....
```

---
## \#31 Posted by: treenutter Posted at: 2016-03-14T20:21:50.741Z Reads: 240

```
@elkick agreed! The cost seems really high. Although I'll admit that I like the concept quite a lot and I think it's way cooler that buying a standard mass-market eskate. The swappable frame\battery kit is a very cool idea. I suppose with a standard battery it's not that hard to write some code into the ESC that limits charging once a full charge is present. 

This sounds like another idea to add to the feature request for VESC!
```

---
## \#32 Posted by: dogeatgod Posted at: 2016-03-14T20:22:11.047Z Reads: 239

```
Wow - that's a statement, a known problem then. 

If the regen settings or regen on a full battery is proven to cause brake failure I'm glad I'm not selling these commercially - sounds like just a matter of time before that feature is confirmed. 

I came close to leaving my teeth in a car bonnet.
```

---
## \#33 Posted by: treenutter Posted at: 2016-03-14T20:23:23.894Z Reads: 240

```
@dogeatgod Right, this was my point... it's a known problem. I wonder what all of those lecdec\backfire clones do to prevent this issue; they all have regen (or claim to).
```

---
## \#34 Posted by: trbt555 Posted at: 2016-03-14T20:27:41.020Z Reads: 237

```
Wow, thanks for the link.
Those products look really slick.
I like the idea of the swappable battery pack.
```

---
## \#35 Posted by: treenutter Posted at: 2016-03-14T20:48:58.499Z Reads: 239

```
@trbt555 yes, and they advertise as "water and dust proof" with video of them drive through mud puddles. That is extremely cool, although I sthink that riding on wet roads is a terrible idea in terms of safety.
```

---
## \#36 Posted by: elkick Posted at: 2016-03-14T20:57:58.900Z Reads: 247

```
I think there are some things to clarify with regen braking and VESC, normally it should not go offline at all while breaking. And if it does, I doubt it's related to regen and full batteries. First of all, the regen effect is around 10-15% only and even though the VESC is regen capable, it doesn't apply for speeds below a certain ERPM value.

These are Benjamins remarks about that:  "Max ERPM at full brake in CC mode” is the highest RPM at which applying full brake by shorting all the motor windings is allowed. Setting this value too high can cause much mechanical stress in some circumstances.

So, conventional braking is implemented in the VESC. Assumption: if regen braking fails, it should switch to "conventional" braking, but not reboot the VESC.
```

---
## \#37 Posted by: elkick Posted at: 2016-03-14T21:05:45.215Z Reads: 231

```
Additionally, it's easy to avoid the problem by limiting the BMS on lion batteries to 4.1V for charging. This leaves enough room for regen braking even down a steep hill with "full" batteries.

I think that's exactly what mellow uses to avoid this.
```

---
## \#38 Posted by: treenutter Posted at: 2016-03-14T21:15:57.023Z Reads: 229

```
[quote="elkick, post:37, topic:1550"]
it's easy to avoid the problem by limiting the BMS on lion batteries to 4.1V for charging
[/quote]


thanks @elkick, but I think that the issue I'm having is with an incoming current that is too high while braking, as opposed to hitting the battery's capacity... the same issue occurs for me even when the battery is depleted.
```

---
## \#39 Posted by: jacobbloy Posted at: 2016-03-14T21:51:18.732Z Reads: 234

```
I that read that mellow use a capacitor to dump the access regen to then use it again at next take off.

But what has already been said is true, regen will not reset your vesc, but over voltage will. 

I don't know if any of you are setting your voltage settings or not but if you set your max to the exact same as your battery pack then if there is any spike while braking then you will have a problem.

Are you sure your vesc is rebooting? This could actually be a drv fault for a split few seconds, the red light flashes you can do any thing then every thing comes good. In a lot of HW 4.10 or 4.11 this has been a problem and the solution was adding a extra cap on pad c18 I think. @chaka does this but now there is HW 4.12 that fixes it.

One last thing. I know it is said that changing batt min will reduce braking at speed and motor min will reduce braking at stop and low speed, but I feel there is a big cross over that I discovered while testing my hub motors, braking would just throw me off because it was instant. it is best to try and lower motor min to like -20 and batt min to -10 then go for a test ride if it fixes the cut out then move them up as needed.
```

---
## \#40 Posted by: dogeatgod Posted at: 2016-03-14T22:24:49.919Z Reads: 253

```
I seem to have rectified my problem but whatever caused the brake failure has not been clearly identified. 

If it is voltage spike then adjusting settings should allow the problem to be recreated - before doing this, could it damage either the VESC/battery or would protection (drop out) kick in? 

Not sure if VESC is rebooting – it was only happening under load and it’s not possible to view the VESC whilst driving on my set up. VESC is 4.10 so could be drv fault.

My earlier ESC had “conventional” braking only and never had the brakes drop out.

I hope that root cause can be identified swiftly and knowledge shared to improve performance or prevent an undesirable event.
```

---
## \#41 Posted by: treenutter Posted at: 2016-03-17T01:58:49.999Z Reads: 244

```
@jacobbloy @dogeatgod @elkick thanks for hanging with me as I sort this out!

Tonight I took a look at my VESC settings; here they are on 2.15:

<img src="/uploads/db1493/original/2X/c/c9426a5b5ad2f11f9d0e50538b0c00950da51ddc.jpeg" width="690" height="448">

Tonight I updated to 2.16, ran the FOC motor detection tools, and configured everything again. I did a few things differently; I tried @jacobbloy's suggestion to  move motor min -20 and batt min to -10. I also edited the min pulsewidth for PPM to .9, where it had been set at 1.0 previously. As expected, these changes makes the brakes much softer, it takes more time to come to a complete stop. I have to push the trigger pretty close to the max braking position to trigger a reboot, and I can only do that when I'm moving very slowly or not at all. This seems much better, since it is unlikely that I'll ever use that much braking force on a normal ride.

The obvious downside is that now the braking is much softer than before and I don't have as much control over speed when I'm on the move.

It still seems like something isn't right. What I really want is for the brake to never trigger a reboot in any circumstance. Maybe I should upgrade to a newer VESC that has the upgrade caps? Is it possible that this is as good as it gets using FOC with a 4.7 VESC?
```

---
## \#42 Posted by: elkick Posted at: 2016-03-17T07:40:55.649Z Reads: 227

```
Two questions: Even though it doesn't matter in FOC, why are you limiting max ERPM to 40K? Also, how long are your cables connecting the VESC with the battery in total? This might have an impact especially on FOC.

4.7 should not be an issue with FOC (I'm also driving them in several of my boards), unless you go up to 12s where you will need the C18 mod.
```

---
## \#43 Posted by: dogeatgod Posted at: 2016-03-17T08:18:48.317Z Reads: 228

```
You've got to get this sorted - I drove soft brakes for a few weeks, you get used to it, but having to compensate with total awareness and reduction to speed takes fun and confidence out of a ride. 

My motor min is at -55 and bat min -38 - I've got decent brakes and by mechanically reducing trigger movement have not had a drop out since.

Suggest:-

Putting settings back to previous and trying the wedge of foam technique. If this works you can remove it whilst trouble shooting and replace it for riding. 

Can you borrow a later edition VESC and see if that solves the issue?
```

---
## \#44 Posted by: treenutter Posted at: 2016-03-17T12:13:46.118Z Reads: 220

```
@elkick I limit ERPM when I'm testing settings to keep myself from hitting speeds beyond what I can "run out;" 40K ERPM limits my speed to about 15 MPH, which is fast enough for testing. When I'm done with testing I still keep the max speed at 18-19MPH, even though my build could go faster. 

The cable length between VEC and battery is minimal; although I have a battery arming switch with a button-activated resistor in between the battery and the VESC. Does anyone know what the symptoms are of an excessively long battery cable in FOC?
```

---
## \#45 Posted by: treenutter Posted at: 2016-03-17T12:18:35.889Z Reads: 226

```
Thx @dogeatgod I'm sure that if I limit the swing of the trigger mechanically I will indeed see that reboots don't occur as often. I was aiming for a solution that allows full trigger swing (and thus better braking precison). I'll keeping trying different settings with the motor and batt mins to see if I can dial it 
in. 

I don't know anyone with a VESC in my area to borrow from, good suggestion though!

Could you share a pic of your foam wedge in your badwolf enclosure?
```

---
## \#46 Posted by: dogeatgod Posted at: 2016-03-17T12:52:14.671Z Reads: 226

```
<img src="/uploads/db1493/original/2X/1/17e9194cddb59559ba51a78f81e6149dd639dea2.jpg" width="565" height="480">
<img src="/uploads/db1493/original/2X/e/e3d4798f04b6ba515a8cc66f02fdad6603416c6b.jpg" width="640" height="480">
```

---
## \#47 Posted by: FLATLINEcustoms Posted at: 2016-03-21T20:34:30.471Z Reads: 211

```
Had it happen twice yesterday. The second time I tried to leave the trigger where it cut off and stepped off the board. It immediately shot in reverse, almost like the pause on an electric R/C vehicle stopping and going into reverse.
```

---
## \#48 Posted by: treenutter Posted at: 2016-03-22T00:54:19.943Z Reads: 207

```
@FLATLINEcustoms That sounds like you've got the Control Mode (on the App Config>PPM tab)  set to "Current" instead of "Current no rev w brake" or just "Current no rev." Try setting it to "Current no rev w brake."
```

---
## \#49 Posted by: FLATLINEcustoms Posted at: 2016-03-22T15:38:32.724Z Reads: 210

```
Oh sorry, yes I am running reverse for now. Just definitely a dead zone of over voltage or over heating then boom, reset and back at it.
```

---
## \#50 Posted by: FLATLINEcustoms Posted at: 2016-03-24T13:40:32.850Z Reads: 208

```
I am heading up to the north Georgia mountains in a couple of weeks. If I just turn off regen will it solve the braking issues? Not that I want to, but kind of want a strong reliable brake when I head up there.
```

---
## \#51 Posted by: dogeatgod Posted at: 2016-03-24T16:53:56.691Z Reads: 209

```
When braking the motor acts as a generator and that energy has to go somewhere, so not sure that regen is something you can actually switch off through the VESC, without melting something somewhere else.

I don’t use reverse – I’m finding enough problems with just stop and go as it is. If reverse is not critical then give, as suggested, ‘current no reverse with brake’ a go and try to recreate the brake failure.

@treenutter @FLATLINEcustoms - Just out of interest what is your max and min pulse width with the GT2B? In App Config/PPM turn on display and read full trigger and full brake.

@treenutter – I’ve had a couple of other unresolved issues recently and been tossed off a couple of times, once with @RogerD!
```

---
## \#52 Posted by: FLATLINEcustoms Posted at: 2016-03-24T18:23:08.444Z Reads: 212

```

I am not home to check the display, but this is screenshot of what the settings are.
          
        

<img src="/uploads/db1493/original/2X/4/4b2324b61ea80b6bb2e79dfb5384a63b5185cb42.png" width="690" height="393">
```

---
## \#54 Posted by: FLATLINEcustoms Posted at: 2016-03-25T22:23:57.028Z Reads: 207

```
Braking was 1.024ms
Acceleration was 2.063

Should I change those settings from 1 min and 2 max? @dogeatgod
```

---
## \#55 Posted by: dogeatgod Posted at: 2016-03-26T15:42:10.298Z Reads: 202

```
They are fine - the range is pretty much 1.

If the range had changed, like mine had, that may have been what was causing your problems.

Did you get a chance to try a run without reverse? if so did that make a difference?
```

---
## \#56 Posted by: FLATLINEcustoms Posted at: 2016-03-28T22:49:25.341Z Reads: 199

```
Couldn't replicate it with the reverse off, yet. It kept braking until drive wheel would lock up.
```

---
## \#57 Posted by: dogeatgod Posted at: 2016-03-29T16:09:24.255Z Reads: 209

```
That sounds positive - keep testing and fingers crossed no more failures.

You could post on [Vedder's Forum][1] to see if a solution can be found that enables you to use reverse.


  [1]: http://vedder.se/forums/
```

---
## \#58 Posted by: FLATLINEcustoms Posted at: 2016-03-30T14:23:27.713Z Reads: 210

```
I didn't know that forum existed. I got tossed off my board, so there will be a few days before I can further test the release of the brakes without reverse enabled.
```

---
## \#59 Posted by: treenutter Posted at: 2016-03-31T12:28:34.523Z Reads: 218

```
@FLATLINEcustoms @dogeatgod @elkick I was poking around on Vedder's forum and found another person noting braking problems that are similar to ours, which lead me to a response form Vedder: [this thread about DRV problems when using FOC][1]

Of note, Vedder suggests soldering an additional 2.2µF capacitor to GVDD on the drv8302 (C18).

<img src="/uploads/db1493/original/2X/7/73826b868b1f8219d0f27a5859b7da2137e5082a.jpg" width="484" height="416">
So I order [some of these from Mouser:][2]<img src="/uploads/db1493/original/2X/d/dc4a8ddedac907f080d5264f27401163bcab8880.jpg" width="150" height="150">

At least one person (Whitepony) reported that it solved their issue with FOC braking. I'll report back once get them in the mail and try it.

@dogeatgod  

[quote="dogeatgod, post:51, topic:1550"]
what is your max and min pulse width with the GT2B?
[/quote]

They are nearly the same as others reported, very close to 1.0 and 2.0. Nothing remarkable.


  [1]: http://vedder.se/forums/viewtopic.php?f=5&t=68
  [2]: http://www.mouser.com/search/ProductDetail.aspx?R=0virtualkey0virtualkeyC1608X5R1C225M
```

---
## \#60 Posted by: elkick Posted at: 2016-03-31T12:59:31.593Z Reads: 210

```
It works with FOC. The C18 mod is basically the update in 4.12.
```

---
## \#61 Posted by: treenutter Posted at: 2016-03-31T13:04:29.996Z Reads: 223

```
Thanks @elkick that's good to know! I hope my soldering skills are up to par! I think I recall that you use VESC HW 4.7 on some of your builds, did you apply this update to your VESC?
```

---
## \#62 Posted by: elkick Posted at: 2016-03-31T13:09:23.151Z Reads: 227

```
Not on the 4.7 VESCs since I drive them only with 7s and 10s with FOC.
 I had the breaking problem as well in 4.7, but it was related to BMS/battery cutting off (too high regen current if batteries are only capable of taking 1 or 2A charge current - changed cells!) and/or wrong settings in the min./max. current in BLDC tool.
```

---
## \#63 Posted by: FLATLINEcustoms Posted at: 2016-03-31T13:30:58.193Z Reads: 221

```
I believe my C18 is double stacked from @chaka. I have 4.11 VESC with the C18 mod.
```

---
## \#64 Posted by: chaka Posted at: 2016-03-31T13:46:43.753Z Reads: 225

```
I use a 4.7uf 16v capacitor instead of stacked 2.2uf caps. Stacking the caps puts too much leverage on the solder pads and could lead to them being ripped off. I have been using these:  http://www.mouser.com/ProductDetail/TDK/C1608X5R1C475M080AC/?qs=sGAEpiMZZMukHu%252bjC5l7YegWuDAL%252b4n3PASDuuxtVww%3d

Mouser is out of stock on the TDX brand but you could use the equivalent from Murata :  http://www.mouser.com/ProductDetail/Murata-Electronics/GRM188R61C475ME11D/?qs=sGAEpiMZZMukHu%252bjC5l7YbA1Uz8mFEbwIIDNOsfvAdY%3d
```

---
## \#65 Posted by: treenutter Posted at: 2016-03-31T13:52:28.063Z Reads: 222

```
@FLATLINEcustoms Dang maybe this won't solve any of my problems. It seems like it is worth a try though, and may improve performance since it is now implemented in the new HW.

@elkick If I apply this hardware update, could I encounter issues with uploading new firmware in the future? That is, are new versions of 4.7 firmware created anticipating that this additional cap is not there... I'd hate to fry my VESC in an effort to improve it!
```

---
## \#66 Posted by: chaka Posted at: 2016-03-31T13:54:44.864Z Reads: 206

```
No you wont have any issues with firmware. It only increases the capacitance making it more robust.
```

---
## \#67 Posted by: treenutter Posted at: 2016-03-31T13:58:05.108Z Reads: 199

```
Thanks @chaka! That's helpful to know!
```

---
## \#68 Posted by: treenutter Posted at: 2016-04-07T15:27:25.188Z Reads: 202

```
@dogeatgod @FLATLINEcustoms @elkick @chaka OK my cap for the C18 mod arrive. This thing is really small! Imagine taking a grain of rice and dividing it into 8 pieces... it looks like a tiny breadcrumb! 

Time to get out the tweezer and magnifying glass. Any pro tips on adding something so small. I have a pretty good soldering kit with the pin-point tip.
```

---
## \#69 Posted by: FLATLINEcustoms Posted at: 2016-04-07T16:42:26.222Z Reads: 196

```
Good luck @treenutter! Hope it works for you.
```

---
## \#70 Posted by: chaka Posted at: 2016-04-07T17:18:19.278Z Reads: 205

```
 I place about a 500 of those tiny little caps and resistors everyday! I use hot air but you can use an iron too. take your time and breath, but not too hard! Once you get the fresh cap in place you can hold it down rather than grasping with your tweezers and touch each end with your iron. There should be enough residual solder on the pads that it will flow with the aid of a little flux.
```

---
## \#71 Posted by: FLATLINEcustoms Posted at: 2016-04-11T20:21:06.344Z Reads: 204

```
@treenutter any luck? I spent Saturday on some steep twistie mountain roads. Didn't have the brake release once with reverse turned off.
```

---
## \#72 Posted by: treenutter Posted at: 2016-04-11T22:33:46.037Z Reads: 207

```
@FLATLINEcustoms @elkick @dogeatgod @chaka I got the cap on there! It's a little bit crooked, but I managed to make a connection on both sides. A few rides have proven successful! The only time I lose braking is if I'm on the board, not moving, and I apply full brake and move the deck forward and backward by shifting my bodyweight. After about six rocks the brakes release. But since that is a behavior that I never need to replicate in real riding, I think I'm good to go! I'm still curious about what causes the release, but I'm happy to be moving in FOC mode!
<img src="/uploads/db1493/original/2X/3/3c01311c2f373eacf66f82a5c2bc234b92badbe5.jpeg" width="500" height="500">
```

---
## \#73 Posted by: elkick Posted at: 2016-04-12T05:15:29.952Z Reads: 191

```
Sounds good. Did you cut those hall sensor pins where your cables are running across on the back side of your VESC? If not, you should do that. They can perforate the insulation of your red wire and full voltage will be applied to the v5 pin of the sensor port and that's bad.
```

---
## \#74 Posted by: FLATLINEcustoms Posted at: 2016-05-25T13:24:15.946Z Reads: 179

```
Mine just released again last night... ugh. No reverse still, maybe it was because I was full throw on the brake?
```

---
## \#75 Posted by: dogeatgod Posted at: 2016-05-25T18:29:33.067Z Reads: 177

```
Bah - worrying. 

Intermittent faults are the worse.

I've not had it occur since limiting trigger movement - fingers crossed it's not just a matter of time.....
```

---
## \#76 Posted by: FLATLINEcustoms Posted at: 2016-05-25T18:30:49.984Z Reads: 177

```
I just posted up over on VESC forum. http://vedder.se/forums/viewtopic.php?f=7&t=222

It has to be the worst feeling on earth... not knowing when the brake is going to fail.
```

---
## \#77 Posted by: elkick Posted at: 2016-05-25T18:36:15.355Z Reads: 178

```
Could be that you are generating voltage spikes when full breaking on 12s exceeding the voltage limit of the VESC in certain parts of it. Just a guess, it didn't happen to me yet.
```

---
## \#78 Posted by: FLATLINEcustoms Posted at: 2016-05-25T18:39:36.812Z Reads: 185

```
I was riding with the battery around 44.2 volts but we have speculated that the regen maybe exceeding the max amperes. Just don't know how to replicate it all the time. Just want it worked out. I like being able to stop when traveling around 36mph when I need to.
```

---
## \#79 Posted by: Michaelinvegas Posted at: 2016-05-25T19:11:15.955Z Reads: 181

```
Did you try riding with 10s and see if it happens again? Of course please try it in a parking lot ...with bushes at the end.....
For science and possible amusement
```

---
## \#80 Posted by: elkick Posted at: 2016-05-25T19:23:36.456Z Reads: 185

```
Did you try "current no reverse with brakes"? Also, try to lower batt min regen to -30, could also help preventing it.
```

---
## \#81 Posted by: FLATLINEcustoms Posted at: 2016-05-25T19:28:56.574Z Reads: 187

```
I am on current no reverse with brakes I can try to turn down the min regen. What exactly does that control the minimum ammount of current that will regen? Wouldn't I need to adjust max regen?
```

---
## \#82 Posted by: FLATLINEcustoms Posted at: 2016-05-25T19:34:13.184Z Reads: 183

```
@Michaelinvegas I can only do 8s or 12s... Will be willing to try anything for silence as soon as my big toe is healed. Road rash is healed enough I could take some more. Might just put my motorcycle race suit on though....for science of course and record for amusement.
```

---
## \#83 Posted by: elkick Posted at: 2016-05-25T19:37:02.279Z Reads: 184

```
You could do both (batt and motor) yes. Go as low as you can but of course only to a level which still allows full braking. Just to test things and to rule out any spikes.
```

---
## \#84 Posted by: chaka Posted at: 2016-05-26T18:33:23.755Z Reads: 185

```
What type of pack are you using? Capacity and C rating? Have you implemented FOC?
```

---
## \#85 Posted by: FLATLINEcustoms Posted at: 2016-05-26T18:40:10.030Z Reads: 176

```
I have 4 Turnigy 5000mAh 3S 20C lipos in series. No FOC, what would that do?
```

---
## \#86 Posted by: chaka Posted at: 2016-05-26T18:46:55.708Z Reads: 172

```
Sometimes a VESC will behave this way after having been run on FOC. Do you have any way of monitoring the voltage as you apply the brakes?
```

---
## \#87 Posted by: FLATLINEcustoms Posted at: 2016-05-26T18:54:24.611Z Reads: 175

```
In real time on the board... How would one do that?
```

---
## \#88 Posted by: chaka Posted at: 2016-05-26T19:06:55.577Z Reads: 177

```
I thought you had a voltage display on your board? If the voltage is peaking over the VESC's threshold during braking it will reset causing  a loss in brakes momentarily.
```

---
## \#89 Posted by: FLATLINEcustoms Posted at: 2016-05-26T19:18:03.871Z Reads: 175

```
Oh yes I do have that, I thought maybe like a laptop monitoring. It never goes anywhere near peak voltage. I was braking in the mountains last month hard and could never get it to climb over voltage. Never had a release when I was there though...
```

---
## \#90 Posted by: Randyc1 Posted at: 2016-05-27T00:13:58.826Z Reads: 175

```
Battery was charged at 42V (10s) , BLDC Max Voltage set at 43V .

Had this brake issue (brakes letting go after a sec oŕ two) for first time this afternoon. Happened at least 4-5 times in a row. I wld shut badwolf on/off , try again. Then try powering on/off board , try again,..after 4-5 times, braking regained normal function.

Chaka :... if i charge to 42V should I set my Max Voltage a little higher (46-47) v to avoid this brake shutdown fron Regen Voltage peak ??

Also ,...Is there a specific order of powering ON board and controller (badwolf) , should i power ON controller before board?
```

---
## \#91 Posted by: chaka Posted at: 2016-05-27T01:31:02.320Z Reads: 173

```
Are you running with or without a bms? It could also b that your cells are failing and the regen current is causing voltage spikes.
```

---
## \#92 Posted by: Randyc1 Posted at: 2016-05-27T02:34:32.687Z Reads: 178

```
Without bms , battery pack is new.

This was the only time it has done this , battery was full at 42v. Took another ride tonight at a lower charge 40v , ..no problem.

Would have to try this again at full charge 42v and try braking to see if it happens only at full charge?
```

---
## \#93 Posted by: FLATLINEcustoms Posted at: 2016-06-15T22:39:14.190Z Reads: 183

```
Just posted this over on Veeder's forum. 

The following faults were registered since start:

Fault            : FAULT_CODE_ABS_OVER_CURRENT
Current          : -3.5
Current filtered : 131.1
Voltage          : 50.22
Duty             : 0.00
RPM              : 2871.4
Tacho            : 138462
Cycles running   : 27058
TIM duty         : 263
TIM val samp     : 131
TIM current samp : 26505
TIM top          : 52747
Comm step        : 1
Temperature      : 48.34

Would like maximum braking, what would I need to adjust to keep this from happening?
```

---
## \#94 Posted by: FLATLINEcustoms Posted at: 2016-06-16T14:01:37.613Z Reads: 176

```
@elkick over at Vedder's forum a guy is suggesting turning down absolute max current. I am not home to check this out, but will after work. That may allow for stiff brakes and no cut outs... maybe.

@chaka do any of the settings in the fault code show you anything?
```

---
## \#95 Posted by: chaka Posted at: 2016-06-16T14:33:21.397Z Reads: 176

```
Honestly the drv chip is likely failing. I have done a number of upgrades to the components used in the construction of our VESC in the last few weeks/months and I no longer get these drop outs in braking. I also keep my max motor amps down to 30-50 amps depending on the motor at 12s. I go higher with lower voltages. I have never experienced these drop outs on smaller motors that have a max output within the specs of the VESC, I only have trouble with larger motors with a max output that exceeds the version 4.12 VESC specs.

If you would like to send your unit in for a retrofit let me know. Cover shipping and parts and we can call it good!
```

---
## \#96 Posted by: elkick Posted at: 2016-06-16T14:34:49.076Z Reads: 178

```
You are hitting 131A with a 12s setup. That's quite weird. I'd assume that if you lower that limit from 130 to 100A for example the VESC might even cut off earlier. Although it would be excellent if it works. 

But to be honest, I think there is something else which isn't working correctly (motor maybe).
```

---
## \#97 Posted by: FLATLINEcustoms Posted at: 2016-06-16T15:19:29.216Z Reads: 179

```
@Chaka I would love that. I'll email you. 

@elkick I am seeing it that way, if I am hitting 130 and lower it that means failure quicker. What would the motor be doing that isn't correct?
```

---
## \#98 Posted by: hexakopter Posted at: 2016-06-16T15:27:00.133Z Reads: 181

```
You should read this: http://vedder.se/forums/viewtopic.php?f=7&t=200
Had the same problem like you. Maybe it are the shunts for you also.
```

---
## \#99 Posted by: elkick Posted at: 2016-06-16T15:30:40.759Z Reads: 181

```
It's just significant that it's generating 131A while breaking. Maybe that's normal for that motor, but it's quite high. I have no idea if and what could go wrong, short term shorts or something? Only guessing, it's difficult to predict. Strange thing is, that it never occurred with my motors again, since I changed Amps for motor and battery.
```

---
## \#100 Posted by: FLATLINEcustoms Posted at: 2016-06-16T15:31:11.858Z Reads: 187

```
Interesting @hexakopter, I am sending mine back to @chaka to look at.
```

---
## \#101 Posted by: hexakopter Posted at: 2016-06-16T19:55:44.388Z Reads: 192

```
The 130A peak came from the "Absolute max" setting in bldc tool. When I changed it to 100A I got a fault with Current filtered around 100A and when changing to 80A a current filtered of around 80A. That wasn't the current really floating there, just a wrong reading because of the bad soldered shunt. So the STM32 was just thinking the high current was there because of the input reading.
```

---
## \#102 Posted by: Bender Posted at: 2016-07-13T03:02:26.808Z Reads: 180

```
I'm having this same problem in FOC
Did you ever get this figured out?
```

---
## \#104 Posted by: WARMAN Posted at: 2017-02-14T19:58:37.533Z Reads: 86

```
Same problem here too im using vesc 4.12 from diy.com with the gt2b cho mod brakes are pretty much non existent! Vesc just flashes pink
Really need a fix for this! Anyone found the issue
```

---
