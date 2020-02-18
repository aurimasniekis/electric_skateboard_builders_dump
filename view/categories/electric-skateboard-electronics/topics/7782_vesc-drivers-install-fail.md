# VESC Drivers Install Fail

### Replies: 13 Views: 1469

## \#1 Posted by: racidon Posted at: 2016-08-17T01:58:34.139Z Reads: 117

```
Hi Guys,

I was having some intermittent issues with my board today on my way to work. It would stop working, almost felt like brakes kicking in. Then if I were to hop off and try the remote again it would go to spin the motor and jerk. If I left it for a minute or two it would run again. I would be able to push off and travel again for about 100ms and it would cut out again. I think this is an issue with heat.
So I'm at work and trying to use the BLDC tool. However the drivers don't seem to be installing for some reason. Has anyone had this issue and fixed? Or have suggestions?

I tried rebooting etc and tried installing the drivers using the installer in the BLDC folder and got the following:

<img src="/uploads/db1493/original/2X/4/45da84030c1ffc2c406435732b6a9edc6bc027ce.png" width="513" height="399">

Thanks :)
```

---
## \#2 Posted by: torqueboards Posted at: 2016-08-17T02:00:49.583Z Reads: 107

```
Always use a USB 2.0 port. Don't use a 3.0. Sometimes, you can change the driver. You'll kind of have to play with it until it works as it does depend on the computer your using.
```

---
## \#3 Posted by: racidon Posted at: 2016-08-17T02:16:33.041Z Reads: 104

```
Hi bud, that might actually be the issue. I'll move to another computer later as my work laptop only has usb 3.0 and didn't realise that until now. It amazes me that all 4 ports are 3.0 when so many 2.0 devices aren't compatible with 3.0.
```

---
## \#4 Posted by: torqueboards Posted at: 2016-08-17T02:31:00.842Z Reads: 96

```
Yeah, definitely. I do think all these devices are more legacy type devices though. Most new devices should be fine with 3.0 but yeah.. it is annoying especially on a laptop to have nothing but 3.0.
```

---
## \#5 Posted by: racidon Posted at: 2016-08-17T02:50:42.272Z Reads: 86

```
The other issue is DACs as some can have interference from using USB 3.0
I might even look in the bios if I can force 2.0 mode on one of the ports.
```

---
## \#6 Posted by: t1m0007 Posted at: 2016-08-17T03:32:29.315Z Reads: 79

```
curious- is this USB3 limitation the same on the mac version?
```

---
## \#7 Posted by: racidon Posted at: 2016-08-17T04:08:12.688Z Reads: 71

```
if no one can confirm this I can test this as I have access to a mac too :)
```

---
## \#8 Posted by: paul775 Posted at: 2016-08-17T04:18:39.493Z Reads: 71

```
I programmed my VESC using iMac 2013 if that helps.
```

---
## \#9 Posted by: racidon Posted at: 2016-08-17T04:29:55.988Z Reads: 72

```
but did you use USB3.0 ports?
```

---
## \#10 Posted by: paul775 Posted at: 2016-08-17T04:39:31.847Z Reads: 69

```
Yep. They all are USB 3.0.

<img src="/uploads/db1493/original/2X/7/7caf58f52f354aad4551e720399e68a3500d59b1.png" width="417" height="189">
```

---
## \#11 Posted by: racidon Posted at: 2016-08-17T04:58:14.515Z Reads: 67

```
looks like @t1m0007 got his answer :) thanks bud
```

---
## \#12 Posted by: t1m0007 Posted at: 2016-08-17T16:44:47.523Z Reads: 60

```
thanks all
```

---
## \#13 Posted by: racidon Posted at: 2016-08-18T01:12:12.582Z Reads: 52

```
I still couldn't seem to get this to work. I tried a laptop with USB2.0 but it is also windows 8.1 where as my home PC (which I used last night) is windows 7 and USB 3.0 worked...
I would be willing to bet it's more a chipset limitation rather than anything to do with USB type.
Either way I solved my problem (bad connection on motor to VESC, I was getting ABS_MAX_CURRENT)
```

---
