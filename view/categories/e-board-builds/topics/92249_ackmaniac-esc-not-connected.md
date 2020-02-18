# Ackmaniac - ESC not connected

### Replies: 11 Views: 374

## \#1 Posted by: MrDGOrman Posted at: 2019-04-29T21:41:50.232Z Reads: 108

```
Hi everyone,

I have had the Ackmaniac app and HM10 BT module since my 2nd build. It sometimes works, it sometimes doesn't. Usually after an update of some sort it kills the connection and I struggle to get it working again. It's VERY frustrating to say the least.

The app seems to connect to the BT module but as soon as I go to view some of the data it comes up with ESC not connected. I don't get what's going wrong? Baudrate is set to 9600 as suggested.

Does anyone have any advice?
FOCBOX single drive, HM10 BT module.

Cheers guys!
Dan

PS. Yes, I've searched the forum but I can't seem to locate the specific problem or a fix. My apologies if this has already been discussed - I must be searching the wrong thing.
```

---
## \#2 Posted by: J0ker3366 Posted at: 2019-04-29T22:48:30.951Z Reads: 95

```
The only thing you forgot to mention is what device your using to connect BLE
```

---
## \#3 Posted by: MrDGOrman Posted at: 2019-04-29T23:59:42.923Z Reads: 93

```
Huawei Mate 20 Pro. The app has worked on this phone before
```

---
## \#4 Posted by: mynamesmatt Posted at: 2019-04-30T00:42:59.063Z Reads: 81

```
try changing the baud rate to 115200. Might fix something? idk. might be a loose connection or faulty hm10?
```

---
## \#5 Posted by: MrDGOrman Posted at: 2019-04-30T09:47:38.193Z Reads: 70

```
Thanks I'll give this a shot.

It's really frustrating because for some reason my board seems to go into a limp mode of some sorts. I was hoping to get some real time data so that I can narrow down the issue!

It's almost like something is getting too hot and it's kicking it into a safety mode.

Cheers though, I'll look into the baudrate.
```

---
## \#6 Posted by: Bookeh Posted at: 2019-05-22T18:34:25.795Z Reads: 52

```
Hi there, First post on this forum so hopefully this ends up in the right place,
I have a Turnigy esk8 VESC running 4.12 and Firmware 3.57. I have just ordered a HM10 (https://www.amazon.co.uk/DSD-TECH-Bluetooth-iBeacon-Arduino/dp/B06WGZB2N4). I have the ackmaniac app and it "connects" to the HM10, the red LED stops flashing and is a solid red light. But when i hit "mode" on the app it says "esc not connected". Has there been a fix for this?
In the VESC software i am running PPM and UART with the UART at 9600 bps.
I have tested connecting on:
-Galaxy S9 on Android 9
-Nvidia Shield running android 7.0
-Iphone SE on ios 11
Both android phones connect (LED stops flashing)..
The iphone can't see the HM10
Any help would be great,
Cheers
```

---
## \#7 Posted by: MrDGOrman Posted at: 2019-05-22T19:27:01.919Z Reads: 48

```
Hey bro. You ended up replying to my thread rather than making your own. To make your own make sure you're on the forum home page.

Either way, it's the app at fault. The app doesn't support the vesc fireware version yet. I had the same issue. You can either change system altogether or go without. Changing system would be going for the Metr or Trampa option. I went down the Trampa route.
```

---
## \#8 Posted by: J_Dizzle Posted at: 2019-05-22T19:42:41.956Z Reads: 45

```
Hello, I’m having the same problem as you also. I’m pretty sure Akc 3.101 and 3.102 are supported. The most recent firmware, 3.103, is not. I had to downgrade to 3.102 but I still can’t get the Vesc to connect however the Bluetooth does. What would you recommend?
```

---
## \#9 Posted by: gaetjen Posted at: 2019-05-22T20:28:11.805Z Reads: 43

```
Same problem here. I can connect to the module, but it doesn´t show any data and then says that the VESC is not connected. Has been working before that for a long time and nothing in my setup has changed. @Ackmaniac any idea?
```

---
## \#10 Posted by: jun1208 Posted at: 2019-05-28T06:46:06.294Z Reads: 36

```
Same thing here too..connected to the bluetooth module but app says ESC not connected..
```

---
## \#11 Posted by: Rodeodave Posted at: 2019-07-10T05:12:46.658Z Reads: 25

```
Had the same problem with my Raptor 2, got to make it work with these settings in the ackmaniac tool:
9600 baud for UART
"APP to use" for master focbox set to "PPM and UART"

After running the input wizard, APP to use was set to APP only, had to manually switch to PPM and UART.
```

---
