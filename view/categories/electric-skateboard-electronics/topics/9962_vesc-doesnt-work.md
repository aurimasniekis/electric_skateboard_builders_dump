# VESC doesnt work

### Replies: 7 Views: 1632

## \#1 Posted by: rasmukri Posted at: 2016-09-22T01:28:22.672Z Reads: 184

```
Yeah yeah another VESC inop thread but nobody has posted shit about this one.
Just got my VESC yesterday and am trying to get it programed and that's where the trouble started.
when i connect my VESC to windows i get the du du du sound and when i open BLDC tool i click connect and it says connected for about 2 seconds before going to "NO FIRMWARE READ RESPONSE" then disconnected.
When i open device manager it shows uninstalled device ChibiOS/RT Virtual COM Port   WTF?! is this shit? and how do i find a driver for it? Because that is the VESC it comes and goes when i plug and unplug the controller.
The VESC just sits around with both a red and blue light both on at the same time while its connected, no blinking after the initial boot.
I have the new firmware ready to install but the damn thing wont connect long enough for me to install it. Just goes to buffer erase timeout because the damn thing is not connected apparently.
I have tried uninstalling the BLDC tool and reinstalling it with various power cycling of the computer attempts as well.
```

---
## \#2 Posted by: chaka Posted at: 2016-09-22T01:52:36.472Z Reads: 180

```
If you are using something other than a linux/ubuntu OS you may have an issue with the usb port id. Seems strange that the red led is on constantly??? If you purchased this from us, "OllinBoardCo", we will take care of whatever issues you seem to be having. If not then hopefully it is just a port id issue.

Try finding the port id and entering it into the bldc-tool before connecting. Could also be a bad usb cable or usb port.
```

---
## \#3 Posted by: rpn314 Posted at: 2016-09-22T02:15:27.681Z Reads: 168

```
Bootloader issue? I don't remember if that's what mine did before I flashed the bootloader
```

---
## \#4 Posted by: rasmukri Posted at: 2016-09-22T23:18:50.350Z Reads: 135

```
so after extensive google searches for this thing I found some random driver, so of course I installed it and bam it worked. Not too sure why windows couldn't find any drivers but whatever it is all hooked up and I took my first test drive this morning.
```

---
## \#5 Posted by: sl33py Posted at: 2016-09-22T23:38:09.993Z Reads: 131

```
i've seen a lot of USB 3.0 driver issues - a lot of the time just plugging into another slower USB 2.0 port seems to fix.
```

---
## \#6 Posted by: ARollNation Posted at: 2017-01-07T01:59:45.846Z Reads: 98

```
Do you know where you found that driver?? Im having the same issue
```

---
## \#7 Posted by: jaykup Posted at: 2017-02-19T04:34:29.596Z Reads: 74

```
This worked for me - 

https://www.pjrc.com/teensy/td_download.html

During install it checks for the USB driver and installs it if needed (was needed for me). Then you can cancel the full setup after the driver install.
```

---
