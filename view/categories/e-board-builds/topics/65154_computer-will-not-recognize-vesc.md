# Computer will not recognize VESC

### Replies: 12 Views: 281

## \#1 Posted by: jerry9800 Posted at: 2018-08-17T06:17:13.274Z Reads: 91

```
Hello Esk8 community!

This is my first build and i'm running into a problem. The computer will not recognize my VESC. I have tried two cables so far and used it on a different computer with no luck.

Here is my set up
102sp battery(ownboard) connected to mboard power switch IN side via 12 awg wire with xt 60 connectors. Power switch is connected to torqueboard vesc via xt60 connectors. VESC connected to motor. It does power on. The power switch glows blue and the vesc flashes 3 blue lights

Any help would be appreciated as i really want to ride!

Thanks Guys!
```

---
## \#2 Posted by: myreala Posted at: 2018-08-17T07:09:18.402Z Reads: 80

```
When this happened to me it was the usb cable. Some cables are charge only and data lines are not connected, those will not work. I would just recommend trying different cables.
```

---
## \#3 Posted by: L3chef Posted at: 2018-08-17T07:13:12.666Z Reads: 73

```
Probably usb cable or drivers
```

---
## \#4 Posted by: Andy87 Posted at: 2018-08-17T07:15:41.341Z Reads: 74

```
Look in your windows settings, maybe it’s just not auto detect or the drivers not installed
```

---
## \#5 Posted by: paul1 Posted at: 2018-08-17T08:21:05.702Z Reads: 69

```
i had the same problem after a bumpy ride i thought the usb cable had come loose so i tried another and it worked so i dont know what happened to the cable supplied with the vesk maybe the fragile connectors got bent or something with  the vibrations.
anyway try another cable see if that works.
```

---
## \#6 Posted by: jerry9800 Posted at: 2018-08-18T02:59:11.324Z Reads: 55

```
Hey guys,

I bought a new cable and still my computer does not recognize it. i also made sure the cable is able to transfer data. I also installed the stm32 driver. I don't know if i installed it right.. but do you guys have any links/tutorals for installing the correct driver? 

Thanks guys
```

---
## \#7 Posted by: mccloed Posted at: 2018-08-18T04:19:46.753Z Reads: 50

```
Windows 10?
```

---
## \#8 Posted by: jerry9800 Posted at: 2018-08-18T14:15:57.684Z Reads: 40

```
Yes, i'm using windows 10. also tried it on mac and no luck either.
```

---
## \#9 Posted by: Andy87 Posted at: 2018-08-18T14:19:23.006Z Reads: 40

```
Maybe your micro usb broken on the vesc.
If I understood right there is a way to connect to your vesc via uart port, but for this you need a stl link
```

---
## \#10 Posted by: Andy87 Posted at: 2018-08-18T17:43:20.624Z Reads: 38

```
You could also connect via Bluetooth and set up your vesc with the vesc app.
For this you need a Bluetooth modul, but a Bluetooth module is never a bad idea to have.
```

---
## \#11 Posted by: jerry9800 Posted at: 2018-08-18T18:37:36.527Z Reads: 31

```
a Bluetooth module would work with the diyelectricskateboard vesc? 

collections/esc-speed-controller/products/torque-esc-bldc-electronic-speed-controller
```

---
## \#12 Posted by: Andy87 Posted at: 2018-08-18T19:38:30.869Z Reads: 27

```
Yes why not. You have one plug for CAN, one for sensor wires, one for your receiver and one for UART. The UART is where you connect your Bluetooth module.
```

---
