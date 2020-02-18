# VESC 4.12 not connecting to pc

### Replies: 10 Views: 266

## \#1 Posted by: florr Posted at: 2019-07-04T19:04:23.400Z Reads: 40

```
Hello,

my VESC 4.12 suddenly stopped moving the motor mid driving.
All LED's are lighting up (without blinking) when the power is connected. It is not communicating over UART anymore. 
Furthermore, the connection to the VESC tool is not working (tried different cables and different PC's). (Device is not found)
I do not see any visual damage to the components.

Any ideas? Is it broken?


![IMG_20190704_203642|375x499](upload://ooaid4VWiQK88YOLr6ylaeT0jou.jpeg)
```

---
## \#2 Posted by: Sn4pz Posted at: 2019-07-04T19:31:36.178Z Reads: 33

```
1) Post more / better photos of the vesc

2) You said all LEDs light up, but I assume you mean they're red... Right? 

3) What were you doing before it stopped? An honest answer is required for an accurate diagnosis 🤔
```

---
## \#3 Posted by: florr Posted at: 2019-07-04T19:46:33.126Z Reads: 32

```
1) More images: https://photos.app.goo.gl/eou46LxmSoXtsPMw9
Unfortunately, the focus of my camera is limiting the image quality..
I've checked like 100 times, if the cables soldered to the UART ports have a shortage - they don't.

2) There are three LEDs on my VESC: Blue, Green and Red - all of them light up

3) Well... I've used my board on rough terrain - but without me driving on it. Due to the low friction, it only went at about 5km/h for a few meters. Then it stopped working. So the vibration are responsible?
```

---
## \#4 Posted by: Sn4pz Posted at: 2019-07-04T20:51:20.595Z Reads: 30

```
Well I'm no expert, but that negative ( black) wire seems to be connected via solder to another component... Which all of my previous 4.xx vescs havnt had 🤔 

What happens when you plug the vesc into your PC and go to device manager? Any signs of life?

The vesc might have just shorted itself out 🤷

Calling the wiz @JohnnyMeduse
```

---
## \#5 Posted by: florr Posted at: 2019-07-04T21:02:08.023Z Reads: 27

```
Yes, the black wire is connected via solder to another component - but they are connected via the PCB anyway (as far as i can tell)

The device is showing up - but with errors:

Unknown USB-device (Error on retrieving device description)

![DeviceManager|402x455](upload://lOyTeTWCQ0PIG2wsRQ8UdpdQ1bA.jpeg)
```

---
## \#6 Posted by: Sn4pz Posted at: 2019-07-04T21:42:35.686Z Reads: 25

```
https://www.electric-skateboard.builders/t/vesc-not-recognized-by-os/3858

https://www.electric-skateboard.builders/t/vesc-problem-need-help/31375/10?u=sn4pz

Here are some interesting threads, maybe one has a lead

It sort of sounds like the mcu has gone kaput, but I would do more investigation before removing anything

Do you have a multimeter?
```

---
## \#7 Posted by: florr Posted at: 2019-07-04T22:01:49.233Z Reads: 25

```
Unfortunately, i did not find anything useful in the threads.

Yes, i do have a multimeter - but i do not know, which Voltage should be where...
```

---
## \#8 Posted by: laurnts Posted at: 2019-07-04T23:14:58.518Z Reads: 26

```
I think you messed up your bootloader and require you to reflash the firmware.
You can do this with Stlink v2 or using another VESC to reflash the broken vesc (you will need vesc with firmware 3.57 or above. There will be an option in VESC Tool called SWD prog to reflash a vesc with another vesc).
```

---
## \#9 Posted by: florr Posted at: 2019-07-05T06:33:25.592Z Reads: 19

```
Thanks for the answer.

I do not have a second vesc atm., but orderd a Stlink v2.
I guess the tutorial (https://www.electric-skateboard.builders/t/vesc-boot-loader-installation-tutorial/32103) should still work?
```

---
## \#10 Posted by: FirstTimeBuilder Posted at: 2019-07-06T18:20:43.265Z Reads: 12

```
Hi, 

I had a big issue with two of my vescs and i contacted a guy called Martin who is fixing them for me, 35euro to fix ans ship back. If the StLink doesnt work (it didnt with mine) i recommend sending them to him. PM me and i can send his email over if you need it.
```

---
