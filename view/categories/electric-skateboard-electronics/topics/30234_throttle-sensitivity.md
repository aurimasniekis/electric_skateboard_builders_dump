# Throttle sensitivity

### Replies: 38 Views: 2557

## \#1 Posted by: Russell23 Posted at: 2017-08-10T10:32:35.425Z Reads: 244

```
Can someone help me out in here, im having a problem with the sensitivity of the throttle on my gt2b
when i put the the pmm control mode on current no reverse with brake, the throttle is so sensitive,light trigger will make the motor reach its full rpm
https://www.youtube.com/watch?v=w6STi35EYso&feature=youtu.be
i tried fixing this by trimiming the throttle and adjusting the minimum and maximum pulsewidth but it didnt work and the throttle is still very sensitive.

The only way for me to not have a sensitive throttle is to put the control mode on duty cycle. the throttle sensitivity duty cycle is normal but its unridable and dangerous as brake is neutral so when you go full speed you wont be able to ease  into braking and it will throw you off your board and risk injury.
https://www.youtube.com/watch?v=FZIJ3o47gf0&feature=youtu.be
I tried using a different remote but its glitching out and sending random commands to the motor making it move without me triggering it. i tried rebinding both of these controllers and they still do the same exact thing.
https://www.youtube.com/watch?v=_AEKIPMNdT0&feature=youtu.be
```

---
## \#2 Posted by: Vieo Posted at: 2017-08-10T10:41:26.865Z Reads: 216

```
I has this issue, but it was because I was free-wheeling it. When I put a load (body weight) on it and it worked correctly
```

---
## \#3 Posted by: Russell23 Posted at: 2017-08-10T10:53:03.585Z Reads: 213

```
unfortunately for me ,even when i put my body weight on it , the throttle is still sensitive
```

---
## \#4 Posted by: krloz Posted at: 2017-08-10T11:12:48.014Z Reads: 210

```
Try lowering start-up boost and min current in the misc tab
Or use ackmaniacs modes firmware with the throttle curve
```

---
## \#5 Posted by: Jinra Posted at: 2017-08-10T15:30:27.944Z Reads: 202

```
This is how the current control mode works. You cannot gauge sensitivity unless you put a load on it. However, since you said it's still too sensitive when you're on the board, either lower motor max in bldc tool, increase the dead band in PPM, or (most recommended) use Ackmaniac's extended BLDC tool and F/W as @krloz mentioned to customize your throttle curve.
```

---
## \#6 Posted by: Russell23 Posted at: 2017-08-10T20:56:21.518Z Reads: 175

```
I already tried increasing the deadband,it didn't help  the throttle is still very sensitive.  I've got a maytech vesc so I can't use the ackmaniac mod bldc tool.
```

---
## \#7 Posted by: Jinra Posted at: 2017-08-10T21:07:11.266Z Reads: 160

```
Sensitive as in too much torque in the beginning?
```

---
## \#8 Posted by: Russell23 Posted at: 2017-08-10T22:22:22.649Z Reads: 148

```
no actually the start up is smooth but after seconds after the start up you get a sudden boost thats even when i barely hit the trigger  @Jinra
```

---
## \#9 Posted by: Russell23 Posted at: 2017-08-10T22:42:13.867Z Reads: 141

```
@krloz
 my startup boost and my min current is pretty low already
<img src="/uploads/db1493/original/3X/7/a/7a1ca67bd888b27a25b302636714c5dd18dabaa1.png" width="690" height="387">
```

---
## \#10 Posted by: Russell23 Posted at: 2017-08-10T22:45:24.878Z Reads: 133

```
according to my pulsewidth display, my neutral is 58% and when the motor starts spinning is at 65% and when it reaches its full rpm is at 68/69%. so i have 3/4% of the throttle to work with
```

---
## \#11 Posted by: Jinra Posted at: 2017-08-10T22:49:35.728Z Reads: 129

```
You have to understand how current control works. Your VESC in current control mode will always try to ramp up to full duty cycle (95%). The throttle controls the max current applied to the motor, and if that current overcomes the load on the drive train, it'll ramp to 95% duty cycle. The throttle controls the strength of accleration, not speed. Holding it even 10% will cause it to slowly ramp to higher speeds until the given current can no longer overcome load.

The G2TB has a throttle trim that you can adjust so you're as close to 50% as possible, try adjusting that so the deadband is accurate.
```

---
## \#12 Posted by: Russell23 Posted at: 2017-08-10T22:55:08.078Z Reads: 123

```
i did adjust it to 50% but its useless, the motor wont move until i reach 65% and it reaches its full rpm once i hit 68% . changinbg ut to 50% doesnt change the sensitivity @Jinra
```

---
## \#13 Posted by: Jinra Posted at: 2017-08-10T22:58:04.893Z Reads: 120

```
What's your current deadband?
```

---
## \#14 Posted by: Russell23 Posted at: 2017-08-10T23:01:55.708Z Reads: 120

```
<img src="/uploads/db1493/original/3X/6/9/69c3d94b118ccb83389c6c7c6e50238d421ca422.png" width="690" height="387">
```

---
## \#15 Posted by: Jinra Posted at: 2017-08-10T23:04:33.062Z Reads: 118

```
Yea it's taking a lot to move it because the deadband is so high. Trim the throttle or adjust the PPM to get 50% neutral. Leave deadband at .1 or .15. You'll have to get used to using the remote to control **acceleration** and not **speed**
```

---
## \#16 Posted by: Russell23 Posted at: 2017-08-10T23:07:45.539Z Reads: 112

```
i mean it was taking a lot to move when i had it on 50%, ive got my neutral on 58% which is closer to 65% @jinra
```

---
## \#17 Posted by: pshaw Posted at: 2017-08-10T23:33:00.396Z Reads: 111

```
[quote="Jinra, post:15, topic:30234, full:true"]
Yea it's taking a lot to move it because the deadband is so high. Trim the throttle or adjust the PPM to get 50% neutral. Leave deadband at .1 or .15. You'll have to get used to using the remote to control **acceleration** and not **speed**
[/quote]

is there a way to control speed instead of acceleration (might have to be outside of ack firmware) ?
```

---
## \#18 Posted by: Jinra Posted at: 2017-08-10T23:35:20.242Z Reads: 106

```
PID speed control or duty cycle. The problem with these modes is if you go to neutral it'll brake to reduce the speed since the throttle is going back. Trust me, once you get used to current/watt control, you'll find it just as good as speed control if not better.
```

---
## \#19 Posted by: Russell23 Posted at: 2017-08-10T23:39:01.119Z Reads: 106

```
duty cycle is dangerous because brake is neutral and when your going 25mph, you wont be able to ease in to the brake and it will throw you off the board and you risk injury
```

---
## \#20 Posted by: Jinra Posted at: 2017-08-10T23:45:41.316Z Reads: 102

```
Yep that's why you should use current/watt control with the vesc for esk8
```

---
## \#21 Posted by: pshaw Posted at: 2017-08-11T00:44:10.618Z Reads: 94

```
[quote="Jinra, post:18, topic:30234, full:true"]
PID speed control or duty cycle. The problem with these modes is if you go to neutral it'll brake to reduce the speed since the throttle is going back. Trust me, once you get used to current/watt control, you'll find it just as good as speed control if not better.
[/quote]

Ah I gotcha. Wonder how boosted pulls it off then... don't think it works that way but is still speed control not accel.
```

---
## \#22 Posted by: Jinra Posted at: 2017-08-11T00:53:51.205Z Reads: 92

```
Yea them and evolve have custom fw's and escs for speed based control
```

---
## \#23 Posted by: racidon Posted at: 2017-08-11T01:14:50.672Z Reads: 93

```
Another option you can try is putting your controller in "reverse" so that moving the throttle forward is acceleration. It has more movement so it's easier to adjust to what you want. It takes a little getting used to using it in reverse but it's my preferred method now.
```

---
## \#24 Posted by: Titoxd10001 Posted at: 2017-08-11T01:25:27.903Z Reads: 88

```
I feel your pain. What you're looking for is Duty Cycle  which every other esc uses. Unfortunately due to bldc firmware it's not usable on vesc. Only hope is that Vesc-tool comes with usable Duty Cycle which is what I'm waiting for. Could be available this week or next year who knows.
```

---
## \#25 Posted by: pshaw Posted at: 2017-08-11T02:25:20.567Z Reads: 87

```
Weird. How the hell isnt this available yet? Cost, hardware limitations only companies with deep pockets can afford? 

It strange just getting into this hobby how much in it's infancy it is. I fly drones and it's amazing how complex and quickly that tech moves. 

Is eskate just too small of a market?
```

---
## \#26 Posted by: Russell23 Posted at: 2017-08-11T02:34:53.265Z Reads: 84

```
i guess i have to stick to what ive got right now and wait for the new vesc tool for vesc 6.0 which is compatible  with 4.12 vesc  and especially maytech vesc with no bootloader. or i can buy a new vesc which will cost a lot
```

---
## \#27 Posted by: Titoxd10001 Posted at: 2017-08-11T02:36:31.099Z Reads: 82

```
The only thing needed is firmware upgrade. Some people don't like Duty Cycle and don't mind watt/current mode. Don't know what they're missing out on. Only person that can make changes is Benjamin the creator of vesc.
```

---
## \#28 Posted by: pshaw Posted at: 2017-08-11T02:57:37.204Z Reads: 82

```
Wow only one person can make firmware changes?!? What about ackmaniac ?
```

---
## \#29 Posted by: Jinra Posted at: 2017-08-11T03:00:46.764Z Reads: 83

```
I've tried the duty cycle control mode of the Carbon GT, but I much prefer the current control mode of the VESC.
```

---
## \#30 Posted by: Titoxd10001 Posted at: 2017-08-11T03:56:59.618Z Reads: 83

```
I know its not for everyone. I tried a evolve and it was a bit touchy. The throw of the remote is small. With something like a gt2b it would be better imo from trying duty cycle on vesc. Duty cycle has sense of more power at low rpm at low speeds but is still controllable at high speeds. If you increase power/watts in the settings in watt mode it has even less throttle range. So if you put 6000watts for a 4wd I wonder how much throttle range you'd have. If you did the same 6000watts on Duty cycle in theory you'd still have to press full throttle for full speed.
```

---
## \#31 Posted by: krloz Posted at: 2017-08-11T07:34:21.582Z Reads: 80

```
What do you mean by

[quote="Titoxd10001, post:27, topic:30234"]
Only person that can make changes is Benjamin the creator of vesc.
[/quote]
```

---
## \#32 Posted by: krloz Posted at: 2017-08-11T07:35:56.752Z Reads: 76

```
You can install the boot loader and change the firmware in a maytech. Search for st-link in the forum
```

---
## \#33 Posted by: Titoxd10001 Posted at: 2017-08-11T07:45:40.760Z Reads: 77

```
Vedder will probably release updated Duty Cycle with his new firmware. If he doesn't, there are few people able or willing
```

---
## \#34 Posted by: krloz Posted at: 2017-08-11T08:08:03.937Z Reads: 79

```
That is true.  But somebody did get to make a new control method. Sorry for insisting but @Ackmaniac 's firmware  is so cool I just can't stop advertising it

https://www.electric-skateboard.builders/t/extended-bldc-tool-with-watt-control-mode-ppm-cruise-control-individual-throttle-curve-and-android-app/12286/1394
```

---
## \#35 Posted by: pshaw Posted at: 2017-08-11T12:12:20.056Z Reads: 82

```
I certainly hope so!
```

---
## \#36 Posted by: pshaw Posted at: 2017-08-30T02:45:31.543Z Reads: 70

```
anyone heard if a new improved duty cycle control mode is coming out anytime soon?
```

---
## \#37 Posted by: Titoxd10001 Posted at: 2017-09-18T05:27:29.573Z Reads: 65

```
Looks like Duty Cycle (with neutral) might not happen after all. I tried to convince vedder but he's either not interested or hardware limitation, not sure. Someone said it worked for them maybe on vesc-6. Post comment on vedder forum to let him know we want duty cycle and maybe he'll take a look.
```

---
## \#38 Posted by: pshaw Posted at: 2017-09-25T01:34:59.803Z Reads: 55

```
Lame 10char
```

---
