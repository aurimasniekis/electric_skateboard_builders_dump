# Help with Focbox firmware / bootloader upgrade \[VESC TOOL\]

### Replies: 51 Views: 3531

## \#1 Posted by: Enigmacpl03 Posted at: 2017-10-05T01:52:59.031Z Reads: 366

```
Hey guys,

So I installed new motors on my build and when I hooked up my vesc's to vesc tools, I received the error that my firmware was old and I needed to update.  (FW3.26) ( HW410)

On my master vesc, everything worked out fine it is now running 3.29. My slave foc seems to show signs of a missing bootloader. I go to update the firmware it shows complete, the vesc shuts off but does not restart. 

I know the vesc tools offers the bootloader option when doesnt seem to do anything. I am currently stuck in an endless cycle of "old firmware" on this 1 focbox.

Can someone help guide me in the right direction? Any help is greatly appreciated.

-Chris
```

---
## \#2 Posted by: Blasto Posted at: 2017-10-05T01:55:59.733Z Reads: 346

```
Well if it's any help, if you were able to update to v3.26, you do indeed have a bootloader

But from 3.26 to 3.29... no clue, restart the tool and power cycle the boxes
```

---
## \#3 Posted by: Enigmacpl03 Posted at: 2017-10-05T01:58:19.871Z Reads: 333

```
Yeah that is true, I have tried power cycling the boxes, Computer, software and different USB cable to try to narrow it down but no luck. 

> Well if it's any help, if you were able to update to v3.26, you do indeed have a bootloader

> But from 3.26 to 3.29... no clue, restart the tool and power cycle the boxes
```

---
## \#4 Posted by: Enigmacpl03 Posted at: 2017-10-06T01:27:54.909Z Reads: 302

```
Welp still nothing. Tried manually pushing Ackmamiac's firmware via Vesc tool with no luck.
```

---
## \#5 Posted by: PatRocks Posted at: 2017-10-06T01:30:59.518Z Reads: 298

```
Are you uploading firmware while the slave vesc is configured as such? If so, disconnect can, and then upload. Once uploaded use the new firmware to reconfigure

I think... 

What I would do in your situation is go step by step, as if you were configuring the slave as a standalone for the very first time. Then again, I have not used firmware 3.6
```

---
## \#6 Posted by: Enigmacpl03 Posted at: 2017-10-06T01:33:35.309Z Reads: 277

```
Canbus is disconnected and I am plugged directly into the slave. It behaves as if everything flashes fine but it doesnt complete the power cycle and its stuck on the old firmware
```

---
## \#7 Posted by: PatRocks Posted at: 2017-10-06T01:35:15.141Z Reads: 268

```
I think I'm out of my element here. I don't know what to do for sure, and don't want to mess your s*** up
```

---
## \#8 Posted by: Enigmacpl03 Posted at: 2017-10-06T01:36:47.903Z Reads: 264

```
I mean any info would be great, Unless you know where I can download the bin for 3.26 and the version of vesc tools so I can "downgrade" the master and I guess be stuck there.
```

---
## \#9 Posted by: PatRocks Posted at: 2017-10-06T01:44:03.914Z Reads: 255

```
Have you thought about running y-piece?
```

---
## \#10 Posted by: Enigmacpl03 Posted at: 2017-10-06T01:45:08.608Z Reads: 254

```
Not sure what you mean?
```

---
## \#11 Posted by: Enigmacpl03 Posted at: 2017-10-06T02:09:47.788Z Reads: 248

```
Well I found the vesc tool 079 for 3.26 thanks to @BigBoyToys and downgraded my master. Seems like my only option :-\
```

---
## \#12 Posted by: Blasto Posted at: 2017-10-06T05:59:28.066Z Reads: 235

```
Where you located? Think this could use some programming via the SWD port
```

---
## \#13 Posted by: Enigmacpl03 Posted at: 2017-10-06T09:41:22.259Z Reads: 233

```
Queens NY .. I'm hoping someone can help me.
```

---
## \#14 Posted by: scepterr Posted at: 2017-10-06T09:47:50.597Z Reads: 234

```
Can be delivered today
HonYan Mini Emulator Downloader ST-Link V2 STM8 STM32 Programming Unit (Random Color) https://www.amazon.com/dp/B01MZZ6USL/ref=cm_sw_r_cp_apa_he11zbBBPBNAN
```

---
## \#15 Posted by: Enigmacpl03 Posted at: 2017-10-06T10:00:08.267Z Reads: 227

```
With the individual pin connectors will that fit on a Focbox?
```

---
## \#16 Posted by: scepterr Posted at: 2017-10-06T10:11:22.814Z Reads: 227

```
Yeah you're gonna need to open up the focbox to access
There might be silicone over the pin holes, carefully peel it away
Ooo with that one you will need female to male leads, it only comes with female to female
You can convert female to male pretty easily though, snip off some resistor/led legs off and stick them in
```

---
## \#17 Posted by: Enigmacpl03 Posted at: 2017-10-06T10:17:45.649Z Reads: 223

```
Hmm ok so I don't need to buy JST connectors then? Do you have a guide to flash the focbox? I have seen a few guides but for just regular vescs. Not sure since of the HW version it would be different.
```

---
## \#18 Posted by: scepterr Posted at: 2017-10-06T10:18:42.124Z Reads: 227

```
It's hw version 4.12, flashing it is the same as any other
https://www.electric-skateboard.builders/t/vesc-x-will-now-be-called-enertion-focbox-motor-controller/23382/50
```

---
## \#19 Posted by: Enigmacpl03 Posted at: 2017-10-06T10:24:23.873Z Reads: 222

```
Mine are coming up as 4.10
```

---
## \#20 Posted by: scepterr Posted at: 2017-10-06T10:24:59.985Z Reads: 226

```
That's where your issue might be...
There are no hw4.10 focbox
```

---
## \#21 Posted by: Enigmacpl03 Posted at: 2017-10-06T10:25:55.858Z Reads: 215

```
Well they are (vesc-x) versions but Vesc tool shows the HW version on both as 410
```

---
## \#22 Posted by: scepterr Posted at: 2017-10-06T10:26:21.647Z Reads: 211

```
Don't you choose hw version when flashing?
```

---
## \#23 Posted by: Enigmacpl03 Posted at: 2017-10-06T10:30:58.616Z Reads: 208

```
Unfortunately with Vesc tool when you go to flash the HW version is bunched together. 4.10, 4.11, 4.12 no was of selecting just one.
```

---
## \#24 Posted by: scepterr Posted at: 2017-10-06T10:36:08.196Z Reads: 202

```
Do you have hw 4.10 or 4.12, it should be printed on the pcb
```

---
## \#25 Posted by: Enigmacpl03 Posted at: 2017-10-06T10:36:43.607Z Reads: 199

```
I will have to pull them from my board
```

---
## \#26 Posted by: Enigmacpl03 Posted at: 2017-10-06T10:43:23.737Z Reads: 199

```
I will need to check when I get back home. Thanks for the help so far ive ordered the STlink. If worst comes to worst can you help me out locally?
```

---
## \#27 Posted by: scepterr Posted at: 2017-10-06T10:43:50.510Z Reads: 199

```
Yeah that's not a prob
```

---
## \#28 Posted by: Enigmacpl03 Posted at: 2017-10-07T18:42:16.773Z Reads: 195

```
Ok so picked up the STlink then went to Microcenter today and they actually have Male to female 9" jumpers which fit perfectly. And was able to flash the bootloader -> then was able to downgrade to 2.54. Looks like I am all set  thank you for helping me @scepterr
```

---
## \#29 Posted by: okp Posted at: 2017-10-21T15:17:59.991Z Reads: 197

```
@Enigmacpl03 Hey Christian, how did ya wire the jumpers to connect the focbox to the stink ?

<img src="/uploads/db1493/original/3X/c/5/c563f01657e92104070115482ecfd7762503cc1c.jpg" width="522" height="500">
```

---
## \#30 Posted by: dAeM0N1K3 Posted at: 2017-11-03T02:37:14.755Z Reads: 195

```
Guys, I just flashed my brand new FOCBOX's with the firmware included in the Ackmaniac-ESC-Tool. All was going well and I was going through the standard motor setup wizard and was running through the resistance parameter test when on the first test both FOCBOXs stopped working and are no longer powering on. Please help, I freaking out about them being fried. I just bought these things for $280. How can I get them back on?

Prior to running the resistance parameters in the wizard, I set the voltage limits to Min voltage 8V Max voltage 57 Battery cutoff start 35V and Battery cutoff end to 33V on my 10S3P SPACECELL BMS. Is this fried? How can I get them to power up? Any help is greatly appreciated
```

---
## \#31 Posted by: Enigmacpl03 Posted at: 2017-11-03T15:27:04.645Z Reads: 191

```
When you plug it into the computer are you still getting the connection sound?


You need to make jumpers or buy them from microcenter or Amazon but you would connect them here.


<img src="/uploads/db1493/original/3X/1/f/1f69b7de74c5b8c1e5342f10cc54480f1d8ccb33.jpg" width="374" height="499">
```

---
## \#32 Posted by: dAeM0N1K3 Posted at: 2017-11-03T18:01:11.896Z Reads: 188

```
Thanks for the reply. I think I may have found the problem. It looks like the 40A fuse to the BMS blew out. I hope this is the only thing that blew out hopefully because its a very easy fix. I'm running to the hardware store now
```

---
## \#33 Posted by: sMATTEr Posted at: 2018-07-19T18:13:16.074Z Reads: 121

```
Hey!

Did you ever figure out why the vesc didn’t take the new firmware? I’m having the same problem.
```

---
## \#34 Posted by: Eboosted Posted at: 2018-09-13T19:03:17.995Z Reads: 107

```
@okp or @anyone have you guys figure out how to connect the STlnk to a Focbox?
```

---
## \#35 Posted by: okp Posted at: 2018-09-13T19:22:29.159Z Reads: 107

```
of course; I used a STLINKv2 to revive some of the FOCBOX that I had challenges with. Worked fine.
```

---
## \#36 Posted by: Eboosted Posted at: 2018-09-13T21:48:22.252Z Reads: 105

```
Can you give me the instructions?

I acccidentally flashed the HW48 firmware can't go back to v4.12
```

---
## \#37 Posted by: Blasto Posted at: 2018-09-13T21:53:13.688Z Reads: 107

```
Upload the 4.12fw via the custom fw tab
```

---
## \#38 Posted by: Eboosted Posted at: 2018-09-13T22:26:44.189Z Reads: 110

```
[quote="Blasto, post:37, topic:34810"]
ia the custome fw tab
[/quote]

I downloaded [this](https://github.com/vedderb/bldc-tool/tree/master/firmwares/hw_410_411_412) firmware:

![image|690x430](upload://9CKza4sPgikjVJ663zbiQ0KalCc.png)

Uploaded the firmware through custom file tab:

![image|690x439](upload://dN2nhxf2fdbaDahwEsblhXUFtRc.png)
![image|690x440](upload://buoI0AYLKA7VujNmwcoNk9p67je.png)

Then still on 48 hardware:

![image|690x436](upload://zDRbWxtXsIpwzN4b6L5DrJFI2to.png)
```

---
## \#39 Posted by: Blasto Posted at: 2018-09-13T22:33:32.394Z Reads: 106

```
Load the bootloader first... looks like the original got overwritten
```

---
## \#40 Posted by: Eboosted Posted at: 2018-09-13T22:50:37.862Z Reads: 109

```
I uploaded the bootloader:

![image|690x437](upload://tVQvLKNlW1750nE1GOLv1TxeOef.png)

Clicked "Yes"and got this error:

![image|519x168](upload://l1MyrBnE9V1BOqSqGUa084TXVYV.png)

So I used the @ackmaniac esc tool, which had the matching ESC tool for the wrongly updated firmware:

![image|690x497](upload://uD5cD4lgjtoh9EW6dLNYxINzzRt.png)

Waited 10 seconds, but nothing happened, I had to tunrn off/on the board and connected the ESC tool again, same HW:48 version :sob: 

![image|690x494](upload://1xamPR8h6ROMSQDGx07r7knIIl6.png)
```

---
## \#41 Posted by: Eboosted Posted at: 2018-09-13T22:51:11.380Z Reads: 94

```
Now I need help to connect the ST Link to the Focbox to upload the correct firmware.
```

---
## \#42 Posted by: Blasto Posted at: 2018-09-13T22:55:28.107Z Reads: 94

```
Once you upload the bootloader, you need to upload via the custom fw again
```

---
## \#43 Posted by: Eboosted Posted at: 2018-09-13T23:16:15.406Z Reads: 99

```
[quote="Blasto, post:42, topic:34810, full:true"]
Once you upload the bootloader, you need to upload via the custom fw again
[/quote]

I just did it, samething. I'm looking for the procedure to connect the ST Link to FocBox, can't find it anywhere
```

---
## \#44 Posted by: Eboosted Posted at: 2018-09-13T23:26:45.680Z Reads: 100

```
I found [this](https://www.electric-skateboard.builders/t/vesc-project-com-is-online-public-vesc-tool-download/32268/557?u=eboosted) procedure from a post by @Trampa but the FocBox does not have these pin labels:

![image|690x367](upload://qOrTUtJFVlhNgpXIrh91zAuTyhg.png)

On the Focbox I only have these pins:

![20180913_182336|281x500](upload://woVlHLFTyKwSCVwdxq9HY9mgFwj.jpg)
```

---
## \#45 Posted by: trampa Posted at: 2018-09-14T04:38:25.028Z Reads: 89

```
Someone thought the customer doesn't need access to the SWD and saved a bit on cost...
It's only on the PCB, you need to solder on some cable after opening the device. Make sure to replace the heat pad when re-assembling the unit. Buy the good stuff, 5Wmk.....
```

---
## \#46 Posted by: Andy87 Posted at: 2018-09-14T05:12:34.522Z Reads: 91

```
In case you didn’t already solved it, here you need to connect 
![image|690x496](upload://3VRevpWO3FzHvUcTEaejPp9Jf28.jpeg)
```

---
## \#47 Posted by: Eboosted Posted at: 2018-09-14T05:39:25.944Z Reads: 89

```
@Andy87 thanks a lot for your help

I was able to connect the FocBox to the ST Link, here is some usuful information in case someone uploads an incorrect firmware to his FocBox in the future.

1. If you get the message "Can not connect to target" on ST Link software is because, in addition to the 4 wires to the ST Link (RST, CLK, SWDIO and GND), you need to power on the VESC.

![97cd74bf-29f5-42ba-9250-af1bd38697a9|690x388](upload://7HeOjJnkl7w6qSotcNV3ugSticx.jpg)

2. You  need to flash not only the Bootloader but the firmware, use the same method than when flashing the HEX bootloader file but select the the 4.12V firmware downloded from [here](https://github.com/vedderb/bldc-tool/blob/master/firmwares/hw_410_411_412/VESC_default.bin)
```

---
## \#48 Posted by: craigthemachine Posted at: 2018-10-05T22:32:18.471Z Reads: 78

```
@Eboosted where can i get the HEX bootloader file?
```

---
## \#49 Posted by: taz Posted at: 2018-10-07T16:38:52.116Z Reads: 74

```
I think this is the link

http://vedder.se/forums/download/file.php?id=6&sid=a6b085428455d0f9a617d880da259517
```

---
## \#50 Posted by: craigthemachine Posted at: 2018-10-07T17:14:21.449Z Reads: 74

```
Thanks, found it yesterday.
```

---
## \#51 Posted by: GinjaNinja Posted at: 2019-11-18T00:10:28.003Z Reads: 14

```
[quote="taz, post:49, topic:34810"]
http://vedder.se/forums/download/file.php?id=6&sid=a6b085428455d0f9a617d880da259517
[/quote]

This link isn't working for me. I get this error saying the file is unable to be delivered.
```

---
