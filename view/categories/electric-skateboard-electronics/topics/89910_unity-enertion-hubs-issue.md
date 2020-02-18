# Unity + Enertion Hubs issue

### Replies: 13 Views: 394

## \#1 Posted by: ThomasL Posted at: 2019-04-09T08:29:54.105Z Reads: 163

```
Hello there,

As a proud owner of a Unity and Enertion Direct drive mounted with a 12s5p battery pack from Eskating.eu and Nano-x remote, I would like to know if one of you guys had the same issue as me:

- While going full throttle from a complete stop, the power cuts out, becoming really dangerous as it does not happen at the beginning, but 3/4 seconds after, once the board is already around 20/25mph. My friend had a crash on it last Saturday

<iframe width="560" height="315" src="https://www.youtube.com/embed/7Y1M7El13Mc" frameborder="0" allow="accelerometer; autoplay; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>

- The board has close to no power while going uphill, and if I press the throttle down, the power cuts out, same as the issue described before

Here you have my UNITY set up:

![ui|240x500](upload://siNTEsJ8DllB2DeIoITs8IXKBZa.png) ![ui|240x500](upload://wsyh8OUZNQ8LAxVWJgPnyQo79Gm.png) ![ui|240x500](upload://fPbESaUvfsa0n6RCY0pzfzyeaNg.png) 

Does anybody has a fix on that ?
Which part would most likely create this issue ?

Thank you,
```

---
## \#2 Posted by: goldrabe Posted at: 2019-04-09T09:05:39.471Z Reads: 139

```
@barajabali @CarlCollins @Deodand @Blasto
```

---
## \#3 Posted by: CarlCollins Posted at: 2019-04-09T11:14:49.244Z Reads: 128

```
Looks like it's the issue with of the firmware, can you please let us know which firmware version you are using on Unity?
```

---
## \#4 Posted by: epss4 Posted at: 2019-04-09T14:04:13.732Z Reads: 112

```
I think your beta value should be 4100 but im sire that not what causing this problem but it will help with thermal throttle
```

---
## \#5 Posted by: epss4 Posted at: 2019-04-09T14:06:36.220Z Reads: 108

```
But i have the same issue with the new firmware., on 12s5p as well... it’s really make me worried.... i crash once and i wont try my board again until they fix it
```

---
## \#6 Posted by: AlanZhou Posted at: 2019-04-09T14:09:32.787Z Reads: 106

```
@b264 not a direct drive :wink:
```

---
## \#7 Posted by: b264 Posted at: 2019-04-09T20:35:02.752Z Reads: 86

```
Hub motors are actually direct drive.  I call them "radial direct drive" instead of "axial direct drive" à la Carvon-style.

Or you can just call them hub motors.

They don't contain gears.
```

---
## \#8 Posted by: Roan_Psyko Posted at: 2019-04-09T22:51:08.948Z Reads: 72

```
Try to re-calibrate your remote and make sure it's in R-spec mode when you do, then run motor detection again. I've had a similar issue in the past after calibrating on slow mode only.
```

---
## \#9 Posted by: sofu Posted at: 2019-04-10T00:05:19.984Z Reads: 63

```
This may be related to incorrect motor detection issue. I'm not sure if there's a firmware update that's been released but there is a fix that I've been testing that does fix this. @Deodand would know better.
```

---
## \#10 Posted by: ThomasL Posted at: 2019-04-10T07:22:27.862Z Reads: 45

```
I am using the firmware 24.42, as it was the one fixing the braking issue at low speed (too aggressive)

Is there another firmware to be downloaded?
Can the Max motor temp create this issue, would it help to raise it to 120/130 ?

@Roan_Psyko  It was calibrated in R-Spec already

I will try later on the new firmware, but I am afraid to retry the test (full acceleration on the remote) as I broke my wrist already on it... Any suggestion to do the test in a "safe" way ?

Thank you all
```

---
## \#11 Posted by: goldrabe Posted at: 2019-04-10T11:46:20.369Z Reads: 42

```
Your Beta is too low, but that is not related to your issue. 23.42 is the latest official firmware, so usually your Beta should have the correct value. Where did you downloaded your firmware?  If not from Enertions website, try to reflash it with the official release.\
I still think that is not the cause of the issue. I have cogging trying to accelerate uphill from really low speed despite my sensors where detected correctly and I get a kind of cogging when I get close to topspeed, but it doesn't feel like a complete power loss, so I am not sure if it's the same.\
Thermal throttling is more noticeable at acceleration in loss of torque. How far do you have set your thermal cut off values set apart? 100°C start 140°C end?
```

---
## \#12 Posted by: ThomasL Posted at: 2019-04-10T12:18:05.767Z Reads: 34

```
I downloaded it from the app on my phone. will try to reinstall it later on tonight.

It does not feel like a power loss, but the inertia from the massive torque to this state makes the board extremely unstable, really dangerous.

Where do you see the cut off value ? I only have the max allowed temp, no start/end
```

---
## \#13 Posted by: goldrabe Posted at: 2019-04-10T13:39:43.213Z Reads: 28

```
Did you updated the firmware with your phone via Bluetooth?\
Enertion does not recommend this. Seeing the old Beta value in the new firmware looks like the update didn't got through correctly. The temp limits can be set in the Focbox tool not the UI.\
Lately there are a few reports on the same issue you have, mostly with higher kv 6374 motors, but not so many with the R-Spec hubs. It's said that there will be a firmware update anytime soon which should solve the issue. I feel you it's scary to get on a board with a known issue. That's the culprit of having the latest tech. Let's hope that with the new firmware everything will perform as expected!
```

---
