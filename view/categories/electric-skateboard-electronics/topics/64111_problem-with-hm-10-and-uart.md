# Problem with HM-10 and UART

### Replies: 14 Views: 521

## \#1 Posted by: Strassa Posted at: 2018-08-07T09:56:26.889Z Reads: 133

```
Hey fellow esk8er,

I recently bought an HM-10 that I want to use with @Ackmaniac APP to display realtime info but I cannot get it to work. My status is:
Phone with ESC Monitor is connected to the HM-10 Module, but no info is shown. Set Baudtrate to 9600 and PPM+UART and crossed TX and RX from HM-10 to VESC.
I used following pins of the 7 pin JST:   x-TX-RX-x-GND-x-5V 
I use a chinese copy of the HM-10 but since I can connect my phone to it, it doesn't seem to be the problem.

Thanks for helping :slight_smile:
```

---
## \#2 Posted by: Acido Posted at: 2018-08-07T10:38:57.972Z Reads: 123

```
Did you reverse the order of rx and tx pins
```

---
## \#3 Posted by: Strassa Posted at: 2018-08-07T10:50:30.414Z Reads: 122

```
tried both but still no data (APP claims: "ESC not connected" when i try to read faults)
```

---
## \#4 Posted by: rok Posted at: 2018-08-07T10:56:31.250Z Reads: 124

```
Which android version? Some experienced problems on OREO i think.
Are you sure you have UART+PPM enabled in vesc tool?
```

---
## \#5 Posted by: Acido Posted at: 2018-08-07T11:19:11.054Z Reads: 116

```
Have you installed ackmaniacs firmware?
```

---
## \#6 Posted by: Strassa Posted at: 2018-08-07T12:50:50.031Z Reads: 104

```
Real time data should work without Ackmaniac firmware, right? I tested it with my Xiaomi which has Android 7.1 and the same Problem occurs :frowning:
```

---
## \#7 Posted by: cryo Posted at: 2018-08-07T13:37:30.482Z Reads: 93

```
Have you turned your board off since you changed vesc settings? I had the same problem and restarting my board seemed to fix it.
```

---
## \#8 Posted by: Strassa Posted at: 2018-08-07T13:51:04.919Z Reads: 90

```
yes, restartet it multiple times :slight_smile: 
is there any way to check the uart connection?
```

---
## \#9 Posted by: AutoItKing Posted at: 2018-08-07T15:32:21.810Z Reads: 82

```
What firmware version are you running on your ESC?
```

---
## \#10 Posted by: Strassa Posted at: 2018-08-07T15:48:27.022Z Reads: 77

```
4.30 , the newest one I think :slight_smile:
edit: misstyped should be 3.40
```

---
## \#11 Posted by: AutoItKing Posted at: 2018-08-07T15:58:13.966Z Reads: 75

```
3.40? If so, BV made a change that breaks these apps. Options: downgrade if you have an older version of VESC Tool available, or wait until ackmaniac updates the app.
```

---
## \#12 Posted by: thisguyhere Posted at: 2018-08-07T16:43:28.126Z Reads: 78

```
does your bt module show up as BT05 when the app is scanning for devices?

mine does too, it just doesn't want to work.

this person changed baud rates and seems to be working.

https://www.electric-skateboard.builders/t/bluetooth-module-with-ackmaniacs-app/32220/49
```

---
## \#13 Posted by: RyuX Posted at: 2018-08-07T17:17:41.207Z Reads: 72

```
@thisguyhere 
Just as clarification - I have the metr.at bluetooth module (not the pro one). And it is recommended to have this running at 115200 bauds.. but good luck for all the other people getting theirs to work
```

---
## \#14 Posted by: Strassa Posted at: 2018-08-07T17:29:07.841Z Reads: 65

```
flashed the ackmaniac firmware, now it works flawlessly, big thanks to @AutoItKing
```

---
