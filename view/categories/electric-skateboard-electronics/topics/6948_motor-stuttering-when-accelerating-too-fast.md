# Motor stuttering when accelerating too fast

### Replies: 50 Views: 4214

## \#1 Posted by: Jinra Posted at: 2016-08-01T16:41:10.653Z Reads: 322

```
Hey all,

I got my Honey Driver build finished recently but am having an issue with the motor stuttering when I go full throttle from standstill or if I otherwise accelerate too quickly. Any help on this would be appreciated! Details below..

##Video##
https://goo.gl/photos/sszh3BA5Lzcqv4wK7

##Settings##
<img src="/uploads/db1493/original/2X/9/934f94bf4dde63845fc645ddbf8ae4baf94b4597.png" width="690" height="386">
<img src="/uploads/db1493/original/2X/1/17813d76ae0161dc3b24029dd53662f5dfc3e1f2.png" width="690" height="386">
<img src="/uploads/db1493/original/2X/d/dc867d3af6d992011dca7ebe8ccd0ac957b0e535.png" width="690" height="386">

##Notes##
* Using PPM with min/max pulsewidth custom set to for the remote.
* Multiple ESCs over CAN set for both VESCs
* Dual diag configuration
* Slave (front) VESC has "send status over can" enabled
* I'm 79kg
* This doesn't happen when accelerating slowly then speeding up, so I think it has something to do with the sensors.
* Tried upping the sensorless eRPM from 2000 to 6000.
* Tried lowering the sensorless eRPM from 2000 to 1500 (as shown in pic)
```

---
## \#2 Posted by: elkick Posted at: 2016-08-01T17:47:01.612Z Reads: 290

```
[quote="Jinra, post:1, topic:6948"]
Multiple ESCs over CAN set for both VESCs
[/quote]

That's not a good idea, it should be enabled on the master only and not on the slave. 

Also, it might be better to set  the "max. current ramp step" to the default of 0.0400.
```

---
## \#3 Posted by: Jinra Posted at: 2016-08-01T18:36:18.299Z Reads: 279

```
Sorry that picture was before I wrote config. It changed to .04 after I wrote.

Also, if I dont turn on multiple ESCs on the slave, wouldn't it not have traction control? That's the main reason I turned it on.
```

---
## \#4 Posted by: chaka Posted at: 2016-08-01T18:45:25.607Z Reads: 275

```
@Jinra Try lowering your motor and battery amps. You might be tickling the over current cuttoff on your BMS.
```

---
## \#5 Posted by: Jinra Posted at: 2016-08-01T18:47:05.518Z Reads: 270

```
I think the BMS should be able to handle burst current. I'm not confident this is the issue since the board never cuts out, just stutters on dead stop hard acceleration. Note in the video I release throttle just to show the issue; if I held the throttle it would eventually get up to speed and travel smoothly.
```

---
## \#6 Posted by: chaka Posted at: 2016-08-01T18:49:45.522Z Reads: 263

```
Is the problem only occurring when you stuff the throttle? Does it behave when you gradually apply the throttle?

FYI, I can trip the over-current on a bms with 100 amp capability with the setting you currently have. I am pretty sure the bms you have is not capable of 100 amps.
```

---
## \#7 Posted by: Jinra Posted at: 2016-08-01T18:50:51.296Z Reads: 248

```
It happens when I full throttle, or otherwise accelerate too fast from stand still. If I ramp up more gradually, it works perfectly.
```

---
## \#8 Posted by: chaka Posted at: 2016-08-01T18:59:13.964Z Reads: 247

```
Also, try lowering your low voltage start to 33v. You could be triggering the back off strategy when you apply heavy throttling.
```

---
## \#9 Posted by: Jinra Posted at: 2016-08-01T19:00:25.182Z Reads: 245

```
I can try that as well. I've been testing this from full charge.
```

---
## \#10 Posted by: chaka Posted at: 2016-08-01T19:06:14.189Z Reads: 251

```
This is one of the main reasons I use 60+ cells in my builds. You really only want to pull a maximum of 10 amps from those cells regardless of their 20 amp rating.  Try lowering your settings to 20 amp battery and 30 amp motor max. Personally I think that is still to high for a 40 cell pack but it should work with fresh cells.

 Ideally we would only pull a maximum of 5 amps per cell but that requires a very large pack.
```

---
## \#11 Posted by: Jinra Posted at: 2016-08-01T19:25:45.662Z Reads: 245

```
Here's what vedder said about the option. I noticed he mentioned that send status should be on slave, but made no mention on how"multiple escs over can"should be configured. I was assuming it's okay to have it on all VESCs.

> Multiple ESCs over CAN can be enabled to connect several VESCs over CAN bus. All VESCs must have different Controller ID and the slave VESCs must have Send status over CAN enabled
```

---
## \#12 Posted by: Jinra Posted at: 2016-08-01T19:35:04.015Z Reads: 242

```
Thanks for the recommendation @chaka. I'll take note of those settings. However, I do go up pretty steep hills with no problems. I have a hunch that this is a sensor issue, but haven't tried running the setup in sensorless yet.
```

---
## \#13 Posted by: elkick Posted at: 2016-08-01T19:38:51.348Z Reads: 241

```
[quote="Jinra, post:3, topic:6948"]
Also, if I dont turn on multiple ESCs on the slave, wouldn't it not have traction control? That's the main reason I turned it on.
[/quote]

The slave always takes the commands from the master and traction control will work. So, if it's enabled at the master that's ok. But it should definitely not be enabled on the slave.
```

---
## \#14 Posted by: Jinra Posted at: 2016-08-01T19:39:46.546Z Reads: 234

```
Gotcha, I'll try it out and report back :)
```

---
## \#15 Posted by: Jinra Posted at: 2016-08-03T01:08:03.690Z Reads: 219

```
Update! https://goo.gl/photos/Lyt73DdMZoMXDsVe8
@elkick @chaka
I explained in the video, but the problem seems to be less severe and less likely to throw me off now. It still happens if I crank to full/near full throttle too fast from a dead stop.

Changed settings are as follows:

* min erpm now at 200 from 250
* sensorless erpm now at 2000 from 1500
* motor max now at 40 from 60
* battery max now at 30 from 40
```

---
## \#16 Posted by: chaka Posted at: 2016-08-03T03:02:25.147Z Reads: 211

```
Have you tried running through calibration again?  Integrator limit and bemf coupling measurements seem a little off.
```

---
## \#17 Posted by: Jinra Posted at: 2016-08-03T03:04:38.029Z Reads: 210

```
i calibrated on 6s but haven't done it on 10s since i didn't want to redo my loctite, but I'll give it a shot. What's yours?
```

---
## \#18 Posted by: chaka Posted at: 2016-08-03T03:17:10.484Z Reads: 218

```
I run calibration with the belt on, just make sure the wheel can spin free. My board with 200kv is set , Integrator Limit 130, BEMF Coupling 860. I usually run motor calibration a number of times and take the average measurement.

Honestly I prefer sensorless operation for simplicity. I still would like to find out what is going on with you settings.
```

---
## \#19 Posted by: Jinra Posted at: 2016-08-03T03:24:16.697Z Reads: 215

```
Oh really? I always heard you should run calibration with a free spinning motor. When i did calibration with pulleys, my results were higher i just never set it.
```

---
## \#20 Posted by: chaka Posted at: 2016-08-03T03:54:08.482Z Reads: 212

```
Until you get your settings sorted out I would refrain from applying full throttle from a dead stop. Even after you get it sorted out I would refrain from doing this as it is bad practice on anything with a motor.
```

---
## \#21 Posted by: Jinra Posted at: 2016-08-03T03:57:26.732Z Reads: 209

```
True. I never really go full throttle from dead stop, I was just bothered that it happens.

I just did calibration on both motors (with pulleys and wheels on) and got this.

106/906 on front motor
110/909 on back motor

Seems accurate to what I had before right?
```

---
## \#22 Posted by: chaka Posted at: 2016-08-03T03:59:26.204Z Reads: 201

```
Is it buttery smooth when you ease the throttle from a dead stop, no cogging?
```

---
## \#23 Posted by: Jinra Posted at: 2016-08-03T04:00:04.314Z Reads: 201

```
Yep! (10 chars),

Small  vid:
@chaka
https://goo.gl/photos/fDzBuxcBLY1o3sig6
```

---
## \#24 Posted by: elkick Posted at: 2016-08-03T06:37:13.634Z Reads: 204

```
That's how it shoul be. :slight_smile:
```

---
## \#25 Posted by: Jinra Posted at: 2016-08-03T06:45:38.954Z Reads: 211

```
Thank you both, Im content with how it's currently running. :)
```

---
## \#26 Posted by: onloop Posted at: 2016-08-03T10:26:57.150Z Reads: 217

```

You can adjust the startup boost between 0.01 to 0.1 in steps of 0.01 - I would suggest starting lower than 0.05 and going up past it to see if you find a sweet spot.

That is the only way to fine tune the start torque based on your weight.

Changing the other motor parameters wont do much.

Also; The shuddering effect will be amplified with a diagonal drive system. Dual drive will have less studdering as the truck won't be able to see-saw 

Also; There is a chance your sensors are not working, I would disable the sensor mode and see what happens.
```

---
## \#27 Posted by: Jinra Posted at: 2016-08-03T14:17:55.790Z Reads: 207

```
I don't think the startup boost actually does anything (at .01-.05 duty cycle) in my setup given that it's a sensorless value and my hybrid setup runs sensored until 2000erpm. I changed it from .01 to .05 to see if it would help, but it made 0 difference.

I know one of the chances i made helped the stutter a lot (though it still happens), but i haven't tracked down which change it was. I do suspect that it was losing the motor max. Throttling to 60A per motor from dead stop may have caused it to freak out.
```

---
## \#28 Posted by: onloop Posted at: 2016-08-03T14:32:23.183Z Reads: 202

```
Yeah... to much current in your motor is never really a great idea....

Maybe Need to turn sensor mode off to get start boost working.

It definitely works though.
```

---
## \#29 Posted by: chaka Posted at: 2016-08-03T14:35:34.643Z Reads: 198

```
You could also try adjusting your phase advance. Setting it to 1.0 gives no phase advance and setting it to 0.0 gives 30 degrees (maximum) phase advance.
```

---
## \#30 Posted by: Jinra Posted at: 2016-08-03T14:48:49.321Z Reads: 197

```
oh im sure it does something just probably not on sensored/hybrid :) I love my smooth start from dead stop too much to turn sensors off. I love in SF and it really helps with all the hills since it's hard to kick start upwards.

@chaka Could you explain what phase advance does exactly?
```

---
## \#31 Posted by: chaka Posted at: 2016-08-03T15:11:29.642Z Reads: 185

```
Ok I was able to replicate what you are experiencing. If you want to make the vesc foolproof you will need to lower the ramping, max current ramp step (at 1 khz) to .004     This has given me good results.

Remember the multiplier bug still exists so you will need to input .0004 to get the right setting. This will give the motor enough time to rotate and allow the processor to log position before applying heavy loading. You may lose a little snap on the throttle response. Since you are using the canbus and there is a processor lag the slave may still cog so you may want to split your ppm signal wire and run each VESC independent.

The best solution if you want raw performance is to ease the throttle and only go full throttle when you get at least a partial revolution.
```

---
## \#32 Posted by: Jinra Posted at: 2016-08-03T15:13:38.540Z Reads: 173

```
Thanks chaka! Does the change have to be in a multiple of 10? what if i were to try somewhere in between .04 and .004?
```

---
## \#33 Posted by: chaka Posted at: 2016-08-03T15:21:35.053Z Reads: 164

```
Probably, this seems to be an issue with processor speed. you could also reduce the deadband from 15 to 10 in the ppm menu, be careful if your transmitter strays to far from 50% at dead stick. this should give the processor a little more time.
```

---
## \#34 Posted by: Jinra Posted at: 2016-08-03T15:30:43.465Z Reads: 165

```
it's already at .10 :) I might just leave the settings as they are and not full throttle too fast too often. Thanks again for all your help.
```

---
## \#35 Posted by: chaka Posted at: 2016-08-03T15:34:47.767Z Reads: 171

```
Thank you! Trouble shooting other riders systems is what gives me more experience and a greater understanding of the VESC.
```

---
## \#36 Posted by: Jinra Posted at: 2016-08-06T04:08:09.351Z Reads: 183

```
Hey @chaka,

Did some more testing today and I've completely eliminated the issue. I noticed that the same kind of 'cogging' would happen when I broke very hard (just as how I started hard). I have a strong feeling that it has something to do with me running 'current mode' instead of 'current no reverse with brake'. Here are the changes I've made since.

Motor Max: 45 (I wasn't happy with my acceleration)
Battery Max: 35 (I know you're not a fan of this but I promise I'll keep an eye on my heat :slight_smile:)
Motor Regen (min): 45
Sensorless eRPM: 6000
Max Current Ramp Gain: 0.02 (half of default)
PPM mode: Current no reverse with brake
Startup Boost: 0.01
Integrator Limit: 120 (re-ran detection a couple times and got 120 average)
BEMF Coupling: 850 (got about 860-870 after re-running detection)
Turned off traction control
Added ferrite ring on sensor wires

A separate issue I noticed was that my slave VESC, front motor, would sometimes fail to respond, or have a delayed response, which meant that I would suddenly get a boost to braking/accelerating a second or two after I throttle the respective direction. I had a feeling this may be due to the long sensor wires sitting right next to the motor phase wires. This is why I added a ferrite ring to the sensor wires closer to the slave VESC.
```

---
## \#37 Posted by: Kasper Posted at: 2016-10-08T18:59:18.742Z Reads: 139

```
Hi,

Recently i purchased an Enertion Dual Raptor and i'm having the same problem as Jinra in the beginning. When i want to start riding the board from a dead stop or uphill, it stutters until i give more throttle of if i push it a bit up to speed first. It does the same when i give full throttle immediately. The rest is working perfectly. I followed the steps mentioned in the steps above but nothing worked.. Any advice from anyone?
Thanks! 

Down here you can see my settings.

<img src="/uploads/db1493/original/3X/1/a/1a2688cdf2d30603833b19bd6bb7415fe08d517f.png" width="690" height="388">
```

---
## \#38 Posted by: Jinra Posted at: 2016-10-08T19:11:36.762Z Reads: 126

```
that's actually because you have unsensored motors. you have to kick off first then throttle. it's different than the issue i was having
```

---
## \#39 Posted by: Kasper Posted at: 2016-10-08T19:39:04.805Z Reads: 127

```
[quote="Kasper, post:37, topic:6948"]
When i want to start riding the board from a dead stop or uphill, it stutters until i give more throttle of if i push it a bit up to speed first. It does the same when i give full throttle immediately. The rest is working perfectly.
[/quote]

I see. Well i tried to put into sensor mode but then the motors did not do anything anymore. They simply did not respond to the remote, while the vesc's were receiving the signal.
```

---
## \#40 Posted by: Jinra Posted at: 2016-10-08T20:02:59.465Z Reads: 124

```
The motors are unsensored, they won't work in sensored mode. You have to hit get sensored motors if you want to start from dead stop
```

---
## \#41 Posted by: Kasper Posted at: 2016-10-08T20:05:23.872Z Reads: 118

```
Alright, thanks for the info! So that basically means i always have to push it first a bit and then go, there is no other option with this board?
```

---
## \#42 Posted by: Jinra Posted at: 2016-10-08T20:06:01.176Z Reads: 118

```
yep that's right
```

---
## \#43 Posted by: Kasper Posted at: 2016-10-08T20:07:54.873Z Reads: 118

```
Ok, well there are worse things in the world.. LOL But seriously, thanks for the information, that helped a lot in understanding this board and its capabilities.
```

---
## \#44 Posted by: onloop Posted at: 2016-10-10T08:38:34.474Z Reads: 111

```
You could fine tune the startup boost & motor/battery current settings to match your weight. It might make a slight difference.

Otherwise just take one slight push forward.
```

---
## \#45 Posted by: davey8 Posted at: 2016-10-14T21:31:48.508Z Reads: 92

```
Hey @ Jinra and Chaka,

I'm 200lbs and running 12s3p on 2 R-Spec 6355 motors. Should copying these settings sort out my stuttering start?
```

---
## \#46 Posted by: Jinra Posted at: 2016-10-14T21:46:51.001Z Reads: 90

```
Are your problems exactly the same as mine? If they are, then turning off traction control was the solution.
```

---
## \#47 Posted by: davey8 Posted at: 2016-10-14T22:29:39.746Z Reads: 86

```
Actually... No.  LOL.  Thanks for getting back to me so quickly though. I just took my first build out for it's first test run. It was stuttering on startup in the house, but did much better outside for some reason.  Now I'm wondering how to safely tune for more torque.
```

---
## \#48 Posted by: Jinra Posted at: 2016-10-14T22:55:58.788Z Reads: 84

```
sounds like you have unsensored motors which will stutter if you try to start from a dead stop. You'll need to give it a little kick before you throttle.
```

---
## \#49 Posted by: saul Posted at: 2016-10-15T21:34:55.902Z Reads: 85

```
thats weird, I can start from a stop with a single 6374 uncensored. as long as i'm not rolling backwards...
```

---
## \#50 Posted by: Jinra Posted at: 2016-10-15T22:19:43.845Z Reads: 83

```
it will occasionally cog. This only applies if your accelerating from dead stop.
```

---
