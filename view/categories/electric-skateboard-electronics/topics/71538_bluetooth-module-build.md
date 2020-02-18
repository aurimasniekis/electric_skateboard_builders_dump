# Bluetooth module build

### Replies: 13 Views: 268

## \#1 Posted by: Blacksheep Posted at: 2018-10-17T15:12:49.641Z Reads: 103

```
Ok so i live in mexico and want to make my own Bluetooth modules
1- do I need to program the hm-10 or not? 
2- are this the connectors ? ![image|281x499](upload://jI7A1D2tzWU8SYPZkLBi8yOsLxF.jpeg)
```

---
## \#2 Posted by: Blacksheep Posted at: 2018-10-17T15:16:09.084Z Reads: 91

```
Help @rey8801 hehe
```

---
## \#3 Posted by: rey8801 Posted at: 2018-10-17T15:18:32.123Z Reads: 87

```
You need JST PH 7 pins. Well you will use 4 pins in total so they will also work but why bother about it when you can get it for cheap anyway. I will post one link. https://www.aliexpress.com/item/10-Sets-JST-2-0mm-PH-7-Pin-Female-Housing-Connector-with-Wire-and-Male-Connector/32823550472.html?spm=a2g0s.9042311.0.0.27424c4dPX360m
For the module depends which phone you have and which module you buy. Which phone do you have?
```

---
## \#5 Posted by: Blacksheep Posted at: 2018-10-17T17:08:16.723Z Reads: 71

```
I have iPhone 7 but I would like to make for iPhone and Android
```

---
## \#6 Posted by: rey8801 Posted at: 2018-10-17T17:10:34.363Z Reads: 65

```
for iphone you don't need. For Android Oreo there is the risk. Is not that diffiucult. I found that this clone in 80% of the case works with Android too https://www.aliexpress.com/item/AT-09-BLE-Bluetooth-4-0-Uart-Transceiver-Module-CC2541-Central-Switching-compatible-HM-10/32460561807.html?spm=a2g0s.9042311.0.0.27424c4dZKdfqb. But better to flash it because can be that with futher updates it won't be compatible anymore. That what I do for the modules I see
```

---
## \#7 Posted by: Blacksheep Posted at: 2018-10-17T17:11:26.733Z Reads: 60

```
Do i have to program it ?
And do you have a correct wire diragram
```

---
## \#8 Posted by: rey8801 Posted at: 2018-10-17T17:13:26.987Z Reads: 61

```
If you read above I just answered. I have like 20 of them. The most recent ones work with Android Oreo. Although I can not be sure it will work in the future. In case you can flash it later
```

---
## \#9 Posted by: rey8801 Posted at: 2018-10-17T17:14:22.163Z Reads: 61

```
The wire diagram is posted everywhere on the forum

Anyhow shortly

HM-10          /        vesc
VCC              /       5V
GND              /       GND
RX                 /      TX
TX                 /       RX
```

---
## \#10 Posted by: Blacksheep Posted at: 2018-10-17T17:20:12.803Z Reads: 58

```
Ok i así about this because the ones that I bought where connected to 3v
```

---
## \#11 Posted by: rey8801 Posted at: 2018-10-17T17:21:05.453Z Reads: 56

```
this module handles 5V no problem :wink:
```

---
## \#12 Posted by: Lambjr088 Posted at: 2018-10-17T17:45:01.533Z Reads: 50

```
Would u happen to have a link on how to flash the modules for oreo?
```

---
## \#13 Posted by: rey8801 Posted at: 2018-10-17T18:38:03.760Z Reads: 45

```
Here we go
https://forum.arduino.cc/index.php?topic=393655.0
Check on YouTube like flash hm10 firmware on... And you will find a video too.
```

---
## \#14 Posted by: mtuan293 Posted at: 2018-10-18T01:13:31.164Z Reads: 29

```
Just want to say that after flashing mine with the original HM-10 firmware, it works a lot more reliable with my iPhone on iOS 11. It used to fail to write configs using Xmatic app and took several tries to make it work.
```

---
