# Trying to connect hm-10 to vesc app

### Replies: 33 Views: 3646

## \#1 Posted by: Zoomy Posted at: 2017-01-25T22:02:53.407Z Reads: 437

```
I've wired up my hm-10 bluetooth module to my vesc and the vesc app says it has connected to "BT05" and the red light on the hm-10 stops flashing but nothing happens when I tap on read configuration.

<img src="/uploads/db1493/original/3X/5/0/50cda10f27f3e6b68920cff22026265a0aaed76d.png" width="281" height="500">
```

---
## \#2 Posted by: lox897 Posted at: 2017-01-25T23:37:37.109Z Reads: 399

```
Is this Jacob's app? I am getting a similar error, "service not found"

Maybe the man himself could help? @jacobbloy
```

---
## \#3 Posted by: Ackmaniac Posted at: 2017-01-25T23:45:18.859Z Reads: 384

```
I guess you have to set the UART baud rate to 9600.
```

---
## \#4 Posted by: jacobbloy Posted at: 2017-01-26T00:14:13.990Z Reads: 383

```
The baud rate has to be set to 9600 and there is time out settings that are changed in the firmware to help it work. If you are not using firmware from my website then it won't work as Iv set these up already.
```

---
## \#5 Posted by: Zoomy Posted at: 2017-01-26T00:19:59.447Z Reads: 373

```
The baud rate is set to 9600 and Im using the software from your website.
```

---
## \#6 Posted by: Ackmaniac Posted at: 2017-01-26T00:34:38.720Z Reads: 358

```
Which hm-10 module is it exactly? Maybe you have the link where you bought it.
```

---
## \#7 Posted by: lox897 Posted at: 2017-01-26T02:23:41.971Z Reads: 345

```
I believe I changed my bt module to 115200 a while back. I tried changing it to 115200 in BLDC but it didn't work. I'll reset it later
```

---
## \#8 Posted by: Zoomy Posted at: 2017-01-26T02:31:39.976Z Reads: 336

```
I bought it from here 
http://www.lillyelectronics.com/hm-10-transparent-bluetooth-4-0-serial-port-module-with-logic-level-translator

Are you supposed to do some sort of set up for it?
```

---
## \#9 Posted by: Ackmaniac Posted at: 2017-01-26T07:41:51.017Z Reads: 322

```
Do you power it by the 3.3V pin of the VESC or the 5V pin. It isn't written on the board and also not available in the description but I think it is the 3$ version from China so you should connect it to the 5V pin. The most of these boarders can handle 3.6V to 6V. So 3.3V is not enough.
```

---
## \#10 Posted by: Eboosted Posted at: 2017-02-16T04:40:08.155Z Reads: 308

```
@Zoomy did you fix the issue?, I'm having the same exact issue as you
```

---
## \#11 Posted by: Zoomy Posted at: 2017-02-16T05:52:47.128Z Reads: 303

```
Sorry no, I haven't got around to it yet. However after skimming over the replies above I noticed that @jacobbloy mentioned that the firmware from his website won't work. I must have read that as if it did.... what firmware should should work?
```

---
## \#12 Posted by: jacobbloy Posted at: 2017-02-16T06:12:57.245Z Reads: 301

```
The board needs to be on the 9600 baud rate.

Make sure you have RX and TX opposite on the vesc then to the BLE module.

You need to be running the firmware from my website that is linked in the download .exe or the DMG file.

If you are running windows the exe installer will not replace the old firmware files in your program files folder so you will need to delete them before installing BLDC Tool on your computer.

The app will tell you an error like no firmware detected if there is a problem with connection.

If you are using firmware from Chakka,enertion,maytech,DIY electric skateboards or any other custom firmware then my app will no work.

Currently I have not payed my hosting bill so my websit is down.
```

---
## \#13 Posted by: Ackmaniac Posted at: 2017-02-16T07:31:56.876Z Reads: 277

```
Is the Bluetooth module connected to the 5V pin?
```

---
## \#14 Posted by: Marty Posted at: 2017-04-25T13:41:44.445Z Reads: 259

```
By the way - does anyone know how  the values in the "Settings" page of the App are stored ?
At every relaunch I have to type in my specs (Motor pulley, diameter, Battery Type, etc) new again.
Is there a way to store it ?
```

---
## \#15 Posted by: Ackmaniac Posted at: 2017-04-25T14:55:00.916Z Reads: 256

```
Which app?
```

---
## \#16 Posted by: Marty Posted at: 2017-04-25T15:31:31.561Z Reads: 253

```
sorry I didnt specify - the "VESC Connect" App running on iOS
exact the Screenshot as in the Picture on the beginning of this topic
```

---
## \#17 Posted by: Marty Posted at: 2017-04-29T21:09:41.724Z Reads: 241

```
everytime I start the "VESC Connect" app new the settings are all over the place and I have to set them up again to get the right readings
```

---
## \#18 Posted by: rpn314 Posted at: 2017-04-29T21:21:01.084Z Reads: 246

```
I personally cannot recommend the VESC Connect app at this time. If you're on iOS, go with metr and perimetr (same developer, different purposes. Both free, but require you to purchase the bluetooth module from him, because they don't all work). On android, hand down @Ackmaniac's app. Heck, I use my android tablet, even though I'm an iOS user, because his app is that good :slight_smile:
```

---
## \#19 Posted by: Marty Posted at: 2017-04-30T12:40:57.709Z Reads: 241

```
thats for sure I like the android app as well - that would be great having on iOS.
And as I have a "normal" HC10 BLE modul I cant use the Metr app
```

---
## \#20 Posted by: rpn314 Posted at: 2017-05-02T11:51:48.353Z Reads: 237

```
Unfortunately there's no solution for you at the moment. Sorry.
```

---
## \#21 Posted by: marwa Posted at: 2017-05-10T10:52:09.071Z Reads: 219

```
Hello, i'm having trouble connecting to the android app, i'm using nrf51822 with the uart exemple but i'm afraid that the problem is caused by the firmware i'm using in my board, would you please give me the link of the appropriate firmware?
```

---
## \#22 Posted by: jacobbloy Posted at: 2017-05-10T11:51:06.517Z Reads: 213

```
Can't use an nrf board sorry
```

---
## \#23 Posted by: marwa Posted at: 2017-05-10T12:35:05.840Z Reads: 210

```
oh :( okey can i have the firmware for windows plz? not in hex form, project for keil or something like this so i can send some data to my nrf via uart
another question: cab the hc-05 bluetooth module be used?
```

---
## \#24 Posted by: Angelus Posted at: 2017-05-25T09:18:44.993Z Reads: 201

```
I have the same problem, have any solutions? Pls help Thx.
```

---
## \#25 Posted by: ZackoryCramer Posted at: 2018-02-22T08:59:49.178Z Reads: 137

```
Revive! 👻 

I got a hm-10 recently and I am having the same problem you guys described: device name “BT05”, can’t connect to app. As a programmer, I am not giving this up. I looked into the open source vesc app tools and found that they all seems to used a piece of code from “Vesc logger” 

https://github.com/gpxlBen/VESC_Logger/blob/master/VESCLogger/VESCLogger/ViewController.m

which is a partial port of the UART library for Arduino. What theoretically was supposed to happen what the iPhone is supposed to act as an arduino and the module as the “wire” connecting the tx and rx. 

What’s basically causing the problem for my case is that the UUID of the hm-10 did not match the pre-coded UUID in the app. But even after changing the device and characteristics uuid it still ran into problems receiving data. And since it was written in obj-c, I gave up finding the glitch.

I tried again by reusing my own Bluetooth connection protocol I programmed for a previous app in swift and bridged to obj-c uart data parsing functions given by “vesc-logger” It kind of worked in that I was able to transmit data correctly but only got garbage back. The data wasn’t able to be fully interpreted in the function checking the crc sum. I am not sure if the vesc is acting weird or the data parse is messed up.

If anyone has an iOS parsed library for uart hm-10 please advise sharing. 😃🙏🏻
```

---
## \#26 Posted by: ZackoryCramer Posted at: 2018-02-22T22:20:52.910Z Reads: 125

```
GUYS!!!! I figured it out!! :sob::sob::joy::joy::rofl::rofl::confetti_ball::confetti_ball:

The HM-10 module send the Vesc data in four packets and the obj-c library was interpreting the packets consecutively instead of contiguously. After I concatenated every four packets recieved I was able to successfully verify the CRC and read the bldcMeasure. :face_with_monocle::nerd_face::nerd_face: 

I'll be uploading the full demo some where in the near future in github. :cowboy_hat_face:

![42 PM|521x500](upload://eyUKr5RkLFhzpVinCEoy6jhvvRd.png)
```

---
## \#27 Posted by: DavidBanner Posted at: 2018-02-22T22:23:26.158Z Reads: 115

```
nicely done @ZackoryCramer :+1:
```

---
## \#28 Posted by: TarzanHBK Posted at: 2018-02-23T17:29:05.030Z Reads: 114

```
Buttboarder and Bugfinder!
No for real, good find :slight_smile:
(@Cobber first :hugs:)
```

---
## \#29 Posted by: muchflywow Posted at: 2018-06-15T02:52:52.847Z Reads: 95

```
so i just got the HM-10 module from longhairedboy, on the site it says to use 9600 baud rate which i tried but it won't connect. i've tried probably 10 different baud rates and not a single one works. the only app that recognizes it on my LG G5 on android 7 is VESC Connect Pro, ackmaniac's doesn't work, metr.at doesn't work. nothing connects to the module. RX is to TX and vice versa, the HM-10 just continues flashing forever, what am i missing here?
```

---
## \#30 Posted by: Eboosted Posted at: 2018-06-15T05:48:42.860Z Reads: 92

```
Samething here can't connect on any of my boards
```

---
## \#31 Posted by: muchflywow Posted at: 2018-06-16T04:21:07.436Z Reads: 88

```
i'm talking to support at LHB but they're just telling me the basics of course, we'll see if i can figure something out.
```

---
## \#32 Posted by: QGruschkof Posted at: 2018-11-27T14:11:02.250Z Reads: 50

```
Hey I have the problem that i connected my HM10 board to 5v set everythig up baud rate to 9600 and ppm and uart but as soon as i connect my phne no realt time data is coming trouth like it says esc not connected but i set everyting up
I use HW 4.12 and FW 3.40 do you have an idea
```

---
## \#33 Posted by: Ackmaniac Posted at: 2018-11-27T21:14:58.261Z Reads: 46

```
The app doesn't support 3.40 yet.
```

---
