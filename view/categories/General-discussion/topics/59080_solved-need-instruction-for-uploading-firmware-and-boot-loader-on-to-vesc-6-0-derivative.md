# \[SOLVED\] Need Instruction for uploading Firmware and Boot loader on to VESC 6.0 derivative

### Replies: 6 Views: 587

## \#1 Posted by: chuttney1 Posted at: 2018-06-16T06:02:19.400Z Reads: 103

```
I got HW4.7 VESC and know how to upload bootloader and firmware and this version requires an external battery to power up to upload firmware and bootloader. 

What's the procedure for HW6.0 and up? Do you need to supply power or is that 5V USB power from the computer good enough?
```

---
## \#2 Posted by: Minim Posted at: 2018-06-16T06:12:54.012Z Reads: 98

```
I don’t know if this is relevant but close to the USB port there is a resistor spot for a 0ohm resistor that will allow the usb to power the chip. If this is not in its spot I need a battery for the vescs power supply to power the chip and if it’s in place Usb will power it. I read that people had problems with this populated since you then can’t have battery and usb hooked up at the same time so I’ve never tested with mine installed.
```

---
## \#3 Posted by: pat.speed Posted at: 2018-06-16T06:24:00.113Z Reads: 91

```
There was talk about this with @bimmer and the b boxs, I think it turned out that it could potentially ruin the vesc by powering it through the two different sources, something to do with a ground loop maybe? Although @stewii said he hadn’t had any problems. 

I think someone said that they just plugged the Vesc into the normal battery, and cut the power wires off the USB cable.

It’s very confusing, something to do with r1 or r0 I can’t remeber
```

---
## \#5 Posted by: DougM Posted at: 2018-06-16T16:10:33.917Z Reads: 69

```
I think you might need Reset as well.
```

---
## \#6 Posted by: chuttney1 Posted at: 2018-06-17T04:26:15.795Z Reads: 61

```
I will update this on how I went about for future references for anyone using Ubuntu Xenial. Programing was done with a STM32F4 Discovery making sure to match the pins on the derivative with the SWD port on the discovery board I had sitting around and a micro USB cable for 5V power from computer on the VESC derivative.

To program a new VESC derivative with no firmware and boot-loader. The codes on Vedder's blog found here (http://vedder.se/2015/01/vesc-open-source-esc/) typed/pasted below, Ignore bulletpoint when typing into terminal in Ubuntu.

* sudo apt-get install build-essential qt-sdk openocd git libudev-dev libqt5serialport5-dev
* sudo adduser $USER dialout
* sudo apt-get remove modemmanager

The modemmanager and udev rules can be configured if you run the VESC tool provided by the https://vesc-project.com/ I do not know if 
 
"Note: Before running the make upload command, you should open conf_general.h and select which hardware version you are using."

Git, make, upload firmware. 
* mkdir BLDC
* cd BLDC
* git clone https://github.com/vedderb/bldc.git bldc-firmware
* cd bldc-firmware
* make upload
* cd ..

Same with Git, make, and upload bootloader.
* mkdir BLDC
* cd BLDC
* git clone https://github.com/vedderb/bldc-bootloader.git bldc-bootloader
* cd bldc-bootloader
* make upload
* cd ..

I have to figure out how to get this to now connect to the pc  and find COM port even with battery connected and USB connection.
```

---
## \#7 Posted by: Nanorider Posted at: 2019-01-04T07:17:03.349Z Reads: 25

```
do you have a link to hw60 for st-link upload?
```

---
