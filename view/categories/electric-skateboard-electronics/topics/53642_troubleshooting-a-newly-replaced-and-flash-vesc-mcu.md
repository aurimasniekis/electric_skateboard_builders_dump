# Troubleshooting a newly replaced and flash VESC MCU

### Replies: 3 Views: 427

## \#1 Posted by: Mike_Lemon Posted at: 2018-04-27T11:36:02.375Z Reads: 63

```
Hello,

I've got a vesc I recently fixed by replacing the MCU and DRV chip and flashing the MCU with a bootloader and the 2.18V firmware not when I connect it to the PC it reacts aight and can read the device firmware but when trying to do the motor test and move it at all it doesn't move the motor but shows the red led getting brighter when pushing the arrow keys.

Also have to mention that nothing on the board gets warm or hot(Except the MCU a very little but I assume it's ok sins it's a high speed arm processor)

Nothing in the faults although sometimes it gives me this error when the motor is connected but not consistent: 



The following faults were registered since start:

Fault            : FAULT_CODE_DRV8302
Current          : 0.2
Current filtered : 0.3
Voltage          : 23.30
Duty             : 0.95
RPM              : 4.6
Tacho            : 4
Cycles running   : 0
TIM duty         : 3990
TIM val samp     : 1050
TIM current samp : 3150
TIM top          : 4200
Comm step        : 5
Temperature      : 21.98

Any idea what is going on?

Thanks for helping.
```

---
## \#2 Posted by: chocol4te Posted at: 2018-04-27T11:40:37.885Z Reads: 50

```
Did you use a reflow oven for replacing the chips? If so I’d recommend rechecking all pins have enough solder, that nothing else got dislocated or bumped, then applying a generous amount of flux and rebaking.

 Can you post the output of st-util info and when you flash the boot loader. Then read back the on chip firmware and compare checksums.
```

---
## \#3 Posted by: Mike_Lemon Posted at: 2018-04-27T11:50:02.590Z Reads: 49

```
Well, 

I did not reflow it just used the hot air to desolder the chips


That's the programming settings:

![image|686x500](upload://gLFiNIqxaSXkwajd3b6jPTGgwuN.png)


and here are the logs afterwards:

14:47:04 : ST-LINK SN : 55FF78065088485238332287
14:47:04 : ST-LINK Firmware version : V2J29S7
14:47:04 : Connected via SWD.
14:47:04 : SWD Frequency = 4,0 MHz.
14:47:04 : Connection mode : Normal.
14:47:04 : Debug in Low Power mode enabled.
14:47:04 : Device ID:0x413 
14:47:04 : Device flash Size : 1MBytes
14:47:04 : Device family :STM32F405xx/F407xx/F415xx/F417xx
14:47:12 : [BLDC_4_Bootloader.hex] opened successfully.
                  Address Ranges [0x080E0000 0x080E01AC] [0x080E01B0 0x080E10A0] 
14:47:12 : [BLDC_4_Bootloader.hex] checksum : 0x00055E07 
14:48:14 : Memory programmed in 4s and 547ms.
14:48:14 : Verification...OK
14:48:14 : Programmed memory Checksum: 0x00055E07
```

---
