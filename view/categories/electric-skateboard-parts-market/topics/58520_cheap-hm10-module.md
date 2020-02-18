# Cheap HM10-module

### Replies: 9 Views: 981

## \#1 Posted by: legend27 Posted at: 2018-06-11T14:42:02.600Z Reads: 174

```
Hi everyone :slight_smile:

I have found a cheap DIY solution for a HM-10 module :slight_smile: If you can wait 30-50 days will it cost you **$5.22**. I've bought the parts but haven't received them yet. Don't know if they will work but I will give you an update :slight_smile:

**PARTS:**
- **1x $3.22** - [10pcs JST Mini 2.0 PH 7-pin](https://www.aliexpress.com/item/10pcs-Micro-JST-Mini-2-0-PH-2-3-4-5-6-7-8-9-10/32868201984.html?spm=a2g0s.9042311.0.0.5aec4c4d0Awt3x)
- **1x $2** - [HM-10 module](https://www.aliexpress.com/item/Freeshipping-HC-06-Wireless-Bluetooth-Module-With-baseboard-Slave-Wireless-Serial-Port-for-arduino-with-Dupont/1568545615.html?spm=a2g0s.9042311.0.0.5aec4c4d0Awt3x)

Thanks a alot to the guy who made this video https://www.youtube.com/watch?v=yBid4kL96TM&t=77s

![Screenshot_18|651x499](upload://7SOkwbwoHazFvx8COfIZD2uSpsS.jpg)
```

---
## \#2 Posted by: rey8801 Posted at: 2018-06-11T14:54:43.782Z Reads: 163

```
You could just ask on the forum. Yes it will work. There is also a toturial how to wire the bluetooth module http://www.electric-skateboard.builders/t/vesc-hm-10-bluetooth-wiring/12838/19

Basically:
HM-10 - VESC
VCC - 5V
GND - GND
TX - RX
RX - TX

Connect HM-10 cables to master VESC UART port
Change application from PPM to PPM and UART and set baud to 9600. Done!

Just to know the one you have is a clone of course, not the real HM-10. Don't worry, almost everyone has a clone :wink:. In case you would need more and fast in the future I have some left http://www.electric-skateboard.builders/t/esk8-flea-market-eu-ww-small-cheap-parts-hm-10-bluetooth-android-oreo-compatible-volt-meter-3dprinting/57463.

Ciao ciao
```

---
## \#3 Posted by: legend27 Posted at: 2018-06-11T15:01:17.129Z Reads: 149

```
Thanks! What are the difference between clones and the real ones? How can you tell if its a clone?
```

---
## \#4 Posted by: rey8801 Posted at: 2018-06-11T15:07:18.569Z Reads: 143

```
https://blog.yavilevich.com/2016/12/hm-10-or-cc41-a-module-automatic-arduino-ble-module-identification/
Basically first thing the real HM-10 cost more, so that it's already something to take into account. Then if you look inside the blog page, they differ for the breakout board and some component on the module itself. Could be without the 5v to 3.3V converter ecc... In general they will all work, but the main concern about is that they run another firmware compare HM-10, and with the last Android update Oreo you could have the problem that your phone doesn't detect them. For the previous Android version and IOS no problem. What you can do is flash the orignal firmware following this procedure https://forum.arduino.cc/index.php?topic=393655.0. PAste the same in you tube and you will find a video about it.
```

---
## \#5 Posted by: Acido Posted at: 2018-06-11T15:48:41.946Z Reads: 115

```
I got 20 of them in stock
6$ not wired, comes with wires 7 
11$ wired and shipped

Shipping from Croatia
```

---
## \#6 Posted by: Acido Posted at: 2018-06-11T15:49:20.869Z Reads: 110

```
hm 10 that show up as hm05 is the same crap they work at 5v and they function the same as the "geniue" hm 10 module so why bother
about oreo idk whats the problem tho
```

---
## \#7 Posted by: rey8801 Posted at: 2018-06-11T16:23:22.827Z Reads: 105

```
The original HM-10 firmware shows up as hm-10. I only said that the ones I have seen around are usually CC2541 and those are clone not HM-10 or HM-5. They are detected as CC41 on the phone.
```

---
## \#8 Posted by: Acido Posted at: 2018-06-11T16:28:21.233Z Reads: 102

```
i ordered from atleast 10 sellers on ebay alibaba and aliexpress all were hm10 in the item description but all of them showed up as hm05
```

---
## \#9 Posted by: rey8801 Posted at: 2018-06-11T16:34:27.844Z Reads: 98

```
I also have like 30 of them from different seller. I always got MBL-5 like the one @legend27 bought or CC41. You can read the name of the cheap on the module.
```

---
