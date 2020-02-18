# Cant connect to FOXBOX 2.54 :(

### Replies: 13 Views: 1134

## \#1 Posted by: driver Posted at: 2017-10-07T17:09:44.342Z Reads: 109

```
Hey guys,

i ve tried to connect the vesc (FOCBOX 2.54) to the pc (win 10) but it does not recognize the usb device.

i red that windows should connect via COM 1,2,3.... but i just have COM1 and i get the error "no firmware read response".

i ve tried the Virtual COM Port driver from STMicroelectronics  but it dows not work.
the device manager says "unknown usb device (error at getting discription)

can anybody please help me?
```

---
## \#2 Posted by: Michael319 Posted at: 2017-10-07T17:19:49.761Z Reads: 105

```
What BLDC tool are you using. Where did you download it from?
```

---
## \#3 Posted by: Michael319 Posted at: 2017-10-07T17:30:52.004Z Reads: 101

```
Also, 2.54 is what @Ackmaniac uses for his firmware. It sounds like you downloaded the wrong BLDC tool
```

---
## \#4 Posted by: deucesdown Posted at: 2017-10-07T20:14:27.911Z Reads: 86

```
I got a recent focbox, it was 2.18 out of the box.

But, the firmware version wouldn't/shouldn't affect what COM port it shows up as in windows. If I were you I'd try a different microusb cable, and maybe try with the focbox cover off, as the port seems quite recessed. fwiw my microusb cable connected fine without removing the cover.
```

---
## \#5 Posted by: driver Posted at: 2017-10-08T08:45:19.637Z Reads: 70

```
I ve downloaded it with a Link from the Forum here.
Where do I get the latest version?
```

---
## \#6 Posted by: driver Posted at: 2017-10-08T08:51:56.633Z Reads: 70

```
I don't know what wrong with my windows... I had to delete all USB hubs in the device manager. So I can't even click reboot because keyboard and mouse where dead... Anyways.. It works.. COM3 shows up.

Now I just need the right version
```

---
## \#7 Posted by: deucesdown Posted at: 2017-10-08T15:11:34.575Z Reads: 67

```
Try this

http://www.enertionboards.com/new-focbox-speed-controller/focbox-bldc-tool-win/
```

---
## \#8 Posted by: MrHappy Posted at: 2017-10-08T16:18:16.407Z Reads: 62

```
Another issue ive run into before is that i was missing arduino nano drivers. once they were installed I could read it just fine.
```

---
## \#9 Posted by: driver Posted at: 2017-10-09T20:44:02.309Z Reads: 56

```
found this one:
[https://www.dropbox.com/sh/t7dl90owz5ccbyl/AADNOs3g9TfYw-VAyYey3hZNa/BLDC-TOOl and Firmware?dl=0](http://)

This worked.
```

---
## \#10 Posted by: Michael319 Posted at: 2017-10-09T20:47:45.813Z Reads: 53

```
Did you install 2.54 firmware as well. I just want you to realize what you just did. It looks like you installed @Ackmaniac's bldc tool, which is not necessarily recommended unless you know what you're doing. It has more advanced features than what you need.
```

---
## \#11 Posted by: driver Posted at: 2017-10-09T21:14:44.495Z Reads: 49

```
The firmware was on the vecs before i got it.
```

---
## \#12 Posted by: deucesdown Posted at: 2017-10-09T21:44:25.981Z Reads: 48

```
just in case you didn't know, there's a buggy version of 2.18 firmware/bldctool that has what's called the "current ramp step bug". Really sad that the fix didn't bump the version number.

https://www.electric-skateboard.builders/search?q=current%20ramp%20step%20bug

Try doing a write followed by a read, and check the current ramp step field and make sure it hasn't increased 10x. I can't remember if it's the firmware or bldc-tool, but I believe the 10x happens on read config, not write config.

If you get around to checking this plz add a note to your post with the dropbox link for others.
```

---
## \#13 Posted by: cwazy1 Posted at: 2017-10-09T23:26:53.238Z Reads: 45

```
I had this issue, turned out to be that my micro USB was not reaching all the way into the port on the focbox due to the thick ass enclosure around the port.
```

---
