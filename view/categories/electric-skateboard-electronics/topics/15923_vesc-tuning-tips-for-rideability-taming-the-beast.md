# Vesc tuning tips for rideability? Taming the beast

### Replies: 34 Views: 4192

## \#1 Posted by: lrdesigns Posted at: 2017-01-12T02:25:49.739Z Reads: 311

```
I have been having trouble getting a really smooth acceleration from my board, something that does not scare the poop out of me with acceleration but still has the power for a few steep hills at low speed which are part of my commute. Can I have booth? 

My setup is somewhat unusual. 
**-  Dual 5060 270kv motors.** Build quality not the best but they work. 
**- 12s Lipo, 8ah. 350wh.** From two 6s packs. Turnigy nano tech. Hobbyking does not even sell one this large any more, I got these from a friends para-motor project. 
**- 4:1 gearing.** 3D printed gears I designed myself. This ratio is for reducing motor load and giving me a theoretical top speed of 40kph. And yes I have ERPM limits too, that seems to work perfectly. 
**- 97mm wheels.**
**- GT2B controller** in mini buffalo case.
_*before the safety police come out, I have used lipo for years with RC models, I have a separate monitor for the voltage and have plently experience building systems that don't burn down._

At the moment the bottle neck in the system is the cheap motors when ambient is over 35c and rider skill. Batteries are always at ambient and vesc's get slightly warm.

My board far more power and acceleration than I can comfortably use, and the other issue is when I set the vesc for more power I have to use less throttle throw to control it. I heard the watt mode firmware is meant to fix this but I need to buy a programmer before I can install that due to no bootloader on my maytech vesc's. :disappointed_relieved: So its v2.18 current mode tuning for now. 

I did find a setting that has nice smooth acceleration but this came with two other issues. Above 50% speed there is some un-expected acceleration when under medium load, to ride around this I only use about 50% of the throttle throw and just accelerate to top speed a bit slower. 
**- This setting was motor 30amp and battery 20amp. X two vesc's**
- On Devin's constant claiming about setting the motor limit much higher than battery limit would fix the un-expected acceleration mid speed issue I thought why not I will give it a go. I didn't go extreme as his math due to me being cautious with my motors. So I tried these settings
**- Motor 50amp battery remains at 20amp.** 
I honestly didn't think it would make much difference but I noticed this, much better hill climb power, flat ground acceleration is now scary, just on the limit of what I find safe/unsafe. I could get used to it maybe but the worst part is now Im only using like 25% of the throttle throw. My tracking app shows I hit 40kph while the day before I only got to 33kph. I don't really need to go over 30kph, I dont have enough long straights to make my commute shorter with the extra speed. 

So Im thinking of trying the opposite, just to see what the affect is, put the motor limit back down to 30a and increase the battery to 40a. 

***One extra issue that is un-related to acceleration I just experienced. **Braking at full speed down hill.** I was going down a gentle hill at max speed then applying a modest amount of brake, the brake would come on for a couple of seconds then switch off, so I kept pulsing it until I was going slow enough to jump off and run. The battery was at 50% level so its not over charging, maybe my battery regen limit is too low? its set at **-25a**

I'm open to other suggestions. 

*Devin we have seen your math in several threads so we don't need it again here. :stuck_out_tongue_closed_eyes: While it did give me more low end power it did not help my other issues.
```

---
## \#2 Posted by: lrdesigns Posted at: 2017-01-12T02:26:43.309Z Reads: 282

```
<img src="/uploads/db1493/original/3X/6/8/685ea888ef490f097e1c359a86b32a23fc69f316.JPG" width="690" height="421">
```

---
## \#3 Posted by: NickTheDude Posted at: 2017-01-12T02:38:02.322Z Reads: 275

```
I'd recommend keeping the motor amps relatively high so you don't run into the sudden acceleration that occurs when your motor max supersedes the battery max, as well as lowering your battery amps.

Try 40ish motor amps and 10ish battery amps. If you don't have enough power slowly increase battery amps until it feels right, and if you run into the sudden acceleration raise the motor amps as well.

EDIT: Also I could be wrong about this but I heard somewhere that the min ERPM will cut out the motor when its reached. It would make sense that this is why your brakes are cutting out, however I don't know if lowering your min ERPM could potentially damage the VESC. Since you have such  high gearing it doesn't take much speed to reach your ERPM limit.
```

---
## \#4 Posted by: PXSS Posted at: 2017-01-12T02:42:36.306Z Reads: 258

```
Your braking issue could still be you hitting the amp limit on charge, I dont know why it would completely disable braking instead of just limiting it...
```

---
## \#5 Posted by: lrdesigns Posted at: 2017-01-12T03:07:50.551Z Reads: 254

```
Thanks, seems logical. I might give that a go with lower battery limit. 

Luckily I was going down a gentle hill and not a steep one, its the kind of issue I don't really want to spend time testing as its dangerous.
```

---
## \#6 Posted by: PXSS Posted at: 2017-01-12T03:27:11.171Z Reads: 244

```
I would not lower that limit! 25A is already a 3C charge. Any higher and you might damage your LiPos
```

---
## \#7 Posted by: saul Posted at: 2017-01-12T03:38:20.832Z Reads: 238

```
it might be too late. its a dual so 25A each! over 6C charge that is way too high even for nano tech.

I have mine set at -12A (single drive) for a 10ah pack that has 2C max charge..
```

---
## \#8 Posted by: devin Posted at: 2017-01-12T03:49:53.061Z Reads: 234

```
<p>This post was flagged by the community and is temporarily hidden.</p>
```

---
## \#9 Posted by: lrdesigns Posted at: 2017-01-12T04:26:10.723Z Reads: 226

```
Thanks for the concern, but I'm not too worried as this only happens for a very short amount of time, not enough to warm the batteries up. Heat is the main killer and also the danger. If I was coming down a very long and steep hill for like 30 mins it might be an issue. Luckily none of those hills on my commute :wink: They are also advertised as 5c charge. <img src="/uploads/db1493/original/3X/e/4/e4a4ac5440f49663b26b384854a201a91e5b957b.jpg" width="375" height="500">
```

---
## \#10 Posted by: NickTheDude Posted at: 2017-01-12T04:33:38.301Z Reads: 209

```
You definitely need to change your voltage cutoffs as well. I do cutoff start at 3.6V per cell and end at 3.4V per cell. So yours would be 3.6 * 12 = 43.2 and 3.4 * 12 = 40.8
```

---
## \#11 Posted by: lrdesigns Posted at: 2017-01-12T04:41:16.576Z Reads: 208

```
ohh yeah I didn't remember to times it by 2. I was running 6s at first to get used to the board. And I know my per cell limits are a bit too low but I have a separate system to monitor the individual cell voltage, I don't rely on the vesc for that.
```

---
## \#12 Posted by: lrdesigns Posted at: 2017-01-12T05:05:52.104Z Reads: 210

```
Ok going out to test 10amp max battery while leaving motor at 50. And adjusted my min battery voltage cut off. But as I said I dont rely on the vesc for this function. 
<img src="/uploads/db1493/original/3X/1/c/1c52d200e1ec10418c66214608bcd46cde27ce3f.JPG" width="690" height="380">
```

---
## \#14 Posted by: lrdesigns Posted at: 2017-01-12T05:52:21.874Z Reads: 199

```
OK, but please don't turn this thread into one of the others here with walls of your text and math equations. If you really need to do that PM them to me. Something short and concise here will be fine. Also this thread is for ride-ability of my over powered board I dont need or want more low end power except in a hill climb scenario. Results are 0.2386 ohms.
```

---
## \#15 Posted by: lrdesigns Posted at: 2017-01-12T05:58:17.525Z Reads: 194

```
Done a short test on my lunch break, it is more controllable than the 20 amp limit. I feels like more power than my first setting of 30 motor 20 battery. Somewhat between the two. There is still the acceleration surge at speed but its a little less abrupt. Needs some more ridding to really feel it out. 

This might be crazy but I was thinking a future vesc could have a tilt sensor so it could measure the slope angle when going up a hill then give you more power in a sort of hill climb mode, while still being low power on the flats. That would be cool!
```

---
## \#16 Posted by: devin Posted at: 2017-01-12T06:02:07.215Z Reads: 193

```
<p>This post was flagged by the community and is temporarily hidden.</p>
```

---
## \#40 Posted by: treenutter Posted at: 2017-01-12T22:23:27.805Z Reads: 163

```
[quote="lrdesigns, post:14, topic:15923"]
OK, but please don't turn this thread into one of the others here with walls of your text and math equations.
[/quote]

Heh!

@Irdesigns do you want me to split this thread so that you can follow your original thought? There seems to be a divergence of topics here. We can have the others continue in a new thread...
```

---
## \#42 Posted by: lrdesigns Posted at: 2017-01-13T01:26:46.674Z Reads: 156

```
Yes please. :grinning:  How did I know it would get out of hand? :stuck_out_tongue_closed_eyes: hahah. The subject is interesting but somewhat of a tangent to the original subject.
```

---
## \#43 Posted by: lrdesigns Posted at: 2017-01-13T01:31:09.240Z Reads: 156

```
[quote="Ackmaniac, post:18, topic:15923"]
But i also have no explanation for your dropout during braking. Could it be that you have a BMS in between and that the BMS maybe cuts off because of a too high voltage during braking.BTW you can also raise your motor min to -60 if you want more brake power.
[/quote]

No BMS, actually nothing between the battery and the vesc except some XT90 plugs. I have the battery monitor from the balance plugs. 

My theories are either the ERPM limit somehow disables braking OR could the motors be generating too high of a voltage, like over 57v which would trigger some protection?
```

---
## \#44 Posted by: devin Posted at: 2017-01-13T01:31:35.037Z Reads: 145

```
<p>This post was flagged by the community and is temporarily hidden.</p>
```

---
## \#45 Posted by: lrdesigns Posted at: 2017-01-13T01:44:16.468Z Reads: 143

```
[quote="saul, post:7, topic:15923, full:true"]
it might be too late. its a dual so 25A each! over 6C charge that is way too high even for nano tech.

I have mine set at -12A (single drive) for a 10ah pack that has 2C max charge..
[/quote]

I was thinking about this last night, and 1c means its fully charged from empty in 1 hour. 6c would mean its fully charged from flat in 10 minutes! That's a lot of energy to pump in a short amount of time. Im not sure that would even be possible with the hardware and a HUGE hill? Would like an electrical engineers thoughts on that.

I have charged some smaller nano tech's at 4C on a charger they got slightly over room temp. So long as the battery's are not heating up I don't see an issue with a few quick bursts of 6C charge and not over charging over 4.2v per cell.
```

---
## \#46 Posted by: lrdesigns Posted at: 2017-01-13T01:47:24.261Z Reads: 134

```
[quote="devin, post:44, topic:15923, full:true"]
@lrdesigns did u try 5/33/33? anything to report?
[/quote] Probably be a week till I can do any more experiments with the settings, raining today. Weather not looking great. :sob:  But why reduce the absolute to 33amps, what affect will that have?
```

---
## \#47 Posted by: devin Posted at: 2017-01-13T01:54:41.326Z Reads: 128

```
<p>This post was flagged by the community and is temporarily hidden.</p>
```

---
## \#48 Posted by: PXSS Posted at: 2017-01-13T02:02:13.925Z Reads: 132

```
You're still damaging them. It's not the heat that kills them, it's the chemical reaction inside them.
```

---
## \#13 Posted by: treenutter Posted at: 2017-01-13T13:59:14.680Z Reads: 132

```
25 posts were split to a new topic: [Linear Acceleration and VECS Parameter Calculations](/t/linear-acceleration-and-vecs-parameter-calculations/16030)
```

---
## \#49 Posted by: lrdesigns Posted at: 2017-01-19T06:18:51.231Z Reads: 123

```
An update. I have been riding around for a few days with 
**50A motor**
**10A battery**   x2vesc. 
At first it seemed slightly too fast but I have got used to the power and I'm happy with the performance. I can only use like 20% of the throttle throw but you can get used to it. Waiting until I can try watt mode. Top speed at this setting is 33kph.

So tried another setting for science
**60A motor**
**5A battery**
Just enough power to get up my hill but acceleration was extremely limited. Once your moving past walking speed you can hold the throttle in any position and get a slow steady acceleration. Might be a good beginner mode but otherwise boring. 

Next experiment
**40A motor**
**15A battery**
Damn it is fast! Some mid speed acceleration surging. I think I will ride this for a few days to see how I like it but I think half way 12.5A might be my preferred level. I think top speed will go up at this power level

Another thing I have been adjusting is the Regen amps. I have left the motor at -30 but have been adjusting the battery down from -25
**Regen motor -30A**
**Regen battery -25A, -20A, -15A -10A, -8A.**  Really didnt notice much if any change untill below -10A. Still enough to slow me down the slow speed hill near my office.
```

---
## \#50 Posted by: lrdesigns Posted at: 2017-01-19T07:27:54.864Z Reads: 122

```
[quote="PXSS, post:48, topic:15923, full:true"]
You're still damaging them. It's not the heat that kills them, it's the chemical reaction inside them.
[/quote]

The batteries are rated for 5c charge, 6c is not going to kill them.

I would agree you could shorten their cycle life if you always charged them at 6c on a charger, but you would need a 2500watt charger though! 

After looking at this lithium battery research it seems the worst thing you can do to them is to fully discharge them or charge them above 4.1v. (http://batteryuniversity.com/learn/article/how_to_prolong_lithium_based_batteries)  Charging them to 4.1 instead of 4.2 can double cycle life, only discharging them 50% can triple cycle life. 

My batteries are quite oversized for my needs, I typically only take 40% out of the pack before recharging so my cycle life should be pretty good!

Furthermore I just dont think its even possible to achieve a 6c charge rate with the vesc, my motors and the hills I have available. I noticed little if any difference in braking power with regen battery setting of -25A, -20A, -15A and -10A. Motor regen was at -30 for all these tests. Suggesting the actual output is much lower than -25A for any appreciable amount of time. If you could produce 25amp per vesc for 10 ten minutes and the batteries where flat when you started you could achieve a 6c rate and you did that every morning on your commute it would for sure be bad for the cycle life. But a few seconds at 50 amps for batteries this large should be a non issue. 

I dont want to start a flame war and I would like to get back on topic. For the record I am more concerned my brakes have good performance than battery cycle life.
```

---
## \#51 Posted by: lrdesigns Posted at: 2017-03-29T06:16:42.400Z Reads: 107

```
I just want to give an update. I did finally get to a point where it was controllable, settings below. With erpm limited to 65k I got max speed of 35kph. 

But then I wore out all my 12 tooth drive pulleys and only had 15 tooth on hand. Changing the gear ratio from 4:1 to 3.2:1  this made a HUGE difference to the power delivery, now it is ultra smooth and easy to control. But it did sacrifice some hill climb power and less braking power. I really want the breaking power back as now the top speed is 43kph. The gear ratio made much more difference than tuning of the vesc settings so thats something for people to think about. 

12s lipo and 4:1 gearing leads to brutal acceleration. It also shredded a lot of belts. The long term plan is to use 140kv motors and 2:1 ratio for much better belt and drive pulley life, as the motor pulley will be 20 tooth. Also the wheel pulley is way too close to the ground even with 97mm wheels, so the belts get hit by rocks and things which can damage them. 

<img src="/uploads/db1493/original/3X/7/a/7a2c808624b4c4491fc98b5fc6c64a109ef63cef.JPG" width="690" height="330"><img src="/uploads/db1493/original/3X/0/6/06848cf36a1fb8294228e11fd19ef4a79a4e23aa.JPG" width="690" height="330">
```

---
## \#52 Posted by: ninja Posted at: 2017-03-29T06:19:23.663Z Reads: 93

```
Your lipo on the left seems a bit puffy, don't blow up yourself...:scream:

Maybe it's just a picture, optical illusion, hope so...:cold_sweat:
```

---
## \#53 Posted by: lrdesigns Posted at: 2017-03-29T06:34:35.563Z Reads: 99

```
[quote="ninja, post:52, topic:15923"]
Your lipo on the left seems a bit puffy
[/quote]

They are not puffed its just the picture. I have puffed quite a lot of lipos in RC cars, planes and quads. It only seems to happen when you pull too much current from them, at or over the C rating. Which I can not do from these as I would need to draw 200 amps to get to the C rating. At 45 volts that is like 9000 watts! The Vesc settings limit power to 1200 watts. 

Even though I mention it at the start that I didnt want the lipo safety police on this thread, but it seems they are always out in force. :smirk:

Here is something that will make their skin crawl, a slightly puffed battery is not dangerous after it has cooled down. And is not an indication that is going to blow up in the future. It "could" continue to be used in a lower draw application. Though I wouldn't use it in anything I didn't mind loosing. 

These batteries are way bigger and higher C than I need for the application so they are very under stressed.
```

---
## \#54 Posted by: ninja Posted at: 2017-03-29T06:43:34.144Z Reads: 95

```
O.K. that is good then..:wink:
```

---
## \#55 Posted by: Ackmaniac Posted at: 2017-03-29T06:45:22.436Z Reads: 94

```
You should give my firmware mod a try to team the beast. Watt control and adjustable throttle curves are developed to make it more controllable.
```

---
## \#56 Posted by: lrdesigns Posted at: 2017-03-29T06:48:50.581Z Reads: 99

```
[quote="Ackmaniac, post:55, topic:15923"]
You should give my firmware mod a try
[/quote]

I want to a lot but maytec vesc with no bootloader. :cry: and I didnt order a programmer yet.
```

---
## \#57 Posted by: lrdesigns Posted at: 2017-07-05T02:47:01.741Z Reads: 79

```
[quote="Ackmaniac, post:55, topic:15923"]
You should give my firmware mod a try to team the beast.
[/quote]

I finally got a programmer and installed your firmware. Its awesome sauce!!  I did eventually tame the beast though before I installed the firmware. I changed the gearing from 4:1 12-48 gears  to 3.2:1 15-48 gears. This made a huge difference and really smoothed out the acceleration. And the 15 tooth motor pulleys last like 4 times longer than the 12s. The only downside was less braking power. 

I recently converted the board from 270kv motors to 140kv motors with 2:1 gearing so I guess the thread is closed then. They also have sensors and are much smoother, more torquey feeling and good brake performance. 

<img src="/uploads/db1493/original/3X/5/6/565354fef10edbc407380d525184afe7c3d0522c.jpeg" width="666" height="500"><img src="/uploads/db1493/original/3X/4/b/4bb41474a17dfc378ba13ecaf2dc57ee7c3634b5.jpg" width="666" height="500">
```

---
## \#58 Posted by: lrdesigns Posted at: 2018-06-29T09:17:34.502Z Reads: 38

```
In case anyone is wondering, with a years more experience I can say for sure, gear ratio makes a HUGE difference to feeling and performance. 

Just a few teeth difference on the motor will make a big difference. Also never use lower than 15 tooth on the motor or your pulleys will wear out too quickly and start to shred belts. 

Larger motor pulleys are really good for belt life, but will result in less torque for both acceleration and braking, so you can way up your options. 

Since going to a lower kv motor and 20t motor pulley, and then now 18t motor pulley I have not broken a single belt in a year.
```

---
