# VESC gurus, please help!

### Replies: 33 Views: 615

## \#1 Posted by: robthebuilder Posted at: 2019-04-18T06:19:40.609Z Reads: 169

```
Hi guys! :)

I have a problem I've never encountered before. I just got a new VESC 4.12 from TB for my dual motor setup.

Last week I upgraded the firmware on my old VESC (also from TB) to 3.54 with the latest VESC Tool and it was seamless. Now that I try to upgrade the new VESC it says that my firmware is too old, just like the old one. But when I've upgraded the firmware and reconnected the VESC, it still says that the firmware is too old.

It doesn't seem to store the new firmware. I've also tried to upgrade the bootloader but it doesn't fix the problem.

This is what I use:

VESC Tool - Version 1.08

VESC HW - Version 4.12

VESC FW - Version 3.50 (I want to upgrade to version 3.54 like my other VESC).


Please help me! :disappointed_relieved:
```

---
## \#2 Posted by: robthebuilder Posted at: 2019-04-18T06:25:54.290Z Reads: 156

```
Or, is it possible to download the correct VESC Tool that supports FW version 3.50? I can't find it anywhere :/
```

---
## \#3 Posted by: Friskies Posted at: 2019-04-18T06:45:45.067Z Reads: 147

```
You would have to download the older firmware and manually install it or just use the tool that you originally used with your other Vesc. I would just update both with the new tool.

https://vesc-project.com/vesc_tool
```

---
## \#4 Posted by: robthebuilder Posted at: 2019-04-18T06:52:56.671Z Reads: 140

```
Thanks for ur reply! :)

I used the new tool for my old VESC. Same tool for this one but still it doesn't want to upgrade...
```

---
## \#5 Posted by: Friskies Posted at: 2019-04-18T06:57:17.590Z Reads: 128

```
Oh interesting... And they are both the same hardware?
```

---
## \#6 Posted by: robthebuilder Posted at: 2019-04-18T06:57:59.520Z Reads: 117

```
Yup, HW 4.12

But the old one came with FW 2.18 and the new one with FW 3.50
```

---
## \#7 Posted by: Andy87 Posted at: 2019-04-18T06:58:53.996Z Reads: 112

```
I would double check the bootloader thing. I know you checked, but usually missing bootloader is what does not give you to update a new FW.
```

---
## \#8 Posted by: robthebuilder Posted at: 2019-04-18T07:02:12.154Z Reads: 108

```
Thanks!

The thing is that it does actually write the new firmware, it just doesn't seem to save it.. It writes just fine but then when I reconnect it still says that it's too old.. :(
```

---
## \#9 Posted by: Friskies Posted at: 2019-04-18T07:16:30.119Z Reads: 102

```
Maybe just install acks firmware instead and see how that goes?
```

---
## \#10 Posted by: robthebuilder Posted at: 2019-04-18T07:32:17.241Z Reads: 99

```
Oh, haven't heard of that. Does it work with VESC Tool? :)
```

---
## \#11 Posted by: Andy87 Posted at: 2019-04-18T07:32:18.348Z Reads: 96

```
I think that’s exactly what it looks like if no bootloader. Vesc tool will not give you a fault message. You can start the fw flashing and it finish successfully, but after reboot the fw is not updated.

I think with the new vesc tool you can upload the bootloader without need of an st v2 link. Just give it a try.
```

---
## \#12 Posted by: robthebuilder Posted at: 2019-04-18T07:33:00.131Z Reads: 93

```
Yup, that's what I did. I uploaded the bootloader with the latest VESC Tool!
```

---
## \#13 Posted by: Andy87 Posted at: 2019-04-18T07:33:14.409Z Reads: 88

```
You need the ackmaniac version of the vesc tool, but if your bootloader not give you to update that will also not work.
```

---
## \#14 Posted by: robthebuilder Posted at: 2019-04-18T07:34:13.379Z Reads: 85

```
Ok, this is so wierd :confused:
```

---
## \#15 Posted by: Andy87 Posted at: 2019-04-18T07:34:34.491Z Reads: 87

```
Did you try loading any other older fw? Maybe 3.38 or something you have at home?
```

---
## \#16 Posted by: robthebuilder Posted at: 2019-04-18T07:36:11.885Z Reads: 87

```
No I don't have anything else than the one installed..
```

---
## \#17 Posted by: robthebuilder Posted at: 2019-04-18T07:36:34.333Z Reads: 86

```
Oh, yes I've tried with an older version of VESC Tool
```

---
## \#18 Posted by: Andy87 Posted at: 2019-04-18T07:37:18.594Z Reads: 91

```
The same?[](http://)
```

---
## \#19 Posted by: trampa Posted at: 2019-04-18T07:55:52.262Z Reads: 93

```
You need to use one ESC as a programmer to flash the other. 
Simply connect both SWDs together (GND IO and CLK only)
GND to GND, IO to IO, CLK to CLK. Cables should be  short, 6-8cm only!

Then you connect to the working ESC ( the one with the latest FW on) via VESC-Tool and open the SWD PROG tab.
Now you flash the non working ESC with the 410,411,412 file.

Easy!
```

---
## \#20 Posted by: Friskies Posted at: 2019-04-18T07:59:38.159Z Reads: 91

```
That's a cool way to do it. so for people that don't have st link they just need to make a cable if they have a dual setup. 

I would have thought that without the bootloader the esc won't even connect to the PC though..
```

---
## \#21 Posted by: robthebuilder Posted at: 2019-04-18T08:01:00.175Z Reads: 85

```
Awesome! I will try this after work! :D
```

---
## \#22 Posted by: trampa Posted at: 2019-04-18T08:03:02.763Z Reads: 85

```
don't spin a motor while you are connected!
```

---
## \#23 Posted by: trampa Posted at: 2019-04-18T08:05:12.927Z Reads: 84

```
It's a little hack for your convenience. A present from Benjamin to the community. It was not easy to implement but is very beneficial.
```

---
## \#24 Posted by: robthebuilder Posted at: 2019-04-18T10:00:26.941Z Reads: 78

```
AMESOME! It worked :D :D Thank you so much! This was a great fix! :star_struck:
```

---
## \#25 Posted by: trampa Posted at: 2019-04-18T11:47:25.663Z Reads: 74

```
You are welcome!
```

---
## \#26 Posted by: tecknocreeper Posted at: 2019-04-30T12:34:11.231Z Reads: 64

```
could you post a tutorial of this? 
im a having the same issue
```

---
## \#28 Posted by: robthebuilder Posted at: 2019-05-13T12:46:19.929Z Reads: 61

```
Just follow the steps Trampa posted above! :)

[quote="trampa, post:19, topic:90962, full:true"]
You need to use one ESC as a programmer to flash the other. Simply connect both SWDs together (GND IO and CLK only) GND to GND, IO to IO, CLK to CLK. Cables should be short, 6-8cm only!

Then you connect to the working ESC ( the one with the latest FW on) via VESC-Tool and open the SWD PROG tab. Now you flash the non working ESC with the 410,411,412 file.

Easy!
[/quote]
```

---
## \#29 Posted by: trampa Posted at: 2019-05-13T13:11:30.043Z Reads: 57

```
Both VESCs should be powerd by a battery, so that both STM processors are up and running.
Both VESCs are interconnected SWD to SWD ( GND, IO and CLK only)

Open the **SWD PROG** tab (menu on the left at the bottom), hit connect and then you select the VESC you have and click upload. Programming has never been easier!
Make sure not to choose the wrong hardware! 
When the upload has been done, you wait for 10 seconds and disconnect everything and then you are good to give things a try.
```

---
## \#30 Posted by: kchxaz Posted at: 2019-08-08T08:16:51.074Z Reads: 35

```
Why the 410, 411, 412 file? I think my VESC 6.6 dual came with 60 on it. Or at least thats what has always been on it for me. Irregardless that I am having major issues with cogging and not being able to get both sides of the VESC to run properly. It's maddening..

What does flashing the bootloader do? Is something corrupt maybe?
```

---
## \#31 Posted by: robthebuilder Posted at: 2019-08-08T12:31:17.809Z Reads: 30

```
Since I'm using VESC 4.12
```

---
## \#32 Posted by: kchxaz Posted at: 2019-08-16T01:05:02.116Z Reads: 26

```
Quick technical question here: Trampa indicates that the SWD cable should be 6-8cm in length...why? Is there too much internal resistance in the wire?

Edit: Actually, that question was for anyone/everyone if they have any input....

Much oblige mates
```

---
## \#33 Posted by: trampa Posted at: 2019-08-16T10:05:29.030Z Reads: 24

```
Longer cables cause problems on SWD. 

This is an explanation for JTAG, which is similar to SWD when it comes to max cable lengths. 
http://infocenter.arm.com/help/index.jsp?topic=/com.arm.doc.dui0517b/Chdbgcdj.html
```

---
## \#34 Posted by: kchxaz Posted at: 2019-08-17T21:21:57.728Z Reads: 15

```
Still having issues, soooo when you say disconnect everything else, do you mean the 3 motor wires too (non-sensored motors so hall sensors wires N/A)? Remote or bluetooth (if we have one)? 

We need to have at least one USB data cable connected to the good VESC of course, right?
```

---
