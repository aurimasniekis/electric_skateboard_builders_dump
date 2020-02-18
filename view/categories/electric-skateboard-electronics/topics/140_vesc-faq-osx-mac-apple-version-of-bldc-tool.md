# VESC FAQ &#124; OSX MAC APPLE Version of BLDC tool

### Replies: 72 Views: 11074

## \#1 Posted by: onloop Posted at: 2015-08-26T04:33:55.714Z Reads: 531

```
Download this file to Install the BLDC Tool on your Apple Computer. 

This link will stay updated with the latest compatible BLDC tool & firmware version.

https://drive.google.com/open?id=0Bym9XrdeViekVG9vQUU1S2ljT2s
```

---
## \#3 Posted by: Moja Posted at: 2015-10-28T03:36:25.569Z Reads: 417

```
Hi Jason, I have the VESC 4.7, do I need to install the firmware through terminal on Ubuntu as shown on Vedder's walk through on his site or does it have firmware pre installed? I have bought a discovery board to upload the firmware but could do with some guidance on how I need to go about these final steps of setting up VESC using my Mac. 
Cheers!
```

---
## \#4 Posted by: onloop Posted at: 2015-10-28T11:54:15.751Z Reads: 396

```
hey, the firmware should be loaded already. just need to make sure you have correct BLDC tool version. its not backwards compatible.

I must admit i am rather novice when it comes to all this firmware & loading stuff onto chips..

let me see if i can find out more
```

---
## \#5 Posted by: Moja Posted at: 2015-10-28T12:48:40.527Z Reads: 357

```
Cheers, is the BLDC version you posted in this threat the right one for the 4.7 VESC's?
```

---
## \#6 Posted by: elkick Posted at: 2015-10-28T17:03:58.655Z Reads: 343

```
Yes it is. If you need to update  the firmware you'll find the mc_config&FW.zip here: https://drive.google.com/folderview?id=0Bym9XrdeViekfkRETmRndENkcVpySW5sWjIzOWdrLThCY01HY3BPOXpqYVRHUlQxS0R5ZlU&usp=sharing

Within that zip you need to choose the default FW for 4.7.when asked in the BLDC tool (tab Firmware -> chose)
```

---
## \#7 Posted by: Moja Posted at: 2015-10-31T03:57:52.448Z Reads: 314

```
Thanks. I have uploaded the 1.14 default firmware to the VESC through BLDC, I get the message "connected, limited" then "no firmware read response" in the bottom right corner when trying to connect to the VESC. I assume there is a problem with uploading the firmware.
Any suggestions? 

Cheers, 
Moja.
```

---
## \#8 Posted by: elkick Posted at: 2015-10-31T08:13:08.652Z Reads: 294

```
Did you upload the FW through the FW-tab in the BLDC-Tool?
Also, it could be the case that the bootloader (needed to update the FW) is not correctly installed. If this is the case you'd need a STlink V2 to upload it. Sounds complicated, but it is not - just follow Benjamin's instructions on his page how to connect the STlink to the VESC and how to upload the BL. You'd need Ubuntu though (could be installed on a thumb drive too).

Edit: if you are in Europe you could send it to me and I'd do that for you!
```

---
## \#9 Posted by: Moja Posted at: 2015-11-02T22:07:57.924Z Reads: 276

```
Cheers, I though I was going to have to go through that process in the first place so I've bought the gear needed to upload the firmware manually, I'll get cracking on that :)
```

---
## \#10 Posted by: siggs3000 Posted at: 2015-11-12T03:10:01.965Z Reads: 265

```
ok this is a possibly dumb question but I've been staring at the Mac BLDC tool for about 15 straight minutes and I can't find the "connect" button anywhere! I hate to post this but can anyone help me out? I've got it connected via USB at the moment. And the BLDC tool from the link at the top of this thread.
```

---
## \#11 Posted by: onloop Posted at: 2015-11-12T03:12:30.805Z Reads: 250

```
should be at top right hand side.
```

---
## \#12 Posted by: siggs3000 Posted at: 2015-11-12T03:22:12.549Z Reads: 249

```
Gah, it opened up perfectly cut off on the right side of the screen so I didn't see that whole right pane. Thanks @onloop

I think I need to read up on how to use this though. I thought I could just connect it to my computer via USB and update the settings (to use the nunchuck for instance) but I think I need a programmer between the computer and the vesc. Is that right?
```

---
## \#13 Posted by: chaka Posted at: 2015-11-12T03:29:44.148Z Reads: 236

```
You may have to resize your screen. Sometimes the right hand side and the bottom section of the bldc tool will be hidden.

Edit: nevermind you got it! :stuck_out_tongue:
```

---
## \#14 Posted by: onloop Posted at: 2015-11-12T03:34:29.291Z Reads: 236

```
you don't need a programmer
```

---
## \#15 Posted by: onloop Posted at: 2015-11-12T03:34:52.185Z Reads: 230

```
READ ALL THIS :)
http://www.electric-skateboard.builders/search?q=vesc%20faq
```

---
## \#16 Posted by: siggs3000 Posted at: 2015-11-12T07:48:02.429Z Reads: 237

```
Ok that first question was embarrassing... I'm actually a software engineer! lol 

I've been reading up now all night on here and on Vedder's site but having a bit of trouble now that I've found the connection fields and buttons. The VESC is wired up and lighting up it's cool shade of blue and looking good thus far. 

What values should be in the connection fields to be able to "connect" via USB. If I leave the default value of: `/dev/tty.usbmodem261` in there, it says `Device not found` so I'm assuming there's a different value that should be in there.
```

---
## \#17 Posted by: chaka Posted at: 2015-11-12T08:09:28.814Z Reads: 228

```
Try      /dev/ttyACM0
If you have more than one usb device then you need to type in the port that the VESC is plugged into. I am linux user so I may not be of much help finding the port ID. 

Edit: Sorry, I realized the the port ID I gave you is probably PC specific.  The green light should be on too.
```

---
## \#18 Posted by: siggs3000 Posted at: 2015-11-12T17:04:52.447Z Reads: 234

```
@chaka - The green light is on too. I'm assuming that you should have the power connected to the VESC while it's connected to USB, right? 

If I do that, connect the USB and then open a terminal and run: `sudo dmesg | tail`, 

I get this: 

```USB (XHCI Root Hub USB 2.0 Simulation):Port 2 on bus 0xa connected or disconnected: portSC(0xe0206e1)``` (if that helps to figure out what address I need to put in the connection field. 

I've worked with Arduino and Raspberry PI but they usually autodetect the port so this is uncharted for me.
```

---
## \#19 Posted by: chaka Posted at: 2015-11-12T17:20:24.710Z Reads: 223

```
I have walked a few of my customers through configuration on os x but we never had any usb port issues. Do you have any other devices plugged in? If you do, you might try disconnecting everything and trying again with just the vesc. Hopefully jacobbloy will chime in with a solution if that does not work.
```

---
## \#20 Posted by: siggs3000 Posted at: 2015-11-12T17:33:53.896Z Reads: 231

```
Thanks again. It's currently the only usb device plugged in. I may just try to connect it to a PI and use the Linux version since there's much more documentation for that setup. If I can't figure out the OS X issue by later today, I'll five that a go.
```

---
## \#21 Posted by: treenutter Posted at: 2015-11-12T17:50:06.824Z Reads: 239

```
[quote="siggs3000, post:18, topic:140"]
you should have the power connected to the VESC while it's connected to USB, right?
[/quote]

@siggs3000 That's correct.
```

---
## \#22 Posted by: treenutter Posted at: 2015-11-12T17:54:46.526Z Reads: 226

```
@siggs3000 are you using the correct version of BLDC Tool? If the firmware on your VESC is older than the BLDC Tool version that you're using (1.10, 1,12, etc) you'll have issues (although I'd be surprised if this is causing a connection issue w your usb port).
```

---
## \#23 Posted by: siggs3000 Posted at: 2015-11-12T18:54:09.894Z Reads: 210

```
I believe so. I have the newest Enertion VESC and the BLDC build from the link at the top of this thread.
```

---
## \#24 Posted by: onloop Posted at: 2015-11-12T22:03:20.451Z Reads: 213

```
@jacobbloy might be able to help you with this, he uses mac.

make sure the vesc has power running to it from battery or dc power supply, then plug in usb, it should detect.

on windows it normally needs to install a driver for the ST chip, then its ready to go.

try a few different usb cables.
```

---
## \#25 Posted by: cmatson Posted at: 2015-11-12T22:17:34.887Z Reads: 210

```
I'd also try switching out the USB cable if you can.v  know I have multiple different usb B cords, and not all of them work with the VESC, or my camera- 

They are more than just power, but for some reason, there are just some that don't play nice with some of my devices... 

I'm on OSX too by the way
```

---
## \#26 Posted by: jacobbloy Posted at: 2015-11-12T22:53:51.418Z Reads: 191

```
@siggs3000  Change the port from 261 to 301

When I did the pull request on git the standard was 261 so I set that for default I'll look at changing it or adding a drop down box, if it ever doesn't connect you need to check the port in terminal.

Open up terminal  copy this code

CODE: SELECT ALL
ls /dev/tty.*
to find the usb device name it falls under a usb bluetooth device but you will see it like this 
CODE: SELECT ALL
screen /dev/tty.[yourSerialPortName]
copy and past it into BLDC tool in the port section and click connect!

standard are /dev/tty.usbmodem261 or as i said /dev/tty.usbmodem301

i have added a read me file to the OS X FW1.14 

FW2.0 will be out soon i have a copy of it along with BLDC TOOL but vedder is still making a lot of updates with FOC as soon as that is out i will update OS X and WINDOWS BLDC TOOL
```

---
## \#27 Posted by: siggs3000 Posted at: 2015-11-12T23:26:49.419Z Reads: 170

```
Thanks a million, @jacobbloy

I ran  `ls /dev/tty.*` and sure enough it was port 301. I updated the value in the connect field to `/dev/tty.usbmodem301` and I'm connected and on my way. Firmware recognized and all. 

Hope this thread helps some other Mac users out there. Thanks again!
```

---
## \#28 Posted by: jacobbloy Posted at: 2015-11-12T23:36:12.406Z Reads: 159

```
@siggs3000 your welcome!
```

---
## \#29 Posted by: Alex Posted at: 2015-11-22T01:38:54.739Z Reads: 158

```
Im new to this community but I was wondering if you guys could help me out. 
I currently have the most recent El Capitan 10.11.1 software.
When attempting to open ._BLDC_Tool FW1.14.app I get the error message "You can’t open the application “_BLDC_Tool FW1.14-3.app” because PowerPC applications are no longer supported"

Is there a simple fix for this or am I required to dual boot with linux or Microsoft?
```

---
## \#30 Posted by: King1017 Posted at: 2015-11-22T03:20:07.842Z Reads: 144

```
On Mac the first time you launch it you have to right click it, then press open when the dialog box opens. Then it will give you a warning, just say ok and you should be good to go.
```

---
## \#31 Posted by: lox897 Posted at: 2015-11-22T09:20:08.142Z Reads: 141

```
Do you have it in the applications folder when launching?
```

---
## \#32 Posted by: siggs3000 Posted at: 2015-11-22T19:14:27.227Z Reads: 138

```
A lot of applications are running into this issue on El Capitan. Don't move it from it's download folder (don't put it in Applications) and then right click and choose "open" on it and it should work. After you run it the first time, you can move it into Applications if you want and that should be ok.
```

---
## \#33 Posted by: lox897 Posted at: 2015-11-22T20:18:45.414Z Reads: 136

```
I have El Capitan. I downloaded it. Opened it. Allowed it. Error. Move to Applications folder. Works!
```

---
## \#34 Posted by: siggs3000 Posted at: 2015-11-22T20:20:58.198Z Reads: 133

```
Oh nice. It was opposite for me and the same error for Spotify. Looks like @lox897 way works for this one!
```

---
## \#35 Posted by: lox897 Posted at: 2015-11-22T20:33:55.043Z Reads: 136

```
Yep! Try my way! Hehehe
```

---
## \#36 Posted by: Alex Posted at: 2015-11-23T01:42:03.023Z Reads: 142

```
Thanks everyone for the help. I am still unable to open BLDC tool unfortunately. I attempted to open the file as suggested and still the same issue. 
I noticed there are 2 folders to choose from after unzipping. One named __BLDC_Tool FW1.14.app and the other named BLDC_Tool FW1.14.app so I tried the second one and now it displays  BLDC_Tool FW1.14.app quit unexpectedly
```

---
## \#37 Posted by: Alex Posted at: 2015-11-23T01:44:18.575Z Reads: 137

```
I may just wait until I have access to a PC because I feel it may be an issue with my computer
```

---
## \#38 Posted by: cmatson Posted at: 2015-11-23T04:34:44.557Z Reads: 156

```
[quote="Alex, post:37, topic:140, full:true"]
I may just wait until I have access to a PC because I feel it may be an issue with my computer
[/quote]

I used the OSX BLDC tool for the previous version(because I just downloaded it, and it worked without any troubleshooting), but then dug out my old windows laptop to use version 1.14.

It's not that I don't like the OSX version, it's just that so far I've heard tons of people say the windows version "just works", while the OSX one takes a little more fine tuning here and there. And it does just plain work by the way.. even on my super old p.o.s laptop, it ran just fine. 

litterally, if you just download the windows BLDC here:
http://www.electric-skateboard.builders/t/vesc-faq-windows-version-of-bldc-tool/141
it takes less than 10 minutes from downloading the file, to setting up your VESC. There is one driver (needed to run 1.14) that you need to install (easily labeled in the "BLDC Drivers" folder), and then it is just running the program (again, super easy to find) and you are in business!
```

---
## \#39 Posted by: trbt555 Posted at: 2016-01-15T10:56:23.244Z Reads: 140

```
[quote="jacobbloy, post:26, topic:140"]
@siggs3000  Change the port from 261 to 301
[/quote]

Is there any way of setting port 301 by default, other than recompiling the code ?
```

---
## \#40 Posted by: jacobbloy Posted at: 2016-01-15T11:27:36.366Z Reads: 146

```
Yes, as I set the default to 261 originally.

In the source code, open main window.cpp

The do a find search for /dev/tty.usbmodem261 then replace 261 with 301, but next updat I will change it to 301, or implement a way that it tries both.
```

---
## \#41 Posted by: jacobbloy Posted at: 2016-01-15T12:47:43.991Z Reads: 149

```
Please download FW2.8 again, Iv added a second field, so if the first fails then the second is tried, please download it and test it.
```

---
## \#42 Posted by: trbt555 Posted at: 2016-01-15T15:07:23.090Z Reads: 138

```
The tool now connects to port 301 without having to type it. Thanks.
I assume other functionality remains unchanged.
```

---
## \#43 Posted by: jacobbloy Posted at: 2016-01-15T23:20:15.896Z Reads: 137

```
Every thing will work the same!
```

---
## \#44 Posted by: jacobbloy Posted at: 2016-01-29T05:45:08.102Z Reads: 144

```
Recently i have setup a website for the use of downloading of BLDC-TOOL for windows and OS X and all VESC related Firmware and files, this link will soon be a fully set up website with active download links, support documents and videos as well as offering vesc support via remote access and video call.
the new link for BLDC-TOOL updates is:

http://www.vesc.support  or
http://www.bldc-tool.support

if any one has the knowledge and wants to help me set this website up that would be great i will pay maybe in vesc!

also BLDC TOOL 2.10 is know available
```

---
## \#45 Posted by: jacobbloy Posted at: 2016-02-09T04:49:02.950Z Reads: 135

```
check my latest updated OS X version of bldc tool.

http://vesc.support

iv actually been working on the installer so know it packed in a DMG
NEW:
if you plug in your vesc before loading bldc tool then bldc tool automatically detects the vesc and sets the correct serial port while tagging that serial port (vesc) so the user knows its detected. you simply just click connect. soon ill add auto connect.
there is also a refresh button that locates the vesc just incase you didn't plug it in before opening.

this is all apart of trying to reduce confusion with 261 and 301 address.

I'm about 2 weeks away from finishing a bldc tool esc setup wizard that will have a single button to detect foc and bldc settings and app data to make it easy for customers with no knowledge.

please every body i need feed back on my site.
```

---
## \#46 Posted by: onloop Posted at: 2016-02-09T04:50:15.249Z Reads: 125

```
fucking awesome!... the simpler the better.
```

---
## \#47 Posted by: trbt555 Posted at: 2016-02-09T06:04:21.943Z Reads: 122

```
With all due respect @jacobbloy, I do not see the need for an OSX installer.
If anything it just adds overhead.
As far as I can see, the tool already came with all dependencies and doesn't require registering anything with the OS.
Clean, simple, easy to delete and replace by a next version. Click-and-play.
I understand this may make things easier for new users. I assume we'll still be able to extraxt the executble and the dependencies ?
Are these code changes being published on Github ?
```

---
## \#48 Posted by: jacobbloy Posted at: 2016-02-09T06:25:32.930Z Reads: 122

```
All i said @trbt555  is that OS X is know packed in a DMG, which in my opinion is better then a zip file and shows a degree of professionalism.

OSX is easy because all dependancies all packed in the .app and cam be extracted very easy.

the main work i have been doing with installation is for windows where drivers where required and there is more to do then simply double click like in OS X's case.

all changes that i have made to the serial ports vender id detection will be published to github as soon as vedder accepts the pull request.
```

---
## \#49 Posted by: trbt555 Posted at: 2016-02-09T06:35:03.016Z Reads: 117

```
I see, thanks.
I was under the impression you'd made an OSX installer.
Good work.
```

---
## \#50 Posted by: trbt555 Posted at: 2016-02-09T12:20:51.963Z Reads: 123

```
Slightly off topic: wouldn't it be great if the BLDC tool would be able to save entire configs (not just the MCC config, but also the app configs) to XML ? That would make swapping VESC's and even sharing configs so much easier.
Also, wouldn't it be great if you click READ CONFIG, BLDC reads the whole config (also the app configs) and populates all tabs with only one click ? I've always found this clunky.
```

---
## \#51 Posted by: onloop Posted at: 2016-02-09T14:36:02.508Z Reads: 122

```
I have always thought a beginner's and advanced version of BLDC should exist. 

The begginers interface could be very simplified. It could have scripts that run all the seperate tasks In the background but make it automated one button stuff on the front end....maybe have sliders or dials that represent the range of data that you can or should choose.. out of the 100+ parameters available in BLDC we only ever tend to change 6 or 8 of them anyway. So they should all be on one screen. Save them all together once configuration is done, one save button. Load them all in one go from presets.
```

---
## \#52 Posted by: BigAl Posted at: 2016-02-09T17:04:58.646Z Reads: 119

```
@jacobbloy Thanks for the work you put into this community!

Al...
```

---
## \#53 Posted by: arpitdave Posted at: 2016-04-01T03:08:11.611Z Reads: 120

```
[quote="elkick, post:8, topic:140"]
could
[/quote]

did you figure this out? if you did what did you do. i have same problem
```

---
## \#54 Posted by: elkick Posted at: 2016-04-01T04:59:43.127Z Reads: 122

```
You are referring to the missing bootloader? If so, an STlinkV2 (8€ at eBay) will do the job, but you have to work with Ubuntu and follow the steps mentioned at vedder.se.
```

---
## \#55 Posted by: rmrf Posted at: 2016-06-13T19:24:57.460Z Reads: 121

```
Are you sure it only works with Ubuntu? I can upload bldc-firmware with OS X and I kinda can upload the bootloader, but it hangs after verifying the checksum OK, is that normal?

    bldc-bootloader/ $ make upload 
    #qstlink2 --cli --erase --write build/BLDC_4_Bootloader.bin
    openocd -f interface/stlink-v2.cfg -c "set WORKAREASIZE 0x2000" -f target/stm32f4x_stlink.cfg -c "program build    /BLDC_4_Bootloader.elf verify reset"
    Open On-Chip Debugger 0.9.0 (2015-11-15-05:34)
    Licensed under GNU GPL v2
    For bug reports, read
    	http://openocd.org/doc/doxygen/bugs.html
    0x2000
    WARNING: target/stm32f4x_stlink.cfg is deprecated, please switch to target/stm32f4x.cfg
    Info : auto-selecting first available session transport "hla_swd". To override use 'transport select <    transport>'.
    Info : The selected transport took over low-level target control. The results might differ compared to plain     JTAG/SWD
    adapter speed: 2000 kHz
    adapter_nsrst_delay: 100
    none separate
    Info : Unable to match requested speed 2000 kHz, using 1800 kHz
    Info : Unable to match requested speed 2000 kHz, using 1800 kHz
    Info : clock speed 1800 kHz
    Info : STLINK v2 JTAG v17 API v2 SWIM v4 VID 0x0483 PID 0x3748
    Info : using stlink api v2
    Info : Target voltage: 3.246592
    Info : stm32f4x.cpu: hardware has 6 breakpoints, 4 watchpoints
    target state: halted
    target halted due to debug-request, current mode: Thread 
    xPSR: 0x01000000 pc: 0x0800c000 msp: 0x20000400
    ** Programming Started **
    auto erase enabled
    Info : device id = 0x10076413
    Info : flash size = 1024kbytes
    target state: halted
    target halted due to breakpoint, current mode: Thread 
    xPSR: 0x61000000 pc: 0x20000042 msp: 0x20000400
    wrote 131072 bytes from file build/BLDC_4_Bootloader.elf in 5.563057s (23.009 KiB/s)
    ** Programming Finished **
    ** Verify Started **
    target state: halted
    target halted due to breakpoint, current mode: Thread 
    xPSR: 0x61000000 pc: 0x2000002e msp: 0x20000400
    verified 4256 bytes in 0.076163s (54.570 KiB/s)
    ** Verified OK **
    ** Resetting Target **
    ^Cmake: *** [upload] Interrupt: 2 <-- Here it hangs and I interrupt it with Ctrl+C
```

---
## \#56 Posted by: hexakopter Posted at: 2016-06-13T20:14:23.998Z Reads: 122

```
That point with the hanging after reset the target is normal. I have the same behavior with my Mac (never tried Linux, just flashed with the Mac) and the firmware upload is completed. After that I can connect to the USB of the VESC normally.
```

---
## \#57 Posted by: Namasaki Posted at: 2016-09-05T00:58:31.783Z Reads: 105

```
Can someone tell me what these settings are for?
And should they be left alone?
<img src="/uploads/db1493/original/2X/b/b9043743d43ad3e39d6bec6a3e2472264b0c39ae.png" width="267" height="405">
```

---
## \#58 Posted by: Jinra Posted at: 2016-09-05T01:07:08.841Z Reads: 105

```
for testing the motor on the bench
```

---
## \#59 Posted by: Namasaki Posted at: 2016-09-05T01:22:45.363Z Reads: 104

```
For like motor detection?
```

---
## \#60 Posted by: Jinra Posted at: 2016-09-05T01:24:02.152Z Reads: 107

```
more so to test the motor with various currents or speeds. You can see if your motor will spin up with lower currents or something.
```

---
## \#61 Posted by: Namasaki Posted at: 2016-09-05T01:26:22.962Z Reads: 115

```
I don't get how you would use this panel. What button do you press to activate the motor with these settings?
```

---
## \#62 Posted by: Jinra Posted at: 2016-09-05T01:29:42.228Z Reads: 115

```
If you want to spin it up with current, type the current you want and hit "current" (it's a button)
```

---
## \#63 Posted by: Namasaki Posted at: 2016-09-05T01:33:16.128Z Reads: 122

```
Cool, Thanks for explaining it.
My Vesc's are working great and no problems at all so I'm being very careful and I'm not gonna touch any setting if I don't know what it is.
```

---
## \#64 Posted by: ARollNation Posted at: 2017-01-07T02:29:10.118Z Reads: 103

```
Where could I find the driver to download for that chip on the VESC?
```

---
## \#65 Posted by: arussellsaw Posted at: 2017-04-08T11:08:42.694Z Reads: 92

```
hey! looks like this link isn't working anymore, and i can't get the source to build for some reason :/ would you be able to fix the link?
```

---
## \#66 Posted by: Print3r Posted at: 2017-04-14T13:53:28.562Z Reads: 83

```
The links you have given lead to a 'no DNS' error!
```

---
## \#67 Posted by: robthebuilder Posted at: 2017-04-19T15:07:07.177Z Reads: 89

```
I can't find this BLDC software anywhere. Can somebody help me with a link? Thanks
```

---
## \#68 Posted by: JohnnyMeduse Posted at: 2017-04-19T15:09:36.889Z Reads: 90

```
Look on Enertion web site 😉
```

---
## \#69 Posted by: robthebuilder Posted at: 2017-04-19T15:42:32.601Z Reads: 93

```
Awesome! Thank you :D
```

---
## \#70 Posted by: trancejunkiexxl Posted at: 2017-08-02T21:56:59.208Z Reads: 73

```
vesc fw says 2.54 but bldc says 2.17 2.18.. so limited connection been trying to get it up on mac for settings on the go.. =) 
anybody know how fix?
```

---
## \#71 Posted by: JohnnyMeduse Posted at: 2017-08-02T22:04:58.883Z Reads: 76

```
2.54 Firmware is realted to @Ackmaniac Bldc tool.

 http://www.electric-skateboard.builders/t/extended-bldc-tool-with-watt-control-mode-ppm-cruise-control-individual-throttle-curve-and-android-app/12286?u=johnnymeduse

If you want to use the regular 2.18 BLDC tool you need to reflash the firmware
```

---
## \#72 Posted by: trancejunkiexxl Posted at: 2017-08-02T22:14:38.535Z Reads: 75

```
got it, i was just being stupid =)
```

---
## \#73 Posted by: ChipHerendeen Posted at: 2018-06-13T00:25:33.269Z Reads: 35

```
Just got the BLDC tool loaded on to my computer. Plugged in my VESC (Turnigy sk8 esc, hardware 4.12) and hit "connect", and got this error message: "Serial Port Error: 2". I'm running Mac High Sierra. Really confused here... what am I missing? Vesc is connected to power and my remote is on.
```

---
