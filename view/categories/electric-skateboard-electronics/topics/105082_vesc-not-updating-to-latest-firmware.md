# VESC not updating to latest firmware

### Replies: 3 Views: 95

## \#1 Posted by: Froger Posted at: 2020-01-05T21:18:02.916Z Reads: 31

```
Hi !

Long story short: I have old Koowheel hubs and am currently trying to set them up with Flipsky dual FSESC 420. It looks like 2 VESC glued up. When connected to master ( first ) VESC via USB I got a popup wanting to upgrade the firmware. It went smoothly. Unfortunately second VESC wasn"t so cooperative. I can send new firmware to the board, but it newer gets updated. After some search it looks like this VESC ( Flipsky ) does not support bootloader. That is especially weird considering the first one did get updated. Right now I got slave ESC stuck at firmware 3.4 and master is at 3.65. As it is I can't use dual motors because the tool prevents me from doing so ( limited mode ).

Is it possible to update the slave to 3.65 without STLINK ? Or maybe it is a better idea to downgrade master VESC to 3.4 ? I read somewhere that VESC-tools comes with firmwares preinstalled so legacy version could in theory solve my problem. 

Thanks for help in advance !
```

---
## \#2 Posted by: BillGordon Posted at: 2020-01-06T00:59:36.567Z Reads: 26

```
Try both using Ackmaniac. Hit me up on the other forum and I can hook you up with a great tutorial (with download link) on Ack done by @mmaner
```

---
## \#3 Posted by: trampa Posted at: 2020-01-06T07:31:34.471Z Reads: 19

```
Simply ad the bootloader, using the bootloader tab. The Bootloader tab is in the Firmware menu, top of the window. If that does nor work, you need to flash the ESC via SWD Prog. You can use the working side to flash the non working side.

Minute 5 onwards:

https://www.youtube.com/watch?v=PFFiVxFHDM4
```

---
