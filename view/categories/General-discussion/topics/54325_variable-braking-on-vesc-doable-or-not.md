# Variable braking on VESC - doable or not?

### Replies: 48 Views: 1149

## \#1 Posted by: cot709394 Posted at: 2018-05-04T02:03:45.607Z Reads: 149

```
This must be a newbie question, but I haven't come across a definitive answer yet.

**My configuration** - Chinese 250W BLDC motor connected to VESC (v2.18 firmware) with Hall sensors supplied by a juicy 22.2V cell pack

PPM input as throttle control and it was verified to cover the full range (0 to 100%) when displayed on BLDC Tool.

**Question** - When freewheeling downhill, I want to be able to apply a variable amount of braking instead of simple on/off. _Is that possible with a PPM throttle?_ I have tried tuning the "Motor min (regen)" and "Batt min (regen)" current limits already, but it made no difference.

If regen braking cannot do it, _are there other methods?_

**Supplementary info** - When I used PID speed control, variable speed propulsion forward and reverse was totally achievable.
```

---
## \#2 Posted by: Deckoz Posted at: 2018-05-04T02:20:07.013Z Reads: 139

```
Vesc is progressive braking unlike RC escs. Post up your motor min and battery min amperage settings, and your weight and setup etc..

Also you should be running Current Control with brakes, no reverse optional.
```

---
## \#3 Posted by: MysticalDork Posted at: 2018-05-04T02:24:48.549Z Reads: 131

```
Yes, it does variable braking by default.
```

---
## \#4 Posted by: cot709394 Posted at: 2018-05-04T02:30:30.071Z Reads: 123

```
**Snapshot of motor control settings**

Motor max    60A
Motor min (regen)   -10A
Batt max   60A
Batt min (regen) -10A
Absolute max   130A

Already in "Current no reverse with brake" mode.

Physical configuration: single motor direct drive

Body weight   55kg

What other info is needed?

Thanks for a speedy response.
```

---
## \#5 Posted by: MysticalDork Posted at: 2018-05-04T02:32:03.411Z Reads: 107

```
set your motor min to like -40 or -60.

Depending on your battery, you may also want to increase your battery min by a little too.
Be aware that if you have a nearly full battery, on a long hill, you may reach an overvoltage on the battery, at which point the brakes will cut out.
```

---
## \#6 Posted by: cot709394 Posted at: 2018-05-04T02:33:05.875Z Reads: 106

```
In that case I must have missed something in the settings. The braking right now is just simply on/off.

I want to be able to coast downhill with speed control. Too much to ask for? :slight_smile:
```

---
## \#7 Posted by: MysticalDork Posted at: 2018-05-04T02:33:55.437Z Reads: 97

```
It really isn't just on/off. Increase your minimum barking current and try again.
```

---
## \#8 Posted by: cot709394 Posted at: 2018-05-04T02:35:31.657Z Reads: 97

```
Oh yes, the full battery issue was already explored, but that wasn't the reason.

The power pack I have is spec'd at 7500mAh at 22.4V. It does propel uphill quite well.
```

---
## \#9 Posted by: MysticalDork Posted at: 2018-05-04T02:36:19.673Z Reads: 95

```
What type of battery specifically? Lipo? Li-ion? What brand?
```

---
## \#10 Posted by: cot709394 Posted at: 2018-05-04T02:36:24.347Z Reads: 91

```
"Increase minimum braking current" means more -ve. Right?
```

---
## \#11 Posted by: MysticalDork Posted at: 2018-05-04T02:37:29.754Z Reads: 84

```
I need more details on your battery first.
```

---
## \#12 Posted by: cot709394 Posted at: 2018-05-04T02:39:09.751Z Reads: 80

```
The battery pack is made up of a bank of 18650 cells wired in a 6-cell series, with up to 3 packs in parallel.
```

---
## \#13 Posted by: cot709394 Posted at: 2018-05-04T02:41:00.004Z Reads: 79

```
These cells are Samsung Li-ion ones.

I have also tried a 22.2V Li-Po pack, but it made no difference.
```

---
## \#14 Posted by: MysticalDork Posted at: 2018-05-04T02:42:03.816Z Reads: 76

```
What **Specific** samsung li-ion cells are they? What does the text on the wrapper say?
```

---
## \#15 Posted by: cot709394 Posted at: 2018-05-04T02:44:26.261Z Reads: 73

```
Samsung INR18650-29E
```

---
## \#16 Posted by: MysticalDork Posted at: 2018-05-04T02:51:17.809Z Reads: 77

```
Those cells are only good for about 10 amps each discharge, and 2.5 amps each charge. With a 6s3p. that means your maximum safe battery current is 30 amps, and your maximum regen current is about -7.5 amps.

This is far from ideal for an esk8, it severely limits your available power, as well as your available braking current, which may be contributing to your braking issue.

If you plan to continue using this pack, set your vesc as follows:

Motor max: 60
motor min: -40 to -60
batt max: **-30**
batt min: **-7.5**

You will have good braking at low speed, but it will be crappy at high speed, and the only way to improve this is to use a battery that can handle a higher charge current (Battery min)
```

---
## \#17 Posted by: cot709394 Posted at: 2018-05-04T02:55:59.135Z Reads: 72

```
Thanks, MysticalDork.

I knew that these cells are reasonably cheap and the chemistry is a bit slow to charge, but they do yield a decent peak current.

What if I am happy to burn the power off instead of regen, would that give me more control on the variable braking? I suspect that this is kinda undermining the VESC design.
```

---
## \#18 Posted by: MysticalDork Posted at: 2018-05-04T02:57:41.076Z Reads: 74

```
Unfortunately, to my knowledge, the vesc is only able to "burn off" power when braking at 100%, and only at low speed. More than that would cause the vesc to blow up.
```

---
## \#19 Posted by: MysticalDork Posted at: 2018-05-04T02:59:07.818Z Reads: 73

```
I can tell you that with the exact same settings that you have there, with the exception of a higher battery minimum (and batteries that can handle it), both of my previous builds had smoothly variable braking.
```

---
## \#20 Posted by: cot709394 Posted at: 2018-05-04T02:59:22.960Z Reads: 75

```
Gotcha, thanks!
```

---
## \#21 Posted by: MysticalDork Posted at: 2018-05-04T03:00:22.816Z Reads: 67

```
As a temporary measure, you can try the lipo batteries you were using - They can generally handle a lot more charging current.
```

---
## \#22 Posted by: cot709394 Posted at: 2018-05-04T03:02:20.380Z Reads: 68

```
I only have a single 1600mAh Li-Po pack in hand. Will try to get my hands on more to run them in parallel.
```

---
## \#23 Posted by: E1Allen Posted at: 2018-05-04T03:14:06.589Z Reads: 69

```
That lipo pack is to small for eskate application even in parallel it's not worth it.
```

---
## \#24 Posted by: cot709394 Posted at: 2018-05-05T02:07:29.706Z Reads: 54

```

Well, it's been changed to a 11000mAh Li-Po pack.

But still the gradual braking does not seem observable. :frowning:
```

---
## \#25 Posted by: E1Allen Posted at: 2018-05-05T03:44:47.217Z Reads: 53

```
I someone help me out here.  In his first post he said a Chinese 250w motor? I don't think that motor would provide very much brake Force at all.  Think this is the problem?  Max amps for his voltage is like 11a...
```

---
## \#26 Posted by: telnoi Posted at: 2018-05-05T05:50:05.656Z Reads: 50

```
Did you properly configure your ppm range? Also do note that unsensored FOC tends to break hard at slow speed.
```

---
## \#27 Posted by: cot709394 Posted at: 2018-05-05T06:35:01.187Z Reads: 48

```
Thanks, E1Allen.

I could feel that the Chinese motor is providing decent braking, but the action is binary instead of gradual. I think most of us would appreciate the problem of snap-braking especially with going downhill.
```

---
## \#28 Posted by: cot709394 Posted at: 2018-05-05T06:39:19.725Z Reads: 48

```

Thanks, telnol.

Using BLDC Tool, I can visualise the PPM range from my RC. It does cover the full 0 to 100% range in a gradual sweep.

I have also got an Arduino pumping out the same control waveform to let me develop without tying one hand to the RC.

BTW, the motor is sensored, and i have connected them to the VESC. The sensor pattern discovered in "Start Detection" in BLDC Tool has been copied into the motor configuration.
```

---
## \#29 Posted by: MysticalDork Posted at: 2018-05-05T06:40:03.645Z Reads: 46

```
Quick stupid question: at what speed have you tested the brakes?
```

---
## \#30 Posted by: cot709394 Posted at: 2018-05-05T06:42:51.291Z Reads: 48

```
The testing was done at low RPM, typically below 1000.
```

---
## \#31 Posted by: danielz Posted at: 2018-05-05T06:42:55.885Z Reads: 47

```
Just to avoid confusion. All braking is regen.
https://vesc-project.com/node/398
```

---
## \#32 Posted by: cot709394 Posted at: 2018-05-05T06:45:01.512Z Reads: 47

```

Correct, danielz.

I am not attempting active braking, although that would make an interesting addition to supplement the VESC. :smirk:
```

---
## \#33 Posted by: MysticalDork Posted at: 2018-05-05T06:45:16.135Z Reads: 45

```
This may be your problem. The braking at low speed can be a bit jerky, especially in sensorless FOC. Try it at higher speed.
```

---
## \#34 Posted by: MysticalDork Posted at: 2018-05-05T06:46:44.433Z Reads: 42

```
there's also a setting on some versions of bldc tool (missing in ack's iirc) called something like "minimum ERPM to apply full brake", you can try lowering that value to like 500.
```

---
## \#35 Posted by: cot709394 Posted at: 2018-05-05T06:48:52.904Z Reads: 43

```
Oh dear. If the low speed is the problem, then I have to go back to the drawing board. The motor is on direct drive with planetary gears, chain or belt to play with.

Although I use it with sensors enabled, there wasn't much difference in controllability compared to the case when I had them disabled.

The active braking idea above has sown a seed. Good or bad - I don't know.
```

---
## \#36 Posted by: cot709394 Posted at: 2018-05-05T06:49:35.572Z Reads: 44

```
"Without" gear, chain or belt.
```

---
## \#37 Posted by: b264 Posted at: 2018-05-05T06:52:03.678Z Reads: 44

```
Have you modified the firmware?  Try using stock version 2.18
```

---
## \#38 Posted by: MysticalDork Posted at: 2018-05-05T06:53:08.052Z Reads: 44

```
Try this. ![braking|690x371](upload://8p5ylojCFUOjiCWYCDOh9ySmYzA.jpg)
```

---
## \#39 Posted by: cot709394 Posted at: 2018-05-05T06:54:01.289Z Reads: 43

```
Thanks, b264.

I am supposed to be using stock 2.18 firmware. How could I tell if it isn't stock?

When connected to BLDC Tool, Firmware 2.18 is always reported.
```

---
## \#40 Posted by: b264 Posted at: 2018-05-05T06:56:12.609Z Reads: 44

```
You aren't supposed to be using anything in particular, you can use whatever you want by whomever you want.  I just asked because you mentioned you were developing and the old 2.18 release by Benjamin Vedder has been heavily tested by members here.  So let's start with one we know doesn't have a braking problem while we troubleshoot.
```

---
## \#41 Posted by: cot709394 Posted at: 2018-05-05T07:25:19.185Z Reads: 40

```
Thanks, MysticalDork.

The "Limit EPRM with negative torque" box was unchecked already, and the Max EPRM at full brake raised to 500.

BTW, since I have switched to the Li-Po cells, the Motor min (regen) and Batt min (regen) were raised to -60A and -45A respectively.
```

---
## \#42 Posted by: b264 Posted at: 2018-05-05T07:27:10.763Z Reads: 38

```
Battery Min at -45A is pretty steep, for troubleshooting that's cool -- but double check your lipo battery to ensure it can charge at that rate before using it extensively that way.
```

---
## \#43 Posted by: MysticalDork Posted at: 2018-05-05T07:31:44.966Z Reads: 37

```
make sure the second minimum erpm box (the one related to current control mode) is also set to 500.

And like b264 said, you may want to set the batt. minimum to like -20 or so, -45 is a bit hard on the cells.
```

---
## \#44 Posted by: cot709394 Posted at: 2018-05-05T07:40:26.739Z Reads: 36

```
Yes, Batt min (regen) at -45A was a bit much. At the low RPM I am running, it's never reached, except with the odd spikes.

For a normal ride, probably -20A is sufficient. The new Li-Po cells cost a bit...

Just to confirm, both Max ERPM at full brake boxes are at 500 already.
```

---
## \#45 Posted by: E1Allen Posted at: 2018-05-05T08:56:35.594Z Reads: 34

```
If I'm going slow enough. 1-5mph.  Depending on how I hit the brakes my rear wheel sometimes stops and can momentarily drag the wheel.  Is this what you experience. Or do you experience something different that feels like the board will stop and throw you off.  What speeds are you experiencing this?  I would say most VESC users on this forum with fairly normal settings can control their braking by increasing or decreasing controller input.  It's not a hard stop when going fast to slow. It's gradual.  However at slow speeds you may experience more abrupt but manageable stops.
```

---
## \#46 Posted by: cot709394 Posted at: 2018-05-06T08:55:12.528Z Reads: 28

```
When braking is activated, it comes in pretty well 100%, which really takes some getting used to. That's why I was looking to do it gradually.

It is particularly annoying when I coast gently downhill (estimated at less than 3mph) and try to come to a "graceful" dead stop while keeping both feet on the board.

Occasionally at extreme slow speed, braking would disappear for no obvious reason, and I would need to release the throttle back to 50% and re-apply braking to get it back.

The braking behaviour of the VESC at low speed has been really perplexing. I guess not many would rely on braking as a feature.
```

---
## \#47 Posted by: telnoi Posted at: 2018-05-06T08:58:59.947Z Reads: 29

```
At this point I have no clue what's going on with your setup, but braking is extremely precise and controllable for me. 10s, unsensored bldc at 149KV with 5:1 ratio.
```

---
## \#48 Posted by: cot709394 Posted at: 2018-05-07T09:04:23.522Z Reads: 23

```
Just as as an experimental set-up to get to the bottom of my issue, I have hooked up a second VESC, hub motor and wheel combo to act as a simulated road surface to visualise the braking behaviour.

There were two interesting findings:

1. Gradual braking is achievable when the braking motor is running beyond 4000rpm. At lower speeds, braking appears to be a binary on/off action.

2. According to "Realtime Data" in BLDC Tool, the regen battery current in my set-up only reaches no more than -2.00A. Perhaps the Li-Po cells are a little extravagant.

Given observation (1), I don't think I have a choice but to introduce some gearing to make sure a sufficiently high RPM even when coasting at low speed (estimated at 600rpm). The downside is that my top speed is going to take a massive hit. :disappointed_relieved:
```

---
