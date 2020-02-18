# VESC data logging advice

### Replies: 9 Views: 1303

## \#1 Posted by: Msk8 Posted at: 2017-07-08T06:01:36.402Z Reads: 143

```
I will go on my first efoil test run **with a VESC** contoller tomorrow morning [(see project info here)](http://www.electric-skateboard.builders/t/diy-hydrofoil-build-build-porn-at-its-finest/26369).  I know it's not directly a skateboard, but tech is very close and in a way it's a water-skateboard ;) ...so hope you don't mind me asking here. 

The VESC is especially awesome because of all the data logging capabilities. I have a completely new design and am pretty sure something will go wrong. Know where and why is key.

So I spent all afternoon trying to figure out what logging software to use. Here is the HW I have tomorrow:
- OLLIN VESC HW 4.12
- **BT-05 module** (from https://miamielectricboards.com on Feb 12 2017)
- iPhone
-Android Phone (just went to BestBuy and got a $79 Samsung just for this because I could not find a iOS logging app)

So I am still struggling to find any logging apps that work with this HW. Here is what I tried:
- VESC Connect Pro (Android) - connects fine, no logging capabilities
- VESC Connect Lite (Android) - can't connect, don't know if it has logging
- VESC Monitor (Android) from Ackmaniac, I changed FW to his 2.54 and then after that I read that his app only works with the HM-10 Bluetooth module. I went back to FW 2.18 
- Metr (iOS) - only works with his BT modules. I have a couple of these modules on order but they are not here for my test tomorrow,
- VESC Logger (iOS) - could not connect
- VESC Status (iOS) - could not connect

Is there any other logger app for Android or iOS that works with my BT-05 module I can try?
```

---
## \#2 Posted by: Jinra Posted at: 2017-07-08T06:23:13.095Z Reads: 127

```
@evoheyax has an iOS app
```

---
## \#3 Posted by: JdogAwesome Posted at: 2017-07-08T06:25:55.373Z Reads: 123

```
I dont think anybody would mind you asking, eboard or not! So your pretty much looking for some device the just logs the VESC not just displays it on an app like most of them do. I swear I remember seeing a Bluetooth logger on here that could log VESC info to like a micro sd or something, but im not sure. If you want to ask @Ackmaniac about it and his VESC Monitor app, definitely do so hes a nice guy! I would love to see some sort of dongle you can connect to your VESC that simply records the VESC, batt voltage, amperage, rpm whatever onto a micro sd and you can either access it via Bluetooth or just by plugging the micro sd into your computer. Personally id love to see something like that so I may try designing one, cant imagine it'd be to hard.
```

---
## \#4 Posted by: Pimousse Posted at: 2017-07-08T06:30:37.685Z Reads: 108

```
Recording on a microsd is not a big deal, I did it easily with an Arduino nano, sd card breakout board and using @RollingGecko library.
However, you should go with a HM10 to use VESC Monitor from @Ackmaniac ! Mostly if you already use his firmware.
Anyway, I'll look to your project, it seems so cool !
```

---
## \#5 Posted by: Msk8 Posted at: 2017-07-08T06:42:14.602Z Reads: 99

```
@Jinra, I tried @evoheyax app and could not connect. Maybe it also only works with the HM-10?

@JdogAwesome SD card logging would be nice but for tomorrow I am ok taking my phones in waterproof cases out with me. So for now I am just looking for an app that connects to my BT-05 and logs. And also the phone give me GPS speed which is important for my tuning process.

@Pimousse yes I like what @Ackmaniac has done with the watt control and throttle curves, am using it on my eskate and don't want to miss it. His app looks great too. Will get a HM10. 

.... still browsing for something that works with the BT-05 for tomorrow.
```

---
## \#6 Posted by: Pimousse Posted at: 2017-07-08T07:22:25.306Z Reads: 89

```
With a HC05, go for VESC Monitor from Solarturtle (Ackmaniac took the same name of app, not easy to sort it out sometimes :smile: ).
It should work but only for monitoring.
```

---
## \#7 Posted by: Msk8 Posted at: 2017-07-08T13:06:36.326Z Reads: 78

```
Thanks for clarifying @Pimousse. I have that app and will it again. Could not connect yesterday but I just read that people have success with the HC-05 at 115200bps, need to check my settings.

.. ok, settings checked. tried 115200, can't pair. Back to 9600bps now. The Solarturtle app needs it to be paired before using it - unlike the VESC_Connect app. But I keep getting the "pairing rejected by bt05" message when pairing in the android BT settings.
```

---
## \#8 Posted by: evoheyax Posted at: 2017-07-08T15:41:39.797Z Reads: 66

```
My app logs both locally to your phone and the websites server. But it requires an adafruit BT module.
```

---
## \#9 Posted by: Msk8 Posted at: 2017-07-08T17:46:52.659Z Reads: 60

```
Thanks @evoheyax. I finally got the Ackmanic app to run, got confused with the same names.
```

---
