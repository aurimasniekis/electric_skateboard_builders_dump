# VESC derivative will not establish com port connection

### Replies: 6 Views: 242

## \#1 Posted by: chuttney1 Posted at: 2018-06-18T06:59:00.373Z Reads: 78

```
So the situation is after posting two posts about the red led issue and the uploading of the firmware and boot-loader do I run into the issue of my derivative not being able to establish a com port. With a 12V battery connection, I have a solid blue light, no green led, and no red led errors going off. The firmware and boot-loader upload using the binary files in the "bldc-tool" folder from GitHub were a success with the STM32 ST-Link program. I know the green led turns on one the MCU is functioning correctly, but this is really something else if I can't get the STM32 chip to give me a com port. 

I run Windows 10 and it works with my old VESC HW4.7.
```

---
## \#2 Posted by: aethyr Posted at: 2018-06-20T01:46:12.977Z Reads: 57

```
Is anything else connected to the vesc? Try disconnecting everything except the battery. Also make sure your usb cable is not a phone/charge-only cable. I just made the mistake of using a charge-only cable and couldn't establish a connection. Swapped cables, and problem solved.
```

---
## \#3 Posted by: chuttney1 Posted at: 2018-06-20T02:17:51.240Z Reads: 54

```
[quote="aethyr, post:2, topic:59250"]
Is anything else connected to the vesc?
[/quote]

Only a 12V battery to verify MCU startup. Micro-USB cable is the type that comes with the Smartphone, but I believe most micro USB cables sold are the same. Are all 5 pins suppose to be present on the micro USB cable, itself? This not asking about USB-A connector which goes to the computer. I got two different micro-USB cables, one with 4 pins and one with 5 pins present. I just checked, the missing pin is number 4 which is in reference to the USB OTG function. VESC 6.X schematic doesn't use that pin on the port.

As for the green led, is it supposed to be present after starting up on VESC 6.X?
```

---
## \#4 Posted by: aethyr Posted at: 2018-06-20T04:49:26.008Z Reads: 41

```
My vesc 6 based ESCape has a green led after startup. Maybe 12V is too little? Try 24V?
```

---
## \#5 Posted by: chuttney1 Posted at: 2018-06-21T01:27:27.133Z Reads: 34

```
I'm sure 12V is enough to start the MCU because it only needs 1.8V for bare minimum operation and 3.3V for full operation of memory speed and I/O. That's more than enough for the buck converter on the DRV8301 chip to get the MCU working.
```

---
## \#6 Posted by: aethyr Posted at: 2018-06-21T07:18:39.075Z Reads: 23

```
I agree that 12V should be enough to power the DRV. However, I think the blue and green leds are status lights to indicate if everything is kosher. When I had shorted sensor wires on my motor, my ESCape was on, but the blue and green leds did not light up, indicating that while power was there, something was amiss. The moment I removed the sensor plug from the ESCape, the blue and green leds lit up and I was able to connect via usb.
```

---
