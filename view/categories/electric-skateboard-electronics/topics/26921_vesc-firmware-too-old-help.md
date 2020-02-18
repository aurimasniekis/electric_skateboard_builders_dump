# VESC firmware too old? help!

### Replies: 11 Views: 1837

## \#1 Posted by: SpacedOut Posted at: 2017-07-06T16:55:59.228Z Reads: 173

```
Put all my parts together this week and went to start BLDC Tool, but when I try to connect it, it shows me "The firmware on the connected VESC is too old. Please update it using a programmer." I purchased my VESC  from diyelectricskateboard, where it says that the bootloader and firmware is already installed and tested. I am very confused.

I have tried Windows 7 and 10, and many versions of BLDC Tool that I have found around the forums since vesc.net.au is down.
```

---
## \#2 Posted by: psychotiller Posted at: 2017-07-06T17:01:05.045Z Reads: 168

```
This happened to me before too! Be very careful what you do next.  Does it tell you what your firmware is? Safest thing to do would be to find the older version of bldc. If not that send it to someone who knows how to update it without frying it.
```

---
## \#3 Posted by: SpacedOut Posted at: 2017-07-06T17:04:29.216Z Reads: 161

```
In BLDC Tool's Firmware tab, the firmware version simply says "Old Firmware". I have tried to update it but I always get "Buffer Erase Timeout". I'll try to look for an older version, the only problem is I don't know what version to look for.
```

---
## \#4 Posted by: psychotiller Posted at: 2017-07-06T17:14:01.825Z Reads: 156

```
Yeah, I would send it back then. Get what you paid for.
```

---
## \#5 Posted by: SpacedOut Posted at: 2017-07-06T17:16:47.168Z Reads: 150

```
I'll try contacting them to see what they can do.
```

---
## \#6 Posted by: Jinra Posted at: 2017-07-06T17:22:07.510Z Reads: 149

```
Are you using Ackmaniac's BLDC tool? If so that might be why. You have to use a special F/W with his BLDC tool.
```

---
## \#7 Posted by: SpacedOut Posted at: 2017-07-06T17:26:11.350Z Reads: 144

```
I tried all BLDC Tool versions 2.18, 2.17, 2.16, 2.15, 2.13 in that order and then tried Ackmaniac's. Same problems and now I'm here :(
```

---
## \#8 Posted by: Gorfo99 Posted at: 2018-05-18T00:49:30.802Z Reads: 93

```
im having the same issue here, what did you have to do in order to fix it?
```

---
## \#9 Posted by: daarellano Posted at: 2018-05-30T22:47:35.383Z Reads: 85

```
I am having the same issues have you been able to fix it?
```

---
## \#10 Posted by: RedEagle Posted at: 2018-05-31T00:23:11.242Z Reads: 88

```
This indicates a improperly programmed mcu. 
Next step would be hooking it up to a stlink or discovery board. Then uploading a bootloader. 
After that uploading the firmware with the vesc tool(the new one). 
That's how I did it.
```

---
## \#11 Posted by: RobbyRocket Posted at: 2019-05-17T17:48:53.905Z Reads: 35

```
Hi, I am having this " The firmware on the connected vesc is too old. Please update it using a programmer." However my vesc did not come like this, it happened after I decided to create my own remote, which communicates via SPI. To enable SPI, I have to make a change in conf_general.h, a file included in Vedder's VESC firmware on github. I followed Vedder's online instructions for uploading firmware: http://vedder.se/2015/01/vesc-open-source-esc/
I am on a virtual machine of ubuntu 14.04. when I try make upload, I get the following error message: 

arm-none-eabi-objcopy -O binary build/BLDC_4_ChibiOS.elf build/BLDC_4_ChibiOS.bin --gap-fill 0xFF
openocd -f board/stm32f4discovery.cfg -c "reset_config trst_only combined" -c "program build/BLDC_4_ChibiOS.elf verify reset exit" # For openocd 0.9
Open On-Chip Debugger 0.7.0 (2013-10-22-08:31)
Licensed under GNU GPL v2
For bug reports, read
	http://openocd.sourceforge.net/doc/doxygen/bugs.html
srst_only separate srst_nogate srst_open_drain connect_deassert_srst
trst_only combined trst_push_pull
Info : This adapter doesn't support configurable speed
Error: open failed
in procedure 'transport'
** OpenOCD init Failed **
shutdown command invoked

So, I followed another guy's instructions on how to flash/upload firmware through windows, using the ST-Link Utility program for windows:
https://www.electric-skateboard.builders/t/vesc-boot-loader-installation-tutorial/32103/4

The link he provides for the .hex file is missing, but someone posts its location in the comments below, and now that I have uploaded the .hex file BLDC_AND_MAIN_MERGED, it tells me the firmware is too old, that I should upload it using a programmer. 

I've tried both Ubuntu and stlink utility three times and plugged/ unplugged the VESC and ST-link to power cycle them. This is my first exposure to programming stm32 chips and installing firmware on the vesc.  All I want to do is use the ARM toolchain through ubuntu OR stlink utility to create a hex file for my 4.12 vesc that enables hardware SPI, and upload that firmware, so I can use a remote that uses SPI!  Please help. I know to go into the conf_general.h file and change the hardware SPI line and select the 4.10(but also 4.12 version).  I've uploaded some wiring photos of my STLink, but if wiring was an issue I don't think It would let me program with St-link utility.
![IMG_3741%20(1)|375x500](upload://drgDT437IIFPNCpEQs1sBrNdLUX.jpeg)
```

---
