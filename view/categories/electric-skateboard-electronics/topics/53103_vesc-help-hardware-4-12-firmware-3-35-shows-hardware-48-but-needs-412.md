# VESC help - Hardware 4.12 Firmware 3.35 shows hardware 48 but needs 412

### Replies: 20 Views: 1384

## \#1 Posted by: moronicity Posted at: 2018-04-22T07:47:55.697Z Reads: 156

```
I am unable to get my vesc to update the firmware on my vesc. This is what the faults say on the VESC terminal
The following faults were registered since start:

Fault            : FAULT_CODE_OVER_TEMP_FET
Current          : -0.0
Current filtered : -0.0
Voltage          : 34.06
Duty             : -0.290
RPM              : -0.0
Tacho            : 4
Cycles running   : 0
TIM duty         : -2434
TIM val samp     : 2
TIM current samp : 4200
TIM top          : 8400
Comm step        : 0
Temperature      : 440.66
 

Any help would be great! Running out of things to try.
```

---
## \#2 Posted by: L3chef Posted at: 2018-04-22T09:06:51.007Z Reads: 139

```
4.8 and 4.12 are hardware versions..not firmware
```

---
## \#3 Posted by: moronicity Posted at: 2018-04-22T16:52:01.007Z Reads: 122

```
Thanks, do you have any ideas on how to fix this without a ST link?
```

---
## \#4 Posted by: L3chef Posted at: 2018-04-22T21:04:08.081Z Reads: 106

```
Well if you flashed the wrong firmware and run the motors afterward, yoi might have toasted the vesc already.

What hardware version is your vesc?
What firmware version is currently flashed on it?
```

---
## \#5 Posted by: moronicity Posted at: 2018-04-22T21:21:57.021Z Reads: 106

```
Hardware: v4.12
![37 PM|561x500](upload://iLhP9LNkdJfdBISXd4RTYoqOJQV.png)
Also it says hardware version 48 in the Vesc tool which im guessing needs to show 412
Firmware: 3.35

Also, thanks for responding quickly, I was hoping to finish my build today but this threw a nice big wrench into it.
```

---
## \#6 Posted by: b264 Posted at: 2018-04-22T21:24:14.210Z Reads: 101

```
Disconnect your motor ASAP before you fry the vesc, if it's not already.  You need HW 410, 411 or 412

As long as you don't run the motor you can recover from this without an ST-Link, I did it, but I don't remember how.
```

---
## \#7 Posted by: moronicity Posted at: 2018-04-22T21:31:10.382Z Reads: 101

```
The motors are not connected anymore but they were briefly last night but I didnt run anything or testing. Right now there is blue light and a green one showing. Also, when i try to upload a custom firmware it shows as if its uploading and then it disconnects but then, nothing happens and after a power cycle, it shows the same data as above. Running the BLDC tool, i see a message saying 

"The firmware on the connected VESC is too old. Please update it using a programmer." 
Also, tried using @Ackmaniac tool![16 PM|690x434](upload://vdRSqhPiOSVG6VlBtRyF6Ylg2vC.png)![11 PM|690x365](upload://xiLNMNmdHD8JXI0yMNSz2gRET2m.png)
```

---
## \#8 Posted by: moronicity Posted at: 2018-04-22T21:33:33.139Z Reads: 93

```
I also get responses back from the vesc terminal, which tells me it may not be fried yet.

pong

Firmware: 3.35
Hardware: 48
UUID: 3D 00 29 00 11 47 36 34 38 34 36 33
Permanent NRF found: No
```

---
## \#9 Posted by: CBom Posted at: 2018-10-26T18:08:18.510Z Reads: 59

```
Any update on the hw 48 problem? Ran into it as well.
```

---
## \#10 Posted by: Jansen Posted at: 2019-04-26T05:10:04.778Z Reads: 44

```
Dealing with this issue now, anyone know how to get the vesc (focbox) back to the right hardware version, I flashed ack's latest firmware but accidentally said it was 48 hardware and not 410, 411, 412 like I needed too, how can I flash back to this?n Any advice @Ackmaniac???
```

---
## \#11 Posted by: Andy87 Posted at: 2019-04-26T05:20:01.217Z Reads: 45

```
if you have one that is working right now you can install the lates firmware on that one and than connect the one with the wrong fw via can bus and upload the firmware.

if both are with wrong firmware than you you need a st v2 link.
search for it here an you will find more than enough information how to flash back the right firmware.
```

---
## \#12 Posted by: Excess Posted at: 2019-04-26T05:41:35.132Z Reads: 45

```

Here’s the quick instructions from Trampa for flashing via swd interconnect
If you have one working vesc as Andy said 

[quote="trampa, post:6, topic:89755, full:true"]
Interconnect two ESC via SWD (IO, CLK; GND). Do not interconnect VCC! Use short cables (6cm) Connect to the working ESC and go to the SWD PROG tab. You will get relevant FW listed, which you can select. Choose correct FW (e.g. 410,411,412 FW for Hw 4.12). Click Upload.
[/quote]

Edit: don’t spin up motors while connected via Swd (per trampa)
```

---
## \#13 Posted by: trampa Posted at: 2019-04-26T06:37:12.857Z Reads: 42

```
There is a custom file tab, which allows you to upload FW from file. Download the 410 411 412 FW from Benjamin Vedders Github, select it, upload it.
```

---
## \#14 Posted by: Jansen Posted at: 2019-04-26T17:28:24.319Z Reads: 36

```
[quote="trampa, post:13, topic:53103"]
Download the 410 411 412 FW from Benjamin Vedders Github
[/quote]

Ok cool, thanks @trampa / Frank, really appreciate it my man. Any chance you have a link directly to that FW on his Github? I can browse for it but not till later so figured I'd ask and see if you might have the time. Thanks either way!
```

---
## \#15 Posted by: trampa Posted at: 2019-04-26T17:30:57.636Z Reads: 34

```
https://github.com/vedderb/vesc_tool/tree/master/res/firmwares

It's the default.bin in the correct Hardware version folder.
```

---
## \#16 Posted by: Jansen Posted at: 2019-04-26T17:47:37.559Z Reads: 32

```
[quote="trampa, post:15, topic:53103"]
default.bin in the correct Hardware
[/quote]

Got it, ok. See it there, thanks so much Frank. Last question for now then just to make sure I do this correctly the first time around.... Do I need to find and d/l Benjamins VESC tool or can I still upload that firmware from his page to put on the VESC/Focbox I need to from Ackmaniacs VESC tool like I did prior? LMK when you have a minute and thanks again, really appreciate the help!
```

---
## \#17 Posted by: trampa Posted at: 2019-04-26T20:08:39.826Z Reads: 29

```
Use VESC-Tool, connect ESC, upload FW.
```

---
## \#18 Posted by: Jansen Posted at: 2019-04-26T21:08:15.368Z Reads: 27

```
That’s what I i was just wanting to confirm with you first, so use Vedders VESC tool and not @Ackmaniac  VESC tool like I did originally when I updated firmware the other day. Correct? Sorry for asking the same / similar question if your answer was already clear enough, just want to be certain I don’t brick my FOCBOX is all. Better safe than sorry at the end of the day though right....? Lol. Thanks again @trampa
```

---
## \#19 Posted by: Jansen Posted at: 2019-04-27T00:20:43.809Z Reads: 23

```
[quote="trampa, post:17, topic:53103, full:true"]
Use VESC-Tool, connect ESC, upload FW
[/quote]

Hey Frank, a lil help.... I d'l the .bin file for the default firmware I need in the appropriate hardware section (410,411,412) but it won't let me upload that firmware in the VESC tool and keeps trying to get me to open up the BLDC tool instead... any idea why it's doing that? I see the file is for the VESC tool but then when I hit upload firmware in the VESC tool after putting the d/l there it won't allow t.... I just want to go ride my new set up.... ugh. Please lmk what i'm doing wrong.... or am I supposed to do it through the BLDC tool then switch over to VESC tool after that....? @trampa
```

---
## \#20 Posted by: trampa Posted at: 2019-04-27T06:41:21.446Z Reads: 21

```
You can use the old Bldc-tool to upload that FW. Just don't try to configure the ESC via BLDC-Tool after upload.
```

---
