# BLDC tool for MAC isn&rsquo;t recognizing VESC

### Replies: 11 Views: 760

## \#1 Posted by: Fecm93 Posted at: 2017-11-23T19:08:39.480Z Reads: 88

```
Hi! 

I'm trying to change my ride setup to FOC, but my BLDC tool does not recognize my VESC.

<img src="/uploads/db1493/original/3X/6/7/6764a0b9d75458b76b1bf7e303729436d0957787.png" width="253" height="133">

 I've all ready tried changing usb cables and ports but the outcome is the same.

I had previously managed to configure my ride settings and had no issue at all so I don't think it is a compatibility issue between my VESC version and the BLDC tool version. I have never updated any of them. I think it might be related to software update on my laptop. I'm using MacBook pro with macOS Sierra 10.12.6

Any ideas on what could be wrong?

Thank you in advance for any help!
```

---
## \#2 Posted by: Namasaki Posted at: 2017-11-24T04:44:09.696Z Reads: 78

```
Are you connecting the cable then turning on the vesc then opening the bldc tool?

Then again, this might be a blessing in disguise if your trying to switch to FOC....

So many people have had problems with FOC and so many Vescs have died.
```

---
## \#3 Posted by: wafflejock Posted at: 2017-11-24T04:54:43.911Z Reads: 75

```
Not really familiar with MacOS I use Ubuntu though so familiar with whatever is common from UNIX/Posix compliance looks like they also have dmesg though for seeing new connected devices

https://discussions.apple.com/thread/4170078?start=0&tstart=0

when I hook up my VESC 4.10 HW and go to terminal and type `dmesg` (enter) I get something like below:
```
[937419.047632] usb 2-1.1: new full-speed USB device number 30 using ehci-pci
[937419.134552] usb 2-1.1: New USB device found, idVendor=0483, idProduct=5740
[937419.134560] usb 2-1.1: New USB device strings: Mfr=1, Product=2, SerialNumber=3
[937419.134564] usb 2-1.1: Product: ChibiOS/RT Virtual COM Port
[937419.134567] usb 2-1.1: Manufacturer: STMicroelectronics
[937419.134570] usb 2-1.1: SerialNumber: 301
[937419.135065] cdc_acm 2-1.1:1.0: ttyACM0: USB ACM device
```
I just upgraded mine to the 3.33 firmware and using the new VESC tool has been working well as far as I can tell on a couple of small trips (new interface with wizards for motor and control config worked without a hitch too, took me a while to realize the write app was separate from write motor config for adding UART for metr support but otherwise good to upgrade too).
```

---
## \#4 Posted by: Fecm93 Posted at: 2017-11-24T12:45:33.285Z Reads: 61

```
Hi! Yes, but still the bldc tool seems to not recognize the VESC. 

The VESC seems to work fine, I haven’t had any issues while riding my board and the last time I updated my riding settings (one month ago) bldc tool was working fine, that’s why I think is more of a driver issue or something like that since MacOS last upgrade :frowning2:
```

---
## \#5 Posted by: Namasaki Posted at: 2017-11-24T15:58:18.740Z Reads: 55

```
Did you upgrade from Sierra to High Sierra ?
```

---
## \#6 Posted by: WARMAN Posted at: 2017-11-24T16:05:16.921Z Reads: 54

```
I had that same problem but not on Mac,are your vesc's flashing ie do they have power when you turn your power suply on? Mine was a driver issue,i just installed a new one and was good to go.
```

---
## \#8 Posted by: Fecm93 Posted at: 2017-11-26T19:53:01.428Z Reads: 54

```
hi!

Yes, vesc's are flashing when they have power.
```

---
## \#9 Posted by: Fecm93 Posted at: 2017-11-26T19:55:17.542Z Reads: 52

```
Yes, the upgrade was from Sierra to High Sierra. Have all ready re-installed BLDC tool but the problem still persist, the VESC does not appear when connected.
```

---
## \#10 Posted by: Namasaki Posted at: 2017-11-26T20:51:38.462Z Reads: 50

```
I'm not sure what happened. I have not upgraded from Sierra.
Try connecting something else to the USB port and see if it works.
```

---
## \#11 Posted by: Blacksheep Posted at: 2018-04-25T02:17:53.121Z Reads: 32

```
Where did you get the vesc tool for Mac ?
```

---
## \#12 Posted by: GunnarK Posted at: 2019-04-10T13:05:16.320Z Reads: 14

```
I am running into this problem as well. Anyone figure this out?
Got a 2017 MacBook Pro without touchbar running Mojave 10.14.3
The 2 USB-C model. I got a Satechi USB hub
```

---
