# Hitting max erpm when driving?

### Replies: 9 Views: 1047

## \#1 Posted by: vicciu Posted at: 2018-04-23T06:27:03.833Z Reads: 209

```
Hey guys, I'm currently running a Turnigy SK3 5045 450kV on a 6S battery in BLDC mode and from my calculations the max eRPM should be around 70K which is over the VESC limit of 60K eRPM. Does anyone have any experience on what happens when you hit the eRPM limit while riding? I really wouldn't like to fall because the vesc suddenly brakes at over 40km/h.
```

---
## \#2 Posted by: Exiledd_Top Posted at: 2018-04-23T06:52:19.074Z Reads: 202

```
if u pass the erpm limit u fry  your vesc or it shuts off can't handle it , your kv is way to high at most people would run 200ish-260 kv at 6s and 170-190kv for 10-12s  your hitting erpm limit to fast and no throttle curve,  plus I think it clogs  if kv to high because there not meant for electric skateboards but rather planes, boats ,ect to much load to high of kv
```

---
## \#3 Posted by: Trdolan03 Posted at: 2018-04-23T06:56:05.203Z Reads: 202

```
Is there any way to effectively limit the speed then via programming the vesc?
```

---
## \#4 Posted by: TehAtheist Posted at: 2018-04-23T07:21:59.164Z Reads: 191

```
It is possible to set up ERPM max value on the VESC with for example the VESC tool.
On this tab you have "MAX ERPM" (also for reverse if you use this, but if you use the current with brake no reverse option, you don't need to set this.)

It's also highly recommended to setup the ERPM limit start, this means for example for 80%, that at 80% of the topspeed, your acceleration will decrease. This way you don't suddenly stop accelerating at your desired speed.
I have mine set at 75%. The  lower your max speed, the sooner you want to decrease acceleration.

![image|690x347](upload://pzf0GIPOJz2WrClRLAwumz7v4cZ.png)

Whatever you do, don't benchtest your drivetrain without limiting the RPM I guess? Other wise a burned DRV will be the result I think.
```

---
## \#5 Posted by: Exiledd_Top Posted at: 2018-04-23T07:26:04.251Z Reads: 168

```
his kv motor is 450 and it's a small motor 5045 that thing has no Torque what so ever and to much of high kv  he can try to limit it but I don't think it works with high kv because of certain factors I can't think of rn
```

---
## \#6 Posted by: vicciu Posted at: 2018-04-23T07:51:52.661Z Reads: 165

```
@Exiledd_Top actually I have plenty of torque with the dual motors and 12:38 gearing on 82mm wheels. It takes about 5 seconds or so to get to 30km/h with my weight being 80kg.

@TehAtheist thanks for the advice, I'll think about that. The main problem is that I want to keep the 40km/h top speed(that's the speed at 60K erpm) and by making rpm limit start at 80% means that my top speed will drop by about 5km/h. Also I see in your screenshot that your Max ERPM is 100K. Can the VESC run that high?
```

---
## \#7 Posted by: TehAtheist Posted at: 2018-04-23T15:52:18.614Z Reads: 148

```
@vicciu If you calculate the ERPM for your motors for 40km/h ( with the factors wheel diameter, gear ratio, etc) and set that value, you will reach it. Settings the ERPM limit start will NOT lower it, it just makes the top speed less abrupt.

If you were to try to accelerate at max acceleration from 0 to 60 km/h, with the limit on 40km/h, your board would suddenly stop accelerating at 40km/h and you would be thrown off due to the sudden change in acceleration.
If you set the ERPM limit to lets say 80% and to the same test, your board would start to decrease the ACCELERATION (not speed!) at 32 km/h, you will still be going faster and faster, but at a slower rate as if you were releasing the throttle a little. This way, the max speed of 40 km/h will be reached but without the sudden change in acceleration.

The value on my screen of 100000 is the default value I think (My vesc isn't connected, I just opened the tool to show a screenshot), my board is limited to either 25, 30 or 40 km/h, depending on the profile I set in metr.at (the phone application). So that's around 36000 I believe, in my case atleast. The default value is that high, just to not use the value, it doesn't mean that you can reach it without damaging.

Cheers.
```

---
## \#8 Posted by: E1Allen Posted at: 2018-04-23T16:03:16.520Z Reads: 130

```
Also, uncheck the box that says Limit ERPM with negative torque.  If that box is checked, reaching erpm limit will apply brakes on its own.  Not good while going fast in the forward direction
```

---
## \#9 Posted by: TheCookieHunter Posted at: 2019-04-05T16:04:53.743Z Reads: 39

```
How do you set a limit to km/h?
```

---
