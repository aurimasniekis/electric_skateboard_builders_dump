# Updating my VESC to latest firmware and don&rsquo;t know which firmware to download

### Replies: 55 Views: 11364

## \#1 Posted by: Tampaesk8er Posted at: 2017-02-02T23:59:47.669Z Reads: 715

```
I plugged my vesc to the bldc tool and the popup states that my vesc firmware is old and i need to update it. The issue is, when i clicked on firmware folder, there are alot of different firmware versions, I dont know which firmware i should download, can someone help me out? Much thanks!
```

---
## \#2 Posted by: chuttney1 Posted at: 2017-02-03T04:30:08.194Z Reads: 678

```
Firmware version is dependent on the HW version of the VESC you having meaning it's either 4.7, 4.8, 4.9, 4.10, 4.11, or 4.12. Once you make the update to latest version everything is fine.
```

---
## \#3 Posted by: Tampaesk8er Posted at: 2017-02-03T10:22:00.952Z Reads: 656

```
I was looking on the vesc and found (had to use magnifier) it says vedders 4.12, I assume i have to download firmware 4.12, correct?
```

---
## \#4 Posted by: Ackmaniac Posted at: 2017-02-03T10:48:05.331Z Reads: 647

```
4.12 is the Hardware Version. Benjamin improved the hardware components over the time to make the VESC more robust. When you have a closer look at the VESC then you will see that number printed on the Board. 
<img src="/uploads/db1493/original/3X/9/2/925521c9851a6356c1c02b77d4358a9da3329773.jpg" width="690" height="463">

What you need is a update of the Firmware. So it would be the best that you tell us which Hardware version of the VESC you have so that we can tell you the correct firmware.
```

---
## \#5 Posted by: Tampaesk8er Posted at: 2017-02-03T19:40:29.027Z Reads: 598

```
My vesc says exactly like the picture shows (4.12). What next? Thank you.
```

---
## \#6 Posted by: Ackmaniac Posted at: 2017-02-03T21:02:12.763Z Reads: 596

```
Then i would recommend you to use my firmware mod because when you hover with the mouse over the parameter labels it gives you a Tooltip text that helps you to understand what the parameter is good for. 

http://www.electric-skateboard.builders/t/extended-bldc-tool-with-watt-control-mode-ppm-cruise-control-individual-throttle-curve-and-android-app/12286

Otherwise you can also download the actual original Version 2.18 here. 
http://vesc.net.au/
```

---
## \#7 Posted by: Tampaesk8er Posted at: 2017-02-03T21:11:45.630Z Reads: 559

```
Thank you, I'll check it out on my pc. I have been reading everything on vedders page and watching all the videos Really trying to understand the whole thing. Thank you so much for the help, can't wait to get home and start this thing.
```

---
## \#8 Posted by: Tampaesk8er Posted at: 2017-02-03T23:14:57.113Z Reads: 506

```
Trying to upload vesc version 4.12 firmware and it won't upload, it says "buffer erase timeout" what can I do to make this work?<img src="/uploads/db1493/original/3X/4/9/49dd9a4acfff42eb74fa817af42d2a97da91c775.jpeg" width="499" height="499">
```

---
## \#9 Posted by: Tampaesk8er Posted at: 2017-02-03T23:17:16.041Z Reads: 476

```
<img src="/uploads/db1493/original/3X/b/8/b85d2a070aa906613fd83172a9f663eb572ea077.jpeg" width="499" height="499">
```

---
## \#10 Posted by: Ackmaniac Posted at: 2017-02-03T23:21:59.703Z Reads: 452

```
Are you sure you first connected so that the message popped up and after that tried to flash the firmware?
```

---
## \#11 Posted by: Tampaesk8er Posted at: 2017-02-03T23:22:20.355Z Reads: 452

```
ok, it uploaded, finally. firmware version is (2.16) how do i get 2.16 so i can have this thing working?<img src="/uploads/db1493/original/3X/8/2/82c1cab9d406c3f038ecee774e5294d4bc1356e1.jpeg" width="669" height="499">
```

---
## \#12 Posted by: Ackmaniac Posted at: 2017-02-03T23:23:56.646Z Reads: 433

```
Just reconnect again. If you have uploaded the correct firmware it should show 2.18.
```

---
## \#13 Posted by: Tampaesk8er Posted at: 2017-02-03T23:26:58.404Z Reads: 422

```
ok, let me try it
```

---
## \#14 Posted by: Tampaesk8er Posted at: 2017-02-03T23:29:52.658Z Reads: 430

```
Now it says this, "Firmware version on connected vesc: X,Y"<img src="/uploads/db1493/original/3X/3/c/3c34c2f778b4b772522e2788b320782ddc784237.jpeg" width="669" height="499">
```

---
## \#15 Posted by: Ackmaniac Posted at: 2017-02-03T23:30:55.156Z Reads: 403

```
Press the disconnect and then the connect button.
```

---
## \#16 Posted by: Tampaesk8er Posted at: 2017-02-03T23:31:30.352Z Reads: 398

```
ok hold on
```

---
## \#17 Posted by: Tampaesk8er Posted at: 2017-02-03T23:33:39.233Z Reads: 416

```
now i got this again
<img src="/uploads/db1493/original/3X/7/1/71fbeebf2ba544e83b68a39de8a2cc832bb3d401.jpeg" width="669" height="500">
```

---
## \#18 Posted by: Ackmaniac Posted at: 2017-02-03T23:40:34.010Z Reads: 407

```
Try to flash with the file "VESC_Ackmaniac_2_53.bin" which you can find at this link.

https://www.dropbox.com/home/Public%20Files/BLDC-TOOl%20and%20Firmware

And also use the BLDC-Tool you can find there for your operating system. I guess it is windows.
```

---
## \#19 Posted by: Tampaesk8er Posted at: 2017-02-03T23:44:20.394Z Reads: 402

```
yes, windows, i'll get back to it in a few, gotta get dinner and feed my son, Thank you,
```

---
## \#20 Posted by: Tampaesk8er Posted at: 2017-02-04T15:30:00.708Z Reads: 400

```
Ok found this using google, is it ok to download firmware version 2.16 for my vesc? Has anyone done this?

http://vesc.net.au/BLDC-TOOL/Firmware/OLD%20Firmware/<img src="/uploads/db1493/original/3X/2/4/2484bb61aea2d7e673d52886c8852b5ddd01d2e4.png" width="666" height="500">
```

---
## \#21 Posted by: PXSS Posted at: 2017-02-04T15:48:51.028Z Reads: 369

```
Firmware 2.16 is the wrong one... 
You need 2.18
```

---
## \#22 Posted by: Tampaesk8er Posted at: 2017-02-04T16:19:12.986Z Reads: 368

```
I know the latest is 2.18 but the vesc software keeps telling me my vesc is 2.16, i guess they never did the firmware update to the latest. So should I upload 2.16 first and then do the 2.18 after just to get my vesc going?
```

---
## \#23 Posted by: Tampaesk8er Posted at: 2017-02-04T16:25:50.185Z Reads: 368

```
See it says "FIRMWARE VERSION ON CONNECTED VESC : 2.16"

<img src="/uploads/db1493/original/3X/8/2/82c1cab9d406c3f038ecee774e5294d4bc1356e1.jpeg" width="669" height="499">
```

---
## \#24 Posted by: PXSS Posted at: 2017-02-04T21:51:44.896Z Reads: 348

```
yes and then it says.. SUPPORTED FIRMWARES 2.17-2.18.

IS 2.16 PART OF 2.17-2.18?
```

---
## \#25 Posted by: Ackmaniac Posted at: 2017-02-04T22:49:02.074Z Reads: 350

```
Seems that the upload is not working on you VESC. After the upload it should show 2.18 but it seems that it doesn't do that. Just try if it works with my firmware that i showed in my last post. Otherwise i also don't know what to do. Maybe the bootloader is missing.
```

---
## \#26 Posted by: Tampaesk8er Posted at: 2017-02-04T22:58:01.985Z Reads: 347

```
ok, thanks, i'll keep you updated.
```

---
## \#27 Posted by: Tampaesk8er Posted at: 2017-02-05T15:22:12.815Z Reads: 348

```
What is a bootloader and how can i install it? If i download your program, do i have to input command promps to the vesc?
```

---
## \#28 Posted by: Ackmaniac Posted at: 2017-02-05T16:24:45.576Z Reads: 341

```
My firmware behaves the same as the original firmware. Only has some extra features. But you need my modded version of the BLDC-tool. 
If the upload of this firmware also doesn't work then it seems that the bootloader is missing. 
I recommend to watch some videos about the VESC configuration on YouTube. Otherwise it will be very time consuming when we give you a advice and you  ask immediately if that advice is correct.
```

---
## \#29 Posted by: Tampaesk8er Posted at: 2017-02-05T17:30:47.046Z Reads: 342

```
1- Can you post the link to the exact firmware that i need to your modded version so i can download it and try it?

2- If i need a bootloader, where can i find it and how do i install it?

3- I have been watching videos on youtube on vesc for a week, i have created a library of all the videos i have watched over and over, i have learned the basics of the vesc already, i've even sent emails to (onloop), (Jacob from vesc.net.au) and no one has replied back to me yet. So your software will be my last option that i'm gonna try, can you please walk me through it? 
 If this doesnt work, im throwing the vesc in the trash, i contacted the place that i bought it from for a return and refund this morning, im still waiting for the reply back from them.

Believe me, I appreciate everything you have done for me, i just want this vesc working already, my first build and all new parts i have purchased, this eboard is a gift to my son and it has giving me headache after headache with this vesc.
Again, Thank you so much for taking the time to help me.
```

---
## \#30 Posted by: Ackmaniac Posted at: 2017-02-05T17:40:14.235Z Reads: 329

```
Her you can find my mod.
https://www.dropbox.com/home/Public%20Files/BLDC-TOOl%20and%20Firmware

Just use the BLDC-Tool for your windows machine "BLDC-Tool_ACKMANIAC_Mod_Windows 2_53.zip" and flash the VESC with the firmware file "VESC_Ackmaniac_2_53.bin".
If this doesn't work then you would need to install a bootloader.

But you can also use the BLDC-Tool for Firmware version 2.16
http://vesc.net.au/BLDC-TOOL/Windows/OLD%20Versions/
```

---
## \#31 Posted by: Tampaesk8er Posted at: 2017-02-05T18:45:07.790Z Reads: 310

```
im gonna try it all, i let you know what happens, thanks again.
```

---
## \#32 Posted by: Tampaesk8er Posted at: 2017-02-05T19:12:06.652Z Reads: 305

```
[quote="Ackmaniac, post:30, topic:17115"]
"BLDC-Tool_ACKMANIAC_Mod_Windows 2_53.zip" and flash the VESC with the firmware file "VESC_Ackmaniac_2_53.bin"
[/quote]

Dropbox says file cannot be found
```

---
## \#33 Posted by: Tampaesk8er Posted at: 2017-02-05T22:52:54.222Z Reads: 314

```
dropbox says file doesnt exist. i downloaded old versions of vesc 2.16 yesterday and i tried the link you gave me of 2.16 also but no luck. it still says (BUFFER ERASE:TIMEOUT) and OLD FIRMWARE.

<img src="/uploads/db1493/original/3X/e/1/e1f1eb92c61f2a34ea7eec34e9f71edccf7a8a6b.jpeg" width="669" height="499">
```

---
## \#34 Posted by: Tampaesk8er Posted at: 2017-02-05T22:55:34.194Z Reads: 287

```
I also contacted onloop for help but no reply back yet. im gonna order another vesc, do you know from what website I can order a vesc that has been tested and with current firmwares?
```

---
## \#35 Posted by: Tampaesk8er Posted at: 2017-02-05T22:56:50.381Z Reads: 282

```
Thank you @Ackmaniac for trying to help me with this issue.
```

---
## \#36 Posted by: SeanHacker Posted at: 2017-02-05T22:58:51.626Z Reads: 292

```
It's what @Ackmaniac does best. Or make super awesome firmware. :smiley:
```

---
## \#37 Posted by: Ackmaniac Posted at: 2017-02-05T23:15:36.293Z Reads: 307

```
Just download the 2.16 bldc-tool in the second link I posted and try to work with that one. Then it should be possible to work with that one instead of flashing the firmware of the current firmware on the vesc is 2.16.
If that works then it also might be possible to flash a new firmware via that bldc-tool.

And this here should be the correct link for my firmware mod if you want to give it a try.

[Dropbox](https://www.dropbox.com/sh/t7dl90owz5ccbyl/AAANyC-yQCMeveA7errNRnYqa?dl=0)
https://www.dropbox.com/sh/t7dl90owz5ccbyl/AAANyC-yQCMeveA7errNRnYqa?dl=0

And you also should try another USB cable and USB Port. I also had a Laptop where one of the USB Ports caused trouble.
```

---
## \#38 Posted by: Tampaesk8er Posted at: 2017-02-06T02:13:00.117Z Reads: 296

```
ok, thank you
```

---
## \#39 Posted by: Tampaesk8er Posted at: 2017-02-08T22:39:47.488Z Reads: 312

```
UPDATE: FINALLY GOT MY VESC TO CONNECT AND UPDATE?😎
Much thanks to all the people that were involved and sharing their amazing knowledge in Eboards.
 Now, I need help with the numbers to program the vesc settings, turnigy 6374 sk3 149kv, Torque Boards on off switch,  2X Zippy Flightmax 5000mAh 3s batts. Here is a pic. of the current settings based on stuff I read.
(would also like to setup regen. braking, dont really need reverse at the moment) still trying to learn all this stuff, many thank yous to all, my son is a very happy kid today.<img src="/uploads/db1493/original/3X/a/c/ace893d709397cd3cc92aac638d911ed973cb8a3.jpeg" width="669" height="499">
```

---
## \#40 Posted by: haand22 Posted at: 2017-06-17T09:13:31.593Z Reads: 304

```
Hey!
Just got my VESC and BLDC says its version 2.18. The vesc is 4.12. I would like to try out Ackmaniacs mods, cause it seems real cool :) The thing is I cant get the firmware upload working. There is no errors or anything, just says FW Upload done. The vesv does not restart as ive seen it do on Youtube. It just lits up the blue led and nothing more. When Power cycling and connecting it still says 2.18.
@Tampaesk8er did you do anything special to get it working?
The link for all bldc versions seems to be down.
```

---
## \#41 Posted by: Tampaesk8er Posted at: 2017-06-17T11:22:34.843Z Reads: 296

```
Everytime you change a setting, click write config on bldc tool, then hit the reboot button on bldc tool and connect again.
I tried to install acks. modified version of bldc tool and i had too many issues with it so i just use my vesc as is. Both my boards are riding between 19 & 22mph so im good with that.
```

---
## \#42 Posted by: Tampaesk8er Posted at: 2017-06-17T13:31:29.718Z Reads: 292

```
Here is a file that has windows and mac versions of bldc tool, download file and also save it in a memory card so you always have it.

https://drive.google.com/drive/mobile/folders/0Bym9XrdeViekfkRETmRndENkcVpySW5sWjIzOWdrLThCY01HY3BPOXpqYVRHUlQxS0R5ZlU?usp=drive_web#list
```

---
## \#43 Posted by: TarzanHBK Posted at: 2017-06-17T14:33:17.755Z Reads: 297

```
you´re missing a bootloader.
http://www.electric-skateboard.builders/t/vesc-installing-a-bootloader/752
```

---
## \#44 Posted by: haand22 Posted at: 2017-06-17T15:07:24.883Z Reads: 286

```
Its a mess if i miss the bootloader but it should work with version 2.18, right? Just need the right bldc tool for that version. http://vesc.net.au/ are down and nothing can be downloader from there. Does anyone have a bldc tool for 2.18? :)
```

---
## \#45 Posted by: haand22 Posted at: 2017-06-17T15:37:39.002Z Reads: 280

```
Oh, finaly found some older versions of bldc tool. Using the one for 2.18 workes like a charm for me.

http://www.electric-skateboard.builders/t/new-bldc-tool-download-links/1149/33?u=haand22
```

---
## \#46 Posted by: Tampaesk8er Posted at: 2017-06-17T15:41:40.396Z Reads: 281

```
Use the file i just gave you, its the same bldc tool that was on vesc.net.au

the file i just sent you works cause i installed it on my pc and on 3 different laptops and on a flash drive. 

when you connect your vesc to the bldc tool, make sure you click on top right corner, where it says "serial connection" click the little tab on the left side where it says connect. by doing this, it gives you the correct serial connection for your vesc. it worked for me, after you click that little black circular arrow next to where it says connect, it refreshes your serial connection for your vesc. follow these steps exactly, you might not need to download bootloader, it might be installed. i had same issue and i didnt have to download bootloader. you see in the picture how it says "COM5"
<img src="/uploads/db1493/original/3X/2/1/211e81b0f7e733b75500b201be51ae6e5715a765.jpg" width="666" height="500">
```

---
## \#47 Posted by: haand22 Posted at: 2017-06-17T15:59:18.806Z Reads: 244

```
Connecting is not an issue. Using the 2.54 Ackmaniac bldc tool, it says the firmware is old. Using the bldc tool for 2.18 works with no messages. I Think i will go with 2.18 so I can try my motor and och get the thing on the road before I start messing with the firmware again :p Thanks for your help!
```

---
## \#48 Posted by: Tampaesk8er Posted at: 2017-06-17T16:17:22.595Z Reads: 243

```
ok cool, i had too many issues with acks. tool so i never installed it, i just couldnt figure it out. Just stay using your vesc normally and you shouldnt have any issues, just tweak it to your likeness.
```

---
## \#49 Posted by: Ackmaniac Posted at: 2017-06-18T00:06:21.901Z Reads: 243

```
To use my modded bldc-tool you also need to flash the vesc with my firmware file. And if you can't flash it then it is very likely that you have a maytech vesc.
```

---
## \#50 Posted by: ATLesk8 Posted at: 2017-07-07T03:47:22.834Z Reads: 237

```


I purchased two used vescs from a user on here and I'm just getting around to figuring them out. He mentioned they have ackmaniac firmware but not which one. I have only used the bldc tool from the enertion website on multiple Torqueboards vescs...so
a. Is there a way to figure out which firmware is currently on a vesc?

b. Where can I find this software for Mac os?(if even available)?

c. is it easy to update these vescs easily? I don't want to damage them. 

Thank you for all the help.
```

---
## \#51 Posted by: Tampaesk8er Posted at: 2017-07-07T09:16:36.620Z Reads: 227

```
Try this link, i wouldnt try ackermans version, i had many issues with it, glitches for some 4.12 vesc. Try these:


https://drive.google.com/drive/mobile/folders/0Bym9XrdeViekfkRETmRndENkcVpySW5sWjIzOWdrLThCY01HY3BPOXpqYVRHUlQxS0R5ZlU?usp=drive_web#list

vesc-bldc-tool-download-link/
```

---
## \#52 Posted by: Tampaesk8er Posted at: 2017-07-07T09:29:35.167Z Reads: 232

```
vesc simple setup: 

http://www.youtube.com/playlist?list=PLICpQdAXJazRzoXJByGA_5wd-B4cifmbh

https://youtu.be/dxDXUrk-7ek

https://youtu.be/1TF8XARDa6U
```

---
## \#53 Posted by: DevinG Posted at: 2018-04-17T19:33:16.608Z Reads: 109

```
im getting error that says no firmware read response 
:face_with_raised_eyebrow:
```

---
## \#54 Posted by: Tampaesk8er Posted at: 2018-04-17T21:59:44.480Z Reads: 108

```
Use the new Vesc Tool and then you might have to install bootloader to your vesc if it dosnt have it installed. is your vesc a Maytech vesc?
```

---
## \#55 Posted by: DevinG Posted at: 2018-04-17T22:51:18.717Z Reads: 103

```
i just had to change com port so I'm moving on over to motor detection failed..
Thanks
```

---
