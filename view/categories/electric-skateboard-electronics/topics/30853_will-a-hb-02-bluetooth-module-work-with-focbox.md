# Will a HB-02 Bluetooth module work with FOCBOX?

### Replies: 10 Views: 1435

## \#1 Posted by: RiGo Posted at: 2017-08-17T04:54:53.160Z Reads: 191

```
I have an old BT module I use to tune my racing quadcopter and would like to repurpose it for my new build.

Do you guys know if this will work with a FOCBOX? And how would I need to connect it?

Default baud rate is 115200 and can't really change it as I'd need an Arduino or programming card. Do VESCs communicate at 9600bps?

<img src="/uploads/db1493/original/3X/9/b/9bc2397d5cd9fd5f644a18767ead2c225bc1abfe.jpg" width="499" height="499">

<img src="/uploads/db1493/original/3X/d/d/ddef506323d9b3bcc47914ef7050eb4c0863e25c.jpg" width="500" height="500">
```

---
## \#2 Posted by: velox Posted at: 2017-08-17T16:14:07.963Z Reads: 161

```
Hi, your bluetooth module looks like HC-05/HC-06 to me, but I might be wrong. The default UART baud rate for VESC (hw 4.12, FOCBOX may be different) is 115200 but you can easily change it using BLDC tool. If your bluetooth module supports 115200 you should use this for better data throughput. To set up the module you may connect it to an Arduino or some FTDI USB breakout thing (RX pin goes to TX and vice versa, common GND). Then start the serial monitor from Arduino IDE to set up the bluetooth module using AT commands. Here is a link that helped me a lot https://arduino-info.wikispaces.com/BlueTooth-HC05-HC06-Modules-How-To
```

---
## \#3 Posted by: evoheyax Posted at: 2017-08-17T16:30:58.865Z Reads: 157

```
I'm not sure if theres any apps supported by this module, so you would have to write your own app. Your better with an hc-10 or adafruit uart buddy chip, which are both supported by multiple apps.
```

---
## \#4 Posted by: longhairedboy Posted at: 2017-08-17T16:34:04.491Z Reads: 155

```
wouldn't the HM-10s be better for that?
```

---
## \#5 Posted by: evoheyax Posted at: 2017-08-17T16:39:14.530Z Reads: 150

```
I mean HM-10... HM, HC, all the same.... hahaha
```

---
## \#6 Posted by: longhairedboy Posted at: 2017-08-17T16:52:34.892Z Reads: 143

```
oh ... well in that case.. i have them for $8.

https://longhairedboy.com/collections/all/products/hm-10-ble-bluetooth-serial-adapter-for-vesc-type-motor-controllers

I wanted to try them out and couldn't help but buy a few extras so i listed them.
```

---
## \#7 Posted by: RiGo Posted at: 2017-08-17T20:47:28.136Z Reads: 125

```
@Ackmaniac do you know if this module would work with your android app?
```

---
## \#8 Posted by: RiGo Posted at: 2017-08-17T22:29:53.127Z Reads: 111

```
[quote="evoheyax, post:3, topic:30853"]
I'm not sure if theres any apps supported by this module
[/quote]

How does that work though...? If you're able to connect to the BT module, say on your phone or computer, doesn't it just act as a bridge for the UART connection? So:

(VESC) ----UART----> (BT Module) ----UART-over-BT-protocol----> (phone/computer)

instead of

(VESC) ----UART-via-USB----> (computer)

So why do some BT modules (like this one) not work?
```

---
## \#9 Posted by: velox Posted at: 2017-08-18T07:18:20.795Z Reads: 94

```
An UART bridge would look like:
(VESC) ----UART----> (BT module A) ----UART-over-BT-protocol----> (BT module B, eg. HM-05/06/10 or built-in module)  ----UART----> (receiving software on phone/computer)
Both BT modules must be
- paired properly (BT version has to be compatible eg. BLE will not work with non-BLE BT)
- in BT pass-through mode
- run at the same baud-rate (which has to be at least as fast as the VESC baud-rate)
Given that the BT types of the modules are the same the rest can be set-up easily using AT commands. Android BT stack might also add constraints. As far as I've read in this forum HM-10 seems to be the most compatible module.
```

---
## \#10 Posted by: RiGo Posted at: 2017-08-18T12:58:05.699Z Reads: 89

```
Got it, thanks! :slight_smile:
```

---
