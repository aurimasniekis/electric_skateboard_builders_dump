# Vesc Can&rsquo;t connect to Pc

### Replies: 22 Views: 2407

## \#1 Posted by: solarscape Posted at: 2016-12-31T18:41:35.278Z Reads: 134

```
HI i plugged in the vesc usb and plug the battery into it yet on the bldc tool it doesn't show any ports simply not connected. I checked device manager and it shows up as chibiOS/RT Virtual COM Port. Blue and red light is on whenever I turn the vesc is flashes three times and stays on. I downloaded the bldc tool from the vesc website where I type in my email and get the files. I tried switching usb cables but didn't change anything. Please help asap.
```

---
## \#2 Posted by: chuttney1 Posted at: 2016-12-31T19:05:54.245Z Reads: 133

```
I am assuming you gave it a few minutes for Windows to install the drivers before accessing VESC. Which light stays on? Blue, red or green. I think blue is power, red is errors, and green is for STM32F4 chip. The lights just for clarification that one or both lights are on after startup.
```

---
## \#3 Posted by: JohnnyMeduse Posted at: 2016-12-31T19:13:32.395Z Reads: 129

```
If the red flash 3 time at the start, it mean that the bootloader is instal, so it should be alright
```

---
## \#4 Posted by: solarscape Posted at: 2016-12-31T19:29:29.791Z Reads: 125

```
update: mottor dectection works and vesc is connected everything works except the remote ocnnection. I have the 2.4ghz rc remote I set it to ppm I folowed the pairing insturction but to no avial it doesnt work.
```

---
## \#5 Posted by: Alextech Posted at: 2016-12-31T22:07:43.667Z Reads: 108

```
What remote do you have?
```

---
## \#6 Posted by: solarscape Posted at: 2017-01-01T05:14:52.691Z Reads: 89

```
TorqueBoards 2.4Ghz Mini Remote Controller
```

---
## \#7 Posted by: shwill Posted at: 2017-01-01T05:37:16.519Z Reads: 85

```
Which version of bldc .might need old Windows version download for it to sync up that was an issue I ran into but I'm new to this stuff so don't know just a thought.
```

---
## \#8 Posted by: solarscape Posted at: 2017-01-01T05:39:17.568Z Reads: 82

```
i believe 2.18
```

---
## \#9 Posted by: solarscape Posted at: 2017-01-01T06:17:08.564Z Reads: 80

```
im using the enertion standard vesc what verison and firmware should I have used?
```

---
## \#10 Posted by: Pathaim Posted at: 2017-01-01T06:25:46.156Z Reads: 77

```
Did you watch jacobs vide about setup? he explains how to setup your controller. http://vesc.net.au/ has it all,
```

---
## \#11 Posted by: solarscape Posted at: 2017-01-01T08:40:09.246Z Reads: 69

```
yes i did but no matter what my controller isnt moving the hub motor
```

---
## \#12 Posted by: rwxr Posted at: 2017-01-01T14:33:21.314Z Reads: 67

```
Post screenshots from bldc-tool please
```

---
## \#13 Posted by: solarscape Posted at: 2017-01-01T20:12:34.916Z Reads: 65

```
<img src="/uploads/db1493/original/3X/6/0/6006e8d8a9b8e673010e4709ea7657b01f2a1c59.png" width="690" height="407"><img src="/uploads/db1493/original/3X/1/7/1740f882df6c89d60e7ee55c142692a0c79b9983.png" width="690" height="406"><img src="/uploads/db1493/original/3X/7/4/74207abb8e5ce63de4e3172e0177ed96f39d5843.png" width="690" height="407"><img src="/uploads/db1493/original/3X/b/8/b8c005bc2c2daa51b01e42c000ca19c8fd36dbbd.png" width="690" height="407"><img src="/uploads/db1493/original/3X/a/f/af8411916eb76b7f7d99f97eba6bfaf20d3affba.png" width="690" height="407"><img src="/uploads/db1493/original/3X/d/f/df0b386d50a87d5ddd19a70f34d09323081a9162.png" width="690" height="407"><img src="/uploads/db1493/original/3X/3/a/3a2cadffd583f07692ddcb94df9d2f508835a8ce.png" width="690" height="406"><img src="/uploads/db1493/original/3X/d/f/df791e55aca91f46c790672267ea2b68e01ab03b.png" width="690" height="407"><img src="/uploads/db1493/original/3X/6/4/64a245c6b3757e8bb001d0b02c4ab1cc94de8c77.png" width="690" height="407"><img src="/uploads/db1493/original/3X/f/d/fd1f4a21ccf88733c2eb7639851897ba99b3a831.png" width="690" height="406"><img src="/uploads/db1493/original/3X/2/5/2562e73aa7315c5b1dba5825ed30f3c2ce3ad041.png" width="690" height="406">
```

---
## \#14 Posted by: Ackmaniac Posted at: 2017-01-01T20:17:42.704Z Reads: 51

```
Please check first if you have the 3 wires from right vesc to the remotes receiver connected correctly.
```

---
## \#15 Posted by: solarscape Posted at: 2017-01-01T20:19:08.640Z Reads: 52

```
yes its connected correctly
```

---
## \#16 Posted by: Ackmaniac Posted at: 2017-01-01T20:20:04.576Z Reads: 53

```
Is the remote already  binded to the receiver?
```

---
## \#17 Posted by: solarscape Posted at: 2017-01-01T20:22:13.032Z Reads: 55

```
yes
i followed every instruction the diyelectricskateboard video said to do
```

---
## \#18 Posted by: JohnnyMeduse Posted at: 2017-01-01T21:23:04.073Z Reads: 52

```
did you reboot your vesc after setting the app in PPM mode... (and before setting the rest in the ppm tab)
```

---
## \#19 Posted by: Namasaki Posted at: 2017-01-01T21:46:18.785Z Reads: 50

```
which receiver channel do you have the vesc plugged into?
```

---
## \#20 Posted by: Namasaki Posted at: 2017-01-01T21:54:24.157Z Reads: 47

```
https://youtu.be/OtuofrQr3F8
```

---
## \#21 Posted by: solarscape Posted at: 2017-01-01T21:54:24.600Z Reads: 45

```
yes i did reboot i used channel 2
```

---
## \#22 Posted by: solarscape Posted at: 2017-01-02T07:28:17.184Z Reads: 40

```
So i tried using another version of bldc but then when I got to device manager, chibios/rt virtual com port shows up and it needs to be updated but so far I can't get it to update
```

---
