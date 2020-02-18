# Motor slipping, very LOW torque

### Replies: 37 Views: 1614

## \#1 Posted by: Mohammed Posted at: 2017-09-01T09:34:53.086Z Reads: 178

```
So I've read a couple of post similar to mine with some pretty convincing solutions which i have tried on my board but with no use. My problem is that the motor jitters and shakes on low throttle and on full ( i can stop the motor from spinning with my hand). on full the motor can barely pull the board let alone if i stand on it. i left a couple of screenshots of my configuration. I've already tried to change start up boost in the advanced tab in motor configuration (changed the value from 0.01-0.1, i was told to not go over 0.1). any ideas?<img src="/uploads/db1493/original/3X/8/e/8e89269dcea37b2a59668fc2127d75503dc56588.png" width="690" height="419"><img src="/uploads/db1493/original/3X/f/5/f5a290a66c72c410253818c149201d058f0d9e0a.png" width="690" height="419"><img src="/uploads/db1493/original/3X/3/7/373ae58b04c39b96f2695f3c21449dcd448bee72.png" width="690" height="419"><img src="/uploads/db1493/original/3X/5/5/55a02b18ed30bfa972337fa97b333782df28cd5f.png" width="690" height="419"><img src="/uploads/db1493/original/3X/f/3/f30381047cd117c77a2eadf5dc89b79b625ba06e.png" width="690" height="419"><img src="/uploads/db1493/original/3X/4/e/4e30609a6c27f1e47ce6dd2344d05efc912effcd.png" width="690" height="419">
My setup is:
-10S4P 18650 battery
-Turnigy SK3 6374 motor
-Enertion VESC-X 
-Enertion Nano-X remote
```

---
## \#2 Posted by: Skitzor Posted at: 2017-09-01T09:43:25.204Z Reads: 143

```
Does disabling traction control resolve the low end side ? Did you do motor detection ? (sorry to ask.)
```

---
## \#3 Posted by: Mohammed Posted at: 2017-09-01T10:04:38.678Z Reads: 138

```
I've done a motor detection yes, and i have entered the values for the IL & BEMF coupling.
if your referring to the traction control in the ADC tab in app configuration, it's off initially.
```

---
## \#4 Posted by: Skitzor Posted at: 2017-09-01T10:34:03.193Z Reads: 139

```
Looks like the current is not getting there. Try these battery settings. its for 10s3p. see if it helps, you probably can tune it further for 4p.<img src="/uploads/db1493/original/3X/f/8/f83d11278bbf71d00b2326d00b778d916f4bc7bb.PNG" width="690" height="393">

Edit: im referring to the voltage limits. you can leave the current limits
```

---
## \#5 Posted by: Mohammed Posted at: 2017-09-01T11:20:32.985Z Reads: 113

```
The values where also initially close to yours then I changed it in hopes it would work, besides I think the cut off you suggested is too low.
```

---
## \#6 Posted by: SirDiff Posted at: 2017-09-01T11:33:52.372Z Reads: 110

```
Liions can go down to 2.5V, 2.8 is good enough imho
```

---
## \#7 Posted by: Mohammed Posted at: 2017-09-01T11:58:16.077Z Reads: 106

```
okay, so i did try that configuration and still got the same results
```

---
## \#8 Posted by: TarzanHBK Posted at: 2017-09-01T12:03:10.552Z Reads: 107

```
Always leave your minimum input at 8V and your maximum input Voltage at 57V.

Do a new motor detection. If it works, hit Apply and then Write Configuration. Reboot your Vesc and see if something changed.
If your detection fails, you have to investigate further on your motor.
```

---
## \#9 Posted by: GrecoMan Posted at: 2017-09-01T12:07:32.544Z Reads: 102

```
Loosen your motor mount screws a bit and see what happens.  If that fixes your problem you just need shorter screws
```

---
## \#10 Posted by: TarzanHBK Posted at: 2017-09-01T12:08:25.417Z Reads: 99

```
Thats a good advice! A few others had problem with little shorts due to that!
```

---
## \#11 Posted by: GrecoMan Posted at: 2017-09-01T12:08:46.616Z Reads: 95

```
Haha yea, I was one of them 😉
```

---
## \#12 Posted by: Mohammed Posted at: 2017-09-01T12:09:19.514Z Reads: 100

```
i returned the values and did a detection test, but still no use. the detection was successful by the way
```

---
## \#13 Posted by: Mohammed Posted at: 2017-09-01T12:12:27.887Z Reads: 99

```
I just tried that, but still no use. But can one of you guys explain how that screws could be the issue? if your talking about the screws gripping on to the shaft or stator then its not, i can clearly see a big gap around both screws, everything is far away from them.
```

---
## \#14 Posted by: GrecoMan Posted at: 2017-09-01T12:14:23.303Z Reads: 99

```
If the screws touch the windings in the motor, the motor will short.  There would not be enough power going to the motor to make it spin fast.  The screws would essentially be robbing the motor of voltage
```

---
## \#15 Posted by: Mohammed Posted at: 2017-09-01T12:16:39.109Z Reads: 96

```
if thats the case, then I'm pretty sure I'm safe from that.
```

---
## \#16 Posted by: GrecoMan Posted at: 2017-09-01T12:18:22.564Z Reads: 92

```
Hmmm, maybe look take a look inside your motor while your spinning it.  If there's a spark I guarantee that's your problem. Watch all 4 of the mount screws to see if there is any sort of spark around them.
```

---
## \#17 Posted by: Mohammed Posted at: 2017-09-01T12:21:16.007Z Reads: 93

```
unless the sparks are really tiny or invisible, i couldn't spot anything
```

---
## \#18 Posted by: GrecoMan Posted at: 2017-09-01T12:22:26.676Z Reads: 86

```
Hmm alright, the sparks are relatively large so that probably isn't the reason.  You said your motor detection worked right?
```

---
## \#19 Posted by: Deckoz Posted at: 2017-09-01T12:22:36.950Z Reads: 85

```
Friend of mine got brand new motors and the set screws on the shaft to bell were stripped allowing the shaft to spin around the pressed on bell. 

Have you checked your shaft to bell set screws?
```

---
## \#20 Posted by: Mohammed Posted at: 2017-09-01T12:23:58.842Z Reads: 86

```
Yup, pretty smooth too.<img src="/uploads/db1493/original/3X/d/c/dcd02fa106200c8b3a45a225b1d9b6a99c61edca.png" width="690" height="89">
```

---
## \#21 Posted by: Mohammed Posted at: 2017-09-01T12:25:08.640Z Reads: 82

```
sorry, didn't really get what your trying to say?
```

---
## \#22 Posted by: TarzanHBK Posted at: 2017-09-01T12:25:19.335Z Reads: 81

```
And you hit Apply, Write Configuration and then reboot and still nothing?
```

---
## \#23 Posted by: Mohammed Posted at: 2017-09-01T12:25:43.441Z Reads: 80

```
Yup, still nothing
```

---
## \#24 Posted by: TarzanHBK Posted at: 2017-09-01T12:29:19.955Z Reads: 76

```
Hmm then I´ve no idea...:confused:
```

---
## \#25 Posted by: NickTheDude Posted at: 2017-09-01T14:18:09.254Z Reads: 72

```
I guess you could try typing "faults" in the console to see if anything comes up.
```

---
## \#27 Posted by: Deckoz Posted at: 2017-09-01T15:16:31.067Z Reads: 68

```
you said the board doesn't really move/motor is slipping..

the shaft is pressed into the bellhousing(the can that spins), the pressed in part is on the end that is not mounted to the motor mount... on that end there are set screws/grub screws to hold the shaft from spinning on the bellhousing. 

You may have to remove the bell with shaft to see the set screws as some are internal. I was suggesting to check these to ensure the shaft isnt spinning in the bell...
```

---
## \#28 Posted by: Jinra Posted at: 2017-09-01T15:28:14.152Z Reads: 66

```
A video of the issue would be helpful.

@Mohammed oh btw, if you're running a single turn off "Multiple ESCs over CAN" and "Send status over CAN"
```

---
## \#29 Posted by: Mohammed Posted at: 2017-09-02T01:05:06.519Z Reads: 59

```
I can't upload the video on to YouTube for some reason. I will though when I can.
My problem is quite simple, the outer case and the shaft spin fine, but the moment I add a load ie my hand or my weight, it starts jittering, like there's not enough power getting to the motor
```

---
## \#30 Posted by: itsmikeholland Posted at: 2017-09-02T05:20:45.153Z Reads: 56

```
who made your battery? maybe the issue is there?
```

---
## \#31 Posted by: Mohammed Posted at: 2017-09-02T05:35:31.097Z Reads: 56

```
Made it my self, I'm getting proper 10s battery readings though, 42v when full charged. I doubt it's the battery
```

---
## \#32 Posted by: Mohammed Posted at: 2017-10-17T09:17:56.045Z Reads: 48

```
https://www.youtube.com/watch?v=NBxj477-cIQ
```

---
## \#33 Posted by: Jinra Posted at: 2017-10-17T15:32:22.859Z Reads: 39

```
Looks good, you'll need sensors if you want smooth startup from standstill.
```

---
## \#34 Posted by: onepunchboard Posted at: 2017-10-17T16:42:00.881Z Reads: 37

```
it's normal.
```

---
## \#35 Posted by: Mohammed Posted at: 2017-10-17T21:03:52.158Z Reads: 32

```
I'm sorry, but I don't understand how that's normal? When I stand in the board it can't move at all...
```

---
## \#36 Posted by: Mohammed Posted at: 2017-10-17T21:04:28.413Z Reads: 33

```
Can you explain further please?
```

---
## \#37 Posted by: Jinra Posted at: 2017-10-17T21:04:31.554Z Reads: 34

```
That's normal for a board without sensors, you have to give it a kick push before throttling.
```

---
## \#38 Posted by: Clonkex Posted at: 2017-10-18T05:36:25.111Z Reads: 25

```
It's still possible there's something wrong, but it definitely looks like it's fine based on the video. Unsensored brushless motors don't work very well at all until they're spinning a bit. Get on the board, give it a push (the old fashioned way, with your foot), then apply some throttle and see if it pulls you.
```

---
