# Calling coding and computer experts

### Replies: 32 Views: 336

## \#1 Posted by: dg798 Posted at: 2018-07-03T19:03:06.233Z Reads: 126

```
I have a chromebook in dev mode and have installed the full vesc-tool apk and it works fine. The problem is that the chromebook can’t communicate with the vesc via the USB port. Any ideas to fix this problem? I have heard about certain apis you could use but I’m not so sure how to implement them. I think it would be amazing to be able to use the vesc-tool on a chromebook.
```

---
## \#2 Posted by: b264 Posted at: 2018-07-03T20:04:33.329Z Reads: 111

```
Can you boot it from a flash drive and just boot a different linux distro?
```

---
## \#3 Posted by: mikenyc Posted at: 2018-07-03T20:06:40.352Z Reads: 105

```
I think chromebooks run Ubuntu under the hood
```

---
## \#4 Posted by: Kug3lis Posted at: 2018-07-03T20:11:04.201Z Reads: 94

```
No it runs plain Linux Kernel, I think Chome OS limits direct access to USB/hardware or etc :)
```

---
## \#5 Posted by: b264 Posted at: 2018-07-03T20:11:12.838Z Reads: 83

```
I think they run ChromeOS.  If you can boot Ubuntu from a flash drive, you'd be all set.
```

---
## \#6 Posted by: dg798 Posted at: 2018-07-03T20:11:20.343Z Reads: 76

```
I’m in dev mode
```

---
## \#7 Posted by: dg798 Posted at: 2018-07-03T20:11:49.565Z Reads: 75

```
I have crouton installed so I can dual boot Linux and chrome os but USB ports don’t work inside the Linux environment
```

---
## \#8 Posted by: b264 Posted at: 2018-07-03T20:12:37.348Z Reads: 69

```
Can you boot from a flash drive?
```

---
## \#9 Posted by: dg798 Posted at: 2018-07-03T20:12:48.653Z Reads: 68

```
I downloaded the vesc tool apk and it works but i need some sort of api to allow it to recognize the vesc but I don’t know how to install the api
```

---
## \#10 Posted by: dg798 Posted at: 2018-07-03T20:13:08.492Z Reads: 64

```
I already have Ubuntu running alongside chrome os
```

---
## \#11 Posted by: Kug3lis Posted at: 2018-07-03T20:13:38.781Z Reads: 55

```
chroot doesnt mean it will add functionality like hardware access layer if its not present in base os
```

---
## \#12 Posted by: dg798 Posted at: 2018-07-03T20:14:36.194Z Reads: 55

```
I know that’s why I downloaded the vesc tool directly into the chrome os and it works but I need some sort of api to recognize the usb
```

---
## \#13 Posted by: b264 Posted at: 2018-07-03T20:15:23.142Z Reads: 51

```
[quote="dg798, post:10, topic:60823, full:true"]
I already have Ubuntu running alongside chrome os
[/quote]

I don't know what "alongside" means.  Just boot Ubuntu directly.
```

---
## \#14 Posted by: Kug3lis Posted at: 2018-07-03T20:16:00.088Z Reads: 50

```
:man_facepalming: ChromeOS doesn't support USB serial ports, either you need to find a way to install it or its just not available or it is available just not the way vesc tool supports
```

---
## \#15 Posted by: dg798 Posted at: 2018-07-03T20:16:13.201Z Reads: 49

```
It means I can either be in Ubuntu or chrome os
```

---
## \#16 Posted by: dg798 Posted at: 2018-07-03T20:16:53.493Z Reads: 47

```
Correct but I looked at some developer options and one of them was installing a serial usb api but I’m not sure how to do that
```

---
## \#17 Posted by: b264 Posted at: 2018-07-03T20:17:21.992Z Reads: 48

```
Run Ubuntu.  Not ChromeOS.  Follow the instructions in Vedder's repo.  Ask if you have any questions.
```

---
## \#18 Posted by: dg798 Posted at: 2018-07-03T20:17:48.770Z Reads: 48

```
Meaning just have Ubuntu on chromebook? Not both
```

---
## \#19 Posted by: b264 Posted at: 2018-07-03T20:18:20.497Z Reads: 46

```
It doesn't matter what's on the chromebook.  It only matters what you are running.
```

---
## \#20 Posted by: Kug3lis Posted at: 2018-07-03T20:18:40.235Z Reads: 47

```
Easiest way ask a friend for a normal windows computer and just install vesc tool
```

---
## \#21 Posted by: dg798 Posted at: 2018-07-03T20:19:45.298Z Reads: 43

```
Got it.
I know there’s a way in dev mode to enable usb serial ports I’m just not sure exactly how it works
```

---
## \#22 Posted by: Kug3lis Posted at: 2018-07-03T20:20:42.792Z Reads: 44

```
Yes, there is but it doesn't mean that it will be the way VESC Tools needs it to be, Chrome OS apps supports usb/serial port through its API not through dev sockets like vesc tool expects it :)
```

---
## \#23 Posted by: dg798 Posted at: 2018-07-03T20:22:12.485Z Reads: 44

```
Ok I would like to try the api way I’m just not sure how to install an api. I searched all over and I still don’t know how to. Would you be able to get me started with just how to install the api?
```

---
## \#24 Posted by: Kug3lis Posted at: 2018-07-03T20:23:46.224Z Reads: 41

```
You dont need to install anything it's inside chrome native api, but it will not work with vesc tool because its not compatible...

https://developer.chrome.com/apps/app_serial
```

---
## \#25 Posted by: dg798 Posted at: 2018-07-03T20:25:06.323Z Reads: 39

```
Ohh ok. So I’m pretty much stuck?
```

---
## \#26 Posted by: b264 Posted at: 2018-07-03T20:27:06.533Z Reads: 38

```
I suggested multiple times how to do this.
```

---
## \#27 Posted by: dg798 Posted at: 2018-07-03T20:28:39.388Z Reads: 37

```
No I understand your way I just like chrome os a lot.
I meant I can’t use the serial port api!
```

---
## \#28 Posted by: dg798 Posted at: 2018-07-03T20:29:32.798Z Reads: 38

```
How do I run the api. How do I create the manifest.json file and incorporate into chrome os
```

---
## \#29 Posted by: Kug3lis Posted at: 2018-07-03T20:30:14.833Z Reads: 39

```
Man, you can't just take a something and try to make it work... It's just not how it works...

https://gluestickmum.files.wordpress.com/2015/03/img_3995.png?w=640
```

---
## \#30 Posted by: dg798 Posted at: 2018-07-03T20:32:50.794Z Reads: 39

```
I hear that. I was just curious to see if it maybe just maybe can work but if you really don’t think so then I won’t try.
```

---
## \#31 Posted by: mikenyc Posted at: 2018-07-04T00:38:06.970Z Reads: 29

```
[quote="dg798, post:27, topic:60823"]
I just like chrome os a lot.
[/quote]

Why? Lol

10char
```

---
## \#32 Posted by: dg798 Posted at: 2018-07-04T00:45:23.896Z Reads: 30

```
I’m a student in school and it suits my needs very well for the time being.
```

---
