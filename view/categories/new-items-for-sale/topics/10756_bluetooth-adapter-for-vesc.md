# Bluetooth Adapter for VESC

### Replies: 40 Views: 8179

## \#1 Posted by: oriol360 Posted at: 2016-10-07T01:35:51.210Z Reads: 752

```
Hey eSk8!

http://miamielectricboards.com/shop-1/vesc-bluetooth-adapter

With a hurricane coming my way I had some time to work on a BLE Adapter for the VESC to work with Jacob's app.
I used 5-pin JST connections since it's what i had available to me today, but shipped models will have 7-pin connection.
<img src="/uploads/db1493/original/3X/a/2/a2372cd42322633a5e876dd8a3347f2d42cd8bcf.jpg" width="375" height="500">

I noticed my latest Enertion VESC did not have the 7-pin JST on the board so I soldered a 5-pin JST on to it real quick to confirm it worked with as well and my VESC.
<img src="/uploads/db1493/original/3X/e/8/e879442163cbe132537d9af0a4b8b67fe10e560b.jpg" width="375" height="500"> 
<img src="/uploads/db1493/original/3X/d/2/d23c3fbe34612082450283d1cfa709cef1c927d8.jpg" width="375" height="500">

Adaptor worked fine with both VESC!
Made a quick Video and now adapters will be on pre-order for a few weeks while I gather the materials to make about 50 for sale. 
https://youtu.be/R6HAVd0KUjI

http://miamielectricboards.com/shop-1/vesc-bluetooth-adapter
```

---
## \#2 Posted by: Norrmalm Posted at: 2016-10-07T16:57:05.452Z Reads: 630

```
Is it possible to have one shipped to Sweden?
```

---
## \#3 Posted by: rpn314 Posted at: 2016-10-07T18:07:06.863Z Reads: 588

```
Is the HC-05 or HM-10?
```

---
## \#4 Posted by: evoheyax Posted at: 2016-10-07T18:58:17.176Z Reads: 562

```
I thought Jacobs app had a lot of bugs?

Anyways, love the competition. It's about time that Bluetooth modules become the standard for vesc's.

I personally wish vedder would build one in to the VESC.
```

---
## \#5 Posted by: mccloed Posted at: 2016-10-07T19:47:34.754Z Reads: 518

```
Hm-10. At least, that's what it looks like and that's what I used and it works.
```

---
## \#6 Posted by: elkick Posted at: 2016-10-07T22:11:44.299Z Reads: 494

```
At least there will be a nrf24l01 on board.
```

---
## \#7 Posted by: oriol360 Posted at: 2016-10-08T10:37:22.729Z Reads: 474

```
@Norrmalm yup, just pm me or email me and I can let you know the shipping charges, it shouldn't be too much. 

@rpn314 I'm using HM-10  

@evoheyax yup it does have a few. Main functions are really solid though and realtime stats are really useful to see when riding. I'll be donating to Jacob from the sale of these adapters, just wanted to get more people out there using these apps. I'll send some money your way too if these modules are compatible with your app as well.
```

---
## \#8 Posted by: Pablo_702 Posted at: 2016-10-12T06:05:52.410Z Reads: 440

```
Whats the price?
```

---
## \#9 Posted by: rpn314 Posted at: 2016-10-12T06:47:33.231Z Reads: 428

```
The link in the original post has them for pre-order at $19.99
```

---
## \#10 Posted by: Pablo_702 Posted at: 2016-10-12T07:01:47.327Z Reads: 414

```
Thank you 
10 characters
```

---
## \#11 Posted by: rpn314 Posted at: 2016-10-12T07:16:05.181Z Reads: 401

```
Anytime!
10 chars
```

---
## \#12 Posted by: ralphy Posted at: 2016-10-16T21:30:55.558Z Reads: 387

```
Once i get my motors i gotta buy a pair of these. Can i use just one for both vesc?

Im in miami too
```

---
## \#13 Posted by: oriol360 Posted at: 2016-10-17T05:11:36.692Z Reads: 377

```
yeah so for programming you would need two Bluetooth adaptors one for each vesc if you didn't want to be switching the Bluetooth adaptor between vesc.
After they are programmed however if you set it up for canbus you just need one on the main vesc and that one will read all the information and relay it back to the app. 

My suggestion though. Is just get one for reading the information. Jacobs app is still a bit buggy and the programming does not always work over Bluetooth from my testing. The realtime data is the main reason I use this to see how efficient my boards are running
```

---
## \#14 Posted by: rpn314 Posted at: 2016-10-17T16:56:45.879Z Reads: 357

```
To add onto @oriol360, it is theoretically possible to have a single bluetooth module change the parameters of both VESCs using the CAN-bus between them, however I don't believe that any app is configured to do that (including Jacob's). And I have heard of some buggy-ness using Jacob's app with a single VESC, as @oriol360 said.
```

---
## \#15 Posted by: evoheyax Posted at: 2016-10-20T22:31:47.933Z Reads: 356

```
I'm in the process of researching how I can access data from slave vesc's that are connected via canbus. You should only need one.

Btw, I don't believe my app is compadible with this chip. The Bluetooth communication class im using was written specifically for the adafruit chip.
```

---
## \#16 Posted by: solarcross Posted at: 2016-10-30T01:31:14.463Z Reads: 334

```
hello can anybody confirm that using a 3-wire throttle on UART with a bluetooth module is possible ??
```

---
## \#17 Posted by: SeanHacker Posted at: 2016-10-30T03:24:58.521Z Reads: 341

```
@oriol360 Is the app opensource? I'd like to contribute. I know it's on the market. I just can't find anything on git or bitbucket. My repos are here if you'd like to see https://github.com/task650. I can pretty much figure out whatever most of the time.
```

---
## \#18 Posted by: oriol360 Posted at: 2016-10-30T03:37:46.794Z Reads: 338

```
currently that has not been tested as all our remotes are ppm signals. But I would recommend using the uart port for one applications whether it's remote or Bluetooth. 

@SeanHacker yeah it's in stock at my online store. 
 http://miamielectricboards.com/shop-1/vesc-bluetooth-adapter
It's plug and play with the raptor. Vesc code and app codes are all open source so you can code your own app to read the hm-10 ble from this adaptor
```

---
## \#19 Posted by: SeanHacker Posted at: 2016-10-30T03:47:06.875Z Reads: 326

```
Sweet. Thanks! Purchased @oriol360
```

---
## \#20 Posted by: solarcross Posted at: 2016-10-30T03:48:44.164Z Reads: 330

```
well I cannot use a remote because I use VESC for E-bike use so I need the 3-wires for hall twist-throttle
ADC - GND - 3.3V
```

---
## \#21 Posted by: rpn314 Posted at: 2016-10-30T22:09:46.092Z Reads: 312

```
If you are using the UART port for anything else, a bluetooth module made for that same port will not work for you. 1 UART device per port (without some sort of in between module). So yeah, unless you use a different port (which should be theroetically possible, and should be pretty easy since all you really need is the ADC. 3.3V and GND can be gotten from other ports, but you'd probably need a custom firmware) you won't be able to use this module.
```

---
## \#22 Posted by: solarcross Posted at: 2016-11-03T01:18:38.198Z Reads: 301

```
I see..perhaps USB
```

---
## \#23 Posted by: rpn314 Posted at: 2016-11-03T02:04:04.246Z Reads: 303

```
[quote="solarcross, post:22, topic:10756, full:true"]
I see..perhaps USB
[/quote]

you mean to plug a bluetooth module into the usb port on the vesc?
```

---
## \#24 Posted by: solarcross Posted at: 2016-11-04T05:37:29.938Z Reads: 286

```
not quite .. I mean USB to Windows PC.. running BLDC tool in Live mode.. 
thats the only way I know so far..
```

---
## \#25 Posted by: Atimu Posted at: 2017-02-11T05:43:06.970Z Reads: 258

```
@oriol360 I recently received 2 vesc bluetooth adapters from you (Miami boards) and tried both (separately) with my brand new vesc and battery and two new motors (which I tried separately in single motor setups. torque board vesc and motors, 190kv, 12s5p battery), but it doesn't work beyond successfully connecting. In the app, after connecting, pressing buttons doesn't do anything. It won't read configuration, do motor detection, etc. The flashing red light turns a solid red, indicating the connection as you mention in your video on how to connect it. Everything on BLDC tool on my computer works perfectly fine however. 

Any suggestions?
```

---
## \#26 Posted by: Bender Posted at: 2017-02-11T14:37:11.186Z Reads: 246

```
What's your baud rate set to in BLDC Tool?
Which app are you using?
Different apps use different baud rates to communicate
```

---
## \#27 Posted by: Atimu Posted at: 2017-02-11T17:54:43.119Z Reads: 238

```
@bender I've used vesc connect and vesc monitor, but it would only connect to vesc connect. 
I found the baud rate under UART in app configuration and its set to 0. What should it be for this to work?
```

---
## \#28 Posted by: Bender Posted at: 2017-02-11T19:52:28.967Z Reads: 240

```
It should be 9600 or 115600
Can't remember which Jacobs app is
```

---
## \#29 Posted by: Atimu Posted at: 2017-02-12T00:08:22.762Z Reads: 247

```
So I tried both 9600 and 115600. Only the first one connects (the second doesnt get detected at all) but after connecting its the same as it was before :sweat: nothing else in the app works. I'm sticking to vesc connect since it seems to be the best from the few I've tried, but if you think another might work better or anything let me know.
```

---
## \#30 Posted by: Deakbannok Posted at: 2017-02-12T15:45:58.738Z Reads: 245

```
Have you tried to connect on a different phone , Android or iPhone , laptop?
```

---
## \#31 Posted by: Ackmaniac Posted at: 2017-02-12T15:50:23.537Z Reads: 242

```
@Atimu

do me a favour and try if it works with my app. 

[Ackmaniac VESC Monitor Android App](https://play.google.com/store/apps/details?id=ackmaniac.vescmonitor&hl=de)
```

---
## \#32 Posted by: emepror Posted at: 2017-02-12T15:54:15.430Z Reads: 246

```
Try 115200, 115600 isn't a standard baud rate
```

---
## \#33 Posted by: Atimu Posted at: 2017-02-13T18:15:09.167Z Reads: 251

```
I tried it on two different android phones and its the same problem. I don't know about any Windows bluetooth vesc apps or anything. 

The Ackmaniac VESC Monitor app connects just like the vesc connect app but nothing seems to be working. 

The 115200 baud rate connects in the app, but the same problem occurs. I also noticed the disconnect button in the app doesn't work. But the app lets me input values and stuff so I know it's not crashing or anything.
```

---
## \#34 Posted by: Ackmaniac Posted at: 2017-02-13T19:53:24.433Z Reads: 242

```
Please try a baudrate of 9600 with my app and connect it to the master VESC.
And you need to connect the VCC of the Bluetooth module to the 5V pin of the VESC.
RX on the VESC needs to connect to TX on the module.
TX on the VESC needs to connect to RX on the module.
```

---
## \#35 Posted by: ARetardedPillow Posted at: 2017-10-04T22:29:16.333Z Reads: 139

```
I have the module but not the app, cant find it in the app store
```

---
## \#36 Posted by: gee Posted at: 2018-02-02T07:25:53.840Z Reads: 114

```
would this work?
https://www.aliexpress.com/item/WAVGAT-AT-09-4-0-Bluetooth-module-for-ble-with-backplane-serial-BLE-CC2540-CC2541-Serial/32826166129.html?ws_ab_test=searchweb0_0,searchweb201602_2_10065_10344_10130_10068_10324_10547_10342_10325_10546_10343_10340_10548_10341_10545_10084_10083_10618_10307_10313_10059_10534_100031_10103_441_10624_442_10623_10622_10621_10620_10142,searchweb201603_25,ppcSwitch_5&algo_expid=a4d31e4e-17f7-4be8-8a8a-8579d061ed34-5&algo_pvid=a4d31e4e-17f7-4be8-8a8a-8579d061ed34&priceBeautifyAB=0
```

---
## \#37 Posted by: cryo Posted at: 2018-07-22T16:34:14.609Z Reads: 77

```
Hey guys just got an hm10 module and have been trying to get it working. It connects but doesnt show any data. I have baudrate at 9600 and ppm+uart selected. I suspect i have the pins mismatched but i dont want to take the white wrapping off the meb vesc to check. Could someon who has the oesc from meb tell me the pinout from the uart port?

![20180721_113308|666x500](upload://fAbX9DuChtbbnU1MfL6zyEJUnCB.jpg)

Currently have it like this, black is hm10 vcc, white is hm10 gnd, orange is hm10 rxd, green is hm10 txd.

@oriol360
```

---
## \#38 Posted by: oriol360 Posted at: 2018-07-23T18:21:36.882Z Reads: 70

```
![Vesc%20Pin%20layout|374x500](upload://gV8mh3b0eNCZ884TIABmojvS5U9.jpg)

@cryo what app you using?
```

---
## \#39 Posted by: cryo Posted at: 2018-07-23T19:09:05.845Z Reads: 63

```
vesc monitor from ackmaniac
on his firmware 2.54 and android 7.0

edit: Nvm its working now for some reason... guess I just had to power cycle for settings to take effect? Thanks for the help.
```

---
## \#40 Posted by: luis99945 Posted at: 2018-10-03T13:49:42.897Z Reads: 36

```

what meters do you have?
you have diy electric skateboard vescs?(i broke one of my vescs and i need remplace it)
```

---
