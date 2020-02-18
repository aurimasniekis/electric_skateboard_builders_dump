# Help with VESC needed

### Replies: 14 Views: 363

## \#1 Posted by: AgileCow Posted at: 2018-07-12T17:26:59.911Z Reads: 92

```
Can you help a fellow in need? I am unsure as to wtf is happening with my VESCs 4.12 from esk8.de (1.2 version)

I had the setup up and running in BLDC mode using the BLDC tool, dual VESCs over CAN-bus. I wanted to upgrade firmware and move to the VESC tool since I am more comfortable in that tool.
I verified that things were indeed working on both VESCs at this point.

I opened up VESC tool 0.94, picked the "410 & 411 % 412" firmware, pressed upload FW on it, upload went ok, VESC powered down. Never came back on. Recycled power with on/off switch.
VESC came back on, connected in VESC tool again, no firmware upgrade was done. Did the same exercise again, but pulled the plug on the VESC (waited about 1min), now it’s not coming back up at all, and I cannot connect to the slave VESC that was connected over CAN-bus either… Ideas?
```

---
## \#2 Posted by: rich Posted at: 2018-07-12T20:58:42.270Z Reads: 75

```
If the FW upload doesn't work you need to install the bootloader first in VESC Tool (my esk8 1.1 controller had bootloader installed, strange). But try FW upload again to get sure it's not possible to upload before installing bootloader.

So one of the controllers is not working anymore or you just can't connect to the slave via CAN bus?

Was the CAN bus cable between the vescs connected and only one vesc powered on?
```

---
## \#3 Posted by: AgileCow Posted at: 2018-07-13T05:06:29.054Z Reads: 64

```
Hi Rich!

Thanks for the input, here's some answers:

* None of the VESCs work anymore
* Correct

I have talked to @sMATTEr (at least I think that's his nick here) about it and he has made the remote diagnosis that I managed to fry the DRV and the u40 chip. 

I also learned that it's a Very Bad Idea™ to disconnect one VESC from power while they are connected over CAN, i.e. sure way to fry them. 


First time working with the VESC4, I sure learned some things :-) So the units are going away for a repair at Mattias' place today.
```

---
## \#4 Posted by: pat.speed Posted at: 2018-07-13T05:13:02.581Z Reads: 56

```
Yep disconnecting one while connected over can will do it. That’s quite a common problem new users have. Hopefully you can get back out riding soon
```

---
## \#5 Posted by: AgileCow Posted at: 2018-07-13T05:16:03.944Z Reads: 54

```
@pat.speed not to worry, I have a backup board ;-) This was a project for me to learn more about other types of components. My other build is based around Trampa stuff and VESC6. 

So far I have to say that the VESC6 is very robust, yet pricey in comparison. It's going to be an experience actually riding the esk8.de 1.2 in this build to comapare performance :slight_smile:
```

---
## \#6 Posted by: sMATTEr Posted at: 2018-07-13T05:28:39.530Z Reads: 54

```
I’ve said it before and I’ll say it again, cattle should not tamper with electronics :wink:

There should be a big red sticker with canbus info, this seems to happen alot.
```

---
## \#7 Posted by: AgileCow Posted at: 2018-07-13T05:34:09.709Z Reads: 53

```
Haha! Well, normally I like to fidget with electronics and I have made a couple of Arduino projects, set up a couple of controllers for temperature controlling my homebrewing system. 

A reflection though, the VESC has a steep learning curve, and there is not one place where the best practices are gathered, correct? That would have massively helped me out to have when starting.

Maybe we should build one?
```

---
## \#8 Posted by: sMATTEr Posted at: 2018-07-19T19:14:24.380Z Reads: 44

```
So I’m having some problems with one of the vescs after canbuschip and drv replacement. One of them works fine.

The vesc connects to the computer, I upload the new firmware to the vesc - 100%. The vesc does not reboot and the green light turns off. It starts and connects again after i reboot it. But it it’s back to the old 2.18fw.

I’m getting a st-link to check if the mcu works or not and if I’m able to upload the firmware from there.

@Martinsp @JohnnyMeduse I know you guys probably came across this before. Any clue on why this happens?
```

---
## \#9 Posted by: JohnnyMeduse Posted at: 2018-07-19T19:16:37.634Z Reads: 40

```
What brand of vesc do you have ? sound like there is no bootloader
```

---
## \#10 Posted by: sMATTEr Posted at: 2018-07-19T19:30:43.437Z Reads: 40

```
[quote="JohnnyMeduse, post:9, topic:61669, full:true"]
What brand of vesc do you have ? sound like there is no bootloader
[/quote]

It’s a esk8.de vesc. I tried uploading a bootloader from the vesctool. No luck.

I guess st-link is my only option?
```

---
## \#11 Posted by: Martinsp Posted at: 2018-07-19T20:18:56.430Z Reads: 38

```
If the VESC works correctly with the old firmware, the MCU is ok, just the bootloader is missing. That can be solved easily  https://www.electric-skateboard.builders/t/2x-vesc-4-12-2016-from-enertion-not-connecting/60816/7 I posted the bootloader file in this thread you can download it and flash it on with the ST link just like you would a firmware.
```

---
## \#12 Posted by: sMATTEr Posted at: 2018-07-20T05:44:27.917Z Reads: 31

```
Thanks, appreciate it! I’ll try a old bldc tool. :sunglasses:
```

---
## \#13 Posted by: Martinsp Posted at: 2018-07-20T08:23:40.576Z Reads: 28

```
Not sure if I understand correctly what you mean but you will need an ST-link V2 and the ST-link utility software to flash the bootloader first, than the desired firmware .hex/.bin file not just older BLDC tool version unfortunately
```

---
## \#14 Posted by: sMATTEr Posted at: 2018-07-20T09:21:18.874Z Reads: 27

```
ST-link it is. :wink:
```

---
