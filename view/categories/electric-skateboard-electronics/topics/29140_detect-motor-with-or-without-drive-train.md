# Detect motor with or without drive train?

### Replies: 14 Views: 819

## \#1 Posted by: cledus Posted at: 2017-07-30T18:54:08.467Z Reads: 141

```
Hi!

I'm new to the forum and new to building esk8. I have 3, probably easy questions that I hope some would be kind enough to help me with. 
1. Are you supposed to have the belt connected to the wheel when you do the motor detection in bldc tools?
2. If I want to use FOC do I have to do the motor detection on the BLDC tab first?
3. I did the motor measure on the FOC tab (with the belt connected to the wheel and without doing the motor detection on the BLDC tab). When I move the throttle the motor stutters before it slowly starts to rotate. But even att full throttle the motor spins very slow. What am I doing wrong?

Thanks!
```

---
## \#2 Posted by: Jinra Posted at: 2017-07-30T19:08:29.986Z Reads: 138

```
1. I've done both, but I'm lazy and just do it with the drive train attached now. It doesn't really matter too much.

2. No, they're separate and you do not need to do one to use the other.

3. Did you setup your app config values? Also did you actually apply and write your detection values?
```

---
## \#3 Posted by: cledus Posted at: 2017-07-30T19:31:51.133Z Reads: 128

```
Thank you Jinra for replying!
Now you got me wondering. Maybe I did forget to write the detection values. But I think did setup the remote correctly. I did calibrate it so it goes from 0-100%
```

---
## \#4 Posted by: Jinra Posted at: 2017-07-30T19:33:11.409Z Reads: 121

```
Check your battery cutoff values too, if they're higher than battery voltage you won't be getting much power
```

---
## \#5 Posted by: cledus Posted at: 2017-07-30T19:34:47.727Z Reads: 117

```
I'll do that. 

Thanks again!!!
```

---
## \#6 Posted by: c4Lvin Posted at: 2017-07-30T19:51:43.652Z Reads: 109

```
While we are on this subject, if I may ask if changing to radio system would require to plug in and detect once again? Currently I'm using the GT3B and got a long time from a group buy those TB type smaller controller that uses 2 AA batts. Or do I just replace it without having to go into the damn program. Thanks in advance and sorry I've been away for awhile so lost touch of a lot of stuff!
```

---
## \#7 Posted by: Jinra Posted at: 2017-07-30T19:52:46.022Z Reads: 103

```
You should recalibrate/check for any new controller receiver pair
```

---
## \#8 Posted by: Hummie Posted at: 2017-07-30T20:03:17.215Z Reads: 103

```
I leave the wheel on when doing it but lately thinking the better coupling between the motor and esc the better and I read that's a lot of loss in efficiency here with brushless motors being sent trapezoidal waves and noise with non-sine commutation. Something like that
```

---
## \#9 Posted by: cledus Posted at: 2017-07-31T10:04:53.518Z Reads: 84

```
Hi again!

You were right @Jinra! I had forgotten to write the configuration :slight_smile:! Now it seems to work better. But there is still one mystery. After I have measured R and L I try to measure the ƛ (Req: R) I get an error but if i try again it works. Also does anyone know how to setup failsafe so the board does not continue at full speed if it loses control with the remote? 

Thanks again!
```

---
## \#10 Posted by: krloz Posted at: 2017-07-31T10:11:08.413Z Reads: 85

```
I think that depends on the remote you are using
```

---
## \#11 Posted by: Namasaki Posted at: 2017-07-31T11:32:05.541Z Reads: 78

```
[quote="Jinra, post:2, topic:29140"]
I've done both, but I'm lazy and just do it with the drive train attached now. It doesn't really matter too much.
[/quote]

I recently did a motor detection with just the pulley on and belt removed and then removed the pulley and ran detection again and the coupling valued changed 100 points. 
I don't know what difference that value makes but there is a difference.
```

---
## \#12 Posted by: longhairedboy Posted at: 2017-07-31T11:59:02.816Z Reads: 71

```
I usually do detection like last thing before bolting the box down while its hooked up to the drive train but I think from now on I'm going to do it before i put the belts on to see what kind of difference it really makes. In the past i couldn't tell any difference at all. But using motors with sensors full time has changed some things. 

I've noticed that the numbers change slightly too when unloaded. I've also noticed that the rounded values of the detection results aren't the best values when using hubs sometimes ( we finally got those older Hummies to start up without jittering and being stupid by constantly fiddling with the numbers for like 3 weeks )  and also they may not be the best values for sensored outrunners either. I've started putting the detected numbers in those slots, or as close as it will let me, and i'm seeing a slight improvement. 

using 2.18 fw/bldc tool on linux with focboxes.
```

---
## \#13 Posted by: Jinra Posted at: 2017-07-31T14:35:50.099Z Reads: 62

```
Vedder himself said the numbers weren't too important and applying config can give you up to 50 points less since it rounds down to the nearest 50. I've done both and haven't noticed that much of a difference in detection.
```

---
## \#14 Posted by: cledus Posted at: 2017-07-31T15:38:55.028Z Reads: 56

```
But has anyone had the same problem as me with the second measure on the FOC-tab doesn't work the first time?
```

---
