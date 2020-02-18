# Brakes release/cut out

### Replies: 23 Views: 2296

## \#1 Posted by: WARMAN Posted at: 2017-02-14T20:19:44.007Z Reads: 160

```
Searching this forum and can't find a fix for this basically when I brake the brakes release and I have nothing! 
Happens at high and low speed and upon inspection the vesc is flashing pink when this dropout ocurs.
I'm using the mastercho mod for the gt2b and my vesc is v4.12 from diy.com 
I did come across a thread from 7 months ago with people with the same problem @chaka @FLATLINEcustoms did you ever find a fix for this I'm using ppm,current no reverse with brake,bldc
```

---
## \#2 Posted by: LukeL Posted at: 2017-02-14T21:11:39.519Z Reads: 153

```
What's your maximum input voltage set to on the bldc tool?
```

---
## \#3 Posted by: Titoxd10001 Posted at: 2017-02-14T21:22:27.821Z Reads: 147

```
Did you try the gt2b before the mod and did you still have this problem? I had issue when adding enclosure because it allows to much brake trigger movement that the vesc can't register it.
```

---
## \#4 Posted by: JohnnyMeduse Posted at: 2017-02-14T21:25:29.980Z Reads: 140

```
Can you post some picture and bldc tool screen of your setting ?
```

---
## \#5 Posted by: WARMAN Posted at: 2017-02-14T21:38:08.288Z Reads: 129

```
Yeah had a feeling it might be this or the band pulse width will try fix the brake length on the gt2b mod first.
seen someone use a bit of foam,failin that I'll upload my bldc readings tomorrow
```

---
## \#6 Posted by: WARMAN Posted at: 2017-02-14T23:21:43.458Z Reads: 129

```
[quote="Titoxd10001, post:3, topic:17704"]
I had issue when adding enclosure because it allows to much brake trigger movement that the vesc can't register it
[/quote]

@MasterCho had anyone else with this problem does it alow more brake movement in the trigger?
```

---
## \#7 Posted by: Cuprani Posted at: 2017-02-14T23:23:49.580Z Reads: 127

```
I have the same problem.

DIY VESC
Single 190 kv 3150 watt motor
12S1P Lipo (20c) 5000mAh

Here is a log of a recent run
https://metr.at/r/W8Ak0

At 50 - 75% brake, the regenerative current gets to high and as a result it stops braking.
This gives really dangerous situations.
The max braking current is set at -12A, but as you can see above at 7:31:39 PM at about -3A it stops braking as a result of over current.

Here are my settings.

[img]https://sites.google.com/site/nilsvdg2/home/BLCD_Motor.jpg[/img]

[img]https://sites.google.com/site/nilsvdg2/home/BLCD_BLCD.jpg[/img]
(detection of motor was OK)

[img]https://sites.google.com/site/nilsvdg2/home/BLCD_Advanced.jpg[/img]
(did not change anything here)

[img]https://sites.google.com/site/nilsvdg2/home/BLCD_PPM.jpg[/img]
(Receiver gets to 99,9% at ful throttle and 0% at full brake)
```

---
## \#8 Posted by: Ackmaniac Posted at: 2017-02-14T23:59:31.060Z Reads: 115

```
Just use my firmware mod. There you can use the full throttle range of the acceleration and the brake by setting a center position.
```

---
## \#9 Posted by: Titoxd10001 Posted at: 2017-02-15T00:00:48.542Z Reads: 117

```
Here is a pick of gt2b and look how the case limits the brake travel 
<img src="/uploads/db1493/original/3X/2/2/2200fe3da5d68b9ed5541e8778a5654bb69bd1fa.jpg" width="375" height="500">
with a enclosure mod badwolf and madmunkey, idk about others there is nothing stopping it
<img src="/uploads/db1493/original/3X/7/1/713f3db5a87ca15802ece99fb4c4185597b1f8ad.jpg" width="375" height="500">
This is with madmunkey (still need to fix since I just made switch from badwolf). If you change pulsewidth without limiting trigger to like .7 and 1.9 you CANNOT set failsafe properly. when you limit trigger it will be closer to 1 and 2 and you'll be able to set failsafe at exactly 50%. I always assumed it was over voltage but it was not
```

---
## \#10 Posted by: WARMAN Posted at: 2017-02-15T05:22:12.205Z Reads: 108

```
Interesting @Titoxd10001 I will connect a gt2b later see if that eliminates it! Like @Cuprani said it creates some dangerous situations and we all need to find the cause asap.
@Ackmaniac thanks man where can I find your firmware upgrade
```

---
## \#11 Posted by: Titoxd10001 Posted at: 2017-02-15T08:57:49.866Z Reads: 109

```
Your firmware upgrade is on my to-do list, but besides cutting out, having all that extra brake travel is uncomfortable on the trigger finger. Also the cutting out problem happens in car ESCs so it might be beneficial to have a physical stop
```

---
## \#12 Posted by: Ackmaniac Posted at: 2017-02-15T11:50:06.136Z Reads: 106

```
Here you can find my firmware mod

http://www.electric-skateboard.builders/t/extended-bldc-tool-with-watt-control-mode-ppm-cruise-control-individual-throttle-curve-and-android-app/12286

And you could also change the throttle curve for braking to have a full brake already at like 70% brake throttle. And you could fine tune the throttle curve by a Android app to find the sweet spot on the road.
Problem in the firmware is that when the pulsewitdth signal is more then 20% away from the full brake position then the VESC thinks it's a problem with the signal.

e.g.
max pulsewith = 2.00
min pulsewith = 1.00
so theoretical center is 1.5 (in my mod you can adjust the precise center)
when the pulsewith is now at 0.91 it thinks it's already a full brake but excepts it. (18% off)
when the pulsewith is now at 0.79 it thinks it's to far off and something must be wrong. (22% off)
```

---
## \#13 Posted by: Kaly Posted at: 2017-02-15T15:27:00.769Z Reads: 100

```
[quote="Ackmaniac, post:12, topic:17704"]
e.g.max pulsewith = 2.00min pulsewith = 1.00so theoretical center is 1.5 (in my mod you can adjust the precise center)when the pulsewith is now at 0.91 it thinks it's already a full brake but excepts it. (18% off)when the pulsewith is now at 0.79 it thinks it's to far off and something must be wrong. (22% off)
[/quote]

With your firmware this situation  is avoided ?
```

---
## \#14 Posted by: Ackmaniac Posted at: 2017-02-15T17:35:19.247Z Reads: 97

```
Not really. But you can adjust min,  max and center position. So you can use the full throttle range for both directions. And you can adjust the throttle curve to your needs.

And by this the problem doesn't exist in my firmware mod.
```

---
## \#15 Posted by: WARMAN Posted at: 2017-02-15T17:59:48.927Z Reads: 92

```
After browsing through a similar thread about the same topic I found this from @dogeatgod 
<img src="/uploads/db1493/original/3X/0/d/0da294655e1deff1a2a6053f42e56d528e4ae0b8.jpg" width="382" height="500">
seems restricting the brake trigger movement on the moded gt2b and changing pulse width should work! 
Been too busy today to pull the board apart but will try it tomorrow and report back.
```

---
## \#16 Posted by: WARMAN Posted at: 2017-02-18T23:46:50.356Z Reads: 86

```
@Cuprani @Kaly check this out think it's a software bug,also take the poll.
[POLL] Do you have braking loss? Even on BLDC? - General Discussion - Electric Skateboard Builders Forum | Learn How to Build your own E-board
http://www.electric-skateboard.builders/t/poll-do-you-have-braking-loss-even-on-bldc/17571
```

---
## \#17 Posted by: Cuprani Posted at: 2017-02-27T20:03:01.465Z Reads: 78

```
I've filled in the poll.
Tonight I didn't turn off my board for a change (I usually forget to leave it on when the brake error have occured).
I logged the following fault and this was during braking.

The following faults were registered since start:
Fault            : FAULT_CODE_ABS_OVER_CURRENT
Current          : 47.0
Current filtered : 100.9
Voltage          : 49.08
Duty             : 0.00
RPM              : 2248.6
Tacho            : 694719
Cycles running   : 16227
TIM duty         : 263
TIM val samp     : 131
TIM current samp : 26505
TIM top          : 52747
Comm step        : 3
Temperature      : 43.77

Vesc 4.12 with stock 2.18 firmware
36T on 90mm wheel
16T on 190kv motor (3300 watt)
85 kg
```

---
## \#18 Posted by: Blasto Posted at: 2017-02-27T20:16:33.553Z Reads: 73

```
[quote="Cuprani, post:17, topic:17704"]
Current filtered : 100.9
[/quote]

your abs max current may be set a little low, is it at 130A? you're running a 12S setup?
```

---
## \#19 Posted by: Cuprani Posted at: 2017-02-27T20:21:47.917Z Reads: 73

```
Because I had a lot of heat I just lowered it today to 100A. 
I'm running 12S and it was on 130A before.

If this caused the fault I will change it back to 130A
```

---
## \#20 Posted by: Blasto Posted at: 2017-02-27T20:33:40.460Z Reads: 72

```
the abs max current is a safety feature, this is the current where the vesc will shutdown beyond this current threshold. 

For example: one of your windings in your motor shorts out, you will most likely hit this threshold.

If you want to lower your generated heat, you need to lower your batt current.
```

---
## \#21 Posted by: Ackmaniac Posted at: 2017-02-27T20:37:03.093Z Reads: 70

```
Yes this caused the fault.
The VESC detects the actual current and adjusts the duty cycle to this current. By the remote input you tell the VESC which current it should use but is is always a little bit off that value and so the VESC constantly adjusts the duty cycle to reach the correct current.
So the VESC needs some wiggle room between the motor max and the absolute max.
So as Blasto sayed the absolute max is there to protect the VESC from errors. But when you choose it too low then it causes issues.
```

---
## \#22 Posted by: Cuprani Posted at: 2017-02-27T21:06:15.653Z Reads: 69

```
@Blasto
I also changed my motor and battery current from 80A to 65A earlier today.
I now changed the max amps back to 130A.

Also I changed my configuration from sensorless to sensored and from BLCD to FOC mode just to see if there is any difference.
I just drove 5 kilometres and I was not able to get any errors at full brake. 
It drove really smooth. I think I stick to this setup for a while to see if the problem is solved for good now.
```

---
## \#23 Posted by: WARMAN Posted at: 2017-04-18T06:12:02.654Z Reads: 55

```
Just thought I'd update the thread,im now using a space cell,haven't changed any of my vesc settings or made any modifications to my gt2b master cho mod and the problem has gone away.
It must have been a bms problem while braking,I read somewhere that the new space cell is bypassing the bms for discharge and is only used for charging! Would explain why my problem has now dissappeared.
For some it might be vesc settings but thought I'd leave some info on what was causing mine to help others diagnose the problem.
```

---
