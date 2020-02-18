# Ultimate GT2B mod - BadWolf + glow + Bluetooth VESC telemetry

### Replies: 28 Views: 4362

## \#1 Posted by: NerijusM Posted at: 2016-05-03T19:50:42.132Z Reads: 539

```
There is nothing big to say, just photos... Everyone knows how to do that, so - it works :slight_smile: 

<img src="/uploads/db1493/original/2X/f/fe85904d5825a9013317a48aa4df628ba29c02e7.jpg" width="526" height="394">

<img src="/uploads/db1493/original/2X/2/2021c1535d976272bbaabe4190d719dd288b89c4.jpg" width="666" height="500">

<img src="/uploads/db1493/original/2X/4/4ca9f75c780389167fe54bda5f2f43b90779a1dd.jpg" width="666" height="500">
```

---
## \#2 Posted by: evoheyax Posted at: 2016-05-03T20:13:49.402Z Reads: 522

```
This... is... epic!

How did you use bluetooth like that?

And do you have any reading materials about this stuff, and how to get data from the vesc for this?

I looked over the code of the vesc, but I don't even know where to begin to add code to this. My thought process would be to create a TelemetryData class, but I don't know where in the stack of vesc code to initialize it. What data should I pass to it? I really want to learn more about extending the vesc code to do more, and I've read through the uart application article that ben wrote, but other than the bit on his website, I don't know where to really start.
```

---
## \#3 Posted by: DeathCookies Posted at: 2016-05-03T20:14:21.340Z Reads: 499

```
Well, what did Display is it and from where do you  get the data?
```

---
## \#4 Posted by: NerijusM Posted at: 2016-05-03T20:28:57.229Z Reads: 490

```
There is no single modification to VESC code - everything is "outside" stuff.
Just pick UART mode in BLDC tool and you are ready to read UART port.
Im using https://github.com/RollingGecko/VescUartControl library.
There is 2 arduinos - one near VESC - gets UART data and streams over HC-05 bluetooth module.
Another - in remote - gets data and displays on OLED 0.96 screen.

There is no VESC control signal going over Bluetooth - GT2B is left stand alone for best signal.
```

---
## \#5 Posted by: evoheyax Posted at: 2016-05-03T21:01:55.557Z Reads: 473

```
How do you test your code? There's no simulator, is there? Couldn't a mistake fry the vesc?
```

---
## \#6 Posted by: NerijusM Posted at: 2016-05-03T21:12:06.721Z Reads: 458

```
Test it with arduino serial monitor.
There only read VESC - no power, no fancy connections - no danger.
```

---
## \#7 Posted by: monkey32 Posted at: 2016-05-03T21:17:05.745Z Reads: 447

```
That is beautiful -nice work
```

---
## \#8 Posted by: chipoi84 Posted at: 2016-05-03T22:09:58.940Z Reads: 441

```
You should do a "How to" guide for this. It is going to be really popular.
```

---
## \#9 Posted by: evoheyax Posted at: 2016-05-03T22:56:48.696Z Reads: 424

```
I know your solution to getting telemetry data is to use the ardino for the bluetooth proccessing, but is that necessary for a wired connection? My goal is to create an object that people can put into the firmware which is a uart app, and wire the screen directly to the uart port, creating something that can be plug and play for the community.
```

---
## \#10 Posted by: samusaki Posted at: 2016-05-30T05:30:05.583Z Reads: 380

```
Hi, How can i contact you ? I saw your topic on the VESC  in Lithuania, did you get them ? :) Have any spares?
```

---
## \#11 Posted by: NerijusM Posted at: 2016-05-30T06:02:43.826Z Reads: 365

```
Hi, i got then and sorry, dont have any spare....
```

---
## \#12 Posted by: samusaki Posted at: 2016-05-30T06:10:51.428Z Reads: 362

```
Well, it might sound silly, but i can't figure out how to pm you :D Maybe its because of my entry level account in this forum ?
```

---
## \#13 Posted by: chipoi84 Posted at: 2016-05-30T06:33:37.516Z Reads: 351

```
Click on the username of the person, and then click on "message".
```

---
## \#14 Posted by: samusaki Posted at: 2016-05-30T06:37:38.990Z Reads: 341

```
Now its available, But first you have to get GRAND BASIC badge. Thanks !
```

---
## \#15 Posted by: kyo Posted at: 2016-05-30T06:46:02.667Z Reads: 358

```
@NerijusM 
Hi great work. Looks awesome. Few questions though

- did you test the bluetooth connecttion? Any dropout during the ride?
- let say it did dropout or lost connecttion, does the board still run? Or does it reconnect automatically ?

Really appriciate that you would make a know-how doc for this.
```

---
## \#16 Posted by: NerijusM Posted at: 2016-05-30T16:08:16.177Z Reads: 351

```
BT is only for telemetry data.
Board controler is GT-2B 2.4ghz. I use both in one case.
```

---
## \#17 Posted by: mason Posted at: 2016-05-31T02:28:13.650Z Reads: 350

```
this is too kick ass. I need a tutorial.
```

---
## \#18 Posted by: hamminitup Posted at: 2016-05-31T02:46:15.970Z Reads: 344

```
This is amazing. Would love a guide or an overview! :grin:
```

---
## \#19 Posted by: kyo Posted at: 2016-06-01T08:10:29.839Z Reads: 329

```
@NerijusM 
2 types of connection its kinda redundant dont you think? Why dont you do it with just one ? Beside it costs a bit more.
```

---
## \#20 Posted by: oripaamoni Posted at: 2016-11-12T18:30:01.891Z Reads: 234

```
THIS IS AWESOME! great work! Love the relibility on the GT2B for control, this completes it. Would you be willing to share the source code for both the sketches?
```

---
## \#21 Posted by: tueboard Posted at: 2016-12-19T00:24:19.879Z Reads: 203

```
that's really impressive! i wanted to do something like that, do you will share some step by step guide? or are you planning to sell it?
```

---
## \#22 Posted by: num3a Posted at: 2017-01-02T23:06:33.680Z Reads: 184

```
Are you using an Arduino Nano, connected to the GT2B battery ?

Did you have to increase the remote size to put the arduino inside ?
```

---
## \#23 Posted by: Shogu12 Posted at: 2017-01-03T17:04:24.332Z Reads: 180

```
I'm thinking about doing something similar but complete bt control via raspberry pi zero and an oled display.
```

---
## \#24 Posted by: num3a Posted at: 2017-01-12T15:18:34.670Z Reads: 172

```
Hello, 
Did you have to modify the remote case ? Is there any space to add an arduino, a HC-05 module and the screen ?
Can you post a picture of the remote internals please ?
```

---
## \#25 Posted by: ElskerShadow Posted at: 2017-03-27T15:04:51.901Z Reads: 145

```
Do you plan to do something with it ? Give it to the community ? or sell it ? Really looking forward to copy your remote. it's amazing work
```

---
## \#26 Posted by: ElskerShadow Posted at: 2017-03-27T15:19:27.974Z Reads: 143

```
[quote="NerijusM, post:1, topic:2864"]
Everyone knows how to do that, so - it works :slight_smile:
[/quote]
Actualy not everyone :stuck_out_tongue:
```

---
## \#27 Posted by: NAF Posted at: 2017-07-05T17:05:13.351Z Reads: 94

```
Any plans on selling these to the community ?
```

---
## \#28 Posted by: notger Posted at: 2017-07-07T20:01:51.377Z Reads: 79

```
Oh yes asolutely !! also interested in such a thing, but not smart enough to build it by myself ;-(

if, i'll take one

notger
```

---
