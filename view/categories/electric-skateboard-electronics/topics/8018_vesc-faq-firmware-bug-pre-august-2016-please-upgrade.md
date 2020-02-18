# VESC FAQ &#124; Firmware Bug &#124; Pre August 2016 &#124; Please Upgrade

### Replies: 31 Views: 3408

## \#1 Posted by: onloop Posted at: 2016-08-20T23:52:19.800Z Reads: 312

```
The community has found that there is a bug in the current firmware that was shipped with your vesc before **August 2016**. But good news we have found a solution and want to let you know how to update your firmware. Also, all files at vesc.net.au have been updated so when downloading  BLDC TOOL don't be afraid of getting the wrong firmware.

We recommend you do this now or when you receive your vesc. 
If you have a raptor or an enertion r-spec motor don't worry, the motor setting have already been applied for you.

Please download the new firmware for 
http://vesc.net.au/BLDC-TOOL/Firmware/VESC_4.10_default.bin

You will need BLDC TOOL to update the firmware that you can download from 
http://vesc.net.au/download-now/
```

---
## \#2 Posted by: Dedbny Posted at: 2016-08-21T00:10:25.439Z Reads: 293

```
What about batch 1 Raptors, mine was back in for repairs mid April. What issue does the patch fix?
```

---
## \#3 Posted by: onloop Posted at: 2016-08-21T00:17:20.514Z Reads: 279

```
if your raptor is working don't do anything.... the bug appears when you are making/applying  changes in the BLDC.
```

---
## \#4 Posted by: Dedbny Posted at: 2016-08-21T00:19:30.549Z Reads: 262

```
So if you do makes changes under bldc tool you have to update to the new firmware.
```

---
## \#5 Posted by: Titoxd10001 Posted at: 2016-08-21T03:52:50.525Z Reads: 252

```
Are you sure this works the link doesn't work and I've tried downloading the firmware that was updated August 15 and still have ramp bug
```

---
## \#6 Posted by: E-Boarding Posted at: 2016-08-21T06:47:00.795Z Reads: 225

```
what kind of bug is that, what happend when it don't get fixed?
```

---
## \#7 Posted by: Svenska Posted at: 2016-08-21T06:52:57.626Z Reads: 217

```
You blow up your VESC...
The bug is in one of the advanced features, it's a setting that keeps taps on your power ramping. Aka, lightly ramp up the current instead of hitting it in the face.
But it only come in the moment you read the settings from your VESC and write them back. If you don't plan on writing any settings to the VESC you're sweet.
```

---
## \#8 Posted by: Just_esk8in Posted at: 2016-08-21T13:08:32.368Z Reads: 205

```
Wait so I got mine about the 29th of July and I haven't used it at all yet should I do this before I use it
```

---
## \#9 Posted by: cesargrimmelprez Posted at: 2016-08-21T14:12:54.553Z Reads: 197

```
Yes you should
```

---
## \#10 Posted by: cesargrimmelprez Posted at: 2016-08-21T14:13:06.460Z Reads: 197

```
Just to be sure
```

---
## \#11 Posted by: ikjahaa Posted at: 2016-08-21T14:16:20.308Z Reads: 190

```
Did the file "/VESC_4.10_default.bin" get deleted ?
I get "Oops! That page can’t be found." message.
```

---
## \#12 Posted by: Just_esk8in Posted at: 2016-08-21T19:53:10.018Z Reads: 179

```
Ok thank you
```

---
## \#13 Posted by: sprocket12 Posted at: 2016-08-22T15:20:43.684Z Reads: 169

```
Same here!
```

---
## \#14 Posted by: ikjahaa Posted at: 2016-08-22T16:05:22.606Z Reads: 183

```
[quote="ikjahaa, post:11, topic:8018, full:true"]
Did the file "/VESC_4.10_default.bin" get deleted ?I get "Oops! That page can’t be found." message.
[/quote]


@onloop ? could you inform us...
```

---
## \#15 Posted by: bigpianist Posted at: 2016-09-06T12:06:02.906Z Reads: 164

```
Hey guys, just watch out because the August Enertion VESC's still have this problem. I ordered 2 mid August and they both have the current ramping bug, so don't think that because it's August that your VESC won't have the bug. Really watch out because it'll fry your VESC.
```

---
## \#16 Posted by: yaca Posted at: 2016-10-02T21:05:23.965Z Reads: 130

```
Hi, should the new firmware solve the "Max Current ramp step" problem? I downloaded it and gave it into the firmware folder. I opened the BLDC Tool and choosed "VESC_4.10_default.bin. Then i pressed upload. The green bar starts to run till 100%. It writes "FW Upload Done" and in the same moment on the button right it appears "Device not found" and then "Not conected". I connect again and the bug with the "Max current ramp step" is still there. I tried it many times but it doesn't work for me.
What's wrong? Please help me!
```

---
## \#17 Posted by: ninja Posted at: 2016-10-03T09:00:25.063Z Reads: 126

```
Hi! 
That firmware link http://vesc.net.au/BLDC-TOOL/Firmware/VESC_4.10_default.bin 
is not opening, it shows that it's VLC media file, and VLC player not opening it anyway. About BLDC tool, in this link  http://vesc.net.au/download-now/ down load botton for windows is not working, but i tried to click on Old Versions, than click on Parent Directory, than click on  BLDC_Tool.exe. Is this BLDC_Tool.exe is fine or it's bad? 
So i have enertion VESC, ordered it in middle of August, now it's in shelf,never was tried it because i'm waiting for my remote.  So when my remote arrives i'll be doing VESC programming, so i need to be sure what BLDC TOOL to use, where to get it, also where to get that bugless Firmware, because those links not working. Also question about power supply for first connecting to PC, so can i use 8s lipo, if my set up will be 8s? Or better use 4s lipo? Or never use lipos for programming VESC?
```

---
## \#18 Posted by: yaca Posted at: 2016-10-03T20:00:40.167Z Reads: 122

```
My problem with the firmware update is solved. I remembered I had similar problems with an other ESC a few years ago. So I tried like last time to install BLDC Tool on the account of my wife ( same computer) and now i can update the firmware. I dont understand why it is not possible on my account but now I can do it with my wifes account and I'm happy. Is there a computerfreak and can explain me the reason?

@ninja   Your firmware  link works. You have to download it and then copy it into the firmwarefolder of the BLDC Tool. The BLDC Tool software I downloaded from here: http://www.esk8.de/tutorials-d-e-f/ 
Don't use the "Depugged Firmware 2.18 for ...", it doesnt work, use your firmware link " ... 4.10_default.bin" 
Power supply: I'm not sure about this. I used a 3s Lipo with antispark xt90 in the pluswire.
Some say it's just a problem when the VESC gets power the first time. Vesc from enertion are already have seen power I think.
```

---
## \#19 Posted by: ninja Posted at: 2016-10-04T10:42:16.566Z Reads: 108

```
O.K. i downloaded that BLDC TOOL version 2.18 for windows from http://www.esk8.de/tutorials-d-e-f/. But when i click on http://vesc.net.au/BLDC-TOOL/Firmware/VESC_4.10_default.bin, it's downloading as VLC media file, also VLC player not recognize it anyway. Is some other place i can get that firmware from?
```

---
## \#20 Posted by: elkick Posted at: 2016-10-04T10:55:41.805Z Reads: 106

```
The right firmware is included in the bldc tool zip file on esk8.de. Also, the stand alone debugged version 2.18 for VESC 4.12 works too, I just checked again.
```

---
## \#21 Posted by: ninja Posted at: 2016-10-04T11:06:01.151Z Reads: 98

```
So i can use that BLDC TOOL version 2.18 for windows from http://www.esk8.de/tutorials-d-e-f/, and don't need anything else? That debugged version is some kind of file i cannot open, so i don't need it since everything is included in that BLDC TOOL 2.18? Also about batteries- can i do configurations with my 8s lipo or better do 4s lipo or some laptop power supply?
```

---
## \#22 Posted by: elkick Posted at: 2016-10-04T11:09:45.685Z Reads: 100

```
[quote="ninja, post:21, topic:8018"]
That debugged version is some kind of file i cannot open,
[/quote]
you don't need to open that file. 

The standalone FW can be opened in BLDC tool only (with clicking the Firmware tab, then update and selecting the downloaded file form your disk). 

But since I didn't have the bug version of the FW 2.18 on my page you can just go the normal way too, selecting it in the downloaded BLDC Tool folder.

If the VESCs you have are made with genuine parts and pre-tested you would not need a laptop power supply. But if you are unsure it's better to use it though.
```

---
## \#23 Posted by: ninja Posted at: 2016-10-04T11:24:24.615Z Reads: 92

```
It's enertion VESC, so i think than i can do lipo, but 8s or 4s? And what i should write in BLDC TOOL if i'm using 4s, i mean, i still need to write numbers as it is for 8s, because my setup will be 8s 8000mah?
```

---
## \#24 Posted by: elkick Posted at: 2016-10-04T12:11:41.202Z Reads: 89

```
If you're trying it with 4s you need the specs for voltage cut off start and end for 4s (in the Voltage Limits field). You can change it back later to 8s specs. Don't touch min. and max. voltage there, it's not necessary.
```

---
## \#25 Posted by: ninja Posted at: 2016-10-04T13:26:08.248Z Reads: 83

```
I want to try it with 8s, my question was is that safe? I want to write all things in BLDC TOOL for 8s, and go to skate. So as far as i understand: 1) connect VESC to motor
                                                    2) turn on remote
                                                    3) switch on VESC with 8s battery via xt90s anti spark loop key
                                                    4) connect VESC to pc via USB
                                                    5) at BLDC TOOL connect software connection
                                                    6) upgrade newest firmware
                                                    7) App configuration (which control mode should i use?)
                                                    8) do motor configuration
  Then what?.. Turn of battery and go for test ride? What should i know about braking adjustments and how i can make my board a little slower for first time, like beginner mode or something, till i get use to that speed!?
```

---
## \#26 Posted by: elkick Posted at: 2016-10-04T15:13:29.092Z Reads: 82

```
In general, your steps are correct, but switch point 8 and 7: first motor detection, then app config.

In the app config:  if you have a 2.4GHz remote, take ppm and then "current no reverse with brakes". After "write config" in the app section don't forget to klick "reboot". 

All those points are described in the FAQ section here.
```

---
## \#27 Posted by: ninja Posted at: 2016-10-04T15:41:02.250Z Reads: 73

```
O.K. thanx a lot!
```

---
## \#28 Posted by: Jebe Posted at: 2016-10-04T22:08:55.927Z Reads: 76

```
@EnertionSupport Is this covered by warranty ?
```

---
## \#29 Posted by: ninja Posted at: 2016-11-19T10:58:26.016Z Reads: 63

```
Hi! 
I have some issues with VESC. So i have  enertion VESC 4.12, connected to BLDC TOOL, it even read configuration, so no problems so far! Then i tried to upload new firmware, i took it from 4.12 folder, it called vesc default bin. It showed than it uploaded 100%, but since it uploaded it disconnected from BLDC TOOL, when i tried to connect again it showed 
<img src="/uploads/db1493/original/3X/5/5/5543a32f4527096541e3481cb349bf8336806486.png" width="564" height="206">
So what i should do now? Strange is that when i connected i think it showed that connected vesc had 2.17 or 2.18, but now it shows that connected vesc have 2.15 firmware. But my BLDC tool is supported for 2.17 and 2.18. But maybe VESC had 2.15 version of firmware already.

So I downloaded BLDC tool for 2.15, so everything working now! But i want new version without bugs, like 2.18. How can i upload 2.18 if it allows only 2.15? How does it possible that my VESC has so old firmware 2.15, i bought it maybe just 3 months ago? So it means that they sold me some old VESC or something? O.K. i don't care if it's 2.15 or 2.18 as long as it's without firmware bugs. So how can i tell if my 2.15 version have bug or not?
```

---
## \#30 Posted by: GhettoFab.rictation Posted at: 2017-12-23T17:52:01.166Z Reads: 33

```
download this vesc tool for free then use your current bldc tool to upload the bootloader from the link I'm going to show you: http://vesc-project.com/vesc_tool  .. It said the same things to me and I was still able to upload the bootloader then upgrade my vesc!! Just use the bootloader file from new link and upload the bootloader file through your bldc tool that is used for your wanted firmware!!
```

---
## \#31 Posted by: GhettoFab.rictation Posted at: 2017-12-23T17:53:59.712Z Reads: 33

```
I have an issue though about my motor detection and I can't even get my motor to make noise :unamused: ..  http://www.electric-skateboard.builders/t/vesc-bad-motor-detection-0-faults-motor-solder-joints-ok-fw-2-18-vesc-4-12-please-help/41742
```

---
