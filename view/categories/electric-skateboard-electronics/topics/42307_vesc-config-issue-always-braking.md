# VESC config issue: &ldquo;always braking&rdquo;?

### Replies: 15 Views: 544

## \#1 Posted by: escarabin Posted at: 2017-12-30T16:26:18.151Z Reads: 85

```
Hi guys,

I just finished my DIY build today (a Boosted board Dual+ damaged by water that I got back on the street with fresh new VESCs and battery) and everything works great except for one annoying behavior: It is "always braking". I mean that if I am going forward and then abruptly release the throttle without actually moving the throttle backwards to brake, it instantly brakes really hard, that feels very dangerous, I cannot just go "free wheels". 
That means that if I want to slow down when going full speed, I have to carefully slowly move the throttle down to stop. Also, if I try to spin the wheel with my hand, it shows some heavy resistance.

What do you think I should do to my config? 

I got a TORQUE ESC VESC ® BLDC from DIYELECTRICSKATEBOARD

Thanks a lot﻿ for your help
```

---
## \#2 Posted by: bigben Posted at: 2017-12-30T16:29:08.646Z Reads: 86

```
You should set up in the vesc settings. You may also be able to do it on your trim on the remote. Which remote do you have?
```

---
## \#3 Posted by: escarabin Posted at: 2017-12-30T16:33:34.112Z Reads: 84

```
Thanks, I use the ABSIMA "CR2S.V2" but I don't think the issue actually comes from the remote, the board is braking even when the remote is off/disconnected. Also, I tried modifying the trim but it didn't help.
```

---
## \#4 Posted by: MysticalDork Posted at: 2017-12-30T17:14:26.201Z Reads: 82

```
Post a screenshot of your vesc configuration in the PPM tab.
```

---
## \#5 Posted by: faithfulpuppy Posted at: 2017-12-30T17:29:31.115Z Reads: 77

```
to me, this sounds like the VESCs are set with the min/max pulsewidth set too high. To fix this:

plug one of the VESCs into your computer and turn it on, and check the pulsewidth when the controller is at the neutral/freewheel position (App configuration > PPM > check the box that says "display"). Ideally, it will read about 50% and the pulsewidth (for my hardware at least) should be about 1.5ms (that could be different depending on your remote and receiver)

if it's not at 50%, give full throttle, and check the pulsewidth. Set the max pulsewidth to about that value. Then, Give full brake, and set the min pulsewidth to that value. At this point, the pulsewidth should read 50% at neutral. If it doesn't, you're probably gonna have to mess around with this stuff a little.

Finally, use the median filter and deadband (not 100% on how exactly those functions work, so play around with them a bit) to create a deadzone at the neutral position.
```

---
## \#6 Posted by: laurnts Posted at: 2017-12-30T21:21:22.262Z Reads: 60

```
Agree with @faithfulpuppy I think you need to recalibrate the PPM setting.
```

---
## \#7 Posted by: faithfulpuppy Posted at: 2018-01-01T19:12:25.735Z Reads: 54

```
What happened with this?
```

---
## \#8 Posted by: escarabin Posted at: 2018-01-01T19:25:29.980Z Reads: 50

```
thanks a lot for your suggestions & help. Sorry I have been travelling for the past few days, I will have access to the board tomorrow and will let you know!
```

---
## \#9 Posted by: escarabin Posted at: 2018-01-02T10:50:10.422Z Reads: 43

```
@faithfulpuppy so I tried to follow your instructions but I actually already set my pulse min/max before.
When at neutral position, it is around 50% (see screenshot below).
Also, I have reverse mode activated so when I am at neutral position it seems to be the "braking" position, even when remote is off, the wheels don't want to spin freely.

<img src="/uploads/db1493/original/3X/a/3/a3647fc1a538351600e47bef4bad0c73230230c8.png" width="690" height="431">
```

---
## \#10 Posted by: faithfulpuppy Posted at: 2018-01-02T12:02:03.942Z Reads: 37

```
>I have reverse mode activated

Oh yeah I had that problem with reverse mode. Don't know how to fix it. Maybe someone else here will? Otherwise you can use non braking mode
```

---
## \#11 Posted by: PXSS Posted at: 2018-01-02T12:04:34.360Z Reads: 35

```
You are using duty cycle. At 50% throttle, you are commanding 0rpm, that’s why it brakes.
```

---
## \#12 Posted by: escarabin Posted at: 2018-01-03T11:10:27.324Z Reads: 27

```
So which mode should I use? If I use "Current" mode I can have my wheels to spin freely but it always goes full speed if I just slightly push the throttle, I have no control over it
```

---
## \#13 Posted by: PXSS Posted at: 2018-01-03T13:00:27.411Z Reads: 25

```
This only happens on the bench because there is no load on the motor. Have you tried riding it with either mode???
```

---
## \#14 Posted by: escarabin Posted at: 2018-01-03T13:22:36.380Z Reads: 22

```
Oh ok...I just tried riding it in "current" mode and found myself pretty stupid, it does work perfectly.

I had a Boosted Board and I was able to control motor speed even if I wasn't on the board, that's why I find it surprising.

Thanks a lot
```

---
## \#15 Posted by: PXSS Posted at: 2018-01-03T13:31:06.650Z Reads: 21

```
Have you tried riding in duty cycle??
I think if you disable the negative torque limit, you can cruise without it braking but I’m not entirely sure.

Post your settings in motor tab and general tab
```

---
