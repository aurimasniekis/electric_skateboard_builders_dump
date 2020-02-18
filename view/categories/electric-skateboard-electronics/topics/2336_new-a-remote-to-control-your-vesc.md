# NEW! A remote to control your VESC!

### Replies: 17 Views: 5811

## \#1 Posted by: jacobbloy Posted at: 2016-04-13T19:03:55.744Z Reads: 535

```
This will change the way we ride our electric skateboards!

Mobile app and remote connected to the same receiver!

https://youtu.be/N98Oqr0WRG0
```

---
## \#2 Posted by: appelton Posted at: 2016-04-13T19:07:15.572Z Reads: 522

```
This is just superb!! Beyond words! Awesome job!
```

---
## \#3 Posted by: onloop Posted at: 2016-04-13T23:36:37.096Z Reads: 490

```
some more footage of the phone app working.

https://www.youtube.com/watch?v=9LYkgey1dX0&nohtml5=False
```

---
## \#4 Posted by: Blasto Posted at: 2016-04-14T00:23:06.546Z Reads: 472

```
Well look at what we have here, guess i don't have a choice to try it out
<img src="/uploads/db1493/original/2X/5/5575a03f17b2bb4d11962515889c7e82a337588e.jpg" width="375" height="500">
```

---
## \#5 Posted by: jacobbloy Posted at: 2016-04-14T00:50:22.770Z Reads: 442

```
I'm really sorry mate but there HC-06 modules and the app is made for ble you will need a HM-10 or HM-11<img src="/uploads/db1493/original/2X/0/09b8468e263c0f05b968136389d17d6bed330acf.jpeg" width="375" height="500">

See the difference!
```

---
## \#6 Posted by: FLATLINEcustoms Posted at: 2016-04-14T20:17:20.240Z Reads: 412

```
@jacobbloy will this work? http://www.amazon.com/Diymall%C2%AE-Bluetooth-Module-Anti-lost-Android/dp/B00O2TTUEW
```

---
## \#7 Posted by: ikjahaa Posted at: 2016-04-14T21:01:47.695Z Reads: 409

```
So if the communication goes by bluetooth, what security measures are you using ?
```

---
## \#8 Posted by: jacobbloy Posted at: 2016-04-15T00:08:18.610Z Reads: 409

```
None! I know the boosted board got hack and they had to fix it, but it's just as easy to do the same to a nrf24lo1 chip or any other RC remote, even with boosted boards encryption I could still sniff there app packets being sent.
```

---
## \#9 Posted by: jacobbloy Posted at: 2016-04-15T00:08:59.800Z Reads: 408

```
Yes this will work but you don't know the quality.
```

---
## \#10 Posted by: hexakopter Posted at: 2016-04-15T09:06:39.313Z Reads: 406

```
Looks good. But why are you not using a baud rate of 115200? Changing the baud of the HMSoft modules is easy. Do you also have tested it on HM-12 dual bluetooth modules? I hope that it would be possible to use the nunchuk connected over BT 2.0 and the mobile phone over BT4.0 at the same time. It has a "DUAL Work Mode" stated in the data sheet to "allow two connections at same time (SPP and BLE)".

Have you tested your app with iOS 7? I have the chance to get access to an jailbroken device with iOS 7. I already have one HM-10 and two HM-12 devices.
<img src="/uploads/db1493/original/2X/3/321cc686f623e5ffd389213b560905a218132f51.jpg" width="375" height="500">
```

---
## \#11 Posted by: jacobbloy Posted at: 2016-04-15T10:19:43.498Z Reads: 390

```
a baud rate of 115200 yes i have tried it and no it does not work well, the SPP uart service that the ble devices use get bottle necked. if you are using spi and connecting to multiple uuid services and multiple characteristics on the device  for different activities of the device then it could work at 115200.

even the nordic uart service can not operate at 115200 and they use 2 characteristic for the uart, 1 for RX and another for TX where HMsoft only use 1 for both. (adafruit limit there nrf51822 uart chip to 9600 where there spi version can use 115200)

also the genuine HM-10,11,12 chips run write with out response which is limited to 20 byte packets so i have already had to implement a rolling chunk data write where the string is repeated until all data is written.

for example when just writing motor limits and not motor configuration it is writing over 400bytes so in this case 9600 baud rate wouldn't help at all.

fake chines chips like the one that it looks like you have in the middle (unless you have removed the extra crystal) are write with response so this isn't an issue but they can cause other issues with services to working correctly with the BLE SDK in QT.

as for the nunchuk i don't think there is a need to add the hm-12 chip but you can use it if you would like.
the reason is (as per my understanding) i have modified the nunchuk firmware for uart and uart uses the SPP in the chip, and this can only be used by one of the protocols at a time, you can use BLE and spp at the same time but this requires creating customer services and characteristics or just using the ibeacon service in BLE so again no real benefit.

i could write custom firmware for the nunchuk that can do this but i don't have the time to do it sorry! i have spent so long with this project both the app and the nunchuk, i wrote the first version of firmware for the usb bridge that benjamin vedder implemented into the nunchuk but then he completely rewrote it and know it works amazing. 
it is just where I'm floored with experience i have to ask for help or pay a freelancer and my bill is over $2000 ATM and sadly because I'm doing this as and open source project i will never make this money back but who every starts selling the nunchuk will, and the app will only complement @chaka and @onloop sales.  

benjamin vedder is writing customs firmware for the nrf51822 chip and this will work with both the vesc and nunchuk and will use dual protocol of nrf24lo1+ and BLE at the same time and he has a much greater understanding of how to do this then i do and when it is completed it will be supported by my app.

at the moment i can not afford to pay for an apple developer licence so i can't distribute the app to iOS for testing, any support for this will help every one!

But as of today i have started implementing video logger into my Mobile APP so you can record your ride while logging the vesc output data.
```

---
## \#12 Posted by: Haimindo Posted at: 2016-05-02T18:33:07.975Z Reads: 336

```
Just got my HM-10 module, can you send me the android version of your app? More than happy to test it out and report the experience :slight_smile:
```

---
## \#13 Posted by: CSC Posted at: 2016-11-24T16:21:15.612Z Reads: 235

```
Hi jacobbloy.  Really great stuff. Thanks for making this available! Can't wait to install the HC-10 module, and stop disassembling my board to re-program the VESCs using USB. Question: Will I still be able to use my 2.4GHz (Winning) remote (with its own receiver) that is currently connected to the 3-pin Servo header, using PPM? If they can both be operational at the same time, is there some additional safety measure in powering down the HC-10 during normal board use (i.e., an in-line switch on the Vcc line to cut power to the BT module), assuming I don't want to track info with my phone at that time?  Thanks again!
```

---
## \#14 Posted by: mccloed Posted at: 2016-11-24T16:44:45.198Z Reads: 221

```
Hey @CSC, I have used this with a gt2b along with the phone app. You just need to set the VESC to PPM and UART. At least, that's what worked for me.
```

---
## \#15 Posted by: CSC Posted at: 2016-11-24T17:02:29.624Z Reads: 218

```
Thanks, mccloed. Yeah, I see now in BLDC that there is a "PPM and UART" option in the App Config/General tab. I should have looked there before asking the question. Do you leave both the gt2b and BT modules permanently powered up? Do you ever have conflicts between the two in normal operation (unwanted throttle, for example). Thanks.
```

---
## \#16 Posted by: mccloed Posted at: 2016-11-24T17:50:24.383Z Reads: 204

```
I've actually have only ridden it a couple of times and did not experience any issues. I only used the app for the monitors.
```

---
## \#17 Posted by: CSC Posted at: 2016-11-25T07:10:44.520Z Reads: 183

```
Thanks @mccloed. I'll try it out this weekend, when my BT module arrives. If any issues arise, I will add an in-line switch to cut power to the BT module's Vcc pin, and post my observations to this forum. But reading your post and an email from http://miamielectricboards.com, I'm not anticipating any issues. Thanks again.
```

---
