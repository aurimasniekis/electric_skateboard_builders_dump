# How to Programm/flash a new born VESC 4.12 with st link V2?(Widows 10)

### Replies: 27 Views: 2386

## \#1 Posted by: Mike_Lemon Posted at: 2018-04-19T19:28:10.273Z Reads: 176

```
Hello, 

I've brought back to life a vesc that had a bad MCU with it and replaced it using a hot air and soldering iron.

Now I'd like to get it to operation after verifing the st link V2 can read the data in there.

I'd like to ask what are the steps for making it work and where can you get the hex files for flashing the firmware onto it along with how it should be done using windows 10 and the st link programmer.

Thanks.

I could only find some info about it in the VESC web page but it's just for using ubuntu and the Windows page in unavailable.
```

---
## \#2 Posted by: Mike_Lemon Posted at: 2018-04-19T22:59:35.408Z Reads: 165

```
Also another question,

Does the Bootloader and firmware have to go in two steps or there is an ability to upload them in a single file?
```

---
## \#4 Posted by: Mike_Lemon Posted at: 2018-04-19T23:19:49.742Z Reads: 153

```
Well it has a firmware updater there but sins it's a blank chip I need to flash it with SWD(ST link) and I don't think it supports it.
```

---
## \#5 Posted by: RedEagle Posted at: 2018-04-19T23:29:08.735Z Reads: 148

```
http://www.electric-skateboard.builders/t/vesc-boot-loader-installation-tutorial/32103
```

---
## \#6 Posted by: danielz Posted at: 2018-04-19T23:32:38.828Z Reads: 145

```
yep, the above link, use st utility. I flashed a firmware included in bldc tool, then fired up vesc tool to update to latest.
```

---
## \#7 Posted by: Mike_Lemon Posted at: 2018-04-20T00:11:55.746Z Reads: 141

```
Yeah but when connecting a usb to the VESC(and powering in on with the battery) the computer doesn't recognize it and the ST link with the SWD does read the chip.
```

---
## \#8 Posted by: JLabs Posted at: 2018-04-20T00:14:34.688Z Reads: 133

```
I’m pretty sure your not suppose the have the power on or connected over USB wile flashing
```

---
## \#9 Posted by: Mike_Lemon Posted at: 2018-04-20T00:23:09.633Z Reads: 122

```
But then the PC software would say it is not connected and not recognized.
```

---
## \#10 Posted by: JLabs Posted at: 2018-04-20T00:36:14.764Z Reads: 115

```
Double check your connections and redo the steps. I recently did the on windows 10 as well and it worked perfectly
```

---
## \#11 Posted by: Mike_Lemon Posted at: 2018-04-20T00:39:00.301Z Reads: 109

```
USB connection is fine and I tried it with other vescs.

are you sure this: http://vedder.se/forums/download/file.php?id=6&sid=a6b085428455d0f9a617d880da259517

 is the only file I have to flash with the utility tool to get the device to life?
```

---
## \#12 Posted by: JLabs Posted at: 2018-04-20T00:40:54.502Z Reads: 104

```
I’m not sire but after reading your topic again it seems that you will need more than a boot loader, and that is above my pay grade and left to someone with more in depth knowledge of VESC’s, like @JohnnyMeduse
```

---
## \#13 Posted by: Mike_Lemon Posted at: 2018-04-20T00:44:10.153Z Reads: 98

```
Yeah I also think I just need the actual hex firmware file to upload it with the ST link somehow.
```

---
## \#14 Posted by: danielz Posted at: 2018-04-20T01:49:47.293Z Reads: 97

```
no usb needed the stlink powers it, bootloader did nothing for me, i just wrote the entire firmware to it. Its done the same way. Get the firmware from

C:\Program Files (x86)\BLDC Tool\Drivers\firmwares\hw_410_411_412

Obviously install bldc tool. This is the way i did it last week when my mcu corrupted and usb stopped working.
```

---
## \#15 Posted by: RedEagle Posted at: 2018-04-20T10:03:23.075Z Reads: 92

```
1 Connect st link to the vesc. 
2 Upload the bootloader hex file. 
3 Unplug uart and plug in the USB. 
4 Start up the vesc tool and upload firmware. 

That's how I did it. It should work fine.
```

---
## \#16 Posted by: Mike_Lemon Posted at: 2018-04-20T10:26:28.366Z Reads: 90

```
Done that and it kinda work the BLDC tool detect the device and firmware but now when I try to drive a motor with it after configuring it  the middle red led flashes at 600ms approx intervals.

after doing the same steps on my other VESC it is able to drive a motor properly(using 6S battery for tests) 

Any idea why it does that?
```

---
## \#17 Posted by: Mike_Lemon Posted at: 2018-04-20T10:27:28.173Z Reads: 84

```
The problem is that the bool loader doesn't contain the code to enable the MCU USB peripheral to allow the BLDC tool software to detect it.
```

---
## \#18 Posted by: Mike_Lemon Posted at: 2018-04-20T10:47:47.825Z Reads: 90

```
OK Now when I try to upload the latest firmware with the latest BLDC tool version it sort of lets me do that but ends up not actually working after rebooting no matter how many times I try also tried updating the bootloader but with no luck.
```

---
## \#19 Posted by: Mike_Lemon Posted at: 2018-04-20T11:01:13.325Z Reads: 92

```
OK after diagnosing it with the terminal here are the logs: 

Any ideas?



The following faults were registered since start:

Fault            : FAULT_CODE_DRV
Current          : 0.6
Current filtered : 0.7
Voltage          : 23.57
Duty             : 0.009
RPM              : 0.7
Tacho            : 6
Cycles running   : 0
TIM duty         : 38
TIM val samp     : 1050
TIM current samp : 3150
TIM top          : 4200
Comm step        : 6
Temperature      : -10.36
 
Fault            : FAULT_CODE_DRV
Current          : 0.6
Current filtered : 0.6
Voltage          : 23.57
Duty             : 0.007
RPM              : 0.7
Tacho            : 6
Cycles running   : 0
TIM duty         : 29
TIM val samp     : 1050
TIM current samp : 3150
TIM top          : 4200
Comm step        : 6
Temperature      : -10.33
 
Fault            : FAULT_CODE_DRV
Current          : -8.6
Current filtered : -8.4
Voltage          : 23.57
Duty             : 0.450
RPM              : 0.7
Tacho            : 6
Cycles running   : 0
TIM duty         : 1889
TIM val samp     : 1050
TIM current samp : 3150
TIM top          : 4200
Comm step        : 6
Temperature      : -12.49
 
Fault            : FAULT_CODE_DRV
Current          : -6.9
Current filtered : -6.6
Voltage          : 23.57
Duty             : 0.357
RPM              : 0.7
Tacho            : 6
Cycles running   : 0
TIM duty         : 1500
TIM val samp     : 1050
TIM current samp : 3150
TIM top          : 4200
Comm step        : 6
Temperature      : -12.46
 
Fault            : FAULT_CODE_DRV
Current          : -9.8
Current filtered : -9.9
Voltage          : 23.59
Duty             : 0.440
RPM              : 0.7
Tacho            : 6
Cycles running   : 0
TIM duty         : 1848
TIM val samp     : 1050
TIM current samp : 3150
TIM top          : 4200
Comm step        : 6
Temperature      : -12.46
 
Fault            : FAULT_CODE_DRV
Current          : 0.6
Current filtered : 0.5
Voltage          : 23.57
Duty             : 0.007
RPM              : 0.7
Tacho            : 6
Cycles running   : 0
TIM duty         : 31
TIM val samp     : 1050
TIM current samp : 3150
TIM top          : 4200
Comm step        : 6
Temperature      : -11.71
 
Fault            : FAULT_CODE_DRV
Current          : -13.5
Current filtered : -13.3
Voltage          : 23.57
Duty             : 0.662
RPM              : 0.7
Tacho            : 6
Cycles running   : 0
TIM duty         : 2781
TIM val samp     : 1050
TIM current samp : 3150
TIM top          : 4200
Comm step        : 6
Temperature      : -11.78
 
Fault            : FAULT_CODE_DRV
Current          : -11.8
Current filtered : -11.8
Voltage          : 23.57
Duty             : 0.674
RPM              : 0.6
Tacho            : 6
Cycles running   : 0
TIM duty         : 2830
TIM val samp     : 1050
TIM current samp : 3150
TIM top          : 4200
Comm step        : 6
Temperature      : -11.85
 
Fault            : FAULT_CODE_DRV
Current          : -13.9
Current filtered : -13.8
Voltage          : 23.60
Duty             : 0.734
RPM              : 0.6
Tacho            : 6
Cycles running   : 0
TIM duty         : 3082
TIM val samp     : 1050
TIM current samp : 3150
TIM top          : 4200
Comm step        : 6
Temperature      : -11.47
 
Fault            : FAULT_CODE_DRV
Current          : -13.1
Current filtered : -12.8
Voltage          : 23.57
Duty             : 0.715
RPM              : 0.5
Tacho            : 6
Cycles running   : 0
TIM duty         : 3002
TIM val samp     : 1050
TIM current samp : 3150
TIM top          : 4200
Comm step        : 6
Temperature      : -9.16
 
Fault            : FAULT_CODE_DRV
Current          : -13.8
Current filtered : -13.9
Voltage          : 23.59
Duty             : 0.744
RPM              : 0.4
Tacho            : 6
Cycles running   : 0
TIM duty         : 3125
TIM val samp     : 1050
TIM current samp : 3150
TIM top          : 4200
Comm step        : 6
Temperature      : -12.17
 
Fault            : FAULT_CODE_DRV
Current          : -10.2
Current filtered : -10.0
Voltage          : 23.57
Duty             : 0.606
RPM              : 0.4
Tacho            : 6
Cycles running   : 0
TIM duty         : 2546
TIM val samp     : 1050
TIM current samp : 3150
TIM top          : 4200
Comm step        : 6
Temperature      : -12.21
 
Fault            : FAULT_CODE_DRV
Current          : 1.7
Current filtered : 1.7
Voltage          : 23.57
Duty             : 0.011
RPM              : 0.4
Tacho            : 6
Cycles running   : 0
TIM duty         : 46
TIM val samp     : 1050
TIM current samp : 3150
TIM top          : 4200
Comm step        : 6
Temperature      : -12.28
 
Fault            : FAULT_CODE_DRV
Current          : -14.6
Current filtered : -14.3
Voltage          : 23.56
Duty             : 0.925
RPM              : 0.4
Tacho            : 6
Cycles running   : 0
TIM duty         : 3883
TIM val samp     : 1050
TIM current samp : 3150
TIM top          : 4200
Comm step        : 6
Temperature      : -11.85
 
Fault            : FAULT_CODE_DRV
Current          : -1.6
Current filtered : -1.7
Voltage          : 23.56
Duty             : 0.650
RPM              : 0.3
Tacho            : 6
Cycles running   : 0
TIM duty         : 2730
TIM val samp     : 1050
TIM current samp : 3150
TIM top          : 4200
Comm step        : 6
Temperature      : -11.33
 
Fault            : FAULT_CODE_DRV
Current          : -15.4
Current filtered : -15.2
Voltage          : 23.56
Duty             : 0.950
RPM              : 0.2
Tacho            : 6
Cycles running   : 0
TIM duty         : 3990
TIM val samp     : 1050
TIM current samp : 3150
TIM top          : 4200
Comm step        : 6
Temperature      : -11.33
```

---
## \#20 Posted by: RedEagle Posted at: 2018-04-20T11:08:14.483Z Reads: 73

```
What version of bldc tool are you using? Try using the vesc tool with ackmaniac's firmware.
```

---
## \#21 Posted by: Mike_Lemon Posted at: 2018-04-20T11:10:37.372Z Reads: 78

```
Don't know how to tell but I've tried both versions the old one and the newest 0.91 one but here are the logs does that DRV data makes any sens?
```

---
## \#22 Posted by: RedEagle Posted at: 2018-04-20T11:13:40.038Z Reads: 77

```
It does. You've said earlier that you replaced the MCU. It now seems you also have to replace the DRV and try again. Although the bad DRV shouldn't affect the flashing process, only during detection. I would also check the vesc for shorts.
What lights are you seeing after flashing?
```

---
## \#23 Posted by: Mike_Lemon Posted at: 2018-04-20T11:47:26.643Z Reads: 78

```
Well I see the Vcc 3.3V led always on meaning the DRV step down circuit works along with the 3.3V regulator but now after cleaning the memory and reflash the boot loader and firmware onto it the USB doesn't detect it and the other leds won't blink.


Edit: actually now I got to a point where everything is alright except when I try to turn the motor with the old BLDC tool software the motor wont move but "LED_GREEN" gets brighter when I hit one of the four keys and the "faults" in terminal is empty.
```

---
## \#24 Posted by: danielz Posted at: 2018-04-20T14:13:51.517Z Reads: 76

```
have you checked the fets
```

---
## \#25 Posted by: Mike_Lemon Posted at: 2018-04-20T14:44:17.260Z Reads: 71

```
how do you do that?
```

---
## \#26 Posted by: danielz Posted at: 2018-04-20T21:22:09.507Z Reads: 65

```
if its spinning they are probably ok though. Measure resistance from source to drain. They should be all roughly the same.
```

---
## \#27 Posted by: RedEagle Posted at: 2018-04-20T21:27:24.715Z Reads: 63

```
What happens when you use the bldc tool compatible with the firmware? Does it run with no problems?
```

---
## \#28 Posted by: Mike_Lemon Posted at: 2018-04-20T21:35:19.439Z Reads: 61

```
No it's not running at all just making the led go a bit brighter when pushing the arrow keys but no response also nothing in the faults.
```

---
