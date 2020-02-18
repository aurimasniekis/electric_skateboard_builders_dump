# Help! my board randomly stops working

### Replies: 49 Views: 1152

## \#1 Posted by: wieg16 Posted at: 2018-03-24T04:04:12.403Z Reads: 104

```
hello everyone, i haven't posted on here in a while. i started making my board 2 years ago and it ended up turning out just how i wanted. i had some problems at first but that is to be expected with a beginner like me. after working all the kinks out it finally ran perfectly. i rode it for about a year with zero problems. however just recently it started acting weird. randomly when i turn it on it wont work. the vesc light turns on the the remote light turns solid to where it says its connected but when i pull the the throttle nothing happens. i will turn it off and on multiple times, check that all the connections are good and still nothing happens. ive found if i turn it off and let it sit for a day itll work. i have no idea why and i was hoping somebody could help me figure out what is going on. also something else has been happening, i dont know if its related but sometimes when im riding the board will start to throttle itslef and brake itself. sometimes its so sudden and powerful it throws you off the board. this only happens 1/10 times when i ride. could these problems be originating from a bug in the vesc software? please help!!!!
```

---
## \#2 Posted by: pat.speed Posted at: 2018-03-24T04:05:54.813Z Reads: 100

```
What remote are you using? And post some pics of Vesc settings. Also type faults into the Vesc tool to see if there are any errors
```

---
## \#3 Posted by: wieg16 Posted at: 2018-03-24T04:08:46.923Z Reads: 97

```
im using the TORQUEBOARDS 2.4GHZ MINI REMOTE CONTROLLER from  and sorry i havent used the BLDC program in forever ill have to check it.
```

---
## \#4 Posted by: wieg16 Posted at: 2018-03-24T04:12:49.893Z Reads: 88

```
sorry i dont think i replied directly to this post
```

---
## \#5 Posted by: pat.speed Posted at: 2018-03-24T04:14:30.105Z Reads: 85

```
No worries, when you get a chance check bldc tool that will help a lot
```

---
## \#6 Posted by: wieg16 Posted at: 2018-03-24T04:16:01.668Z Reads: 80

```
working on it right now, will i have to update my bldc tool? i havent used it in 2 years??
```

---
## \#7 Posted by: wieg16 Posted at: 2018-03-24T04:17:44.513Z Reads: 80

```
sorry i did it again hahaha
```

---
## \#8 Posted by: wieg16 Posted at: 2018-03-24T04:34:25.565Z Reads: 75

```
how do i test using the bldc tool i cant figure it out and i dont remember. i dont wanna mess my vesc up.
```

---
## \#9 Posted by: Namasaki Posted at: 2018-03-24T04:36:57.053Z Reads: 74

```
If you built your board 2 years ago then you also  need to make sure you don't have the ramp step bug in your firmware
```

---
## \#10 Posted by: wieg16 Posted at: 2018-03-24T04:38:06.095Z Reads: 72

```
how do i check that. im on 2.18 firmware
```

---
## \#11 Posted by: Namasaki Posted at: 2018-03-24T04:46:16.068Z Reads: 74

```
You have to connect to the bldc tool and read your configuration and then check the 
Max Current Ramp Step(at 1khz)
It should be 0.0400

If you have the bug, it will multiply the setting every time you write configuration.
If the setting gets too high it will cook your Vesc.
This is an old problem that was corrected with a firmware update about a year or more ago

![47 PM|690x422](upload://v3yK0Ny65rDsRhvrXE35HM4WfGq.png)
```

---
## \#12 Posted by: wieg16 Posted at: 2018-03-24T04:49:42.106Z Reads: 66

```
mine is set at 50?? why havent i had a problem until now??
```

---
## \#13 Posted by: Namasaki Posted at: 2018-03-24T04:50:47.705Z Reads: 65

```
I would say you are very lucky that you haven't toasted your vesc yet
```

---
## \#14 Posted by: wieg16 Posted at: 2018-03-24T04:51:40.302Z Reads: 64

```
holy crap..... ive literally been daily riding it for a year and a half now at school going up steep hills and topping out at 30 mph
```

---
## \#15 Posted by: wieg16 Posted at: 2018-03-24T04:51:57.910Z Reads: 61

```
do i change it to .004
```

---
## \#16 Posted by: Namasaki Posted at: 2018-03-24T04:52:26.309Z Reads: 63

```
You need to update firmware
```

---
## \#17 Posted by: wieg16 Posted at: 2018-03-24T04:53:55.214Z Reads: 64

```
my bldc tool says it only supports 2.17 and 2.18, do i need to update it as well?
```

---
## \#18 Posted by: Namasaki Posted at: 2018-03-24T04:54:41.956Z Reads: 64

```
The bug was in an early version of 2.18
A fixed version of 2.18 came out after the problem was discovered
```

---
## \#19 Posted by: wieg16 Posted at: 2018-03-24T04:55:18.112Z Reads: 64

```
okay do i download the version somewhere online?
```

---
## \#20 Posted by: Namasaki Posted at: 2018-03-24T04:55:55.303Z Reads: 65

```
You have a couple options here,
give me a second while I check on something
```

---
## \#21 Posted by: Namasaki Posted at: 2018-03-24T04:58:45.611Z Reads: 62

```
I can email you the fixed 2.18 firmware or
you can download the bldc tool with firmware here:
http://www.enertionboards.com/FOCBOX-speed-controller.html

Or you could download the new Vesc Tool with firmware
https://www.vesc-project.com/vesc_tool
```

---
## \#22 Posted by: wieg16 Posted at: 2018-03-24T05:02:19.839Z Reads: 62

```
okay im downloading it. also i tapped the arrow keys while my board was connected and now the controller wont control the board, this has happened before but i dont rmeber what setting i change to fix this
```

---
## \#23 Posted by: Namasaki Posted at: 2018-03-24T05:04:53.639Z Reads: 60

```
When you update your firmware, it should put everything back to factory default settings so you have to set it all up again but the update may fix the other problems your having.
```

---
## \#24 Posted by: wieg16 Posted at: 2018-03-24T05:05:32.472Z Reads: 58

```
okay, and do i need to download the firmware from somewhere or is it built into the program?
```

---
## \#25 Posted by: Namasaki Posted at: 2018-03-24T05:06:10.494Z Reads: 57

```
It will be in a folder that comes with the bldc tool.
Are you on windows or Mac?
```

---
## \#26 Posted by: wieg16 Posted at: 2018-03-24T05:06:32.793Z Reads: 58

```
I am on windows 10
```

---
## \#27 Posted by: Namasaki Posted at: 2018-03-24T05:07:43.673Z Reads: 59

```
When you unzip the download file, there should be a folder in the package with firmware files.

If not, send me a pm with your email address and I will email you the file.
```

---
## \#28 Posted by: Namasaki Posted at: 2018-03-24T05:11:39.564Z Reads: 58

```
the firmware files I have are Mac bin files so not sure if it will work with the windows bldc tool or not.
Hopefully the bldc tool download will have the files packaged with it
```

---
## \#29 Posted by: wieg16 Posted at: 2018-03-24T05:12:24.639Z Reads: 59

```
I have found the file I’m trying to update it now
```

---
## \#30 Posted by: Namasaki Posted at: 2018-03-24T05:12:57.317Z Reads: 60

```
use the vesc_default.bin
```

---
## \#31 Posted by: wieg16 Posted at: 2018-03-24T05:13:33.638Z Reads: 55

```
I’m watching a Esk8 support video right now
```

---
## \#32 Posted by: wieg16 Posted at: 2018-03-24T05:14:45.747Z Reads: 52

```
It didn’t fix the controller problem
```

---
## \#33 Posted by: Namasaki Posted at: 2018-03-24T05:15:25.860Z Reads: 49

```
did you already go through all the settings and write config?
you need to set everything and write config and check your ramp step to make sure it's not multiplying.
You will also need to recalibrate your controller in the bldc tool.
```

---
## \#34 Posted by: Jebe Posted at: 2018-03-24T05:15:33.883Z Reads: 48

```
try a different receiver - may have burnt out the channel on that one. esp if you have removed it and connected it the wrong way
```

---
## \#35 Posted by: wieg16 Posted at: 2018-03-24T05:16:38.064Z Reads: 47

```
No I don’t remember what all I have to do, I have only read the current configs
```

---
## \#36 Posted by: Namasaki Posted at: 2018-03-24T05:18:05.426Z Reads: 49

```
When you update the firmware it should be like new and needs to be setup. Vesc have never been plug n play
```

---
## \#37 Posted by: Namasaki Posted at: 2018-03-24T05:21:53.829Z Reads: 49

```
It's been so long since I updated my firmware but I think you will have to start over from the beginning.
Current and voltage settings, Motor detection, controller calibration,
```

---
## \#38 Posted by: wieg16 Posted at: 2018-03-24T05:22:35.287Z Reads: 49

```
Okay thank you I’m watching a video on how to do it now I’ll check in when I’m done
```

---
## \#39 Posted by: Namasaki Posted at: 2018-03-24T05:23:10.159Z Reads: 54

```
I'm going to bed in a few min but I'll check back in the morning to see how it went
```

---
## \#40 Posted by: Namasaki Posted at: 2018-03-24T05:24:45.697Z Reads: 55

```
Here is a good video on how to setup your controller in the bldc tool
https://youtu.be/OtuofrQr3F8
```

---
## \#41 Posted by: Eboosted Posted at: 2018-03-24T05:26:31.359Z Reads: 52

```
You need to check if you get throttle input when configuring you ppm settings
```

---
## \#42 Posted by: wieg16 Posted at: 2018-03-24T05:39:54.161Z Reads: 51

```
okay so after my updating my firmware i re did all the settings but when i hit the throttle it instantly was full throttle. i went through the settings again and everything looks right and now when i try it nothing happens. not even when i try and control it with the arrow keys on my computer. what did i do to cause this?
```

---
## \#43 Posted by: wieg16 Posted at: 2018-03-24T05:40:59.811Z Reads: 50

```
the throttle was connecting and working but now its not moving when i pull the throttle
```

---
## \#44 Posted by: wieg16 Posted at: 2018-03-24T05:42:51.556Z Reads: 48

```
just kidding im getting a response i forgot i unplugged my vesc
```

---
## \#45 Posted by: pat.speed Posted at: 2018-03-24T09:07:37.699Z Reads: 44

```
Lolololol, it might be a ppm issue as to why you were getting full throttle.
```

---
## \#46 Posted by: GrecoMan Posted at: 2018-03-24T11:53:30.296Z Reads: 40

```
sounds more like incorrectly setup failsafe to me
```

---
## \#47 Posted by: Namasaki Posted at: 2018-03-24T15:39:42.681Z Reads: 38

```
The Vesc in current control mode will spin the motor at full RPM at the beginning of throttle curve when there is no load on the motor as when testing with the board upside down on the bench. 
This is because the Vesc in current control delivers full voltage  throughout the entire throttle curve and voltage determines RPM. 
The Vesc will increase current as more throttle is applied which will increase speed under load.
```

---
## \#48 Posted by: wieg16 Posted at: 2018-03-24T16:59:42.097Z Reads: 31

```
i dont know what i did, i followed all the steps exactly but nothing was working and i found out im now getting a drv8302 error so i think at some point last night i messed something up and burned the chip.
```

---
## \#49 Posted by: wieg16 Posted at: 2018-03-29T22:55:27.551Z Reads: 22

```
 Just to check back in I found out that I had a blown the DRV chip,  I decided just to spend the money and buy a new VESC instead of dealing with the hassle of trying to find someone to fix it. I got the new VESC up and running and it works great! ![image|375x500](upload://8XOPQlw52ckZl73xkbT4GLzTRSW.jpeg)![image|374x500](upload://2dtX8K1EQhxmo2obsIz6SMaVWwN.jpeg)
```

---
