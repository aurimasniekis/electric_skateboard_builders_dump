# VESC BASED CONTROLLERS - Brakes locking at low speed for larger wheels in FOC - possible Unity Fix

### Replies: 161 Views: 3489

## \#1 Posted by: thisguyhere Posted at: 2018-11-05T17:19:58.964Z Reads: 363

```
@Deodand
@Eboosted
@mmaner
@psychotiller
 
with the unity under active development, i thought we could persuade @Deodand to finally address the locking brakes issue for larger diameter wheels in FOC.

it's kind of been started already:

https://www.electric-skateboard.builders/t/focbox-unity-official/64944/597

using this thread isolate the topic.
```

---
## \#2 Posted by: Deodand Posted at: 2018-11-05T17:22:08.663Z Reads: 332

```
@thisguyhere, you ordered a unity, and have a board that exhibits this behavior?  When you have your unit in hand mind spending a couple hours with me debugging/solving the issue? Basically get the board setup with the issue active, we will test a few config settings, if that doesn't work then I'll send you some modified FW to test with different fixes. Once I find a fix I'll open an issue on Vedder's git so it gets fixed there as well. 

If anyone with a beta unit has the issue I could start testing sooner.

Detailed descriptions of the problem, and also if it occurs in FOC/BLDC, Sensored/unsensored, and what is wheel diameter motor kv and gearing would be helpful.
```

---
## \#3 Posted by: thisguyhere Posted at: 2018-11-05T17:26:00.173Z Reads: 306

```
you got it, yea i've got unitys on the way.

will test it out when they get here, for sure.
```

---
## \#4 Posted by: mmaner Posted at: 2018-11-05T17:30:24.680Z Reads: 295

```
I'd be happy to help. I've got multiple boards the have this issue. 

It would be no problem to swap out the FocBox's in my Bludgeon 6 shooter build. I'm running 15/60 gears on 10s4p. 

My latest build has the issue as well, phat Matson deck on 107 flywheels with dual FocBox's on 12s3p. 

My gear drive build had the issue buy I'm testing arc 200s in it at the moment. It's a caldera deck on 7in numies with 12s4p.
```

---
## \#5 Posted by: Sender Posted at: 2018-11-05T17:36:42.870Z Reads: 281

```
Yup, all my builds have this and I have learned to live with it.  I just don't understand how it is like this going forward but "slowing down" and stopping while in reverse doesn't produce it.  If that makes sense.

I really hope this goes away with the Unity.
```

---
## \#6 Posted by: briman05 Posted at: 2018-11-05T17:37:16.877Z Reads: 277

```
Could this be a issue with 12s battery setups that we saw on the flipsky esc as well maybe for some reason these are not able to handle a 12s battery
```

---
## \#7 Posted by: Blasto Posted at: 2018-11-05T17:37:33.577Z Reads: 272

```
I have a engineering test unit in a Lacroix deck, dual 6374

I think my setting are:
motor:
60A
-50A

batt:
60A
-20A

![image|666x500](upload://aD3ZbCOkms785xvuzNw5YL61Fyg.jpeg) 

I have not felt this behavior
```

---
## \#8 Posted by: thisguyhere Posted at: 2018-11-05T17:38:03.809Z Reads: 255

```
What size wheels?
```

---
## \#9 Posted by: Blasto Posted at: 2018-11-05T17:39:43.627Z Reads: 262

```
`Hmmm not sure about the wheel size, 6”?  @Arch can you answer that`

7"

![image|466x500](upload://1MuoXcyQRPbHPa0AwDYifOL5bDc.jpeg)
```

---
## \#10 Posted by: psychotiller Posted at: 2018-11-05T17:39:56.358Z Reads: 253

```
I'll be setting up this build 10s. 220kv. 107s I'll let you know
```

---
## \#11 Posted by: Deodand Posted at: 2018-11-05T17:42:56.156Z Reads: 253

```
Can we potentially change the title to VESC BASED CONTROLLERS - Brakes locking at low speed for larger wheels in FOC

Edit: Thanks!
```

---
## \#12 Posted by: Deodand Posted at: 2018-11-05T17:58:15.134Z Reads: 243

```
One thing that I'll be implementing is scaling the plethora of erpm based settings based on motor flux-linkage during config. Essentially the flux linkage determines the amount of volts for a given ERPM, the amount of volts determines the signal quality that the unity has, and so for instance when to switch over from hall sensors to sensorless should just scale with the motor flux linkage and not require an additional config setting to work properly.
```

---
## \#13 Posted by: mmaner Posted at: 2018-11-05T18:02:56.069Z Reads: 243

```
[quote="briman05, post:6, topic:73547, full:true"]
Could this be a issue with 12s battery setups that we saw on the flipsky esc as well maybe for some reason these are not able to handle a 12s battery
[/quote]

Nope, it happens on 2 of my 10s builds.
```

---
## \#14 Posted by: brenternet Posted at: 2018-11-05T18:07:05.063Z Reads: 240

```
Links to those older threads if anyone wants to catch up 

https://www.electric-skateboard.builders/t/vesc-based-controllers-brakes-locking-at-low-speed-for-larger-wheels-in-foc-possible-unity-fix/73547

https://www.electric-skateboard.builders/t/wheels-brake-locking-in-foc-right-before-dead-stop/39136
```

---
## \#15 Posted by: DAddYE Posted at: 2018-11-05T18:11:33.814Z Reads: 216

```
I was able to solve this locking issue with my 105mm wheels by reducing the deadband from 15% to 2%. I’ve the mini remote. Give a shoot.
```

---
## \#16 Posted by: skatardude10 Posted at: 2018-11-05T18:25:30.372Z Reads: 217

```
I've always had this issue to some degree regardless of gearing/wheel size on my FOC sensored 10S setup. I've learned to live with it, but it would be great to not have to deal with it.

I'm not hip to how this stuff works, but talk of scaling something based on the back emf/erpm or whatever sounds sexy... This issue is one of those **SUDDEN** type things, and if it were even to just ramp slowly into the locking brakes that would be *so much* nicer.
```

---
## \#17 Posted by: Eboosted Posted at: 2018-11-05T19:23:38.683Z Reads: 217

```
[quote="DAddYE, post:15, topic:73547, full:true"]
I was able to solve this locking issue with my 105mm wheels by reducing the deadband from 15% to 2%. I’ve the mini remote. Give a shoot.
[/quote]

This is new, I'll give it a try
```

---
## \#18 Posted by: Jinra Posted at: 2018-11-05T19:29:32.322Z Reads: 214

```
Are you talking about the full short braking when you reach a certain eRPM threshold? I thought there was a setting for this in 2.xx firmware which seems to be missing in 3.xx; or at least i can't find it.
```

---
## \#19 Posted by: lrdesigns Posted at: 2018-11-05T21:54:32.345Z Reads: 218

```
Yeah I found “max erpm at full brake” is missing in 3.x firmware. 

For me in BLDC mode lowering the number made the slow to stop much smoother. 

https://www.electric-skateboard.builders/t/extended-ackmaniac-esc-tool-based-on-vesc-tool/35116/708?u=lrdesigns
```

---
## \#20 Posted by: rich Posted at: 2018-11-06T00:14:32.367Z Reads: 213

```
[quote="DAddYE, post:15, topic:73547"]
reducing the deadband from 15% to 2%
[/quote]

Gonna try that, too.

I got used to the locking brakes but would love to get rid of it. My bigger problem is when riding really steep downhill with my MTB with full braking, often the wheels block 100% and I start slipping or fall. This is really annoying. I have Vesc6 FW 3.38  with 149kv 6374's running in FOC (12s) with 1:5 gearing on 8" wheels.
```

---
## \#21 Posted by: lrdesigns Posted at: 2018-11-06T00:41:11.522Z Reads: 190

```
I have a theory that its worse on low KV motors. I run 140kv what all you guys that had problem running?
```

---
## \#22 Posted by: Jinra Posted at: 2018-11-06T00:42:18.235Z Reads: 181

```
That would make sense if the full short occurs at a specific eRPM as indicated on 2.xx firmware
```

---
## \#23 Posted by: rich Posted at: 2018-11-06T00:47:35.548Z Reads: 180

```
149kv with 1:5 gearing on 8" wheels.
Edited my previous post, too
```

---
## \#24 Posted by: thisguyhere Posted at: 2018-11-06T01:57:45.065Z Reads: 180

```
[quote="DAddYE, post:15, topic:73547"]
reducing the deadband from 15% to 2%
[/quote]

This is just a workaround but doesnt address the actual problem. 

Max erpm at full brake is a setting that works great in bldc, the same should be available for foc, imho. 

I believe Deodand can do it with feedback from us.
```

---
## \#25 Posted by: Trdolan03 Posted at: 2018-11-06T15:47:15.312Z Reads: 172

```
Similar question but is there any setting to hold the position of the board and not “creep” down a slight hill? I have the same issue listed above. 190kv 12s 8” wheels.
```

---
## \#26 Posted by: thisguyhere Posted at: 2018-11-06T16:00:36.805Z Reads: 169

```
at no speed the brakes should feel like their locked in foc with some slippage.

short of a mechanical brake the motor can't lock the brakes 100%.
```

---
## \#27 Posted by: Trdolan03 Posted at: 2018-11-06T17:20:31.003Z Reads: 168

```
[quote="thisguyhere, post:26, topic:73547"]
foc with some slippage.
[/quote]

Why is this so? They have sensors so shouldn’t they be able to fully lock
```

---
## \#28 Posted by: thisguyhere Posted at: 2018-11-06T17:24:46.643Z Reads: 168

```
the motor magnets aren't nearly strong enough to have a complete attractive force.
```

---
## \#29 Posted by: ShutterShock Posted at: 2018-11-06T18:09:35.000Z Reads: 170

```
I am gonna keep really close watch on this thread, it is absolutely annoying to be riding slow along next to someone and touch the brakes and jerk. 

I have 90mm wheels, 12s, 190kv.  Two focboxes,  never had an issue in BLDC when I had my Torqueboards controllers, but as soon as I switched, and switched to FOC, I have had the locking issue.  

Also sidenote I couldn't get BLDC to even work on my FOCBOX's.  No idea why, Sensored FOC works perfectly fine.
```

---
## \#30 Posted by: thisguyhere Posted at: 2018-11-06T18:14:19.955Z Reads: 164

```
curious, 90mm wheels shouldn't be affected.

but, let's see how this develops.
```

---
## \#31 Posted by: Trdolan03 Posted at: 2018-11-06T19:49:58.116Z Reads: 169

```
[quote="ShutterShock, post:29, topic:73547"]
Also sidenote I couldn’t get BLDC to even work on my FOCBOX’s. No idea why, Sensored FOC works perfectly fine.
[/quote]
Could you explain this further?
```

---
## \#32 Posted by: skatardude10 Posted at: 2018-11-06T20:10:35.857Z Reads: 167

```
You can try current with reverse. This is what I do to hold position on a downhill slope- come to a stop as much as possible and engage reverse and hold that slightly to keep held in one position. Don't know if something similar is possible with current no reverse.
```

---
## \#33 Posted by: ShutterShock Posted at: 2018-11-06T21:12:38.878Z Reads: 168

```
So I'm talking about when you do motor detection.  When I had the TB vescs, I only ran them in hybrid BLDC, which worked perfectly.  I could run motor detection perfectly fine, and I never tried FOC.

However, as soon as I got the FOCBOX's I tried to set them up to run BLDC and I could never get motor detection to run and detect the motors.  I had nothing on the motors, and even tried looking around, all over the forum and I couldn't figure out why.  Tried increasing amps, etc.  So I ended up just doing sensored FOC which detected perfectly fine on both.
```

---
## \#34 Posted by: Trdolan03 Posted at: 2018-11-06T21:54:21.183Z Reads: 164

```
That’s weird. I had issues getting them to detect when I had my gear drives and pneumatics attatched but when I ran it with just the motor it worked just fine. I like FOC more anyways but something to try if you really want BLDC
```

---
## \#35 Posted by: trampa Posted at: 2018-11-06T22:26:18.105Z Reads: 164

```
Do you use symmetric settings for motor regen and battery regen. Like -30A and -30A?
Some people use crazy high motor regen values but terrible low battery regen values. Like -80A and -10A. In that case your brakes at speed would be super weak and would get super aggressive when you are slow. Such a setting could lock your wheels if you don't release the trigger fast enough. Symmetric settings give the most linear braking behavior and guarantee good brakes at speed.
```

---
## \#36 Posted by: Jinra Posted at: 2018-11-06T22:37:17.710Z Reads: 161

```
that's not really true, i use -60/-15 and my brakes are just fine. using -30a battery regen, especially with dual, is insane as your battery is not equipped to handle that much charge current.
```

---
## \#37 Posted by: rich Posted at: 2018-11-07T08:31:39.383Z Reads: 168

```
I want to shoot a video with telemetry data where we can see what's happening when the wheels lock up.
I got a hole in my trousers and a bit bloody knee from last week in a skate park, guess why? The wheels locked while braking on a concrete hill :laughing:

[quote="trampa, post:35, topic:73547"]
Do you use symmetric settings for motor regen and battery regen
[/quote]

No but nothing extreme (see data below)
I have some telemetry data of 3 different motors on my mountainboard.

Interesting is that the batt regen while braking never came close to set limits, in most cases below 50% 
So I don't think it makes any difference when setting higher batt regen values.

The following pics show data of both motos together.
____

SK8 6374 149kv | 10T/50T gear drive | 200mm wheels
Settings: Motor max 80A | Batt max 50A | Motor regen -40A | Batt regen -15A

![SK8_20181015|195x122](upload://4caR8spNeWfDKHdo0Gt16FpU8vW.jpeg) 

____

TRAMPA 6364 136kv | 15T/66T belt drive | 200mm wheels
Settings: Motor max 50A | Batt max 50A | Motor regen -25A | Batt regen -15A

![TrampaMotor_20180215|195x122](upload://sg7A44EJuvGkXpgQbG6bHWRcqzS.jpeg) 

____

UNIK 6374 150kv (sealed Maytech) | 10T/50T gear drive | 200mm wheels
Settings: Motor max 65A | Batt max 50A | Motor regen -35A | Batt regen -15A

![Unik_Telemetry1|414x259](upload://3TZZopvAiW3dwdd5FSIWPMwLJIY.jpeg)
```

---
## \#38 Posted by: trampa Posted at: 2018-11-07T09:03:12.532Z Reads: 160

```
Try symmetric settings and your brakes will be super linear and very controllable. Benjamin Vedder does the same BTW. He knows why. Try -30A -30A or -30A and -25A. 
Battery Max Regen defines the brake strength at speed and Motor Max Regen becomes more dominant with  lower speeds. The transition between the two values can be very aggressive and uncontrollable when you have non symmetric values.  Battery Max Regen will swell down very fast anyway and your battery can handle that short spike for sure.
```

---
## \#39 Posted by: rich Posted at: 2018-11-07T09:25:48.125Z Reads: 167

```
[quote="trampa, post:38, topic:73547"]
The transition between the two values can be very aggressive and uncontrollable when you have non symmetric values
[/quote]

But as the thread title states it is about locking wheels at low or very low speed. Do you mean the transition is happening at this very low speed?


My brakes at higher speed are fine with -15A batt max regen each motor, I don't want stronger brakes at speed.

The brakes are fine at lower speed as well so the only way to get it more symmetrical is to lower the motor regen to -20A instead of -40A which is half break strength. But I can test it for science just to know if the wheels lock, too.
```

---
## \#40 Posted by: trampa Posted at: 2018-11-07T09:28:17.442Z Reads: 159

```
Do that, try -20 -20. They will be butter smooth.
```

---
## \#41 Posted by: Deodand Posted at: 2018-11-07T09:47:27.651Z Reads: 149

```
I do not agree that this will solve the issue. Assymetric values will cause your brakes at high speed to be weaker than your brakes at low speed but the transition will be a linear ramp, not a sudden jerk just before coming to a stop that throws you from your board as is being described here.
```

---
## \#42 Posted by: Trdolan03 Posted at: 2018-11-07T18:11:38.746Z Reads: 150

```
Use bindings and you don’t get thrown🤣
```

---
## \#43 Posted by: thisguyhere Posted at: 2018-11-07T18:23:21.481Z Reads: 148

```
belt slips when it locks
```

---
## \#45 Posted by: thisguyhere Posted at: 2018-11-07T18:32:10.726Z Reads: 146

```
good for u
```

---
## \#46 Posted by: hexakopter Posted at: 2018-11-07T21:46:04.771Z Reads: 154

```
I haven't followed all the linked threads before this one, but for me it sounds like what you describe as "lockup" is the phase where the VESC switches from regen braking to shorting the motor phases. At least that is what I notice on my bike using a 11.9 kV motor. I searched for a log from the past to show that behavior, because right now can't test it. I found that:
https://metr.at/r/UzGCa
There you can see that the braking after 16:53:34 switches at around 6 km/h. (don't get distracted from the high current pull before, were I was testing steep hill climb capabilities :slight_smile: )  You can clearly feel that the braking changes and I wouldn't be surprised that this is what you describe as "locking issue" because it is abrupt and changes the braking force drastically.
```

---
## \#47 Posted by: Deodand Posted at: 2018-11-07T21:58:00.619Z Reads: 148

```
this is BLDC or FOC?
```

---
## \#48 Posted by: hexakopter Posted at: 2018-11-07T21:59:03.465Z Reads: 150

```
FOC  10 char
```

---
## \#49 Posted by: Deodand Posted at: 2018-11-07T22:20:57.480Z Reads: 157

```
Ok great this is super helpful! Looking at the [mcpwm_foc.c](https://github.com/vedderb/bldc/blob/master/mcpwm_foc.c) code at line 1676 looks like it might be one possible source of the issue:

    
		// When the filtered duty cycle in sensorless mode becomes low in brake mode, the
		// observer has lost tracking. Use duty cycle control with the lowest duty cycle
		// to get as smooth braking as possible.
		if (m_control_mode == CONTROL_MODE_CURRENT_BRAKE
				//				&& (m_conf->foc_sensor_mode != FOC_SENSOR_MODE_ENCODER) // Don't use this with encoders
				&& fabsf(duty_filtered) < 0.03) {
			control_duty = true;
			duty_set = 0.0;
		}
interestingly this bit of code is enabled with or without hall sensors enabled. The only bit that doesn't make sense is this should be triggered when the duty cycle is less than 3% but in hexakopter's plot we see the duty cycle plummet is starting at 19% duty cycle which is strange. 

Are you running a sensored motor?
```

---
## \#50 Posted by: hexakopter Posted at: 2018-11-07T22:46:51.607Z Reads: 152

```
Great that it is helpful. Maybe someone else with a Metr Pro module can share a record were he is braking and noticed that locking problem. The problem with my record is that I can't remember if and how much I was using the mechanical brake of my bike, which would distort the data. In general I am just using the mechanical brake at slow speeds because I don't like that switching phase, so its hard to find another log where I am using the VESC to brake at very slow speeds.

Yes, I am using the hall sensors from my motor. So sensored FOC. The brake settings are -100A motor current and -12A battery current. I also would like to use motor current = battery current to get a linear feeling, but thats just not possible with my battery without destroying it. So for me @trampa's suggestion to just put in -30A battery current on a dual ESC setup sounds quite dangerous or at least not healthy for the battery, because just very few batteries can handle that.
```

---
## \#51 Posted by: Deodand Posted at: 2018-11-07T22:54:22.753Z Reads: 145

```
Re- examining the data and re-reading your post now I actually think this is a very good candidate for the bit that causes the phenomenon described. I'm not certain why if you have hall sensors it would be preferable to keep this enabled. Maybe I should hop over to Vedder's forum and see if he can explain the reasoning.
```

---
## \#52 Posted by: Deodand Posted at: 2018-11-08T03:11:01.855Z Reads: 146

```
Just tried out some FW with this subsection commented out, definitely not an improvement :smile: though I trust vedder enough to know it wasn't there for nothing. Even with hall sensors the motors vibrate like crazy when approaching low rpms.


~~I had an idea for a solution. People that are experiencing issues with this problem in FOC, go into vesc tool and try turning down the following two variables by like, a factor of 10 (just to effect dramatic change)~~

Motor Settings -> FOC -> Advanced -> Duty Downramp Kp
Motor Settings -> FOC -> Advanced -> Duty Downramp Ki 

~~I think the defaults are 10 and 200 so try instead 1 and 20. Then go out and use your breaks and report back please!~~

EDIT: 

    			if (fabsf(duty_set) < (duty_abs - 0.05) ||
					(SIGN(m_motor_state.vq) * m_motor_state.iq) < m_conf->lo_current_min) {

Because of this if statement on line 1696 (our duty cycle is at most 3% off and this sets a threshold of 5%) the duty downramp controller is never used for that final 3% margin that causes unsmooth motion. I'm getting closer to a solution here but need to sleep. Don't bother changing those gains it won't effect anything.
```

---
## \#53 Posted by: thisguyhere Posted at: 2018-11-08T03:12:12.130Z Reads: 139

```
Bookmarked, will try it and report back
```

---
## \#54 Posted by: trampa Posted at: 2018-11-08T08:55:15.004Z Reads: 142

```
[quote="hexakopter, post:50, topic:73547"]
So for me @trampa’s suggestion to just put in -30A battery current on a dual ESC setup sounds quite dangerous or at least not healthy for the battery, because just very few batteries can handle that.
[/quote]
First of all: On a skateboard no one pulls a 100% brake at full speed. It would throw you off. 
You wouldn't pull your front brake on your bike 100% at speed, same thing. You have a build in Amp limiter in you hand.
Second: once the speed gets lower you will not be able to push the full current injection. Battery currents drop fast with decreasing speed. If your motor is maxed at -30A regen, your battery will see a max of 15A at half the speed. In reality values are even lower.
Third: When do you need strong brakes you are happy to have them and a linear behaviour is always more controllable and predictable.
Fourth: If your battery will ever see a 20A injection, it will be for a very very short time only. A MTB 12S 4-7P battery pack can handle that with ease. Big Lipos will swallow such a short current injection even better.
```

---
## \#55 Posted by: jadatmag Posted at: 2018-11-08T10:02:49.428Z Reads: 145

```
Current raptor 2's have a battery min of -10 out of the box. You can change this to -12 but anything lower won't work.

So with my current settings it's battery -12A and Motor -55A. And the lockup is real. At high speeds I can fully brake while doing the [Karate kid final kick](https://youtu.be/nle_WV_UY5E). And below a certain speed the wheels suddenly start skidding.

Here's a video of me going from full speed to full brake.
https://youtu.be/0Eg0bDobu0Y?t=3m35s

Setting up braking linear on the Raptor 2 can't be done. I'm really tempted to void warranty by flashing non-Raptor 2 firmware. -20A/-24A motor min would change how I ride this board.

Will the Unity change this for Raptor 2.1?
```

---
## \#56 Posted by: deucesdown Posted at: 2018-11-08T15:10:11.710Z Reads: 146

```
[quote="jadatmag, post:55, topic:73547"]
void warranty by flashing non-Raptor 2 firmware
[/quote]

I think we are okay to flash?

https://enertionboards.zendesk.com/hc/en-us/articles/360000406455-How-to-configure-R2-with-BLACK-motors-OR-stuttering-problems

@barajabali
```

---
## \#57 Posted by: barajabali Posted at: 2018-11-08T15:12:58.249Z Reads: 146

```
Technically,  Flashing with anything other then 2.18 or 2.8 can void your warranty. 

But we haven't had to enforce that recently
```

---
## \#58 Posted by: Deodand Posted at: 2018-11-08T17:38:44.165Z Reads: 148

```
I think this asymmetric braking issue is something different from the problems described in this thread where  at the final little bit before stopping wheels lock. It is good to bring up to differentiate between the two behaviours though. 

I am determined to get the topic issue of this thread solved. I think I have identified the FW bits that are the culprit which is awesome! Now it's just a matter of figuring out how best to implement a fix. I tried about 10 different things last night, its a tricky problem let me see if I can explain the issue here:

The braking mode in FOC works by always applying a current relative to the throttle pull in the opposite direction of the current velocity. As the velocity gets very small it becomes exceedingly difficult to determine what the direction of travel is. Even if you have hall sensors, as one hall sensor ticks up it indicates you are going 1 direction if you apply brake current and it then sends you in the opposite direction, the hall sensor will kick back and you end up with vibrational behaviour as the motor bounces back and forth between the two halls. Additionally each time there is a zero crossing the vesc applies full braking current in the opposite direction, the results are noisey and not ideal if you try to use this method close to zero speed.

Simply releasing the brake at extremely low speed probably isn't acceptable either as it would be quite annoying to always roll smooth until small speed picked up then jerk to a stop when full brake held in. 

My understanding of what happens instead is at a certain low speed the software simply shorts all the motor leads together, and this causes active field collapse which induces a viscous damping effect within the motor. Please someone correct me if this understanding is incorrect! Take a motor on your bench, electrically connect all three of its leads and feel the result. The problem is, the braking force of this phenomenon may not match well with the braking force of normal braking, and the hard switch (an if statement that duty cycle < 0.03 AKA 3% of max speed) causes behaviour that feels non-smooth and is one of the last parts of the vesc FW that doesn't behave intuitively. 

I think this braking behavior is also responsible for that Gummy/hysteresis feel in your brakes at lower speed and high braking force down steep hills if anyone has felt that phenomenon before. I'm talking down a steep hill when you are braking hard and you let on and off the brakes and feel kind of a soft latching/unlatching feeling in the brakes.
```

---
## \#59 Posted by: ShutterShock Posted at: 2018-11-08T17:41:18.761Z Reads: 139

```
Well you have definitely hit the nail on the head about what the problem is, this exactly describes everything that is annoying haha.

Now just to figure out if there is a way to fix it
```

---
## \#60 Posted by: thisguyhere Posted at: 2018-11-08T17:43:33.395Z Reads: 140

```
Incredible, great analysis.  And your description of the phenomena is 100% on point.

Again, amazed at the time you're putting into this, I am deeply humbled.
```

---
## \#61 Posted by: Deodand Posted at: 2018-11-08T17:43:57.497Z Reads: 142

```
I have more than a few ideas to try out, If I can get my hands on a test board to use in the hotel in Shenzen next week I'll try to crack this over some beers in the hotel with @Blasto.
```

---
## \#62 Posted by: trampa Posted at: 2018-11-08T18:51:56.812Z Reads: 142

```
Since open source you can flash whatever you like and then flash the original FW back whenever you like.
No one can proof that you used different FW in the meantime. 
If you don't have the original FW you can ask for it and there is a duty for Enertion to send it to you or offer a download. They need to do that for another 3 years after last distribution of software or hardware with that FW on. 
You should always use the latest VESC-Tool and FW anyway. There are some safety improvements in VESC-Tool that do not come with the older stuff. Benjamin highly recommends not to use the old BLDC-Tool any longer. It doesn't get any critical safety updates and is outdated.
One feature that is very important to have is **Acceleration temperature decrease.** Without that feature your brakes can drop out at when your motors reach critical temperatures. The ESC will cut back the power when the motors overheat. It will also cut back the power of the brakes! In consequence you will not have any brakes when needed.  **Acceleration temperature decrease** will give the brakes headroom to work at any time. Especially with hub motors this feature can be your life saver! Hubs tend to overheat faster and the risk of ending up without brakes is very high. 

Since sources for the Enertion distribution of BLDC-Tool are still non existent, the community has no chance to work such a feature into that software or find existing issues. Open Source should work in a way that many eyes look at the code and weed out the weaknesses, so that it gets better and better, safer and safer.
```

---
## \#63 Posted by: trampa Posted at: 2018-11-08T18:54:55.358Z Reads: 137

```
[quote="Deodand, post:61, topic:73547"]
I have more than a few ideas to try out, If I can get my hands on a test board to use in the hotel in Shenzen next week I’ll try to crack this over some beers in the hotel with
[/quote]

Some other guys might also have an idea how to solve the matter. They just can't find the sources...
```

---
## \#64 Posted by: Deodand Posted at: 2018-11-08T18:59:22.231Z Reads: 137

```
The issue is with all vesc firmwware? The code I'm talking about is all in reference to vedders repository. The unity code would be completely useless as no one has unity hardware for testing. Anything I code up should be plug and play with a regular vesc but I've only identified what I think is the problem so far.
```

---
## \#66 Posted by: Deodand Posted at: 2018-11-08T19:58:22.547Z Reads: 133

```
@trampa I'm going to flag this as off topic because I don't want to distract from the issue this thread is trying to address, but I hear what you are saying. We actually tracked down the source files for the raptor 2 tool and they were supposed to be posted weeks ago, I'm not sure why that never happened but I will get it fixed. The focbox firmware is just stock firmware with a few #defines changes and the vesc project ethos page suggests not creating new repos for such small changes. 

Seeing as to how the focbox is working reliably for many users with the firmware that is locked into it I think there are pros and cons to continuous firmware updates that you aren't addressing. The phrase "If it ain't broke don't fix it" comes to mind. That said I am personally a fan of the rolling FW updating but you can't ignore the fact that there are tradeoffs.
```

---
## \#67 Posted by: Sender Posted at: 2018-11-08T19:59:03.059Z Reads: 134

```
[quote="Deodand, post:61, topic:73547"]
Shenzen next week I’ll try to crack this over some beers in the hotel with @Blasto.
[/quote]

Wait. Is @blasto their with you? Just curious. Sorry to drop the D in Derail.
```

---
## \#68 Posted by: Blasto Posted at: 2018-11-08T20:02:48.587Z Reads: 135

```
Yeah i’m heading over there tomorrow morning... well actually i’ll arrive saturday night, 24+hrs of travelling... can’t wait🐲
```

---
## \#69 Posted by: Sender Posted at: 2018-11-08T20:04:16.710Z Reads: 135

```
Thats awesome!  Have fun!
```

---
## \#70 Posted by: Pedrodemio Posted at: 2018-11-08T20:16:58.304Z Reads: 135

```
Just throwing some ideas, I remember about vedder saying about active braking in his old forum a few years back, could this be an answer? Using energy to modulate the braking a really low speed or you get back to same problem since you can't determine the motor position and speed?

And the behavior is exactly what you describe, the worst is that when you actually enter the shorting phase you can't modulate it anymore, some hills you want to go down really slow, below the 3%, but full brake will still bring you to a stop
```

---
## \#71 Posted by: Deodand Posted at: 2018-11-08T20:20:34.809Z Reads: 140

```
The other thing that happens is once you enter that braking range the duty is **commanded** to zero so even if you speed back up going down the hill it stays in the full stop mode and doesn't exit properly.

My thoughts were to look into a model for active field collapse, see if maybe I could get some kind of torque estimate, then pwm rapidly in and out zero duty and modulate it to try and better match forces during transition. Just one idea though.
```

---
## \#72 Posted by: trampa Posted at: 2018-11-08T21:24:36.492Z Reads: 143

```
On Topic: Geared systems suffer less since the motor spins 3 - 6x faster at a low speeds. Higher ratio = smoother braking. A high accuracy encoder works very well (AS5047P) to run the motor at super slow ERPMs  Non geared systems have a lower ERPM at the same physical speed. "Lockups" will probably happen at higher speeds. I Never tried it out, no hub to hand - still paddling my bike to work. 

Personally I never encountered such lockup issues. I can brake any of my boards to a standstill without a motor lockup. Just before the board totally stops (1-2KM/h) you can feel that the motor can't be tracked properly any more. A generator works when it spins.... 

[quote="Deodand, post:66, topic:73547"]
The focbox firmware is just stock firmware with a few #defines changes and the vesc project ethos page suggests not creating new repos for such small changes.
[/quote]

OFF Topic: The Ethos page suggests no to fork for minor changes that could also be worked into the original distribution. A repo is always needed along with all other obligations. Once you run a fork you are all in!
A small change can make a big difference. For example a changed FW revision number can make FW updates impossible. Small change big impact! This is why any changed software needs to be shared.
```

---
## \#73 Posted by: lrdesigns Posted at: 2018-11-09T00:32:07.734Z Reads: 140

```
[quote="Deodand, post:58, topic:73547"]
I think this braking behavior is also responsible for that Gummy/hysteresis feel in your brakes at lower speed and high braking force down steep hills if anyone has felt that phenomenon before. I’m talking down a steep hill when you are braking hard and you let on and off the brakes and feel kind of a soft latching/unlatching feeling in the brakes.
[/quote]

This is exactly the thing I was trying to describe in the @Ackmaniac  firmware thread. It's a sticky latching type feeling on steep hills that is kinda dangerous. The slow speed to stop on flat ground also feels similar to me. Just less violent. 

I run BLDC so its not just a FOC thing. It may be more apparent in FOC I don't know I have not tried. I did not experience it in the firmware 2.17 but then did in 3.102. I kept the same settings when I switch over to 3.1.

I have kind of got used to it, just need to release the brake slowly as you slow down, where as before I could just hold the brake in one positing and get fairly constant stopping force relative to speed. Not an increase in stopping force when the speed decreases. 

For reference. I am using 4.12 hardware in BLDC, ackmaniac 3.102 firmware, 12s lipo, 140kv 5065 dual, 18:36 gearing, 97mm wheels, 100kg rider. :skateboard:
```

---
## \#74 Posted by: hexakopter Posted at: 2018-11-10T00:39:59.408Z Reads: 140

```
[quote="Deodand, post:58, topic:73547"]
My understanding of what happens instead is at a certain low speed the software simply shorts all the motor leads together, and this causes active field collapse which induces a viscous damping effect within the motor. Please someone correct me if this understanding is incorrect!
[/quote]
That is the same understanding that I have and tried to explain in my first post in this thread. Its great to see that you are working on it. :+1: The only perfect solution I see right now to solve that low speed tracking issue is using encoders.

Off topic:
[quote="trampa, post:54, topic:73547"]
First of all: On a skateboard no one pulls a 100% brake at full speed. It would throw you off.
[/quote]
That is actually what I do on the skateboard. Pulling 100% brake at full speed. At full speed the battery current is the one limiting braking and I actually would like to brake harder and am far off from being thrown off. But I can't use higher values without harming the battery.
When you recommend people to use -30A battery current on dual setups then it is your thing. Just thinking about my board with 5200mAH LiPos that are specced at 1C max charge the 60A you recommend are more than 11 times as high as the manufactures max specification. That leads to more than just a slightly decreased battery lifetime....

[quote="trampa, post:62, topic:73547"]
One feature that is very important to have is **Acceleration temperature decrease.** Without that feature your brakes can drop out at when your motors reach critical temperatures. The ESC will cut back the power when the motors overheat. It will also cut back the power of the brakes! In consequence you will not have any brakes when needed. **Acceleration temperature decrease** will give the brakes headroom to work at any time. Especially with hub motors this feature can be your life saver! Hubs tend to overheat faster and the risk of ending up without brakes is very high.
[/quote]
One fact that you just oversee is that your motor needs a temp sensor inside for that feature and thats just not the case for a lot of motors, so that this "very important life saving" feature is useless for builds using the popular SK3 motors for an example.
```

---
## \#75 Posted by: lrdesigns Posted at: 2018-11-10T01:31:08.991Z Reads: 133

```
Off topic. 1c is full charge from empty in 1 hour. What we are doing is high amp pulse charge for a few seconds. 

As far as I know there is no scientific research on this use case and it’s effect on battery life. 

It’s logical that a battery can take a much higher pulse then it’s rated C charge. How that effects it’s life we don’t know. 

Most people will choose shorter battery life over a high speed crash though.
```

---
## \#76 Posted by: trampa Posted at: 2018-11-10T06:58:12.954Z Reads: 138

```
[quote="hexakopter, post:74, topic:73547"]
When you recommend people to use -30A battery current on dual setups then it is your thing
[/quote]

Yes I do recommend to have settings that result in a strong and reliable brake. Better a slightly decreased battery life than a decreased personal life. In reality your battery will not see 30A ever. 
The C rating refers to a complete charge.
A Twin MTB like @rich has doesn't run of a single 5200mAh pack. 

Acceleration temp decrease: No motor sensors no problem. You will be able to push your motor temp till the motor falls apart. Most loose magnet issues happen because of to high motor temps. 
The heat expansion cracks up the glue holding the magnets.

The problem with sensors on outdated software: If the ESC cuts back the power due to hitting motor temp limits, it also cuts back the brakes. 
Motors get hot when you cane the board and when you go fast. In that scenario you don't want to end without brakes! We tested it out with deactivated setting, driving our motors to 110deg. 100% loss of brakes! Benjamin had the fix out within a night shift. 

The R2 has sensors, hot motors, lacks the feature and the riders do not necessarily understand the tech. This combo ain't good and in consequence users should update to Vesc-Tool ASAP. Discouraging people to do so puts people at risk! If the source code would be public someone could have updated the Software. This is a perfect example why it is important to have the sources accessible. 

Motor lockups at ultra low speed: We will have a look into this next weekend. Without having encoders installed low speed FOC rotor tracking and ultra low ERPM motor driving is an issue.
It's nothing you can solve with ease.
```

---
## \#77 Posted by: ShutterShock Posted at: 2018-11-10T18:22:03.005Z Reads: 131

```
I think this motor temperature thing is really not a concern for certain individuals.  My motors rarely ever even get warm to the touch and I run 80A -80A, so I think that is completely different than the raptor which basically has motor cozies (the wheel) around the motor.
```

---
## \#78 Posted by: hexakopter Posted at: 2018-11-16T22:36:05.678Z Reads: 142

```
[quote="Deodand, post:49, topic:73547"]
Ok great this is super helpful!
[/quote]


Did a new recording with full electrical braking to a full stop (no mechanical brakes). You can see how the motor phase gets shorted at around 8-10kmh. Maybe you are also interested in the current graph from that record.
https://metr.at/r/iG122
```

---
## \#79 Posted by: Deodand Posted at: 2019-01-07T18:45:57.502Z Reads: 136

```
Testing a fix: 

https://www.electric-skateboard.builders/t/need-a-few-testers-with-focbox-unity-builds-low-speed-braking-fix-needs-testing/80201?u=deodand
```

---
## \#80 Posted by: skatardude10 Posted at: 2019-01-09T05:38:16.291Z Reads: 134

```
THANKS @Deodand!!!  Works great with [changes applied to Ackmaniac's FW](https://www.electric-skateboard.builders/t/need-a-few-testers-with-focbox-unity-builds-low-speed-braking-fix-needs-testing/80201/57?u=skatardude10) on my dual FOCBOX setup!
```

---
## \#81 Posted by: ervinelin Posted at: 2019-01-09T08:51:42.362Z Reads: 132

```
Has anyone ported this over to the regular VESC firmware?
```

---
## \#82 Posted by: skatardude10 Posted at: 2019-01-09T21:22:17.961Z Reads: 131

```
I did for Ackmaniac's FW v3.102, see link above.  I could make the change on the latest standard firmware, and as long as the firmware builds without errors I can upload it tonight, I won't be testing it though.

It seems this fix is still a work in progress, some quirks but progress for sure.
```

---
## \#83 Posted by: skatardude10 Posted at: 2019-01-10T01:20:41.836Z Reads: 131

```
Here's vedder's latest firmware recompiled with Jeff's FOC brake modification.

https://drive.google.com/drive/folders/1hzGp4itbqEqvEZpJ_Gx3BuWK38q1RL0K?usp=sharing

Under /bldc/build_all/ you will find all of the hardware versions for flashing. The rest of the code is there in case anyone feels the need to verify, only changed lines 1680-1685 of mcpwm_foc.c. Didn't fork because my account already has a fork of bldc from Ack and don't want to make another github just for this.
```

---
## \#84 Posted by: ShutterShock Posted at: 2019-01-29T20:46:03.534Z Reads: 118

```
Is there a video of anyone with this working?  What are the results?
```

---
## \#85 Posted by: Deodand Posted at: 2019-01-29T20:48:32.896Z Reads: 121

```
I fixed most of the chatter with the following change: 

    if (m_control_mode == CONTROL_MODE_CURRENT_BRAKE
        //              && (m_conf->foc_sensor_mode != FOC_SENSOR_MODE_ENCODER) // Don't use this with encoders
        && fabsf(duty_filtered)*GET_INPUT_VOLTAGE() < 0.5
        && (fmax( fabsf(m_iq_set) , 0.5/(m_conf->foc_motor_r*2/3) ) >  (double) fabsf(m_motor_state.iq_filter))) {
      control_duty = true;
      duty_set = 0.0;
    }
```

---
## \#86 Posted by: ShutterShock Posted at: 2019-01-29T20:48:56.169Z Reads: 117

```
Is that the one that makes the weird noises?
```

---
## \#87 Posted by: skatardude10 Posted at: 2019-01-29T20:58:50.949Z Reads: 114

```
Yeet, thanks Jeff can't wait to try this tonight 😎😎
```

---
## \#88 Posted by: Bjork3n Posted at: 2019-01-29T21:05:12.706Z Reads: 110

```
Let us know if it works :)
```

---
## \#89 Posted by: kalebludlow Posted at: 2019-01-29T23:35:06.333Z Reads: 109

```
big yeet
10char
```

---
## \#90 Posted by: DAddYE Posted at: 2019-01-30T01:34:11.307Z Reads: 119

```
Tested! **Works like a charm!**

I patched the standard Vedder firmware. I'm using focboxes, MBS 100MM, and 200kv BKB motors.

It never stopped that smooth. I'm happy! Thank you  @Deodand!

Here my changes:

https://github.com/vedderb/bldc/compare/master...DAddYE:fix_stop

If you want you can download the stock firmware with @Deaodand patch by downloading from:

https://github.com/DAddYE/bldc/tree/fix_stop

These files under:

```
build_all/410_o_411_o_412/
build_all/46_o_47/
build_all/48/
build_all/60/
```

Happy DYIng
```

---
## \#91 Posted by: skatardude10 Posted at: 2019-01-30T02:06:25.461Z Reads: 116

```
Did you try his original fix? 

If so, how does the updated code compare to the first iteration?
```

---
## \#92 Posted by: Deodand Posted at: 2019-01-30T02:37:38.434Z Reads: 110

```
I missed an absolute value somewhere that was causing majority of chatter.
```

---
## \#93 Posted by: DAddYE Posted at: 2019-01-30T02:50:15.271Z Reads: 108

```
Nope, I didn't because here was raining; I tried just this one. 
Brakes are smooth as butter when you come to a dead stop, and there is no chatter.
```

---
## \#94 Posted by: ShutterShock Posted at: 2019-01-30T02:52:39.060Z Reads: 111

```
Wait so this link above

[quote="DAddYE, post:90, topic:73547"]
Tested! **Works like a charm!**

I patched the standard Vedder firmware. I’m using focboxes, MBS 100MM, and 200kv BKB motors.

It never stopped that smooth. I’m happy! Thank you @Deodand!
[/quote]


Is this the one that is working great?
```

---
## \#95 Posted by: skatardude10 Posted at: 2019-01-30T04:23:28.668Z Reads: 115

```
Patched Ackmaniac 3.102 firmware: 

https://github.com/skatardude10/bldc

Firmware rebuilt under build_all in that repo.

Loading up for testing now myself.

Edit: Shur enough, works great! No more stuttering, and smooth stopping without locking up in FOC! Thanks again Mr. Jeffery! :stuck_out_tongue: 

Edit 2: I love the feel of these brakes- I couldn't even have imagined brakes this refined prior to now. Originally, with wheels locking up, that sucked- always wished for better FOC brakes. The first iteration solved the main issue- no more locking, but it left an aesthetic hiccup- stutter. Now, the aesthetics are just straight plush.  If I can try to describe it, coming to a stop feels like a strong braking force (obviously?), with the force curved just right to where it feels like you are landing into a thick down pillow, and the landing is a full stop, no jarring, just comfort. I can't think of a better way to describe it.
```

---
## \#96 Posted by: Bjork3n Posted at: 2019-01-30T08:00:18.644Z Reads: 112

```
That's great! Good news! 
Maybe @Ackmaniac should release a 3.103 update with the fix applied 😇🤞
```

---
## \#97 Posted by: Ackmaniac Posted at: 2019-01-30T10:24:44.100Z Reads: 111

```
I will give it a try. Sounds interesting.
```

---
## \#98 Posted by: Ackmaniac Posted at: 2019-01-30T11:58:47.696Z Reads: 111

```
I just gave it a try and my motors have a short rattle in the transition from controlled brake force to shorting the fets. I guess that depends on the motor your using. But i don't know if that rattle is really healthy.
```

---
## \#99 Posted by: skatardude10 Posted at: 2019-01-30T15:57:47.216Z Reads: 111

```
You tried Jeff's latest code fix? There was stuttering / rattle for me previously with the first iteration, but it's gone for me now. 

If you are using the latest code, interesting... Do you have a video or audio so we can see what you are experiencing?
```

---
## \#100 Posted by: Ackmaniac Posted at: 2019-01-30T16:58:53.434Z Reads: 112

```
Just try it with different brake threngths. When you brake hard by the remote it is fine and when you brake gently it sometimes rattles. But I think I solved it already but need more time for testing.
```

---
## \#101 Posted by: skatardude10 Posted at: 2019-01-30T18:14:45.652Z Reads: 112

```
Nice
10char
```

---
## \#102 Posted by: DAddYE Posted at: 2019-01-30T23:50:40.849Z Reads: 115

```
@Ackmaniac and @Deodand I've made a PR for Vedder:

https://github.com/vedderb/bldc/pull/69

and he said:

> Looks like a sensible fix, thanks! I will give it a try and see how it performs on different setups. The only thing I don't like about the code is the use of fmax and casting to double in performance-critical code. The FPU in the cortex m4 is 32 bits only, so double precision operations are handled in software, making them up to 50 times (!) slower than single precision operations. In general, when using functions from math.h, you should use the versions ending with an f (e.g. sinf, fabsf, cosf, powf). In this case that would be fmaxf instead of fmax, and omitting the double. This is the reason I switched on the double promotion warning.
```

---
## \#103 Posted by: Deodand Posted at: 2019-01-31T00:37:26.526Z Reads: 113

```
Yeah seems reasonable. Hadn't spent any time optimizing I'll make that switch.
```

---
## \#104 Posted by: linsus Posted at: 2019-02-01T12:22:19.767Z Reads: 114

```
I forwarded this thread to him about 3 weeks ago as well :slight_smile:
```

---
## \#105 Posted by: SkaterBoy58 Posted at: 2019-02-03T23:18:48.474Z Reads: 113

```
Anyone tried this updated FW on Vesc 6 yet?
```

---
## \#106 Posted by: DAddYE Posted at: 2019-02-04T01:36:58.390Z Reads: 115

```
I believe that part of the code is common to all versions
```

---
## \#107 Posted by: SkaterBoy58 Posted at: 2019-02-04T01:54:40.994Z Reads: 113

```
Thanks -Will give it a try on Flipsky dual 6 tonight.
```

---
## \#108 Posted by: SkaterBoy58 Posted at: 2019-02-04T23:28:38.441Z Reads: 114

```
Tried to update firmware  on dual 6 Flipsky - when new firmware loaded , the red light comes on and it throws a DRV fault

So went back to old firmware

Cheers
```

---
## \#109 Posted by: DAddYE Posted at: 2019-02-05T02:06:49.675Z Reads: 113

```
Weird! Did you use my firmware or compiled yourself? Did you use the _no_hw_limits?
```

---
## \#110 Posted by: skatardude10 Posted at: 2019-02-05T07:26:50.849Z Reads: 114

```
Did you just go back to standard latest vedder firmware?
```

---
## \#111 Posted by: SkaterBoy58 Posted at: 2019-02-05T22:05:10.638Z Reads: 107

```
used your FW but the default
tried the no limits version last night and no faults!
havent tried the stopping yet
```

---
## \#112 Posted by: SkaterBoy58 Posted at: 2019-02-05T22:05:32.666Z Reads: 105

```
yeah from the tool
```

---
## \#113 Posted by: DAddYE Posted at: 2019-02-06T01:05:33.648Z Reads: 102

```
Awe! Glad it loaded. Let’s us know how it works!
```

---
## \#114 Posted by: SkaterBoy58 Posted at: 2019-02-08T12:36:05.591Z Reads: 104

```
tried it out on a ride today on  flipsky dual 6

All good with the 3km/hr max brakes effect totally gone

Still a bit of brake slight increase just before dead stopped-but maybe that is intentional.

Thanks a lot @DAddYE for FW update

Cheers from Australia
```

---
## \#115 Posted by: Bjork3n Posted at: 2019-02-08T12:56:49.614Z Reads: 102

```
Were you able to solve it?
```

---
## \#116 Posted by: Ackmaniac Posted at: 2019-02-08T15:09:51.322Z Reads: 104

```
Yes, by a adding a hysteresis to the software. But i can't really feel a big difference in the transition between normal braking and a full brake compared to the old version of the software. Think it depends a lot on the motors and gearing that you use. Need to do bit more testing when i find the time. Maybe the unity behaves different when it comes to the transition.
```

---
## \#117 Posted by: Pedrodemio Posted at: 2019-02-08T15:16:19.880Z Reads: 104

```
Exactly that, if the torque your motors can produce when shorting the phases in final braking is not enought you will not feel it, or if your gearing is too tall even with large motor it may not be noticeable
```

---
## \#118 Posted by: DAddYE Posted at: 2019-02-11T19:17:02.696Z Reads: 104

```
For all the folks that have still some cogging while stop, Vedder did an update to the code:

```c
static bool was_full_brake = false;
if (m_control_mode == CONTROL_MODE_CURRENT_BRAKE &&
		fabsf(duty_filtered) < m_conf->l_min_duty * 1.5 &&
		(m_motor_state.i_abs * (was_full_brake ? 1.0 : 1.5)) < fabsf(m_iq_set)) {
	control_duty = true;
	duty_set = 0.0;
	was_full_brake = true;
} else {
	was_full_brake = false;
}
```

I'll try to update my branch asap so everyone can test it.
```

---
## \#119 Posted by: DAddYE Posted at: 2019-02-11T23:10:27.646Z Reads: 104

```
Hi,

if anyone is interested I've compiled the binaries:

https://github.com/DAddYE/bldc/tree/fix_stop/build_all

Rember  to use the [60/default_hw_no_limits](https://github.com/DAddYE/bldc/blob/fix_stop/build_all/60/VESC_default_no_hw_limits.bin) for Flipsky vesc 6
```

---
## \#120 Posted by: Deodand Posted at: 2019-02-12T01:45:06.864Z Reads: 105

```
Let me know how these changes compare, I'll integrate this into the unity too if it feels smooth.
```

---
## \#121 Posted by: Bjork3n Posted at: 2019-02-12T10:28:05.555Z Reads: 102

```
Interesting! So it's solved now? Full speed to full standstill and no cogging or locked brakes? 😃👏
```

---
## \#122 Posted by: Deodand Posted at: 2019-02-14T01:44:35.415Z Reads: 102

```
FYI, I just tested this code and the results were not great. Just a sample size of one so doesn't mean too much but I'm guessing Vedder must be work in progress on this as I get some weird stuttering from this.
```

---
## \#123 Posted by: DAddYE Posted at: 2019-02-14T02:49:43.331Z Reads: 103

```
Thanks for the feedback. Unfortunately SF weather hasn’t been nice lately so I didn’t get a chance to try it :’(
```

---
## \#124 Posted by: Eboosted Posted at: 2019-02-26T00:34:22.335Z Reads: 101

```
@deodand can you specify what was the problem with the fix you compiled?

@skatardude10 you said it works great, but according to @Deodand the results were not great, can you elaborate?

BTW when you download the code from github it downloads a lot of files, I wonder if I should only download this file:

VESC_default_no_hw_limits.bin or
VESC_default.bin

and flash it with @ackmaniac ESC tool?
```

---
## \#125 Posted by: Eboosted Posted at: 2019-02-26T01:15:49.129Z Reads: 102

```
[quote="DAddYE, post:15, topic:73547, full:true"]
I was able to solve this locking issue with my 105mm wheels by reducing the deadband from 15% to 2%. I’ve the mini remote. Give a shoot.
[/quote]

I tried this fix but I still felt the brakes locking, maybe a tad less, however I had issues with the remote giving some throttle when the trigger was in dead center position, so at the end the trouble was bigger than the fix, I went back to 15% of dead band.
```

---
## \#126 Posted by: skatardude10 Posted at: 2019-02-26T01:21:22.929Z Reads: 104

```
Hey man, 

The first iteration of Jeff's fix had some stuttering at the end. The latest version of the fix has no stuttering for me anymore.

I've modified Acks firmware (3.102) to include Jeff's latest fix. If you want that, it can be flashed with Acks ESC tool, just select custom firmware and download your HW version from my git or recompile from source on your own. 

https://github.com/skatardude10/bldc/tree/master/build_all

Changes to 3.102 listed here if you are interested 

https://github.com/skatardude10/bldc/commit/010b7ea4e0e7424e313f9b3373eeefdf78820717
```

---
## \#127 Posted by: Eboosted Posted at: 2019-02-26T01:25:08.821Z Reads: 95

```
Thanks man, I'm downloading at the moment.

What vesion would you suggest?, VESC_default.bin or VESC_default_no_hw_limits.bin for a regular 4.12 Focbox?

![image|690x262](upload://AsGx7pSFs7GovdTrwwPvfWZU9fl.png)
```

---
## \#128 Posted by: skatardude10 Posted at: 2019-02-26T01:33:23.843Z Reads: 94

```
I go 410 411 412.  Default.bin for my focboxes
```

---
## \#129 Posted by: lrdesigns Posted at: 2019-02-26T01:36:48.529Z Reads: 99

```
[quote="Eboosted, post:127, topic:73547"]
VESC_default_no_hw_limits.bin
[/quote]

This version is only if you want to push any settings higher then the max limit set in the standard firmware. For most people its not needed, unless your setup is unusual or you have HUGE power. The standard version has limits on the settings so it is not easy to blow stuff up with a wrong setting while "no hw limits", has no such limits.

For example you wanted to set your motor current to 250 amps, you can only do that in "no hw limits" version.
```

---
## \#130 Posted by: skatardude10 Posted at: 2019-02-26T01:41:36.644Z Reads: 100

```
I think the FSESC 6.6 needed no_hw_limits in order to function for some reason, note for others trying on that.
```

---
## \#131 Posted by: chrischo1996 Posted at: 2019-02-26T01:51:54.944Z Reads: 98

```
I'm having these similar issues of wheels on my FSESC Dual 6.6 running BLDC with large 6 inch wheels. Anyone else have these issues?
```

---
## \#132 Posted by: thisguyhere Posted at: 2019-03-20T21:03:59.903Z Reads: 92

```
ok please don't yell at me but is this where i get the latest unity firmware?

https://github.com/DAddYE/bldc/tree/fix_stop/build_all/60

and do i use this file?

![image|466x468](upload://9jKyxlAAXfFfEfRmaXozHxBFnQ3.png)

@DAddYE 
@Deodand
```

---
## \#133 Posted by: Blasto Posted at: 2019-03-20T23:01:16.247Z Reads: 88

```
No. Enertion’s git hub, only place for the Unity fw

https://github.com/EnertionBoards/FOCBOX_UI?files=1
```

---
## \#134 Posted by: DAddYE Posted at: 2019-03-20T23:08:21.148Z Reads: 88

```
Mine is for stock Vesc (Focboxes,Flisky etc)

For unity the FW, was posted by @Deodand
```

---
## \#135 Posted by: thisguyhere Posted at: 2019-03-20T23:15:42.401Z Reads: 87

```
where though?

isn't the firmware a *.bin file?

i see no bin file in either repos.

does it require a build or something?
```

---
## \#136 Posted by: Blasto Posted at: 2019-03-20T23:20:54.151Z Reads: 87

```
It’s built-in the focboxUi tool.

Or

You get it here

https://github.com/EnertionBoards/FOCBOX_UI/tree/FOCBOX_UI/res/firmwares/UNITY
```

---
## \#137 Posted by: thisguyhere Posted at: 2019-03-21T00:08:51.172Z Reads: 86

```
I see, so does the UI supply all the incremental changes @Deodand has comitted in this thread?

If so, good to know I'm on the latest then. 

Thanks!
```

---
## \#138 Posted by: Deodand Posted at: 2019-03-21T04:52:08.136Z Reads: 86

```
No sorry those changes aren't going to be pushed until I've tested them further.
```

---
## \#139 Posted by: ervinelin Posted at: 2019-03-21T05:53:09.812Z Reads: 85

```
By the way this issue has been resolved for me after upgrading to the latest official VESC firmware (dual Focboxes spinning 8" wheels).

Previously I would get thrown off just before the board comes to a stop. After the firmware upgrade I can crawl along without having to worry about my wheels locking up anymore.
```

---
## \#140 Posted by: thisguyhere Posted at: 2019-03-21T06:34:18.216Z Reads: 86

```
which firmware?  like, which version and where did you source it?
```

---
## \#141 Posted by: ervinelin Posted at: 2019-03-21T06:44:46.000Z Reads: 86

```
https://vesc-project.com/vesc_tool here
```

---
## \#142 Posted by: thisguyhere Posted at: 2019-03-21T07:00:45.644Z Reads: 85

```
so the firmware that comes baked into the latest vesc tool, right?  if so, sweet.
```

---
## \#143 Posted by: ervinelin Posted at: 2019-03-21T07:29:04.767Z Reads: 85

```
Yeah download the latest tool, update your ESC firmware from there. I think it's version 1.07 now... There's some oddity happening with the new wizards so some fiddling might be required...
```

---
## \#144 Posted by: trampa Posted at: 2019-03-23T12:04:40.929Z Reads: 84

```
1.07 is the latest, but will soon be replaced again. Benjamin Vedder is producing quite some code at the moment, since things blocking him are now a matter of the past.
```

---
## \#145 Posted by: visnu777 Posted at: 2019-03-23T12:09:00.243Z Reads: 84

```
Why is it I always think about you and Benjamin as Lord Vetinari and Leonard of Quirm? :smiley:
```

---
## \#146 Posted by: trampa Posted at: 2019-03-23T12:37:17.586Z Reads: 83

```
Because we ask ourselves questions like: Could a VESC be used as a SWD programmer, flashing a second VESC or other device via a SWD to SWD link cable.
```

---
## \#147 Posted by: Silverline Posted at: 2019-03-23T18:33:22.982Z Reads: 81

```
When do you invite Benjamin, to this secret forum ?
```

---
## \#148 Posted by: trampa Posted at: 2019-03-23T18:36:22.648Z Reads: 82

```
It's not a secret to him. He focuses on technical issues and the vesc-project.com froum is the place for that.
```

---
## \#149 Posted by: Silverline Posted at: 2019-03-23T18:45:56.064Z Reads: 80

```
But all the actual vesc users is in here.... We are talking about BV, like he is not among us anymore
```

---
## \#150 Posted by: banjaxxed Posted at: 2019-03-24T00:21:50.390Z Reads: 79

```
VESC is used in many applications besides esk8
```

---
## \#151 Posted by: yousefnjr Posted at: 2019-04-04T14:22:25.922Z Reads: 77

```
Took my first DIY build out on its maiden voyage yesterday and almost ate it while braking :sweat_smile: thanks for finding a fix, hopefully it releases soon! 

Strictly buttboarding til then because I’m a b**** lol
```

---
## \#152 Posted by: Eboosted Posted at: 2019-04-14T17:28:55.846Z Reads: 68

```
Is there a fix for brakes locking at low speeds on regular dual FocBoxes yet?
```

---
## \#153 Posted by: PatRocks Posted at: 2019-04-16T01:06:23.314Z Reads: 66

```
Vesc tool 1-1.08 has it "fixed" (very slight cogging before full stop)
```

---
## \#154 Posted by: Eboosted Posted at: 2019-04-16T01:13:41.627Z Reads: 67

```
Is this version compatible with v4.12 VESCs variants like Focboxes?
```

---
## \#155 Posted by: PatRocks Posted at: 2019-04-16T01:15:04.945Z Reads: 68

```
Yes, I'm running v1.08 firmware on my dual focbox currently! Working great for me!
```

---
## \#156 Posted by: skatardude10 Posted at: 2019-04-16T01:24:47.058Z Reads: 67

```
If you want ackmaniacs FW 3.102 I've got it compiled with Jeff's second iteration of the fix on my GitHub, I get no cogging, focbox.

https://github.com/skatardude10/bldc/commits/master
```

---
## \#157 Posted by: pookybear Posted at: 2019-04-16T01:33:33.063Z Reads: 67

```
I see vesc6 on your github. Can I safely assume that you have also merged this on vesc6.0? 

TIA
```

---
## \#158 Posted by: skatardude10 Posted at: 2019-04-16T01:37:09.062Z Reads: 65

```
I just hit compile and it successfully compiled all versions by default. I haven't tried other than focbox with these bins, but I see no reason why it shouldn't work if you run ackmaniacs FW just fine right now, only change is the brake fix in mcpwm_foc.c
```

---
## \#159 Posted by: pookybear Posted at: 2019-04-16T01:38:29.652Z Reads: 62

```
Yes, I'm currently running ack 3.102. I'll try them when I get a chance. Thanks!
```

---
## \#160 Posted by: ervinelin Posted at: 2019-04-16T02:39:51.907Z Reads: 64

```
I am running 1.08 now, it's MUCH MUCH better than before on dual focboxes... At least I don't get ridiculously thrown off my board when I come to a stop at a traffic junction...
```

---
## \#161 Posted by: yousefnjr Posted at: 2019-04-16T03:35:48.482Z Reads: 63

```
I take it this doesn’t work on Unity? :grimacing:
```

---
## \#162 Posted by: skatardude10 Posted at: 2019-04-16T04:04:02.016Z Reads: 61

```
This fix started on the unity. The firmwares for standard vescs may brick your unity, look for the unity version from @Deodand/Jeffery
```

---
## \#163 Posted by: pookybear Posted at: 2019-05-10T06:34:00.453Z Reads: 50

```
Forgot to update you.

Yes, it works on Vesc 6. I have been using it for weeks now. Thanks!
```

---
