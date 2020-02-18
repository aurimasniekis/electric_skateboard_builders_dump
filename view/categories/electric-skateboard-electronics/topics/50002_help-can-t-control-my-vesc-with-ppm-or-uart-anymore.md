# HELP - Can’t control my VESC with PPM or UART anymore

### Replies: 54 Views: 1318

## \#1 Posted by: ElskerShadow Posted at: 2018-03-24T11:47:24.783Z Reads: 114

```
After recieving my new module for the photon I finally decided to install it.. little I knew i should have not ! Now i tried 3 different remotes and nothing works. 
I typed faults looking for errors 
Tried with and without CANbus 
With PPM and UART 
I just can’t get the motors to spin and i can’t see any pulsewidth displayed on the BLDC tool 

Please help me I have a group ride in a few hours it’s the first day of sun since decades ! 
![image|677x499](upload://pPxEJxRY211SLrnfoAKnmb23DPA.jpeg)![image|382x500](upload://fiAf3QO3DdRxRObEIb15niliMdz.jpeg)
```

---
## \#2 Posted by: rey8801 Posted at: 2018-03-24T11:52:08.419Z Reads: 100

```
That sucks! I am sorry for that. I hope someone can help you asap.

Otherwise one thing you can try is upgrade to the 3. Firmware. Either the normal one or Ackmaniac ( I am using the latest one). Then use VESC tool instead of BLDC tool for configuration. Maybe it will work out.
```

---
## \#3 Posted by: ElskerShadow Posted at: 2018-03-24T11:57:47.207Z Reads: 101

```
I ll try that, i have no other choice so....
```

---
## \#4 Posted by: rey8801 Posted at: 2018-03-24T11:58:25.436Z Reads: 100

```
If you never use it and needs help just let me know. I did it 2 days ago
```

---
## \#5 Posted by: ElskerShadow Posted at: 2018-03-24T11:58:28.202Z Reads: 99

```
But i m not sure the 3 firmware is supported by the photon
```

---
## \#6 Posted by: rey8801 Posted at: 2018-03-24T11:59:35.784Z Reads: 97

```
You should check inside thier thread. I mean is the most advance one, it should be able to. Otherwise it worth a try and you can use another remote for today.
```

---
## \#7 Posted by: ElskerShadow Posted at: 2018-03-24T11:59:49.228Z Reads: 93

```
I m not sure about how to upgrade my vesc either
```

---
## \#8 Posted by: rey8801 Posted at: 2018-03-24T12:00:21.195Z Reads: 92

```
that I can help I did it 2 days ago...it's all inside the VESC tool
```

---
## \#9 Posted by: RedEagle Posted at: 2018-03-24T12:00:32.082Z Reads: 86

```
What vesc are you using? your erpm limit seems way too high.
```

---
## \#10 Posted by: ElskerShadow Posted at: 2018-03-24T12:01:01.145Z Reads: 89

```
FOCBOX 
I let the erpm how it was can’t remember the limits
```

---
## \#11 Posted by: ElskerShadow Posted at: 2018-03-24T12:01:57.880Z Reads: 90

```
There’s no vesc tool for mac...
```

---
## \#12 Posted by: RedEagle Posted at: 2018-03-24T12:02:13.971Z Reads: 90

```
max 60.000 min -60.000
Although focbox is known to handle more than that. I doubt you'll exceed 60k with that motor of yours.
```

---
## \#13 Posted by: rey8801 Posted at: 2018-03-24T12:03:00.083Z Reads: 87

```
Ackmaniac yes https://www.dropbox.com/sh/t7dl90owz5ccbyl/AAANyC-yQCMeveA7errNRnYqa?dl=0
download the ESC tool folder. Inside one is for Windows the other for mac.
```

---
## \#14 Posted by: GrecoMan Posted at: 2018-03-24T12:03:31.699Z Reads: 86

```
don’t upgrade. i’ve heard nothing but problems about 3.xx. reflash the vesc with your current fw. in the firmware tab of the bldc tool. redo all your settings and give it a shot.

btw erpm should be set to 60k just to be safe, also uncheck “limit erpm with negative torque”
```

---
## \#15 Posted by: GrecoMan Posted at: 2018-03-24T12:04:09.752Z Reads: 81

```
please use commas lol.

60.000 is much different than 60,000
```

---
## \#16 Posted by: ElskerShadow Posted at: 2018-03-24T12:04:25.447Z Reads: 81

```
God Photon pisses me off so hard, nothing but problems with it since i have it.. i won’t struggle much more if i can’t make it work i ll ressell i have lost enough time with this shit already...
```

---
## \#17 Posted by: ElskerShadow Posted at: 2018-03-24T12:04:33.174Z Reads: 81

```
Thanks i ll do that now
```

---
## \#18 Posted by: RedEagle Posted at: 2018-03-24T12:05:45.968Z Reads: 80

```
The message still comes across the same, no?
```

---
## \#19 Posted by: GrecoMan Posted at: 2018-03-24T12:05:48.031Z Reads: 81

```
make sure you choose 412 in the firmware files, you’ll know what i’m talking about when you get to it
```

---
## \#20 Posted by: GrecoMan Posted at: 2018-03-24T12:06:13.896Z Reads: 94

```
it took me a few times reading it to realize you meant 60000 instead of 60
```

---
## \#21 Posted by: ElskerShadow Posted at: 2018-03-24T12:06:51.813Z Reads: 91

```
![image|666x500](upload://9RA4NHCo0I3H2ak9QEmyEZhpp6H.jpeg)
```

---
## \#22 Posted by: scepterr Posted at: 2018-03-24T12:08:09.196Z Reads: 89

```
Need to use the Extended BLDC Tool, don't know if there's a Mac version
```

---
## \#23 Posted by: GrecoMan Posted at: 2018-03-24T12:08:50.663Z Reads: 87

```
![image|665x500](upload://cNHzBOxT12UDR9YaZmpojsi7G7D.jpeg)
```

---
## \#24 Posted by: ElskerShadow Posted at: 2018-03-24T12:09:02.444Z Reads: 82

```
I just don’t get why plugging the photon remote would make all my vesc freak out ?????
```

---
## \#25 Posted by: ElskerShadow Posted at: 2018-03-24T12:09:45.640Z Reads: 79

```
I got the selecting part but i don’t have the firmware on my computer and i can’t find it on the vesc website
```

---
## \#26 Posted by: scepterr Posted at: 2018-03-24T12:10:17.645Z Reads: 80

```
Yeah that's a bit weird, I would write default app config, reboot and resetup app config, reboot, check
```

---
## \#27 Posted by: GrecoMan Posted at: 2018-03-24T12:10:30.703Z Reads: 78

```
wait did you plug it into the right port?
```

---
## \#28 Posted by: scepterr Posted at: 2018-03-24T12:10:57.510Z Reads: 77

```
Lol that would be funny..
And to the correct side of the correct port..
```

---
## \#29 Posted by: ElskerShadow Posted at: 2018-03-24T12:11:59.682Z Reads: 76

```
I plugged it in the uart port 
![image|375x500](upload://5gmC97KEpB3YgrAD9HPSoQeQ9bl.jpg)
```

---
## \#30 Posted by: scepterr Posted at: 2018-03-24T12:13:39.648Z Reads: 77

```
I would be careful holding it barehanded unless it's coated, could easily static shock it or even short across your skin
```

---
## \#31 Posted by: RedEagle Posted at: 2018-03-24T12:13:47.992Z Reads: 78

```
[quote="Wajdi, post:635, topic:24654"]
I have been looking into this for the past few days, and I found the problem. I forked the bldc source code and applied necessary changes to get this working again. I will release a modified FW 3.34 tonight that should get cruise control, reverse, and nunchuck controls back on UART.
[/quote]

[quote="Wajdi, post:637, topic:24654, full:true"]
I just managed to have the controls compatibility issue fixed. The modified version is FW 3.35, thats the latest release, I made changes to fix nunchuck compatibility issues with the Photon receiver.

You can download the FW from my GitHub here https://github.com/wajdib/bldc/tree/master/build_all

Make sure to choose the correct hardware version, and the default FW available.

For this you will need the latest version of the VESC TOOL as well, V0.88.

This also applies to anyone that wants to update to latest vesc versions and have problems with controls or telemetry, this should fix it for the old Photon receivers.

Let me know if this works for you.
[/quote]


[quote="Dizzee, post:636, topic:24654"]
For those that need it and can make use of it, here’s a link to the previous releases of VESC Tool for MAC OS. [MAC VESC Tool Releases](https://github.com/rpasichnyk/vesc_tool/releases)
[/quote]

Did you download the modified firmware?
```

---
## \#32 Posted by: GrecoMan Posted at: 2018-03-24T12:16:41.853Z Reads: 74

```
can i see a picture of your app configuration?
```

---
## \#33 Posted by: trancejunkiexxl Posted at: 2018-03-24T12:21:02.577Z Reads: 74

```
Check the cables one time I had them backwards at the rx side, took me awhile to notice.. I was losing my marbles

Looks like u tried that nvm 🤐
```

---
## \#34 Posted by: ElskerShadow Posted at: 2018-03-24T12:21:57.268Z Reads: 74

```
![image|686x500](upload://zkfSn7NBd86QCEH38vuiVByvjG.jpeg)
```

---
## \#35 Posted by: ElskerShadow Posted at: 2018-03-24T12:23:27.515Z Reads: 76

```
No i did not and was not aware of this issue. I will update my VESC with it and tell you if it works ! Hope it will
The weird thing is that even the gt2b don’t work anymore. 
Thanks for the mac version of the vesc tool
So i just should download vesc tool update the firmware re do all the parameters , motor detection etc
```

---
## \#36 Posted by: GrecoMan Posted at: 2018-03-24T12:24:46.359Z Reads: 76

```
the gt2b shouldn’t work anymore, you set it to uart only.
```

---
## \#37 Posted by: ElskerShadow Posted at: 2018-03-24T12:25:26.672Z Reads: 76

```
I m not that stupd bro, when i plug the gt2B i swith to PPM
```

---
## \#38 Posted by: RedEagle Posted at: 2018-03-24T12:25:49.903Z Reads: 75

```
A quick search in the Photon thread does wonders.. Don't ya think? :joy:
Yup, update and configure.
```

---
## \#39 Posted by: ElskerShadow Posted at: 2018-03-24T12:26:55.634Z Reads: 73

```
True that, i knda stopped watching the thread since i had a bad module for months !
```

---
## \#40 Posted by: RedEagle Posted at: 2018-03-24T12:28:31.779Z Reads: 72

```
[quote="ElskerShadow, post:39, topic:50002"]
stopped watching the thread
[/quote]


Tsk tsk.. Who taught you that nonsense? :sweat_smile:
```

---
## \#41 Posted by: ElskerShadow Posted at: 2018-03-24T12:29:13.739Z Reads: 68

```
My frustration with the remote heh
```

---
## \#42 Posted by: trancejunkiexxl Posted at: 2018-03-24T12:30:17.799Z Reads: 69

```
U could try setting up another vesc.. I always just start switching crap out when things don't go my way
```

---
## \#43 Posted by: Wajdi Posted at: 2018-03-24T14:01:24.078Z Reads: 64

```
@ElskerShadow Dont upgrade to FW3 !
You will only face more problems.

Also I don't really see how the photon receiver would cause any of this, since PPM does not work as well it seems like a misconfiguration on your part.
```

---
## \#44 Posted by: Wajdi Posted at: 2018-03-24T14:03:23.323Z Reads: 64

```
Can you show your real time data from the BLDC tool?
```

---
## \#45 Posted by: Blasto Posted at: 2018-03-24T14:46:51.983Z Reads: 63

```
When changing apps, the esc needs to be rebooted for the changes to apply
```

---
## \#46 Posted by: ElskerShadow Posted at: 2018-03-24T15:08:14.664Z Reads: 62

```
I have made it work by updating the firmware and it works with no problem i have used the software in your github 
I am currently riding now so what you says worries me
```

---
## \#47 Posted by: Wajdi Posted at: 2018-03-24T15:10:45.423Z Reads: 62

```
Thats fine then, if you got it working then your receiver version is compatible. Nothing to worry about.
```

---
## \#48 Posted by: ElskerShadow Posted at: 2018-03-24T15:12:57.708Z Reads: 61

```
Yeah i guessed that since you sent me a new reciever not long ago it would be fine .
I am finally riding the remote and i m having a blast
With a few tuning in the software of the remote it will be even better
```

---
## \#49 Posted by: Sebike Posted at: 2018-03-24T15:21:53.911Z Reads: 62

```
Actually, in many European countries (maybe other countries as well), we use periods or a blank space where you use commas, and a comma where you use a period.

Therefore 60,000 = 60
And 60.000 = 60000 = 60.000,00 = 60 000
Lol
```

---
## \#50 Posted by: GrecoMan Posted at: 2018-03-24T15:27:06.881Z Reads: 61

```
yea I understand that, but (imo) this is a pretty US dominated forum (we’ve got 90% of vendors over here, and tons of members
```

---
## \#51 Posted by: Sebike Posted at: 2018-03-24T15:30:51.122Z Reads: 61

```
... which makes this a golden opportunity to learn from each other 😋 (about commas and periods.. Lol)
```

---
## \#52 Posted by: GrecoMan Posted at: 2018-03-24T15:32:28.217Z Reads: 62

```
touché 

hahaha 😁

i’m actually sitting on the side of a pool eves dropping on an aussie talking to an american, damn we sound stupid
```

---
## \#53 Posted by: ElskerShadow Posted at: 2018-03-24T18:52:45.340Z Reads: 60

```
And If I may, when we talk of any measure you are dominated by the whole world , so lean towards us ! 
Still one of the last few coutry that use this Imperial nonsense
```

---
## \#54 Posted by: GrecoMan Posted at: 2018-03-24T18:56:09.954Z Reads: 57

```
oh yea, imperial is a joke

i can agree on that
```

---
