# VESC FAQ &#124; Firmware Upgrade Guide - Windows &amp; OSX

### Replies: 6 Views: 6372

## \#1 Posted by: onloop Posted at: 2015-12-31T08:56:23.407Z Reads: 678

```
Lots of people are having problems upgrading the firmware of the VESC. Loading firmware can be confusing, this is mostly due to the incompatibility between the hardware versions, firmware version & BLDC tool versions. 

**WARNING: Loading the incorrect firmware can permanently damage the VESC. If you have doubts about how to upgrade firmware do not proceed. Hardware failures due to bad firmware installation may not be covered under manufacturer's warranty.**

> NOTE: It is important to ensure you use the version of BLDC tool that matches the version of VESC firmware. Upgrading one without the other will likely cause problems.

If you have a newer version of BLDC tool on your computer that is not compatible with your older VESC firmware you may see this warning message instructing you to upgrade your firmware. 
http://www.electric-skateboard.builders/uploads/db1493/original/2X/7/7529f1bc2ba3c1276dbfd3830e474e9d1484ebe0.PNG


Thanks to @trbt555 we now have a simple step-by-step guide. 

 - [Download][1] the latest compatible BLDC & Firmware Version (currently FW2.7 FOC) 
 - Connect VESC to reliable power supply.
 - Connect the VESC to USB and let BLDC tell you the firmware is old (above warning message)
 - Go to firmware tab, select "choose"
 - Navigate to folder, example: "firmwares 2.7 FOC" and then the folder for your hardware version written on your VESC
 - Select "default.bin"
 - Update the firmware


  [1]: https://drive.google.com/folderview?id=0Bym9XrdeViekfkRETmRndENkcVpySW5sWjIzOWdrLThCY01HY3BPOXpqYVRHUlQxS0R5ZlU&usp=drive_web#list
```

---
## \#2 Posted by: DeathCookies Posted at: 2016-03-03T12:27:55.550Z Reads: 536

```
How can I determine which hardwareversion is compatible with what firmwareversion?
```

---
## \#3 Posted by: trbt555 Posted at: 2016-03-04T07:09:43.806Z Reads: 491

```
In the firmwares folder, there are different folders for different hardware versions. Pick the folder that corresponds to your hw version.
```

---
## \#5 Posted by: ralphy Posted at: 2017-01-08T14:05:01.672Z Reads: 294

```
Nice thanks I always saw 3 versions in the folder and default was one of them. I will try it out.
```

---
## \#7 Posted by: ArniJoronen Posted at: 2017-05-29T15:30:33.930Z Reads: 192

```
Where do i get the firmware folder
```

---
## \#8 Posted by: Money Posted at: 2017-07-27T01:20:10.867Z Reads: 143

```
The files that get downloaded contain a read me file with a url to download the latest firmware. But the  urls do not work.
```

---
