# DIY NRF Remote Personal Attempt

### Replies: 1 Views: 184

## \#1 Posted by: ZFreaky Posted at: 2018-08-15T22:38:07.974Z Reads: 67

```
Hey frendos,

I've been working on a remote solution for a while and I just wanna mention my projects existence <s>maybe get more twitch followers in the process</s>.

Anyway, in revision 2 I'm planning a designed board, but the current model works with stuff I have lying around, though slightly ergonomically and aesthetically cancerous to look at.

Current specs are that it uses a joystick board salvaged from a generic Wii nunchuck, an 18650 from a recycled drill battery at 2000 mah with a 1s bms, an overpowered power system that steps up to 9v, into the arduino nano for 5v, then a separate converter for the 3.3v line off the 9v line, and an OLED display that displays speed, remote battery voltage, and board voltage. Future tweaks include making the telemetry display more... graphical. I have been streaming the assembly process on [twitch](https://www.twitch.tv/zfreaky), and I'm archiving the streams so if ya'll wanna see the specifics, or follow to see more of what I do.

The receiver is also a nano+NRF combination that communicates over UART with the VESC through a level shifter, which the remote has too, to communicate with the nunchuck joystick.

Any comments or questions please ask!

![IMG_3271|375x500](upload://dueLIH5Hj69Ck0uzpGfQR6X7LxS.JPG)

![IMG_3273%5B1%5D|375x500](upload://j6kcPR2yDyibbURynPCpIYBLLZE.JPG)

![IMG_3274%5B1%5D|375x500](upload://uTThFU6fmvyb0FbDm9fy8RDtiEf.JPG)

![IMG_3275%5B1%5D|375x500](upload://vxqAwEriOCDbcMIrCYZBum7wowl.JPG)
```

---
