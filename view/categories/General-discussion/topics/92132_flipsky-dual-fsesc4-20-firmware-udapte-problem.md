# Flipsky Dual FSESC4.20 firmware udapte problem

### Replies: 7 Views: 432

## \#1 Posted by: guigui Posted at: 2019-04-28T20:36:25.082Z Reads: 94

```
Hey,
I have a problem with my Flipsky Dual FSESC4.20 100A VESC, when I open vesc tool 1.09 and connect my VESC, it says that my vesc firmware is too old and that I need to udapte it, vesc tool 1.09 only support 3.55 firmwares, my vesc is 3.4, so I udapte the firmware in the software, everything seems to work, but after I reboot the VESC it still says 4.3 version and please udapte the firmware, over and over again.
Also I tried to udapte the bootloader, it doesn't fix my problem.

Does anyone now what the problem is ? If you don't, can someone at least send me the older (but "latest") version of the vesc tool firmware that supports 3.4 VESC ? that would be awesome.

Note that I tried to go through the motor configuration process but when It tries to identify/spin the motor, it reminds me that the version is too old.
```

---
## \#2 Posted by: chickengun Posted at: 2019-04-28T21:16:15.837Z Reads: 85

```
You need vesc tool 0.95, the newest firmware there is 3.40. I downloaded it some time ago and I had to use it for my vanda vesc 4.12. Unfortunately I am not home for the next 2 weeks, maybe someone else can provide it.
```

---
## \#3 Posted by: jun1208 Posted at: 2019-04-29T01:45:53.897Z Reads: 74

```
If I rmb correctly, the update should be done on both side of the VESC, have you plug the USB into the other side of the VESC and perform the FW upgrade and see if the problem persist?
```

---
## \#4 Posted by: xsynatic Posted at: 2019-04-29T14:03:38.928Z Reads: 62

```
Same on 3.55 and HW 410 from Torqueboard.

Just updated from 3.54 to 3.55 not both my vescs blink and the Motor detection fails.

Can’t even fnish the Motor setup.
```

---
## \#5 Posted by: sayekim Posted at: 2019-04-30T14:20:52.453Z Reads: 51

```
Get it here:

https://github.com/rpasichnyk/vesc_tool/releases/tag/v0.95-fw3.40

And you can check his other releases too of course. 

Bookmark that page. He’s got them all.
```

---
## \#6 Posted by: guigui Posted at: 2019-05-01T15:44:25.606Z Reads: 39

```
Thank you all for your help, but after 30 tries it finally worked ! :slight_smile: 
 I have no idea why since I did the same procedure over and over. Now I have a belt skipping problem but I think I need to make another thread to talk about that
```

---
## \#7 Posted by: Oibu Posted at: 2019-07-27T20:23:23.173Z Reads: 22

```
Hey, I've the same problem but I can't fix it with VESC Tool 1.11, do you know where I could get 1.09? It would help me a lot... Thanks :grinning:
```

---
