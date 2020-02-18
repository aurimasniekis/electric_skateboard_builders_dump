# Is there a log of Firmware versions somewhere?

### Replies: 5 Views: 508

## \#1 Posted by: evoheyax Posted at: 2017-12-27T17:53:38.349Z Reads: 87

```
Working on the VESC Status iphone app again, and I'm trying to support as many firmwares as possible. 

Does anyone know of a list of firmwares somewheres? Didn't see anything on vedders new site, or on here. I don't even know what version is in the github right now... lol.
```

---
## \#2 Posted by: Deckoz Posted at: 2017-12-27T17:56:45.280Z Reads: 85

```
Vedder BLDC tool 2.18(past two years)
Ackmaniac BLDC tool 2.54

VESC tool 3.xx (3.19-3.37 currently I think)
Ackmaniac VESC tool 3.100
```

---
## \#3 Posted by: evoheyax Posted at: 2017-12-27T18:05:25.061Z Reads: 82

```
Thank you so much. Weird thing is when I go through the the github, I see a lot of FW: 3.7 and FW: 3.9 even as comments to commits (https://github.com/vedderb/bldc). Maybe he hasn't released it ye, idk...

Do you know if @Ackmaniac released the firmware source code for 3.10? I see the package installer for mac and windows, but not the source code (like for 2.54). Trying to combine all of the data types first so the datatypes.h file is what I'm after.
```

---
## \#4 Posted by: Deckoz Posted at: 2017-12-27T18:11:36.620Z Reads: 73

```
I'm not sure if he did or not.
```

---
## \#5 Posted by: ShutterShock Posted at: 2017-12-28T02:05:42.798Z Reads: 53

```
Idk if this is helpful or not but I just setup a FOCBOX on my second board with FOC, and when I updated the firmware in the latest VESCTool it gave me FW 3.34.

The tool itself says it supports 3.32, 3.33, 3.34.  If your firmware is older than that it just tells you  to upgrade and installs the latest, 3.34
```

---
