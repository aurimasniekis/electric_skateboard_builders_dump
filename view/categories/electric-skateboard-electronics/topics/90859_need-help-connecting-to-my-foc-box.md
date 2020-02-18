# Need help connecting to my foc box

### Replies: 27 Views: 240

## \#1 Posted by: 2Fat2Fly Posted at: 2019-04-17T11:47:16.303Z Reads: 62

```
I have been a lurker for a Long time, and made a board i had up and running. Then I began to upgrade and bought some foc boxes for a dual set-up.

A few month ago I connected to them and uploaded ackmaniac's firmware. Now I have gotten all the last peices for my project. And the weather has finally become ridable.

The problem is now I can't get a connection to do a setup. 
I've tried everything I can think of, and all I can find on this great forum.

I have posted some pictures that might help troubleshooting.

English is not my first language, sorry for any misspellings.

![IMG_20190417_133835|229x500](upload://At9xlavyuOwmzNYz14RrDVd0WLs.jpeg) ![IMG_20190417_133755|690x316](upload://7fX5SNkLDc8ZL8n1K0Hjs5f5ERU.jpeg) ![IMG_20190417_133849|229x500](upload://pQ9mUmhGQM4vkkV7lXXhP8ohO3U.jpeg) ![IMG_20190417_133637|229x500](upload://fsLXUMb2FDn0BbIQBzIDQcbqVRN.jpeg) ![IMG_20190417_133629|690x316](upload://dUEwv3GaKHarUpDR37NAEOVDKTi.jpeg) ![IMG_20190417_133658|229x500](upload://eKDAMrUXwAyfVdeBxdjsSL5s4rC.jpeg)
```

---
## \#2 Posted by: 2Fat2Fly Posted at: 2019-04-17T15:52:45.993Z Reads: 44

```
Please help. Bump
```

---
## \#3 Posted by: Jinra Posted at: 2019-04-17T15:57:12.589Z Reads: 41

```
Are you sure it's connected to the cable? The focbox micro usb header is a bit recessed and requires a longer connector to reach, or alternatively you can take off the housing to  connect with any cable.
```

---
## \#4 Posted by: 2Fat2Fly Posted at: 2019-04-17T15:59:30.621Z Reads: 41

```
Yes I have taken the enclosure off for that specific reason.
```

---
## \#5 Posted by: Blasto Posted at: 2019-04-17T16:01:29.235Z Reads: 41

```
probably worth checking if you have an unknown device in your device manager, you've managed to change the fw, so the usb was in working order.

make sure you are using a usb cable that can transfer data, not those crappy charge only cables
```

---
## \#6 Posted by: Jinra Posted at: 2019-04-17T16:04:34.238Z Reads: 38

```
Okay, it's just that the picture you have on there still has the enclosure on.
```

---
## \#7 Posted by: 2Fat2Fly Posted at: 2019-04-17T16:39:40.058Z Reads: 34

```
The picture was after I gave up and put it all back together 😀 

Might be a stupid question but how do I check if I have an unknown device ?
```

---
## \#8 Posted by: 2Fat2Fly Posted at: 2019-04-18T08:30:51.222Z Reads: 27

```
Back at it again....![IMG_20190418_102954|690x316](upload://5cQrr0E7BEV5PAK915LXyGtGMov.jpeg)
```

---
## \#9 Posted by: Andy87 Posted at: 2019-04-18T09:25:38.972Z Reads: 21

```
looks like you already tried different cables right? If no, do so.

Also switch of bluetooth on your laptop just in case it´s on.

Check if you have all driver installed you need. Should be if you used it before, but who knows, never bad to check that.
https://www.st.com/en/development-tools/stsw-stm32102.html
```

---
## \#10 Posted by: 2Fat2Fly Posted at: 2019-04-18T09:29:02.305Z Reads: 21

```
I tried that link but it couldn't find any flight controller
![IMG_20190418_112744|229x500](upload://tXLW5xMNUO6epF1KksubEmG82aQ.jpeg)
```

---
## \#11 Posted by: 2Fat2Fly Posted at: 2019-04-18T09:32:09.756Z Reads: 16

```
And yes I've tried 7 different cables
```

---
## \#12 Posted by: 2Fat2Fly Posted at: 2019-04-18T09:33:06.487Z Reads: 16

```
It just continues searching 

![IMG_20190418_113216|229x500](upload://AoFJZgXGkSHt4ewlysCX58WazKo.jpeg)
```

---
## \#13 Posted by: Andy87 Posted at: 2019-04-18T09:35:29.043Z Reads: 17

```
try this one

https://www.st.com/en/development-tools/stsw-stm32102.html

might be easier

and check if your USB port is set to auto detect.
```

---
## \#14 Posted by: 2Fat2Fly Posted at: 2019-04-18T09:38:33.534Z Reads: 17

```
Wich of the programs should I run and how do I check my USB port is set to auto detect
```

---
## \#15 Posted by: Andy87 Posted at: 2019-04-18T09:40:17.294Z Reads: 16

```
in the last link you should find the right driver you need.

unfortunately I can´t tell you how to set it to auto detect on a WIN pc. Might just need to goolgle it. shouldn´t be a big thing.
```

---
## \#16 Posted by: Andy87 Posted at: 2019-04-18T09:43:45.066Z Reads: 16

```
If you plug in the USB cable to your PC and the focbox, you hear a ping noice that the device was recognized?
```

---
## \#17 Posted by: 2Fat2Fly Posted at: 2019-04-18T09:44:04.352Z Reads: 16

```
Sadly I don't.
```

---
## \#18 Posted by: 2Fat2Fly Posted at: 2019-04-18T09:54:19.945Z Reads: 16

```
I have tried 3 different computers as well
```

---
## \#19 Posted by: Andy87 Posted at: 2019-04-18T10:10:05.817Z Reads: 15

```
hm that sound not good.
how the LEDs on the focbox when you power everything on? some red light blinking?

maybe some dirt came inside of the mini usb on the focbox?
```

---
## \#20 Posted by: 2Fat2Fly Posted at: 2019-04-18T10:18:17.533Z Reads: 14

```
the is a blue and green light on both foc boxes
```

---
## \#21 Posted by: Andy87 Posted at: 2019-04-18T10:19:20.711Z Reads: 13

```
and you have same issue on both of them?
```

---
## \#22 Posted by: 2Fat2Fly Posted at: 2019-04-18T10:23:25.678Z Reads: 13

```
yes i have the same problem on both, wich is weird because i installed the firmware maybe two month ago and back then it worked fine.
```

---
## \#23 Posted by: 2Fat2Fly Posted at: 2019-04-18T10:24:59.560Z Reads: 11

```
And I worked afterwards as well. So I know for a fact that the firmware installed correctly. I just didn't have all my parts, so I didn't finish me setup
```

---
## \#24 Posted by: Andy87 Posted at: 2019-04-18T10:29:11.083Z Reads: 12

```
jap that´s strange, you used 

7x different cables

different pc´s 

have all drivers

no red LEDs

USB port is clean

and same issue on different focboxes.


Do you remember you shorted something on the usb port maybe during that time?
```

---
## \#25 Posted by: meesie Posted at: 2019-04-18T10:29:36.705Z Reads: 11

```
i remember somthing about there being a "charge only" cable and a "communication" cable when talking about micro USB. maybe it's that?
```

---
## \#26 Posted by: 2Fat2Fly Posted at: 2019-04-18T10:32:04.886Z Reads: 11

```
im not sure about drivers but i have been looking through everything i can find, i have tried 7 different cables 3 different computers, tried different usb ports on the computers, i have tried lokking for dirt in the ports. 99 % sure i didnt short anything.
```

---
## \#27 Posted by: 2Fat2Fly Posted at: 2019-04-18T11:34:41.671Z Reads: 9

```
I really appreciate all the help and ideas :slight_smile:
```

---
