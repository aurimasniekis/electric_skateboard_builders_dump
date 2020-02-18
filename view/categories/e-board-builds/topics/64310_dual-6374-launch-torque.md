# Dual 6374 Launch Torque

### Replies: 25 Views: 688

## \#1 Posted by: ksfacinelli Posted at: 2018-08-09T03:37:38.623Z Reads: 241

```
Ok... So been playing around with my dual 6734 190kv 10s build and have made a number of observations and would like ideas of better tuning perimeters.

I am using the Ack tool for ESC setup and have been very impressed with all the options.  I currently have my board running 200mm slicks and gearing of 16x72 with 15mm belts.  The board works great no belt slippage but real aggressive launch torque so much so that it jerks pretty hard on acceleration.  I have PPM control type set to current no reverse brake, mapped throttle and using a expo- natural curve at -20. Motor and battery max current set at 60 and running sensor-FOC . 

I also noticed the acceleration at launch was increased with tire pressure.  I am running 50lbs as I like the stiff feel but think this may also be contributing to torque during initial launch.   

Options I am considering: 

1) Lower motor and/or battery max current - will I loose top end?
2) Keep lowering throttle gain?
3) lower tire pressure?

Where do think I should start to smooth out launch acceleration and preserve ride quality and top end?

All suggestions welcomed however could you please let me know...I could also pull some screen shots of configuration tabs if that would help.

Greatly appreciated,

Kevin
```

---
## \#2 Posted by: Sender Posted at: 2018-08-09T03:45:44.037Z Reads: 226

```
Lower the motor amps to 40amps each vesc and that should mellow it out a bit.... keep battery amps where they are.  Then when that feels slow, boost it back up
```

---
## \#3 Posted by: ksfacinelli Posted at: 2018-08-09T03:46:27.860Z Reads: 216

```
Thanks will do......
```

---
## \#4 Posted by: ksfacinelli Posted at: 2018-08-09T03:48:25.001Z Reads: 213

```
How much does throttle curve effect launch acceleration? Does max motor amps effect top end? or hill climbing?
```

---
## \#5 Posted by: rich Posted at: 2018-08-09T07:16:23.819Z Reads: 187

```
[quote="ksfacinelli, post:1, topic:64310"]
but real aggressive launch torque so much so that it jerks pretty hard on acceleration.
[/quote]

My bet is that you have problems with hall sensors because in sensored FOC the motors shouldn't jerk no matter which settings.

Maybe bad hall sensor detection or connectors.

Can you post a screenshot of both hall tables?
```

---
## \#6 Posted by: ksfacinelli Posted at: 2018-08-11T03:26:13.335Z Reads: 138

```
Here is the table for the master:

![image|690x286](upload://pvOMCNVWHtaAhOmFYMPkvN1AEup.png)

I may be describing the action of the board poorly.  If I am very careful with the handheld controller it will take off smooth but seems over sensitive and well a bit to aggressive...I just feel the board has to much low end torque. I can be doing 10mph and it just pulls real hard and still requires me to be careful with the controller.

Kevin
```

---
## \#7 Posted by: Sender Posted at: 2018-08-11T03:48:05.825Z Reads: 121

```
Did you try to lower the motor amps yet?
```

---
## \#8 Posted by: ksfacinelli Posted at: 2018-08-11T03:51:57.012Z Reads: 119

```
Yes, will report once I get on it in the morning.

![image|690x311](upload://rRAHhKwq7K50Q6hil7p0GBwXdVV.png)
```

---
## \#9 Posted by: ksfacinelli Posted at: 2018-08-11T04:00:19.365Z Reads: 114

```
Does this all look correct?

![image|690x323](upload://ngpTgiGWU1PhqEyvzej3UcWJlxh.png)

Throttle Curve

![image|690x378](upload://vANLHIB3BrCXHBGg52BoHqlAfZu.png)
```

---
## \#10 Posted by: TowerCrisis Posted at: 2018-08-11T04:10:21.227Z Reads: 102

```
In your PPM settings do you have a significant deadband? I've found that decreasing this as much as possible helps with startup jerking (does not affect cogging).

As long as your remote is sensitive enough, it should be picking up the low end of throttle fine.


Also, it definitely is not your motor amps. You are not pulling 40 amps from a gentle startup. The only time that would happen is if you are trying to gun it from the start, which it sounds like you are trying to accomplish the opposite.

I would set motor amps Max at whatever the motor is spec'd at. If the motor doesnt have a spec for that you can claculate it, an 8s max 2000w motor should have a Max of 60A. Simply W=VA
```

---
## \#11 Posted by: deucesdown Posted at: 2018-08-11T04:16:49.839Z Reads: 98

```
Side note, 60a batt max is a lot for dual. You're potentially asking 120a from your pack.
```

---
## \#12 Posted by: ksfacinelli Posted at: 2018-08-11T04:17:08.263Z Reads: 95

```
I like the idea of adjusting the dead band here is current settings.

![image|690x384](upload://wTZr3KcBnX5D317bVaxjqb3tMx4.png)
```

---
## \#13 Posted by: TowerCrisis Posted at: 2018-08-11T04:20:09.160Z Reads: 93

```
My lord a 15% deadband??

That is wayyyy too high. The instant you pull the trigger past that point it's going to be trying to pull at least 5A from the motors, and if you're just coasting that's a huge jolt.

I've kept mine at ~2%. Just high enough so that my motors won't jiggle or whine when I'm not touching the trigger.
```

---
## \#14 Posted by: ksfacinelli Posted at: 2018-08-11T04:22:11.656Z Reads: 92

```
Thanks....I think you may have solved what I am dealing with....made the change.

![image|690x204](upload://8IWaHIzWz0QqqFbErqQd4CaMA0n.png)
```

---
## \#15 Posted by: TowerCrisis Posted at: 2018-08-11T04:23:13.960Z Reads: 90

```
Awesome, let us know how it goes! 😃
```

---
## \#16 Posted by: ksfacinelli Posted at: 2018-08-11T04:23:35.339Z Reads: 90

```
Will do!!!!
```

---
## \#17 Posted by: ksfacinelli Posted at: 2018-08-11T04:27:15.559Z Reads: 92

```
Yea so the purpose of the dead band is for the motors to have less sensitivity or as you stated not jiggle at rest?  I made the change and the motors are quite with the remote sitting idle.
```

---
## \#18 Posted by: TowerCrisis Posted at: 2018-08-11T04:36:31.393Z Reads: 93

```
As long as the motors aren't trying to move while you're not pulling the trigger, you're fine :)
```

---
## \#19 Posted by: rich Posted at: 2018-08-11T08:32:03.667Z Reads: 89

```
[quote="TowerCrisis, post:10, topic:64310"]
In your PPM settings do you have a significant deadband? I’ve found that decreasing this as much as possible helps with startup jerking (does not affect cogging).
[/quote]


Maybe I misunterstood the thread, jerking and cogging is for me the same (but english is not my language :wink:). What's the difference?

@ksfacinelli the hall table looks fine. 
Maybe this has nothing to do with your problems but in general the Battery Current Max should be lower or equal the Motor Current Max.  So if you set 40A motor max then set 40A batt max or lower.

Your max wattage (and braking) is set to 15kW :crazy_face:
```

---
## \#20 Posted by: TowerCrisis Posted at: 2018-08-11T08:39:19.763Z Reads: 84

```
In this context cogging is when the motor rotation can't keep up with the phase wire switching, which leads to the back and forth jerking we all know too well. That is a result of the motor being stalled.

What OP is experiencing is jerking on startup. He means that when he first pulls the throttle the board will try to go forward very hard and yank the rider forward unexpectedly. This is not a result of cogging, he is experiencing acceleration at low speed that is not corresponding to his trigger pulling.
```

---
## \#21 Posted by: rich Posted at: 2018-08-11T09:01:28.550Z Reads: 78

```
Great explanation, thanks! And I was wrong :laughing:

Then it could be as you mentioned PPM settings.

@ksfacinelli which remote do you use? 

I found out that different remotes react different (without throttle curve adjustments) e.g. I have a steez which is very sensitive and smooth accelerating/braking from 0% to 100%. Then I have this new Maytech remote (also tested on the same board) which is not so nice (without addjustments). It takes forever until the acceleration starts (when push throttle) and it's kinda strange feeling in general. Same for breaking, it takes some time and then suddenly very strong brakes. I have much more fun with the steez but I'll try to adjust the curves for the Maytech remote to see if it's getting usable.
```

---
## \#22 Posted by: Andy87 Posted at: 2018-08-11T09:36:06.646Z Reads: 73

```
Question to the wattage.
Thought it will be restricted anyhow by your max current settings?🤔
Read that somewhere in the ackmaniak thread. Even in the watt mode the max current has priority. So for me it would mean that even with watt settings over the edge you never come over the max current*voltage you actually drive with.
Is it wrong?
```

---
## \#23 Posted by: rich Posted at: 2018-08-11T10:20:47.740Z Reads: 70

```
Makes sense that it's restricted by max current settings but I'm no expert in wattage and used ackmaniacs FW only last year on V4 for some time. When I remember right the default max wattage was 1500W that's why I mentioned the set 15000W.
```

---
## \#24 Posted by: ksfacinelli Posted at: 2018-08-11T16:50:26.786Z Reads: 64

```
@rich,

I checked this and it is the default value is 15000W in the ACK tool.......here is the help message. I think it is set this high just ensure it is disabled. 

![image|690x370](upload://qpXohkVutjHHkBuTuXOOYeFmLIL.png)
```

---
## \#25 Posted by: ksfacinelli Posted at: 2018-08-14T00:53:40.359Z Reads: 58

```
@TowerCrisis,

Thank You!!!! The issue was definitely due to dead band setting.  Worked like a charm by pulling it down to 2%. Really appreciate the advice as I was stumped.  This is why the community works so well.

:grinning:

Kevin
```

---
