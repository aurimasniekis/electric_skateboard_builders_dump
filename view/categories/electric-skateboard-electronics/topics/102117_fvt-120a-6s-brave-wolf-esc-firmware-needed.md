# Fvt 120a 6s Brave Wolf ESC Firmware needed

### Replies: 20 Views: 250

## \#1 Posted by: Baumeister_RHGB Posted at: 2019-09-23T11:52:50.062Z Reads: 44

```
Hi, I am working on my second Board and decided to get the FVT 120a ESCs and upload new firmware to them. The original firmware was the 190710, an on the Computer it shows as V2.00_190710.
I then uploaded the Brakeline firmware from their website (V1.00_161214) and since then I can't get the ESC to work properly. It won't spin the motors anymore but does accept the throttle input when doing a throttle calibration. This only works when uploading the firmware and not changing any setting, else even the throttle calibration won't work. the ESC does beep with the motors tho. They are no shorts and the Voltage should be within normal limits as im using a 5s pack rn to test but will go up to 6s. The red and green Led are both on and not blinking and im running uncensored.

I assume the problem is bc of a different Bootloader (read this in another discussion) and bc of the different versions.

Does anyone have a firmware that has the V2? You can only see the versions in the program btw.
Is there another solution or another firmware that works on it?

I really want the brakeline firmware as I read it works really well but the normal firmware is preferable if thats the only one working.
```

---
## \#2 Posted by: Baumeister_RHGB Posted at: 2019-10-09T07:41:40.778Z Reads: 24

```
Noone?
The board is done and I just need the firmware to get it going. Too bad.
```

---
## \#3 Posted by: Tamatoa Posted at: 2019-10-09T07:59:15.547Z Reads: 24

```
Hi, I don’t have the firmware but @whaddys was talking about being able to locate firmwares for the 12s version on the other forum. Maybe he can help you although I am not sure. Ask your question there too I know some of the regulars stopped coming here.
```

---
## \#4 Posted by: Baumeister_RHGB Posted at: 2019-10-09T08:40:24.029Z Reads: 21

```
Thanks a lot I'll try that. 
I didn't even think about going there as I thought this forum would go to normal since onloop "left".
Once again, thanks a lot
```

---
## \#5 Posted by: whaddys Posted at: 2019-10-09T12:51:16.797Z Reads: 19

```
@Baumeister_RHGB I gotchyu bro bro http://szfvt.com/en/download-25-5-6-6.html

Also super helpful video:
https://www.youtube.com/watch?v=xQCT_84BGzI&t=459s
```

---
## \#6 Posted by: Baumeister_RHGB Posted at: 2019-10-09T13:08:37.226Z Reads: 18

```
Thank you.
The problem is that I tried both the 6s versions from this page. Downloaded em there but both won't work. I also don't think it's an throttle calibration issue as they both worked fine before with the stock firmware. When I uploaded the firmware I also can just do the the throttle calibration when I upload the firmware and don't change any settings.
```

---
## \#7 Posted by: Okami Posted at: 2019-10-09T13:13:21.903Z Reads: 19

```
I know someone had FVT engineers skype contact, u should search more. But it might be that once u go to brake line firmware u cant really go back, but check more what others have done maybe it is reversible, otherwise u are in bad position if nothing works
```

---
## \#8 Posted by: Baumeister_RHGB Posted at: 2019-10-09T13:31:29.929Z Reads: 19

```
I'm sorry I should have given more insight. I already contacted FVT via Skype and email. I didn't hear back through the email and in Skype it still says they (she) has to accept the message. I have read once that you can't go back but only if you go to a 12s firmware on the 6s ESC.  The last I read for the brakeline firmware is that I works with the ESC. I have a few hours into googling now and haven't found the firmware nor anything about the V2 bootloader except for one post, but idk where or what it says anymore.
```

---
## \#9 Posted by: Baumeister_RHGB Posted at: 2019-10-09T13:35:19.368Z Reads: 19

```
The Skype contact is also on there website if someone needs it
```

---
## \#10 Posted by: Okami Posted at: 2019-10-09T14:29:31.135Z Reads: 19

```
@Idea might have the firmwares?
```

---
## \#11 Posted by: Okami Posted at: 2019-10-09T17:03:27.604Z Reads: 16

```
@kaspars 

https://www.electric-skateboard.builders/t/fvt-firmware-update-psa-make-sure-you-have-the-right-firmware/8463/28
These no good ?
```

---
## \#12 Posted by: Idea Posted at: 2019-10-09T17:13:54.853Z Reads: 16

```
I haven't updated my ESC for 3 years, I don't have the latest firmware version
```

---
## \#13 Posted by: Baumeister_RHGB Posted at: 2019-10-09T17:21:20.630Z Reads: 17

```
I don't think so sadly. After looking at the firmware and the cell count I came to the conclusion, that the versions starring with 16 are for 6s and these with 17 for 12s. The versions kaspars has there are for 6s and 12s, so I tried the one with 16 and it didn't work.
```

---
## \#14 Posted by: Baumeister_RHGB Posted at: 2019-10-09T17:21:45.093Z Reads: 16

```
Has anyone maybe tried the 12s version on a 6s ESC and it worked?
```

---
## \#15 Posted by: whaddys Posted at: 2019-10-10T14:24:46.818Z Reads: 14

```
I would just try doing everything exactly like in the video I posted and see if it works.
```

---
## \#16 Posted by: Baumeister_RHGB Posted at: 2019-10-11T17:25:13.553Z Reads: 14

```
Tried it again now. The problem is the ESC won't even start beeping. It was able to calibrate the throttle bevor the update. Now it doesn't anymore. The throttle was set to 1500μs (midpoint), which is the most common way why it won't work. The receiver and transmitter are also paired.
```

---
## \#17 Posted by: Baumeister_RHGB Posted at: 2019-10-11T17:33:05.448Z Reads: 13

```
![IMG_20190917_161245|374x500](upload://ljQ28FdoEMcuik4MKl6oOHyIT8a.jpeg) ![IMG_20190917_161426|374x500](upload://p5Wd7cEwGYHLicpp71jn1YJhqn8.jpeg) 

These are the pictures of the firmware in the program. I also assume the first numbers have to do smth with the date the firmware is published. 
Lots of conspiracy going around in my head and the meaning of the firmware names lol.
```

---
## \#18 Posted by: Baumeister_RHGB Posted at: 2019-10-25T10:16:12.481Z Reads: 9

```
Did some more just now. I uploaded the 16124 firmware and without changing any setting I started the ESC up and pulled the trigger all the way (somehow it doesn't matter if its all the way negative or positive). The ESC then beeped and I could get the wheel to spin. SUCCESS. 
BUT I can't change any setting or it won't work anymore. If I brake it sometimes works again and sometimes stops working (maybe if I go over a certain throttle level?). I also couldn't do the throttle calibration.
```

---
## \#19 Posted by: Baumeister_RHGB Posted at: 2019-10-26T18:51:19.599Z Reads: 6

```
And did even more, as I got motivated by my previous "success". The ESC only works if one doesn't touch the settings nor does a throttle calibration.
As for now: Both work, but I can't have the settings the way I want them to. And one ESC has its throttle midpoint a smitch before the other, so it starts a bit earlier. I'll see if that's a problem or is okay like this.
If anyone needs a firmware hit me up, I collected quite a few by now.
```

---
## \#20 Posted by: Baumeister_RHGB Posted at: 2019-10-26T18:58:19.038Z Reads: 6

```
I tried this too and the ESC behaves weirdly. It brakes the motor at midpoint and somewhat stutters when I try to accelerate. It didn't get the motor to spin tho.
Don't recommend this.
```

---
