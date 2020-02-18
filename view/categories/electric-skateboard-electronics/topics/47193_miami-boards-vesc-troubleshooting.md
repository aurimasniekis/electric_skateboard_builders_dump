# Miami Boards Vesc - Troubleshooting

### Replies: 12 Views: 849

## \#1 Posted by: Stunamar Posted at: 2018-02-22T20:21:49.052Z Reads: 102

```

I have a VESC 4.12 from Miami Electric Boards however  I'm having some issues. I tried updating the firmware according to the VESC Tool and it loaded but crashed at the end and now when I power up it gives me a solid yellow led and won't connect to the tool via usb. I thought maybe I needed to flash the bootloader but the pin layout is different than the other Vesc's so I'm not sure which conncetions I need to make. If someone can tell me which pins to use and the wiring configuration it'd be appreciated. 


Thank you in advance,


Joe
```

---
## \#2 Posted by: RedEagle Posted at: 2018-02-22T20:48:11.197Z Reads: 93

```
You can try flashing the bootloader using vesc tool.
```

---
## \#3 Posted by: Stunamar Posted at: 2018-02-22T21:44:41.785Z Reads: 82

```
Is there a way I can do that if Vesc tool won't connect via usb?
```

---
## \#4 Posted by: banjaxxed Posted at: 2018-02-22T21:54:08.143Z Reads: 78

```
A stm can do it I think

http://www.electric-skateboard.builders/t/vesc-boot-loader-installation-tutorial/32103
```

---
## \#5 Posted by: RedEagle Posted at: 2018-02-22T22:07:53.222Z Reads: 70

```
If it won't connect via usb you can try another bldc tool. If that won't work your only option is stlink. Check the thread above. You can also do it with a raspberry pi if you have one.
```

---
## \#6 Posted by: Stunamar Posted at: 2018-02-23T00:03:23.417Z Reads: 65

```
Thank you for the info.. Just one more question.
Which set of pins do I use on this Vesc? The layout is different and without indication.

-Joe![IMG_0310|375x500](upload://kI6x5aXaoxdtpbRIGRnHRyMghwr.JPG)![IMG_0311|375x500](upload://2dmKWhSPH995qc7mQsu1MAyZxJG.JPG)![IMG_0312|375x500](upload://zI3I8AW6RUE7RmLLhClYrmulzdk.JPG)
```

---
## \#7 Posted by: RedEagle Posted at: 2018-02-23T00:27:07.884Z Reads: 54

```
Unfortunately I'm not much help with that. 
Use the search function. There's lots of info about this subject already here. 
I've had similar problems and I've seen posts detailing the pinout. It's just a matter of finding them.
```

---
## \#8 Posted by: ThermalM16 Posted at: 2018-02-23T18:11:26.986Z Reads: 41

```
![fa471b2f04a32bc5db1ffb4c97c0b72951e553fe|666x500](upload://dHbFnpiqwiB5pmNfr7BlCjGP4Cv.JPG)
```

---
## \#9 Posted by: Stunamar Posted at: 2018-02-23T20:37:17.992Z Reads: 33

```
Thank you for the help. 
What is the pin configuration for the st link?
I tried, starting from the left side, 3.3v, SWCLK, GND, SWDIO, RST however even with this configuration I'm still having difficulty connecting to the STLink Utility..

I'm at a loss with this and would greatly appreciate some help.

Thank you,
Joe
```

---
## \#10 Posted by: ThermalM16 Posted at: 2018-02-23T22:10:45.801Z Reads: 28

```
Here's a pic of what's written under the connector

![IMG_5908|374x500](upload://9sVKjuf5wLN3yyx0pUEZUc9Qhe3.jpg)
```

---
## \#11 Posted by: Stunamar Posted at: 2018-02-23T23:02:03.682Z Reads: 25

```
I tried that configuration without luck..
```

---
## \#12 Posted by: ThermalM16 Posted at: 2018-02-24T00:04:04.199Z Reads: 24

```
Hmm, that's an identical VESC, so those should match up. Unfortunately I do not have schematics for that one, so that's the best I can do right now. When you plug it in are you getting any lights to come on?
```

---
