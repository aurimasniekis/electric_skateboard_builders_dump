# USB devices Disabled

### Replies: 8 Views: 1186

## \#1 Posted by: malik Posted at: 2016-04-24T13:29:11.879Z Reads: 77

```
Hello,

I am plugging the VESC to USB, with or without power source, and I always get the same notification:

"USB devices Disabled - Unplug the device using too much power to re-enable USB devices."

I have tired on Mac, Ubuntu and the result is the same. 

Anyone has solved this issue already?

Thank you
```

---
## \#2 Posted by: Ulfberht Posted at: 2016-04-24T20:56:00.492Z Reads: 60

```
This might sound silly, but did you try using different cables? I've had experiences with USB where one cable works and one doesn't. Not sure why. Both cables might transfer data, but one might not charge my phone or power up a device. I'd also test that USB port to see if other devices work.
```

---
## \#3 Posted by: malik Posted at: 2016-04-27T10:58:16.885Z Reads: 40

```
hello sorry for late reply. 
yes i have tried different cables of course and still the same. The usb port is not the problem nor the cable.
I removed the cables's connector to keep just the pins, plugged them upside down and it worked. But i have been told it is not an issue. How come? I dont understand what's the deal with it.
thank you
```

---
## \#4 Posted by: chaka Posted at: 2016-04-27T13:11:14.933Z Reads: 36

```
Sounds like you have a VESC with the incorrect usb port attached. Upload a picture, let see what we are dealing with.
```

---
## \#5 Posted by: malik Posted at: 2016-04-27T13:21:53.927Z Reads: 35

```
I am pretty sure it is upside down, but the design on github were like this. Actually, i dismounted a usb cable, wired everything the other way around (pin1->pin5... pin5->pin1) and it worked perfectly. the only thing is that it is not a sustainable technic and might end up breaking the usb connector.
Here are 2 pics:

<img src="/uploads/db1493/original/2X/5/5e29e2bea02d0e1f352a26c395b43d39a819f914.JPG" width="666" height="500">
<img src="/uploads/db1493/original/2X/c/c6cdcbdbca767def97cf2fe7d6a79f4c2449a9c8.JPG" width="375" height="500">
```

---
## \#6 Posted by: chaka Posted at: 2016-04-27T13:44:19.455Z Reads: 35

```
Sweet, you found your problem! You have a couple of options, splice a usb cable in reverse or rework the pcb to change out the port with the correct part. Reworking would require a hot air station.
```

---
## \#7 Posted by: malik Posted at: 2016-04-27T14:37:30.733Z Reads: 31

```
Can I do it otherwise with bluetooth for instance? reworking the pcb is not in my skills at all.
```

---
## \#8 Posted by: chaka Posted at: 2016-04-27T16:53:22.111Z Reads: 26

```
Just cut the cord and rewire it in reverse if you want to hobble it together, no shame in that. Get it rolling!
```

---
