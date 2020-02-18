# VESC Firmware update

### Replies: 32 Views: 5694

## \#1 Posted by: Blasto Posted at: 2015-09-25T23:28:02.324Z Reads: 313

```
I got 2 VESC from enertion's August build, they came with the firmware version 1.10 

Now I am trying to update to update to 1.13, the BLDC tool only works with 1.13... What to do? do I need the BLDC tool that is compatible with 1.10 and use it to upload the 1.13 firmware?  (chiken or the egg kind of thing)

My other option is to go through the SWD cable, which is a PITA, my discovery board is at work, 1hr away, kinda hoping to get away with this update via USB.

Thanks~

Charles.
```

---
## \#2 Posted by: jacobbloy Posted at: 2015-09-26T06:13:55.398Z Reads: 311

```
mate you can use the bloc 1.13 software to update the esc.
```

---
## \#3 Posted by: jacobbloy Posted at: 2015-09-26T06:18:04.139Z Reads: 301

```
when i update the windows and mac software i use the latest software to update the vesc,
but if you need the old version then just download it to from my google drive.

https://drive.google.com/folderview?id=0Bym9XrdeViekfkRETmRndENkcVpySW5sWjIzOWdrLThCY01HY3BPOXpqYVRHUlQxS0R5ZlU&usp=sharing
```

---
## \#4 Posted by: treenutter Posted at: 2015-09-26T11:16:41.955Z Reads: 276

```
@Blasto I would love to know this as well. I couldn't find a version of BLDC Tool for Windows that would read my VESC's firmware. It just reads "old firmware."

@Blasto does BLDC read your firmware version?

I'm wondering if there is any firmware installed on this shipment of VESC. @cmatson was your August Enertion VESC shipped with firmware installed?
```

---
## \#5 Posted by: jacobbloy Posted at: 2015-09-26T15:44:06.956Z Reads: 249

```
Yes they come with firmware installed.

So go plug in your vesc into the latest version of BLDC tool, then click the firmware tab, once your in the tap, there will be a button for you to choose the latest firmware, then can also be downloaded from my google drive link I posted above or direct from here https://drive.google.com/open?id=0Bym9XrdeViekb3lzcGNDdjk4QUU

You click the default.dll file I think it is and then click upload, wait maybe 30 seconds and bam your vesc will know work with BLDC tool.

If you don't want to update the firmware (not recommended) then just down load BLDC Tool fW 1.10 here is the link exactly to that version or get it from the first link I posted.
https://drive.google.com/open?id=0Bym9XrdeViekdmZHRm5pTmpUMVU
```

---
## \#6 Posted by: cmatson Posted at: 2015-09-26T16:06:02.749Z Reads: 224

```
ya, mine came pre loaded with v1.10, and I have just used the v1.10 BLDC tool.
```

---
## \#7 Posted by: Blasto Posted at: 2015-09-26T18:08:11.353Z Reads: 216

```
In the BLDC tool, I click on the firmware tab, i choose the proper bin file. /BLDC/BLDC/bldc-tool/firmwares/hw_46_47/VESC_default.bin

hit upload, the progress bar progresses to the end, the usb disconnects, then I power cycle the VESC, reconnect the USB... still version 1.10 :\

@jacobbloy i'll try out your links and let you know the results

Thanks!
```

---
## \#8 Posted by: Blasto Posted at: 2015-09-26T18:14:48.122Z Reads: 195

```
@treenutter yes I am able to read the FW version, sadly I can't post a screen shot being a new user and all.

im using ubuntu, i'll try the windows version
```

---
## \#9 Posted by: elkick Posted at: 2015-09-26T18:45:46.262Z Reads: 187

```
Same here, it's locked at FW1.10. Tried it with Ubuntu, OSX and Win, but after reconnect it's still on 1.10. Doesn't accept anything else above.

At the end it's not s big thing to stay with it that way and using BLDC on 1.10, but the Enertion VESC is the only one I have which is behaving like this (I have some more from Benjamin and Marcin too).
```

---
## \#10 Posted by: jgeating Posted at: 2015-09-26T20:33:44.636Z Reads: 182

```
Same thing here. Tried in Ubuntu 14.04 and Windows. Says firmware finished uploading, then I can no longer connect to the board. Have to remove power (not just usb). When I reapply power and reconnect, it is still at v1.10. I'm going to try it with the other 3 I bought, but I'm not too hopeful. I'll just use v1.10 for now then. Glad someone posted this, I was really banging my head against the wall thinking I was the only one who couldn't get these to work.
```

---
## \#11 Posted by: Blasto Posted at: 2015-09-26T21:08:03.120Z Reads: 177

```
So i tried with the windows version of the BLDC tool, same result, stuck at 1.10

Drove to work, picked up my discovery board, drove back and success! now at FW 1.13, through the SWD

I did have to retry a couple of times when I loaded the bootloader, maybe this could be the issue, the bootloader was not properly flashed?
```

---
## \#12 Posted by: jacobbloy Posted at: 2015-09-26T22:39:17.454Z Reads: 169

```
I would say it is that the bootloader didn't flash, I have some very cheap stlinkv2 I can get if any one needs it!

One thing I could suggest is to try BLDC tool 10.12 or BLDC tool 10.10 to try and load the newer firmware, it could be an error with BLDC tool version 1.13! But I think it's the bootloader!
If any one doesn't have the ability to install Linux but is OK buying a cheap stlinkv2 (good thing to have with the vesc! ) then I have access to software that I can load the bootloader for you!
```

---
## \#13 Posted by: treenutter Posted at: 2015-09-28T13:57:17.766Z Reads: 166

```
@Blasto I figured out my issue; I was using an unsupported version of windows (my "shop" laptop that I don't care for very well). Once I tried on Windows 8.1, BLDC Tool recognized my VESC and its firmware.

Thx @cmatson; this was a very helpful clue!
```

---
## \#14 Posted by: treenutter Posted at: 2015-09-28T14:00:51.681Z Reads: 162

```
@elkick @Blasto @jacobbloy @jgeating I've got the same issue with the same VESC; I can't seem to update the firmware. I'll try with BLDC Tool 10.12 and 10.10 later tonight; it definitely didn't work w BLDC Tool 10.13.
```

---
## \#15 Posted by: Blasto Posted at: 2015-09-28T14:34:33.485Z Reads: 156

```
@treenutter if you're able to get your hands on a discovery board and flash only the bootloader, then try to update the fw using the bldc tool, the root cause would be isolated.
```

---
## \#16 Posted by: elkick Posted at: 2015-09-28T14:38:34.850Z Reads: 149

```
I ordered a stlink v2 locally and will try it as soon as it arrives. FW1.10 works good, but I'd like to be able to update to future versions. :smile:
```

---
## \#17 Posted by: treenutter Posted at: 2015-09-28T19:27:11.299Z Reads: 156

```
Thx @Blasto I'm looking for the changelog to see if there is anything significant in 1.13 that I need. So far 1.10 is working very well; although I'd hate to miss out on all the future updates. Updating VESC with new additions is going to be half of the fun I think!

@elkick please let us know how it turns out.
```

---
## \#18 Posted by: jacobbloy Posted at: 2015-09-29T05:53:03.610Z Reads: 152

```
hi every one, jason is on holidays but we have to apologise that the bootloader is the problem, when uploading 100+ esc's a few of them didn't upload correctly, as i have said if you can not install linux i can upload it for you remotely but you will need an stlinkv2 i have about 10 in stock and i can send you one free just pay for shipping.
```

---
## \#19 Posted by: elkick Posted at: 2015-09-30T12:25:53.309Z Reads: 157

```
Received the stlinkv2 today and it took me just 10 min. to get the bootloader flashed - no big deal and really easy! All the information are on vedder.se, it didn't even require to power the VESC on, just connect the stlinkv2 and follow Benjamins instruction for bootloader creation and upload under Ubuntu. 

And a big thanks to you Jacob, for providing always the latest OSX and Win versions of the BLDC tool! That's really convenient and I am sure a lot of people are very happy about it, but never giving you feedback. I know a hand full of guys using your BLDC versions here in Germany, and they're very happy not being forced to install Ubuntu!

Just on a side note: maybe you'd like to add the missing FW1.13 file in the current OSX Version on google drive? That would be nice.
```

---
## \#20 Posted by: jacobbloy Posted at: 2015-09-30T13:22:38.347Z Reads: 153

```
all updated mate and thanks for the support. just a shout out if any one has a motor config file that they want to send me shoot it over, ill add it to the collection.
```

---
## \#21 Posted by: Blasto Posted at: 2015-09-30T14:48:10.292Z Reads: 145

```
[quote="elkick, post:19, topic:237"]
t didn't even require to power the VESC on, just connect the stlinkv2
[/quote]


This is interesting, maybe during the manufacturing process, the bootloader should be loaded before the fw, to avoid any contention on the SWD. Because i did retry loading the bootloader 3-4 times before it passed.

I'll make a new thread of my project i am building when i receive my parts back from anodizing. It has nothing todo with skateboards, but i am using the  vesc, with a high kv motor (2000 kv)

I'm building a Japanese style sumo robot for the upcomming event in Tokyo december 13th
```

---
## \#22 Posted by: elkick Posted at: 2015-09-30T18:22:47.258Z Reads: 130

```
I'm curious to see your project, sounds really special!

I think you're right about the VESC bootloader.It should indeed be flashed before booting up the device else the FW would prohibit the overwriting of the bootloader.
```

---
## \#23 Posted by: claudiofiore88 Posted at: 2015-09-30T18:42:58.963Z Reads: 130

```
I ordered two VESC's from @onloop, from their October batch. Is this something I'm gonna have to worry about?
```

---
## \#24 Posted by: elkick Posted at: 2015-09-30T20:08:00.716Z Reads: 125

```
I don't think so since it's a new batch and I ordered one too. 😉
```

---
## \#25 Posted by: cmatson Posted at: 2015-09-30T20:10:35.794Z Reads: 125

```
I'm getting one too- I guess we won't know until we have them, but the current vesc is a success, so I can only imagine the next version will be even better.
```

---
## \#26 Posted by: sl33py Posted at: 2015-09-30T22:03:54.132Z Reads: 127

```
x-post from Vedder as i'm not sure he's on this forum:
[quote="vedder"]I just tested hw4.8 on my rc buggy with lizards 1717 motor (the most difficult testing platform I have access to right now) and it is a big improvement over 4.7 for sure. I have changed the shunts to 0.5mOhm to allow higher current and set the current limit to 120A. Even without extra capacitors there were no drv faults. With 4.7 I would get drv faults at that current now and then even with extra capacitors (these were nor permanent though and got reset after one second). The bad news is that the current offset is still there, but it is better than before. This means that v4.8 is better than 4.7 in every possible way, so if you want to order something now I strongly recommend 4.8.

Regarding the current offset that is not solver completely yet, I have an idea about a routing update. If I have time I will fix that tomorrow and order v4.9 tomorrow for testing. It should then arrive in a few weeks.

I also have a BLDC motor with an encoder now, so I will try to get started with FOC this weekend. The plan is to first make it work with an encoder then implement a sensorless observer.[/quote]

I am hoping to get some 4.8 boards at some point, but might wait for 4.9 if it helps with the current offset (not 100% sure what that does...).  Luckily i have 5 VESC's currently so backups.  (also have 4 boards - 2 are dual motor).
```

---
## \#27 Posted by: jacobbloy Posted at: 2015-10-08T03:38:25.684Z Reads: 120

```
hi mate, this October batch will not have this problem, Jason and i will be uploaded the FW and bootloader our self's last time it was the factory. the october build will be 4.8 but if you have interest in v4.10 then i would contact jason i think he was looking to get some made asap.

any contributions help i would love if you contribute to benjamin him self but i do spend  bit of time preparing these files.

but the real reason for this post FW1.14 is know out so i have update windows and OS X bldc tool to work. 
as always i have left v1.13 available and the others.
[url]https://drive.google.com/folderview?id=0Bym9XrdeViekfkRETmRndENkcVpySW5sWjIzOWdrLThCY01HY3BPOXpqYVRHUlQxS0R5ZlU&usp=sharing[/url]

i had a problem with v1.13 not allowing me to do motor detection but I'm yet to test if v1.14 fixes this.
```

---
## \#28 Posted by: Moja Posted at: 2015-11-01T22:08:22.596Z Reads: 118

```
I am trying to update my VESC firmware from 1.1 to 1.4. I have a discovery board with stlinkv2, how do I flash the bootloader? I have no idea what the latter 2 terms mean. 

Thanks, 
Moja.
```

---
## \#29 Posted by: elkick Posted at: 2015-11-02T09:36:21.902Z Reads: 121

```
You need to go through the steps described here (firmware and bootloader section): http://vedder.se/2015/01/vesc-open-source-esc/

Prior to this you need to do the steps described in the preparation section.
```

---
## \#30 Posted by: Stielz Posted at: 2016-01-06T03:43:50.210Z Reads: 121

```
I have the same issue where it says the FW update is complete but it doesnt actually change the FW firmware version. Same thing happened last time I updated too. Looks like i'll be flashing with the ST link again. 

I'd like to know how to fix this problem though, its a PITA having to take the VESCs out for flashing. Would've thought that flashing through the ST link last time I had the issue would have fixed any problems with the bootloader but seems not. Any ideas on how to fix it? I've tried on windows 7 and 8
```

---
## \#31 Posted by: Blasto Posted at: 2016-01-06T04:09:11.726Z Reads: 127

```
i loaded the boot loader with linux and a discovery board and follow the steps described by @elkick
```

---
## \#32 Posted by: Stielz Posted at: 2016-01-07T01:30:40.789Z Reads: 122

```
On that note, does anyone have the complied bootloader file handy? I dont have access to a linux computer to compile it myself..
```

---
