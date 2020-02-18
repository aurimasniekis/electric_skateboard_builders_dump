# Weird Focbox problem? Video included

### Replies: 17 Views: 474

## \#1 Posted by: TrainRider Posted at: 2018-10-13T12:33:07.732Z Reads: 103

```
Hello!

I was hoping someone on the forums might be able to help me with a problem I am experiencing with one of my focbox's.

Originally the problem I had was a drv fault, I got that repaired locally and ever since then when plugged in the focbox does the below, it is also not being recognized via usb:

https://youtu.be/V1GWEq3_0jc

I contacted Enertion support who suggested that the problem was with caused by the FOCBOX missing the bootloader, so I've followed [this tutorial](https://www.electric-skateboard.builders/t/vesc-boot-loader-installation-tutorial/32103) combined with information [in this thread](https://www.electric-skateboard.builders/t/bricked-focbox-and-st-link/45864) about the port differences which seemed to all work well. The last information from the ST-Link Utility was:

> 13:41:02 : [BLDC_4_Bootloader.hex] opened successfully.
                  Address Ranges [0x080E0000 0x080E01AC] [0x080E01B0 0x080E10A0] 
13:41:02 : [BLDC_4_Bootloader.hex] checksum : 0x00055E07 
13:41:46 : Memory programmed in 3s and 438ms.
13:41:46 : Verification...OK
13:41:46 : Programmed memory Checksum: 0x00055E07
13:42:30 : Disconnected from device.

But this hasn't changed the behavior, when powered I still get the weird light pattern and it is not recognized via USB.

It's worth noting that all 3 status LED's are lighting up when connected via ST-LINK so they are working fine.

Does anyone have any idea what's going wrong with the FOCBOX and how I might be able to fix it?

Thanks in advance,
Liam
```

---
## \#2 Posted by: Jc06505n Posted at: 2018-10-13T13:50:18.379Z Reads: 82

```
You wouldn’t have happened to upgrade the firmware via tcp at anytime have you ?
```

---
## \#3 Posted by: TrainRider Posted at: 2018-10-13T14:07:30.883Z Reads: 78

```
I have tinkered with some settings with the ackmaniac phone app via bluetooth, but haven't changed the firmware.
```

---
## \#4 Posted by: taz Posted at: 2018-10-13T15:43:56.075Z Reads: 74

```
After uploading the bootloader, did you also upload the firmware.bin file via the st-link?
If not, you have to before proceeding.
```

---
## \#5 Posted by: TrainRider Posted at: 2018-10-16T17:57:38.908Z Reads: 62

```
Thanks for the suggestion, I'm struggling to find a .bin for the firmware. Could you point me in the right direction?
```

---
## \#6 Posted by: taz Posted at: 2018-10-16T18:04:16.011Z Reads: 61

```
https://github.com/vedderb/vesc_tool/blob/master/res/firmwares/410_o_411_o_412/VESC_default.bin
```

---
## \#7 Posted by: TrainRider Posted at: 2018-10-16T18:09:07.676Z Reads: 58

```
Thank you! Unfortunately I get the same result..
```

---
## \#8 Posted by: taz Posted at: 2018-10-16T18:14:36.368Z Reads: 59

```
Did you connect the pins like shown [here](https://www.electric-skateboard.builders/t/did-i-just-brick-my-focbox-heeelllppppp/70433/69?u=taz)?
```

---
## \#9 Posted by: TrainRider Posted at: 2018-10-16T18:22:39.617Z Reads: 60

```
I used this wiring diagram https://www.electric-skateboard.builders/uploads/db1493/original/3X/1/7/175d1af2861de11333348dc0f0af767df4af07e8.png
```

---
## \#10 Posted by: taz Posted at: 2018-10-16T18:24:41.766Z Reads: 60

```
You only need 3 pins (DIO - GND - CLK) as long as you power the vesc with your battery
```

---
## \#11 Posted by: TrainRider Posted at: 2018-10-16T18:27:01.504Z Reads: 59

```
I wasn't powering with my battery, only via st-link would that make a difference?
```

---
## \#12 Posted by: taz Posted at: 2018-10-16T18:43:33.538Z Reads: 54

```
No idea.
I read [here](https://vesc-project.com/comment/208#comment-208) it can blow up the 3.3V regulator on the VESC6 so decided not to risk it even in 4.12HW
```

---
## \#13 Posted by: CarlCollins Posted at: 2018-10-16T21:19:13.798Z Reads: 51

```
@TrainRider
Have you tried plugging it to the battery and then use ST-Link to flash firmware?
```

---
## \#14 Posted by: TrainRider Posted at: 2018-10-18T21:22:50.736Z Reads: 49

```
Just tried this, it doesn't appear to be getting power and isn't being recognized by USB. Seeing as it was working when being powered by the ST link I assume this means I have a problem with the 3.3V power on the FOCBOX?
```

---
## \#15 Posted by: CarlCollins Posted at: 2018-10-19T22:28:07.866Z Reads: 38

```
@TrainRider
Double confirm your drivers and USB cable, also check if your FOCBOX's MCU chip survived
```

---
## \#16 Posted by: TrainRider Posted at: 2018-10-20T12:30:54.959Z Reads: 31

```
How do I check the MCU survived?
```

---
## \#17 Posted by: CarlCollins Posted at: 2018-10-21T05:49:18.778Z Reads: 26

```
@TrainRider
Use multimeter to do that
```

---
