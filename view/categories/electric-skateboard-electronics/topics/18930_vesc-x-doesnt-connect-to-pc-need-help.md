# Vesc X doesnt connect to PC, need help

### Replies: 21 Views: 1847

## \#1 Posted by: KenTw Posted at: 2017-03-12T03:55:44.794Z Reads: 135

```
Guys, can anyone help me out?
i got both of my vesc x connected to the space cell 4 battery and to the 6374 motors from enertion
but when i plugged it onto my PC the BLDC doesnt seem to recognize the vesc x
i tried five different usb cables, including the one provided by the nano x remote, still doesnt work
i then tried on my laptop and my dad's desktop and still no signs of BLDC connecting to my vesc X....
what did i do wrong? or is this just faulty vesc?
i dont know man, the lights are on when i turned on the battery, so i know they arent dead, but they just dont seem to connect to any computer with any usb cables....
help please, anyone?
```

---
## \#2 Posted by: JLabs Posted at: 2017-03-12T04:05:34.638Z Reads: 133

```
Are you positive that'll all of your connections are right? What firmware do you have selected?
```

---
## \#3 Posted by: SeanHacker Posted at: 2017-03-12T04:46:36.020Z Reads: 134

```
Hopefully the USB cables are data transfer capable. Some only work for charging. Also. Depending on if you're using Windows, make sure you have those installed and reboot the computer.
```

---
## \#4 Posted by: Alextech Posted at: 2017-03-12T05:19:31.747Z Reads: 127

```
Do you have the drivers installed my man?
```

---
## \#5 Posted by: Luke Posted at: 2017-03-12T05:26:42.865Z Reads: 120

```
I was trying to help him earlier, we had the vescs plugged in right, but didnt check for drivers. Is it even possible to select firmware if it cant even connect to BLDC tool?
```

---
## \#6 Posted by: Alextech Posted at: 2017-03-12T05:28:30.442Z Reads: 113

```
That's a negative.
```

---
## \#7 Posted by: JohnnyMeduse Posted at: 2017-03-12T05:31:54.992Z Reads: 110

```
@KenTw did you try to contact enertion support, on there web site. ?
```

---
## \#8 Posted by: SeanHacker Posted at: 2017-03-12T05:58:31.632Z Reads: 109

```
No need to worry about firmware yet. Gotta get the computer to detect the USB device (vesc).  What operating system? Windows? Ubuntu?
```

---
## \#9 Posted by: Luke Posted at: 2017-03-12T06:09:25.397Z Reads: 105

```
It was windows
```

---
## \#10 Posted by: KenTw Posted at: 2017-03-12T06:20:00.361Z Reads: 105

```
I gave their website and their email my problem, havent had replies
The 5 usbs cables, two of them are used to transfer data from my phone and a sony camera, so should be data transferable
Not too sure about the other two and the nano x one, but all of them didnt detect the vesc x
And this exact setup was again ran through my laptop
```

---
## \#11 Posted by: KenTw Posted at: 2017-03-12T06:22:53.363Z Reads: 103

```
I also checked if the pc usb prt was faulty, but it read my mouse, my camera and phone memory, and an SD card reader all fine... But somehow both computers failed to read the vescx
But the vesc x looks fine, not like I can tell if it is working or not, but at least I can tell that the battery is giving it juice cuz it has a stable blue light
```

---
## \#12 Posted by: SeanHacker Posted at: 2017-03-12T06:38:49.623Z Reads: 101

```
You could setup a virtualbox and run Ubuntu to see if that works. I know nothing about Windows at all. Haven't run it in many years. If you do get a VB setup you can just follow the instructions here. http://vedder.se/2015/01/vesc-open-source-esc/

Wish I could help out more. Sounds like Windows needs drivers for it to pickup your vescs.
```

---
## \#13 Posted by: Luke Posted at: 2017-03-12T09:06:21.854Z Reads: 98

```
if it's an issue of drivers could it mean that other computers could work for him? I've helped set up plenty of vescs for people and never had to deal with installing drivers
```

---
## \#14 Posted by: thylen11 Posted at: 2017-03-12T10:27:14.827Z Reads: 89

```
I had the dame problem. I swapped pc and used my laptop and I didnt have a problem there. If you can try a different computer/laptop
```

---
## \#15 Posted by: KenTw Posted at: 2017-03-12T10:31:37.046Z Reads: 87

```
ok, ill try it at my office tmr xD
thanks for the suggestions guys!
```

---
## \#16 Posted by: KenTw Posted at: 2017-03-12T10:41:35.355Z Reads: 85

```
question, am i suppose to see the vesc x in the my computer folder?
like u know how we get to see phones, cameras, on the my computer folder but not mouse and keyboard
i want to know if vesc x is suppose to be there when connected, if it is it would be easier for me to go to other computers and try them out without installing the BLDC onto every one of them
can any users vertiify this?
```

---
## \#17 Posted by: thylen11 Posted at: 2017-03-12T12:00:52.765Z Reads: 82

```
My pc's both gave me the sound of a new device connecting. However on the PC that didn't read the vesc there was a warning right after the sound. On the laptop where the vesc was reading and interacting with the BLDC tool the sound of a device connecting was there but not the warning. Hope that helps. Otherwise it's just trying GL!
```

---
## \#18 Posted by: JohnnyMeduse Posted at: 2017-03-12T13:49:50.220Z Reads: 81

```
did you press the refresh arrow in the bldc tool, before the connect button. 

<img src="/uploads/db1493/original/3X/5/f/5fcd3bfb8d6fdb2ca37c4f6991478722db454e0f.jpg" width="690" height="402">
```

---
## \#19 Posted by: KenTw Posted at: 2017-03-12T15:07:48.147Z Reads: 75

```
GUYS, i tried it again tonight and it magically worked...
idk all i did was change the com1 to com3
i still dont get why this would different the result, but yeah thats how it worked for me
com1 i cant find the vesc but com 3 it found my vesc!
```

---
## \#20 Posted by: flatsp0t Posted at: 2017-03-13T21:24:27.088Z Reads: 67

```
Well, this are different virtual Serial Ports. if there is already a device on COM1, the VESC will not be able to mount there.
```

---
## \#21 Posted by: CaptainMerricka Posted at: 2017-03-13T21:46:14.119Z Reads: 64

```
for me it wasnt working at first. 
Problem 1 was using a crappy cable.
Problem 2) I have to open BLDC tool AFTER I plug in the vesc. Otherwise it never finds it.
```

---
