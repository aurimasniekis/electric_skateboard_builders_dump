# VESC firmware update through bluetooth

### Replies: 8 Views: 995

## \#1 Posted by: RiGo Posted at: 2017-08-20T04:59:28.972Z Reads: 138

```
Is this possible? I mean connecting the BLDC tool to the VESC via a BT module plugged into the UART port and updating the firmware.  Or can it only be done by connecting through the USB port on the VESC.
```

---
## \#2 Posted by: MontPierre Posted at: 2017-08-20T05:20:03.326Z Reads: 136

```
I'm not sure if you can but here is great app and Bluetooth module to adjust settings on the fly 

http://www.electric-skateboard.builders/t/configuration-and-telemetry-for-vesc-ios-android/13483?u=montpierre
```

---
## \#3 Posted by: RiGo Posted at: 2017-08-20T05:33:07.046Z Reads: 129

```
Thanks, but that doesn't help with my question... ¯\\\_(ツ)_/¯
```

---
## \#4 Posted by: RiGo Posted at: 2017-08-20T21:09:06.429Z Reads: 98

```
Still hoping to get an answer for this... Bump
```

---
## \#5 Posted by: Ackmaniac Posted at: 2017-08-20T21:40:54.582Z Reads: 89

```
Bluetooth isn't ideal for this. Because it is quite common that some packets get lost. And there is a difference between normal Bluetooth and Bluetooth Low Energy (BLE). 
BLE has a max of 20 bytes in each packet but on the other side it only uses roughly 15 ma of current.
And to upload the firmware you need like 200000 bytes. That will be 10000 single packets (200000 / 20). If a single packet is lost the firmware is corrupt. So in theory it would be possible to do that but the software needs to be improved to identify missing packets which need to be resend.  Via USB the connection is very stable.
```

---
## \#6 Posted by: RiGo Posted at: 2017-08-21T00:18:40.432Z Reads: 71

```
Thanks Nico. One more questions (hopefully the last one).

I'm pretty sure that you can flash firmware using an ST-Link unit. However, can this be done through the BLDC tool? In other words, is the BLDC tool able to communicate with the VESC using ST-Link in the same way that it does through the VESC's USB port?

Thanks!!!
```

---
## \#7 Posted by: Ackmaniac Posted at: 2017-08-21T00:21:16.418Z Reads: 72

```
benjamin Vedder offers this feature for the new VESC-Tool. I never invested a thought about it but it is for sure a nice feature. Only thing i know is that when you killed the firmware of your VESC badly then your computer can't even detect the VESC when you connect it via USB. In this case you his bootloader option also wouldn't work,
```

---
## \#8 Posted by: RiGo Posted at: 2017-08-21T00:43:22.581Z Reads: 70

```
The firmware is ok. Just wondering if it can be updated using ST-Link through the BLDC tool.
```

---
