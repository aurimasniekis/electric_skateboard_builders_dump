# Which file to flash on VESC6?

### Replies: 2 Views: 101

## \#1 Posted by: chickengun Posted at: 2019-02-05T19:20:13.360Z Reads: 38

```
I soldered together the ESCape kit (VESC6 HW64). I got all the parts from bimmer. I can also connect to the VESC using a STLink programmer. Now I am asking myself which file to flash? To my understanding I need to flash the bootloader because my goal is to connect to the VESC using the 'VESC Tool', is this correct? Below are two links I found, the first one seems to be the bootloader and the other one the firmware. Which one of these should I flash so that I can connect over USB using the VESC Tool? Thanks!

https://github.com/vedderb/vesc_tool/blob/master/res/bootloaders/60_o_75_300.bin
or
https://github.com/vedderb/vesc_tool/blob/master/res/firmwares/60/VESC_default.bin
```

---
## \#2 Posted by: FullMetal_Machinist Posted at: 2019-02-05T19:47:33.207Z Reads: 27

```
If you flash bootloader (first file) you will have to upload firmware after.
If you flash firmware (second file) you can connect to VESC Tool immediately, providing that soldering of components on pcb is ok.
So flash second file. Remember to tick "verify file after flashing".
```

---
