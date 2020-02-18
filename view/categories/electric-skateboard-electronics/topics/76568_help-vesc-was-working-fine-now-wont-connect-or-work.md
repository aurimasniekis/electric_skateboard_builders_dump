# HELP: VESC was working fine, now wont connect or work!

### Replies: 41 Views: 455

## \#1 Posted by: AdamE3399 Posted at: 2018-11-30T01:39:40.258Z Reads: 98

```
So I recently made my new board and everything was working fine, I set my vesc settings in vesc tool, set one and slave and the other as master and connected them and set the appropriate settings: motor max: 60 amps min -40 Bat max: 30 min: -20, the battery cutoff, set the max erpm to 60000 and -60000, took it for a ride and everything was working perfectly, got home unplugged the loop key and came back to it 5 mins later plugged loop key back in and remote wouldn't connected so I opened the board and plugged in the vesc and now it isn't connecting to the computer, either of them! I tried using different cables unplugging and plugging back in but I wont connect to the pc, please help.

My boards specs:
dual flipsky vesc 4.12
dual sk3 6364 190kvs
5ah Turnigy 25c lipo
```

---
## \#2 Posted by: AdamE3399 Posted at: 2018-11-30T01:41:09.387Z Reads: 90

```
Any ideads @dareno or @Winfly? Help would be appreciated
```

---
## \#3 Posted by: dareno Posted at: 2018-11-30T01:43:00.346Z Reads: 89

```
Who dares summon me?  


Whats the lights on the vesc telling you?
```

---
## \#4 Posted by: Winfly Posted at: 2018-11-30T01:49:19.454Z Reads: 81

```
Do the led turns on at all? And is there a red led lit up ( red is fault)?
```

---
## \#5 Posted by: AdamE3399 Posted at: 2018-11-30T01:52:22.525Z Reads: 81

```
there is a blue and a green light lit
```

---
## \#6 Posted by: Winfly Posted at: 2018-11-30T01:59:23.158Z Reads: 78

```
Well that means the VESC still turns on. Do you have a 4.20 dual or 2 singles?
```

---
## \#7 Posted by: AdamE3399 Posted at: 2018-11-30T02:00:36.304Z Reads: 80

```
2 singles over can-bus
```

---
## \#8 Posted by: mynamesmatt Posted at: 2018-11-30T02:08:50.819Z Reads: 76

```
if you switch it off, disconnect canbus and just power one vesc up with the receiver, does it then work?
```

---
## \#9 Posted by: mynamesmatt Posted at: 2018-11-30T02:09:20.220Z Reads: 77

```
also type fault into the terminal of each vesc and post the results
```

---
## \#10 Posted by: AdamE3399 Posted at: 2018-11-30T02:12:25.606Z Reads: 78

```
the power cables are wired together so I cant only power one but I disconnected them from canbus and tried one but it still wont connect, and I cant check terminal for faults because they wont connect.
```

---
## \#11 Posted by: mynamesmatt Posted at: 2018-11-30T02:13:08.509Z Reads: 78

```
welp, i tried i got nutting
```

---
## \#12 Posted by: AdamE3399 Posted at: 2018-11-30T02:13:51.422Z Reads: 80

```
I just don't understand because they were just working
```

---
## \#13 Posted by: Winfly Posted at: 2018-11-30T02:15:22.439Z Reads: 80

```
Could be that either you USB cable is broken. Or the USB port is broken. Try wiggle the USB port to see if you get connection at some angle.
```

---
## \#14 Posted by: AdamE3399 Posted at: 2018-11-30T02:16:47.349Z Reads: 75

```
tried multiple cables, on multiple ports, across multiple computers
```

---
## \#15 Posted by: AdamE3399 Posted at: 2018-11-30T02:44:14.073Z Reads: 85

```
@Winfly @mynamesmatt now when I try to connect it, it says nor firmware read version even though it had firmware when I edited settings before. How can firmware just disappear?
```

---
## \#16 Posted by: AdamE3399 Posted at: 2018-11-30T02:46:21.800Z Reads: 86

```
Heres is the code from console when it connected:

2018-11-30 11:04:05: VESC® Tool 0.94 started
2018-11-30 11:04:05: Status: Not connected
2018-11-30 11:07:37: Status: Connected (serial) to COM3
2018-11-30 11:07:37: Status: VESC Firmware Version 3.38, Hardware: 410, UUID: 3A 00 28 00 02 50 48 47 50 34 37 20
2018-11-30 11:07:38: Status: MC configuration updated
2018-11-30 11:07:38: Status: App configuration updated
2018-11-30 11:08:08: Status: MCCONF Write OK
2018-11-30 11:08:08: Status: MC configuration updated
2018-11-30 11:08:09: Status: APPCONF Write OK
2018-11-30 11:08:17: Status: Serial port error: The I/O operation has been aborted because of either a thread exit or an application request.
2018-11-30 11:08:20: Status: Not connected
2018-11-30 11:08:40: Status: Connected (serial) to COM3
2018-11-30 11:08:40: Status: VESC Firmware Version 3.38, Hardware: 410, UUID: 3B 00 26 00 02 50 48 47 50 34 37 20
2018-11-30 11:08:48: Status: MCCONF Write OK
2018-11-30 11:08:48: Status: MC configuration updated
2018-11-30 11:08:49: Status: APPCONF Write OK
2018-11-30 11:08:54: Status: Serial port error: The I/O operation has been aborted because of either a thread exit or an application request.
2018-11-30 11:08:57: Status: Not connected
2018-11-30 11:11:12: Status: Connected (serial) to COM3
2018-11-30 11:11:15: Status: No firmware read response
2018-11-30 11:11:18: Status: Not connected
2018-11-30 11:11:20: Status: Connected (serial) to COM3
2018-11-30 11:11:23: Status: No firmware read response
2018-11-30 11:11:26: Status: Not connected
2018-11-30 11:11:38: Status: Connected (serial) to COM3
2018-11-30 11:11:38: Status: Connected (serial) to COM1
2018-11-30 11:11:39: Status: Not connected
2018-11-30 11:11:54: Status: Connected (serial) to COM1
2018-11-30 11:11:58: Status: No firmware read response
2018-11-30 11:12:00: Status: Not connected
2018-11-30 11:12:35: Status: Connected (serial) to COM1
2018-11-30 11:12:38: Status: No firmware read response
2018-11-30 12:11:16: Status: Not connected
2018-11-30 12:11:17: Status: Connected (serial) to COM1
2018-11-30 12:11:21: Status: No firmware read response
2018-11-30 12:11:25: Status: Not connected
2018-11-30 12:13:03: Status: Connected (serial) to COM1
2018-11-30 12:13:06: Status: No firmware read response
2018-11-30 12:13:10: Status: Not connected
2018-11-30 12:16:15: Status: Connected (serial) to COM1
2018-11-30 12:16:18: Status: No firmware read response
2018-11-30 12:42:55: Status: Not connected
2018-11-30 12:42:58: Status: Connected (serial) to COM1
2018-11-30 12:43:01: Status: No firmware read response
2018-11-30 12:43:04: Status: Not connected


As you can see it connected fine and had firmware, I updated the settings , went for a ride and when I came bag and plugged it in, nothing
```

---
## \#17 Posted by: AdamE3399 Posted at: 2018-11-30T03:16:05.112Z Reads: 73

```
Does anyone know what this codes means? @dareno @Winfly
```

---
## \#18 Posted by: Winfly Posted at: 2018-11-30T03:24:49.117Z Reads: 72

```
@JohnnyMeduse
```

---
## \#19 Posted by: dareno Posted at: 2018-11-30T03:25:58.920Z Reads: 74

```
Nice dodge.  I have no clue.
```

---
## \#20 Posted by: JohnnyMeduse Posted at: 2018-11-30T03:30:47.826Z Reads: 76

```
@AdamE3399 Can you still see if the device connects to the PC?
```

---
## \#21 Posted by: AdamE3399 Posted at: 2018-11-30T03:32:04.939Z Reads: 76

```
the pc does not recognize the device when I plug it in
```

---
## \#22 Posted by: JohnnyMeduse Posted at: 2018-11-30T03:35:30.968Z Reads: 77

```
Humm.. could be a corrupted firmware of bootloader, if so you need to program it manually with an st-link.
```

---
## \#23 Posted by: AdamE3399 Posted at: 2018-11-30T03:35:47.189Z Reads: 76

```
how do I do that?
```

---
## \#24 Posted by: JohnnyMeduse Posted at: 2018-11-30T03:37:09.791Z Reads: 75

```
You probably didn't do anything, I've seen some issue like this with this firmware. What is your VESC (sorry I did not read the hole thread)
```

---
## \#25 Posted by: AdamE3399 Posted at: 2018-11-30T03:37:38.880Z Reads: 74

```
its a flipsky 4.12 vesc, 2 of them
```

---
## \#26 Posted by: JohnnyMeduse Posted at: 2018-11-30T03:41:54.668Z Reads: 73

```
Are the 2 doing the same thing?
```

---
## \#27 Posted by: AdamE3399 Posted at: 2018-11-30T03:43:38.768Z Reads: 71

```
yes they are and they were connected over can bus
```

---
## \#28 Posted by: AdamE3399 Posted at: 2018-11-30T03:44:07.831Z Reads: 72

```
After I did get them to connect vesc tool said it could not read firmware, is it possible the firmware was working and now isn't?
```

---
## \#29 Posted by: JohnnyMeduse Posted at: 2018-11-30T03:46:06.242Z Reads: 73

```
[quote="AdamE3399, post:27, topic:76568, full:true"]
yes they are and they were connected over can bus
[/quote]

Can you see some ligh when you power them ?
```

---
## \#30 Posted by: AdamE3399 Posted at: 2018-11-30T03:46:32.545Z Reads: 72

```
there is a green and a blue light
```

---
## \#31 Posted by: JohnnyMeduse Posted at: 2018-11-30T03:47:46.778Z Reads: 72

```
Try to disconect the can... then plug usb each one into the computer (I don't if it is possible) and check if at least they are reconize
```

---
## \#32 Posted by: AdamE3399 Posted at: 2018-11-30T03:50:03.846Z Reads: 70

```
I already did connect the can bus and tried that, but it stills says cannot read firmware
```

---
## \#33 Posted by: AdamE3399 Posted at: 2018-11-30T03:50:46.798Z Reads: 71

```
Cannot read firmware version, it says
```

---
## \#34 Posted by: JohnnyMeduse Posted at: 2018-11-30T03:51:33.025Z Reads: 70

```
Hummm... Really look like a corrupt firmware...
```

---
## \#35 Posted by: AdamE3399 Posted at: 2018-11-30T03:51:56.855Z Reads: 67

```
can I reinstall firmware with this: https://core-electronics.com.au/st-link-stm8-stm32-v2-programmer-emulator.html?utm_source=google_shopping&gclid=Cj0KCQiAuf7fBRD7ARIsACqb8w7qMpX1RHZhqiZf73OYv6xvBC4OYVsA7RvdI22x77R9lu11Kk23HMUaAq2VEALw_wcB
```

---
## \#36 Posted by: JohnnyMeduse Posted at: 2018-11-30T03:53:33.575Z Reads: 64

```
Yes it should work
```

---
## \#37 Posted by: AdamE3399 Posted at: 2018-11-30T03:53:57.055Z Reads: 65

```
ok ill get it now , thanks for your help
```

---
## \#38 Posted by: JohnnyMeduse Posted at: 2018-11-30T03:54:53.544Z Reads: 66

```
No problem. It is always a pleasure.
```

---
## \#39 Posted by: suntorytime Posted at: 2018-11-30T14:05:25.156Z Reads: 60

```
It's a long-shot, but try this:
Assuming you are using a Windows machine, disconnect the USB to your VESC, open the Device Manager and expand the Ports sub-menu. Note what current COM port is listed (if any). Now connect your VESC and observe if a new COM port is added in the Device Manager. If a new port is added, right-click on that port and select "Uninstall device" and also select "Delete the driver software". Go to the top menu of the Device Manager and click Action, "Scan for hardware changes". Your VESC's COM port should be re-detected and added to the Ports sub-menu. Right click on the newly added COM port (it may have a yellow exclamation next to it), then select Update Driver, "Search automatically for updated driver software". Once the driver has been updated for your VESC's COM port and status looks normal, go into the VESC tool, select the COM port that matches what you saw in Device Manager, then connect. Post the latest output that you get from VESC terminal.
```

---
## \#40 Posted by: brenternet Posted at: 2018-11-30T14:15:19.790Z Reads: 58

```
Also try turning your pc off, connecting the usb and starting it up while connected. I had a 6.6 that would only read doing that.
```

---
## \#41 Posted by: AdamE3399 Posted at: 2018-12-02T11:56:42.856Z Reads: 45

```
Thank you! @suntorytime you fixed it!
```

---
