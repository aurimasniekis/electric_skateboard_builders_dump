# Strange motor behavior: OM5065 with Vesc and nunchuck

### Replies: 15 Views: 1128

## \#1 Posted by: ndwallick Posted at: 2016-08-10T03:19:45.049Z Reads: 83

```
Wondering if anybody can help me diagnose this motor behavior.

First here is my setup:
10s LiFe (33 volts)
Vesc from Chaka
OM5065 (170kv) motor from Chaka
Nyko Kama nunchuck (temporary remote)
All components sitting on desk, motor is mounted to board of wood.

A couple strange things that are happening:

1) Motor seems to have more torque in one direction (the default forward direction).
When I try to stop the motor with my hand when it's moving forward it is very difficult, but when I push Z on the nunchuck and spin the motor backwards it is very easy to stop. (I can stop it with 2 fingers). This happens on sensored, unsensored, and hybrid mode.

2) When on hybrid mode and accelerating from 0 while holding C (cruise control) motor hiccups when passing 2000 erpm:
<img src="/uploads/db1493/original/2X/3/3d7b4bf0021589d1f75145c01c7f998ac0e59024.png" width="690" height="392">
I will likely never be accelerating from 0 with cruise control but it is possible that this isn't a result of using cruise control but rather a result of the motor accelerating slowly.

When I do not use cruise control the motor accelerates very fast and I cannot test it accelerating slowly until I have it on my board. (don't even have a motor mount yet :sweat_smile: )

This only happens on hybrid mode.


Any ideas on why it's behaving this way would be great! :slight_smile:
```

---
## \#2 Posted by: chaka Posted at: 2016-08-10T03:34:54.266Z Reads: 74

```
Check your " Max current ramp step (at 1 kHz) on the advanced settings of motor config. It should be set at 0.0400.
```

---
## \#3 Posted by: ndwallick Posted at: 2016-08-10T03:45:40.776Z Reads: 69

```
It was set at 50, I remember reading about this value multiplying by 10 when you write config. So I set it to 0.0040 and wrote config. (then read config to confirm it went up to 0.0400) Both behaviors are still present.
```

---
## \#4 Posted by: chaka Posted at: 2016-08-10T04:14:18.224Z Reads: 69

```
It will be best to get it rolling and see how it performs. What have you changed in your settings or is it still mainly in default?  Can we see some screen shots of your settings?
```

---
## \#5 Posted by: ndwallick Posted at: 2016-08-10T04:31:35.329Z Reads: 66

```
Here are screenshots of my settings, I haven't changed much.
<img src="/uploads/db1493/original/2X/5/51e2ade6a00bca80291c52ff1c2f6489bf6e4731.png" width="690" height="386">
<img src="/uploads/db1493/original/2X/3/3b0676f06d5e43a7622213b6c4f940427d1e3ee0.png" width="690" height="386">
<img src="/uploads/db1493/original/2X/3/3bd3d5fdf36abded203594c240c452fdac612b50.png" width="690" height="386">
<img src="/uploads/db1493/original/2X/e/ee50228972dca2a1a60cd7bfaf8491dcdf3e2986.png" width="690" height="386">
<img src="/uploads/db1493/original/2X/1/102467df4aed7e4d9a883230cdcb98328ddae3c5.png" width="690" height="386">
```

---
## \#6 Posted by: Jinra Posted at: 2016-08-10T04:35:06.773Z Reads: 52

```
Your motor regen is a bit low -7A brake current is very weak. I keep mine at the same as my motor max (45A/-45A).

It looks like it's hiccuping when it hits the sensorless erpm (2000), not sure why it's doing this, but my setup had a similar issue. The two things I turned off that I believe affected it was reverse and traction control. Seeing as how you dont have traction control, may try it in current no reverse with brake (or just current for your nunchuck) and see how it goes.
```

---
## \#7 Posted by: ndwallick Posted at: 2016-08-10T04:59:00.691Z Reads: 52

```
I have the motor and battery regen so low because my batteries max charge rate is only 2c.
2c * 3.6Ah = 7.2 max amps for charging
Can I increase (decrease technicaly) the motor regen and keep the battery regen at -7amps?

I just tried current mode and same hiccup happens.
```

---
## \#8 Posted by: Jinra Posted at: 2016-08-10T05:02:01.610Z Reads: 51

```
Yea, battery regen is the value that determines how much current goes back into the battery, I have my battery regen at -8, and my motor regen at -45.

Unsure as to why you're hiccuping, did you make sure your sensor table is accurate?
```

---
## \#9 Posted by: ndwallick Posted at: 2016-08-10T05:32:01.333Z Reads: 50

```
I ran motor detection again to make sure the table was accurate and it is.

I also just noticed that the hiccup only happens when the motor is spinning forward (CCW), so I switched two of the phase wires, ran motor detection again to update the hall sensors, and now it only happens when spinning backwards (still CCW).

idk if that makes any sense haha but basically the hiccup only happens when the physical motor is spinning CCW regardless of the direction the esc is spinning electrically.

Does the order of the sensor wires matter?
I have 5 sensor wires, positive, negative, and the 3 sensors.
I know I have the + and - right (tested voltage and polarity)
but does the order of the 3 sensor wires matter as long as I run detection and update the table?
```

---
## \#10 Posted by: Jinra Posted at: 2016-08-10T05:34:37.849Z Reads: 45

```
I know if you're running sensored the phase wire order can be a bit picky. Try playing around with it until you get smooth operation. I don't think the sensor wires matter as long as the table is accurate.
```

---
## \#11 Posted by: ndwallick Posted at: 2016-08-10T06:20:59.020Z Reads: 38

```
I tried every phase wire combo and I tried resetting the Vesc to default settings, same thing happens. I noticed the motor makes this small sound once every rotation, at first I thought it was just the bearings or something, but maybe it's something more. Here's the sound: [link](https://youtu.be/-XAd9S2PzMo)

Is this sound normal? @chaka
```

---
## \#12 Posted by: Jinra Posted at: 2016-08-10T06:30:18.556Z Reads: 38

```
I think it's normal, both my OM5065's do that.
```

---
## \#13 Posted by: ndwallick Posted at: 2016-08-10T06:46:00.898Z Reads: 35

```
Good haha, so somehow my first problem is gone now. The motor seems to have equal torque in both directions now. Could have been solved when I reset my Vesc to default settings. I guess I'll have to wait til I get a motor mount to see if the hiccup thing affects riding. Thanks for the help! @Jinra and @chaka
```

---
## \#14 Posted by: chaka Posted at: 2016-08-10T13:18:58.484Z Reads: 24

```
Keep me posted on the performance. We will handle it if something isn't right. ;)
```

---
## \#15 Posted by: ndwallick Posted at: 2016-08-10T15:39:45.492Z Reads: 22

```
Awesome :grinning: il post here how it acts once it's on my board.
```

---
