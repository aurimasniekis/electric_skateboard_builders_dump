# Recording data from VESC? Summary of tools

### Replies: 49 Views: 9279

## \#1 Posted by: evoheyax Posted at: 2016-08-02T18:01:54.899Z Reads: 434

```
Wondering if anyone's come up with a way of recording data from your VESC with out having to hold a laptop that's wired to your VESC and recording the screen (which is what I did once)? My method worked, and I have pretty graphs, but it's too risky riding with a laptop and wires and all.

I was thinking if there was some code running on the VESC that recorded this data to a USB thumb drive, attached via a USB single to the USB port on the VESC. Something simple like that which can save data without a laptop.
```

---
## \#2 Posted by: mcfly777 Posted at: 2016-08-02T18:13:38.113Z Reads: 436

```
+1. I have tried to have the UART work but no luck so far. Ideally if I can program something like an [open logger](https://github.com/sparkfun/OpenLog) to collect these data that would be awesome. I have one of these, just couldn't make the system work at all with the VESC.

Leo
```

---
## \#3 Posted by: evoheyax Posted at: 2016-08-03T02:49:01.515Z Reads: 406

```
Do you know what files/classes this data flouts around in? I want to try to write something to log data, but the structure of the vesc code confused me (could be because I need to learn c, but that's why I'm taking parallel programming this fall).

Do you know where to find more documentation on the vescs code structure? I found only little pieces here and there on vedders site.
```

---
## \#4 Posted by: racidon Posted at: 2016-08-03T02:58:27.588Z Reads: 386

```
has anyone thought of maybe using a PC Stick or NUC?
```

---
## \#5 Posted by: evoheyax Posted at: 2016-08-03T03:04:54.313Z Reads: 383

```
[quote="racidon, post:4, topic:7020"]
PC Stick
[/quote]

I need to research those more, but that sounds like a good idea. I was hoping for a cheaper option though.
```

---
## \#6 Posted by: mcfly777 Posted at: 2016-08-03T03:08:04.047Z Reads: 379

```
Here's what Vedder says about UART comms

http://vedder.se/2015/10/communicating-with-the-vesc-using-uart/

Also, in terms of implementation it would be nice to have a bluetooth or wifi module sending data to a mobile phone app or maybe directly to open logger SD card.

Leo
```

---
## \#7 Posted by: evoheyax Posted at: 2016-08-03T03:10:46.024Z Reads: 373

```
have you seen what @jacobbloy did with the bluetooth module and iphone app? That might just be the solution.

I just need to see what's going on while I'm riding and watt meters are too hard to read while going 25+ mph. A phone in my hand is more reasonable.
```

---
## \#8 Posted by: mcfly777 Posted at: 2016-08-03T03:14:26.514Z Reads: 404

```
Yes I have seen that. That would be good. I don't need to have a real time view, I really don't want to check my phone going 30 mph :slight_smile:. All I want is for it to record the data (and possibly export it) for later review.

And here's a library that communicates with the VESC using an Arduino
https://github.com/RollingGecko/VescUartControl

Leo
```

---
## \#9 Posted by: PB1 Posted at: 2016-09-11T20:09:31.566Z Reads: 376

```
while discussing option for VESC data logging we collected a lot of information in another thread. Now we would like to make this information acessable for everybodey. So here it goes, the current summary of VESC data logging options. Thanks a lot to @makevoid for compiling a lot of the information and investing his time so far!

**@makevoid Arduino SD Data Logger - OpenSource**
Hardware: 
-	Arduino connected to VESC via UART
-	Standard SD Card shield

Code:
-	https://github.com/makevoid/VescUartControl/blob/master/examples/VescUartSample/VescUartSample.ino

This code logs data in a JSON time series format.

Power the arduino off the VESC or use a common ground. The code runs on the Arduino device and pulls the data out of the VESC. The data is then stored on a standard SD card shield connected to the arduino. You need to set the VESC to ppm + uart mode and you only get the right data if the controller is on and connected.
If you want to analyze the data, the SD card needs to be removed. You can then analyze the data either using the JSON data to GIF generator or the graph tool mentioned below. 
If there are enough requests, makevoid might add a CSV format as output. 

*******************************************

**@makevoid JSON data to GIF generator - OpenSource**
@makevoid also made a program that takes the JSON time series and generates a text gif to embed in videos 
Code: 
-	https://gist.github.com/makevoid/d68a4e95ba518cc84ed584afe2445f1d

The program runs on Linux, opens the log file VESC_LOG.TXT and creates a GIF image based on the data in the log file. This image can be included in videos.

***************************************************************
**@makevoid JSON to graph app** to make video overlays
Software: 
- https://github.com/makevoid/vesc-logged-data-overlay

************************************************

**gpxlBen VESC data logger to iOS – OpenSource**
Hardware: 
-	adafruit ble uart chip connected to VESC (e.g. https://www.adafruit.com/product/2479)
-	iOS device

Code: 
-	original code by gpxlBen - https://github.com/gpxlBen/VESC_Logger 
-	fork by @makevoid - https://github.com/makevoid/VESC_Logger

The adafruit chip is connected to the VESC via UART and forwards the serial data to an iOS device. The program runs on the iOS device, no change needed in the VESC firmware. Set the VESC to ppm + uart mode. You only get the right data if the controller is on and connected.
You need somebody with a mac and XCode to compile the code for you and create the iOS app. 
The original app shows VESC values but does not logging (yet). 
The fork by makevoid added code to do logging as well.

*********************************************

**solarturtle vedder esc monitor - Android app**
Hardware: 
-	serial port to bluetooth connector ( e.g. HC-05 https://www.amazon.co.uk/gp/product/B013STJSES/ref=oh_aui_detailpage_o00_s00?ie=UTF8&psc=1) 
-	Android device

Install the app via Google Play, connect the HC-05 to the VESC via UART. The HC-05 forwards the serial data to the android device. Set the VESC to ppm + uart mode. You only get the right data if the controller is on and connected. The app on the device shows real time and peak values. Logging to file possible, Excel format (to be verified)

***********************************************

**Traction app  - for iOS and android**
hardware: 
- serial port to bluetooth connector (E.g. HC-05)

Code:
- https://github.com/bchiu/Traction 

Dashboard app for electric vehicules, similar to solarturtle app, looks very advanced.
```

---
## \#10 Posted by: makevoid Posted at: 2016-09-11T21:12:39.080Z Reads: 326

```
Some screenshots and notes about the 3 apps:

**gpxlBen (iOS):**

<img src="/uploads/db1493/original/3X/f/0/f025ad0c9fef83f26b06f3d7a1ab19f688fa2ea8.png" width="666" height="500">

has nice graphs and logging to file on my branch - somebody could compile it and release a beta on tesflight for users of this forum

---

**Solarturtle (Android): [[DL LINK](https://play.google.com/store/apps/details?id=de.solarturtle.vedder_monitor&hl=en)]**

<img src="/uploads/db1493/original/3X/7/c/7ceee9c39c8e9c0493525413596cd0784a42c806.png" width="281" height="500">

(not open source, we could contact the developer and ask if he wants to release it as open and maybe support him with some donations? or make the Traction app work then we have an app for android already and we don't need this - the upside is that it can be downloaded without compilation as it's already published on the google play store)

---

**Traction:**

http://www.electric-skateboard.builders/uploads/db1493/optimized/3X/e/9/e9a21665c7faa731679d48196adbc78416b19f23_1_690x388.png

the code seems really well done but the current version seems to display only the mosfet temp (the one in the screenshot above labeled as Drive T) out of the box, as all the data it's sent together it shouldn't be too difficult to display (and log to file) the other data as well... I will attempt to do it next week...

---

an useful link: [amazon search of hc-05](https://www.amazon.com/s?ie=UTF8&field-keywords=hc-05&index=blended)

---

demo video using gpxlBen app ([json logfile fork](https://github.com/makevoid/VESC_Logger)) + the [ruby sdl2 tool](https://github.com/makevoid/vesc-logged-data-overlay) to make the video

https://www.youtube.com/watch?v=bxSrCjUnLUc
```

---
## \#11 Posted by: Ackmaniac Posted at: 2016-09-11T22:28:16.124Z Reads: 299

```
That is written for a ESP8266 (Wemos mini D1). So my board has it's own wifi. If anybody wants to have the code i can share the scetch for the ESP and the android apk.

<img src="/uploads/db1493/original/3X/8/1/810cc9cbf28ae5a756a575cf727c94a6b926cddf.png" width="281" height="500">
```

---
## \#12 Posted by: ra.rend Posted at: 2016-09-15T13:50:38.634Z Reads: 285

```
I have the HC-05, do you connect all 6 pins to the vesc? Could you show me a picture of where its connected to the vesc? Sorry I have no knowledge or experience of anything on this forum besides skateboarding, but I'm willing to learn more about electronics. Thanks.
```

---
## \#13 Posted by: devin Posted at: 2016-09-15T14:34:39.670Z Reads: 282

```
<p>This post was flagged by the community and is temporarily hidden.</p>
```

---
## \#14 Posted by: makevoid Posted at: 2016-09-15T14:52:09.900Z Reads: 285

```
You have to connect the HC 05 pins to the UART pins on the VESC

    HC05 --- VESC
    VCC - - -  5V
    GND - - - GND
    RX  - - -  TX
    TX  - - -  RX 

leave the other pins unconnected 

You can use the VESC 3.3V pin as well
```

---
## \#15 Posted by: makevoid Posted at: 2016-09-15T14:55:59.605Z Reads: 276

```
If you have a mac and xcode you can download the project and build it on your device, otherwise you can pm your UDID via pm  and I can send you a compiled app
```

---
## \#16 Posted by: evoheyax Posted at: 2016-09-15T15:21:31.939Z Reads: 270

```
Your in luck because I'm getting my developer account again today and will be putting it in the app store. I have 15 of the adafruit bt chips on their way and I will be soldering them up with plugs. I'm planning in the near future to find time to work on some new apps for this chip.
```

---
## \#17 Posted by: ra.rend Posted at: 2016-09-15T15:34:34.986Z Reads: 264

```
thank you!
```

---
## \#18 Posted by: devin Posted at: 2016-09-15T15:50:36.655Z Reads: 268

```
<p>This post was flagged by the community and is temporarily hidden.</p>
```

---
## \#19 Posted by: evoheyax Posted at: 2016-09-15T15:53:37.643Z Reads: 273

```
I can't make any promises of when it will be in there though... I've never submitted an app before, and I hear the process can be grueling... so we shall see. But I already renewed my developers license and in the proccess of enter the massive amount of info they want, haha.
```

---
## \#20 Posted by: ra.rend Posted at: 2016-09-15T18:41:22.563Z Reads: 289

```
I have everything hooked up but the VSC monitor app (solarturtle) isn't displaying anything (everything still at 0). Im on android btw. Its also already paired to my phone. In bldc tool, its set to ppm+uart. 
Just to make sure it's wired properly:

hc05 -- vesc
5v      -  5v
GND - GND
rx      - tx
tx      - rx

is that correct?

Do I have to configure the Bluetooth module first or will it work out of the box?
```

---
## \#21 Posted by: makevoid Posted at: 2016-09-15T19:56:00.122Z Reads: 281

```
I believe you also have to set the correct baud rate in the uart tab, I can't remember if it's 9600 or 115200. Also you may want to switch to Uart only and test, then try to switch to Uart+ppm again which requires you to have the controller connected and on.
```

---
## \#22 Posted by: PB1 Posted at: 2016-09-15T20:19:08.866Z Reads: 280

```
hello @ra.rend

I'm still desperately waiting for my bluetooth module, grrrrrr

So can't speak out of experience yet. However: baud rate of the bluetooth module and settings in the VESC have to match. Also, I think if you change from PPM to ppm+uart you need to reboot the VESC. 
On the bluetooth module you can change the baud rate using AT commands, for the VESC you can change it in the BLDC tool. Google HC-05 baud and at commands ...
```

---
## \#23 Posted by: ra.rend Posted at: 2016-09-15T20:46:35.588Z Reads: 268

```
@makevoid it's 9600. It works now. Thank you so much for your help. 
@PB1  I wasn't getting any reply from the module, while using Bluetooth terminal (I know nothing about this), but I just changed baud rate in bldc and it works! Thanks guys!
```

---
## \#24 Posted by: lox897 Posted at: 2016-10-10T10:04:34.839Z Reads: 244

```
Just to confirm, you can use the HC05 module with the vesc vision app? Or is it just the adafruit chip? @makevoid @evoheyax
```

---
## \#25 Posted by: evoheyax Posted at: 2016-10-10T15:18:12.674Z Reads: 232

```
It's unclear, it has yet to be tested as far as I know. But if someone has an HC05 and would like to test it...
```

---
## \#26 Posted by: makevoid Posted at: 2016-10-10T23:09:06.101Z Reads: 227

```
You need the adafruit bluefruit, unfortunately it's a bit more expensive than the HC05 and if you want to switch from an ios device to an android one (traction app or vsc app) you need to disconnect one and then connect the other


edit: Jacob's app uses the HM-10
```

---
## \#27 Posted by: lox897 Posted at: 2016-10-11T09:08:39.961Z Reads: 222

```
I think I will use HC05 with Jacob's app then.
```

---
## \#28 Posted by: makevoid Posted at: 2016-10-11T10:29:07.351Z Reads: 213

```
sorry I edited the post to correct it, Jacob's app uses hm-10 module (almost as cheap as the hc-05)
```

---
## \#29 Posted by: lox897 Posted at: 2016-10-11T10:42:00.226Z Reads: 214

```
I asked Jacob and he thought that it could work. Why wouldn't it work?
```

---
## \#30 Posted by: makevoid Posted at: 2016-10-11T10:53:37.236Z Reads: 215

```
then great, when I tried it was not working with the HC-05 but both VSC and Traction were working, but probably it was something else!
```

---
## \#31 Posted by: lox897 Posted at: 2016-10-11T10:54:02.649Z Reads: 215

```
Baud rate maybe? EDIT: Tried to compile traction with xcode. Didn't work. Any chance you could send it to my UDID? @makevoid
```

---
## \#32 Posted by: makevoid Posted at: 2016-10-11T11:38:18.269Z Reads: 215

```
You mean you compiled [VESC_Logger](https://github.com/gpxlBen/VESC_Logger) ? [Traction](https://github.com/bchiu/Traction-reactjs) is a cordova app. Also I don't have a machine with OSX at the moment (gf took the laptop on a trip), did you get a compilation error or another error? on my machine it compiled straight away
```

---
## \#33 Posted by: lox897 Posted at: 2016-10-11T19:03:08.725Z Reads: 210

```
Oh right. I'll follow this guide: http://codingsquare.blogspot.com.au/2013/08/setting-up-apache-cordova-ios-project.html?m=1
```

---
## \#34 Posted by: makevoid Posted at: 2016-10-12T07:17:56.486Z Reads: 206

```
btw Traction is not complete, with the current version it only displays data on the battery voltage gauge, the other data is there but it needs to be renamed/connected to the UI elements I believe, it shouldn't be hard but it can be a bit tricky (add console.log statements on react components render method, open chrome with remote  device debugging, check that the data gets rendered, choose another value/gauge, repeat)  ^^
```

---
## \#35 Posted by: lox897 Posted at: 2016-10-12T07:48:42.386Z Reads: 208

```
Thanks so much for helping me man! I am getting a few errors: <img src="/uploads/db1493/original/3X/8/d/8dd4991fa92dbd111e1fb4613791e0f182ae0d56.jpg" width="375" height="500">

I think this may have to do with the version of cordova
```

---
## \#36 Posted by: lox897 Posted at: 2016-10-12T08:02:06.458Z Reads: 204

```
Quickly googled it. Seems I've fixed it. Can't express my gratitude man! Thanks so much for the help @makevoid

<img src="/uploads/db1493/original/3X/4/9/49f64ad08d5f98539ea40b11274b98183bdd53b9.png" width="690" height="388">
```

---
## \#37 Posted by: ra.rend Posted at: 2016-10-21T02:01:18.493Z Reads: 203

```
Hi, I'm trying to read data from vesc over uart (voltage, rpm etc...) and print it on the serial monitor   of Arduino IDE. How do I do that?

I have an arduino uno connected to the VESC via uart. Assuming that I got the VESC library for arduino already included, what line of code will "get" the rpm, inpvoltage etc...? 

My coding skills: I took one java class in high-school  :sweat_smile:

Any information would be great. Thanks!
```

---
## \#38 Posted by: makevoid Posted at: 2016-10-21T07:23:47.438Z Reads: 201

```
Check out this arduino sketch/script https://github.com/makevoid/VescUartControl/blob/master/examples/VescUartSample/VescUartSample.ino#L76

That's the line that gets data from the vesc, I suppose you're using the same VescUartControl library, if so you can start with the original example or modify mine (if you don't have a sd card module you'll need to delete/comment some lines)

If you already have an sd card module that example should work straight away
```

---
## \#39 Posted by: ra.rend Posted at: 2016-10-22T00:56:48.476Z Reads: 200

```
Does the code: "SerialPrint(values); " print the rpm, voltage, etc? Like in one single String? Sorry for the noob questions. Should I post this in the noob question thread?
```

---
## \#40 Posted by: makevoid Posted at: 2016-10-22T01:05:22.327Z Reads: 202

```
That's fine, you can use Serial.println to write to the arduino console, logfile.println writes to the log file
```

---
## \#41 Posted by: ra.rend Posted at: 2016-10-22T04:09:14.730Z Reads: 194

```
I ran the sample code by RollingGecko, and it's not receiving any data from the VESC. Could it be a hardware issue? Btw I can pull data using hc05 Bluetooth module over uart with the VSC Monitor app. So maybe my arduino's serial port isn't working or not supported? In the VescUart.h file, there's only "avr atmega2560" and "avr nano" (I have the atmega328p).
```

---
## \#42 Posted by: PB1 Posted at: 2016-10-26T08:56:11.613Z Reads: 188

```
Some updates on this topic. 

The Solarturtle **VESC Monitor App** for Android available in the Play Store has been updated. The new version now allows to configure the visible elements and you can switch logging on or off. It also includes some bug fixes. 
Works fine with the cheap HC-05 board. Logging is also working for me but I haven’t tested this extensively (it’s raining cats and dogs). 
Biggest drawback with logging is the absences of any time stamps and sampling rate is unknown too. So while you can analyze the logging data using e.g. Excel you can’t correlate it properly to your ride. 

The app mentions a web site to donate via PayPal. www.vesc-monitor.de 
I’ve donated some $ and sent a notification to the developer with a link to this post here. Maybe he will join us :blush:

In my opinion this app is the easiest way to get real time VESC data on android, even though it lacks some advanced features. And some time stamps would be nice :heart_eyes:

*********************


I’ve also  managed to compile the **Traction** app under Windows. It also connects to my HC-05  and shows data. As @makevoid mentioned, the app looks very promising but needs some tweaking. Biggest drawback is the lack of configuration in the app itself. You need to configure it in your development environment and then re-compile it. 
So not an easy win for most people but a good starting point for somebody who wants to develop a nice app. 
Need to do some further tweaking and testing myself but needs a lot of time as the dev environment has to be set up properly. 
***************

I wasn't successful either in connecting Jacobs VESC Connect app to my HC-05. Looks like this app does expect a Bluetooth Low Energy devices. Waiting for my HM-10 ... 
The app has similar functionality as the BLDC tool with the ability to change the VESC settings. So great for those who want to adjust their settings while on the road. 
****************

Haven’t tested the @evoheyax app yet but looking forward to it.
```

---
## \#43 Posted by: lox897 Posted at: 2016-10-26T09:08:15.808Z Reads: 167

```
Hey @PB1 , I too have compiled Traction and have it on my phone. I am also working on porting the vedder esc monitor android app to iOS using google's j2objc. Any thoughts on this?
```

---
## \#44 Posted by: PB1 Posted at: 2016-10-26T09:23:50.292Z Reads: 163

```
Actually: not many thoughts on this ... as I'm an Android person ;-)

However, did you get the vedder esc monitor apps source code or did the guy even make it open source? 

Regarding Traction, did you manage to display all of the data or just compile it?
```

---
## \#45 Posted by: lox897 Posted at: 2016-10-26T09:28:18.954Z Reads: 162

```
I converted the apk to java files. Now just trying to figure out j2objc. I only have the battery voltage working. I think I will wait for the author to complete it because I don't know how to code haha
```

---
## \#46 Posted by: PB1 Posted at: 2016-10-26T09:47:23.118Z Reads: 168

```
ok, maybe you should contact the developer of the vesc monitor app for the source files. The email address mentioned in the google play store is solarninjaturtle (at) gmail.com . 
You will still need to code the iOS specific part, e.g. User Interface. So some coding will be needed, a good start if you want to learn .... 

Not sure if the author of the Traction app is still working on it, the latest updates are from Nov 2015. 

Btw, I'm no programmer either, haha
```

---
## \#47 Posted by: lox897 Posted at: 2016-10-26T09:49:35.057Z Reads: 166

```
@PB1 I guess I will have a go, maybe I can use cydia and install a java simulator on my phone.
```

---
## \#49 Posted by: celinehedson Posted at: 2017-10-08T09:15:38.318Z Reads: 85

```
Id love to have it. Got the wemos at home here lol.
```

---
## \#50 Posted by: drew Posted at: 2017-10-09T12:45:31.476Z Reads: 83

```
Hi, could you please send me a link to this code? Are you using the RollingGecko lib? i cant get UART between the vesc and the esp8266 to work. the command to request the data is sent to the vesc as shown on the oscilloscope. but the vesc is not responding.

i am on FW3.26 and the RollingGecko lib seems not working anymore for the new UART Interface. I also tried the version from the vesc 6 branch, which seems to be compatible to the new interface, but i cant find the source code from vesc FW3.26  to verify the protocol  version used. 

is your sketch working for FW3.26? 

thanks in advance, 

drew
```

---
