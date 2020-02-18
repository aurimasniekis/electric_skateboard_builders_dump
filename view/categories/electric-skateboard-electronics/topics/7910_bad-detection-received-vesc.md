# Bad Detection Received VESC

### Replies: 59 Views: 4678

## \#1 Posted by: kaiser Posted at: 2016-08-19T17:23:36.133Z Reads: 231

```
Hi 

2 phases hit each other shortly when the motor did like a half spin :/  but it seem like everything looks good , how to see what is defekt or what is working 

i can't get my vesc to detect my motor,, It worked at the start and now it won't work anymore :/ 
can u guys tell whats is worng

It says under terminal when typing fault = FAULT_CODE_NONE
vesc blinks red when pressing the arrow keys 
and when start motor detection,,= Bad Detection Received "in the corner where there stands connected" and Detection failed. in the main window

Battery 7S
 29 V 
7.8 Ah
202WH

Enertion singel motor biggest

(Have tryed to update firmware did not help)

<img src="/uploads/db1493/original/2X/2/2d455320666aacf0d3f16ec99f6c4a16f6e1b8da.png" width="690" height="365"><img src="/uploads/db1493/original/2X/c/c87e1708588d05d60fc53de139ca4bb0c6c683d2.png" width="690" height="365"><img src="/uploads/db1493/original/2X/5/5880137cad5672349317b7f7e8442045ae846f73.png" width="690" height="366"><img src="/uploads/db1493/original/2X/4/441577a053ded59bc7a76381694a78ad26579007.png" width="690" height="365"><img src="/uploads/db1493/original/2X/5/5916624fbb0c58eeeb35519ec8fa94170c196102.png" width="690" height="364">
```

---
## \#2 Posted by: Jinra Posted at: 2016-08-19T17:25:53.389Z Reads: 201

```
Change your max input voltage back to 57v. There's no need to change it from default. Also your cut off is triggering that's why your detection is failing. Your starting battery cut off at 4.1v per cell (29/7). You should really have it at about 3.3v per cell if you're running li-ion 18650s, or 3.5-3.6~ for lipos.

Reset your detection parameters to default as well (6A current, 600 min erpm, .05 low duty)

Lastly, round down the integrator limit to the lowest 5 and bemf coupling to the lowest 50
```

---
## \#3 Posted by: kaiser Posted at: 2016-08-19T17:39:12.428Z Reads: 199

```
Like so? (many i still did something wrong , have also tried whint only default settings)
yes its Panasonic 18650
<img src="/uploads/db1493/original/2X/e/e2b869de53e2a7d94cbbc8d57440b18a3acc6d7d.png" width="690" height="364"><img src="/uploads/db1493/original/2X/d/d10ecc55431e544c41822f1eac6aadd73588b8d1.png" width="690" height="364">
```

---
## \#4 Posted by: Jinra Posted at: 2016-08-19T17:40:37.358Z Reads: 168

```
Your cutoff end should always ben lower than cut off start. Cut off start is when your VESC starts powering down and cut off end is when your VESC completely shuts off. Change the cut off end to 21 or 22 volts.

Also change your detection parameters back to default.
```

---
## \#5 Posted by: kaiser Posted at: 2016-08-19T17:44:22.631Z Reads: 175

```
hmm nope  :/ (Default bldc didt not work either)
<img src="/uploads/db1493/original/2X/1/1d7b9437eca2d87c850e799ef28fe5575736e088.png" width="690" height="365"><img src="/uploads/db1493/original/2X/5/511674dc10b971b5e289cde88ac5cff410130f65.png" width="690" height="365">
```

---
## \#6 Posted by: Jinra Posted at: 2016-08-19T17:45:33.660Z Reads: 155

```
Did you write config before you started detection again? Every change you make you have to write config. Rebooting the VESC doesn't hurt either.
```

---
## \#7 Posted by: kaiser Posted at: 2016-08-19T17:46:02.181Z Reads: 155

```
Yes yes :/
```

---
## \#8 Posted by: Jinra Posted at: 2016-08-19T17:46:53.217Z Reads: 152

```
Can you try changing detection parameters back to default? You still have them on 14A current 690 min erpm and .13 low duty
```

---
## \#9 Posted by: kaiser Posted at: 2016-08-19T17:48:00.922Z Reads: 151

```
<img src="/uploads/db1493/original/2X/3/37d6715431646e141aaca45bfe484cebd62f654e.png" width="690" height="365">
```

---
## \#10 Posted by: kaiser Posted at: 2016-08-19T17:49:08.157Z Reads: 140

```
This menu is default settings now
```

---
## \#11 Posted by: Jinra Posted at: 2016-08-19T17:50:46.235Z Reads: 143

```
This is what I'm asking you to change

<img src="/uploads/db1493/original/2X/2/2b481e24e4189081643885126c18f7307db4c7c1.jpg" width="690" height="365">
```

---
## \#12 Posted by: kaiser Posted at: 2016-08-19T17:56:16.157Z Reads: 142

```
<img src="/uploads/db1493/original/2X/9/9b6ed0cd7e5911cf5c26c2c316f1cb50927405e1.png" width="690" height="364">
Like so?
```

---
## \#13 Posted by: Jinra Posted at: 2016-08-19T17:58:25.474Z Reads: 139

```
Yep, so it seems settings are now correct. They definitely would not work the way it was before. Now, make sure your phase wires aren't shorting on each other and that the rotor can on the motor spins pretty freely. If there's heavy resistance on the can, then the phase wires are shorting out. Make sure none of the phase wires metal parts are touching.
```

---
## \#14 Posted by: kaiser Posted at: 2016-08-19T18:04:52.742Z Reads: 140

```
Still not working out for me :/  they aint touching :)
```

---
## \#15 Posted by: kaiser Posted at: 2016-08-19T18:07:56.877Z Reads: 141

```
Maby its the motor ? .. I am confused what is broken or not :/ (How to check that)
```

---
## \#16 Posted by: Jinra Posted at: 2016-08-19T18:17:25.947Z Reads: 139

```
does the can spin freely?
```

---
## \#17 Posted by: kaiser Posted at: 2016-08-19T18:19:35.466Z Reads: 138

```
Yes ,,

Whit only to phases going to the motor it did wiggle and now its the same again
```

---
## \#18 Posted by: kaiser Posted at: 2016-08-19T18:23:33.815Z Reads: 141

```
its saying same error when motor not plugged in :confused:
```

---
## \#19 Posted by: Jinra Posted at: 2016-08-19T18:24:32.934Z Reads: 153

```
try switching the 3 phase wires around and redetecting.
```

---
## \#20 Posted by: kaiser Posted at: 2016-08-19T18:25:37.449Z Reads: 155

```
tried that did not help only once there was a wiggle
```

---
## \#21 Posted by: Blasto Posted at: 2016-08-19T18:25:55.405Z Reads: 146

```
post pictures of your setup.
```

---
## \#22 Posted by: kaiser Posted at: 2016-08-19T18:36:42.672Z Reads: 150

```
<img src="/uploads/db1493/original/2X/a/ac64540ef2bf204a1362b844e927f2ee14f211c8.JPG" width="666" height="500"><img src="/uploads/db1493/original/2X/2/270678b24dd4a1d3a1f00d7e4f7cd1494d85c664.JPG" width="375" height="500"><img src="/uploads/db1493/original/2X/1/19adf5cab82912726ef00c0efc1cde761b572ab8.JPG" width="375" height="500">
```

---
## \#23 Posted by: kaiser Posted at: 2016-08-19T18:40:28.626Z Reads: 138

```
There are also a green light
```

---
## \#24 Posted by: kaiser Posted at: 2016-08-19T18:44:01.120Z Reads: 139

```
Does yours vesc blink red when not having a motor connected when pressing on the arrows when connected bldc tool ?
```

---
## \#25 Posted by: makevoid Posted at: 2016-08-19T19:44:27.848Z Reads: 141

```
look and take a picture where the motor cables go inside the motor, if they are not properly covered with heatshrink they may short and motor detection will fail, also you could measure the resistance between the cables (not sure which value you need to expect though)

if they are not properly insulated they could cause a failed motor detection and run poorly causing the motor to heat up, in that case see this thread with the solution (opening the motor and heatshrinking the wires)
http://www.electric-skateboard.builders/t/how-to-open-enertion-motor/6965/6
```

---
## \#26 Posted by: Blasto Posted at: 2016-08-19T22:44:43.674Z Reads: 140

```
Did you solder the bullets on the lead or is the wire just sitting in the cup of the bullet?

And heat shrink your leads...
```

---
## \#27 Posted by: kaiser Posted at: 2016-08-21T12:27:49.229Z Reads: 137

```
[quote="Blasto, post:26, topic:7910, full:true"]
Did you solder the bullets on the lead or is the wire just sitting in the cup of the bullet?

And heat shrink your leads...
[/quote]

<img src="/uploads/db1493/original/2X/4/43337de2588116cae8d1ef1770cebd86c5183d72.JPG" width="666" height="500"><img src="/uploads/db1493/original/2X/b/b528a1af316c12bbe76ae0aa045116ac443d7d0a.JPG" width="666" height="500"><img src="/uploads/db1493/original/2X/1/130e5dfba1f54764c8e675ba43db96cbf9635ac3.JPG" width="375" height="500">

I dont see any sign of anything :confused:
```

---
## \#28 Posted by: makevoid Posted at: 2016-08-21T12:52:59.673Z Reads: 134

```
Other side, cables side, you have to look through the openings in the motor and see if pushing the cables they're firm or not, all covered in black or not
```

---
## \#29 Posted by: kaiser Posted at: 2016-08-21T12:53:24.484Z Reads: 138

```
After resampling all parts i finally got an error when typing fault in the terminal , can u guys tell me what it says

..

The following faults were registered since start:

Fault            : FAULT_CODE_DRV8302
Current          : 0.2
Current filtered : -0.2
Voltage          : 27.39
Duty             : 0.01
RPM              : 0.1
Tacho            : 3
Cycles running   : 2
TIM duty         : 554
TIM val samp     : 297
TIM current samp : 24879
TIM top          : 49165
Comm step        : 1
Temperature      : 27.26

Fault            : FAULT_CODE_DRV8302
Current          : 0.2
Current filtered : 0.1
Voltage          : 27.42
Duty             : 0.02
RPM              : 0.1
Tacho            : 4
Cycles running   : 3
TIM duty         : 792
TIM val samp     : 421
TIM current samp : 23542
TIM top          : 46242
Comm step        : 2
Temperature      : 27.44

Fault            : FAULT_CODE_DRV8302
Current          : 0.0
Current filtered : 0.0
Voltage          : 27.44
Duty             : 0.02
RPM              : 2.0
Tacho            : 8
Cycles running   : 2
TIM duty         : 903
TIM val samp     : 10
TIM current samp : 26384
TIM top          : 52747
Comm step        : 6
Temperature      : 27.62

Fault            : FAULT_CODE_DRV8302
Current          : -0.2
Current filtered : 0.1
Voltage          : 27.41
Duty             : 0.01
RPM              : 2.0
Tacho            : 9
Cycles running   : 1
TIM duty         : 554
TIM val samp     : 297
TIM current samp : 24879
TIM top          : 49165
Comm step        : 1
Temperature      : 27.85

Fault            : FAULT_CODE_DRV8302
Current          : 0.2
Current filtered : 0.0
Voltage          : 27.42
Duty             : 0.02
RPM              : 1.9
Tacho            : 10
Cycles running   : 2
TIM duty         : 792
TIM val samp     : 451
TIM current samp : 23572
TIM top          : 46242
Comm step        : 2
Temperature      : 27.82

Fault            : FAULT_CODE_DRV8302
Current          : 0.2
Current filtered : 0.0
Voltage          : 27.39
Duty             : 0.02
RPM              : 2.0
Tacho            : 13
Cycles running   : 2
TIM duty         : 792
TIM val samp     : 421
TIM current samp : 23542
TIM top          : 46242
Comm step        : 5
Temperature      : 27.87

Fault            : FAULT_CODE_DRV8302
Current          : 0.9
Current filtered : 0.1
Voltage          : 27.42
Duty             : 0.00
RPM              : 3.0
Tacho            : 13
Cycles running   : 0
TIM duty         : 8
TIM val samp     : 420
TIM current samp : 2520
TIM top          : 4200
Comm step        : 1
Temperature      : 27.85

Fault            : FAULT_CODE_DRV8302
Current          : 0.2
Current filtered : -0.3
Voltage          : 27.41
Duty             : 0.02
RPM              : 41.5
Tacho            : 1158
Cycles running   : 2
TIM duty         : 792
TIM val samp     : 451
TIM current samp : 23572
TIM top          : 46242
Comm step        : 4
Temperature      : 28.55

Fault            : FAULT_CODE_DRV8302
Current          : 1.1
Current filtered : 0.4
Voltage          : 27.44
Duty             : 0.01
RPM              : 2.9
Tacho            : 1161
Cycles running   : 2
TIM duty         : 554
TIM val samp     : 297
TIM current samp : 24879
TIM top          : 49165
Comm step        : 1
Temperature      : 28.71

Fault            : FAULT_CODE_DRV8302
Current          : -0.5
Current filtered : 0.2
Voltage          : 27.42
Duty             : 0.02
RPM              : 3.9
Tacho            : 1162
Cycles running   : 4
TIM duty         : 965
TIM val samp     : 505
TIM current samp : 22558
TIM top          : 44106
Comm step        : 6
Temperature      : 28.58

Fault            : FAULT_CODE_DRV8302
Current          : -0.0
Current filtered : 0.0
Voltage          : 27.45
Duty             : 0.00
RPM              : 0.4
Tacho            : 1162
Cycles running   : 0
TIM duty         : 8
TIM val samp     : 420
TIM current samp : 2520
TIM top          : 4200
Comm step        : 6
Temperature      : 28.86

Fault            : FAULT_CODE_DRV8302
Current          : 1.3
Current filtered : 1.1
Voltage          : 27.42
Duty             : 0.00
RPM              : 0.1
Tacho            : 1162
Cycles running   : 0
TIM duty         : 7
TIM val samp     : 420
TIM current samp : 2520
TIM top          : 4200
Comm step        : 6
Temperature      : 29.18
```

---
## \#30 Posted by: kaiser Posted at: 2016-08-21T12:54:47.205Z Reads: 132

```
[quote="makevoid, post:28, topic:7910, full:true"]
Other side, cables side, you have to look through the openings in the motor and see if pushing the cables they're firm or not, all covered in black or not
[/quote]


Nothing is in black
```

---
## \#31 Posted by: kaiser Posted at: 2016-08-21T13:04:47.312Z Reads: 133

```
[quote="kaiser, post:29, topic:7910"]
FAULT_CODE_DRV8302
[/quote]


Does it mean i need to replace this chip?
https://www.youtube.com/watch?v=qeWzP2YahNc
```

---
## \#32 Posted by: kaiser Posted at: 2016-08-21T13:07:12.131Z Reads: 132

```
after plugging power off and on its now says
 No faults registered since startup

FAULT_CODE_NONE
```

---
## \#33 Posted by: kaiser Posted at: 2016-08-21T13:08:45.738Z Reads: 135

```
And after trying motor detect and the typing faults again it's says same error Fault            : FAULT_CODE_DRV8302
Current          : 0.1
Current filtered : 0.1
Voltage          : 27.38
Duty             : 0.02
RPM              : 0.2
Tacho            : 7
Cycles running   : 4
TIM duty         : 966
TIM val samp     : 483
TIM current samp : 22530
TIM top          : 44094
Comm step        : 1
Temperature      : 29.73

Fault            : FAULT_CODE_DRV8302
Current          : 0.1
Current filtered : 0.3
Voltage          : 27.38
Duty             : 0.02
RPM              : 0.2
Tacho            : 8
Cycles running   : 3
TIM duty         : 991
TIM val samp     : 523
TIM current samp : 22415
TIM top          : 43784
Comm step        : 2
Temperature      : 29.67
```

---
## \#34 Posted by: ikjahaa Posted at: 2016-08-21T13:28:13.900Z Reads: 120

```
What version of BLDC tool are you using ?
```

---
## \#35 Posted by: kaiser Posted at: 2016-08-21T13:38:24.842Z Reads: 120

```
I dont know :/ i can't download it again :/
```

---
## \#36 Posted by: ikjahaa Posted at: 2016-08-21T13:39:39.157Z Reads: 123

```
Go to the "Firmware" tab
```

---
## \#37 Posted by: kaiser Posted at: 2016-08-21T13:40:26.411Z Reads: 129

```
<img src="/uploads/db1493/original/2X/0/0e1e735a9535d2ab46702fe3c5cfe598038a5341.png" width="690" height="366">
```

---
## \#38 Posted by: ikjahaa Posted at: 2016-08-21T13:41:20.142Z Reads: 132

```
Try using version 2.15, also what vesc version do you have ?
EDIT: found it on your picture, 4.12. try downgrading your vesc firmware to 4.15 aswell.
```

---
## \#39 Posted by: kaiser Posted at: 2016-08-21T13:42:15.995Z Reads: 136

```
BLDC 15-Aug-2016

Vesc 4.12
```

---
## \#40 Posted by: ikjahaa Posted at: 2016-08-21T13:45:47.468Z Reads: 139

```
http://vesc.net.au/BLDC-TOOL/OS%20X/OLD%20Versions/

The firmware files should be in your install directory.
euhm... @jacobbloy has a video on how to change your vesc's firmware version i think...
```

---
## \#41 Posted by: ikjahaa Posted at: 2016-08-21T13:47:21.792Z Reads: 143

```
https://www.youtube.com/watch?v=JZSM_DmKx_Y
```

---
## \#42 Posted by: kaiser Posted at: 2016-08-21T13:50:41.839Z Reads: 145

```
is It safe to downgrade ? 

found it
Vesc motherboard 4.12 
bldc 2.15
Cant find the firmware u talk about?

<img src="/uploads/db1493/original/2X/8/819f62676d1e36f3c8878269444f4b6b9338339a.png" width="284" height="500">
```

---
## \#43 Posted by: ikjahaa Posted at: 2016-08-21T14:00:23.243Z Reads: 132

```
I'm using windows, mine are located in: **D:\Program Files (x86)\BLDC Tool 2_15\Drivers\firmwares\hw_410_411_412\VESC_default.bin**
```

---
## \#44 Posted by: ikjahaa Posted at: 2016-08-21T14:01:47.747Z Reads: 135

```
just follow the youtube video's instructions.
```

---
## \#45 Posted by: kaiser Posted at: 2016-08-21T14:04:57.683Z Reads: 135

```
ok i try this out now if u agree

Vesc motherboard 4.12 
bldc 2.15
firmwares 2.15 FOC.zip  

and this
D:\Program Files (x86)\BLDC Tool 2_15\Drivers\firmwares\hw_410_411_412\VESC_default.bin
```

---
## \#46 Posted by: ikjahaa Posted at: 2016-08-21T14:07:28.521Z Reads: 138

```
no, you don't need firmwares 2.15 FOC.
use the firmware file that came with the 2.15 bldc tool, you don't need to download extra files. Only the bldc 2.15 tool.
```

---
## \#47 Posted by: ikjahaa Posted at: 2016-08-21T14:08:46.330Z Reads: 136

```
I'm just reading.... 
http://www.electric-skateboard.builders/t/vesc-faq-firmware-bug-pre-august-2016-please-upgrade/8018?u=ikjahaa

perhaps you should update to that version instead. I might have to do it as well.
```

---
## \#48 Posted by: kaiser Posted at: 2016-08-21T14:10:31.852Z Reads: 137

```
the folder only had bldc tool when downloaded ?
<img src="/uploads/db1493/original/2X/d/d1bd3374b161dc0dbe30a4d9768c95db57f68f3c.png" width="441" height="499">
```

---
## \#49 Posted by: kaiser Posted at: 2016-08-21T14:11:21.505Z Reads: 128

```
What version is this he are talking about
```

---
## \#50 Posted by: ikjahaa Posted at: 2016-08-21T14:17:20.005Z Reads: 132

```
Not quite, sure the link isn't working for me.
lets just wait for a response..
```

---
## \#51 Posted by: kaiser Posted at: 2016-08-21T14:22:28.300Z Reads: 136

```
i think it this one 
if u see the date it was added the 15 aug

<img src="/uploads/db1493/original/2X/3/3443a2719774dfd1a8a79a36193b91b129f8e9ef.png" width="690" height="199">
```

---
## \#52 Posted by: ikjahaa Posted at: 2016-08-21T14:27:40.528Z Reads: 138

```
probably, yes.
```

---
## \#53 Posted by: kaiser Posted at: 2016-08-21T14:30:49.363Z Reads: 142

```
But that is my current version :/  and firm version also  because there was the firmware inside the downloaded folder
```

---
## \#54 Posted by: hugohammarstrom Posted at: 2016-08-21T19:06:11.803Z Reads: 136

```
If you still have the same settings as you had in the first picture posted you should try to lower the battery cutoff. At 7s this a way to high battery cutoff. 

Try lowering to:
Start: 7*3.3 = 23.1v 
End: 7*3.0 = 21v
```

---
## \#55 Posted by: Sunstart Posted at: 2016-09-16T03:26:07.622Z Reads: 126

```
Yo u saved me it works i was tring for 2 hours i got sk3 6364 245 running a 6s battery thx
```

---
## \#56 Posted by: backinblack626 Posted at: 2016-09-30T22:21:47.411Z Reads: 113

```
So I have two VESCs and both are failing motor detection with my motor. The motor just cogs forwards and backwards instead of smoothly in one direction like it should. I can get it to respond with the arrow keys but not properly. It just jerks back and forth. It will read R and L but not the flux linkage. No fault codes and settings have been pretty thoroughly checked I believe. I cannot for the life of me figure this out. Could it be a shorted wire inside the motor or insulation problem? Does anyone know if there is a tutorial on how to read and what to look for in live data that might give me some insight on what is going on? Both VESCs are 4.12 running 2.18 firmware. One I just received with 2.18 and the other just had the DRV chip replaced so I updated it to 2.18 in order to use the new BLDC tool.
```

---
## \#57 Posted by: Jinra Posted at: 2016-09-30T23:22:57.965Z Reads: 104

```
What are your battery cutoffs and battery?
```

---
## \#58 Posted by: backinblack626 Posted at: 2016-10-03T16:09:27.429Z Reads: 96

```
Using a 6S I set the cutoff start at 21v and cutoff end at 20v for safe discharge. Max voltage is 56v and min is 10v so those limits shouldn't interfere with anything since my LiPo has a full charge at just under 25v (24.7v).
```

---
## \#59 Posted by: Seaha Posted at: 2016-11-20T12:06:15.300Z Reads: 84

```
Hi dude. I am really new at e skateboarding. You have the same hardware like me. Can you please send me your configurations in bldc tool?
Mine didnt work. And you have same motor and same batteties like me.

Thank Mate
```

---
