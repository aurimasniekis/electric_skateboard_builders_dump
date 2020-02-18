# VESC not recognized by os

### Replies: 21 Views: 2434

## \#1 Posted by: ferricx Posted at: 2016-05-26T14:08:06.766Z Reads: 159

```
I have 2 VESCs hw v4.10. One connects to bldc tool, one does not. I get the blue light on the vesc, but nothing else. It is not recognized by the os. 
I have 3 different pcs and 6 usb cables.

Here is what I get:
Connected to win 10, 8, 7, xp - not in device manager. No new device at all.
Connected to Linux (ubuntu, centos) - dmesg results: no vesc, no unknown device.

Connected to working vesc via canbus -  bldc tool: set CAN Fwd get message that cannot connect

Connected to 2 different stlink V2 - make upload: init failed. 

All of these techniques work on the other vesc(except canbus of course) , the one that works.

I have also had stlink wiring checked by someone at vedder's site and it works on the other vesc.
```

---
## \#2 Posted by: JTAG Posted at: 2016-05-27T10:07:30.148Z Reads: 125

```
With respect to ground; is there 3.3V present on the reset and 3.3V pin?
```

---
## \#3 Posted by: ferricx Posted at: 2016-05-28T02:23:12.589Z Reads: 112

```
Yes. 3.3V on both
```

---
## \#4 Posted by: JTAG Posted at: 2016-05-28T11:49:48.498Z Reads: 106

```
To bad, that would have been an easy fix.

There are now 4 main options:
1) the crystal is incorrect / bad soldered.
2) crystal capacitors are bad / wrong value
3) Wrong or no firmware (do you have programmer?)

Or just the general soldering errors around USB / micro controller.
```

---
## \#5 Posted by: ferricx Posted at: 2016-05-28T12:41:35.508Z Reads: 102

```
Yes. I have 2 different stlink v2. I can't get the make upload to work on the bad vesc. I can get each stlink to connect to os properly. But when I try make upload, I get:

Error: open failed in procedure 'transport' 
** OpenOCD init Failed **
shutdown command invoked.
```

---
## \#6 Posted by: JTAG Posted at: 2016-05-28T13:25:42.943Z Reads: 96

```
My apologies, I don't know where my mind was neglecting you tried to program them with a debugger :(.

Well, in this case (3.3 present and reset @ 3.3):
The STM needs only power to be programmed -> check for shorts and opens in the program wires and if STM is placed with correct orientation ( happend to me, don't laugh). Can you maybe post a few pictures?
```

---
## \#7 Posted by: ferricx Posted at: 2016-05-28T13:50:42.197Z Reads: 95

```
<img src="/uploads/db1493/original/2X/0/023f508686b3139b8692d34e3920e951f526945a.jpg" width="690" height="388"><img src="/uploads/db1493/original/2X/1/19669c2ed57e3e5e77c652a6b06a520a21615234.jpg" width="690" height="388">

Wires are 6" long.
```

---
## \#8 Posted by: ferricx Posted at: 2016-05-28T13:56:09.132Z Reads: 90

```
<img src="/uploads/db1493/original/2X/7/75a3418be0b84a8100ccf2ed6d52857d18a226d0.jpg" width="690" height="388">
other programmer
```

---
## \#9 Posted by: ferricx Posted at: 2016-05-28T13:59:04.900Z Reads: 86

```
when i connect either, I get blue light on vesc
```

---
## \#10 Posted by: chaka Posted at: 2016-05-28T14:16:55.211Z Reads: 85

```
You need to connect the data pin, also known as SWIM. On the VESC it is the 6th pin, unlabeled.
```

---
## \#11 Posted by: ferricx Posted at: 2016-05-28T15:13:15.908Z Reads: 84

```
still fails. same error on make upload
```

---
## \#12 Posted by: chaka Posted at: 2016-05-28T15:17:51.886Z Reads: 84

```
Check all the pins on the stm32 chip. Might have a small bridge somewhere.
```

---
## \#13 Posted by: ferricx Posted at: 2016-05-28T15:25:43.175Z Reads: 83

```
ok, checked all the connections. seemed ok. switched to other programmer. same error
```

---
## \#14 Posted by: ferricx Posted at: 2016-05-28T15:36:13.792Z Reads: 81

```
checked continuity on the back of each board. all jumpers are working
```

---
## \#15 Posted by: chipoi84 Posted at: 2016-05-28T15:52:21.496Z Reads: 80

```
I think something might be wrong with the mcu. You might need to replace it. Check for bridges.
```

---
## \#16 Posted by: JTAG Posted at: 2016-05-28T16:46:20.695Z Reads: 76

```
If your wires are really 6" long I am supprised that you managed to program the other ones( did you program the others?). I have bad experience with long wires ( unless you lowered the swd clock speed ).

All other stuff sounds and looks like it should work. Where are you situated? Your name sounds France?
```

---
## \#17 Posted by: ferricx Posted at: 2016-05-28T18:10:03.819Z Reads: 72

```
6" is 6 inches not much longer than the width of my hand
```

---
## \#18 Posted by: ferricx Posted at: 2016-05-28T18:11:51.509Z Reads: 70

```
And I am in denver colorado, usa
```

---
## \#19 Posted by: ferricx Posted at: 2016-06-05T14:35:04.202Z Reads: 65

```
I have carefully looked over the entire board under magnificaion. All the solder joints look perfect to me.
Not sure what to do now.
```

---
## \#20 Posted by: chipoi84 Posted at: 2016-06-05T15:52:58.767Z Reads: 63

```
At this point, you might as well try re-flowing the whole pcb with flux and a heat gun.
```

---
## \#21 Posted by: ferricx Posted at: 2016-06-06T20:43:41.460Z Reads: 61

```
Thing is, I bought these from enertionboards.
```

---
