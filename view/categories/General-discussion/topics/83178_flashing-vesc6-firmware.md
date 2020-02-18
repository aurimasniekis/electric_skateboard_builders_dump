# Flashing VESC6 Firmware

### Replies: 5 Views: 426

## \#1 Posted by: chickengun Posted at: 2019-02-04T22:08:53.747Z Reads: 110

```
I got a ESCape kit from bimmer and soldered all the parts. I got [this](https://www.aliexpress.com/item/1PCS-ST-LINK-Stlink-ST-Link-V2-Mini-STM8-STM32-Simulator-Download-Programmer-Programming-With-Cover/32792513237.html) STLink programmer from aliexpress and connected NRST, SWDIO, GND, SWCLK and VCC in order to flash the vesc 6 firmware. When I plugin the usb dongle I don't hear any connection sound on windows 10. There is no new COM port on device manager. I installed the STlink utility but I can't connect.

Anyone else got the same problem? What could it be? Any help is appreciated.

EDIT: Nevermind. The other VESC worked... but on this one no LED is flashing, I guess a soldering mistake.

Anyways, I am not quite sure. Should I flash the firmware or the bootloader?

https://github.com/vedderb/vesc_tool/blob/master/res/bootloaders/60_o_75_300.bin
or
https://github.com/vedderb/vesc_tool/blob/master/res/firmwares/60/VESC_default.bin
```

---
## \#2 Posted by: linsus Posted at: 2019-02-05T10:14:21.142Z Reads: 80

```
pretty sure you dont need the VCC if the vesc is powered up
```

---
## \#3 Posted by: Pimousse Posted at: 2019-02-06T12:39:29.495Z Reads: 54

```
You don't need the VCC.
Perform a chip erase, flash the FW, then burn the bootloader using VESC Tool.
I had issues burning bootloader using the STlink (weird,  isn't it ?), using VESC Tool was the easier and more reliable way to do so.
```

---
## \#4 Posted by: tecknocreeper Posted at: 2019-05-02T03:40:40.656Z Reads: 34

```
I am having the same issue but i cant get the com to pop up not sure why.
i erased the chip and installed the hex file but i cant find the vesc com 3.
```

---
## \#5 Posted by: chickengun Posted at: 2019-05-02T07:46:11.561Z Reads: 29

```
You soldered the vesc yourself or did you buy it, if so which one?
```

---
