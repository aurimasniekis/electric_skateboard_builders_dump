# Serenity Remote (Feather mod)

### Replies: 3 Views: 332

## \#1 Posted by: BluPenguin Posted at: 2019-06-01T22:46:17.545Z Reads: 115

```
New thread for this thing to leave the Feather remote thread for troubleshooting that particular remote.

Update on the progress, attempting to use a single 18650 as the battery for less charging, more riding. First test print out of PLA for fitment, few things changed around, bar trigger added to be used as cruise control and/or deadman switch.

Current issues looking for input:
1. Location for power switch: originally on back of remote near the bottom, risk of possibly being pressed by palm while being held. Move to nose/tip of remote?
2. Location of feather board + 18650 makes micro USB charging port hard to access without making the remote weird to hold or some odd shape. Ribbon extension of some sort to move microUSB location to another (?) area?

Goal is to have this buildable with easy print + off the shelf parts without creating proprietary PCBs, not sure if good idea, seems doable currently.


![18650|456x500](upload://baNB89L2jePCYOVqSqj25yuCPJK.png) ![EwoNqyo|375x500](upload://bq2snVgh7JSnxSWwJEYa38xM9y0.jpeg) ![Nwbz8Vz|375x500](upload://3VcC4G9xsnWGJ2qJIezucNMq2YN.jpeg)
```

---
## \#2 Posted by: Yegmesh Posted at: 2019-09-24T15:20:38.737Z Reads: 41

```
Yo! Has there been any updates on this? did you ever get the remote working? also is there a 3d file that i can download?
```

---
## \#3 Posted by: BluPenguin Posted at: 2019-09-29T08:38:48.353Z Reads: 28

```
Sadly this was never completed. Unfortunately I have 0 experience with arduino programming and I did not find any help with modifying the feather code to accept dual hall sensors. So while all the parts fit in the actual printed shell, I have no idea if my hall sensor/magnet placements actually work properly or if any wiring traces etc might cause interference. I wish I could test it but without a forked firmware to go with it, it's just a shell for now. If someone is still willing to help me modify the feather version of the code, I will be more than happy to actually complete this, otherwise I'm hoping that maybe the open source board of the FOCBOX Pilot might be configured into this form factor and go from there.
```

---
