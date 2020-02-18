# Focbox, Firmware, and BLDC

### Replies: 22 Views: 2189

## \#1 Posted by: sprocket12 Posted at: 2018-04-08T02:50:19.250Z Reads: 275

```
I've been away for a while waiting on new hardware.  Got a Focbox and had a couple of questions that I haven't found answers to. 

1. What rev is the firmware and where can I download it?
2. Does Ackmaniac's firmware work?  I noticed that the bluetooth was stopping motor/remote detection???
3. Does the new BLDC-Tool support the Focbox?
4. The current BLDC tool says it is HW 4.8, really?

Thanks
```

---
## \#2 Posted by: Deckoz Posted at: 2018-04-08T02:55:08.642Z Reads: 266

```
If you have a focbox it should be reading as 4.12 hardware.

The latest ack firmware is 3.100
http://www.electric-skateboard.builders/t/extended-ackmaniac-esc-tool-based-on-vesc-tool/35116
```

---
## \#3 Posted by: sprocket12 Posted at: 2018-04-08T03:04:34.345Z Reads: 246

```
Thanks @Deckoz.  I found that out the hard way.  I inadvertently loaded 4.8 firmware.  I blown like 8 fuses trying to diagnose.  Just got it figured out when you posted.

Where do I find 3.100 firmware?  Is this Ack's?  I can only find 2.54 which messes with my remote somehow.
```

---
## \#4 Posted by: RedEagle Posted at: 2018-04-08T04:56:25.734Z Reads: 224

```
Here you go

https://www.dropbox.com/sh/t7dl90owz5ccbyl/AAANyC-yQCMeveA7errNRnYqa?dl=0
```

---
## \#5 Posted by: sprocket12 Posted at: 2018-04-08T16:00:24.932Z Reads: 198

```
Thanks @RedEagle.  I've downloaded it but don't seem to see any firmware in the files.  Am I missing something?
```

---
## \#6 Posted by: Exiledd_Top Posted at: 2018-04-08T16:11:00.283Z Reads: 187

```
You click on public files then into bldc folder and u will realize that there's 3 bldcs for 3 different  OS and then the last one is the firmware mod
```

---
## \#7 Posted by: RedEagle Posted at: 2018-04-08T16:11:07.441Z Reads: 184

```
Download the bldc tool and update the firmware on your vesc. The firmware comes bundled in the bldc tool.
```

---
## \#8 Posted by: Exiledd_Top Posted at: 2018-04-08T16:11:43.810Z Reads: 174

```
I didn't know that lol wat  for me I had to Download the mod separately
```

---
## \#9 Posted by: RedEagle Posted at: 2018-04-08T16:12:50.378Z Reads: 167

```
The 2.54 one? Or 3.1?
```

---
## \#10 Posted by: Exiledd_Top Posted at: 2018-04-08T16:13:52.297Z Reads: 164

```
Before 3.1 came out
```

---
## \#11 Posted by: Acidfie Posted at: 2018-04-08T16:14:55.060Z Reads: 161

```
when updating firmware, has the canbus connection to be unplugged?
```

---
## \#12 Posted by: RedEagle Posted at: 2018-04-08T16:20:18.348Z Reads: 157

```
I think it's possible with can bus connected. Nonetheless, I would unplug it just to be safe.
```

---
## \#13 Posted by: Acidfie Posted at: 2018-04-08T16:24:49.868Z Reads: 159

```
i just cant find the post i was looking for, there is a possibility to fry your DRV/CAN Chips when using CANBUS and the cable is not connected, was it when powering on the vescs not at the same time?

want to update but do not really know right now how to. just unplug can bus cable and do it for every vesc?
```

---
## \#14 Posted by: trancejunkiexxl Posted at: 2018-04-08T16:27:12.802Z Reads: 154

```
I'd update the vesc individually honestly to be safe
```

---
## \#15 Posted by: RedEagle Posted at: 2018-04-08T16:29:30.745Z Reads: 153

```
If you don't power on the vescs simultaneously there will be a voltage difference and one can bus will  leech power from the other. That'll result in a fried can chip and possibly drv too.

[quote="Acidfie, post:13, topic:51539"]
just unplug can bus cable and do it for every vesc?
[/quote]

Yes
```

---
## \#16 Posted by: sprocket12 Posted at: 2018-04-08T21:22:52.175Z Reads: 143

```
Interesting.  I've got the 3.1 firmware loaded but my motor now fails on detection.  It does turn while attempting to figure things out.  This worked on 2.18.  Any thoughts?
```

---
## \#17 Posted by: RedEagle Posted at: 2018-04-08T21:37:36.194Z Reads: 139

```
What vesc & motor are you using? BLDC? FOC? Is there *any* load connected to the shaft?(belt, pulleys)
```

---
## \#18 Posted by: Mobutusan Posted at: 2018-04-08T21:47:22.664Z Reads: 142

```
Make sure you choose the correct VESC hardware version for the firmware. Click on thread below.

https://www.electric-skateboard.builders/t/after-vesc-firmware-update-motors-not-detected/39960/21?u=mobutusan
```

---
## \#19 Posted by: sprocket12 Posted at: 2018-04-08T23:15:49.625Z Reads: 134

```
I'm running:

-Focbox 4.12, firmware 3.1
-Sk3 6364 245kv
-8s4p battery
-Configured via BLDC with NO load
```

---
## \#20 Posted by: Deckoz Posted at: 2018-04-09T00:59:20.399Z Reads: 133

```
I if you ran the motor while firmware for hardware 4.8 was flashed, something is likely dead.
```

---
## \#21 Posted by: sprocket12 Posted at: 2018-04-10T12:55:03.939Z Reads: 113

```
I have an inline fuse to protect the VESC. This proved true. 

I went ahead and re-flashed firmware 2.54 and used the older BLDC tool. The motor detection worked fine along with all my other settings.  

I'll read up on the differences in firmware to see what I gain going to 3.1. Perhaps the firmware upload didn't quite take the previous attempt.
```

---
## \#22 Posted by: frankus Posted at: 2019-01-22T17:47:37.703Z Reads: 51

```
I'm having trouble receiving values from the VESC. I'm able to send commands (I know this because the motor spins up when I do), but the data I receive back on the RX line is inevitably a 3 followed by 63 zeroes for all packets. I'm hoping this rings a bell for someone. 

I'm using an "Explore M3" board, which is an Arduino-compatible ARM Cortex M3 thing, using the Serial1 port for VESC communications and Serial (USB) for debugging. VESC Hardware version is 4.12, and firmware is 3.40. The App is set to UART and I've verified that the baud rate for both the VESC and Arduino is 115200.
```

---
