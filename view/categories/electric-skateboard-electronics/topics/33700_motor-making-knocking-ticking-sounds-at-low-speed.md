# Motor making knocking &amp; ticking sounds at low speed

### Replies: 40 Views: 3007

## \#1 Posted by: Sebike Posted at: 2017-09-22T09:57:36.632Z Reads: 174

```
Hey guys!

Just went for a ride and noticed that above a certain RPM my motor started making this high pitched metallic noise. It disappeared as RPM kept increasing, and reappeared as RPM decreased to the previous level. 
Also, after the ride I had this ABS OVER CURRENT fault code.

The motor does the same noise without load.

Before the ride I had adjusted Motor Min from -45A to -55A and Batt Min to -25 from -12. I switched back to the older settings, but the issue remains.

Other than that settings were the same as on previous rides. I had also adjusted the motor mount so it was better aligned to the wheel.

My setup includes
A single 6374 sensored motor from eskating.eu ( @fottaz )
FocBox 
10s4P 30qs and SuPower 60A BMS
and I've been using the extended BLDC tool to set up FOC.

Have always been running in FOC-mode with no issues.

Any idea what this could be and why I got the over current fault?

:smile_cat:

<img src="/uploads/db1493/original/3X/b/e/be9fdeb9e869e9bd84789b562a3f0198a4b6b804.gif" width="690" height="387"><img src="/uploads/db1493/original/3X/7/1/71ad749f0192a236713744be51d660bcd3281a5d.gif" width="690" height="387"><img src="/uploads/db1493/original/3X/b/c/bc82a75bfc3366034baef03932670ddd0f9ab372.gif" width="690" height="387"><img src="/uploads/db1493/original/3X/4/8/48d5d674e640d176a1340eb7cb461fbfdbcfd112.gif" width="690" height="387"><img src="/uploads/db1493/original/3X/5/1/516e7d73a02d3f530f1cbdb7a69136c0a98d54d4.gif" width="690" height="387">

https://youtu.be/hHey1FhLqeI

https://youtu.be/-rGzhA1wy3c
```

---
## \#2 Posted by: scepterr Posted at: 2017-09-22T10:00:37.859Z Reads: 145

```
Try rerunning motor detection?
```

---
## \#3 Posted by: Sebike Posted at: 2017-09-22T10:09:45.826Z Reads: 140

```
Sure, I could do that, but as nothing was changed setting- or setup-wise, apart from what I mentioned, why do you think that would make any difference? 

(As motor detection should be done with no load whatsoever on the motor, I'm afraid I will strip the threads in the motor if I remove and remount the motor mount, as it already happened with the threads one of the holes.. )

Maybe I could try with belt attached..
```

---
## \#4 Posted by: scepterr Posted at: 2017-09-22T10:10:39.638Z Reads: 131

```
Just remove wheel
Well, if new detection looks noticeably different than prior it's likely some kinda hw fault, assuming motor itself is fine
```

---
## \#5 Posted by: Martinsp Posted at: 2017-09-22T10:14:33.164Z Reads: 129

```
Benjamin in one of his videos on setting up FOC did motor detection with belt attached so maybe it is a case of bldc only?
```

---
## \#6 Posted by: Sebike Posted at: 2017-09-22T10:30:06.786Z Reads: 129

```
Ran a new motor detection and I believe values seem to be more or less the same<img src="/uploads/db1493/original/3X/d/2/d2c8287774d71a51343595ba0ba1c2386c14e5c4.gif" width="690" height="387">
```

---
## \#7 Posted by: Sebike Posted at: 2017-09-22T10:58:46.748Z Reads: 121

```
I couldn't replicate the over current error, but the noise is still there, with or without wheel and belt.
```

---
## \#8 Posted by: Martinsp Posted at: 2017-09-22T11:13:20.898Z Reads: 123

```
Hmmm in the video it sounds like at a certain rpm the motor hits some frequency that resonates with the board or some part of it. Try connecting to bldc tool and on the right set the rpm to where it makes the noise and check if there is something rattling or resonating. Maybe try a different motor if you have one...
```

---
## \#9 Posted by: Sebike Posted at: 2017-09-22T11:30:31.036Z Reads: 129

```
Thanks @Martinsp

I listened to the motor carefully and noticed this noise from somewhere in or around the motor that's actually present at all speeds. Sounds like something is touching at each turn of the motor. Probably it's this noise that makes that screeching sound at a certain rpm. 

When keeping the motor running at a low speed you can hear some other repeated noise that follows by the motor loosing some momentum. At this low speed it seems the motor runs a bit uneven or inconsistently, like it keeps loosing power for a split second after that cogging sound?

https://youtu.be/voLj2lPpFKM
```

---
## \#10 Posted by: Sebike Posted at: 2017-09-22T11:37:42.034Z Reads: 125

```
The second noise is probably more audible in this second video. Repeated irregular (?) bumping noises.

https://youtu.be/CxHLp2CCZGU
```

---
## \#11 Posted by: Martinsp Posted at: 2017-09-22T11:39:18.498Z Reads: 123

```
Oh yeah that is definitely a grinding noise. I would suggest you to first check the connections from vesc to motor because the loss of power might be a connector that is not making good connection and when it is vibrating it cuts the power. That would explain the abs over current fault too. 

The grinding noise is probably something I'm the motor it has happened to me that there was a small rock inside and when the rotor is spinning it hits it. If you are worried that you will strip the thread in the motor you can leave the stator of the motor screwed to the mount and just take the pulley off and then the circlip which will allow you to pull the motor apart. Once there check the bearings and look for something that looks out of place. Post pictures before putting it back together, maybe someone here will notice something you might miss.
```

---
## \#12 Posted by: Sebike Posted at: 2017-09-22T12:03:33.629Z Reads: 116

```
Ok. I'm currently disassembling the motor. I checked connections and they're fine, however while running the motor at this lower speed where the "bumping" are present, I noticed that when supporting the motor with my fingers, the sound disappeared. 

Also, the moving part of the motor can be moved about 1 mm (that's how it was when I bought it), and maybe that's got something to do with it, or is it normal?

https://youtu.be/9o0UGmw8Hrc
```

---
## \#13 Posted by: Martinsp Posted at: 2017-09-22T12:07:11.869Z Reads: 113

```
That is either a bearing or the groove where the circlip is on the shaft that got worn and allow this movement. I checked mine and it moves too but significantly less. Take the motor apart and inspect the bearings, you unfortunately can not do it with the motor assembled.
```

---
## \#14 Posted by: Martinsp Posted at: 2017-09-22T12:08:51.926Z Reads: 109

```
Actually... Do you remember if there were any spacers between the bearings and the circlip? I have two pretty thin washers on there, maybe they broke and fell off which is now allowing the movement and vibrations, sounds etc.
```

---
## \#15 Posted by: Sebike Posted at: 2017-09-22T12:18:57.317Z Reads: 114

```
There were two spacers between the circlip and the bearing. Can't see any damage on them and as I mentioned, this is what it was like when I bought it new. 

Here are pictures from inside the motor. Magnets seem to have been rubbing/grinding against something. Can't tell if the copper winding is damaged as well?

<img src="/uploads/db1493/original/3X/d/1/d1a295957339dba884586786b0e9b5b5cbe543d5.JPG" width="281" height="500"><img src="/uploads/db1493/original/3X/d/1/d165c0fd57ef42069e3757f5b6589cb66d83276f.JPG" width="281" height="500"><img src="/uploads/db1493/original/3X/d/7/d7831210403ad3225fad5f7bfdb913c343b9b175.JPG" width="281" height="500"><img src="/uploads/db1493/original/3X/7/6/7690e7553cf0af851cfcc07fb79d4fee51b1dcaa.JPG" width="690" height="388"><img src="/uploads/db1493/original/3X/1/8/18469e772eea24b63d4e472a0c74a915df3e3501.JPG" width="690" height="388"><img src="/uploads/db1493/original/3X/c/9/c9b095eb8106956673e5b0d39064990d3b8fee16.JPG" width="690" height="388">
```

---
## \#16 Posted by: Martinsp Posted at: 2017-09-22T12:33:40.004Z Reads: 108

```
It looks pretty good. It might have been grinding or it is just dirt, dust and stuff on the magnets because it looks like you wiped it off on one of the pictures. The windings look good they are not so easy to damage since they are mostly covered with the steel stator itself. Wipe everything with a dry rag and if there are not any rocks or something like that inside the motor you can put it back together. Do those bearings spin freely? You can try that with your finger, press against the inner rotating part of the bearing and rotate it. If you dont feel any resistance or rough spots when rotating it thy should be good. 

My tip to assemble the motor is to twist some rag so that it is like a rope and put like a U turn around the stator near the motor mount. This is to slow the motor impact when you will be putting it back together. When you were disassembling the motor you had to overcome that magnetic force so this is going to pull the rotor of the motor to the steel stator. KEEP YOUR FINGERS AWAY. The rag is going to prevent the impact, afterwards just pull the rag out and reinstall the circlip pulley etc. There is nothing wrong as far as I can see with the motor.

Just to make sure please check if the motor mount screws are not touching the wire on the inside of the motor.
```

---
## \#17 Posted by: Martinsp Posted at: 2017-09-22T12:34:32.878Z Reads: 105

```
Have a close look at the magnets if any of them are not misplaced or lifted that would cause the rubbing sound
```

---
## \#18 Posted by: Sebike Posted at: 2017-09-22T12:35:20.225Z Reads: 110

```
It looks to me as if magnets have been touching the stators slightly. If so, that would explain why theres been this very slight repeated noise even before while rotating motor by hand. I could never find the source for that sound, but this might have been it. 

If it was the same noise, it has accelerated since, and maybe that bumping noise if from magnets very briefly touching stators and then letting them go because of the momentum?

Inspected copper wiring more closely with better lighting, and it looks fine I believe.
```

---
## \#19 Posted by: Martinsp Posted at: 2017-09-22T12:38:25.578Z Reads: 110

```
There is a very small gap between the stator and rotor, the smaller the gap the more precise the motor was made. When you wipe the magnets you would see scratches on them if what you are saying was happening. Minor scratches are OK but any major scratch is not good. That would mean that the magnet is slowly moving towards the stator.
```

---
## \#20 Posted by: Sebike Posted at: 2017-09-22T12:51:00.742Z Reads: 110

```
Reassembled the motor after cleaning it. Thanks for the tip on how to put the can back! Still got fingers attached to my hand :smile:  

Noise is still there, both the grinding and the bumping/knocking. 

https://youtu.be/8XGurxN26fI
```

---
## \#21 Posted by: Sebike Posted at: 2017-09-22T12:55:32.058Z Reads: 105

```
Didn't notice any major scratches on the magnets though, mostly dust being scratched off as you can see in the pictures and light marks. Seems like one more washer between bearing and circlip would have eliminated movement of the rotor. Bearings spinned freely.
```

---
## \#22 Posted by: Martinsp Posted at: 2017-09-22T12:59:38.920Z Reads: 107

```
:D 

Hmm that is strange. Do you feel any resistance or grinding when rotating by hand? What I am thinking now is that when the power cuts out for a moment i the noise might be the motor stopping and starting to rotate again. Same way as when you start the motor rapidly, that knock or whatever when it jumps from 0 to X rpm.

Can you connect the vesc to a computer and check the red current curve in real time data? if the motor is stopping the current should drop significantly or even to 0 and it should be in sync with the sound you hear. is that the case?
```

---
## \#23 Posted by: Sebike Posted at: 2017-09-22T13:05:38.539Z Reads: 105

```
Both sounds are gone if I support the rotor while the motor in running at low speed, so it must be the rotor moving either from side to side, up and down or both, making the magnets becoming slighlty misaligned to the stator. 

Another washer would hopefully take care of this issue, since it's that gap that allows movement of the can/rotor. Is this something you could help out with @fottaz ?
```

---
## \#24 Posted by: Martinsp Posted at: 2017-09-22T13:08:00.313Z Reads: 101

```
Forgot you said that. Try to put one more or as many washers as you can to make the motor move less. Hope it helps
```

---
## \#25 Posted by: Sebike Posted at: 2017-09-22T13:13:06.617Z Reads: 98

```
Sorry, didn't see this post. I'll check this later! Thanks
```

---
## \#26 Posted by: fottaz Posted at: 2017-09-22T14:54:22.866Z Reads: 92

```
Hey Sebastian!! That noise could happens when motor is not rotating 100% perfectly. 
It maybe hitted something? I had the same noise since a motor hitted the ground very bad
```

---
## \#27 Posted by: fottaz Posted at: 2017-09-22T15:19:37.117Z Reads: 94

```
The circlip is not tight too, it seems.
```

---
## \#28 Posted by: Sebike Posted at: 2017-09-22T15:23:17.538Z Reads: 94

```
Hi Alberto! Motor has never hit anything, so that wouldn't be the cause. No marks or dents suggesting any impact that I didn't notice either. 

Besides, there's been a slight noise since the beginning that sounded as if something grinded against some part of the motor once every turn of the motor (before board was ridden), so maybe it's that noise that has become worse. 

Anyway, I'm pretty sure the noise is due to the slight movement of the rotor along the shaft (the gap between the 2 washers and bearing is too big)  and it seems as eliminating the gap will make the motor run smoothly without noise.
```

---
## \#29 Posted by: Sebike Posted at: 2017-09-22T15:28:18.844Z Reads: 95

```
Yes. First and only time circlip has been removed was now when I disassebled the motor, so the videos that you see here are before I even touched that circlip.
```

---
## \#30 Posted by: fottaz Posted at: 2017-09-22T16:12:38.844Z Reads: 93

```
Just tell me as soon as possible if you have any issue, if that sound there was before don't hesitate to contact me!

If you fixed it by yourself all right, but when you need help on my products write me as soon as you can !
Thanks :slight_smile:
```

---
## \#31 Posted by: Sebike Posted at: 2017-09-22T16:33:40.203Z Reads: 92

```
Ok. I have sent you a pm. :slight_smile:
```

---
## \#32 Posted by: Sebike Posted at: 2017-09-23T16:18:10.428Z Reads: 91

```
Yes, I believe this is the case. Here is a printscreen from the realtime data. Each downward spike represents a "knock" in the motor. 

The grinding noise is gone which was due to the shaft having moved in the direction towards the pulley. After shaft was put back into a better position (I can no longer move the rotor in and out) that noise disappeared and motor runs smoother than ever before upto a certain low rpm where this knocking starts taking place. 

As before, if motor is supported from the bottom the knocking sound is gone as seen in this video.

The screeching noise is also still present at a certain higher rpm. <img src="/uploads/db1493/original/3X/6/0/60259603613695f496e6569908372e99b45ba219.gif" width="690" height="387">

https://youtu.be/OeOaxH7FzTQ
```

---
## \#33 Posted by: Sebike Posted at: 2017-09-23T18:42:19.922Z Reads: 88

```
@Martinsp any thoughts on what these current drops could be?
```

---
## \#34 Posted by: Martinsp Posted at: 2017-09-23T22:48:08.227Z Reads: 86

```
I am not really sure what could cause this problem. Has not happened to me yet. Maybe try changing the settings that caused this back and doing a motor detection again. Since this started happening since you changed settings. And see if there are any weak joints or failing cables just like with headphones where the cable is cutting the sound out sometimes before it fails completely.
```

---
## \#35 Posted by: Sebike Posted at: 2017-09-23T23:09:38.556Z Reads: 84

```
Oh ok. Settings were set back to the previous settings before I even started analyzing this issue, so there's nothing more to change back (unfortunately).

I'll check connections again, although there are not many that could fail right? I have phase wires and sensor wires coming out of the motor going directly to pre-soldered focbox wires via bullet connectors. Also, motor detection gave the same result as when I had no issues. 

And why these current cut-offs only when reaching a certain rpm?

Why are they gone when giving rotor bottoma slight push..?

Getting frustrated and don't want to use the board as long as motor acts this way.. HEEEELP! :joy: :fearful:
```

---
## \#36 Posted by: Martinsp Posted at: 2017-09-23T23:18:10.859Z Reads: 87

```
Now that you mention that it is sensored... sensores are used only until a certain RPM afterwards it is going sensorless because it is better. So sensors are for very low RPM performance only. Try turning the sensors off in the bldc tool. Check the cable precisely. 

I think you can use the board without problems because it seems like under load the motor runs just fine and on a skateboard it is under load constantly...
```

---
## \#37 Posted by: Sebike Posted at: 2017-09-23T23:30:06.214Z Reads: 84

```
That could be possible. Although I believe in FOC hybrid mode (?) sensors are only used until it reaches 2000 erpm and these knocks seems to appear above that at about 2700.

Will try switching sensored mode off though to see if it makes any difference.
```

---
## \#38 Posted by: Martinsp Posted at: 2017-09-23T23:33:16.410Z Reads: 84

```
You can set the "sensorless ERPM" in FOC motor config and the "general" part in the left corner.

I am pretty curious if that will make a difference. I think it will but who knows.
```

---
## \#39 Posted by: raven Posted at: 2017-09-26T14:49:06.094Z Reads: 77

```
You have good current flowing so I must be a mechanical fault. See if the motor gets unduly hot as it could be chaffing from the moving parts.
```

---
## \#40 Posted by: Sebike Posted at: 2018-10-07T06:23:59.522Z Reads: 42

```
Got some recent read on this thread, so it might be worth mentioning that the main problem with this motor was loose magnets.
```

---
