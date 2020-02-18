# Android Smartphone Remote/Receiver (Open-source! w/Nunchuck Conversion)

### Replies: 20 Views: 4407

## \#1 Posted by: VladPomogaev Posted at: 2016-07-19T10:40:45.279Z Reads: 261

```
<img src="/uploads/db1493/original/2X/8/8eb7fbfdbaf72d5a3767787608ac924eaebe4e21.jpg" width="689" height="461">

I recently open-sourced my entire smartphone remote/controller application and receiver project. With this receiver, you will be able to provide your ESC with a signal to control the speed using an **Android** smartphone. While a smartphone is not the most durable controller for an electric skateboard, it adds a very convenient way to control the speed, which is very nice for any commuter e-skate builds. Here are some of the specs:

* Standard Bluetooth Transceiver (not BLE)

* Based on the Arduino platform

* Voltage display up to 6S (30 volts)

* Range is 30 feet

* Signal loss detection (slow to a stop, or slowly release brake)

I tried to mass-produce these after getting an influx of viewers on my [YouTube channel](https://www.youtube.com/user/comsa42) (where I have three e-skate builds/tutorials), but I could never refine the technology enough (I really wanted to use Bluetooth Low Energy, but the software for it was too expensive), so I decided to open-source my controller [**here**](http://www.instructables.com/id/DIY-Nunchuck-Controller-for-Electric-Skateboards/step7).

If anyone really wants to make this controller, I would be willing to sell some parts and prototype PCB's for it. Just drop me a message on YouTube. Also, I have converted a Wii Nunchuck to be used with this controller, and I have another Instructable on it [here](http://www.instructables.com/id/DIY-Nunchuck-Controller-for-Electric-Skateboards/).

Enjoy,

Vlad (comsa42)
```

---
## \#2 Posted by: jrpwit Posted at: 2016-07-20T03:25:32.575Z Reads: 211

```
http://www.electric-skateboard.builders/t/elesk8-receiver-the-receiver-that-makes-your-iphone-into-a-controller/
[quote="longhairedboy, post:4, topic:3348"]
for most of us, that's not a problem that needs fixing. The reason we use GT2Bs, GT2B clones, steez remotes, and other 2.4GHz FHSS remotes is because bluetooth and wifi are notorious signal droppers and prone to being jammed both intentionally and unintentionally. You really want that happening when you're doing 20+ mph down a bike lane?
[/quote]

Also the wireless Wii nunchuks such as the cheap Kama Wireless Controller can be connects the the vesc very easily to be used as a remote. But these nunchuks too can drop out at high speeds.
```

---
## \#3 Posted by: mason Posted at: 2016-07-20T03:44:28.921Z Reads: 192

```
this.

It is a good idea in theory, but in real world performance it lacks reliability.
```

---
## \#4 Posted by: VladPomogaev Posted at: 2016-07-20T05:27:27.030Z Reads: 183

```
I have **never** had any connection problems with this controller. Even if it does lose connection or get jammed (most of the time to long range operation), the software disconnects at the slightest loss of packets. 

Both Bluetooth and WiFi operate on a 2.4Ghz frequency (although the way they send data is fundamentally different), so they are not more susceptible to being jammed or interfered than with an RC remote. Saying that they are "notorious signal droppers" is a big stretch, as Boosted Boards and other electric skateboard manufacturers rely on Bluetooth for their remotes.

I think that my receiver is far more reliable than you guys think, and any connection problems you may have with other Bluetooth receivers tend to boil down to shoddy electronics or improper software handling of a signal-loss.
```

---
## \#5 Posted by: Pantologist Posted at: 2016-07-20T05:31:20.594Z Reads: 167

```
A bunch of Boosted owners complain about connection issues in some parts of their cities.

Oh and.... welcome!
```

---
## \#6 Posted by: jrpwit Posted at: 2016-07-20T05:56:03.235Z Reads: 157

```
I'm just restating what others have said. I actually use the nunchuk cause I like cruise control with the vesc. Many others agree that it is good but for speed it can drop out. But I am probably going to get a new remote when the vesc v6 comes out so I get a higher erpm.
```

---
## \#7 Posted by: XIII Posted at: 2016-07-20T13:04:39.028Z Reads: 152

```
[quote="VladPomogaev, post:4, topic:6328"]
I think that my receiver is far more reliable than you guys think, and any connection problems you may have with other Bluetooth receivers tend to boil down to shoddy electronics or improper software handling of a signal-loss.
[/quote]

I back this completely, I used his design for my smartphone controlled longboard. Only lost connection 5 times where my board proceeded to coast and could establish connection again in 3 seconds after noticing. 

The only reason i changed to a real remote is: My smartphone is expensive. when braking you have to look at your screen to see where your finger is (already braking , still not passed neutral point, etc)
```

---
## \#8 Posted by: DeathCookies Posted at: 2016-07-20T13:11:04.864Z Reads: 137

```
[quote="XIII, post:7, topic:6328"]
could establish connection again in 3 seconds after noticing.
[/quote]

Wow that is lots of time! Many bullshit can happen in 3 seconds. For me it would be to unsafe... i would not risk it with the knowledge that i cannot break for three seconds...
```

---
## \#9 Posted by: XIII Posted at: 2016-07-20T13:21:41.510Z Reads: 134

```
you should not be eskating if you can't footbrake ... 
In the time i had this remote, i had more problems with snapping belts and other problems that made it impossible to brake than this remote. 

If connection get dropped, you need to tap the bluetooth device HC-05 on your phone screen insde the app. and you will be connected in 0.5 seconds. The 2.5 seconds is totally up to you of finding the HC-05 module in your bluetooth list. Mine is quite large.
( 3 seconds was an overestimate by me)
```

---
## \#10 Posted by: DeathCookies Posted at: 2016-07-20T13:32:01.336Z Reads: 127

```
[quote="XIII, post:9, topic:6328"]
you should not be eskating if you can't footbrake ...
[/quote]

Please make a video where you make a footbrake when you are cruising with 30mph...
I want to see how long the stopping distance is :joy:
```

---
## \#11 Posted by: XIII Posted at: 2016-07-20T14:39:02.804Z Reads: 120

```
If i'm home again.  I can link you a video of somoene braking from 130 km/hour.  With footbraking.  

I don't think 30 mph with a smartphone is (again...)  a logical assumption.  You would be using this on a 6s board going 30 km/hour.
```

---
## \#12 Posted by: MidnightOne Posted at: 2016-07-20T16:31:16.157Z Reads: 120

```
Yeah, innovations benefit aside I don't think sliding your finger on cold glass while not looking is not a practical way of controlling a hazardous (and fast) vehicle. Not to mention the price of the phone that you'll need to repair after making a mistake.

Also a part of the reason is the lack of tactile feedback. Would you buy a touch keyboard instead of mechnical one? You would only show it off to your guests and use the regular one when they're gone.
```

---
## \#13 Posted by: XIII Posted at: 2016-07-20T17:02:21.567Z Reads: 115

```
Still if you forget your remote, you have your phone +

You can say: " I have an electric skateboard"

"wow, cool so how do you use it?"

"I  control it with my phone" 

"OMG" 

:)
```

---
## \#14 Posted by: MidnightOne Posted at: 2016-07-20T17:37:02.449Z Reads: 112

```
Both solid points, I was too concerned with practical approach to take them into account. :slight_smile:
```

---
## \#15 Posted by: VladPomogaev Posted at: 2016-07-20T18:53:47.267Z Reads: 112

```
Still, I think that's this is a cool alternative to those big clunky remotes. Why use a GT2B, or even a Nunchuck, when you can interchange between that and a remote that you have in your pocket 99% of the time?
```

---
## \#16 Posted by: VladPomogaev Posted at: 2016-08-15T22:05:23.010Z Reads: 105

```
<img src="/uploads/db1493/original/2X/1/151c1454a00e0190d6c1336821b75cfc32a8014b.jpg" width="690" height="460">

Hello everyone! Here's an update. 

I've had a lot of people ask me about if they could buy the smartphone receiver. I sold the two prototypes that I had, but since people kept asking for them, I decided to outsource my design, make it more "professional",  and build 10 more!

If you would like to get your hands on this convenient controller, I will be posting them on http://currentcontrolsystems.com/ in several weeks. Also, this controller has three channels, meaning you'll be able to control a RC boat or car as well!
```

---
## \#17 Posted by: VladPomogaev Posted at: 2016-09-17T13:59:13.149Z Reads: 89

```
<img src="/uploads/db1493/original/3X/e/2/e2b00ba6646b35bd06442ee2145af736352bdbbb.jpg" width="690" height="460">

^ my desk has turned into an assembly line...

And one more update; I have changed the components a little bit! As a response to everyone mentioning that the Bluetooth is susceptible to interference, I have decided to upgrade the radio to a standard (not Low Energy) Bluetooth variant, which gives it a little bit more oomph.

You can get one of these controllers [here now](http://currentcontrolsystems.com/product/electric-skateboardrc-carboat-android-bluetooth-receiver-w-battery-gauge-ppm/)! Thanks!

Oh yeah, and not only is this controller open-source, but I also put together a (hopefully entertaining) video, showing how  I go about assembling the commercial units as well. https://www.youtube.com/watch?v=W1b1Y-LHR4g
```

---
## \#18 Posted by: VladPomogaev Posted at: 2016-10-16T03:51:58.777Z Reads: 65

```
Thank you guys for your support everyone! I've sold over 25 receivers now, and I have a a dozen or so more on backorder. 

Right now I am working on a redesign of the receiver. These are the features that I am adding:

* Settings and Data Integration with the VESC
* Data recording
* "Signal bypass" so that you can switch back and forth between using your smartphone and 2.4Ghz remote
* A thermometer probe (because why not? They are cheap!) 

This new design is going to be similar to the "Rocket Boards" Bluetooth receiver, except it's going to be a full solution for your remote, AND data acquisition, AND it's going to be compatible with Android (obviously). Also, I designed the width of the PCB so that it can strap perfectly to the back of a VESC. It's hard to explain how this works, but I'll post a picture/video showing it off. Here's the new PCB design; it should be here shortly!

<img src="/uploads/db1493/original/3X/1/3/138c6c79a5d3b9b530e82e1fc9ee75d633ea6573.png" width="568" height="500">
```

---
## \#19 Posted by: lox897 Posted at: 2016-10-16T07:42:26.481Z Reads: 58

```
Yum, black soldermask :heart_eyes:
```

---
## \#20 Posted by: VladPomogaev Posted at: 2016-10-16T07:55:56.433Z Reads: 60

```
;)

<img src="/uploads/db1493/original/3X/4/9/49996f3eca234e7df3c43699ebef89128fc80616.png" width="568" height="500">
```

---
