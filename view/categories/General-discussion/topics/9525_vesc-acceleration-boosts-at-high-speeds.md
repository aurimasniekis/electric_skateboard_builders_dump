# VESC acceleration boosts at high speeds

### Replies: 115 Views: 6092

## \#1 Posted by: Ackmaniac Posted at: 2016-09-13T15:25:14.661Z Reads: 459

```
Hi. I always have a acceleration boost at high speeds when i go full throttle. And many people experience the same problem as i read in other threads. And i think that this is a software bug of the VESC.

My question is if people with other ECS's experience the same issue or if it is only a known problem for the VESC.
```

---
## \#2 Posted by: PB1 Posted at: 2016-09-13T15:35:17.602Z Reads: 443

```
I also experience this at around 25kmh. When the board reaches this speed it really wants to accelerate,  even when I am very light on the throttle. 
Using VESC.
```

---
## \#3 Posted by: Ackmaniac Posted at: 2016-09-13T15:56:43.510Z Reads: 432

```
Does it also happen in FOC mode? Can't use FOC at the moment so i can't test.
```

---
## \#4 Posted by: JohnnyMeduse Posted at: 2016-09-13T16:03:01.945Z Reads: 432

```
It is not consider as a problem for some of us... 

[quote="longhairedboy, post:40, topic:8292"]
usually the sudden bursts of acceleration while already moving are attributed to the motor hitting the "sweet spot." Somepeople call it the secret turbo. That's when the VTEC kicks in as they would have said years ago before literally everyone had variable valve timing.
[/quote]
```

---
## \#5 Posted by: Ackmaniac Posted at: 2016-09-13T16:05:13.970Z Reads: 423

```
I made data loggings and i think the problem is that the duty cycle is not calculated correctly. Because it jumps from 0.86 to 0.95. Before that it climes linear.
```

---
## \#6 Posted by: Hummie Posted at: 2016-09-13T16:17:15.015Z Reads: 412

```
could be your vesc settings and a long topic on it is here.  when you're going slowly the motor amp limit rules and when you get speed up the battery amp limit supersedes
```

---
## \#7 Posted by: Ackmaniac Posted at: 2016-09-13T16:20:27.949Z Reads: 406

```
I know all of that. Only the jump from 0,86 to 0.95 doesn't make sence. Watch the video when it goes up to 0,86 duty cycle. The video is with constantly 50% throttle.

[Data logging](http://sendvid.com/tgpwi02g)
```

---
## \#8 Posted by: makevoid Posted at: 2016-09-13T16:24:09.966Z Reads: 393

```
It happens infrequently to me and I haven't been able to log it via a logging app yet to see what happens. It would be cool to log also the throttle position (ppm value %), something that the current apps seem not to do, is that value something easily pullable from the vesc via uart or does it requires a vesc "custom app" setting + implementation (instead of uart+ppm control mode)?

From what I remember it happened to me around 30k erpm and only when pushing the throttle quite hard (80+% ppm), if I push it slowly (~60%) which is what I usually do at medium/high speeds, it never happens.
```

---
## \#9 Posted by: longhairedboy Posted at: 2016-09-13T16:27:27.018Z Reads: 379

```
its not a problem for me either. I've just come to expect it. It may be a bit of a curiosity though for someone who's never ridden a VESC equipped board before.
```

---
## \#10 Posted by: Ackmaniac Posted at: 2016-09-13T16:30:43.057Z Reads: 364

```
If it is a software bug then it would be nice to fix it and get rid of the problem. I am also working on another control mode which gives you 100% throttle control even at high speeds. Because depending on your VESC settings you loose the control at higher speeds. 
That is the behavior when it doesn't make a difference if you pull the trigger 50% or 100% at higher speeds. Power stays the same. 
But first i want to know if i can fix that issue with the acceleration boost.

@longhairedboy PS. I am a big fan of your builds
```

---
## \#11 Posted by: longhairedboy Posted at: 2016-09-13T16:37:50.195Z Reads: 345

```
i have found that making adjustments to the motor max actually extend the range of acceleration over full throttle so that its easier to maintain a articular level of speed, even lower speeds. The problem is that rider weight greatly affects this kind of thing so settings for a guy like me might be ideal for me but sluggish for a 200 pound guy. Vesc tuning is a very personal thing. I sort of wish i had an app that took rider weight and a selection of graphical acceleration curve depictions and just put the right settings in automatically.
```

---
## \#12 Posted by: NNGG Posted at: 2016-09-13T20:14:25.356Z Reads: 326

```
Isnt @jacobbloy doing that app stuff?
```

---
## \#13 Posted by: whitepony Posted at: 2016-09-13T20:26:44.557Z Reads: 320

```
got the exact same thing, it also feels as if i jerk the throttle. would be great if thats actually a bug with the duty cycle jump. clearly something for the vedder forums!
```

---
## \#14 Posted by: Photorph Posted at: 2016-09-13T20:33:56.383Z Reads: 310

```
Yep, that happens.  It's like turbo boost lol.  Scared me the first time it happened, but after that it's kind of fun actually.  My board that LHB built topped out around mid 30s, so I'd say somehwere in the 27-30 mph it hit like a sudden boost to get to that max speed.
```

---
## \#15 Posted by: chinzw Posted at: 2016-09-13T20:47:06.948Z Reads: 309

```
Does this also happen with Duty Cycle instead of Current Control ?
```

---
## \#16 Posted by: Namasaki Posted at: 2016-09-13T20:53:19.180Z Reads: 303

```
I haven't noticed this issue with dual Vescs, 
Motor max at 60a
Batt max at 30a
Maybe setting batt lower than motor prevents the turbo switch.?
```

---
## \#17 Posted by: PB1 Posted at: 2016-09-13T21:20:11.493Z Reads: 304

```
Does it happen in FOC mode? 

I don't think so, not on my board.  I'm running one board in FOC mode and acceleration is very smooth.  

You mention a potential bug in bldc mode between 85 and 95%. Could be.  
The acceleration boost on my bldc board is at around 20 to 25kmh,  so closer to 50% of top speed.
```

---
## \#18 Posted by: kampfhahn Posted at: 2016-09-13T21:26:07.642Z Reads: 295

```
@whitepony is using FOC for a few weeks now and has also experienced these bursts.
```

---
## \#19 Posted by: Ackmaniac Posted at: 2016-09-13T22:23:14.635Z Reads: 283

```
Can somebody please verify if FOC mode also has that behavior? If that is the case, is it stronger, less strong or the same?
```

---
## \#20 Posted by: Randyc1 Posted at: 2016-09-13T22:29:22.972Z Reads: 280

```
Chaka talked about this recently,

 He thinks and I agree it is probably from Voltage Sag. When accelerating hard a Big Voltage Sag is created initially,... then when voltage comes back to normal Sag,  this boost is felt!
```

---
## \#21 Posted by: Ackmaniac Posted at: 2016-09-13T22:48:53.372Z Reads: 257

```
i don't think thats true. In the Video that i posted above you see that the Voltage sags in about 0,5 volts when the burst happens. So it is the opposit.
```

---
## \#22 Posted by: solarcross Posted at: 2016-09-13T23:15:13.807Z Reads: 257

```
Yep noticed the boost too, Im using 3 wire throttle, sensorless, BLDC, and 245KV Tacon Bigfoot on ADC-UART app. only..

thought it was a result of voltage sag, timing setting or ramp setting..

Does this mean VESC is NOT giving me maximum output power at lower RPM`s ??
```

---
## \#23 Posted by: Ackmaniac Posted at: 2016-09-13T23:28:27.779Z Reads: 260

```
At lower RPM's is no issue. Only the peak at around 0,85 till 0,95 duty cycle seems to have issues. I still try to find out. But it would help if somebody can tell me if he has the same issues with FOC.
Maybe somebody is switching between FOC and BLDC and can tell me if the behavior is the same. At the moment i can't test it myself.
```

---
## \#24 Posted by: Jinra Posted at: 2016-09-13T23:43:29.598Z Reads: 256

```
FWIW I've never experienced this on my dual VESC dual 5065 motors on BLDC
```

---
## \#25 Posted by: devin Posted at: 2016-09-14T04:48:48.342Z Reads: 254

```
<p>This post was flagged by the community and is temporarily hidden.</p>
```

---
## \#26 Posted by: Jinra Posted at: 2016-09-14T04:55:31.254Z Reads: 248

```
[quote="devin, post:25, topic:9525"]
depending on the wattage you desire close to 0rpm, there is only one ratio for batt max and motor max that results in even acceleration.
[/quote]

This simply isn't true, I've never had this issue and have used various motor max/battery max ratios.
```

---
## \#27 Posted by: devin Posted at: 2016-09-14T04:58:01.498Z Reads: 243

```
<p>This post was flagged by the community and is temporarily hidden.</p>
```

---
## \#28 Posted by: Jinra Posted at: 2016-09-14T05:01:11.761Z Reads: 243

```
no I'm saying there is not just 1 ratio that will prevent the random acceleration issue
```

---
## \#29 Posted by: devin Posted at: 2016-09-14T05:03:15.685Z Reads: 254

```
<p>This post was flagged by the community and is temporarily hidden.</p>
```

---
## \#30 Posted by: Ackmaniac Posted at: 2016-09-14T05:12:49.115Z Reads: 250

```
This thread should be about the acceleration boost at high speeds. The settings of the motor max and battery is discussed in another thread already.
```

---
## \#31 Posted by: devin Posted at: 2016-09-14T05:14:58.484Z Reads: 239

```
<p>This post was flagged by the community and is temporarily hidden.</p>
```

---
## \#32 Posted by: chinzw Posted at: 2016-09-14T05:31:14.914Z Reads: 232

```
@devin i think you should open a thread in vedder's forums
```

---
## \#33 Posted by: Ackmaniac Posted at: 2016-09-14T06:29:17.738Z Reads: 223

```
I also can't aggree on that. When you watch the video you can see that the motor amps power already down from 38 to 32 and after that the boost happens when duty jumps from 0.87 to 0.95.

But we should give it a try. That means by your explanation that the boost should not happen when max battery and max motor amps are the same.
```

---
## \#34 Posted by: devin Posted at: 2016-09-14T07:19:46.899Z Reads: 213

```
<p>This post was flagged by the community and is temporarily hidden.</p>
```

---
## \#35 Posted by: Ackmaniac Posted at: 2016-09-14T07:24:27.567Z Reads: 210

```
But in reality that is the moment when it starts. In the video you see that it stays for like 2 seconds between 0,84 and 0,87 duty cycle. And then it jumps directly to 0,95. And that is when the boost kicks in.

BTW throttle is all the time at 50%.
```

---
## \#36 Posted by: devin Posted at: 2016-09-14T07:26:19.823Z Reads: 205

```
<p>This post was flagged by the community and is temporarily hidden.</p>
```

---
## \#37 Posted by: Ackmaniac Posted at: 2016-09-14T07:31:06.301Z Reads: 210

```
But why does it jump to 0,95. All the time the duty cycle increases  very linear. Then it idles at around 0,85 and then jumps to 0,95.
```

---
## \#38 Posted by: devin Posted at: 2016-09-14T07:33:46.018Z Reads: 210

```
<p>This post was flagged by the community and is temporarily hidden.</p>
```

---
## \#39 Posted by: Ackmaniac Posted at: 2016-09-14T07:40:14.824Z Reads: 208

```
But in my posted video this happens already earlier. As you see in the video the motor current decreases already 2 seconds befor the boost from 39 to 32 amps.
```

---
## \#40 Posted by: devin Posted at: 2016-09-14T07:41:23.582Z Reads: 202

```
<p>This post was flagged by the community and is temporarily hidden.</p>
```

---
## \#41 Posted by: SimosMCmuffin Posted at: 2016-09-14T07:43:00.706Z Reads: 199

```
Was your motor amp limit 40 Amps? Because then the algorithm might not allow you to increase the duty cycle at 39 Amps. Although it doesn't explain it why it then allowed the higher duty cycle when the motor amps had decreased to 32 A... Might be a problem with the PID-control loop.
```

---
## \#42 Posted by: Ackmaniac Posted at: 2016-09-14T07:43:03.439Z Reads: 196

```
[Data logging](http://sendvid.com/tgpwi02g)
```

---
## \#43 Posted by: Ackmaniac Posted at: 2016-09-14T07:43:32.261Z Reads: 196

```
Motor amp was at 80 and batterie at 35 and throttle at perfectly constant 50%.
```

---
## \#44 Posted by: SimosMCmuffin Posted at: 2016-09-14T07:46:17.654Z Reads: 193

```
So I'm guessing with the VESC that 80 motor amp limit and 50 % throttle would mean that the PID-loop would try to maintain 40 motor amps.
```

---
## \#45 Posted by: devin Posted at: 2016-09-14T07:47:27.782Z Reads: 192

```
<p>This post was flagged by the community and is temporarily hidden.</p>
```

---
## \#46 Posted by: Ackmaniac Posted at: 2016-09-14T07:51:04.615Z Reads: 193

```
I think the problem is in the BLDC code in the methode update_adc_sample_pos at this line
`if (duty > (uint32_t)((float)top * conf->l_max_duty)) {

         duty = (uint32_t)((float)top * conf->l_max_duty);
   }`

But i am still not sure. Did some calculations and sometimes you get strange numbers exactly around the duty cycle between 0,85 and 0,95. But still hard to understand.

And i just want to know if the same behavior happens in FOC mode. Because there the calculation is not the same.
```

---
## \#47 Posted by: devin Posted at: 2016-09-14T07:52:58.564Z Reads: 186

```
<p>This post was flagged by the community and is temporarily hidden.</p>
```

---
## \#48 Posted by: Ackmaniac Posted at: 2016-09-14T07:57:14.499Z Reads: 188

```
Isn't there anybody in the forum who can tell me if the acceleration burst happens in FOC mode?
```

---
## \#49 Posted by: devin Posted at: 2016-09-14T07:58:10.947Z Reads: 192

```
<p>This post was flagged by the community and is temporarily hidden.</p>
```

---
## \#50 Posted by: SimosMCmuffin Posted at: 2016-09-14T08:15:43.730Z Reads: 200

```
Off-topic reply, but.

Discussed the motor theory with my electronics lab teacher on monday and he confirmed it to be correct. So I can pretty much do almost purely mathematical control. I need to know the motor's kV, Pole count and internal resistance (all constants) + I need to be able to measure the battery DC voltage (Although I can use a constant, but voltage droop exists) + Motor's RPM, which I can measure with the hall-sensors. Basically, because I IMO suck at ADC design, I want to avoid using it as much as possible.

Then I can calculate motor amps, battery amps, power, speed and from those make my control scheme. We also discussed what would be the most natural control scheme and we concluded that speed control is the best option. So I'll probably use speed control and then just calculate the motor amps and battery amps to make sure they stay within limits.

Also did some calculations to figure out battery voltage, wheel size, gearing and motor kV to beat the current world record (95.9 km/h) for electric skateboards :grin:
```

---
## \#51 Posted by: devin Posted at: 2016-09-14T08:26:01.932Z Reads: 200

```
<p>This post was flagged by the community and is temporarily hidden.</p>
```

---
## \#52 Posted by: elkick Posted at: 2016-09-14T08:27:49.389Z Reads: 195

```
None of my 7 bards with FOC shows this problem. All of them are on the debugged FW 2.18:

- 2x FOC sensored/hybrid mode at 10s (dual 6355/200kV)
- 1x FOC sensored/hybrid mode at 12s (dual 6374/190kV eMTB)
- 2x  FOC/nonsensored at 10s (dual, hummies hub motors/90kV)
- 2x FOC/nonsensored at 7s (single, kids mode, limited ERPM, 1x 6355/240kV, 1x 5065/260kV)

But I might not be a reference for that, maybe the setups of others are different.
```

---
## \#53 Posted by: PB1 Posted at: 2016-09-14T08:39:21.407Z Reads: 198

```
@ackmaniac, very interesting video and data. I watched the video many times. 

To me it actually looks that neither motor nor battery LIMITS play any role here. Neither motor nor battery current are hitting the limit. With your throttle setting at 50% the motor is simply not requested to produce enough power to get close to the limits of 80 amps motor and 35 amps battery. 

What is noticeable is that battery voltage drops and is at the lowest level at exactly the point the duty cycle jumps from 0,86 to 0,94. This also seems to indicate an irregularity. 

As mentioned, I haven't noticed the boost in FOC mode. It is very pronounced on another board in BLDC mode, but at lower speeds. 
So why would it be between 0,85 and 0,95???
Could it be at other levels with other settings?
```

---
## \#54 Posted by: devin Posted at: 2016-09-14T08:43:11.211Z Reads: 186

```
<p>This post was flagged by the community and is temporarily hidden.</p>
```

---
## \#55 Posted by: SimosMCmuffin Posted at: 2016-09-14T08:44:58.424Z Reads: 172

```
That chart is only applicable when we are not changing the duty cycle! We can only reproduce that chart if we either give the motor a constant voltage, or static duty cycle. It is a **STATIC** representation.

When we are cruising, we ARE adjusting the duty cycle and therefore it's a **DYNAMIC** situation in which you cannot use that chart directly.
```

---
## \#56 Posted by: devin Posted at: 2016-09-14T08:46:20.312Z Reads: 172

```
<p>This post was flagged by the community and is temporarily hidden.</p>
```

---
## \#57 Posted by: SimosMCmuffin Posted at: 2016-09-14T08:47:54.698Z Reads: 174

```
Sorry. I meant the PMDC performance GRAPH. Sorry.

[quote="SimosMCmuffin, post:55, topic:9525, full:true"]
That _GRAPH_ is only applicable when we are not changing the duty cycle! We can only reproduce that graph if we either give the motor a constant voltage, or static duty cycle. It is a STATIC representation.

When we are cruising, we ARE adjusting the duty cycle and therefore it's a DYNAMIC situation in which you cannot use that graph directly.
[/quote]
```

---
## \#58 Posted by: devin Posted at: 2016-09-14T08:48:54.331Z Reads: 173

```
<p>This post was flagged by the community and is temporarily hidden.</p>
```

---
## \#59 Posted by: SimosMCmuffin Posted at: 2016-09-14T08:50:00.234Z Reads: 166

```
Yes, due to the VESC screwing around with the duty cycle, to stay within the motor amp and battery amp settings.
```

---
## \#60 Posted by: devin Posted at: 2016-09-14T08:51:56.136Z Reads: 160

```
<p>This post was flagged by the community and is temporarily hidden.</p>
```

---
## \#61 Posted by: Ackmaniac Posted at: 2016-09-14T08:57:11.090Z Reads: 152

```
This thread is not about the behavior at 0 rpm. We know that we need to increase the motor max amps drastically to reach high watts at 0.so please stay to the topic about the acceleration boost. 

So it seems that the problem doesn't exist in Foc mode. That brings me back to my theory that this behavior is caused by wrong calculations.  Maybe somebody can test with the same bat and motor settings on bldc and foc and tell us the difference.
```

---
## \#62 Posted by: PB1 Posted at: 2016-09-14T08:57:34.173Z Reads: 155

```
@devin, please note that this diagram is a generic diagram and not a real world motor diagram. Also, it doesn't state any load, which in the real world is constantly changing. 

In the real world when the motor powers a skateboard we have wind resistance which increases with the square of the speed. So we need 1) power to accelerate  (pretty constant in this case) plus 2) power to overcome increasing wind resistance.
```

---
## \#63 Posted by: SimosMCmuffin Posted at: 2016-09-14T08:57:40.914Z Reads: 155

```
Okay. Let's consider the control scheme for a moment.

Which one is best for natural acceleration?
Speed
Torque
Power

Before we agree on which one the controller should use, we can't really discuss the way to go about achieving that.
```

---
## \#64 Posted by: devin Posted at: 2016-09-14T09:00:27.978Z Reads: 153

```
<p>This post was flagged by the community and is temporarily hidden.</p>
```

---
## \#65 Posted by: devin Posted at: 2016-09-14T09:04:19.578Z Reads: 151

```
<p>This post was flagged by the community and is temporarily hidden.</p>
```

---
## \#66 Posted by: elkick Posted at: 2016-09-14T09:08:16.105Z Reads: 148

```
I don't have to prove anything and I am using VESCs since their existence in May 2015. Believe me, I did logging extensively. I am out of this now.
 @devin, and please get a VESC yourself and do those tests. You comments are increasingly annoying.
```

---
## \#67 Posted by: Ackmaniac Posted at: 2016-09-14T09:08:50.057Z Reads: 140

```
That is right.  But you can clearly feel the boost in bldc and if you can't feel it in Foc then that would be enough for me.
```

---
## \#68 Posted by: devin Posted at: 2016-09-14T09:08:53.791Z Reads: 139

```
<p>This post was flagged by the community and is temporarily hidden.</p>
```

---
## \#69 Posted by: elkick Posted at: 2016-09-14T09:11:53.191Z Reads: 138

```
I had these boosts in BLDC mode (control: current no rev w brakes) only, if the max motor current and the max battery current were too far away from each other, especially when motor max was set too high.
```

---
## \#70 Posted by: PB1 Posted at: 2016-09-14T09:13:29.136Z Reads: 138

```
[quote="devin, post:64, topic:9525"]
with no load you'll reach constant 100% rpm on the graph.
[/quote]

Agreed. But in this case with the data shown in the video we are talking about a changing load and a changing duty cycle. So the graph is not fully applicable. 

But let's not high jack this thread.
```

---
## \#71 Posted by: devin Posted at: 2016-09-14T09:15:26.355Z Reads: 133

```
<p>This post was flagged by the community and is temporarily hidden.</p>
```

---
## \#72 Posted by: PB1 Posted at: 2016-09-14T09:17:50.726Z Reads: 138

```
Can you give examples of motor max and battery max when you had the boost? 

Because in the video above, neither motor max nor battery max seem to be limiting. The actual currents are far below any limits. 
Does the VESC have any hard coded default limits that are superseding the settings?
```

---
## \#73 Posted by: devin Posted at: 2016-09-14T09:20:52.019Z Reads: 136

```
<p>This post was flagged by the community and is temporarily hidden.</p>
```

---
## \#74 Posted by: elkick Posted at: 2016-09-14T09:21:51.964Z Reads: 144

```
It was something around 60A motor, 20A battery side. But I think there are more variables to be taken into account since there are many factors influencing. Remote/receiver/control mode/app config etc. 

Are Median Filters enabled? Is that behavior different having them on/off?
```

---
## \#75 Posted by: devin Posted at: 2016-09-14T09:23:20.204Z Reads: 142

```
<p>This post was flagged by the community and is temporarily hidden.</p>
```

---
## \#76 Posted by: devin Posted at: 2016-09-14T09:30:01.549Z Reads: 142

```
<p>This post was flagged by the community and is temporarily hidden.</p>
```

---
## \#77 Posted by: PB1 Posted at: 2016-09-14T09:32:33.524Z Reads: 139

```
yes @devin

However I also have this acceleration boost when coasting (maybe 10% throttle) at 25kmh and then applying throttle very lightly (maybe 20% or 30%). In this case I'm far away from any amp limits and your theory does not apply for this case.

So devin please: do not high jack this threat with your theory. It might be true or not. But @Ackmaniac is after something else here and doing a great job!

**I will refrain from posting any further here. @Devin, please do the same so others can speak up as well!**
```

---
## \#78 Posted by: devin Posted at: 2016-09-14T09:33:41.603Z Reads: 143

```
<p>This post was flagged by the community and is temporarily hidden.</p>
```

---
## \#79 Posted by: devin Posted at: 2016-09-14T09:35:47.512Z Reads: 144

```
<p>This post was flagged by the community and is temporarily hidden.</p>
```

---
## \#80 Posted by: elkick Posted at: 2016-09-14T09:43:29.605Z Reads: 141

```
This whole topic was already discussed with Benjamin Vedder a year ago on ES. This was his statement before he adjusted some specs on SW, FW and also on HW 4.10-12. Nevertheless, under some circumstances it might be still there.


> The power burst that you are feeling is caused by the current measurement problem that I have tried to solve recently. What happens is that at a certain duty cycle (around 80%) one of the shunts will get noise coupled which causes an offset so that too hich current is measured for one commutation cycle and the current backoff kicks in. After this noise disappears the backoff will go back and you feel the kick that you described. With the recent firmwares I have been working on the sample synchronization and some other things to make it better in software, but a hardware solution would be better (by the way, this would not be a problem using three shunts, but using two is more tricky).
```

---
## \#81 Posted by: Ackmaniac Posted at: 2016-09-14T10:16:11.598Z Reads: 124

```
Thanks, this was very helpful. Didn't know that Benjamin made a commitment to this.
I need to analyse this further. Because i don't get rid of the feeling that the code i posted above is causing that.

BTW my settings were motor max 80 and battery max 35 in the video. 
And it still would be helpful if somebody can do the test with the same settings in FOC and BLDC.
```

---
## \#82 Posted by: devin Posted at: 2016-09-14T15:21:18.061Z Reads: 133

```
<p>This post was flagged by the community and is temporarily hidden.</p>
```

---
## \#83 Posted by: Ackmaniac Posted at: 2016-09-14T18:27:36.265Z Reads: 137

```
I made another Video with 100% throttle. (At around 20 km/h i could pull the throttle fully)
Behavior is the same.
Motor max 80 A
Battery max 35 A

https://youtu.be/UOrw2QBK-6A

After that run i made more test runs with different settings and it always happens. One more thing i have to test is with really high Battery Amps but i don't think that this will make a difference.

Also it seems that less Voltage on the Battery softens the boost.
```

---
## \#84 Posted by: devin Posted at: 2016-09-14T20:33:47.733Z Reads: 139

```
<p>This post was flagged by the community and is temporarily hidden.</p>
```

---
## \#85 Posted by: Ackmaniac Posted at: 2016-09-14T21:05:03.493Z Reads: 133

```
Which doesn't help us to get rid of that problem or find the root cause.
```

---
## \#86 Posted by: devin Posted at: 2016-09-14T21:18:40.965Z Reads: 133

```
<p>This post was flagged by the community and is temporarily hidden.</p>
```

---
## \#87 Posted by: chinzw Posted at: 2016-09-14T21:22:54.320Z Reads: 128

```
He could be going flat, downhill, without wind, backwind or whatever other variable you want to add.
```

---
## \#88 Posted by: devin Posted at: 2016-09-14T21:26:03.996Z Reads: 130

```
<p>This post was flagged by the community and is temporarily hidden.</p>
```

---
## \#89 Posted by: chinzw Posted at: 2016-09-14T21:37:56.463Z Reads: 134

```
Not really. A loaded motor vs an unloaded motor will not show the same wattage at the same rpms.
```

---
## \#90 Posted by: Ackmaniac Posted at: 2016-09-14T21:41:40.822Z Reads: 133

```
The explanation for the watt difference is simply the throttle difference. Half throttle vs full throttle.
```

---
## \#91 Posted by: devin Posted at: 2016-09-14T22:08:18.703Z Reads: 134

```
<p>This post was flagged by the community and is temporarily hidden.</p>
```

---
## \#92 Posted by: devin Posted at: 2016-09-14T22:14:35.938Z Reads: 136

```
<p>This post was flagged by the community and is temporarily hidden.</p>
```

---
## \#93 Posted by: Ackmaniac Posted at: 2016-09-15T15:21:42.390Z Reads: 137

```
I posted my analysis in the Vedder forum and hope that he will have a look at it. But i also need to try it myself with a modified firmware.
If anybody is interested in the code analysis you can find it here:
[Vedder Forum Thread](http://vedder.se/forums/viewtopic.php?f=6&t=375)
```

---
## \#94 Posted by: peter Posted at: 2016-09-16T20:04:08.937Z Reads: 138

```
arvidb at the vedder forum has a plausible explanation

http://vedder.se/forums/viewtopic.php?f=6&t=375&start=10

The dutcy cycle is determined by the ON-time divided by the Period. Both ON-time and Period are computed in the function set_duty_cycle_hw(). However, the ON-time is computed based on an old value of the Period. So if the Period decreases (switching frequency increases) the duty cycle is too high.
```

---
## \#95 Posted by: devin Posted at: 2016-09-18T09:04:35.005Z Reads: 149

```
<p>This post was flagged by the community and is temporarily hidden.</p>
```

---
## \#96 Posted by: lrdesigns Posted at: 2017-01-10T08:24:48.643Z Reads: 126

```
I get this surge somewhere above 50% speed. Its scary as frig and really annoying. I have learned to ride around it and typically don't use more than 50% of the throttle movement on the controller. 

Seems like there needs to be some load on the motors and at a certain speed you get a jerk of acceleration. At low loads and or low speed its not there. 

Its not voltage sag because Im using 8ah 12s lipo 25c. My battery limit is 20 amps, the batteries never get over ambient temperature. The batteries should easily be able to provide over 100 amps draw so sag should be very minimal. Also you would get this behavior on steep hills and heavy acceleration if it was due to voltage sag, but for me its more related to speed and throttle position. 

I would like to try the watt mode firmware but I need to buy a programmer first. 

I think my motor amp limit is at 40a, so I will try to increase that without adjusting the battery limit and see if I get any improvement as per devin's suggestion. I hope to come back here and give a comment if it improved the feel and reduced the surge.
```

---
## \#97 Posted by: devin Posted at: 2017-01-10T08:31:52.614Z Reads: 130

```
<p>This post was flagged by the community and is temporarily hidden.</p>
```

---
## \#98 Posted by: lrdesigns Posted at: 2017-01-12T02:36:45.556Z Reads: 127

```
Thanks, I gave it a try. I increased my motor amp to 50, while keeping the battery at 20.  It was actually motor 30 battery 20 before. I didn't expect much difference but low end power was much greater and helped on slow steep hills. But I already had too much power on flat ground and this gave me even more. So in my situation it did not solve my other issues.
```

---
## \#99 Posted by: Ackmaniac Posted at: 2017-01-12T07:40:30.918Z Reads: 124

```
I recommend to use my firmware mod and try watt control mode which makes the throttle better controllable. Next would be to adjust the throttle curve. That softens the throttle again when you have the right settings.
```

---
## \#100 Posted by: lrdesigns Posted at: 2017-01-12T08:31:27.442Z Reads: 128

```
I want to but I need to buy a programmer first :cry: as the maytech vesc has no bootloader. I will eventually get around to that.
```

---
## \#101 Posted by: sebaszz Posted at: 2017-01-12T09:17:22.457Z Reads: 130

```
Interesting i have exactly the same issue. It launched me yesterday after reducing cooling problems from 52 km/u @ 85% to 95% boost to almost 60 km/u before releasing throttle.

your firmware should solve this issue?

https://metr.at/r/6qTuA
```

---
## \#102 Posted by: Ackmaniac Posted at: 2017-01-12T09:21:39.651Z Reads: 134

```
No it doesn't solve that issue. It might only softens it as long as you don't give full power. The problem is the noise on the current sensors at around 85% duty cycle as Vedder mentions on his forum.
What i would be interested in is if the position of the battery and phase wires in the enclosure could make a difference.
```

---
## \#103 Posted by: Benji-Yafal Posted at: 2017-03-20T09:32:30.243Z Reads: 126

```
So if I understand correctly this post (cause my english is so bad)  nothing can solved this issue of Burst at 85% duty cycle ! The problem is relative to the Hardware ( noise on the current sensors ) and the only solution is to expect this boost when you ride or waiting to buy a Vesc 6.

@Ackmaniac 1000 Thanks for your Vesc FW 4.53 with the throttle curve ajustement !!! I ride on UnikBoard Dual and your software give me so much more control and precision during my ride ! Your FW is a "must have" when you ride a powerfull setup. I cant make you a donation for the moment but be sure that i will promote your work. Youre 12s5p flexible battery is also crazy !!! Can you give me the link of the built of your batterie and tell me if i'm right about the top of my post.
```

---
## \#104 Posted by: Ackmaniac Posted at: 2017-03-20T09:59:32.919Z Reads: 127

```
Yes the bower boost is hardware related. On the VESC-X i couldn't recognize a power boost yet on my dual setup. Need to test it on my single because there the power boost was stronger. But it seems that the VESC-X hardware design is better.

 I don't have a buidthread about my bettery but in this thread i have some pictures about my new battery pack.
http://www.electric-skateboard.builders/t/laser-cut-plywood-deck-with-solderless-18650/19005/34?u=ackmaniac
```

---
## \#105 Posted by: Benji-Yafal Posted at: 2017-06-22T14:17:10.594Z Reads: 106

```
I set up the "max duty cycle" to 0.89 and i din't fell the Boost, the max speed is a litle reduce but it's more safe
```

---
## \#106 Posted by: bigben Posted at: 2017-07-12T21:35:19.816Z Reads: 96

```
Has anyone found a solution or a way to make this better?
I have just set up dual enertion Vesc 4s with dual 5065 200kv motors.
The battery leads are very long, could this possibly be causing "noise"?
It is smooth as silk and very quiet but at just over 20mph there is what feels like nitro boost!
Really quick but sometimes a little unnerving?
```

---
## \#107 Posted by: TarzanHBK Posted at: 2017-07-13T06:50:46.193Z Reads: 89

```
download @Ackmaniac BLDC tool and tune the boost via the throttle curve
```

---
## \#108 Posted by: bigben Posted at: 2017-07-13T07:31:24.096Z Reads: 91

```
Cheers @TarzanHBK. 
Something to do this evening....
```

---
## \#109 Posted by: Paulf Posted at: 2017-07-13T07:43:03.424Z Reads: 90

```
If you do get it right, please, post your curve settings :sweat_smile:
```

---
## \#110 Posted by: Benji-Yafal Posted at: 2017-07-13T08:15:38.631Z Reads: 90

```
set up the "max duty cycle" to 0.89 and i din't fell the Boost
```

---
## \#111 Posted by: ninja Posted at: 2017-07-13T08:22:33.012Z Reads: 89

```
I don't think it will sort out this phenomen! It may help, but it will still boost.  http://www.electric-skateboard.builders/t/vesc-acceleration-boosts-at-high-speeds/9525

FOC BOX does it less and VESC 6 do not have this problem. But VESC 4... have that issue. I have it too, and it's very annoying. When I have mot max set to 70A it boost so hard that I cannot physically stand it.
```

---
## \#112 Posted by: Benji-Yafal Posted at: 2017-07-13T08:23:56.793Z Reads: 93

```
@bigben set the duty cycle max to 0.89 to minimize the Boost. 0.86 if you want to cut it totaly. You will loose a litlle of Max speed but increase the level of safety at High speed.
Trust Me ... and you will see that's this boost nothing to see with the throttle curve. Sorry @TarzanHBK but what you tell is wrong
```

---
## \#113 Posted by: TarzanHBK Posted at: 2017-07-13T09:21:38.138Z Reads: 93

```
try it with trottle curve or minimise the duty cycle (although i don´t like this solution) otherwise all you can do is swap to an other vesc without this problem.
Seems like there is nothing else you could do.
```

---
## \#114 Posted by: bigben Posted at: 2017-07-13T10:30:30.884Z Reads: 92

```
Is it just the Vesc 6 without this problem?
```

---
## \#115 Posted by: pshaw Posted at: 2017-09-04T02:27:51.404Z Reads: 74

```
Does anyone have a clear answer on which escs don't have this hardware bug?
```

---
