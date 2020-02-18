# Help! the motor can&rsquo;t handle the board weight

### Replies: 30 Views: 3814

## \#1 Posted by: tueboard Posted at: 2016-08-21T15:27:24.824Z Reads: 230

```
hi,

recently i've build my first electric skate but something is wrong, if i put the skate on the floor i can listen the motor but the board doesn't move forward, but if i flip up it the motor is working and the wheel is spinning fine.

i put two lipo batteries 5500mah 11.1v 35c etc in series and both are fully charged.

the motor and the VESC are from enertion, i bought this kit
http://www.enertionboards.com/diy-electric-skateboard-kits/enertion-single-motor-mount-pro-kit/

the VESC has the default setup, i didn't change anything.

i've recorded a video, as you can see if the wheel don't have any weight on it it works ok, but if i put only my hand without pushing the motor doesn't have power to spin the wheel.
https://www.youtube.com/watch?v=7lR5SZCvT24

if i put the board in the floor and i push it a little bit with inertia it moves slightly but it does not run so fast.

i don't know what is wrong..
- the batteries are not powerful enough?
- the VESC default settings are wrong?
- the cables to connect the two batteries in series with the VESC are 14 AWG not 12 AWG maybe this is wrong?
- the Torque Belt has te be very hard-tight?

any idea? please some help
```

---
## \#2 Posted by: mason Posted at: 2016-08-21T15:31:29.675Z Reads: 210

```
please show us your VESC settings.
```

---
## \#3 Posted by: JohnnyMeduse Posted at: 2016-08-21T15:55:25.912Z Reads: 203

```
Have you done a Motor detection in the BLDC TOOL ?
```

---
## \#4 Posted by: JLabs Posted at: 2016-08-21T15:58:31.858Z Reads: 204

```
[quote="miquelcamps, post:1, topic:8053"]
- the batteries are not powerful enough?
[/quote]

22v is perfectly fine, many people run that with a VESC. A higher voltage will give you more power / top speed[quote="miquelcamps, post:1, topic:8053"]

- the cables to connect the two batteries in series with the VESC are 14 AWG not 12 AWG maybe this is wrong?

[/quote]
14AWG should be fine. [quote="miquelcamps, post:1, topic:8053"]
- the Torque Belt has te be very hard-tight?
[/quote]
The belts looks a little lose, buy I cant tell. You dont want it to be too tight or the motor will have problems. Some pictures would help to decide if the belt should be tightened or stay as is
```

---
## \#5 Posted by: itsmikeholland Posted at: 2016-08-21T16:08:57.745Z Reads: 188

```
I don't know how much resistance you're applying to the wheel, but maybe you need to fix the motor pulley to the motor? Either a keyway or a grubscrew, i think its called.
```

---
## \#6 Posted by: TarzanHBK Posted at: 2016-08-21T16:14:37.099Z Reads: 183

```
your belt is far too loose and you have to do a initial motor detection with your vesc
```

---
## \#7 Posted by: tueboard Posted at: 2016-08-21T16:29:48.484Z Reads: 181

```
sorry i'm noob, i've installed BLCD tool on a mac, i plug the vesc with the computer, can't see it in serial connection of BLCD tool, i've to install some firmware or something?

i've connected the vesc to the batteries and the motor, the blue light is on.

i've to do something with the firmware folder?

thanks
```

---
## \#8 Posted by: crameur Posted at: 2016-08-21T16:34:32.915Z Reads: 169

```
http://www.electric-skateboard.builders/t/vesc-faq-motor-detection-step-by-step-guide/500
```

---
## \#9 Posted by: JohnnyMeduse Posted at: 2016-08-21T16:36:47.173Z Reads: 164

```
Just push connect, if it does't work try the refresh button, then you should be able to see the VESC a connect to it.

**also, I strongly suggest that you read on the basic of the  vesc before even riding it.**
```

---
## \#10 Posted by: JohnnyMeduse Posted at: 2016-08-21T16:39:26.636Z Reads: 161

```
http://www.electric-skateboard.builders/t/vesc-faq-easy-vesc-configuration-in-windows-mac-for-noob/2963
```

---
## \#11 Posted by: TarzanHBK Posted at: 2016-08-21T17:42:51.627Z Reads: 153

```
the vesc is not a plug and play tool! you have to set it up, or you may fry it!
```

---
## \#12 Posted by: tueboard Posted at: 2016-08-21T17:52:19.938Z Reads: 147

```
it's weird i've used a mini usb-usb cable that i use to charge the gopro but it doesn't work with the VESC, tomorrow i will buy another cable, i hope it works.. BTW thank you
```

---
## \#13 Posted by: ra.rend Posted at: 2016-08-21T18:10:54.693Z Reads: 140

```
Gopro uses "micro" usb, vesc has "mini" usb
```

---
## \#14 Posted by: paul775 Posted at: 2016-08-21T18:17:48.934Z Reads: 139

```
I used the ps3 wire that charges the controller. Worked perfectly from mac to VESC
```

---
## \#15 Posted by: tueboard Posted at: 2016-08-21T18:21:26.448Z Reads: 137

```
my enertion vesc has a micro usb like gopro, but it's weird my pc doesn't recognize the vesc
http://www.enertionboards.com/electric-skateboard-parts/vesc-standard/
```

---
## \#16 Posted by: lox897 Posted at: 2016-08-21T20:19:55.396Z Reads: 131

```
Try a different cable. Your belt tension is way to loose, it looks like it is skipping most teeth.
```

---
## \#17 Posted by: Namasaki Posted at: 2016-08-21T22:01:46.283Z Reads: 137

```
Another point that I don't think was mentioned is that you need to calibrate your remote/receiver with the Vesc using the bldc tool. 
https://www.youtube.com/watch?v=OtuofrQr3F8&feature=share
```

---
## \#18 Posted by: tueboard Posted at: 2016-08-22T17:30:37.418Z Reads: 130

```
finally with another micro usb cable my computer detects the vesc in the BLDC tool, i followed some VESC setup youtube videos and i tensed the motor belt, but my board can't move.

https://www.youtube.com/watch?v=UzcHxpHMxyM

i think that the motor goes a little bit faster than before, also i tried to get on the board and push but it's slow like a turtle.

i repeat, my setup is the following motor and 2x batteries connected in series 5500mah, 11.1v, 35c both full charged
http://www.enertionboards.com/diy-electric-skateboard-kits/enertion-single-motor-mount-pro-kit/

i attach you some BLDC tool's screenshots if someone can tell me what is wrong?

<img src="/uploads/db1493/original/2X/3/38858702bebbe720e28bd99c0276aa69ebd7ee93.png" width="690" height="409">

<img src="/uploads/db1493/original/2X/e/e253ffa9adecc907d047cc7e1b665b5997e3f48e.png" width="690" height="406">

<img src="/uploads/db1493/original/2X/5/5aaaa72b150c94b1340ccb440a837a29140c7acb.png" width="690" height="404">

<img src="/uploads/db1493/original/2X/e/eccaad3e6f37e5b5dbb5b282863917505a701fd7.png" width="690" height="406">

<img src="/uploads/db1493/original/2X/3/3f696fc18be216c411074907ce077c55836e757e.png" width="690" height="395">

<img src="/uploads/db1493/original/2X/a/aa912bda3e45d409fd70f64c23a84c4fc665aa33.png" width="690" height="407">

this is my controller setup flysky FS-GT2B

ST (down)
TH (down)
ST.TRIM 0
TH.TRIM 1
ST.D/R 100

<img src="/uploads/db1493/original/2X/c/c895b8234ebbcef192bab03fcf692a68a6bc154d.jpg" width="375" height="500">

<img src="/uploads/db1493/original/2X/6/677184777e4aadf5fa1b93feae784f9b10d3ead2.jpg" width="375" height="500">


thanks
```

---
## \#19 Posted by: devin Posted at: 2016-08-22T17:38:38.516Z Reads: 126

```
<p>This post was flagged by the community and is temporarily hidden.</p>
```

---
## \#20 Posted by: JohnnyMeduse Posted at: 2016-08-22T18:25:15.091Z Reads: 121

```
Have your run motor détection?? Are you setup for sensor or sensor less??
```

---
## \#22 Posted by: tueboard Posted at: 2016-08-22T18:53:50.431Z Reads: 122

```
I've attached the VESC settings, thank you
```

---
## \#23 Posted by: tueboard Posted at: 2016-08-22T18:54:47.864Z Reads: 122

```
Yes, 

i clicked the motor detection, the wheel is spinning but in the BLDC tool appears the message detection failed, any idea?


About sensorless in the BLDC 5th screenshot i selected sensor less.
```

---
## \#24 Posted by: JohnnyMeduse Posted at: 2016-08-22T19:05:41.176Z Reads: 122

```
After... You need to do apply and write
```

---
## \#25 Posted by: JohnnyMeduse Posted at: 2016-08-22T19:07:12.258Z Reads: 128

```
You have A problem... Specialy I you try to run without detection
```

---
## \#26 Posted by: JohnnyMeduse Posted at: 2016-08-22T20:33:27.744Z Reads: 134

```
Do  you have any Picture of the motor connection. And have you send a e-mail to enertionsupport
```

---
## \#27 Posted by: tueboard Posted at: 2016-08-23T01:27:53.018Z Reads: 130

```
hi again,

i've tried some vesc settings to check if BLDC tool can detect the motor.

**settings number 1**

<img src="/uploads/db1493/original/2X/d/dfbccae4edaf228126a917d5f718132adf4fd05b.png" width="690" height="293">

i get this settings from this thread
http://www.electric-skateboard.builders/t/vesc-motor-detection-failing/6640/11?u=miquelcamps

motor detection result: detection failed (the wheels are spinning with the tool and the controller)

video skate on the floor v1
https://www.youtube.com/watch?v=UzcHxpHMxyM

Motor settings v1 - BLDC motor detection
https://www.youtube.com/watch?v=waPHd6NzyqQ

Motor settings v1 with controller
https://www.youtube.com/watch?v=Zb1n-KYhpYs


**settings number 2**

<img src="/uploads/db1493/original/2X/d/d6ed310f5c6601e713d80f7fc368ef25e2664eef.png" width="690" height="298">

i get this settings from @onloop youtube vídeo (i think his motor and vesc are the same as mine)
https://www.youtube.com/watch?v=XSBX0dyq-oU

motor detection result: 
Detection results:
Integrator limit: 108.62
BEMF Coupling: 699.49

Hall sensor detection failed: 
-1, -1, -1, -1, -1, -1, -1, 3


video skate on the floor v2
https://www.youtube.com/watch?v=DYpeveRl7_Q

Motor settings v2 - BLDC motor detection
https://www.youtube.com/watch?v=16M8B7vCrtI

Motor settings v2 with controller
https://www.youtube.com/watch?v=B5L3I_4l_qw


@JohnnyMeduse this is a short video of my setup
https://www.youtube.com/watch?v=t18XBp_6TLE


**some questions**

1- about the settings 2 what does it means the error "Hall sensor detection failed: -1, -1, -1, -1, -1, -1, -1, 3" ? what i can do to solve that?

2- i've tried to stand up on the board with settings 2 and i don't feel safe, it's normal that the skate starts running so fast? what i've to change from settings 2 to start slow as the settings 1?

3- can i burn/break the vesc or motor with the settings 2? which are the best vesc settings to prevent that and be safe?


thank you so much! i'm happy today to see some progress :D a few days ago i felt like i put the money in the trash haha
```

---
## \#28 Posted by: JohnnyMeduse Posted at: 2016-08-23T01:37:01.966Z Reads: 117

```
Thanks and on problem et are here  to help 😊, and you did most of the work 🖐
Also, try the batt max at 45, batt min at -12 and max Erpm at 70000 (this should help Protect the vesc)
```

---
## \#29 Posted by: Blasto Posted at: 2016-08-23T02:21:24.402Z Reads: 114

```
[quote="miquelcamps, post:27, topic:8053"]
some questions

1- about the settings 2 what does it means the error "Hall sensor detection failed: -1, -1, -1, -1, -1, -1, -1, 3" ? what i can do to solve that?
[/quote]

No problem there, you have sensorless motors, thus no hall sensors. Nothing to detect
```

---
## \#30 Posted by: tueboard Posted at: 2016-08-23T18:34:49.696Z Reads: 105

```
sorry, one more question..

if i change the max erpm to 70000, i have to change the min erpm to -70000 ?

thanks
```

---
## \#31 Posted by: JohnnyMeduse Posted at: 2016-08-23T19:29:58.874Z Reads: 100

```
Only if you want to be a wild card and use it in reverse 😜
```

---
