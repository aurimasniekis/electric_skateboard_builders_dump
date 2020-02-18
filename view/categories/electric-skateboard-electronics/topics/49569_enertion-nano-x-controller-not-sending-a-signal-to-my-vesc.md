# Enertion Nano-X Controller not sending a signal to my VESC

### Replies: 9 Views: 412

## \#1 Posted by: isaacwwkelly Posted at: 2018-03-20T00:45:56.784Z Reads: 57

```
Hey guys, I was on BLDC Tool (trying to make the ramping on the VESC more gentle and the brakes less severe, and all of a sudden my Nano-X stopped sending a signal to the receiver. It binds to the receiver and the green LED on the controller is solid once it binds, but the motor won't spin when I throttle it (nor will it brake).
```

---
## \#2 Posted by: isaacwwkelly Posted at: 2018-03-20T00:50:50.132Z Reads: 55

```
![bldc screenshot1|690x369](upload://c1TyTrRXNuXFIUdK7bxutwoJXF7.png)

![bldc screenshot2|690x371](upload://h24b96UszPW4krZFjeO7D1voV2S.png)

These are screenshots of the BLDC tool
```

---
## \#3 Posted by: b264 Posted at: 2018-03-20T00:59:20.769Z Reads: 46

```
It's likely the signal is still being sent but it's not selected for use.  Every time you change screens in the BLDC tool you MUST click "read configuration" then before you leave that screen, "write configuration"


Go to the "App Configuration" tab and the "General" tab and see which Application it's using.  Change that to PPM + UART
```

---
## \#4 Posted by: Blasto Posted at: 2018-03-20T01:05:55.616Z Reads: 44

```
The vesc is not connected

![image|281x500](upload://9C6lk69idifQ8AEcTok247s4qPS.jpeg)
```

---
## \#5 Posted by: isaacwwkelly Posted at: 2018-03-20T01:17:12.612Z Reads: 38

```
I did that and the display in the PPM tab still doesn't move when I throttle it, and the Pulsewidth is just showing 0.
```

---
## \#6 Posted by: isaacwwkelly Posted at: 2018-03-20T01:17:51.124Z Reads: 40

```
These screenshots were after I was using the Tool, same settings though.
```

---
## \#7 Posted by: Blasto Posted at: 2018-03-20T01:19:07.370Z Reads: 41

```
But by disconnecting, you don’t see if the receiver is actually sending a signal. Take the same screenshot but with everything connected
```

---
## \#8 Posted by: isaacwwkelly Posted at: 2018-03-20T01:21:15.405Z Reads: 41

```
![bldc screenshot3|690x370](upload://7ZKC3eJq4XJO3fXhJTzb3t13wOc.png)
This is while it is connected and the nano-x controller is binded
```

---
## \#9 Posted by: isaacwwkelly Posted at: 2018-03-20T01:23:02.498Z Reads: 37

```
Ok I just set it to PPM, wrote config, and rebooted and it works again! Now to ramping the acceleration and brakes so I don't die on this board.

Thanks Guys!
```

---
