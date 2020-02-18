# VESC Monitor - Android App

### Replies: 15 Views: 2640

## \#1 Posted by: Pimousse Posted at: 2016-11-01T15:46:04.955Z Reads: 279

```
Hi all !

"VESC Monitor" is an Android app which is available for free on [Google Play](https://play.google.com/store/apps/details?id=de.solarturtle.vedder_monitor&hl=en).

https://cdn.apkmonk.com/images/de.solarturtle.vedder_monitor.png

As a beta-tester of this app, I would like to open a specific thread for this app in order to collect your issues, questions, features requests, etc.

Currently, the app does :
- Display lives data from VESC
- Record data from VESC in .txt file
- Allow to select which data are displayed live

We're working on other features as well :
- CRC checking (the app makes sure that data received are not corrupted)
- Notifications 

I also created a Excel worksheet that you can use for analyze .txt generated log files with automation script (macro).
It's still in development but it allows to know a lot from a ride (speed, current, etc.) 
https://www.dropbox.com/sh/sgleis0aayzgbj3/AACZzOVOljwZQmvP2tnKlgQRa?dl=0

I'm not sure that the developer wants to release it open-source.
But anyway, I'm pleased to participate to this app project.

I'll keep this thread up-to-date this the latest news ! :wink:
```

---
## \#2 Posted by: Michael319 Posted at: 2016-11-01T15:49:06.246Z Reads: 231

```
Can it edit parameters for the VESC?
```

---
## \#3 Posted by: Pimousse Posted at: 2016-11-01T15:49:58.956Z Reads: 225

```
Unfortunately, no.
As the title of the app says, it's only monitoring.
```

---
## \#4 Posted by: Michael319 Posted at: 2016-11-01T15:54:27.781Z Reads: 214

```
Ah, got it, will still definitely try it out!
```

---
## \#5 Posted by: PB1 Posted at: 2016-11-01T15:56:34.008Z Reads: 220

```
Hello @Pimousse
just as a FYI, there is already a thread discussing this tool and VESC logging in general. 
http://www.electric-skateboard.builders/t/recording-data-from-vesc-summary-of-tools/7020/9 

However I suppose that this VESC logger is important enough and deserves a thread of its own ... 

Are you part of the development team? How do features requests get to the developers? 


And yes, I do have a feature request: 
- I would like to see some sort of timestamps in the log file so we are able to correlate the VESC data to other data, e.g. from a GPS tracking device
```

---
## \#6 Posted by: XIII Posted at: 2016-11-01T16:24:46.818Z Reads: 188

```
Where do you buy/ How do you make the bluetooth module? 
Is it mentioned in the thread you linked ? 

Regards
```

---
## \#7 Posted by: PB1 Posted at: 2016-11-01T16:41:07.329Z Reads: 189

```
yes it's mentioned. Here a short recap.  
- least expensive is a HC-05 bluetooth module. I got mine from dx.com (around 6 USD + free shipping but slow)
- you need to make a cable with the following connections

HC-05  - VESC UART Port
VCC - - -  3,3V
GND - - - GND
RX  - - -  TX
TX  - - -  RX
leave the other pins

Then enable "PPM and UART" in the VESC, set the baud rate to 9600 and do a VESC reboot. Voila...
```

---
## \#8 Posted by: XIII Posted at: 2016-11-01T17:12:46.099Z Reads: 174

```
Great ! Thanks! 
I have a HC-05 module from an other project :)
```

---
## \#9 Posted by: Pimousse Posted at: 2016-11-01T17:13:44.824Z Reads: 180

```
Yeah, I know this thread. It's a very good one afterall, I often visited it.
However, I was thinking the app deserves a whole topic because I could let people know how the dev is going and collect easier your feddbacks. :wink:

There are some HC05 module working in 5V (better for using it directly).
And RX of the BT module needs voltage divider because VESC UART level is 5V.
See a tutorial for connect the HC05 module (works also with a HM10) (sorry, it's in french, but drawings could help):
http://www.e-sk8.fr/forum/viewtopic.php?f=8&t=1126

I programmed mine for 115200 speed and custom name and pin.
```

---
## \#10 Posted by: PB1 Posted at: 2016-11-02T09:11:01.139Z Reads: 157

```
Tracked my 20min run home from the office. First flat, then mostly steep uphill. It was pitch dark so took it easy :-) . 
Note that I'm running a dual setup, the numbers are for one VESC only. Speed is calculated using ERPM, gearing and wheel size. 

I'm getting some good information out of this already. In the picture below you can see the min and max values and the graphs of some values. Produced by excel. The top light green curve is the mosfet temperature. 
Unfortunately correlation to GPS data for location is missing and not possible yet (hint!!). 
<img src="/uploads/db1493/original/3X/e/d/edd87712fe2c8b7584bd0c7e80d7cf699cc8800d.PNG" width="690" height="195">
```

---
## \#11 Posted by: Pimousse Posted at: 2016-11-02T09:30:38.507Z Reads: 146

```
Did you use my Excel sheet ? Or yours ?

EDIT : it seems to be yours.
Can you have a try with mine and see if you get werid values or other issues ?
For speed calculation if find that matching max ERPM with max speed recorder by an app (like Runtastic or Endumondo) is quite more accurate than calculate the ratio with gear and wheels dimensions.
(You can select either calculation or GPS ratios)
```

---
## \#12 Posted by: PB1 Posted at: 2016-11-02T11:08:43.931Z Reads: 133

```
I used mine as I already had it for some other stuff. 

Did download yours and tried - but I get weird values. 
Your excel tool looks very sophisticated and I can use some stuff. Looks like the sampling rate of the app is 0.2 seconds, correct? Also GPS ratio is nice. Need to do a calibration of my setup. 
I will PM you a link to my raw data txt file, maybe you can get it running and it might help you in fixing the app. Let me know what the issue was. My setup uses 13 / 36 gearing, 90mm wheels, big r-spec so 7 poles. 

btw, I'm using my HC-05 without voltage divider and it seems to work.
```

---
## \#13 Posted by: Pimousse Posted at: 2016-11-02T11:14:16.449Z Reads: 128

```
Which values are weird ?
If it's distance and speed (using calculated ratio), it's normal.
I can't find the exact ratio between ERPM and mechanical rotation even using Vedder formula...
I have to spend more time on it.

Anyway, I'm interesting into your raw file. :wink:
```

---
## \#14 Posted by: Bataleon Posted at: 2017-04-23T08:36:52.668Z Reads: 91

```
@Pimousse, I've been using this app for a while now (as I don't have a Bluetooth LE module) and it works great.

I have noticed two bugs in the current version. Would you be able to pass them on to the developer? I tried emailing them but got no response.

All testing was does on a Nexus 5X running Android 6.0.1

**Bug 1:**
The app disconnects from the BT module when the screen orientation changes (I have locked my screen to portrait mode to stop this).

**Bug 2:**
The _battery current_ and _motor current_ readings are always exactly the same value.

Hope this feedback is useful, and a massive thanks to the developer for all their hard work.

P.S. Your analysis Excel spreadsheet looks great, however, I'm unable to import a log file (see the error screens below). I'm running Office 365 on OS X which I know has less features than the Windows version, so it could be that?

Cheers

<img src="/uploads/db1493/original/3X/1/f/1fd1f94a2366c0023394a7f57a4aedf3b34f07e8.png" width="690" height="283">
<img src="/uploads/db1493/original/3X/e/5/e5564744c86132b2b62dc15063e47442be10ec0f.png" width="690" height="495">
```

---
## \#15 Posted by: Pimousse Posted at: 2017-04-23T09:41:59.484Z Reads: 77

```
Sorry, but the developer gave up with his project.
So, sorry but you'd better get a BLE module and enjoy Ackmaniac app instead. ;)
```

---
