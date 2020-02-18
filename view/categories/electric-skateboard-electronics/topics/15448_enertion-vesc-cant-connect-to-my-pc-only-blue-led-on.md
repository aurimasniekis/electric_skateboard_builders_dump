# Enertion Vesc can&rsquo;t connect to my pc.(Only blue led on)

### Replies: 24 Views: 1917

## \#1 Posted by: laikiux Posted at: 2016-12-31T14:22:11.406Z Reads: 117

```
Hello,
I have ordered Enertion 4.12 Vesc from the last batch. Now I'm trying to set up it, and run motor detection.
Firstly, I connented vesc over the usb port and then powered it with 12V PSU.  But only blue led is on. I have tried different usb cables even swopped pc's, but the same problem occurs. Maybe you have suggestion?
```

---
## \#2 Posted by: uncosk8r Posted at: 2016-12-31T15:40:43.320Z Reads: 112

```
Have you checked for errors with the drivers?

I had a similar situation, which was resolved by installing a driver I got from an arduino site.
You can tell if that's the problem by looking in the device manager.(What O.S. is your pc? The following is only relevant if you're using windows)
I can't remember clearly, but i think it was "tiny" or something similar.

I'll try and find the link tomorrow if someone else doesn't beat me to it.
```

---
## \#3 Posted by: laikiux Posted at: 2016-12-31T15:43:35.460Z Reads: 110

```
I'm running windows 8
```

---
## \#4 Posted by: zmoney Posted at: 2016-12-31T16:58:19.072Z Reads: 98

```
You might be missing firmware and/ or boot loader on the vesc. You have to get an STLINK v2 to flash the firmware
```

---
## \#5 Posted by: laikiux Posted at: 2016-12-31T17:00:56.108Z Reads: 95

```
But all of the enertion vesc's has a firmware and are tested before shipping. I'm right @onloop ???
```

---
## \#6 Posted by: zmoney Posted at: 2016-12-31T17:06:27.448Z Reads: 91

```
There's been instances were enertion vescs have shipped without them. You should try contacting their support. If anything it might easier to do it yourself, you can find them on eBay for less than 10 USD.
```

---
## \#7 Posted by: laikiux Posted at: 2016-12-31T17:25:49.529Z Reads: 91

```
but then I need linux or ubuntu... It seems so confusing...
```

---
## \#8 Posted by: JohnnyMeduse Posted at: 2016-12-31T17:31:45.038Z Reads: 91

```
before going to the conclusion that the vesc doesn't have any firmware... 

can you post some picture of it and maybe a video of the booting sequence (to see what the led does when you power up the vesc)

exemple of video:
https://www.youtube.com/watch?v=reMemaOKAnA

Also have you try to contact enertion support ?
```

---
## \#9 Posted by: laikiux Posted at: 2016-12-31T17:46:38.791Z Reads: 87

```
1. I connect vesc over the USB port. (the usb cable is capable to send data)
2. I connected vesc with 12V psu
3. Blue led appears and nothing else happens
4. Open BLDC tool and there is only com1 port...
Maybe I need some kind of drivers?
Yes, I contacted support, but I guess they will say: "go to esk8 builders forum"
```

---
## \#10 Posted by: JohnnyMeduse Posted at: 2016-12-31T17:49:58.765Z Reads: 88

```
Please contact enertion support... if this is a firmware issue they will guide you through the process, you also don't need linux
```

---
## \#11 Posted by: laikiux Posted at: 2016-12-31T17:58:33.310Z Reads: 87

```
can I follow this video? https://www.youtube.com/watch?v=H4sbDhRcaOQ
Can you post a link where I can buy proper STLINK v2?
```

---
## \#12 Posted by: laikiux Posted at: 2016-12-31T20:36:25.143Z Reads: 81

```
The same problem:
https://www.youtube.com/watch?v=nenIvSAVTyA
```

---
## \#13 Posted by: lowGuido Posted at: 2016-12-31T20:58:40.346Z Reads: 79

```
Have you setup the com port correctly?
```

---
## \#14 Posted by: laikiux Posted at: 2016-12-31T20:59:14.342Z Reads: 79

```
How to do that?
```

---
## \#15 Posted by: mmaner Posted at: 2016-12-31T21:48:21.263Z Reads: 80

```
I had the same problem with MEB and DIY VESCs, turned out to be the battery pack.
```

---
## \#16 Posted by: Devo Posted at: 2017-01-01T00:17:31.569Z Reads: 78

```
That video of the VESC won't connect is mine. Enertion support asked for video evidence when I had the same problem as you. After them reviewing the video they agreed that there was no booted loader. I told them I didn't have kwoledge or equipement to flash it myself and they agreed to compensate by replacing it with a VESC x. I'm still waiting for shipment 3 months on I believe.
```

---
## \#17 Posted by: JLabs Posted at: 2017-01-01T03:55:58.514Z Reads: 68

```
[quote="laikiux, post:3, topic:15448, full:true"]
I'm running windows 8
[/quote]

There is your first problem, lol

Sorry that I can't be of any help.
```

---
## \#18 Posted by: uncosk8r Posted at: 2017-01-01T06:27:36.975Z Reads: 68

```
Try installing the stm32 driver mentioned in

 http://www.electric-skateboard.builders/t/vesc-faq-windows-version-of-bldc-tool/141/34?u=uncosk8r

First check in the device manager though to make sure that the lack of driver is your problem, if so, you'll see the usual black "!" on a yellow dot; For some reason it doesn't seem to install correctly on windows 8.
```

---
## \#19 Posted by: laikiux Posted at: 2017-01-01T09:59:09.732Z Reads: 66

```
Hello, but I have already tried ir with windows 7, but the same problem occurs. I think the Vesc actually doesn't have any bootloader/firmware... 
Yes, I tried this driver, but it doesn't work as well.
```

---
## \#20 Posted by: Maxid Posted at: 2017-01-01T10:03:54.411Z Reads: 65

```
I had to use three different usb cables until my computer saw the VESC and installed the drivers (virtual com port) on its own. There are mini usb cables out there that are only used for charging stuff. In the end I used one that came with an Arduino - that way I was sure that data transfer is indeed possible.
```

---
## \#21 Posted by: okp Posted at: 2017-01-01T10:08:32.584Z Reads: 60

```
hey, I had my hand on a VESC that was connecting perfecly with STLINKv2; programming perfectly too; uploading bootloader/firmware but impossible to connect via BLDC on a working environment. The VESC was lighting blue and that's it. It was a maytech one.
```

---
## \#22 Posted by: laikiux Posted at: 2017-01-01T10:12:29.643Z Reads: 58

```
My usb cable is capable to transfer data. I use it to program my arduino nano.
```

---
## \#23 Posted by: laikiux Posted at: 2017-01-01T12:44:53.004Z Reads: 55

```
Maybe there is a problem because I power my Vesc with 12v? Should I use my 10s battery?
```

---
## \#24 Posted by: laikiux Posted at: 2017-01-01T14:26:14.980Z Reads: 51

```
Powered it with the battery, but still nothing happens. @EnertionSupport?
```

---
