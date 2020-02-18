# Setup HM-10 BLE on VESC 4.12

### Replies: 4 Views: 314

## \#1 Posted by: chickengun Posted at: 2019-04-20T23:43:46.054Z Reads: 66

```
I ordered a [HM-10 BLE module from aliexpress](https://www.aliexpress.com/item/AT-09-BLE-Bluetooth-4-0-Uart-Transceiver-Module-CC2541-Central-Switching-compatible-HM-10/32460561807.html) and connected it to my slave vanda vesc over 5V,GND,RX,TX. It is recognized by my android phone (Xiaomi Mi A1) as "JDY-30" and the PIN I needed to connect is 1234. So while I am able to connect to it over android 9 pie I have no luck on any vesc app: With ackmaniacs and vedder's mobil vesc tool I can't find the bluetooth module (when scanning for bluetooth devices in the app) so I can't connect at all. Even when I delete the existing connection within android pie 9 (known devices), it never shows up in the app. As far as I understood I can't test metr.at because it won't work with a regular BLE module. However I installed the app and when I press on Search no Bluetooth device shows up at all (maybe that's normal). There is another app called "VESC Monitor". Here I can connect flawlessly to the HM-10 but I get no telemetry... All the values like battery voltage etc. show zero. I also tested it with my old samsung galaxy s5, same problem. It's quite frustrating. Is there another android app I can test? Any ideas are appreciated.
```

---
## \#2 Posted by: Grozniy Posted at: 2019-04-20T23:47:51.966Z Reads: 62

```
I have same A1 but it doesn't find the ble module. So I use an old Android phone.
I know @rey8801 was flashing them and making them work on new Android
```

---
## \#3 Posted by: rey8801 Posted at: 2019-04-21T00:20:23.969Z Reads: 57

```
I suggest to read better the thread. Bluetooth Low Energy modules do not require you to connect it directly as a normal Bluetooth module. You only need to connect to it through the app that supports the feature. In case of vesc app from Ackmianc of what you are talking about of you can see the modules than you don't need to flash it with HM10 software because already compatible with your phone. You probably didn't set correctly the baud rate and setting on the vesc. That's why don't get twlwmtry or the pin are not correct on the vesc UART port.
```

---
## \#4 Posted by: chickengun Posted at: 2019-04-21T17:51:37.358Z Reads: 35

```
Non of the apps recognized [my bluetooth module](https://www.aliexpress.com/item/AT-09-BLE-Bluetooth-4-0-Uart-Transceiver-Module-CC2541-Central-Switching-compatible-HM-10/32460561807.html). So I tried to flash the firmware following [this](http://forum.arduino.cc/index.php?topic=393655.0) tutorial but I failed as some did too. I guess I will buy a different model or try the HC-05 module
```

---
