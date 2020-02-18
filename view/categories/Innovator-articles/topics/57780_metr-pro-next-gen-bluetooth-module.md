# Metr Pro - Next Gen Bluetooth Module

### Replies: 1133 Views: 37217

## \#1 Posted by: rpasichnyk Posted at: 2018-06-04T15:00:01.362Z Reads: 1703

```
Hey everyone!

Together with @hexakopter we present you the all new **Metr Pro** bluetooth module! It is based on the latest tech from Nordic nRF52 and packs a punch!

![metr-pro|690x460](upload://mfspbyAz53KR9WPBTTBoqGRpQN9.jpg)

<div align=center>

## Hardware Features

</div>

1. **Metal Shield** for interference protection. This is very important because a lot of EMI is coming from our high current fast switching setups in some cases disturbing the correct operation of the module. The main unit is shielded to mitigate that.
2. Optional **external 2.4GHz antenna**. Recommended if you have carbon fiber enclosure or you experience a lot of issues with bluetooth module disconnecting. It makes a noticeable difference. In our tests external antenna doubled the range of operation. But even the default configuration with internal PCB antenna still has much better connection than HM-10.

3. **Three bright colored LEDs** for easy diagnostics.
<table>
<tr>
<td>
<div align=center>

![table_discov_90|425x200,35%](upload://u3dBafqrtPDauRfEPeUtxMKJ05g.gif)

</div>

</td><td>

Blue LED (bottom) is for bluetooth. When it is blinking slowly, the module is in Discovery mode. It is advertising and you should be able to find it within your mobile app.

</td>
</tr>
<tr>
<td>

<div align=center>

![table_ble_90|427x200,35%](upload://gP01tnlJPCuoutpJKFhU1zPVV8o.gif)

</div>

</td><td>

Blue LED rapidly blinking means the data is exchanged via bluetooth. Each incoming and outgoing bluetooth packet results in a little blink.

</td>
</tr>
<tr>
<td>

<div align=center>

![table_uart_90|432x200,35%](upload://1McL16VaM0UYLnKqt39KWGp86j7.gif)

</div>

</td><td>

Green LED (center) is for UART. When it is blinking the module is negotiating BAUD rate and RX / TX pin positions. Usually after half a second it becomes solid green which means the negotiation is successful.

</td>
</tr>
<tr>
<td>

<div align=center>

![table_error|427x200,35%](upload://vZKjg3j4r9VtjaRbGiXW2QSH8kj.jpg)

</div>

</td><td>

Red LED (top) is for errors. When it’s ON, some error has happened. It might be wrong security PIN code, or UART communication problem. Metr Pro will try to report this error back to the Metr app.

</td>
</tr>
</table>

4. **Additional nRF52 pinouts** on the back of the module. Currently these pins are not used but we might have some ideas like adding a Micro SD card or another UART to communicate with some other stuff ;)


<div align=center>

## Software Features

</div>

1. **BLE security** with Elliptic Curve Cryptography and Man-in-the-Middle protection. All the modules that we use today have bad security or no security at all. It is only a matter of time before someone starts messing around with it. Think about it this way: your board can be hacked, your settings can be messed up, this can result in serious injury. The chance is very low, but why risk?
![pincode2|690x328,80%](upload://9FDhBejOLzSlZ09DBGYqnUEs2bS.jpg)
Metr Pro will never bypass communication from an unpaired phone to the VESC. Each Metr Pro module has a random 6 digit PIN code label on the back side which is used for pairing. Once paired, all the communication is encrypted and secure.

2. Works with **all the apps**. We made sure Metr Pro supports every VESC app. There are more and more apps and they are getting better and better. Thanks to all the amazing software developers out there! 
<div align=center>

<table>
<tr>
<td>

<div align=center>

![ackmaniac|360x360,34%](upload://tOMGCYNYYOwfRCpr0qVc2LjLEIj.png)

ACKMANIAC-ESC

</div>

</td><td>

<div align=center>

![eskatevesc|494x500,25%](upload://4TnngBuZOXzCC66sWIssoFVaej0.jpg)

eSkate VESC

</div>

</td>
</td><td>

<div align=center>

![neutral_v|314x278,45%](upload://nPTjdXwbyHtRSbebbgXX8bezRNv.png)

VESC Tool

</div>

</td>

</tr>
<tr>
<td>

<div align=center>

![esk8matics|304x304,37%](upload://iLBHStvA4CSlO5uo9FCK0lsFGDe.png)

eSk8matics

</td><td>

<div align=center>

![metr|515x500,23%](upload://jpc50EXFlLO3tgM4x9P3jrhqU6I.jpg)

Metr

</td>
</td><td>

<div align=center>

![perimetr|503x500,23%](upload://2QhU7MrOXeKrrSzTvxpyHr3aFSl.jpg)

Perimetr

</td>

</tr>
</table>
</div>

3. Latest updates from Benjamin made possible what we call **VESC Tool Direct**. Forget about TCP Bridge. Connect directly from the desktop version of VESC Tool. Supported on Windows, Mac and Linux.
![vesctool|690x362](upload://jPOuxWff5Crlz6mdvzEhgPDLlrv.png)

4. Works with **all the hardware**. No matter what VESC variant you have, no matter what firmware you have installed*, no matter what BAUD rate you have, Metr Pro works with everything. It has automatic BAUD rate detection and automatic RX / TX pins detection. There is only one cable and only one way to connect it. After being connected it detects RX and TX pins as well as BAUD rates programmatically until successful connection is made. And it has no issues with Android Oreo.

5. **Updatable over the air**. The module itself is running a special firmware that implements the whole BLE stack, UART, VESC protocol + custom Metr protocol. New features can be (and will be) constantly added and you can update the module effortlessly with the Metr app over the air.
![ota|320x426,80%](upload://rfnxb5rlMiS4T2EI3A6CarkAzgz.gif)

6. **Parallel VESC firmware update** with automatic settings backup and restore. With just one click the new firmware can be sent simultaneously to both of your VESCs connected via CAN and motor + app configuration will be restored after the update. Everything in just one minute. Ben and Nico have been hitting hard with the new updates and we think that is awesome. With Metr Pro you can keep up without too much hassle.
![vfu|320x427,80%](upload://fIOGenFqtELqH5JWnXIxgAAasKd.gif)

7. **Startup Mode**. From the Modes tab you can assign one of your modes to be a startup mode and it will automatically apply when you power on your VESC, even if your phone is not around. I like to use it as a warm up. I set up a mode with low-amp, low-speed as startup and ride it for 5-10 first minutes before changing to a faster one. This helps to avoid the stressful situations I sometimes had when accidentally pushing trigger too much in the morning on the way to work.
![startup|320x384,80%](upload://wHFSaHiRsrkNR2UMJ6WfXQYvAeF.gif)

8. **True Dual Realtime Data**. Metr Pro constantly communicates with both VESCs connected via CAN, repacks the data and sends it to the Metr app. Just in case you want to see both motor temperatures and both motor currents independently and understand if one motor starts to perform worse and needs some service. The delivery **speed and density** of Realtime Data is also improved. With these modules you will have faster updates and much more detail.
![dual|320x351,80%](upload://3k49qPb27N51hDrDeWfBWGShmIb.gif)

We can’t wait for you to use Metr Pro in your builds! This module is no longer just a serial bridge between VESC and mobile, it is a full-fledged VESC-addon with smart features. Each Metr Pro is crafted in Germany by @hexakopter and individually tested before shipping. It is available starting today. Get yours now!

### Pricing:
Metr Pro €40
Metr Pro with external antenna €52
For EU customers there is additional 25% VAT
Worldwide shipping: €12

![2modules|690x459](upload://qgFkqmhrNky9JpubfL2037kWAnQ.jpg)

https://metr.at/shop

Now hit us with your questions!
```

---
## \#2 Posted by: mmaner Posted at: 2018-06-04T15:06:39.666Z Reads: 1341

```
Does it work with @Ackmaniac 2.54 and 3.x modes?
```

---
## \#4 Posted by: bevilacqua Posted at: 2018-06-04T15:09:15.615Z Reads: 1323

```
[quote="rpasichnyk, post:1, topic:57780"]
 much more detail.
[/quote]
Im so pumped :D 

Ordered!
```

---
## \#5 Posted by: bevilacqua Posted at: 2018-06-04T15:09:35.285Z Reads: 1284

```
no ;) 
10cahr
```

---
## \#6 Posted by: bevilacqua Posted at: 2018-06-04T15:10:48.321Z Reads: 1250

```
[quote="rpasichnyk, post:1, topic:57780"]
Ben and Nico have been hitting hard with the new updates and we think that is awesome. With Metr Pro you can keep up without too much hassle.
[/quote]

I guess it should be
```

---
## \#7 Posted by: oyta Posted at: 2018-06-04T15:11:42.713Z Reads: 1181

```
Impressed! I ordered one as I know you are updating it constantly and keeping it fresh 😁
```

---
## \#8 Posted by: Deckoz Posted at: 2018-06-04T15:16:38.342Z Reads: 1158

```
Looks like I need 4 of these lol...

I will mail you soon @rpasichnyk does your store still charge shipping for each module? Or have you corrected it for one shipping charge with multiple modules
```

---
## \#9 Posted by: Cobber Posted at: 2018-06-04T15:17:12.048Z Reads: 1123

```
looks cool bro :dark_sunglasses: I should trade up from my hm-10...
```

---
## \#10 Posted by: Kug3lis Posted at: 2018-06-04T15:17:35.036Z Reads: 1091

```
I was expecting from pictures something like WiFi TCP/IP bridge or etc :P
```

---
## \#11 Posted by: bevilacqua Posted at: 2018-06-04T15:17:36.340Z Reads: 1057

```
I just ordered: Within PP you select the quantity so I guess it is a single 12e charge for shipping
```

---
## \#12 Posted by: zyphaz Posted at: 2018-06-04T15:24:04.574Z Reads: 1032

```
Should stateside people order direct from you @rpasichnyk ?  Or wait for partners like Jared to get stock?
```

---
## \#13 Posted by: oyta Posted at: 2018-06-04T15:26:24.161Z Reads: 1000

```
But I guess the VESC direct feature and FW OTA update-feature does the job perfectly? 😊
```

---
## \#14 Posted by: Mathias Posted at: 2018-06-04T15:27:37.489Z Reads: 986

```
Wow... this is awesome! 

Does all of this including modes and startup mode work with the stock firmware by Benjamin?
```

---
## \#15 Posted by: BigBrit Posted at: 2018-06-04T15:29:40.061Z Reads: 971

```
Please add a micro SD card to the back for local recording.  That would be so cool and what I was hoping you were going to announce today.  It would be great for those times when you don’t have any phone battery or do not want realtime data.

I love the new in tool connection, thats so nice.
```

---
## \#16 Posted by: Kug3lis Posted at: 2018-06-04T15:39:20.327Z Reads: 959

```
Yes, but then I need to have Bluetooth on computer :) Also VESC-Tool doesn't work well with BLE devices iirc in some Operating Systems :)
```

---
## \#17 Posted by: oyta Posted at: 2018-06-04T15:52:24.284Z Reads: 955

```
@Kug3lis Ah, I see! But you can still use TCP Bridge feature in the metr app or ackmaniac’s app for instance. Even though I see the hassle with the bridge method.
```

---
## \#18 Posted by: Dook Posted at: 2018-06-04T16:16:15.487Z Reads: 953

```
ordered, going straight into the new build 👍
```

---
## \#19 Posted by: fraannk Posted at: 2018-06-04T16:28:57.437Z Reads: 939

```
So still no manual way of duplicating the data when running split PPM? :( I refuse to use CAN.
```

---
## \#20 Posted by: Jc06505n Posted at: 2018-06-04T16:43:26.490Z Reads: 936

```
Any discount for a group buy? @rpasichnyk 


I had to ask 😭
```

---
## \#21 Posted by: E1Allen Posted at: 2018-06-04T17:02:42.481Z Reads: 923

```
Size of external antenna?
```

---
## \#22 Posted by: caustin Posted at: 2018-06-04T17:30:48.316Z Reads: 870

```
Would like to purchase 3 BLE and 1 remote antenna (I assume the antenna is detachable)...Paypal does not look  to be offering me an easy way to purchase 2 BLE w/PCB and 1 BLE w/remote antenna in single order and single shipping charge.  Can you pm me how to get this done?  Thanks!
```

---
## \#23 Posted by: ElskerShadow Posted at: 2018-06-04T18:07:05.377Z Reads: 853

```
Ordered 2 :),
10char
```

---
## \#24 Posted by: rpasichnyk Posted at: 2018-06-04T19:02:05.604Z Reads: 879

```
@mmaner Ackmaniac 3.100+ firmwares are supported, 2.54 not yet, but I can add if there is enough interest

@Deckoz @caustin everyone feel free to put multiple orders for modules with external antenna and without, I will consolidate shipping and will do PayPal refund.

@E1Allen
![antenna|349x500,70%](upload://9cfE32zRhjil37ZfNxiou2CZ0L.jpg)

@Mathias yes, Modes and Startup Mode work with stock firmware

@zyphaz at the moment you can only order at metr.at/shop, but I hope @fottaz will help with distribution in EU and @JLabs in US in the future :+1:
```

---
## \#25 Posted by: Sender Posted at: 2018-06-04T19:06:45.968Z Reads: 819

```
@jlabs do you have some of these coming to the shop?
```

---
## \#26 Posted by: Silverline Posted at: 2018-06-04T19:09:06.589Z Reads: 803

```
We could just tear this rubber duck antenna apart, keeping the internal coax intact , so it dosn`t take so much of a space....

We do it on FPV racing quads all the time
```

---
## \#27 Posted by: Yecrtz Posted at: 2018-06-04T19:12:15.431Z Reads: 784

```
Sweet! Ordered one :smile:
```

---
## \#28 Posted by: E1Allen Posted at: 2018-06-04T19:28:33.767Z Reads: 782

```
Figured as much
```

---
## \#29 Posted by: Pimousse Posted at: 2018-06-04T19:29:14.030Z Reads: 790

```
Congrats Roman !
You achieve a very advanced product here, focused on the real concerns everyday riders can encounter.
Really impressive.
(I need to find spare times to finish my custom FW. Combined to this, that would be amazing ;) ).

Do you sell only 7pin version ? No 8pin for VESC6 ?
```

---
## \#31 Posted by: Cobber Posted at: 2018-06-04T19:39:49.743Z Reads: 772

```
I have a pair of ESCape coming from stewii.

[quote="Pimousse, post:29, topic:57780"]
Do you sell only 7pin version ? No 8pin for VESC6 ?
[/quote]

Will the metr pro not work with them @Pimousse? :thinking:
```

---
## \#32 Posted by: Pimousse Posted at: 2018-06-04T19:43:51.731Z Reads: 749

```
Probably 7pin JST male connector can be plugged into 8pin female connector (last pin is ADC3, not used in VESC FW).
Roman will tell.
```

---
## \#33 Posted by: Cobber Posted at: 2018-06-04T19:50:03.194Z Reads: 735

```
_thanks_ **π** :deer:

:joy: :rofl:

will hang tight & wait :sunglasses:
```

---
## \#34 Posted by: Pimousse Posted at: 2018-06-04T19:51:49.605Z Reads: 735

```
[quote="Cobber, post:33, topic:57780"]
thanks π :deer:
[/quote]

Pi-Elk ? :rofl:
```

---
## \#35 Posted by: Ubbiedude Posted at: 2018-06-04T19:52:51.684Z Reads: 719

```
ordered one :D
```

---
## \#36 Posted by: caustin Posted at: 2018-06-04T19:57:17.841Z Reads: 717

```
Yes definitely need support for ack 2.54 if possible. Many people still using that and older bdlc tool. Thanks!
```

---
## \#37 Posted by: Cobber Posted at: 2018-06-04T19:58:13.156Z Reads: 707

```
mousse (chocolate dessert) = (sounds like) moose = :deer: 
:D
it was either that or go with a mouse :mouse:
:beers:
```

---
## \#38 Posted by: mmaner Posted at: 2018-06-04T19:58:34.948Z Reads: 716

```
[quote="rpasichnyk, post:24, topic:57780"]
@mmaner Ackmaniac 3.100+ firmwares are supported, 2.54 not yet, but I can add if there is enough interest
[/quote]

Great.  I would definitely add support for 2.54, there are lots of people that prefer it to the later versions.
```

---
## \#39 Posted by: rpasichnyk Posted at: 2018-06-04T19:59:06.189Z Reads: 709

```
Yes, 7pin JST can be plugged in VESC6 with last pin ADC3 unused. It will hold there just fine.
```

---
## \#40 Posted by: ElskerShadow Posted at: 2018-06-04T20:59:16.600Z Reads: 706

```
90 % of my builds are in 2.18 no reason to move!
```

---
## \#41 Posted by: Mathias Posted at: 2018-06-04T21:00:12.062Z Reads: 704

```
[quote="rpasichnyk, post:24, topic:57780"]
@Mathias yes, Modes and Startup Mode work with stock firmware
[/quote]

You, sir, deserve my money :joy:, I just ordered. This is exactly what I've been looking for.
```

---
## \#42 Posted by: mmaner Posted at: 2018-06-04T21:00:24.632Z Reads: 691

```
The reason I use 2.54 is the throttle curve, I love it.
```

---
## \#43 Posted by: ElskerShadow Posted at: 2018-06-04T21:11:34.974Z Reads: 644

```
@mmaner  What does this specifically gives?
```

---
## \#44 Posted by: Jc06505n Posted at: 2018-06-04T21:24:47.887Z Reads: 628

```
What future features do you have in mind for the Pro?
```

---
## \#45 Posted by: mmaner Posted at: 2018-06-04T21:31:46.951Z Reads: 625

```
It makes the throttle and brakes more progressive, giving you more control at low throttle break and increasing power the higher throttle/brake you go.
```

---
## \#46 Posted by: i2oadsweepei2 Posted at: 2018-06-04T22:31:48.685Z Reads: 627

```
Yes please to support 2.54 👍
```

---
## \#47 Posted by: Adam0311 Posted at: 2018-06-05T00:15:49.794Z Reads: 640

```
[quote="mmaner, post:45, topic:57780, full:true"]
It makes the throttle and brakes more progressive, giving you more control at low throttle break and increasing power the higher throttle/brake you go.
[/quote]

1+ what @mmaner said. Just reflashed firmware on an older board last week, very noticeable difference. Much smoother, the torque steps are basically gone.
```

---
## \#48 Posted by: zyphaz Posted at: 2018-06-05T04:05:45.940Z Reads: 624

```
Awesome, thanks Roman. Ordered!
```

---
## \#49 Posted by: stormboard1 Posted at: 2018-06-05T04:19:04.300Z Reads: 614

```
Niiiice but is it one for each vesc?
```

---
## \#50 Posted by: mmaner Posted at: 2018-06-05T04:20:55.184Z Reads: 608

```
Nope, just use can bus.
```

---
## \#51 Posted by: Battosaii Posted at: 2018-06-05T04:25:29.649Z Reads: 615

```
Does anyone know if the Metr app works with the Samsung Gear 3 watch? I'd love to get info on my watch while I ride.
```

---
## \#52 Posted by: mrplaygood Posted at: 2018-06-05T05:20:29.920Z Reads: 608

```
Damn, just received the „old“ HM-10 Metr.at module yesterday :/ Any way to monitor dual Vesc setup with this module or do I need the new module for this?
```

---
## \#53 Posted by: KickMe Posted at: 2018-06-05T08:30:42.486Z Reads: 595

```
Which of the new features going to be available with the "old" metr dongles, if any?

Impressive work by the way.
```

---
## \#54 Posted by: CBom Posted at: 2018-06-05T09:27:49.804Z Reads: 592

```
Looks great! Does this one work with Android 8?
```

---
## \#55 Posted by: Yecrtz Posted at: 2018-06-05T09:53:45.048Z Reads: 582

```
Of course, the current one does.
```

---
## \#56 Posted by: CBom Posted at: 2018-06-05T10:10:28.986Z Reads: 581

```
What did you do to make the current one work with Android 8? My new phone with 8.1 can't find the device but the old one with 7 finds it.
```

---
## \#57 Posted by: ElskerShadow Posted at: 2018-06-05T11:13:23.582Z Reads: 575

```
No they never wanted to develop for tizen it's a bummer I wish I could use my s2
```

---
## \#58 Posted by: BigBrit Posted at: 2018-06-05T11:28:17.870Z Reads: 588

```
Same, love that curve! Im currently running -20% on both acceleration and brake and its fantastic
```

---
## \#59 Posted by: i2oadsweepei2 Posted at: 2018-06-05T12:09:08.393Z Reads: 627

```
I think this is what you are looking for. I’m using this with my original module. It doesn’t show separate values on the real-time tab though.

![image|666x500](upload://gZR4XvVbLhC11uNWm0Vl83H89sx.jpeg)

![image|656x365](upload://5x7KgzXFZXn1HOKNWl29uo9vUem.jpeg)
```

---
## \#60 Posted by: Yecrtz Posted at: 2018-06-05T13:38:21.003Z Reads: 598

```
It just worked out of the box. Android 8.1.0 oneplus 6..
```

---
## \#61 Posted by: CBom Posted at: 2018-06-05T13:53:09.977Z Reads: 605

```
Looks like OnePlus solved that problem. My nexus device and my Xiaomi mi mix 2 does not find it.
```

---
## \#62 Posted by: bevilacqua Posted at: 2018-06-05T14:18:48.276Z Reads: 605

```
Do you have any shipping ETA? 
(If ordered on release day)
```

---
## \#63 Posted by: Maxid Posted at: 2018-06-05T15:39:19.152Z Reads: 589

```
I am little confused: the pin protected pairing thing can be done with an HM-10 also, no? Just need to set it up via AT commands.
Also what does startup mode mean? Just have what you want as "startup" as your default in the VESC and then update to a different mode via for example @Ackmaniac's App later while riding. Or am I missing something?
Seems like nice hardware though and i like the dual vesc data - that is really helpful when you are using for example different kv motors in a dual setup.
```

---
## \#64 Posted by: sayekim Posted at: 2018-06-05T16:18:11.299Z Reads: 601

```
This is awesome. Can’t wait to use it for my carvon build. 
I ordered one, thank you for this next great step in bluetooth vesc monitoring. 

![image|281x499](upload://oSamdzMOYMqu94Pc29KIQdKQMx3.jpg)
```

---
## \#65 Posted by: hexakopter Posted at: 2018-06-05T20:39:06.116Z Reads: 600

```
It's very encouraging to see you all excited! A big thanks to everyone that already ordered a Metr Pro module so that we sold all our 22 modules that were already produced on our release data. Thats awesome! :grinning:  I will add pictures of these modules below. We will deliver our best! I am working hard right now to produce some more so that all modules that are bought as of now will be shipped as soon as possible. Right after we finish support for 2.54 and 2.18 and test all use cases, we will start shipping. We will try to ship all the modules that have been ordered so far hopefully before Monday. First orders will be shipped first.

@mmaner @caustin @ElskerShadow @i2oadsweepei2 @Adam0311 we didn't realize how many people are using 2.54 and 2.18, the support for those is being added as we speak. Dual Realtime Data, and Modes will be supported.

[quote="mrplaygood, post:52, topic:57780"]
Damn, just received the „old“ HM-10 [Metr.at ](http://Metr.at) module yesterday :confused: Any way to monitor dual Vesc setup with this module or do I need the new module for this?
[/quote]
You can still monitor both of your VESCs with HM-10, but only one at a time using CAN ID in Settings


[quote="CBom, post:54, topic:57780, full:true"]
Looks great! Does this one work with Android 8?
[/quote]
Yes Metr Pro works with Android 8 Oreo. Tested on Pixel 2 XL. The old module doesn't get discovered on Oreo most of the times according to the forum members.

![4|690x460](upload://fKORwKiUJ5Sbyz22oI7KUBoGUh7.jpg)![3|690x460](upload://iMuJ4oFA10BkP2ZOahnUeqCWEcT.jpg)
```

---
## \#66 Posted by: Silverline Posted at: 2018-06-05T21:54:44.364Z Reads: 553

```
How is the physical size Vs. The old one ?
```

---
## \#67 Posted by: mmaner Posted at: 2018-06-05T21:57:16.048Z Reads: 558

```
[quote="hexakopter, post:65, topic:57780"]
@mmaner @caustin @ElskerShadow @i2oadsweepei2 @Adam0311 we didn’t realize how many people are using 2.54 and 2.18, the support for those is being added as we speak. Dual Realtime Data, and Modes will be supported.
[/quote]

Awesome, I appreciate the work you guys are putting into this.
```

---
## \#68 Posted by: webst Posted at: 2018-06-05T22:05:36.878Z Reads: 552

```
Slightly OT but how is it possible that nobody ported this ideal acceleration curve to newer firmware yet?
```

---
## \#69 Posted by: mmaner Posted at: 2018-06-05T22:13:02.458Z Reads: 543

```
I assume it it @Ackmaniac 3.x but I wasn't able to get it to work on my FocBox's so I Just stayed at 2.54.  I don't have any complaints and dont know of any reason I need to change...
```

---
## \#70 Posted by: hexakopter Posted at: 2018-06-05T22:18:58.786Z Reads: 548

```
[quote="Silverline, post:66, topic:57780, full:true"]
How is the physical size Vs. The old one ?
[/quote]
As you can see on [https://metr.at/shop](https://metr.at/shop) the dimension of the Metr Pro module is 42mm × 21mm × 9mm.

[quote="mmaner, post:67, topic:57780"]
Awesome, I appreciate the work you guys are putting into this.
[/quote]
Thanks a lot. We do our best. :smiley:
```

---
## \#71 Posted by: Gdunn416 Posted at: 2018-06-06T01:19:30.151Z Reads: 520

```
Is it possible to use the Metr Pro in conjunction with the Firefly remote on a dual Focbox setup?
```

---
## \#72 Posted by: bevilacqua Posted at: 2018-06-06T08:16:57.464Z Reads: 520

```
you just need 2 uart ports, so yes. 1 for the remote one for the module.
```

---
## \#73 Posted by: Pimousse Posted at: 2018-06-06T09:30:03.206Z Reads: 513

```
It is in 3.x FW.
```

---
## \#74 Posted by: Emerson Posted at: 2018-06-06T11:38:25.707Z Reads: 518

```
Excited to test these out!
```

---
## \#75 Posted by: i2oadsweepei2 Posted at: 2018-06-06T12:41:21.554Z Reads: 524

```
Thank you!! I am picking one up regardless for my next rebuild.
Is there any other options for antenna? Smaller, flat, just wire maybe?
```

---
## \#76 Posted by: Esk8t.nz Posted at: 2018-06-06T12:59:07.673Z Reads: 544

```
Ordered one.. nw i dont need to deal with my enclosure everytime i tune my vesc.. 👍
```

---
## \#77 Posted by: rpasichnyk Posted at: 2018-06-06T17:52:49.800Z Reads: 555

```
We went with this antenna, because it was recommended by our nRF supplier and gives best results. But feel free to experiment. As you can see on the photos, there are 2 parts:

1) U.FL to RP-SMA extension cable
2) 2.4GHz RP-SMA antenna

I recommend to keep the extension cable and try some small 2.4GHz RP-SMA antennas, like this one

https://www.amazon.com/bestseller2016-2-4Ghz-Antenna-Straight-Shipping/dp/B071ZVTCX6/ref=pd_sbs_147_1?_encoding=UTF8&pd_rd_i=B071ZVTCX6&pd_rd_r=T7C42BQE7TBJ6S927QEZ&pd_rd_w=DXWQC&pd_rd_wg=FDrrg&psc=1&refRID=T7C42BQE7TBJ6S927QEZ
```

---
## \#78 Posted by: Gdunn416 Posted at: 2018-06-06T20:40:40.313Z Reads: 533

```
Just got one! I decided not to get the one with the included antenna, and to instead try the PCB antenna. If it doesn't work well I'll get a mini antenna and short extension cable from amazon.

Thanks!
```

---
## \#79 Posted by: Deodand Posted at: 2018-06-07T01:13:45.296Z Reads: 537

```
[quote="rpasichnyk, post:1, topic:57780"]
Latest updates from Benjamin made possible what we call **VESC Tool Direct** . Forget about TCP Bridge. Connect directly from the desktop version of VESC Tool. Supported on Windows, Mac and Linux.
[/quote]

I was under the impression there isn't bluetooth support for vesc-tool on windows? I don't think QT has a compatible windows bluetooth library unless you run it as a UWP app.
```

---
## \#80 Posted by: rpasichnyk Posted at: 2018-06-07T05:02:12.719Z Reads: 536

```
@Gdunn416 please be aware that modules with antenna and without antenna have 0R resistor soldered in a different position. But with a good soldering equipment it should be easy to resolder.

@Deodand Oh yes it does. The latest Qt version does support bluetooth low energy on Windows 10. You just need to build `wip/win` branch of `qtconnectivity.git`. After that VESC Tool works just fine. Btw, very excited to add FOCBOX Unity support to Metr Pro when it's ready :+1:
```

---
## \#81 Posted by: rpasichnyk Posted at: 2018-06-07T05:08:52.794Z Reads: 549

```
<table>
<tr>
<td>
<div align=center>

![mp4|150x267](upload://jeM5olqFvkYMwomSqqVAaE5oxHP.gif)

</div>

</td><td>
<div align=center>

![mov|150x267](upload://qmpfKqrRM5EauB4s2yyEp5u7V8U.gif)

</div>

</td><td>
<div align=center>

![mp4|150x267](upload://n4kxWsKRBP3JO08qnJwJ4nKF4AJ.gif)

</div>

</td>
<tr>
<td>
<div align=center>

![mov|150x267](upload://2LS2cx6EQxz2ZgzSWupd1zANt5v.gif)

</div>

</td><td>
<div align=center>

![mov|150x267](upload://wEN6InnKUs2RfljhpDlT5cLtBdy.gif)

</div>

</td><td>
<div align=center>

![mov|150x267](upload://cRxS5aaara5Fsqoej9auvXebz5l.gif)

</div>

</td><td>
</tr>
</table>

![win10vesctool|640x343,76%](upload://a2WoHbvzoE8UGlD9uD9xsuPUOEj.gif)
```

---
## \#82 Posted by: Gdunn416 Posted at: 2018-06-07T05:43:57.550Z Reads: 536

```
Thanks for the tip. Hopefully it will work OK without the external antenna! Have you successfully tried it without?
```

---
## \#83 Posted by: Deodand Posted at: 2018-06-07T05:49:35.804Z Reads: 532

```
Ah, so currently the vesc-tool has to be rebuilt from source with the changes to qt libs you suggest? Very excited to hear this; no BLE support in windows was driving me crazy. Couldn't get the website-downloaded windows version to run it in a quick test today, assuming they still need to update it with changes? 

We will do our best to get a unity in your hands soon so you can add support! I'm going to try and make a small document to outline the additional values I added to the RT data packet and motor config to accommodate the extra motor parameters/data alongside the released source code.
```

---
## \#84 Posted by: hexakopter Posted at: 2018-06-08T13:37:27.959Z Reads: 547

```
Quick update. I have good news for all of you. :grin: Metr Pro is now updated to also work with FW2.18 and FW2.54 and you will get the newest firmware already flashed to your module so it will work with these firmwares out of the box. I produce some more modules so all orders as of now are covered. We will try to ship the first orders today and all the rest tomorrow.

To make you the waiting time more pleasant I took some pictures. :grinning: Following two pictures show the modules after first step of soldering.
![1|690x460](upload://jvSGEsh5gVUf31dG0E87DCkHvjX.jpg)![2|690x460](upload://aszLVXvfgjpGg2ZrTU1X59dXDXe.jpg)

Next picture shows you what I call the "Metr Pro Art Pyramid" :smiley:

![3|690x460](upload://rXKIiqOMgngvQR9qzNQ5HtbZC0c.jpg)

And the last picture is a closer look what the modules look like in the final state.

![4|690x460](upload://7rDkDrOPXYDWXpGzzHW37N2QDlk.jpg)
```

---
## \#85 Posted by: mmaner Posted at: 2018-06-08T14:15:55.030Z Reads: 510

```
[quote="hexakopter, post:84, topic:57780"]
Metr Pro is now updated to also work with FW2.18 and FW2.54 and you will get the newest firmware already flashed to your module so it will work with these firmwares out of the box.
[/quote]

That is awesome!  Thanks for taking that on, makes this a lot better fit for me and a lot of people.

Is it possible to reflash the original Metr modules to work with 2.54?
```

---
## \#87 Posted by: bevilacqua Posted at: 2018-06-08T14:34:55.642Z Reads: 508

```
I think that just the app should be updated for that. Thats how we got 3.X support for the Metr and Perimetr apps.
```

---
## \#88 Posted by: i2oadsweepei2 Posted at: 2018-06-09T12:21:49.285Z Reads: 518

```
Mine is working on 2.54 right now Mike. I get a lot of disconnect notifications, but it still seems to record the full stats for the day and the records start and stop well enough.  Also I lost my ferrite ring before I installed it. I just found it last night under the beer fridge 👍. That should fix the disconnect problem I hope.

![image|281x500](upload://fQArvhZ6Ya3LS0xGU9wHgE6r0Ka.jpeg)
```

---
## \#89 Posted by: Manu39 Posted at: 2018-06-09T13:33:49.835Z Reads: 474

```
Ordered one...without antenna since the non pro metr.at works very well on the FORAKER. if I ever decide to buy an antenna later, will that be possible?
```

---
## \#90 Posted by: Yecrtz Posted at: 2018-06-09T13:36:59.614Z Reads: 462

```
Just wondering, when upgrading from the original to the pro. The metr app will probably recognize it as a 'new' board. Any chance we can transfer total board data such as distance ridden and stuff within the app?
```

---
## \#91 Posted by: i2oadsweepei2 Posted at: 2018-06-09T13:57:13.568Z Reads: 469

```
I wondered that too. Thought of setting up the app on my wife’s phone and naming the module the same as my first one.. then trying to connect it to my phone and app with all the stats. I don’t have that many records and stats at the moment though.
```

---
## \#92 Posted by: rpasichnyk Posted at: 2018-06-09T20:52:17.859Z Reads: 472

```
All the orders are shipped! You can find tracking numbers inside your PayPal :slight_smile: 
Tracking can be done here https://www.deutschepost.de/sendung/simpleQuery.html?locale=en_GB
(enter 9 June 2018 as posting date, if it doesn't work, enter 8 June 2018)

@mmaner original metr modules already work with 2.54, but some features are not available (dual realtime data, startup mode, etc.)
@Manu39 yes, you can buy antenna later, but you also need to resolder 0R resistor on the Metr Pro module, between internal PCB antenna and external antenna port
@Yecrtz @i2oadsweepei2 unfortunately it is not possible to transfer the stats from other modules, but thank you for the idea
```

---
## \#93 Posted by: CamBo Posted at: 2018-06-09T23:32:57.422Z Reads: 467

```
Just bought 3.  Love your work Roman.
```

---
## \#94 Posted by: rpasichnyk Posted at: 2018-06-10T19:20:58.136Z Reads: 501

```
I'm sure many of you would like to try VESC Tool with direct BLE connection to Metr Pro.
Here you can find the latest VESC Tool binaries for macOS and Windows.

https://github.com/rpasichnyk/vesc_tool/releases

In Windows, you first need to complete new device pairing procedure:
1. Press Start and type bluetooth. Open Bluetooth and other device settings.
![00|294x500,80%](upload://quYeSNojREiCnNWg9oBNafulpoG.jpg)
2. Click "Add Bluetooth or other device
![48|690x425,80%](upload://ArT4M0QgTQ9HmYoLEtNiZUZw0G.jpg)
3. Wait until you see Metr Pro, click on it and enter PIN code
![06|690x419,50%](upload://iDUzkuiIOdLAyNTiIkR0rmMuWEZ.png) 

After this you should be able to connect via VESC Tool
```

---
## \#95 Posted by: Skitzor Posted at: 2018-06-11T16:16:02.353Z Reads: 448

```
Bro, I'm a bit bummed by your approach on this.
I already had 2 official HM 10 modules. Wanted to use the Metr app with a smartwatch.
Ended up buying one of your modules.
Android updates to 8. Cannot use it any more.
Now you release yet another hardware limitation.
Please look into the issues with android 8 and fix them for your original customers
```

---
## \#96 Posted by: Jc06505n Posted at: 2018-06-11T16:26:44.685Z Reads: 452

```
Have you tired any of the other solutions in the first metr thread?

[quote="Skitzor, post:95, topic:57780"]
Now you release yet another hardware limitation.
[/quote]

How does a new Product = "yet another hardware limitation"? In that case all consoles and their successors are hardware limitations as well.
```

---
## \#97 Posted by: Skitzor Posted at: 2018-06-11T16:44:57.837Z Reads: 441

```
In the context of. I reported the issue. I also offered help in testing. The issue still remains.
New Metr module is compatible with Android 8. So if I want the easy way out, have yet to buy another module
```

---
## \#98 Posted by: Manu39 Posted at: 2018-06-11T16:55:27.803Z Reads: 445

```
@rpasichnyk  the BLE connection does not work with the original vesc tools 0.92 ?
Thanks.
```

---
## \#99 Posted by: Yecrtz Posted at: 2018-06-11T20:46:10.517Z Reads: 453

```
I have no issues with android 8. Only certain phones have issues with it.
```

---
## \#100 Posted by: ElskerShadow Posted at: 2018-06-12T11:05:54.693Z Reads: 478

```
![1528801521136|375x500](upload://pxn83Ww0UH4b9pADoy2zJm0svhw.jpg)
I am so happy right now never again I will remove my enclosure to get to my focbox es!
```

---
## \#101 Posted by: webst Posted at: 2018-06-12T11:08:27.742Z Reads: 467

```
Is this your first metr module?
```

---
## \#102 Posted by: ElskerShadow Posted at: 2018-06-12T11:12:03.839Z Reads: 465

```
I had one before but never done the TCP bridge thing
I am happy it is plug and play now
```

---
## \#103 Posted by: DanSkates Posted at: 2018-06-12T11:13:20.160Z Reads: 469

```
OMG GOD!!!  I need to do this too!  Also, I've destroyed one of the micro USB ports and couldn't change the baud rate to get a new BT module to work to change the settings.  This solves that issue!!!  I can finally change my FOCBOX settings :joy:

Beautiful work @hexakopter and @rpasichnyk.  

Btw, if I order today when is the next batch due to be built and shipped?
```

---
## \#104 Posted by: hexakopter Posted at: 2018-06-12T12:54:08.511Z Reads: 460

```
[quote="ElskerShadow, post:100, topic:57780"]
I am so happy right now never again I will remove my enclosure to get to my focbox es!
[/quote]


Thanks for posting the pic. Good to see you received them. I think you will have a lot of fun with your Metr Pro modules. :grinning:

[quote="DanSkates, post:103, topic:57780"]
if I order today when is the next batch due to be built and shipped?
[/quote]
Glad you like our work. When you order today before 8:00 PM CEST it will be shipped out tomorrow morning. Bear in mind that only two modules with external antennas are left. It will take some time before we have new modules with external antennas back in stock. Metr Pro modules with internal antennas are some more left.
```

---
## \#105 Posted by: Cobber Posted at: 2018-06-12T13:21:09.543Z Reads: 448

```
Well I guess I bought the last two...

stoked to be on "board" boys :smiling_imp:

HaHa @DanSkates... I could prob. wait a bit before I use the second, If you're hard up for one quickly let me know bro we will work something out ;)
```

---
## \#106 Posted by: rpasichnyk Posted at: 2018-06-12T19:26:28.142Z Reads: 442

```
@Skitzor I understand you feelings and I am sorry about that. Android 8 has changes that prevent the old module from being discovered. One way to workaround that is to downgrade to Android 7, perform discovery (Scan) inside the metr app and connect to the module, then upgrade to Android 8 and the module will be still saved in the app. This way you can use it with Android 8.

The new module is not a limitation at all. It is actually a direct solution to the Anroid 8 problem. With insurance. If Google does some trick like this again, the module's firmware can be updated over the air to be compatible with future versions of Android.

@Manu BLE connection does work with the original VESC Tool v0.92 but only on Linux
```

---
## \#107 Posted by: DanSkates Posted at: 2018-06-13T03:35:45.184Z Reads: 431

```
[quote="Cobber, post:105, topic:57780"]
HaHa @DanSkates… I could prob. wait a bit before I use the second, If you’re hard up for one quickly let me know bro we will work something out :wink:
[/quote]

Nicely swooped in there cobber!  I might have to take advantage of your kind generosity here if that's cool and buy one off you ;-)  I'll DM you...
```

---
## \#108 Posted by: Maxid Posted at: 2018-06-13T04:10:08.347Z Reads: 411

```
With @Ackmaniac's app I had good experience updating the hm10 firmware. Takes 10min tops and afterwards Oreo does detect the module again. You need an Arduino though.

See: http://www.electric-skateboard.builders/t/vesc-monitor-android-app/20888/694?u=maxid
```

---
## \#109 Posted by: Maxid Posted at: 2018-06-13T04:38:49.016Z Reads: 405

```
Every phone has the "issue" but not every module has faulty firmware. The problem comes from Oreo being stricter in terms of how the responses have to look like coming from the modules and the clone firmwares are not properly programmed so they are no longer considered by the phone. With an original firmware you don't have that problem.
```

---
## \#110 Posted by: Pimousse Posted at: 2018-06-13T06:30:38.983Z Reads: 400

```
[quote="Maxid, post:109, topic:57780"]
The problem comes from Oreo being stricter in terms of how the responses have to look like
[/quote]
Actually, I would say that the problem comes from the clones that embeds a firmware which does not comply with the BLE standard...
But you're right, updating the firmware isn't a big deal. ;)
```

---
## \#111 Posted by: tsr Posted at: 2018-06-13T09:03:37.680Z Reads: 397

```
Hi, looks great - I ordered one yesterday. I am planning to implement an "endless" mode, like the mellow has - but I need some microprocessor to do so. Do you think its possible to integrate this in the receiver? I would able to do the programming myself.
```

---
## \#112 Posted by: Skitzor Posted at: 2018-06-13T10:01:49.546Z Reads: 398

```
No hard feelings, but I think it can be solved by a hardware/software update on either side.

[spoiler]I would buy your pro module. but it exceeds 25$. which means. in stead of 77 euro with shipping. They'll add almost 60 euros as tax. making it a module worth a focbox... [/spoiler]

edit: nvm: Sweden (thought US) I'll look into it.
```

---
## \#113 Posted by: Skitzor Posted at: 2018-06-13T10:06:35.663Z Reads: 384

```
You are on to something. I'll try it tonight. If that's the solution for the oreo problem. @rpasichnyk should add it to the original topic for everyone to find
```

---
## \#114 Posted by: Surfer Posted at: 2018-06-13T10:23:11.067Z Reads: 390

```
I'm not sure if that will be the solution, if you flash it with the regular firmware, it will be discovered by Oreo, but it will miss the protection @rpasichnyk build on the firmware and still not working with metr, it will be like a regular hm-10
```

---
## \#115 Posted by: Skitzor Posted at: 2018-06-13T11:36:49.686Z Reads: 385

```
Well, that's where I guess his part comes in. whatever checkbit he has programmed. He should adjust the firmware and then we can update
```

---
## \#116 Posted by: Manu39 Posted at: 2018-06-13T13:34:38.025Z Reads: 394

```
@hey, i got the Metr.pro and connected it with no problem on my dual ESCAPE by Stewii ..
it is connected to the slave ID1
recognized nickel, the only problem is that I do not know for it right when I go from normal mode (full power) mode warmup or noobs or pepouze the wheel of the vesc slave turns nickel but the wheel of the vesc master is blocked. ..I am forced to rewrite my backup xml ....and when I plug metr.pro on the master ID0 the problem is the opposite .... Rrrrrrrr
 help ....
```

---
## \#117 Posted by: rpasichnyk Posted at: 2018-06-13T13:41:00.763Z Reads: 387

```
Do both of your VESCs have same firmware?
Metr app → Settings → Show logs → send email to rpasichnyk@icloud.com
```

---
## \#118 Posted by: Manu39 Posted at: 2018-06-13T13:45:38.318Z Reads: 387

```
Logs  send before and alter thé probleme.
Thanks
yes for FW. I just tested my different modes with the Metr.at module that I had before: no problem after several mode changes .....

I just re testing with metr.pro: first mode change ... master wheel lock ID0 ... re setting😡
```

---
## \#119 Posted by: rpasichnyk Posted at: 2018-06-13T15:11:56.220Z Reads: 378

```
@Manu39
1. Power down the board, force close the app
2. Power up the board, open app and connect to Metr Pro
3. Make sure that on Realtime tab the green icon is blinking and you see dual FW3.38 
4. Go to Settings → Motor and check pulley count, poles and wheel diameter, change them if needed
5. Try to apply different Modes again
```

---
## \#120 Posted by: Manu39 Posted at: 2018-06-13T15:21:43.654Z Reads: 366

```
already testing roaman and the problem is the same
the am with metr.pro after reconfiguration vesc ... and no problem if no change of mode ....
```

---
## \#121 Posted by: Maxid Posted at: 2018-06-13T15:38:11.812Z Reads: 378

```
I doubt @rpasichnyk built his own firmware. Otherwise it would be easy to publish a new one that solves the Oreo problem. Everything he added must either come via AT commands or is coded into the App.

@Pimousse yeah my wording was probably not perfect there ;) But since it worked before the oreo update I kind of see the problem on the Android side for being too strict where it might not have been necessary. When you update only one part and the system does not work anymore after the update you always see the problem in the thing you changed no?
```

---
## \#122 Posted by: rene Posted at: 2018-06-13T16:47:35.133Z Reads: 391

```
VESC-Tool 0.94 on Windows 10 - cant see the metr.pro bluetooth.

What am I missing?


![image|532x347](upload://lFupibu5WWEtY12kv5AghsNeyQ7.png)

![image|690x180](upload://vaeEnyG439lXUBHNf03GDEzsQj0.png)
```

---
## \#123 Posted by: rpasichnyk Posted at: 2018-06-13T16:51:09.665Z Reads: 391

```
check post #94
https://www.electric-skateboard.builders/t/metr-pro-next-gen-bluetooth-module/57780/94?u=rpasichnyk
The official VESC Tool does not support BLE on Windows. You can use the compiled version from my GitHub. There are no source code modifications, just slightly different version of Qt library. I hope Benjamin can use the procedure that I described to provide BLE support on Windows in the future.
```

---
## \#124 Posted by: trampa Posted at: 2018-06-14T02:33:06.458Z Reads: 359

```
That only works for Windows 10. Win 7 would not start this moded Version. Win 7 is still very popular, so you can't work it this way. 

Frank
```

---
## \#125 Posted by: webst Posted at: 2018-06-14T06:38:40.791Z Reads: 363

```
Windows 7 is dying OS (support till Jan 2020). You still can update for free to win10 even though it’s not officialy supported.
```

---
## \#126 Posted by: trampa Posted at: 2018-06-14T07:36:25.391Z Reads: 361

```
A lot of users still prefer Win 7 over Win 10 and they will use it till 2020. I bet that Microsoft will extend their support even longer. 
So the VESC-Tool should be able to run on 
Win 7. Locking out users is no good idea. Software should be compatible with active and used operating systems. 
The mobile VESC-Tool works quite well for wireless configuration. In addition to that you can use your smartphone as a bridge between your computer and board. 
Personally I prefer using my android tablet that has the full VESC-Tool installed. 
Plenty of options on the table already...

Frank
```

---
## \#127 Posted by: egzplicit Posted at: 2018-06-14T07:53:08.751Z Reads: 346

```
[quote="trampa, post:126, topic:57780"]
Locking out users is no good idea.
[/quote]

Not having it working on windows IS locking out users. Having a version that works in Windows 10 is better than nothing.
```

---
## \#128 Posted by: Pimousse Posted at: 2018-06-14T08:03:09.605Z Reads: 353

```
[quote="trampa, post:126, topic:57780"]
Locking out users is no good idea.
[/quote]
You're 100% right !
So let users go with Metr Pro and all other "third-party" Hardware / devices / app / (i)OS.
This is a reward for the VESC project, not a theft. ;)
```

---
## \#129 Posted by: sk8l8r Posted at: 2018-06-14T08:27:51.409Z Reads: 352

```
brand new focboxes connected for the first time with Metr Pro on Android - everything just worked! more than happy with it so far :)
```

---
## \#130 Posted by: sayekim Posted at: 2018-06-14T10:00:15.671Z Reads: 372

```
Got it. Thanks. 

![image|375x500](upload://zfAqA4cIIVlsv4vHfLY42k86edb.jpeg)
```

---
## \#131 Posted by: DanSkates Posted at: 2018-06-14T12:24:55.294Z Reads: 367

```
[quote="hexakopter, post:104, topic:57780"]
When you order today before 8:00 PM CEST it will be shipped out tomorrow morning. Bear in mind that only two modules with external antennas are left. It will take some time before we have new modules with external antennas back in stock. Metr Pro modules with internal antennas are some more left.
[/quote]

Placed an order earlier today for the Metr Pro with internal antenna - fingers crossed I managed to get in on the current batch ;-)  Thanks - you guys rock!
```

---
## \#132 Posted by: bevilacqua Posted at: 2018-06-14T12:26:47.853Z Reads: 361

```
@rpasichnyk Roman, is it possible to lower the update interval when using Metr-Pro? For example from 300ms to 200 or even 150ms?
```

---
## \#133 Posted by: Ubbiedude Posted at: 2018-06-14T14:10:14.079Z Reads: 370

```
Postman came by today ![20180614_160826|690x388](upload://w6cNJHJAQ713HQeAgpN4OTh7yyE.jpg)
```

---
## \#134 Posted by: Kug3lis Posted at: 2018-06-14T14:18:04.717Z Reads: 358

```
Most enterprise electronics engineering apps doesn't even work correctly in Win 10 (That's why I am still in win 7)
```

---
## \#135 Posted by: Pimousse Posted at: 2018-06-14T14:34:08.054Z Reads: 356

```
Because they were written at a time when Win10 didn't exist.
No offense, but what's the value of your post ?
```

---
## \#136 Posted by: Kug3lis Posted at: 2018-06-14T14:48:56.523Z Reads: 348

```
They are constantly updated but still suck on win10...

Same as yours?
```

---
## \#137 Posted by: Pimousse Posted at: 2018-06-14T14:56:53.924Z Reads: 348

```
Yes, you're right. I'm sorry man.
```

---
## \#138 Posted by: Manu39 Posted at: 2018-06-14T18:29:45.128Z Reads: 344

```
I think I found the problem: in settings / various the option multiply the data was activated ... by deactivating the change of mode no longer poses any problem apparently ...
here it can help you too.
```

---
## \#139 Posted by: Pimousse Posted at: 2018-06-14T18:47:07.361Z Reads: 343

```
Thanks for the hint @Manu39 !
Anyway, I wrote few lines for the SmartRing that allows you to restart the communication then restart the program if it still can't communicate.
I send it to you ;)
```

---
## \#140 Posted by: Manu39 Posted at: 2018-06-14T18:51:13.918Z Reads: 345

```
you are a boss @Pimousse . thx
```

---
## \#141 Posted by: Necromenz Posted at: 2018-06-14T19:10:20.117Z Reads: 382

```
yesterday the package reached me and I am  very excited about the new module.
After i installed the Modul i Update the FW of my both VESC6 without any Problem.
![20180612_112749|374x500](upload://nYMkHnLgW4b1EE7w2bdAopi0xxV.jpg)
![20180614_181244|666x500](upload://x5J77iYCDz1xiejLewSKbm6BsZJ.jpg)
![Screenshot_20180614-184950_metr|243x500](upload://fSe9Huzz8rIXsuoQRAQO2sFgDt2.jpg)![Screenshot_20180614-185153|690x335](upload://lyZ6FMdkG8iH4kAt47NtRN0nQi0.jpg)
```

---
## \#142 Posted by: Yecrtz Posted at: 2018-06-14T21:53:26.228Z Reads: 366

```
Got the module!

![Screenshot_20180614-233104|236x500](upload://6O8sN9nhZzVdM6QNzoYD516qMkt.jpg)

However, I can't get @Ackmaniac's app (esc monitor) to find the module.
```

---
## \#143 Posted by: Yecrtz Posted at: 2018-06-14T23:10:47.323Z Reads: 366

```
Allright, just did a 14km test dride. Checked 3 times during the ride and every time I opened the app the module wasn't connected anymore and there was no ongoing track. Every time a sec later the module connected back but no trace of the previous started record. Of that whole trip it saved 1.5km to my daily stats.. Oh and I didn't even step off my board.. I'll send you the logs @rpasichnyk 

Using the version without extra entenna and have an abs enclosure. Only had like 3 disconnects ever with the old module in the last 1.5 year..

Edit: allright gents, Android decided to turn back on battery optimization for me again. Without telling me, I suspect it randomly does this after updating the app. If you have any issues, check if it is still off for you. Even if you did turn it off just a day before.

Edit 2: module is still disconnecting. Even after a seven minute ride.
```

---
## \#144 Posted by: Pedrodemio Posted at: 2018-06-15T11:56:14.207Z Reads: 363

```
@rpasichnyk if used on a 4wd board, does the modules have enough bandwidth to send all 4 VESC’s data now?
```

---
## \#145 Posted by: Manu39 Posted at: 2018-06-15T14:44:29.526Z Reads: 368

```
![IMG_1923|666x500](upload://iSaOBlqGf2JC8fp19KS7WyhyKgV.jpg)
here is metr.pro @rpasichnyk in function duo with the Smart Ring @Pimousse  ... again thank you for your work.
```

---
## \#146 Posted by: Pimousse Posted at: 2018-06-15T14:47:37.495Z Reads: 354

```
This is an absolute beauty ! Glad you love the SmartRing !
And again, thank you so much for being my beta tester. :smile:
```

---
## \#147 Posted by: Yecrtz Posted at: 2018-06-15T20:16:35.896Z Reads: 350

```
Smart ring? What did I miss?

Metr pro module seems to work brilliant btw, app just has disconnection issues when the screen doesn't stay on :sweat_smile:
```

---
## \#148 Posted by: Manu39 Posted at: 2018-06-16T06:17:23.870Z Reads: 356

```
[quote="Yecrtz, post:147, topic:57780"]
Smart ring? What did I miss?

[/quote]

to make simple Smart Ring by @Pimousse  is a gauge that gives a return of the remaining battery, engine temperature, accelerator ... but also a lighting / rear brake light
[https://vimeo.com/265188386](https://vimeo.com/265188386)
```

---
## \#149 Posted by: willumpie82 Posted at: 2018-06-16T14:17:33.773Z Reads: 355

```
Hi @rpasichnyk

Today I received my metr pro, neat device! thanks!

had some trouble connecting to android P but worked after a few tries
```

---
## \#150 Posted by: Yecrtz Posted at: 2018-06-16T15:05:48.415Z Reads: 353

```
Curious if you can make a ride with 'keep screen on' turned off and phone locked without losing connection after 200 meters...
```

---
## \#151 Posted by: Manu39 Posted at: 2018-06-17T06:20:37.466Z Reads: 353

```
1st test of the metr.pro module:
[Url] https://metr.at/r/7v7kX [/ url]
Night out of 13 kms with 60% road and 30% way.
Tested the different modes that I programmed everything works nickel,
The phone was on the VAE of a friend which allowed us to test the range of the signal: 50 meters ...
```

---
## \#152 Posted by: ElskerShadow Posted at: 2018-06-17T12:43:38.212Z Reads: 341

```
@rpasichnyk @hexakopter any tizen app for smart watch? We are a lot with Samsung wearable would be could if we could as well have the feature that wear OS and apple watch have
```

---
## \#153 Posted by: Surfer Posted at: 2018-06-17T12:48:13.193Z Reads: 345

```
Hi, I try the perimeter inside the metr, I could read the settings but I can't write.
When I try to write it says communication error, the module is attached to the slave, could be the reason?  
@rpasichnyk your app is like next level dude, congrats !!
```

---
## \#155 Posted by: rpasichnyk Posted at: 2018-06-17T17:43:13.536Z Reads: 356

```
[quote="bevilacqua, post:132, topic:57780"]
is it possible to lower the update interval when using Metr-Pro?
[/quote]
The "Update Interval" setting does not make any difference when connected to Metr Pro. The module determines "Uptate Interval" on it's own (currently about 70ms). This setting is only useful with the old modules.

[quote="Pedrodemio, post:144, topic:57780"]
does the modules have enough bandwidth to send all 4 VESC’s data now?
[/quote]
It does, but this is not yet implemented in the metr app.

[quote="ElskerShadow, post:152, topic:57780"]
any tizen app for smart watch?
[/quote]

I hope I will have time for it right after summer.


[quote="Surfer, post:153, topic:57780"]
When I try to write it says communication error, the module is attached to the slave, could be the reason?
[/quote]

The reason might be that you are using old module and VESC firmware that has low packet timeout. Please try again and right after that go to Settings → Show Logs and email to me.
```

---
## \#156 Posted by: zyphaz Posted at: 2018-06-17T23:25:31.297Z Reads: 355

```
Received my Metr Pro today as well!  I keep getting prompted for a PIN though.  I've tried defaults with no luck.

![Screenshot_20180617-162257|281x500](upload://h5jB9o1ZQ205beNrvJdmlpS1RJ1.png)
```

---
## \#157 Posted by: Jc06505n Posted at: 2018-06-17T23:36:21.970Z Reads: 323

```
I thought tone pin was on the receiver itself like on the post
```

---
## \#158 Posted by: zyphaz Posted at: 2018-06-18T00:07:40.644Z Reads: 322

```
 :man_facepalming: Thanks!  That's the equivalent of a major RTFM.
```

---
## \#159 Posted by: E1Allen Posted at: 2018-06-18T00:32:28.708Z Reads: 324

```
[quote="Manu39, post:151, topic:57780"]
nickel
[/quote]

What is this nickel you speak of?
```

---
## \#160 Posted by: Manu39 Posted at: 2018-06-18T07:11:23.774Z Reads: 333

```
[quote="E1Allen, post:159, topic:57780"]
What is this nickel you speak of?
[/quote]

I'm talking about programming and loading different modes from the apps to the ESCAPE
```

---
## \#161 Posted by: Pimousse Posted at: 2018-06-18T07:14:24.614Z Reads: 341

```
Ahah, this comes from French.
We say "Nickel !" like "Great !" :smile:
```

---
## \#162 Posted by: sk8l8r Posted at: 2018-06-18T07:50:28.684Z Reads: 344

```
[quote="zyphaz, post:156, topic:57780"]
tried defaults with no luck
[/quote]

did you try the number printed on the device?
```

---
## \#163 Posted by: pakue Posted at: 2018-06-18T08:06:31.421Z Reads: 329

```
I there a chance to use the module in combination with an UART remote (like wii nunchuck)? E.g. hooking the module up to a CAN slave and the remote to the master.
```

---
## \#164 Posted by: Pimousse Posted at: 2018-06-18T10:05:32.826Z Reads: 337

```
This is not a problem.
```

---
## \#165 Posted by: sk8l8r Posted at: 2018-06-18T10:38:03.075Z Reads: 303

```
setup metr pro with dual focbox in canbus over the weekend - really pain free :)
```

---
## \#166 Posted by: zyphaz Posted at: 2018-06-18T11:58:13.046Z Reads: 307

```
Thanks, yeah @Jc06505n pointed that out and I'm up and running now.:call_me_hand:
```

---
## \#167 Posted by: ducktaperules Posted at: 2018-06-18T15:14:17.068Z Reads: 319

```
@rpasichnyk is there any difference in the hardware between the module with/without external antenna? 

Eg. if i get the version without external antenna can i fit one at a later date if needed? or do they have other differences in hardware / firmware?
```

---
## \#168 Posted by: lazopm Posted at: 2018-06-18T15:26:38.211Z Reads: 324

```
First commute with the module [https://metr.at/r/dx5OE](https://metr.at/r/dx5OE)
A wasp flew into my shirt and stung me twice, but the module worked great.
Super easy setup, 10/10.
```

---
## \#169 Posted by: bevilacqua Posted at: 2018-06-19T09:04:20.990Z Reads: 332

```
[quote="rpasichnyk, post:80, topic:57780"]
please be aware that modules with antenna and without antenna have 0R resistor soldered in a different position. But with a good soldering equipment it should be easy to resolder.
[/quote]
There you have it
```

---
## \#170 Posted by: Manu39 Posted at: 2018-06-19T12:35:27.220Z Reads: 346

```
If you are like me to know with a module Metr.pro ideal to connect his board in Bluetooth 4.0 but your iMac is like mine too old (2008) so without BLE 4.0 (appeared at apple in 2013 it seems to me) here's how make:
1 / Buy this USB stick bluetooth 4.0:
https://www.amazon.fr/gp/product/B007ZT2AXE/ref=ya_st_dp_summary?ie=UTF8&psc=1

2 / Download this dmg:
Hardware IO tools for Xcode 7.3
http://www.k-upload.fr/afficher-fichier-2018-06-19-1f47a6302hardwareioto.dmg.html
3 / Install the DMG and open Bluetooth Explorer
Then in the bar at the top of your Mac click on TOOLS / HCI Control Selector and finally choose from the Broadcom Corp. drop-down menu.

4 / pair your keyboard again or mouse or trackpad ...

Turn on your board, open VESC Tools and connect in BLE

;)
```

---
## \#171 Posted by: caustin Posted at: 2018-06-20T23:17:38.006Z Reads: 315

```
Missing something, I have used thread procedure to pair MetrPro on Windows fine.  But not seeing the VescTool connection tab for Bluetooth LE, and thus BLE device.  Do I need a different new Vesc Tool download sw?  Currently using pretty old version of Vesc Tool Original v0.84 on Windows...sounds like I am using older version if someone can send link?
```

---
## \#172 Posted by: webst Posted at: 2018-06-20T23:32:04.052Z Reads: 315

```
https://www.electric-skateboard.builders/t/metr-pro-next-gen-bluetooth-module/57780/123?u=webst
```

---
## \#173 Posted by: Riako Posted at: 2018-06-22T09:25:26.437Z Reads: 325

```
hey guys,
just receive mine yesterday :+1: 
Want to try with all the good feature so,
following Roman step, I dl for windows from github, when I unzip the rar files, and run (double clic exe file) VESCTOOL, I just got this : 
https://amadridefr.files.wordpress.com/2018/06/capturetov.jpg
What should I do now ? :sweat_smile:
```

---
## \#174 Posted by: bevilacqua Posted at: 2018-06-22T09:35:34.813Z Reads: 313

```
could stick to TCP. Now it is fast enough to flash (ca. 1-2min per VESC).
```

---
## \#175 Posted by: rpasichnyk Posted at: 2018-06-22T09:38:14.493Z Reads: 323

```
@Riako I guess you are running Windows 7. It is old and does not have built-in BLE support. Install Windows 10. Then check post #94 for more details

http://www.electric-skateboard.builders/t/metr-pro-next-gen-bluetooth-module/57780/94?u=rpasichnyk
```

---
## \#176 Posted by: Riako Posted at: 2018-06-22T10:00:49.690Z Reads: 310

```
Ho, sorry bro, missed the windows info in all that ! (If you could update 1st post it could help for future buyer or user).
... It going to be a long way for me if I need that :sweat_smile:, all my stuff and softwares seens 2012 will stay and work with it well !?.. I have doubts about some ... 
Ok, I'd better try the PCB antenna without the new fw and BLE connection to VESC TOOL for now ...
```

---
## \#177 Posted by: Sn4pz Posted at: 2018-06-22T11:15:33.699Z Reads: 298

```
Could you run it in virtual box? If it's just software you're missing then it seems like it might work(?)
```

---
## \#178 Posted by: Pimousse Posted at: 2018-06-22T13:57:24.688Z Reads: 294

```
Yep, install an Ubuntu virtual machine.
I can help you bro ! ;)
```

---
## \#179 Posted by: ducktaperules Posted at: 2018-06-22T13:58:48.833Z Reads: 305

```
how long does it usually take to ship these modules to uk?
```

---
## \#180 Posted by: wafflejock Posted at: 2018-06-22T14:01:27.293Z Reads: 318

```
Took about a week to get to the US and coming from Germany so probably faster to UK

![Screenshot_20180622-090218|281x500](upload://zg2iVfEhbE0Gee6DOavAUJSncrg.png)

Pretty sure I ordered on the 12th and had tracking the next day.
```

---
## \#181 Posted by: bevilacqua Posted at: 2018-06-22T14:29:13.902Z Reads: 296

```
Hi Roman (@rpasichnyk), 

Is there any plan to add the dual Telemetry to the records tab? 
Motor Temp1 and M.T2, ESCTemp1 and 2 etc etc... 

Thanks for your continuous work :)
```

---
## \#182 Posted by: laurnts Posted at: 2018-06-22T15:00:42.253Z Reads: 293

```
TESTED on Pixel 2, Flawless! @rpasichnyk Nice one!
```

---
## \#183 Posted by: wafflejock Posted at: 2018-06-22T15:40:10.825Z Reads: 303

```
So far appears to be working well also at some point the background tracking started working on my phone too (works with old module, may have been that I toggled off the prefer GPS since imagine the background GPS data is pretty limited).  Anyhow need to replace my battery box so I can go ride without having everything velcro(ed) together.  Nexus 5 here.
```

---
## \#184 Posted by: Riako Posted at: 2018-06-22T18:12:18.142Z Reads: 310

```
haaaahaha ...  :sweat_smile: it dont work too on my w10 computer 
https://amadridefr.files.wordpress.com/2018/06/rps20180622_200833.jpg?w=640
_this application can not run on your PC_
ok Pimousse, thx a lot as usual bro !!!!
```

---
## \#185 Posted by: Riako Posted at: 2018-06-23T09:07:15.190Z Reads: 303

```
Ok so, to understand well, I dl the 1.8Go _Ubuntu_ file ... doesn't understand how it is supposed to work on "_ubuntu_" if it didn't on the real windows 10 ...  Need to make this thing work pleeaaase :sob::upside_down_face:

I buy it cause the last (old) one never really work more than 500m/ride, I totalize around 2 or 3km for the last year (where I made more than 500/1000km). So after riding all the good work made (even if it never worked before), I buy a new module with external antenna (cause you said if we got pb before its better), I receive it without antenna ... discover after there wasn't working one my like you said "old PC" who works better than the w10 one ... but don't work also on my Windows 10 haaaaaaaaaaaa who was supposed to be the solution ...

haannn :sweat_smile: so I should instal _ubuntu_ on my w10 computer to do what ?..
```

---
## \#186 Posted by: Yecrtz Posted at: 2018-06-23T09:38:49.747Z Reads: 302

```
![Screenshot_20180623-113607__01|457x500](upload://wKG36qjWtAjVGuLPTTaR6ARrG.jpg)

Mmmh :thinking:
```

---
## \#187 Posted by: rpasichnyk Posted at: 2018-06-23T09:41:51.699Z Reads: 286

```
@Riako do you have 32 bit or 64 bit Windows 10? You need 64 bit.
@Yecrtz Logs please :) thx
```

---
## \#188 Posted by: Yecrtz Posted at: 2018-06-23T11:58:38.434Z Reads: 285

```
@rpasichnyk happened 8 days ago after I updated the app..
```

---
## \#189 Posted by: i2oadsweepei2 Posted at: 2018-06-23T12:06:12.849Z Reads: 294

```
I received my module. Thanks guys! The build continues.

For anyone interested my module was shipped on the 9th or 10th and was brought to my door on the 20th. I’m in Ontario Canada. Near Toronto. There were no extra fees or duties though that would have been my responsibility anyway. 👍
```

---
## \#190 Posted by: Skifree Posted at: 2018-06-24T18:01:16.261Z Reads: 300

```
Not sure if you've found your solution yet, but I have the galaxy s6 and after it updated to Oreo, my module stopped working. I then realized it was a [clone of a clone](https://blog.yavilevich.com/2017/03/mlt-bt05-ble-module-a-clone-of-a-clone/)  called the MLT-BT05. I bought a genuine HM-10 from robotshop on Amazon, and it now works flawlessly.
```

---
## \#191 Posted by: Mathias Posted at: 2018-06-25T00:51:23.164Z Reads: 305

```
I got my module and the both the VESC tool and the metr app are working nicely on my android phone. Thanks @rpasichnyk and @hexakopter! So awesome to finally have riding modes with the default firmware!

I have two issues with the metr app though: 
1) it seems that it ignores the regenerated energy when calculating the Wh/km. 
2) Could you enable custom discharge curves in the battery setup? I assume you just interpolate from a table? I set my app to Li-Ion but it seems to be pretty far off from 30Qs, which I'm using. So the % displayed doesn't fit my battery at all. This would also be nice for people that e.g. use different voltage cutoffs and so on. 

Another thing, which is not a big deal, but it might be nice if the battery percentage is averaged over a few seconds in the realtime display. The voltage readout on the vesc is so noisy that the battery display "flickers" around like crazy and is just not that nice to look at.
```

---
## \#192 Posted by: rpasichnyk Posted at: 2018-06-25T16:20:30.285Z Reads: 303

```
![mov|300x397](upload://4jc4lIZJrRGJbJraYtO8vAPSUn4.gif)

Flickering is a reminder how fast Metr Pro is.
Good stuff, not a bug ;)
```

---
## \#193 Posted by: strattos Posted at: 2018-06-25T16:32:18.473Z Reads: 290

```
Haha the perfect response. Percentage indicators don't work unless you set them up according to your batteries.

Lookup a discharge curve for the 30Q's and base your percentages from that people! 


On another note hopefully my metr pro's show up this week so I can install them.
```

---
## \#194 Posted by: Mathias Posted at: 2018-06-25T18:29:18.023Z Reads: 292

```
That was a quick fix quick :wink: Just got the updated app!
Thanks, @rpasichnyk!

[quote="rpasichnyk, post:192, topic:57780"]
Flickering is a reminder how fast Metr Pro is.
Good stuff, not a bug :wink:
[/quote]

 Well, yeah... It's a cosmetic detail. Just a suggestion how to make the battery level more accurate. The app is already pretty nice as it is. Especially with the freely configurable RT display.
```

---
## \#195 Posted by: oyta Posted at: 2018-06-25T21:15:51.738Z Reads: 279

```
Niiiice! I have been waiting for this :slight_smile:
```

---
## \#196 Posted by: banjaxxed Posted at: 2018-06-25T21:59:25.386Z Reads: 292

```
I think I’ll have to try one of these, but what would be nice is a shorter JST cable option so as not to have a big loop(space issues) as I would get the external antenna and place it in one of @Kug3lis focbox dual esc enclosures. A small hole drilled to mount the antenna
```

---
## \#197 Posted by: Skitzor Posted at: 2018-06-26T21:22:16.831Z Reads: 292

```
I know it's a matter of firmware/software update. But the Metr has a basic encryption somehow. startbit/endbit whatever. I'm too busy to find out. I have some genuine HM10's but they would not connect to Metr. It's a good basic app, but I mostly like the smartwatch feature. I wish I could use it again. I'm not gonna downgrade one of my cellphones for this
```

---
## \#198 Posted by: Exigent Posted at: 2018-06-27T00:37:05.513Z Reads: 297

```
Yeah. There's nothing special about the antenna. As long as you have the right connector you can use whatever "antenna" you want as long as it's for the right frequency band. Making your own custom antenna isn't at all difficult and amateur radio (and other) websites offer lots of help.
```

---
## \#199 Posted by: Cobber Posted at: 2018-06-27T06:50:38.600Z Reads: 294

```
Got my 2 x Metr Pro modules today, thanks guys, look SAF :sunglasses:
```

---
## \#200 Posted by: banjaxxed Posted at: 2018-06-27T12:06:05.616Z Reads: 286

```
The app is restricted to metr hm-10 MAC addresses afaik, you can install the app but it will only connect to devices in that master list
```

---
## \#201 Posted by: ducktaperules Posted at: 2018-06-27T13:11:34.028Z Reads: 287

```
just received my module but having problems connecting from pixelXL. Open app and device shows up. Hit connect and the app says connected. I then get the pairing prompt. if i type a random pin it said "incorect pin" but if i type the number on the back it just turns the red light on and pairing restarts again.
```

---
## \#202 Posted by: hexakopter Posted at: 2018-06-27T14:10:39.536Z Reads: 289

```
@ducktaperules
Every single Metr Pro module is tested with its pin code on the back, the JST cable it comes with and if realtime data/recording works flawlessly before it is shipped. So the pin code on the back of your module should work.
Have you tried to power down your VESC, force close the Metr app, turn off bluetooth on your phone, turn back on bluetooth on your phone, power on your VESC and reopen the Metr app? After that try to connect to the module again. If that does not work please send us the log file and we will figure out what went wrong.
```

---
## \#203 Posted by: ducktaperules Posted at: 2018-06-27T14:56:02.006Z Reads: 284

```
Seems to be working now. I tried everything and nothing worked, then i restart my phone and it connected first time after :)
```

---
## \#204 Posted by: squad Posted at: 2018-06-27T15:50:24.910Z Reads: 293

```
Ordered one, couldn’t resist 🤷‍♂️ I think the antenna will look nice on my eMTB. I think now I need to add another one for the remote receiver, for the sake of symmetry of course 😂
```

---
## \#205 Posted by: E1Allen Posted at: 2018-06-27T22:03:03.788Z Reads: 279

```
Do you know which pins on the jst connector are required?  Is it the same as the metr module?
```

---
## \#206 Posted by: hexakopter Posted at: 2018-06-27T23:49:05.120Z Reads: 293

```
@ducktaperules Glad that it works for you now.

@E1Allen You need to connect **3.3V, GND, TX** and **RX**. TX and RX can be swapped, Metr Pro will auto detect that on startup and work anyway. So no more trouble with the right TX/RX placement. :smiley:
**It is not possible to power your module with 5V!** 5V is just routed so you have the 7pin count like on most VESCs (so it is only possible to plug it in one way) and to have 5V accessible for future accessories that would need it. So right now the 5V isn't connected to anything so **can not** be used to power your Metr Pro. 3.3V is required to power your module.
SWD and SWC pins are just used for initial flashing so you can let them unconnected. Firmware updates are possible over the air, so no SWD necessary.
```

---
## \#207 Posted by: E1Allen Posted at: 2018-06-28T01:35:42.874Z Reads: 293

```
Thanks, I have the CNC focbox case and the three extra wires made it a tight fit.  It works, easier with four wires.
```

---
## \#208 Posted by: flyingox Posted at: 2018-06-28T21:31:28.735Z Reads: 296

```
Hi, 
Metr-pro BT module and app working well but unable to use with Ackmaniac-Esc monitor app.  I'm using Dual Vesc6 and latest EXTENDED ACKMANIAC-ESC Tools 3.102 and Android 7.  This app works with BT5 module.  Small point I notice Metr-pro firmware update option doesn't show latest firmware.  Finally compiled latest version of ESC tools for Linux and and Win and was unable to connect using bluetooth, is it possibly only select versions are supported?
```

---
## \#209 Posted by: Jc06505n Posted at: 2018-06-29T00:55:00.672Z Reads: 294

```
[quote="rpasichnyk, post:1095, topic:13483"]
I was looking at this issue yesterday and unfortunately I can confirm that Metr Pro modules no longer work with the latest ACKMANIAC-ESC Monitor app. The latest apk version that works is 1.101 (I got it from here [https://apkpure.com/ackmaniac-esc-monitor-unreleased/ackmaniac.vescmonitor/download/143-APK?from=details%2Fversion ](https://apkpure.com/ackmaniac-esc-monitor-unreleased/ackmaniac.vescmonitor/download/143-APK?from=details%2Fversion)) I will try to contact Nico and ask for help
[/quote]

10 character
```

---
## \#210 Posted by: Brad Posted at: 2018-06-29T01:36:14.410Z Reads: 287

```
Awesome work.Unfortunately I already bought 2 older models but should these fail, the new ones will be next!
```

---
## \#211 Posted by: caustin Posted at: 2018-06-29T01:37:32.985Z Reads: 284

```
@Ackmaniac Nico, can you help with this as do not want to revert back to your Vesc Monitor app v1.01 but would like to use your app with Metr Pro as well as the 2 BLE chips I have from you on other builds.
```

---
## \#212 Posted by: E1Allen Posted at: 2018-06-29T01:49:36.910Z Reads: 307

```
I really like the modes.  I should have switched to canbus earlier. Being able to set specific speeds on the fly is awesome.  Having a super chill mode for the kids is great

https://metr.at/r/06w2N

Also like the dual display.  The more info the better 😁😁
You can see the increased refresh rate when the data populates.  I like it a lot.

https://metr.at/r/Q2GBh
```

---
## \#213 Posted by: mmaner Posted at: 2018-06-29T20:31:59.747Z Reads: 304

```
Im having issues getting my Metr Pro up & running.  I am running dual FocBox's with Ack's 2.54 with Can Bus.  

This is all I see is...
![image|281x500](upload://p9rix53fmTAvZqyS1KqukfzfxTW.jpg)

Oddly, this is what I see on the Settings tab...
![image|383x180](upload://tx53rX5XE41tZNC6nzV0MiOXxPq.jpg)

It's weird that the app sees the Metr Pro version but not the VESC firmware or hardware version.  On the adaptor itself the blue light is solid when it connects, then starts a double blink every 2 seconds, but its not the same as when its not connected.  The green light is solid.  No red light at all.  

I've rebooted and restarted my phone multiple times.  Its a Pixel running Android 8.1.  I pu my old HM-10 on the 2nd VESC and it still works fine with Ack's app.  Ack's app does not show any data when connected to the Metr Pro.

@rpasichnyk any suggestions?

* Edit:  I uninstalled and reinstalled the app 2 times, PeriMetr also does not see the Metr Pro module.
```

---
## \#214 Posted by: rpasichnyk Posted at: 2018-06-29T20:48:52.741Z Reads: 287

```
Try to unplug HM-10 and put it aside. Plug Metr Pro there instead. If it still shows no data, please send log to rpasichnyk@icloud.com
```

---
## \#215 Posted by: mmaner Posted at: 2018-06-29T20:51:13.175Z Reads: 288

```
I just put the HM-10 in as a last effort to be able to get data before I closed up the enclosure.  I attempted to run the Metr Pro module on both VESC's.  Ill send you the logs in just a few mins.  Thanks for the quick response.
```

---
## \#216 Posted by: mmaner Posted at: 2018-06-29T20:58:16.907Z Reads: 285

```
logs sent, thanks again.
```

---
## \#217 Posted by: ElskerShadow Posted at: 2018-06-30T10:58:28.283Z Reads: 284

```
Guys I was wondering the metr pro can't be used with escape right?
```

---
## \#218 Posted by: Surfer Posted at: 2018-06-30T11:00:27.931Z Reads: 286

```
Why not? I don't see any reason to not work with. UART is standard protocol.
```

---
## \#219 Posted by: ElskerShadow Posted at: 2018-06-30T11:02:37.032Z Reads: 283

```
I remember reading somewhere the JST port was reversed
```

---
## \#220 Posted by: ElskerShadow Posted at: 2018-06-30T11:08:42.141Z Reads: 304

```
![1530356880338|375x500](upload://9ZZ59MGEJMD1v0c0BjMaqx0hVYH.jpg)
Everything is reversed in the labeling!
Anyone know something?
```

---
## \#221 Posted by: E1Allen Posted at: 2018-06-30T13:03:33.050Z Reads: 308

```
![image|281x500](upload://iAGj0ziGFtoL5RPHojOA14dYlHg.jpeg)If it's reversed just switch those pins. It's super easy and simple with a razor blade or knife tip.  It just has to be Sharp to grab the release tab.

Edit: I had to remove all the pins to slide it through the rubber grommet for the CNC case.

Slightly lift tab in yellow, so it releases from the part marked red.
```

---
## \#222 Posted by: banjaxxed Posted at: 2018-06-30T23:36:32.706Z Reads: 300

```
Hey did you change the baud rate Mike? Oh and UART enabled 

Sounds like something I didn’t do and get similar...but maybe you’ve used em before and not that simple
```

---
## \#223 Posted by: mmaner Posted at: 2018-07-01T00:11:05.709Z Reads: 304

```
I tried with 9600 and 115200 BPS but neither worked. My understanding is that it's supposed auto sense and negotiate the baud rate rate. 

I've got it set to PPM and UART.  Thanks though.
```

---
## \#224 Posted by: caustin Posted at: 2018-07-01T01:08:02.074Z Reads: 308

```
Yes, I tried Metr Pro with both baud rates and it stepped up and down to find each correctly. Have you been able to get your Metr Pro chip working with any configuration, device, software?
```

---
## \#225 Posted by: caustin Posted at: 2018-07-01T01:09:36.467Z Reads: 296

```
Tried a spare uart cable and connectors?  I am not seeing where your issue is, frustrating.
```

---
## \#226 Posted by: mmaner Posted at: 2018-07-01T01:33:21.816Z Reads: 298

```
I haven't gotten it to work, it connect fine but no data.  The green ought is solid and the blue light blinks twice every 4 seconds. I haven't tried a different uart cable, I'll try that when I get back to the office.
```

---
## \#227 Posted by: Pimousse Posted at: 2018-07-06T11:18:40.411Z Reads: 303

```
Hi Roman !
Found some spare time to test this Metr Pro.
First, as we told, JST connector has to be swapped.

First feedback after a quick try : 
- My Macbook Pro can't see the Metr Pro (MacBook Pro 2017).
- In the parameter menu of the module (where you can change the name and see FW infos), the module says that VESC FW is up to date even if it can't communicate with it.
- No problem on Android 8, OnePlus 5T
- TCP bridge works amazingly fast comapred to the previous module ! That makes direct connection to the laptop less needed as this works flawlessly.

Thank you very much again, can't wait to play more with this piece of engineering.
```

---
## \#228 Posted by: sk8l8r Posted at: 2018-07-06T11:56:19.820Z Reads: 291

```
can someone recommend an Android watch that works with Metr?
```

---
## \#229 Posted by: TarzanHBK Posted at: 2018-07-06T12:11:23.066Z Reads: 292

```
I´m running a Sony Smartwatch 3. Cheap, good and works with everything what you throw on it :slight_smile:
I posted a photo here somewhere with it running Ack´s app
```

---
## \#230 Posted by: TarzanHBK Posted at: 2018-07-06T12:13:55.492Z Reads: 295

```
found it:
https://www.electric-skateboard.builders/t/extended-bldc-tool-with-watt-control-mode-ppm-cruise-control-individual-throttle-curve-and-android-app/12286/1312
```

---
## \#231 Posted by: ElskerShadow Posted at: 2018-07-06T12:14:33.787Z Reads: 289

```
I recently bought a Fossil smart watch, it's really great. There was an offer I only paid 130 € instead of 160
The quality and style is really cool, like all the classic Fossil watch.
Sold my gear S2 because tizen is not supported 😭😭
```

---
## \#232 Posted by: banjaxxed Posted at: 2018-07-06T12:18:27.337Z Reads: 285

```
How is it with esk8 apps?
```

---
## \#233 Posted by: ElskerShadow Posted at: 2018-07-06T12:55:22.414Z Reads: 292

```
Should work fine I have not the occasion to try yet. I'll post here what I think when I can! Just the watch by itself works really well
```

---
## \#234 Posted by: rpasichnyk Posted at: 2018-07-06T13:09:00.233Z Reads: 297

```
Make sure the smartphone is not stealing BLE connection (turn off bluetooth) and that you are using VESC Tool that has this fix on your Macbook

https://github.com/rpasichnyk/vesc_tool/commit/1e5cfcff8855f18ee9711c9bd330dc809d1076f5
```

---
## \#235 Posted by: Pimousse Posted at: 2018-07-06T13:15:39.045Z Reads: 289

```
I switched off Blutooth on the phone and use your VT (latest Mac version in Release tab).
I couldn't see the module in Mac bluetooth menu for pairing before connecting VT through BLE.
```

---
## \#236 Posted by: rpasichnyk Posted at: 2018-07-06T13:29:55.930Z Reads: 283

```
On macOS you do not need to perform the pairing manually. Just open the VESC Tool and Scan for BLE devices. It might take some time, like 30 seconds
```

---
## \#237 Posted by: Pimousse Posted at: 2018-07-06T13:45:23.137Z Reads: 290

```
Well ok, I'll again later.
As you stated that the Metr Pro wouldn't bypass serial commands coming from unpaired deviced, I didn't even try scanning in VT.
```

---
## \#238 Posted by: rpasichnyk Posted at: 2018-07-06T14:08:46.777Z Reads: 300

```
No it wouldn't. On macOS you need to perform pairing too. The difference is that Windows doesn't allow apps to initiate pairing procedure, it has to be done by the user in the Control Panel. Hence I wrote a separate post describing how to do it. With macOS it's much more intuitive, everything is done in the app.

![34|690x308](upload://vwycLVhw5rbQ4WdO4KprLGyAQ7Q.png)
```

---
## \#240 Posted by: bevilacqua Posted at: 2018-07-07T14:49:02.166Z Reads: 291

```
normal vesctool works on mac just thanks to roman. 
At least the BLE functionality
```

---
## \#241 Posted by: ElskerShadow Posted at: 2018-07-09T09:38:55.953Z Reads: 298

```
![1531128964493|375x500](upload://zWF20zKpCcdBvc5H7juDBy7aOkf.jpg)
I love the watch!
And it works great, the only thing I miss is the heart rate sensor because over the years I was used to have a constant monitoring of that. I guess that's a trade-off.
```

---
## \#242 Posted by: banjaxxed Posted at: 2018-07-09T09:47:19.893Z Reads: 292

```
Slick, were you able to chose what data is presented and how many can you squeeze in?
```

---
## \#243 Posted by: ElskerShadow Posted at: 2018-07-09T10:09:33.275Z Reads: 291

```
You can choose what's on the screen, I couldn't put anything more than 2 data
Anyway tbh you just do quick glance when you ride
If you want precise info you go on your phone after the ride
```

---
## \#244 Posted by: sk8l8r Posted at: 2018-07-09T11:07:24.562Z Reads: 292

```
that does looks pretty cool, can't believe I'm buying a watch to just wear ek8ing lol
```

---
## \#245 Posted by: AndyBigD Posted at: 2018-07-09T11:23:27.165Z Reads: 295

```
You're not the only one!
I don't wear watches, but was looking into them purely for esk8ing, when a work-mate tells me he has an old Sony SmartWatch 3 he no longer needs so £30 later I have a wrist-mounted speedo and battery meter ready to go!
```

---
## \#246 Posted by: Jamy Posted at: 2018-07-10T16:03:58.560Z Reads: 298

```
Hey @rpasichnyk, I just got my Metr Pro module, and so far I think it's possibly the coolest upgrade I've done for my board.

I noticed 1 bug though. Sometimes it will write the 2nd vesc's hall sensor config to Vesc 1. Since those are different on my board, the vesc 1 motor will not spin at slow speed anymore until I do a redetect through the vesc tool.

Using vesc FW 3.38 on both vescs (Raptor 2, FOCBOX)
```

---
## \#247 Posted by: rpasichnyk Posted at: 2018-07-10T16:22:24.801Z Reads: 297

```
Nice find! Very interesting bug. Can you please go to Settings -> Show Log and send to rpasichnyk@icloud.com? This way I can see your configuration and it will be easier to reproduce the problem here :slight_smile:
```

---
## \#248 Posted by: Jamy Posted at: 2018-07-10T16:25:43.463Z Reads: 298

```
I'll do that as soon as I hit it again :)
```

---
## \#249 Posted by: hexakopter Posted at: 2018-07-10T20:11:44.932Z Reads: 314

```
Good news. Metr Pro modules with external antenna are back in stock. You can now also choose a smaller antenna as it was asked from the community. You can see a size comparison in the picture.
![ExternalAntenna|690x460](upload://7JqI8d3kZiNOelOKobVp1APbbzx.jpg)
The small antenna is 33mm long and 9mm in diameter.
```

---
## \#250 Posted by: i2oadsweepei2 Posted at: 2018-07-10T22:27:53.875Z Reads: 304

```
I like the small one. Was performance good? Will you sell them separate or show us where to get them? 

Thank you, great product 👍
```

---
## \#251 Posted by: caustin Posted at: 2018-07-11T00:52:54.786Z Reads: 306

```
That is great!

For those of us who have already purchased several of the metr chips with larger antenna, can you let us know how or where to purchase the replacement smaller antenna?  Pls pm me if necessary, thanks!
```

---
## \#252 Posted by: hexakopter Posted at: 2018-07-11T10:00:47.171Z Reads: 317

```
I did not noticed any performance difference to the bigger antenna. When you compare antenna gain it is 2.5 dBi for the bigger antenna and 2.0 dBi for the smaller one. So in theory when mounted the antenna correctly you should get a slightly higher range because of the narrower and longer main lobe. But thats just theory and in reality you most likely will not notice. :slight_smile: The main advantage of the external antennas to be able mounting them outside your carbon enclosure or anything else dampening the electromagnetic field massively applys to both antennas. 

It would be possible for us to sell the antenna separately, but also without tracking number shipping is a lot more expensive then what is possible when ordering from China. So here a link where you can get those:
https://www.aliexpress.com/store/product/2-4GHz-Omni-Wifi-uhf-Antenna-Original-CDSENET-TX2400-JZ-3-SMA-Male-2-0dBi-2/2798183_32805526923.html
Feel free to contact us if you still want them from us to get faster shipping.
```

---
## \#253 Posted by: i2oadsweepei2 Posted at: 2018-07-11T11:31:37.265Z Reads: 305

```
Thank you for the fast reply and explanation 👍
```

---
## \#254 Posted by: banjaxxed Posted at: 2018-07-11T17:37:18.371Z Reads: 313

```
even cheaper?!

https://www.aliexpress.com/item/-/32848962210.html?spm=a2g0s.13010208.99999999.259.dcff3c00tWSfA3
```

---
## \#255 Posted by: hexakopter Posted at: 2018-07-11T20:05:57.817Z Reads: 302

```
Looks like it. I think it should work. You can also search for other small 2.4GHz antennas with the fitting connector on Amazon and eBay.
```

---
## \#256 Posted by: plasteroid Posted at: 2018-07-11T21:27:37.038Z Reads: 302

```
Looks good!   same price for small or large antenna?
```

---
## \#257 Posted by: Dmaxx Posted at: 2018-07-12T03:14:01.855Z Reads: 302

```
Hey @rpasichnyk, is there a way to switch from metric to imperial after uploading data? Sorry if this is obvious or already covered, but couldnt figure out how..
```

---
## \#258 Posted by: webst Posted at: 2018-07-12T07:52:48.729Z Reads: 307

```
Have you tried uploading it one more time after switching to metric?
```

---
## \#259 Posted by: rpasichnyk Posted at: 2018-07-12T08:43:30.122Z Reads: 308

```
@plasteroid yes same price

@Dmaxx you can change it like this
![mov|600x457](upload://djyKak05ucG0PsrLmvh4UrqhviB.gif)
```

---
## \#260 Posted by: sayekim Posted at: 2018-07-12T10:23:59.392Z Reads: 301

```
No f$&@in’ way 🤯
```

---
## \#261 Posted by: Dmaxx Posted at: 2018-07-12T14:34:57.255Z Reads: 296

```
😅 That is elegantly simple, so simple I overlooked!
```

---
## \#262 Posted by: Jamy Posted at: 2018-07-14T20:50:36.368Z Reads: 291

```
@rpasichnyk sent an email with logs about that bug. Also, feature request, is it at all possible to put the battery voltage besides the percentage?
```

---
## \#263 Posted by: webst Posted at: 2018-07-15T02:23:22.569Z Reads: 283

```
You know you can edit the screen by long touching?
```

---
## \#264 Posted by: sayekim Posted at: 2018-07-15T08:21:14.456Z Reads: 291

```
@rpasichnyk
I seem to have found two bugs.

When running perimetr and doing motor foc hall sensor detection the values aren’t written. 

The metr temp measurement in real time I had 90 degress Celsius motor temp but when uploading the recorded record it only shows top temperature 66 degrees Celsius max motor temperature.
```

---
## \#265 Posted by: rpasichnyk Posted at: 2018-07-15T13:22:36.679Z Reads: 290

```
@Jamy @sayekim thank you for bug reports, I will look at them! Yes, it is possible to show Voltage on the Realtime Tab, long press to enter layout editing mode and drag cells around, tap to enable/disable, press&hold to resize

Update: bug with FOC Hall Sensor detection confirmed. Working on it.
```

---
## \#266 Posted by: LoR_NiKoN Posted at: 2018-07-16T17:11:22.640Z Reads: 294

```
Hi @rpasichnyk Im sorry to be one of those guys and I'm probably doing/done something wrong but i've recently go one of your dongles, i've followed all the steps on the site and i'm not getting any data from my vesc's.

I've got it installed to my second vesc (ID1) which is set to PPM & UART and the UART is set to 115200 bps but i'm not getting any data through.

Even when clicking on the cog of the module in the app i see the metr pros version but its not pulling any version data from the vesc. i've tried this on stock 3.38 and also your custom 3.28 (if that's still valid) but either FW i'm not getting any telemetry.

Do you have any suggestions on why i may be having issues?

Many thanks in advance for your assistance.
```

---
## \#267 Posted by: rpasichnyk Posted at: 2018-07-16T17:23:52.713Z Reads: 286

```
Please go to Settings -> Show Log and send it to support@metr.at I’ll have a look
```

---
## \#268 Posted by: LoR_NiKoN Posted at: 2018-07-16T17:51:50.094Z Reads: 289

```
Thanks, I've emailed that over as requested.

Seeing a lot of NRF_SERIAL_EVENT_DRV_ERR in the logs..
```

---
## \#269 Posted by: LoR_NiKoN Posted at: 2018-07-16T22:46:46.773Z Reads: 289

```
Thank you @rpasichnyk for your assistance this evening getting this resolved.
```

---
## \#270 Posted by: rpasichnyk Posted at: 2018-07-17T04:09:51.086Z Reads: 293

```
Hey @mmaner how did it go with your Metr Pro module? I think @LoR_NiKoN had a very similar issue and what helped in the end is "forgetting" the module from iOS Settings -> Bluetooth and uninstalling and installing the app again from the App Store.
```

---
## \#271 Posted by: mmaner Posted at: 2018-07-17T11:55:11.576Z Reads: 279

```
My kids enclosure broke, I've been rebuilding his board. I'll try that today  It's Android though. Does that matter?
```

---
## \#272 Posted by: rpasichnyk Posted at: 2018-07-17T15:53:35.588Z Reads: 277

```
On Android you can also "Forget" / remove bluetooth devices saved on the system, try that together with switching bluetooth off and on, if you have the problem.
```

---
## \#273 Posted by: gmurad Posted at: 2018-07-18T12:48:54.265Z Reads: 277

```
Just purchased the metr pro without external antenna, I'm gonna use the ownboard ESC case.

My setup is 2 x Torqueboard VESC, just to confirm, it is compatible right?
```

---
## \#274 Posted by: rpasichnyk Posted at: 2018-07-18T14:43:53.051Z Reads: 268

```
Yes, it is compatible
```

---
## \#275 Posted by: squad Posted at: 2018-07-20T19:32:33.701Z Reads: 276

```
First of all, great work @rpasichnyk and @hexakopter! Module works amazing! 

I have a question about recorded telemetry data, is there a way to see and analyze records from both VESCs separately? I have a problem with hall sensors in one motor (connected do master VESC) and would like to compare it with the good one (connected to slave VESC) to which is also connected Metr.
```

---
## \#276 Posted by: webst Posted at: 2018-07-21T13:37:52.483Z Reads: 261

```
Also: is there any plan to store data in module and send it to the app afterwards?
```

---
## \#277 Posted by: Soul40ne Posted at: 2018-07-21T13:41:33.515Z Reads: 258

```
Can the vesc firmware be updated via Bluetooth
```

---
## \#278 Posted by: rpasichnyk Posted at: 2018-07-21T13:54:31.018Z Reads: 258

```
@squad Not yet. The dual data is only displayed, but not recorded. The recorded data is from the VESC which Metr Pro is connected to. I plan to implement it later in the app.
@webst there is a plan which involves SD card. There are additional pins routed on the back of the module for that. No ETA though. 
@Soul40ne yes it can. Latest VESC firmware v3.39 is available to update via metr app.
```

---
## \#279 Posted by: squad Posted at: 2018-07-21T16:08:23.645Z Reads: 257

```
Thanks for clarification, can’t wait for metr update which will implement recording data from both vescs 😉
```

---
## \#280 Posted by: nuttyjeff Posted at: 2018-07-21T16:17:24.546Z Reads: 248

```
Just ordered one. Cant wait! :d
```

---
## \#281 Posted by: mikenyc Posted at: 2018-07-21T16:22:05.386Z Reads: 272

```
@rpasichnyk my board stopped responding after trying to change modes. an error popped up about firmware being <= 2.18 or something, i didn't write it down before dismissing it.

i tried connecting to the focbox over tcp bridge, and then directly through USB. i'm seeing this error. any ideas?

![06%20PM|690x385](upload://tlTQNK4aBCzAR8MQNdwxm23TC1E.png)![03%20PM|598x500](upload://9jZ12ePoT570otOKVaorp5tyKKT.png)
```

---
## \#282 Posted by: Pedrodemio Posted at: 2018-07-21T17:34:57.920Z Reads: 268

```
When the SD get implemented I will surely get one, I tried to keep track of my mileage but it’s not always that I bring my phone

If all records get stored on board and you only need the phone to view them would be perfect
```

---
## \#283 Posted by: Silverline Posted at: 2018-07-21T23:21:03.438Z Reads: 269

```
Oh that would be fucking awesome 😀
I also forget to start my metr app sometimes , and with the old module i sometimes have connections issues .... With a sd card, you will never loose data :-) ETA. On this :slight_smile:


@rpasichnyk  I'm using this logger on my FPV racing quads, to record data from the flight. Could it be used together with the metr module in the future?https://m.ebay.com/itm/AB01-FPV-BLACKBOX-FLASH-DATA-RECORDER-CLEANFLIGHT-OPENLOG-QUADCOPTER-FPV/132631144430?hash=item1ee16ea7ee%3Ag%3A8PIAAOSwdvpWDzJR&_nkw=Blackbox+openlog&_from=R40&rt=nc&_trksid=m4084.l1313
```

---
## \#284 Posted by: Moros Posted at: 2018-07-21T23:55:09.916Z Reads: 267

```
[quote="Silverline, post:283, topic:57780"]
Btw. @rpasichnyk just ordered the basic module for 40 euro, but i got charged additional 10euro for VAT. ? I thought you where within EU ?
[/quote]

Yep, the site adds €10 VAT and €12 shipping even if its coming from a city an hour away in a flat pack bag.
so a €40 module ends up costing €62. Then if you want to add a €3  [antenna](https://www.aliexpress.com/item/-/32848962210.html?spm=a2g0s.13010208.99999999.299.53b63c009ZRAIc) its another €12 plus €3 VAT for a total of €77 

Shipping is far overpriced for Europe . I sent a 5kg box to sweden from Germany last week tracked for €15, so I don't see how a 20g module sent from an hour away in the next city over and cost almost the same price is justified ...
```

---
## \#285 Posted by: E1Allen Posted at: 2018-07-22T11:35:36.786Z Reads: 259

```
Would anyone use battery cutoff end in the modes section?  I've usually keep conservative cutoffs, however I've been out when the battery has gotten almost to "empty" but the pack has more of you just change the limit to get that extra but of distance.
```

---
## \#286 Posted by: webst Posted at: 2018-07-22T22:54:09.981Z Reads: 253

```
Just set it to your desired battery pack life.
```

---
## \#287 Posted by: E1Allen Posted at: 2018-07-22T23:38:19.071Z Reads: 253

```
I'm talking about changing it on the fly
```

---
## \#288 Posted by: Toleg Posted at: 2018-07-24T10:08:56.265Z Reads: 256

```
Hello, did you find a workaround ?
I've a similar problem: Dual condig with focbox, latest ackmaniac.
Works with metr app.
With esc monitor, i can find the module and connect to it, but no data...
```

---
## \#289 Posted by: squad Posted at: 2018-07-28T13:38:54.290Z Reads: 268

```
Hi @rpasichnyk and all! 


I have my antennas, DO YOU?
![IMG_5901|666x500](upload://cidjP4iEBfZwNX9DCvlaKubYeQX.jpg) 

Metr Pro works great, but I noticed my spent Wh are waaaay off, my battery pack is 12S10Ah LiPo and this equals to roughly 444Wh in the pack. Do You need some log files to look into it @rpasichnyk? 

https://metr.at/r/wNr0z

Have a nice day folks!
```

---
## \#290 Posted by: rpasichnyk Posted at: 2018-07-28T20:54:09.443Z Reads: 253

```
Sweet setup! It’s a known bug I guess. With VESC count being wrong. Will have a look!
```

---
## \#291 Posted by: squad Posted at: 2018-07-28T21:21:31.702Z Reads: 266

```
Thanks! 🙏 
Just finished second ride today, this time it looks like metr Wh count is right.

https://metr.at/r/Q9osS
```

---
## \#292 Posted by: mmaner Posted at: 2018-07-28T21:34:00.458Z Reads: 263

```
[quote="rpasichnyk, post:270, topic:57780"]
Hey @mmaner how did it go with your Metr Pro module? I think @LoR_NiKoN had a very similar issue and what helped in the end is “forgetting” the module from iOS Settings -&gt; Bluetooth and uninstalling and installing the app again from the App Store.
[/quote]

Please don't ask me why, because I don't have a clue.  After the update to the METR android app last week my module started working.  It might have something to do with the firmware of the FocBox's, Im running @Ackmaniac 2.54.  Either way, its working now.
```

---
## \#293 Posted by: Silverline Posted at: 2018-07-29T11:25:58.369Z Reads: 259

```
For people like me, comming from the R/C hobby, these antennas for the Frsky x4r receiver and others, fits perfect and cost like nothing, and dont take up much space, and is 2,4ghz as well
![IMG_20180729_131811|690x388](upload://cvhA7yaGJaKK7N2Sa5IauLsEh3s.jpg)
```

---
## \#294 Posted by: noamlin Posted at: 2018-08-03T15:08:51.517Z Reads: 251

```
I wanted to say I have just bought 3 modules and it is looking very good!
it is the first module that can connect to my Android 8.0!!
I am very satisfied!
the other, cheap, modules do not stand with the security requirements by bluetooth protocol and thus ignored by android 8
```

---
## \#295 Posted by: Silverline Posted at: 2018-08-12T15:02:08.454Z Reads: 256

```
Sorry if this has been asked before. 

But I'm a first time Can-bus user. My ppm receiver is connected to the master (vesc 0) .... Do i also need to connect this module to the master, or is slave okay ?

And is it plug and Play with the escape vesc's ?
 Thanks

Update. Damn... I need a 8p connector :frowning:![IMG_20180812_171513|281x500](upload://jL6TFovUhaKX2jSVqNYsb1aYvrk.jpg)
```

---
## \#296 Posted by: mikenyc Posted at: 2018-08-12T15:18:21.774Z Reads: 246

```
Mine is connected to the master, not the slave
```

---
## \#297 Posted by: Silverline Posted at: 2018-08-12T15:31:41.259Z Reads: 250

```
Okay thanks, i Will do that
```

---
## \#298 Posted by: rpasichnyk Posted at: 2018-08-12T16:56:16.847Z Reads: 253

```
@Silverline you can connect either to master or slave, it doesn't matter. We only supply 7p connector as it works just as well in 8p slot, you shouldn't have any issues with that. Please check the pin order on your ESCape, if I recall correctly they are in reverse order. Not just RX and TX, all pins are in reverse order. Would be great if you confirm that and let us know ;)
```

---
## \#299 Posted by: Silverline Posted at: 2018-08-12T17:32:19.335Z Reads: 254

```
@rpasichnyk thanks for replying back 😀 cool i can use both slave or master. 

This is from the escape 
![IMG_20180812_193035|281x500](upload://iYLOCmsLaO1GuNul6RZPUXKfpxZ.jpg)
```

---
## \#300 Posted by: rpasichnyk Posted at: 2018-08-12T17:41:24.086Z Reads: 245

```
Oh yes it is reversed. You need to pop out all the pins on one side of the cable carefully, flip the plastic part, and insert back in. This thing in ESCape makes me so sad :( Please fix it @stewii, please, please
```

---
## \#301 Posted by: AndyBigD Posted at: 2018-08-12T19:54:51.193Z Reads: 242

```
Nice fuse you got there :wink:
And yeah the pins are completely reversed on the ESCapes. Swapped them all round on mine for the 1st install and everything works fine :+1:
```

---
## \#302 Posted by: AndyBigD Posted at: 2018-08-12T19:56:53.658Z Reads: 246

```
You do have to twist each wire round 180 degrees before putting them back in the connector so the little tang is on the right side. Bit tricky as it's a ribbon cable, easier if you separate the wires back a cm or two.
```

---
## \#303 Posted by: Ubbiedude Posted at: 2018-08-12T20:01:27.759Z Reads: 244

```
Hey guys, could it be that my nano x is causing interference with my metr module? Every time use the throttle it disconnects with my phone
```

---
## \#304 Posted by: Silverline Posted at: 2018-08-12T20:36:56.926Z Reads: 255

```
So the "ADC 3" on the escape is not in use ?

Metr. -> escape
5 v.   ->   5v
3,3v. -> vcc
Gnd.  -> gnd 
Swc. -> adc1
Tx/rx -> rx
Tx/rx. -> tx
Swd -> adc2

Is that right ?

@AndyBigD thanks, it's a nice compact fuse 😀
```

---
## \#305 Posted by: SkaterBoy58 Posted at: 2018-08-12T23:20:48.382Z Reads: 252

```
Roman - Will you updating your vesc tool to run with vesc FW 3.40  or do I need to downgrade  to FW  3.39 to work with metr-pro BTE ?  Thanks
```

---
## \#306 Posted by: riverside.rider Posted at: 2018-08-13T03:27:10.423Z Reads: 243

```
I can confirm that for the ESCape , all connections are in reverse order. I made an adapter and it works very well.
```

---
## \#307 Posted by: Pimousse Posted at: 2018-08-13T06:23:48.448Z Reads: 248

```
Yes, ADC3 is the 8th pin added on HW6 VESCs (official and alternatives).
Let it free.
If you don't want to bother you swapping all the Metr Pro wires, just leave free (but isolated by heatshrink for example) Swd, Swc, and 5V.
I did it on mine to be able to connect Metr Pro on Escape. This 180° twist on pins didn't make so confident in matter of reliability.
```

---
## \#308 Posted by: Silverline Posted at: 2018-08-13T06:32:24.181Z Reads: 253

```
It's an easy task to switch the pins around. It was just to making sure that i was doing it in the right order, hence the writing on the escape dosn't match metr

Like "swc" to adc1
```

---
## \#309 Posted by: willumpie82 Posted at: 2018-08-13T07:10:54.329Z Reads: 253

```
@rpasichnyk can you update us how the is DieBieMS integration is going? 

I can connect to it via the terminal but can only issue a single command and receive a response, after that the input seems ignored.
(dual 4.12 vesc, CAN cable T-splitted to the BMS CAN port, everyting latest (public) version
```

---
## \#310 Posted by: Trdolan03 Posted at: 2018-08-13T07:56:59.827Z Reads: 249

```
I’m sure I had been answered at some point but I don’t have time to read the full thread. If you are running a dual setup via canbus do you need 2 modules to be able to change setting on master and slave Vesc?
```

---
## \#311 Posted by: Pimousse Posted at: 2018-08-13T08:17:55.400Z Reads: 245

```
No, one is enough.
```

---
## \#312 Posted by: isabar Posted at: 2018-08-14T11:52:18.748Z Reads: 258

```
I got 2 modules.  They initially connect, but if I close the app and reopen it, it doesn’t find the module again. Same thing if I power off the vesc and turn it back on.

The only way to get it to work again is to unpair the module and then repair each time, but this is obviously not supposed to work that way.

I am using a Galaxy S6 Android 7, but also saw this issue on other phones I tested. I tried both modules .. same issue.

Vesc firmware: 3.101 (ackmaniac)

Any ideas?
```

---
## \#313 Posted by: Silverline Posted at: 2018-08-14T16:39:34.760Z Reads: 244

```
I have a hard time connecting to vesc-tool from my computer via BLE..... Do my phone need to be connected to the meter module as well, or is the connection made directly between my computer and metr module ?
```

---
## \#314 Posted by: hexakopter Posted at: 2018-08-14T22:17:30.637Z Reads: 256

```
@isabar I respond to your mail you wrote to support@metr.at with the same question. Please send us the log files.

@Silverline No, your phone must be disconnected from your Metr Pro module when you want to connect to VESC Tool over bluetooth. What VESC Tool are you using? As it is stated here
https://www.electric-skateboard.builders/t/metr-pro-next-gen-bluetooth-module/57780/94
you need [this](https://github.com/rpasichnyk/vesc_tool/releases) VESC Tool with some BLE related code changes to get it working.
```

---
## \#315 Posted by: Silverline Posted at: 2018-08-15T10:14:36.916Z Reads: 243

```
Thanks..... i give it at try. I thought that the newest vesc-tool from Vedder, was supporting BLE connection, the "BLE tab" is there, and all that...... Since @rpasichnyk was mentioned that Vedder was implementing BLE function ?

UPDATE. It is working with the version from github :-). What is funny though, is that i was using the regular vesc-tool 0.95..... But with the 0.95 version from Github, vesc-tool tels me that my fw is newer than the tool ?
```

---
## \#316 Posted by: topcloud Posted at: 2018-08-15T13:15:19.611Z Reads: 239

```
ordered, stoked :)  thank you
```

---
## \#317 Posted by: Silverline Posted at: 2018-08-16T19:42:51.342Z Reads: 254

```
What does this mean ? I had some wird behaviour on the ride. Is that what it mean ?


https://metr.at/r/JVyeu

![1534448300982|292x500](upload://o87xMioZH9Ym1v1I3xHAjk2WCkM.jpg)
```

---
## \#318 Posted by: oyta Posted at: 2018-08-16T20:13:54.281Z Reads: 244

```
![image|441x500](upload://1l9eDWkIFbT4pBcr3lnnxULHpGJ.jpeg)

You have at least an over current fault. Looks like you got it while breaking. What are your current settings on the VESC?
```

---
## \#319 Posted by: Silverline Posted at: 2018-08-16T20:19:16.826Z Reads: 232

```
How did you find that in the log ?(update, ohhh the red line cool)

 Both my motor minimum and battery minimum (regen) are -30a ... So not wery high, im using dual escapes.... And no bms (12s lipo) The throttle stop working for a second... But i was not braking....
```

---
## \#320 Posted by: oyta Posted at: 2018-08-16T20:23:21.929Z Reads: 238

```
![image|281x500](upload://fXdIq6CcOgvrG0UlRyh8cqIE1e2.jpeg)

It is marked by a red vertical line in the log. You can see it just to the right of 18:40.
```

---
## \#321 Posted by: Silverline Posted at: 2018-08-16T20:23:45.725Z Reads: 226

```
Yes just saw that. Awesome thanks

But i dont understand why a get this failure. I was not not going fast at All, i was not braking hard at All. It just come random, from time to time.
```

---
## \#322 Posted by: hexakopter Posted at: 2018-08-16T22:23:50.009Z Reads: 244

```
[quote="Silverline, post:315, topic:57780"]
I thought that the newest vesc-tool from Vedder, was supporting BLE connection, the “BLE tab” is there, and all that… Since @rpasichnyk was mentioned that Vedder was implementing BLE function ?
[/quote]
Benjamins version just supports BLE for Linux systems. To get Windows and Mac support you need the linked version with slightly code changes.

[quote="Silverline, post:315, topic:57780"]
UPDATE. It is working with the version from github :-). What is funny though, is that i was using the regular vesc-tool 0.95… But with the 0.95 version from Github, vesc-tool tels me that my fw is newer than the tool ?
[/quote]
Great to hear that it is now working for you. Benjamins VESC Tool got updated to version 0.95 which added FW3.39 support. That 0.95 is what Romans version is based on. After that Benjamin updated version 0.95 to also get FW3.40 support but doesn't changed the new version to 0.96 but is still using 0.95 as version number.

[quote="Silverline, post:321, topic:57780"]
But i dont understand why a get this failure. I was not not going fast at All, i was not braking hard at All. It just come random, from time to time.
[/quote]
What VESC version are you using? I got some random overcurrents with HW4.12 in the past. Please note that this fault has nothing to do with your Metr Pro module and is just based on your VESC. Metr Pro just visualize the over current error inside your record/graph as @oyta said.
```

---
## \#323 Posted by: Silverline Posted at: 2018-08-16T22:28:18.422Z Reads: 235

```
Thanks man, for clearing this up. Then i must "downgrade my fw then :-) Or will the github version soon support 3.40fw ?? @rpasichnyk 

I know it has nothing to do with my metr pro module.... I just wants to find out whats wrong, and maybe metr pro module can help me with that :slight_smile:

I´m on the original 3.40fw with my escapes (vesc 6 ) at the moment...
```

---
## \#324 Posted by: sayekim Posted at: 2018-08-16T22:37:00.912Z Reads: 241

```
Well fuck me I’m colorblind. @rpasichnyk Can you make this line blue? Or have some option for us colorblind folks?   

To me the line looks the same as above 18:40 as after. Well actually the one after is slightly darker I suppose.
```

---
## \#325 Posted by: oyta Posted at: 2018-08-17T06:54:24.942Z Reads: 255

```
[quote="Silverline, post:319, topic:57780"]
Both my motor minimum and battery minimum (regen) are -30a …
[/quote]

With battery min (regen) of -30A I guess you are using LiPo? It seems too low for LiIon.

You can lower the motor min to at least -60 per VESC to get more power on the breaking with low duty cycle.

And what is your absolute current Max?
```

---
## \#326 Posted by: E1Allen Posted at: 2018-08-17T07:16:45.754Z Reads: 251

```
I've gotten it before. I was hard braking and I think one when just locked up. So maybe the difference between one motor turning and one stopped caused it
```

---
## \#327 Posted by: Silverline Posted at: 2018-08-17T07:23:49.105Z Reads: 250

```
Yeah... So with -30a i should'nt get any "over current" fail ? As you can se, i wasnt even braking a lot, only slightly. Or do my braking force need to be higher, to not get this failure. 
Yes i'm using 12s graphene lipo. 

Absolutely max, is default for vesc 6, so i guess 130a if i remember correctly.

@E1Allen but i was barely braking :-/
But what i can se is that the voltage was 50,4v, wich is a full charged 12s lipo. Could i Cold solder join, on the two big capacitors , give some sort of voltage spike ? And trigger over-current failure ?
```

---
## \#328 Posted by: gmurad Posted at: 2018-08-22T23:48:39.521Z Reads: 251

```
When using android wear can the module connect directly to the watch (not needing a phone at all)? Or does the phone connect to the module and the watch connect to the phone?

A bit off topic but what are the best android wear watches to use with Metr Pro for eskating?
```

---
## \#329 Posted by: epster Posted at: 2018-08-24T15:14:25.142Z Reads: 243

```
Couldn`t figure out on your site what the shipping time is could you give me an estimation of that?
Oh yeah another question what is the biggest diffirence between the metr and the metr pro becuase i don`t really see a diffirence except from the antenna. I ask this because i think eskating.eu ships the older ones please correct me if i am wrong.

greetings from a future customer :smile:
```

---
## \#330 Posted by: plasteroid Posted at: 2018-08-26T19:14:51.571Z Reads: 250

```
Trying to setup my new Metr Pro.

I've got it installed on the VESC, and blue and green lights, but can't seem to get it to show in the connection port options as desired - like in the screenshot below.  Only my iPhone is showing up in the list. 

What am I doing wrong? Running 094

https://www.electric-skateboard.builders/uploads/db1493/optimized/3X/8/b/8b04b9b978b7b0a258cb8030cf13eda360416f15_1_690x362.png
```

---
## \#331 Posted by: hexakopter Posted at: 2018-08-28T15:09:07.303Z Reads: 262

```
Sorry for the late response. Wasn't at home the last days, so all open orders will be send tomorrow.

@gmurad I don't have a Android wear device, so I can just answer my presumption. When I understand it right Android wear is just a "light" Android system where Apps are installed over the phone and enable a connection through your phone. So my assumption is that Android wear devices connect to your phone and your phone to your Metr Pro module. But it looks like there are also watches out there running a "full" Android like the one @Klattrup is using where you can directly connect to the Metr Pro module like you can see in his post https://www.electric-skateboard.builders/t/configuration-and-telemetry-for-vesc-ios-android/13483/913 Maybe someone using a Android smartwatch can tell you more.

@epster On average we ship orders within 3 days. [s]We are running out of small antennas right now, so maybe there could be a delay when ordering a module with small antenna the next days.[/s] To get an idea about delivery time of the currier have a look [here](https://www.deutschepost.de/content/dam/dpag/images/B_b/Briefe_ins_Ausland/downloads/dp_laender-und-laufzeiten-2017.pdf). 
To get an idea about the differences I would recommend to read the first post of this thread. All things like BLE encryption, support for all known apps including VESC Tool on desktop systems, baud rate and TX/RX detection, firmware updates over the air for both the Metr Pro module and the VESC, faster update rate etc. are only available for Metr Pro. The standard Metr bluetooth module just behave like a serial bridge, while the Metr Pro is running its own firmware and enables a lot more opportunities. And you are right that eskating currently just sells "old/standard" Metr modules.

@plasteroid I think you are not running the adapted version of VESC tool that has some small BLE changes. You can read more in that post: https://www.electric-skateboard.builders/t/metr-pro-next-gen-bluetooth-module/57780/94

Edit.: Small antennas are out of stock now.
```

---
## \#332 Posted by: DAddYE Posted at: 2018-08-30T23:28:46.243Z Reads: 245

```
I bought it awhile back do you have the scheme to connect to a flipsky VESC 6?
```

---
## \#333 Posted by: somaht21 Posted at: 2018-09-01T01:20:02.045Z Reads: 252

```
I've just received my metr Pro module, works like a charm, the app is really cool and uploading the datas is really easy. Thanks !

I have some questions though:
https://metr.at/r/jP7nx

- As you can see on the data, I don't have the motor temperature. Does it work only with sensored motors ?

- The RPM is not correct. I'm running a 100Kv Outrunner at 12S, meaning the motor can't spin faster than 5000 RPM. Yet, the maximum recorded is 20 000RPM. 
Does anybody knows how to set the app so that I get the right RPM ?
```

---
## \#334 Posted by: Trdolan03 Posted at: 2018-09-01T02:29:14.930Z Reads: 241

```
[quote="somaht21, post:333, topic:57780"]
As you can see on the data, I don’t have the motor temperature. Does it work only with sensored motors ?
[/quote]
Yes, there is a temp wire in the sensor wire
[quote="somaht21, post:333, topic:57780"]
The RPM is not correct. I’m running a 100Kv Outrunner at 12S, meaning the motor can’t spin faster than 5000 RPM. Yet, the maximum recorded is 20 000RPM.
Does anybody knows how to set the app so that I get the right RPM ?
[/quote]
The rpm you are referencing is the ERPM which is the more commonly referred in terms of the Vesc. Is you divide the erpm by the motor pole pair (normally 7) you should get the proper rpm.
```

---
## \#335 Posted by: somaht21 Posted at: 2018-09-01T10:50:52.727Z Reads: 235

```
Thanks !
So with a sensorless motor no temperature, too bad !

How can I know for sure that my motor has 14 poles ( or 7 pairs) ?
```

---
## \#336 Posted by: SkaterBoy58 Posted at: 2018-09-05T01:45:09.004Z Reads: 228

```
Count them !
by turning motor slowly by hand and feeling magnet pole effect
```

---
## \#337 Posted by: goldrabe Posted at: 2018-09-05T11:50:10.989Z Reads: 224

```
Sorry guys, I know this question was asked before, but do i have to simply reverse the pin out with ESCapes?
I could not find the answer immediately.  :stuck_out_tongue_winking_eye:
```

---
## \#338 Posted by: Pimousse Posted at: 2018-09-05T11:58:17.339Z Reads: 230

```
Yes.
10char
```

---
## \#339 Posted by: goldrabe Posted at: 2018-09-05T12:11:15.857Z Reads: 225

```
Thanks mate!
```

---
## \#340 Posted by: alivedom Posted at: 2018-09-05T16:36:45.554Z Reads: 221

```
So i was happy to get the metr pro and immidiatly got disappointed as it uses both ADC. So what do i do now? I wanted to use it for my Ebike project and I have regen braking on ADC2 and Throttle on ADC1... I know i should have checked this before but why does it even need those two ADC? I know i could bypass with a arduino nano to PPM but honestly... this seems way overcomplexed. That moment when you dont check every detail...
```

---
## \#341 Posted by: rpasichnyk Posted at: 2018-09-05T17:10:36.979Z Reads: 226

```
No, it doesn't use ADC. It only uses TX, RX, 3.3V and GND.  You can safely use ADC for your own needs. We supply Metr Pro together with 7pin cable just because it's easier for us. Think how much time it would take to remove those 3 wires from the each cable over and over again ;)
```

---
## \#342 Posted by: alivedom Posted at: 2018-09-05T18:27:35.313Z Reads: 230

```
Ahh thanks so much for the answer. I thought i saw some routing from those two leading to the chip. Thats why i was worried... Thanks again
```

---
## \#343 Posted by: Saturn_Corp Posted at: 2018-09-07T16:07:07.892Z Reads: 227

```
Just ordered a module. Gonna have fun with this.
```

---
## \#344 Posted by: janpom Posted at: 2018-09-10T07:46:27.168Z Reads: 222

```
I'm trying to decide on PCB vs external antenna. Could anyone with the PCB antenna please share their experience with it? What's the range? Any problems with it? Thanks!

@rpasichnyk @hexakopter Do I understand correctly that if I go with the PCB antenna I can still add the external antenna later but I need to resolder one resistor? Could you please provide some guidelines for dummies on that? Also, is it possible to order the external antenna module (i.e. with the resistor at the right place) but without the antenna in case I wanted to add my own antenna? Thanks.
```

---
## \#345 Posted by: visnu777 Posted at: 2018-09-10T09:24:56.595Z Reads: 212

```
After I managed to let the external antenna make contact with the plus pole of my battery I got the PCB only Version which works for me as well despite my CF integrated enclosure. I works perfectly AS long AS you are in the same room.
```

---
## \#346 Posted by: Pimousse Posted at: 2018-09-10T09:35:10.152Z Reads: 215

```
Routing on the module for those pins is needed because they (I guess @hexakopter ) use them for programming the nRF51 chip (refer to the silkscreen marks).
But once connected to the VESC, it's not use anymore. ;)

Still, it's smart from them to design it the most "plug-and-play" way.
The counter side is that for some uses (like ADC), it's a bit less convenient.

@rpasichnyk : this point should be explained in your FAQ/guide, shouldn't it ?
```

---
## \#347 Posted by: hexakopter Posted at: 2018-09-10T18:48:56.280Z Reads: 221

```
@janpom
[quote="hexakopter, post:252, topic:57780"]
I did not noticed any performance difference to the bigger antenna. When you compare antenna gain it is 2.5 dBi for the bigger antenna and 2.0 dBi for the smaller one. So in theory when mounted the antenna correctly you should get a slightly higher range because of the narrower and longer main lobe. But thats just theory and in reality you most likely will not notice. :slight_smile: The main advantage of the external antennas to be able mounting them outside your carbon enclosure or anything else dampening the electromagnetic field massively applys to both antennas.
[/quote]
I hope that helps you a bit to decide. Speaking for myself I am happy with the PCB antenna without any dropouts, but I am not using a carbon enclosure and the phone is near to the module all the time.

Yes you can add the external antenna later with resoldering a very tiny cap to a different place. When you don't have good solder experience I wouldn't recommend doing that yourself. Yes it is possible to get the module without any antenna. Do you need the u.FL to IPEX connector already connected or without antenna and without connector? Please send a request to support@metr.at about what you need especially.

@Pimousse We will update our FAQ/guide over time. Thanks for your suggestion. We will add that later.
```

---
## \#349 Posted by: Snake Posted at: 2018-09-17T14:12:28.446Z Reads: 202

```
Hi guys, 
i want to use the metr-App with two FOCBOXES. Are there any issues known?
Do i have to use two BT-modules or is it possible to send the Telemetrie datas over the Canbus
At the Moment i have two Receivers in use for the throttle-signal (for redundancy)
So i would use the Canbus only for Telemetrie-data, not for throttle-signal...does it work this way?
```

---
## \#350 Posted by: Pimousse Posted at: 2018-09-17T14:18:36.694Z Reads: 210

```
See few posts above.

[quote="Trdolan03, post:310, topic:57780, full:true"]
I’m sure I had been answered at some point but I don’t have time to read the full thread. If you are running a dual setup via canbus do you need 2 modules to be able to change setting on master and slave Vesc?
[/quote]

[quote="Pimousse, post:311, topic:57780, full:true"]
No, one is enough.
[/quote]
```

---
## \#351 Posted by: Snake Posted at: 2018-09-17T14:22:55.673Z Reads: 200

```
Thanks...but does it also work if i have the throttle-signal from an Receiver for every Focbox and only the telemetrie-data over the canbus?
```

---
## \#352 Posted by: Jc06505n Posted at: 2018-09-17T14:27:53.106Z Reads: 197

```
you mean if you're running split ppm AND canbus?
```

---
## \#353 Posted by: Snake Posted at: 2018-09-17T14:32:51.448Z Reads: 193

```
Yes, i have two receivers...one per each Focbox.
```

---
## \#354 Posted by: Pimousse Posted at: 2018-09-17T14:41:24.294Z Reads: 199

```
As long as CAN is enabled, you can retrieve telemetry data through it, whatever the used app (PPM, ADC...).
For mode switching, not sure.
```

---
## \#355 Posted by: mmaner Posted at: 2018-09-17T14:42:23.549Z Reads: 193

```
you only need 1 METR Pro module even if using can or split PPM.  With CAN the values are automatically doubled, with split PPM you have to set the doubling in the config.
```

---
## \#356 Posted by: Snake Posted at: 2018-09-17T14:48:59.767Z Reads: 194

```
Thank you :wink:
Does anyone know if mode switching does work properly with my configuration?

And do i need a special FW on the Focboxes to use the metr/perimetr-apps?
```

---
## \#357 Posted by: Pedrodemio Posted at: 2018-09-17T14:50:54.148Z Reads: 198

```
It works, if the metr app detects two VESC's it will write the config to booth of them when switching modes
```

---
## \#358 Posted by: mmaner Posted at: 2018-09-17T14:52:33.483Z Reads: 197

```
Modes work with @Ackmaniac's firmware, I don't know about stock firmware.  Yes, it will work with stock FocBox's.
```

---
## \#359 Posted by: Riako Posted at: 2018-09-17T19:08:00.394Z Reads: 210

```
Hello guys,

I need help and advice or tips or everything that can help me to fully record my rides! Plzzz

I can not record a single complete ride with metr.pro, what are your parameters side phone those who have an Android?
I removed the battery saver, I activity the non-pumping battery restriction of the apps, I increased the standby time of my phone ...
The apps shut up like that from one moment to the next.
Clearly, when I ride I look very often my phone to just avoid it removes my ride and yet, just like that, when I re-open my phone the app is no longer open!! Grrr, I have to re-click on it! And so it re-opens like the ride had never existed.
Why does not she save at least everything that was first covered?
And then it should automatically resume the record since I activated the autostart record mode?
So that's because the apps close itself, but why?
Has anyone ever met with the problem?

I have the automatic update ...
But I have trouble since the metr module BT 1st generation.
FW 3.40 (FSESC4.20) but I had the problem with my VESC6 too.

So I guess it my phone or the apps the issue, not the module disconnection?
Or is that what would cause the spontaneous break of the apps?

Thanks for your help :pray:
```

---
## \#360 Posted by: mmaner Posted at: 2018-09-17T19:18:29.093Z Reads: 190

```
Its most likely your phone.  I had to uninstall, reboot and reinstall a couple of times to get it to behave correctly on my Pixel.  On my Nexus 5 it runs perfectly.  This is using the same module between the 2 phones.
```

---
## \#361 Posted by: oyta Posted at: 2018-09-17T19:58:43.819Z Reads: 190

```
It works with the original VESC FW.
```

---
## \#362 Posted by: DAddYE Posted at: 2018-09-17T20:02:28.920Z Reads: 193

```
How we embed metr links with preview here in the forum?
```

---
## \#363 Posted by: Pimousse Posted at: 2018-09-17T20:10:12.231Z Reads: 191

```
Look at the thread dedicated to the app : https://www.electric-skateboard.builders/t/configuration-and-telemetry-for-vesc-ios-android/13483?u=pimousse
This one is for Metr Pro module.
```

---
## \#364 Posted by: mmaner Posted at: 2018-09-17T21:07:13.492Z Reads: 192

```
when you upload a record from your phone, at least it does on mine, it automatically opens that web page in chrome.  I just copy & paste the address.
```

---
## \#365 Posted by: DAddYE Posted at: 2018-09-17T21:12:09.405Z Reads: 193

```
Doesn't work with me: https://metr.at/r/xI7ah
```

---
## \#366 Posted by: mmaner Posted at: 2018-09-17T21:18:22.235Z Reads: 207

```
[quote="DAddYE, post:365, topic:57780, full:true"]
Doesn’t work with me: https://metr.at/r/xI7ah
[/quote]

It worked for me...
![image|416x500](upload://76OnOrcll2gnXVJas2lFs7cHF2.png)
```

---
## \#367 Posted by: DAddYE Posted at: 2018-09-17T21:19:27.099Z Reads: 185

```
The forum here sometimes embeds the preview in a box called onebox. Some metr.at links don't get the preview. Some do :(
```

---
## \#368 Posted by: mmaner Posted at: 2018-09-17T21:22:44.043Z Reads: 199

```
[quote="mmaner, post:366, topic:57780"]
https://metr.at/r/xI7ah
[/quote]

thats odd, I dont know the fix for that.  i cut & pasted your link below, it seems to be working for me.

https://metr.at/r/xI7ah
```

---
## \#369 Posted by: DAddYE Posted at: 2018-09-17T21:44:14.505Z Reads: 192

```
Oh lol, you added `?oembed=true` that's it!
```

---
## \#370 Posted by: mmaner Posted at: 2018-09-17T21:44:52.299Z Reads: 191

```
I dont know brother, just pasted your link and it worked.  it may have auto added the embed tag?
```

---
## \#371 Posted by: DAddYE Posted at: 2018-09-18T01:31:55.565Z Reads: 186

```
He must like you better than me :cry:
```

---
## \#372 Posted by: Jc06505n Posted at: 2018-09-18T03:14:36.512Z Reads: 195

```
The forum won’t open a link unless it’s on its own line 

https://metr.at/r/xI7ah
```

---
## \#373 Posted by: hexakopter Posted at: 2018-09-18T16:58:40.112Z Reads: 198

```
@all Just want to let you know that all Metr Pro antenna options are back in stock.

@Riako I would guess its some problem with your phone. Do you have the chance to use a different phone from friend/family and give it a test? It would also be helpful when you send a log to support@metr.at so we can have a look if we spot something wrong. Maybe also reinstalling the app like @mmaner suggested could help fixing your problem.

@DAddYE I think it will just be displayed the way you like it when you post the link directly and not use the hyperlink function. And as @Jc06505n said on its own line. 

Direct link:
https://metr.at/r/xI7ah

Hyperlink:
[https://metr.at/r/xI7ah](https://metr.at/r/xI7ah)
```

---
## \#374 Posted by: longhairedboy Posted at: 2018-09-22T15:27:14.734Z Reads: 193

```
so 've been dicking around with my new metr pro module all morning... I bought two, one for my ride and one for testing and reviewing shit that moves around between Betty and Jake's board. 

i think i have everything figured out. 

so which app gives me the video overlays with speedometer dashboards and shit? i keep seeing that in various places. Can the metr pro feed those kinds of video apps with data as well?
```

---
## \#375 Posted by: Silverline Posted at: 2018-09-22T15:47:14.359Z Reads: 193

```
Look at the metr site : https://metr.at/overlay
```

---
## \#376 Posted by: E1Allen Posted at: 2018-09-22T19:11:22.937Z Reads: 196

```
Did anyone get the apple watch 4 working for this?  I turn random on and followed the steps. Doesn't appear to be working

It works, missed a spot in the settings page
```

---
## \#377 Posted by: Trdolan03 Posted at: 2018-09-23T17:07:33.696Z Reads: 205

```
So I have a question about ride data. I have 2 vescs of can. Both double data and dual data were on. Is the energy consumption shown for both VESC or just one? 

Edit: also, how can I tell what the fault was? There is a little red 1 on the trip data. ![image|281x499](upload://tAXvuujSlp3fNmPQ0etFdOnqGIT.jpeg) 
https://metr.at/r/DeHsN
![image|293x500](upload://i5Yav4ekqAtSSqSq3kJDjvwuEEY.jpeg)
```

---
## \#378 Posted by: taz Posted at: 2018-09-23T17:24:01.230Z Reads: 185

```
Normally there should be a pink strip on the diagram for the duration of the fault.
I can't see anything on your diagram but I do see a point around 23:30 where the voltage dropped to 9.0V so this would be registered as an under voltage fault.
```

---
## \#379 Posted by: Riako Posted at: 2018-09-23T18:52:13.006Z Reads: 183

```
Which phone will be the best value for money to use with Metro.at ?? ANd surely work weel and perfectly good :blush: (to buy used)
Yes, I am at this point :sweat_smile: ... I can't use them cause my phone still closes the apps for no reason, and don't find my old iPhone5 ... (I got metr 1st gen, Metr.Pro WOA and WMA ... so now just want to could reccord ride and make some cool overlay with it !)
Thx :v:
```

---
## \#380 Posted by: rpasichnyk Posted at: 2018-09-23T18:53:55.252Z Reads: 183

```
What phone do you have now?
```

---
## \#381 Posted by: Surfer Posted at: 2018-09-23T19:21:00.440Z Reads: 195

```
Maybe worth a shoot to try, when you go to the multitask screen, usually left bottom of the navbar, there is a lock on the top right part of the screen, this will lock your app to not be closed.

![Screenshot_20180923-211921__01|250x500](upload://dx6bCByhCCiMtwtSp55tltl2VOm.jpeg)
```

---
## \#382 Posted by: Surfer Posted at: 2018-09-23T19:37:44.381Z Reads: 190

```
Hi, long time didn't check this thread because my metr is working awesome.
BUT!!! I just deleted the data of the app and now I can't find the module in Oreo anymore, has been fixed some how the discovery problem in Oreo? I don't want to downgrade to Android 7 and delete everything again.
Edit: no metr pro module yet :)
```

---
## \#383 Posted by: Trdolan03 Posted at: 2018-09-23T19:53:55.682Z Reads: 187

```
[quote="taz, post:378, topic:57780"]
23:30 where the voltage dropped to 9.0V
[/quote]

I had looked for a voltage drop and totally missed this one. That would explain it. Thanks. Any idea about data double/multiply?
```

---
## \#384 Posted by: taz Posted at: 2018-09-23T20:14:35.196Z Reads: 189

```
The energy consumption should be for both VESC.
```

---
## \#385 Posted by: Riako Posted at: 2018-09-23T20:25:26.122Z Reads: 190

```
Hey Roman, thx for your help, I'm using a OnePlus 3 (android).
I will try that thanks for the tips @Surfer !!! ;)
```

---
## \#386 Posted by: Trdolan03 Posted at: 2018-09-23T22:50:00.419Z Reads: 191

```
Does 17-19wh per mile not seem low for an eMTB with helical direct drive?
```

---
## \#387 Posted by: Riako Posted at: 2018-09-23T22:56:51.366Z Reads: 188

```
If you don't uphill a mountain and ride around 25/35kmh mostly on trail, it's seems good, it's almost what I got (22Wh/km).
```

---
## \#388 Posted by: rpasichnyk Posted at: 2018-09-24T06:54:10.324Z Reads: 186

```
There should be no issues on Android, I think this one is specific to your phone. I have another person here in Stockholm who has OnePlus and experiencing same problem. We will hook up his phone to my laptop on Saturday and see what's going on :+1:
```

---
## \#389 Posted by: Riako Posted at: 2018-09-24T10:42:19.741Z Reads: 194

```
Yes, like I report after testing all what I can, and many people feedback too, its clearly a phone issue... thanks for confirming that! ;)

It a bit annoying to have to buy a new phone to could make all work .... but what we didn't do for passion !?.. :smile: 

So, it's why Im asking for some advice about phones that will work for sure and perfectly with your module.
I got 3 Metr.at and Metr.Pro module, and would like to could use them on my esk8, eMTB and eDirt, I know it a phone problem... and would resolve that :blush: 
I will try the Surfer tips and friends got an old Samsung to give it a try ... hop this old boy will handle it !

_edit: Frenglish orthography and gentle emoji :v:_
```

---
## \#390 Posted by: longhairedboy Posted at: 2018-09-24T13:33:38.366Z Reads: 184

```
Perfect! Thanks for the link.
```

---
## \#391 Posted by: Trdolan03 Posted at: 2018-09-25T00:57:22.993Z Reads: 190

```
![image|281x499](upload://46es87mmJd5nAQncCr5zWpdlDI1.png) So I turned on developer mode and the Vesc count is 1. I have a second VESC connected over canbus. Any ideas if this is right or not? I have tried 2 canbus cables and when I limit amps/speed it applies to both but I am more concerned about wh logging
```

---
## \#392 Posted by: mmaner Posted at: 2018-09-25T02:11:11.225Z Reads: 181

```
Go to settings > miscellaneous and click the Multiply Data slider and you will get the correct values. 

![Screenshot_20180924-210948|293x500](upload://gIeuVENOiDDTGXqt8fUSehR1pP3.jpeg)
```

---
## \#393 Posted by: Saturn_Corp Posted at: 2018-09-25T02:17:05.654Z Reads: 163

```
Got my Metr Pro today! Exited to check it out this week.
```

---
## \#394 Posted by: Trdolan03 Posted at: 2018-09-25T02:39:25.401Z Reads: 176

```
I’ve had that all along. ![image|281x499](upload://zvsLllMeikw8QbCGY1I9L5g2V8l.jpeg)
```

---
## \#395 Posted by: mmaner Posted at: 2018-09-25T03:12:51.845Z Reads: 171

```
Then what's your question?
```

---
## \#396 Posted by: Trdolan03 Posted at: 2018-09-25T03:24:53.232Z Reads: 179

```
Something isn’t lining up then. I lost 20% on a 4.5 mil mostly flat route with a 12s 8p 25r battery but metr is showing that I should have lost less than 10%🤔. I’ll start my own thread not to clog this one up.
```

---
## \#397 Posted by: FourteeOZ Posted at: 2018-09-25T03:27:58.555Z Reads: 181

```
@rpasichnyk is this compatible with the flipsky dual 6.6?
```

---
## \#398 Posted by: taz Posted at: 2018-09-25T04:10:41.287Z Reads: 180

```
Uncheck CAN fwd and check dual data.
```

---
## \#399 Posted by: Saturn_Corp Posted at: 2018-09-25T04:17:18.374Z Reads: 182

```
My module connects to my phone fine but I"m not getting any data and along with the solid blue light,. the green one is flashing like there's no tomorrow. Do I need to do something with the bldc tool?

VESC firmware 2.18 
Android 8.0.0
```

---
## \#400 Posted by: Trdolan03 Posted at: 2018-09-25T04:26:17.348Z Reads: 187

```
It still shows VESC count as 1. Has anyone else had this issue before? It is still only showing half of the WH consumed
```

---
## \#401 Posted by: Saturn_Corp Posted at: 2018-09-25T04:41:36.801Z Reads: 180

```
It's also showing 1 vesc for me over CAN. Dual data is on, CAN fwd is off.
```

---
## \#402 Posted by: Trdolan03 Posted at: 2018-09-25T04:51:33.200Z Reads: 174

```
Is your wh correct for both vescs or just for 1 on those trip data?
```

---
## \#403 Posted by: Saturn_Corp Posted at: 2018-09-25T04:52:58.867Z Reads: 180

```
No idea. I can only connect and see the debugging info. I'm hoping I'll get a bit of advice like you, and figure it out tomorrow.
```

---
## \#404 Posted by: taz Posted at: 2018-09-25T04:59:05.988Z Reads: 194

```
No idea then.
Mine is showing both VESC

![Screenshot_20180925-075744_metr|243x500](upload://ovWv1TWfFea9ksoV7H73vclahRV.jpeg)
```

---
## \#405 Posted by: rpasichnyk Posted at: 2018-09-25T06:04:09.408Z Reads: 180

```
Go to Settings, click on Show Logs and send to support@metr.at, thanks
```

---
## \#406 Posted by: Trdolan03 Posted at: 2018-09-25T06:09:34.990Z Reads: 180

```
Sent 10 char
```

---
## \#407 Posted by: rpasichnyk Posted at: 2018-09-25T11:09:06.037Z Reads: 176

```
1. You have CAN Fwd enabled. Why did you enable it? You should leave it disabled.
2. Please read carefully and do all the steps mentioned here https://vesc-project.com/node/178. Complete Wizards for both VESCs.
```

---
## \#408 Posted by: Riako Posted at: 2018-09-25T13:56:08.167Z Reads: 178

```
Hi Roman, glad to say @Surfer find one interesting point to (try to) solve my issues.
Locking the apps seems to work great, but I only make less than 2km ride (and stop the record to not lost it ^^ so bad habit) and two other almost 1km rides.
Tonight I will make a 5km ride test (usually the apps should be closed before the end of the ride ! So we will see !!!).
Thanks to all once again for your help :pray:
```

---
## \#409 Posted by: Riako Posted at: 2018-09-25T19:12:09.424Z Reads: 190

```
Tonight ride, I made a bit more than 10km (my bad if it doesn't take the 5 1st kms of the ride, I did lock the apps to don't crash :sweat: :sweat_smile: ) 
https://metr.at/r/ZvL4k
Some questions for you guys, is the 285Wh energy is what it was draw from my pack ? (10s 5Ah 185Wh ?)
And I regen 23Wh ? (Almost 2 km of ride ! :blush: )
But from the last 5km I could that now my phone can reccord well my ride !!!!
Hiiiiaaaaaaaaaaaaaaaaaaaaaaaaaaaaaa
http://www.reactiongifs.com/r/2013/05/Jim-Carey_Excited.gif
So has I have economize a new phone to buy, I will try to get a way to find a W10 computer with BT :blush:
Thanks all of you once again, Big Up @Surfer and @rpasichnyk :v: 
Now I will could try to play with some  Overlay vids !
```

---
## \#410 Posted by: rpasichnyk Posted at: 2018-09-25T19:35:37.805Z Reads: 178

```
I am glad it helped, thank you @Surfer! The Wh consumption is indeed wrong, and that's because of 2 reasons:

1. Something is wrong with your wired connection between VESC and Metr Pro. I remember you have a lot of UART errors in the log. Check the cables?
2. There is a multiply bug in current Metr Pro firmware, which usually happens after several UART interruptions. We have a fix coming soon. It will be the first official Metr Pro firmware update :slight_smile:
```

---
## \#411 Posted by: Riako Posted at: 2018-09-25T19:37:57.241Z Reads: 185

```
Ok, thanks Roman, I will tcheck this !
I see that metr note me I got 7 ESC, when I right a mode it write it 7 times ... 
https://amadridefr.files.wordpress.com/2018/09/screenshot_20180925-190313.jpg
```

---
## \#412 Posted by: Trdolan03 Posted at: 2018-09-26T03:34:12.480Z Reads: 187

```
I got my app to have all the data at the expense of my records with a simple uninstall- reinstall.
```

---
## \#413 Posted by: rpasichnyk Posted at: 2018-09-27T17:32:12.344Z Reads: 199

```
Metr Pro Firmware update v3.63 is out!
You can upgrade Over The Air

1. Power on.
2. Go to Settings, click on blue gear
3. Click on Upgrade

https://gph.is/2OVBZIy

If you have issues connecting to Metr Pro after upgrade, go to your phone settings and turn Bluetooth Off and On again (happens on some really old phones).

The new firmware includes support for DieBieMS :heart: and FOCBOX Unity :rocket: (beta, no Modes yet). Also highly recommended if you experience multiply bug (@Riako, @rene)
```

---
## \#414 Posted by: rene Posted at: 2018-09-28T18:44:53.497Z Reads: 189

```
Upgrade worked like charm ... will test tomorrow on new 12s10p... if all spot welding goes well.
```

---
## \#415 Posted by: never4getf150forums Posted at: 2018-09-28T22:05:11.294Z Reads: 189

```
is there a reason why the module will all of the sudden start automatically applying settings to the focbox? i've pin pointed an issue where the motors would not work at all, and it seems like the metr module is changing the settings by itself .. but this wasn't an issue in the past, started happening all of the sudden.
```

---
## \#416 Posted by: rpasichnyk Posted at: 2018-09-29T07:27:30.875Z Reads: 186

```
This might be Startup Mode. From the Modes tab you can assign one of your modes to be a startup mode and it will automatically apply when you power on your VESC, even if your phone is not around.

To disable this, open Modes tab, click on the menu dots above and select Clear Startup Mode.
```

---
## \#417 Posted by: sofu Posted at: 2018-09-29T07:34:49.027Z Reads: 184

```
Does the app log the actual fault instead of just showing a red number? I can't seem to find where to read the fault...
```

---
## \#418 Posted by: rpasichnyk Posted at: 2018-09-29T07:37:53.339Z Reads: 183

```
Yes, it's tricky. I need a better way of visualising the faults. If you can't find it, you can go to Settings and click on Show Logs. There search for `!!!Fault`
```

---
## \#419 Posted by: sofu Posted at: 2018-09-29T07:39:24.481Z Reads: 184

```
What about showing the faults of something that happened during a ride? All the log says is "Setting PositionSource.active to true"...
```

---
## \#420 Posted by: rpasichnyk Posted at: 2018-09-29T07:42:04.048Z Reads: 184

```
Can you upload the record with a fault? It should be possible to see it, after you upload
```

---
## \#421 Posted by: sofu Posted at: 2018-09-29T07:48:29.466Z Reads: 188

```
Here it is, I don't see anything? https://metr.at/r/JX1WJ
```

---
## \#422 Posted by: rpasichnyk Posted at: 2018-09-29T08:03:21.027Z Reads: 201

```
Yes, it's very hard to see a fault, when a record is so big. Try to make smaller records next time. But here you go:

![30|605x500,70%](upload://P0TcHLzFBtzZppmj1YRezUAjj2.png) 

Unfortunately that doesn't help much, because the fault code is 138 which seems like corrupted data and not the real fault.

Did you update Metr Pro firmware to latest?
```

---
## \#423 Posted by: sofu Posted at: 2018-09-29T08:05:22.050Z Reads: 199

```
I did. It's on the latest firmware

Well at least if it's not a real fault I can rest easy tonight 🤣

Maybe there can be a way to highlight faults in the web UI? or a way to adjust the resolution of the graph so the faults are more obvious?
```

---
## \#424 Posted by: janpirate Posted at: 2018-09-29T17:28:33.352Z Reads: 194

```
yeah i have the same questions... anyone try it with dual vesc 6 from Flipsky ?
```

---
## \#425 Posted by: janpirate Posted at: 2018-09-30T02:51:50.097Z Reads: 197

```
just received email from flipsky. it is support :)
```

---
## \#426 Posted by: Eretron Posted at: 2018-09-30T15:44:59.489Z Reads: 204

```
DieBieMS support :muscle::muscle::muscle:

You got me with this, I have just ordered one from you.


Just one thing... Since this will be used with Hummie deck, and that deck has 2 layers of carbon between wood, will it interfere with the bluetooth signal? Ive ordered one with small external antenna just to be safe...
```

---
## \#427 Posted by: Riako Posted at: 2018-09-30T17:53:28.914Z Reads: 216

```
Thx Roman, seems to work great directly :+1: 
I make the upgrade open air just now after the evening ride, it just a minute !
And it corrects the Wh consume (? right ?), directly of my current ride from I don't remember exactly to 117Wh (therefore I was around +200/230Wh ... with my 185Wh pack at around 35% at the end of the ride). Cool !
I check as you told me the wiring of the module and put some more heat glue to fix and secure all.
Now when I write modes it well applies to only 2 vesc ;) 

:blush: THANKS ROMAN !!! 

Now I got full ride recorded 
https://metr.at/r/5wKVM
But I got to find the good vesc ......... :laughing: 
https://metr.at/r/5nWnZ
```

---
## \#428 Posted by: visnu777 Posted at: 2018-09-30T18:09:17.422Z Reads: 200

```
I have no luck with the modules. I just tried the upgrade but it got stuck at 54% (its still there). How should I handle this? At some point I have to close the App I guess, it will shutdown the process when I switch to another one :(
```

---
## \#429 Posted by: rpasichnyk Posted at: 2018-09-30T18:20:40.702Z Reads: 195

```
No problem. Shut down everything, force close the app, power on, try again. What phone do you have?
```

---
## \#430 Posted by: visnu777 Posted at: 2018-09-30T18:22:12.284Z Reads: 198

```
A Motorola Moto E (LTE) running Lineageos (Android 7.1) :) Thanks, I'll try :)

edit: Thanks, it worked :)
```

---
## \#431 Posted by: Brucey0 Posted at: 2018-10-01T13:42:53.671Z Reads: 193

```
Hi Team,

Question, Timeout Brake Current, what is this for and what should it be set to?

Thank you 👍
```

---
## \#432 Posted by: amazingdave Posted at: 2018-10-01T14:02:27.668Z Reads: 191

```
It’s to stop you if your remote dies or disconnects. I never used to use it at slow speeds but now I’m going 30mph it is set.

Trial and error for the right amps for your setup and comfort. Remember that you want the board to stop but not throw you off.
```

---
## \#433 Posted by: Brucey0 Posted at: 2018-10-01T14:20:44.491Z Reads: 195

```
Thanks Dave, my question isn’t regarding brake currents but rather in the setup programming screens of the Metr app one of the settings is headed Timeout Brake Current. Does this limit the time you can be applying the brakes?

Appreciate the help guys...
```

---
## \#434 Posted by: Silverline Posted at: 2018-10-01T15:04:12.803Z Reads: 196

```
If i want to read out "faults" and fault via the terminal in the metr app, what code do i use then, to jump via can-bus to my slave vesc ? My metr module is connected to my master vesc,,,, Thanks....

Oh BTW... when "Multiply data" and "Dual data" is set to ON, the total WH i get in my logs, is the total from both the motors right ?
```

---
## \#435 Posted by: Eretron Posted at: 2018-10-02T02:29:41.320Z Reads: 192

```
@rpasichnyk

Do you have any idea when you will be able to ship units that were purchased a few days ago?
```

---
## \#436 Posted by: rpasichnyk Posted at: 2018-10-02T07:45:59.258Z Reads: 195

```
@Silverline yes it is the total Wh. To read faults from slave VESC, enable CAN Fwd, open Terminal and type `faults`. To read from master, disable CAN Fwd, open Terminal and type `faults` 
@Eretron Soon™ https://metr.at/faq#q1
```

---
## \#437 Posted by: Silverline Posted at: 2018-10-02T09:39:09.658Z Reads: 198

```
Thanks.   So no need for "can id" only "can fwd" ?
```

---
## \#438 Posted by: rpasichnyk Posted at: 2018-10-02T11:50:07.457Z Reads: 197

```
CAN ID has to be set correctly as well, when CAN Fwd is enabled.
```

---
## \#439 Posted by: taz Posted at: 2018-10-02T11:59:35.498Z Reads: 201

```
This is not the most intuitive way. Couldn't you make the software inquire the faults from both vescs automatically?
Also, does that mean that recorded faults are only from one vesc?
```

---
## \#440 Posted by: rpasichnyk Posted at: 2018-10-02T12:00:52.883Z Reads: 200

```
Yes, I agree, it is on TODO list 🙂
```

---
## \#441 Posted by: neiru37 Posted at: 2018-10-02T20:12:42.171Z Reads: 205

```
Is there a way to get the raw csv file for the records? If not, can I make a visualization request? I'd like to see a bar graph with time labels on how much I spend on a certain speed range. Something like this but instead if heart rate zones it's speed zones.

![26%20PM|690x288](upload://goLj8pIZbHwsSY8Jjt00m4CIRDz.png)
```

---
## \#442 Posted by: rpasichnyk Posted at: 2018-10-03T07:52:36.429Z Reads: 202

```
This is such a cool idea! Thanks!
Will think about it for sure :)
```

---
## \#443 Posted by: janpirate Posted at: 2018-10-05T20:08:30.617Z Reads: 202

```
please check your msg and email. wrongly place an order pcb. i need small external antenna. thanks :slight_smile:
```

---
## \#444 Posted by: bevilacqua Posted at: 2018-10-15T20:23:17.636Z Reads: 201

```
you can convert the meter file to .json. There you have a field called "speed". just ad "?format=json" at the end of the URL. 

If you got access to Matlab I can send you a function to convert .json files to .csv (with the same structure as on acks app and so on.
```

---
## \#445 Posted by: amazingdave Posted at: 2018-10-18T17:36:15.095Z Reads: 195

```
@hexakopter @rpasichnyk  I’ve just managed to damage the cable between my module and mini antenna....

Can I buy a spare?
```

---
## \#446 Posted by: hexakopter Posted at: 2018-10-19T12:37:00.321Z Reads: 197

```
Yes, that is possible. I will write you a PM.
```

---
## \#447 Posted by: Trdolan03 Posted at: 2018-10-19T19:23:30.390Z Reads: 191

```
Is there anyway to view lifetime stats?
```

---
## \#448 Posted by: SeanHacker Posted at: 2018-10-19T19:29:32.877Z Reads: 199

```
Click this. Select All Time

![Screenshot_20181019-122829__01|690x93](upload://kXKEEdKNhnyB0ey33HttopScO6c.jpeg)
```

---
## \#449 Posted by: Nesquick90 Posted at: 2018-10-21T17:34:06.936Z Reads: 209

```
Quick question. 
Has any of you guys experienced metr not recording the speed (Top Speed, Average Speed) and the distance?
https://metr.at/r/iGYza
Using Flipsky Dual FESC 6.6.

Best Regards
Nesquick
```

---
## \#450 Posted by: hexakopter Posted at: 2018-10-21T17:51:52.984Z Reads: 197

```
When you go to "Settings" -> "Location" -> "Prefer GPS", is it enabled? When you don't have GPS available and use the VESC ERPM value for speed and distance calculation please turn "Prefer GPS" off and check that "Settings" -> "Motor" -> "Motor poles", "Wheel diameter" etc. are set correctly.
In the realtime tab the speed and distance is shown correctly?
```

---
## \#451 Posted by: Gdunn416 Posted at: 2018-10-21T18:43:13.188Z Reads: 195

```
I wanted to chime in and say that the Metr module is working great. I was worried about not buying the version with the extended antenna, but I haven't had a single disconnect, even if I am in a different room as the module. 
I had an issue with some weird numbers recorded (I think the odometer) but that was fixed in the latest update.
```

---
## \#452 Posted by: Nesquick90 Posted at: 2018-10-21T22:14:38.487Z Reads: 194

```
Thanks for your reply. Under the location tab, everything is on and GPS Accuracy is "0".
On the motor tab, everything is setup correctly. 

Regarding the real time data on the app itself, the current speed works, but the distance does not.
Any suggestions?

Best Regards
Nesquick
```

---
## \#453 Posted by: hexakopter Posted at: 2018-10-21T22:48:00.436Z Reads: 184

```
As I said, please disable "Prefer GPS". You can also click on the little question mark beside each setting, to get an idea what it is for. That way you also record your GPS coordinates to see them on your uploaded record later (when GPS was available), but your distance and speed also works without GPS. Just in some rare cases where your motor does not spin all the time (like freewheel etc.) I would enable that setting.
```

---
## \#454 Posted by: Nesquick90 Posted at: 2018-10-21T22:52:19.677Z Reads: 187

```
Oh! My bad. I misinterpreted what you said on the first reply. Yeah it makes sense. 
Will test is tomorrow or next weekend. Thanks for your help.
```

---
## \#455 Posted by: KrisKraanen Posted at: 2018-10-24T14:57:40.541Z Reads: 186

```
if i buy the pcb antenna version can connect my own external antenna to it?
```

---
## \#456 Posted by: taz Posted at: 2018-10-24T16:18:44.272Z Reads: 197

```
Hi, when I select the use of barometer then the altimeter values are completely wrong. Is there some other setting to correct this?
Going to the selftest menu of my phone my sensor works fine ![Screenshot_20181024-193809_HwModuleTest|243x500](upload://sfBDeku7P2ZrihphLf5xxb9pOFi.jpeg)
```

---
## \#457 Posted by: rpasichnyk Posted at: 2018-10-24T19:44:39.133Z Reads: 181

```
Are they completely-completely wrong, or maybe just showing relative altitude? Close to 0 when you start the app, and then changing as you go.
```

---
## \#458 Posted by: taz Posted at: 2018-10-24T19:51:45.591Z Reads: 181

```
The relative altitude seems correct. However instead of showing a correct absolute value it starts at around 0m for the first ride of the day and then from -100m for the second and goes to 30m when I reach my departure point.
```

---
## \#459 Posted by: Pimousse Posted at: 2018-10-24T21:30:30.799Z Reads: 188

```
Hi @rpasichnyk, some people, me included, have troubles with writing configuration.
It happened to a guy when he applied a mode. Metr Pro messed parameters up.
On my side, I having issue when switching BLDC to FOC (and reverse) only. This doesn't work using VESC Tool on mac over Bluetooth.
However, this works using Metr app.

Are there some other feedbacks in this way ?
```

---
## \#460 Posted by: rpasichnyk Posted at: 2018-10-25T07:29:41.199Z Reads: 179

```
No, I didn't get any reports regarding this issue. I assume you are using latest VESC Tool and VESC firmware? What parameters get messed up?
```

---
## \#461 Posted by: Pimousse Posted at: 2018-10-25T07:54:23.556Z Reads: 182

```
Oh sorry : FW 3.40 official, VT 0.95 from your repo.

I.ll get in touch with the other guy and report back more details of his issue.

Thanks for support, as always ! :slight_smile:
```

---
## \#462 Posted by: Pimousse Posted at: 2018-10-25T14:39:41.581Z Reads: 189

```
Ok, more details gathered :

- Dude A (Tartopom) : Metr Pro, FW 2.18 (raptor 2 downgraded).
He applied a custom Beginner mode, no issue. Then he came back to full power mode. This messed CAN ID and BLDC Hall sensors table up. Others parameters like Motor/batt min/max current were ok.
- Dude B (Thomas P.) : after switching modes, nothing was working (no much more details). Don't know the FW (only Metr app version : 3.3.1 )
- Dude C (@goldenkiller) : same issue as Dude A (BLDC Hall sensor table values mixed) using Metr Pro + FW3.40. Not sure about CAN ID.

Other bug reported by Dude A : After having created a new mode in Metr app, if you want to delete another one, sometimes it deletes 2 modes.

That's all I could gather from french Metr Pro users.
If you need more info, feel free to ask.

Cheers !
```

---
## \#463 Posted by: rpasichnyk Posted at: 2018-10-26T19:33:48.537Z Reads: 182

```
[quote="Pimousse, post:462, topic:57780"]
After having created a new mode in Metr app, if you want to delete another one, sometimes it deletes 2 modes
[/quote]

I was able to see and fix it, thanks!

For applying modes and parameters mess up, it would be great if the dudes can reproduce the issues repeatedly and send the log file to support@metr.at
```

---
## \#464 Posted by: ajelex Posted at: 2018-10-27T02:59:36.716Z Reads: 194

```
Hey roman. The app is great. I just installed it in my raptor 2 and it works more or less perfectly! Truly easy to set up and use.

Just got 2 questions: It seems like my ESC temperature is no recorded correctly anymore. It’s always at 25C when it used to work. I don’t know what changed?

https://metr.at/r/GIz6I

Do you have any plan on adding apple shortcut functionalities? It would be awesome to quickly being able to launch metr in the background using Siri.
```

---
## \#465 Posted by: iTzDiego Posted at: 2018-10-27T03:10:06.058Z Reads: 183

```
[quote="rpasichnyk, post:1, topic:57780"]
Worldwide shipping: €12
[/quote]

What is considered "worldwide"?
```

---
## \#466 Posted by: taz Posted at: 2018-10-27T06:14:12.321Z Reads: 185

```
Did you find a solution to the altitude problem I am having?
```

---
## \#467 Posted by: rpasichnyk Posted at: 2018-10-27T08:09:36.905Z Reads: 180

```
Thanks for reporting, I will have a look. Siri shortcuts are interesting, will look into that as well!

@taz The app shows relative elevation instead of absolute when using barometer. And I don’t reset it when starting a new ride. I will so it always starts at 0 in the next version. Thanks!
```

---
## \#468 Posted by: taz Posted at: 2018-10-27T09:04:12.905Z Reads: 181

```
Couldn't you use the Gps altitude for the start of the ride and then use the barometer for relative altitude changes?
```

---
## \#469 Posted by: hexakopter Posted at: 2018-10-27T09:40:01.408Z Reads: 182

```
[quote="iTzDiego, post:465, topic:57780"]
What is considered “worldwide”?
[/quote]


Worldwide means that it doesn't matter if you live in Europe, the US, Australia, or anywhere else around the world, you pay the same for shipping. If you live on an island with special postal rules, contact support@metr.at and we will check if it is possible to ship to you.
```

---
## \#470 Posted by: Pimousse Posted at: 2018-10-29T14:46:58.688Z Reads: 184

```
Hi @rpasichnyk and @hexakopter,
Could you add a point in the FAQ stating that the plug has to be reversed for a use with ESCAPE ?

I spent half an hour with a french guy for troubleshooting an issue with Metr Pro. 
He just didn't know that pins had to be swapped... :pensive:

Thanks mates !
```

---
## \#471 Posted by: Gdunn416 Posted at: 2018-10-29T23:15:10.845Z Reads: 181

```
I may be alone in this request, but does anyone else here think the following would be a useful feature?

Metr app notifies (Vibration and/or pop-up) when battery has reached additional specified voltages.

I realize these notifications exist for low and cut-off voltages, but it would be nice to have one for charging as well. I don't like to charge my batteries all the way to 4.2v, which means that I need to keep a constant eye on Metr or the meter on the board. Plus, I can be a forgetful person.
```

---
## \#472 Posted by: taz Posted at: 2018-10-30T09:00:41.133Z Reads: 180

```
There is already an end of charge voltage setting for that particular reason.
```

---
## \#473 Posted by: lrdesigns Posted at: 2018-10-30T14:39:47.477Z Reads: 184

```
[quote="Brucey0, post:433, topic:57780"]
my question isn’t regarding brake currents but rather in the setup programming screens of the Metr app one of the settings is headed Timeout Brake Current. Does this limit the time you can be applying the brakes?

Appreciate the help guys…
[/quote]

Might be wrong thead but anyhow this is an automatic brake if your remote disconnects “timeout” . Most people leave it off as it can be dangerous if set wrong. Needs road testing and adjustment.

I think its intention is to stop a runaway board. But if its set too high it could be real bad, imagine your riding along at high speed, your remote disconnects then the brakes come on hard then you fly like sack of potatoes into traffic. FUN!
```

---
## \#474 Posted by: Gdunn416 Posted at: 2018-10-30T15:48:04.885Z Reads: 179

```
Your right. Sorry for the noise! I'm not sure why I thought that both notification settings were for low voltage. Thanks for pointing that out to me.
```

---
## \#475 Posted by: KrisKraanen Posted at: 2018-11-01T18:03:51.354Z Reads: 179

```
i have the metr pro, it updates quiet fast so i have the battery level but without doing anything it jumps from 28 up to 39 is there a way to slow the updates so it jumps around less update interval in miscellaneous doesn't seem to be doing anything
```

---
## \#476 Posted by: hexakopter Posted at: 2018-11-03T21:20:06.317Z Reads: 173

```
What do you mean with "_without doing anything_ it jumps from 28 up to 39"? Do you mean that when you strain the battery while driving and then stop, the battery level goes up? Thats normal because the value is calculated from the battery voltage which goes down while you are pulling some amps.
```

---
## \#477 Posted by: caustin Posted at: 2018-11-03T22:43:37.295Z Reads: 173

```
Yup

10char
```

---
## \#478 Posted by: KrisKraanen Posted at: 2018-11-04T11:24:30.699Z Reads: 172

```
i plugged the module in my esc and plugged a 4s battery in for test purpose to see if i could connect and if it al worked, it did but the battery level jumps around without me giving an input or anything
```

---
## \#479 Posted by: hexakopter Posted at: 2018-11-04T14:41:12.929Z Reads: 168

```
Strange. So I guess your battery voltage is also jumping around? You can change your displayed values and layout in the realtime data tab with long pressing on the screen and then arrange the items.
```

---
## \#480 Posted by: hexakopter Posted at: 2018-11-07T21:14:41.020Z Reads: 177

```
[quote="Pimousse, post:470, topic:57780"]
Could you add a point in the FAQ stating that the plug has to be reversed for a use with ESCAPE ?
[/quote]


Totally forgot to mention that we updated the FAQ page and added information about Metr Pro connection, the four absolutely needed pins, external/internal antenna change etc. You can have a look here: https://metr.at/faq
Let us know if you think there is anything else missing.
```

---
## \#481 Posted by: ethel Posted at: 2018-11-08T23:30:26.144Z Reads: 191

```
Raptor 2.0 (old motors) with metr data  [Here](https://metr.at/r/QXgAu)

Updated FW 3.8 from 2.1.8
Added Metr module 
SR front truck

I have multiple faults in the data, mainly over current. One fault I was not moving. Could be my settings are too high?

![image|374x500](upload://jI5oLFRXoReMNJfQQEpO5pDWRyW.jpeg) 

You can see wheels starting to crumble 😮 motors and hanger were hot on touch.

![image|375x500](upload://ysbPAZsvTCMkssmzupnx4KnWs3E.jpeg) 

![image|666x500](upload://47JI6P1TvuQSGo3BKpekVqhkC3S.jpeg)

![image|281x500](upload://9zEJGAnqd6EtltQXPlZnvPIY3vn.jpeg)
```

---
## \#482 Posted by: rpasichnyk Posted at: 2018-11-09T08:34:31.609Z Reads: 178

```
Your settings are definitely too high. I recommend to lower down Max Motor Current :+1:
```

---
## \#483 Posted by: KrisKraanen Posted at: 2018-11-09T10:14:01.355Z Reads: 185

```
i have the module but the update interval doesn't seem to do anything now i get updates so fast that the battery voltage still jumps around a bit
```

---
## \#484 Posted by: KrisKraanen Posted at: 2018-11-09T10:17:34.215Z Reads: 193

```
https://youtu.be/ifN4WLQNR_I
```

---
## \#485 Posted by: rpasichnyk Posted at: 2018-11-09T13:58:27.044Z Reads: 195

```
It's because your VESC sends a bit inaccurate measurements. No worries, this is totally fine.
```

---
## \#486 Posted by: Quiles Posted at: 2018-11-09T14:21:32.175Z Reads: 200

```
hi @rpasichnyk - when are you planning to add 3.39 support? Thanks!
```

---
## \#487 Posted by: rpasichnyk Posted at: 2018-11-09T15:05:06.971Z Reads: 189

```
It’s there already. 3.39 and 3.40 are supported. Is threre something not working for you?
```

---
## \#488 Posted by: KrisKraanen Posted at: 2018-11-09T15:43:13.471Z Reads: 192

```
But the update in millisec wont change i put it to 2000 but still it updates this fast
```

---
## \#489 Posted by: Quiles Posted at: 2018-11-09T23:50:40.811Z Reads: 196

```
It's perimetr app that's giving me the msg below![30|281x500](upload://q2gAMQAXEeiJ73znYhPyCGUjPAj.jpeg)
```

---
## \#490 Posted by: hexakopter Posted at: 2018-11-10T00:01:14.913Z Reads: 188

```
What app version are you using? You can see the version number after going to settings and then scroll down to the bottom. 
I think you are using an outdated app version. You should update the app to the newest version.
```

---
## \#491 Posted by: Quiles Posted at: 2018-11-10T01:12:18.432Z Reads: 191

```
1.4.2....is it old?...there's no update for this app on android store. Last App update: April/28/2018
```

---
## \#492 Posted by: taz Posted at: 2018-11-10T05:36:39.870Z Reads: 190

```
Are you using the separate perimetr app?
The new metr app has integrated the perimetr app so you no longer have to download it separately.
Just go to modes in the metr app,  upper right corner to enter it.
```

---
## \#493 Posted by: Hummie Posted at: 2018-11-10T05:55:07.182Z Reads: 191

```
Can this possibly transmit the separate series cell voltages?
```

---
## \#494 Posted by: rpasichnyk Posted at: 2018-11-10T08:54:30.904Z Reads: 194

```
It can if you have DieBieMS
https://media.giphy.com/media/3OC2r75I9xp9M2hdxa/giphy.gif
```

---
## \#495 Posted by: lrdesigns Posted at: 2018-11-10T09:21:01.770Z Reads: 194

```
DUDE. :exploding_head:
```

---
## \#496 Posted by: Quiles Posted at: 2018-11-10T10:07:36.330Z Reads: 197

```
on perimetr you can manage the majority configs of the vesc....on metr modes, you can only change a few.

For example, i was playing with FOC switching frequency....you can only change it by perimetr app.
```

---
## \#497 Posted by: taz Posted at: 2018-11-10T10:31:32.920Z Reads: 196

```
Again, the perimetr app has been integrated in the metr app.
Just go to modes tap, hit the 3 dots in the upper right corner and select perimetr.
```

---
## \#498 Posted by: Quiles Posted at: 2018-11-10T12:00:48.719Z Reads: 199

```
oh my..:open_mouth:..i am so stupid....thanks @taz
```

---
## \#499 Posted by: evoheyax Posted at: 2018-11-13T07:20:04.140Z Reads: 198

```
@rpasichnyk Back when you first released this app, I was competing with my own app. I quickly brought some updates, and I noticed it kept you on your toes to keep innovating also. I slowed down in development, but you have pushed 5 light years ahead.

I was upset at the shit that happened back then, but I can't let that stop me from using the best tech, so I will be ordering a module soon. My 1 request for you though, is please, PLEASE, add support for 4 vescs instead of just 2. I saw you mentioned it's possible with this new module, just not implemented. I've been seeing a lot more 4wd boards lately, so I know I'm not the only one waiting for this!

Love the diebms integration. Could you post a wiring diagram for this? Is it just the CAN L VESC -> CAN L BMS and CAN H VESC -> CAN H BMS?

Please, 4wd support asap! If you need a beta tester for it, I'm happy to do so.
```

---
## \#500 Posted by: rene Posted at: 2018-11-13T07:36:07.832Z Reads: 196

```
[quote="evoheyax, post:499, topic:57780"]
e CAN L VESC -&gt; CAN L BMS and CAN H VESC -&gt; CAN H BMS
[/quote]

you can find the wireing in the DieBieMS thread. its all four wires DieBieMS needs power from the vesc.
```

---
## \#501 Posted by: evoheyax Posted at: 2018-11-13T07:46:29.657Z Reads: 212

```
[quote="rene, post:500, topic:57780"]
you can find the wireing in the DieBieMS thread.
[/quote]

Ok, I'll check again. There's actually 4 threads (3 were group buy threads, and there's info all over these threads I'm finding), so It's a bit messy, which I why I'm asking for clarification. The DieBieMS also has 5 pins from the canbus to the 4 on the vesc. I saw this picture:

https://www.electric-skateboard.builders/uploads/db1493/original/3X/c/4/c41b073b3b802cde372805e0e67fe719bed3172c.jpeg

Do you know what 0R is? This doesn't seem right either, as CAN H and CAN L are the middle 2 pins on the vesc...

This is why I'm asking because the info I found is confusing at best. I saw you got it up and running. Congrats! I can't sleep right now because I'm too excited to get it going, haha.
```

---
## \#502 Posted by: rene Posted at: 2018-11-13T08:30:18.013Z Reads: 212

```
here is a answer from @JTAG 

https://www.electric-skateboard.builders/t/diebiems-v0-8-2nd-batch-total-48pcs-closed/58327/289?u=rene
```

---
## \#503 Posted by: evoheyax Posted at: 2018-11-13T08:48:47.759Z Reads: 212

```
Thank you. That explains how the bms picks up the push to start also! The more you understand the DieBieMS, the more attractive it becomes.
```

---
## \#504 Posted by: uigiroux Posted at: 2018-11-16T18:09:37.599Z Reads: 206

```
Would you be able to make a wire diagram for 4 VESC's with a DieBieBMS that's also using canbus.
```

---
## \#505 Posted by: evoheyax Posted at: 2018-11-17T03:34:05.846Z Reads: 205

```
I will be putting a lot together a guide soon with everything I find when I get it working myself haha. Right now, I’m stuck on the balance connector lol.

@rpasichnyk how often do you ship out modules? I’m dying to get it going with the diebiems haha
```

---
## \#506 Posted by: hexakopter Posted at: 2018-11-17T05:20:45.730Z Reads: 203

```
[quote="evoheyax, post:505, topic:57780"]
@rpasichnyk how often do you ship out modules? I’m dying to get it going with the diebiems haha
[/quote]


Have a look at https://metr.at/faq#q1. Your order has already been shipped out on 14. Nov 2018 and you can see your tracking number when logging in to your PayPal account or check their mail that they send to you about the order being shipped.
```

---
## \#507 Posted by: evoheyax Posted at: 2018-11-17T18:25:16.381Z Reads: 194

```
Thank you! Sorry for not probing enough!
```

---
## \#508 Posted by: Saturn_Corp Posted at: 2018-11-17T21:17:57.182Z Reads: 199

```
@hexakopter does CAN ID refer to a specific ID number for each vesc, or is it simply 0 for the master and 1 for the slave vesc? Got my replacement antenna in the mail so everything is good again.
```

---
## \#509 Posted by: briman05 Posted at: 2018-11-17T21:45:53.649Z Reads: 189

```
Quick question what does the antenna do and do you need it? May have been posted before but missed it
```

---
## \#510 Posted by: Saturn_Corp Posted at: 2018-11-17T21:49:46.045Z Reads: 194

```
It increases the reception between your phone and Metr module. The bluetooth on the chip should be fine in most cases but if you have a carbon fiber deck or enclosure it's a good idea to have so you don't get disconnections.
```

---
## \#511 Posted by: Saturn_Corp Posted at: 2018-11-17T22:45:01.214Z Reads: 197

```
Reason I ask is because every time I have the Metr module on my board, I lose power to the motor on the slave vesc sometime during my next ride. Easy fix with the bldc tool but it happens every time! I say this sitting on a curb where one of my motors just stopped working.
```

---
## \#512 Posted by: rpasichnyk Posted at: 2018-11-18T19:59:19.764Z Reads: 195

```
When do you lose power? After you change modes? After you power cycle your board? This doesn't sound good. Can you send some logs?
```

---
## \#513 Posted by: Mich21050 Posted at: 2018-11-18T20:00:18.353Z Reads: 190

```
@rpasichnyk Quick question: Can I also pay via bank transfer because my paypal account has been hacked :slight_smile:
```

---
## \#514 Posted by: rpasichnyk Posted at: 2018-11-18T20:04:59.185Z Reads: 193

```
Yes you can, send email to support@metr.at
```

---
## \#515 Posted by: briman05 Posted at: 2018-11-18T21:24:36.556Z Reads: 198

```
I have a 8 ply maple deck and a abs cement
```

---
## \#516 Posted by: Saturn_Corp Posted at: 2018-11-18T22:53:08.931Z Reads: 196

```
After some more testing I discovered it usually happens after the board has been stationary for a while like at a stop light or while taking a short break to rest my feet. A simple restart of the board and it's good again until the next time it happens. No startup mode has been applied nor does it happen when any changes are made in the app. 

I will send logs soon.
```

---
## \#517 Posted by: Sharukh5996 Posted at: 2018-11-20T17:15:17.160Z Reads: 184

```
Is it possible to connect this to a meepo board ESC?
```

---
## \#518 Posted by: mikenyc Posted at: 2018-11-20T21:07:40.860Z Reads: 189

```
@rpasichnyk what kind of shrink wrap are you using to cover the board? i had to resolder the header onto the pcb because it broke off (probably vibrations). needed to cut the shrink wrap off. currently have it taped up with some kapton
```

---
## \#519 Posted by: hexakopter Posted at: 2018-11-21T20:33:49.969Z Reads: 186

```
@Sharukh5996 Respond to your mail that you have send to support@metr.at.

@mikenyc Some 16mm clear heat shrink. Unfortunately I don't remember the actual source. You should be able to find some online when searching for "16mm clear heat shrink".
The whole JST 7pin 2.0mm header broke off? Never heard about something like that and it must have been more then just vibrations to brake it. Is it possible that a bigger force was pulling on the connector, like a loose battery or something like that? Would be great if you can send a picture of the broken module to support@metr.at if you took one.
```

---
## \#520 Posted by: mikenyc Posted at: 2018-11-21T21:02:38.825Z Reads: 184

```
nah, didn't take a picture. it was inside the enclosure, not sure what could have tugged on it. it was pretty snug. perhaps the length of the cable was a bit much, i had to bend it awkwardly, thanks for letting me know about the shrink wrap, i'll check on amazon or ebay
```

---
## \#521 Posted by: Trdolan03 Posted at: 2018-11-22T19:54:45.367Z Reads: 190

```
Anyone else having issue with the TCP connection?
```

---
## \#522 Posted by: hexakopter Posted at: 2018-11-25T11:51:04.803Z Reads: 201

```
@Trdolan03 Is it working for you now? Do you had it working in the past and now it stopped working or do you have problems with setting it up?

@all I received a message that someone almost missed our Metr Pro **two year anniversary and Black Friday 20% sale**, because it is not mentioned in this main thread about the Pro module. Sorry about that.
So here a reminder that we have a 20% discount at the moment that is running out on 25/11/2018 7PM UTC (**[date=2018-11-25 time=19:00:00 format="LLLL" timezones="Europe/Paris|America/Los_Angeles"]**) so in slightly more than seven hours. You can find more details [here](https://www.electric-skateboard.builders/t/metr-pro-20-black-friday-sale/75554).

If you haven't seen it yet, we also released a new Metr app version with **Audio Announcements** :headphones:
You can find more infos in the following thread.


https://www.electric-skateboard.builders/t/configuration-and-telemetry-for-vesc-ios-android/13483/1207
```

---
## \#523 Posted by: Trdolan03 Posted at: 2018-11-25T17:07:50.996Z Reads: 193

```
@hexakopter it has worked in the past and stopped working. I tried yesterday and it wasn’t working. Is there something you changed that I should try again?
```

---
## \#524 Posted by: rpasichnyk Posted at: 2018-11-25T17:15:10.409Z Reads: 190

```
Try it again and if it doesn't work, send logs to support@metr.at
```

---
## \#525 Posted by: Trdolan03 Posted at: 2018-11-25T17:38:28.801Z Reads: 196

```
@rpasichnyk it is working now. The second “TCP server” wasn’t showing up yesterday on my phone as seen that it is today. The 10.0.0.24 wasn’t showing up ![image|281x499](upload://m1rFf8ZJvRnacoI9pKs2IXyXoxk.jpeg)
```

---
## \#526 Posted by: rpasichnyk Posted at: 2018-11-25T17:50:28.622Z Reads: 190

```
Awesome! The first one is your cellular, and probably 65102 port is blocked by your internet provider or something. The second is your Wi-Fi.
```

---
## \#527 Posted by: Trdolan03 Posted at: 2018-11-25T17:53:55.476Z Reads: 193

```
I wasn’t on WiFi when I was trying. That makes a lot of sense.
```

---
## \#528 Posted by: evoheyax Posted at: 2018-11-28T05:57:16.160Z Reads: 189

```
@hexakopter I see my tracking in my paypal, but when I click on it, it doesn’t go to a valid page. I tried the number through usps and dhl and it doesn’t give me anything. It’s been more than 2 weeks since I ordered. Any idea how I can track down where it is?
```

---
## \#529 Posted by: Indiangummy Posted at: 2018-11-28T06:23:06.169Z Reads: 189

```
Try tracking it here! They posted this in the black Friday discount thread
https://www.deutschepost.de/sendung/simpleQuery.html?locale=en_GB
```

---
## \#530 Posted by: hexakopter Posted at: 2018-11-28T06:31:53.998Z Reads: 191

```
@evoheyax Please use the link @Indiangummy posted.
Its also always helpful to check our [FAQ site](https://metr.at/faq#q2), where this link is also mentioned.

Checked your order number and it is waiting for pickup at your local post office since 19. Nov 2018.
```

---
## \#531 Posted by: amazingdave Posted at: 2018-11-28T10:47:25.790Z Reads: 200

```
Why is my metr pro creating extra wh and distance? My last standard metr did the same... 

There are no records with high figures to throw the stats....

![image|230x500](upload://pKQrukljbLT7H4Fga6ls2rYCTkF.jpeg)
```

---
## \#533 Posted by: SkaterBoy58 Posted at: 2018-11-28T12:43:57.223Z Reads: 194

```
@rpasichnyk Roman 
Does the metr app  auto detect the diebieBMS  if can bus id is set to 10 and produce new screens?
Thanks
```

---
## \#534 Posted by: rpasichnyk Posted at: 2018-11-28T13:33:31.753Z Reads: 197

```
@amazingdave it looks like a bug, please send logs (Settings -> Show Logs) to support@metr.at
@SkaterBoy58 yes DieBieMS is autodetected if it has CAN ID 10 (which is default, you don't need to do anything)
```

---
## \#535 Posted by: ethel Posted at: 2018-12-03T01:34:18.037Z Reads: 206

```
@rpasichnyk



What motor settings should I put down for carvon direct drive ? My energy consumption is off.

https://metr.at/r/a1kHq
```

---
## \#536 Posted by: bevilacqua Posted at: 2018-12-03T13:57:51.719Z Reads: 202

```
are you sure? @ a max speed of 60kph + direct drive copper losses it could be realistic (23wh/km). 

Whats your ride weight?
```

---
## \#537 Posted by: ethel Posted at: 2018-12-03T17:01:12.395Z Reads: 208

```
90Kg 

![image|281x500](upload://t4VosTnqcmQawLToq6bio8xRbhf.jpeg)
```

---
## \#538 Posted by: bevilacqua Posted at: 2018-12-03T17:07:52.874Z Reads: 198

```
It can be realistic, 107s are quite big and require big torque to start rolling...

But maybe roman finds something in the data.
```

---
## \#539 Posted by: rene Posted at: 2018-12-03T17:25:51.883Z Reads: 198

```
you got a motor pulley with ONE teeth?
and a wheel pulley with ONE teeth?
```

---
## \#540 Posted by: Indiangummy Posted at: 2018-12-03T17:26:22.275Z Reads: 195

```
its a direct drive.....so its a 1:1 ratio.
```

---
## \#541 Posted by: rene Posted at: 2018-12-03T17:27:04.272Z Reads: 192

```
ohh yeah - sure.
```

---
## \#542 Posted by: sayekim Posted at: 2018-12-03T18:44:33.560Z Reads: 198

```
This is normal for my torque drives. 

I got 45km range on my 12s6p with max speeds of 55kph. 

Maybe it’s even normal for belt too? Just go slower like under 45kph to get way more range.
```

---
## \#543 Posted by: hexakopter Posted at: 2018-12-03T22:35:40.199Z Reads: 198

```
The motor and wheel pulley count of 1 for direct drives is correct. Not sure about the motor poles of the Carvon hubs. But because the max speed of 60kph seems right to the motor specs the motor poles count should also be right.

Why do you think the energy consumption is off? The motor settings you show are just used for rpm based speed calculations.
```

---
## \#544 Posted by: ethel Posted at: 2018-12-03T22:51:08.485Z Reads: 196

```
It seemed like a lot of energy. Will try different wheels size to compare. Thank you all for input.
```

---
## \#545 Posted by: ElectricCoast Posted at: 2018-12-09T18:59:12.638Z Reads: 199

```
Hey guys I'm having two problem with my metr pro.  First I have to unpaired and then pair the metr pro each time I shut power off to my board to get it to connect via bluetooth.

Secondly nt metr pro is not reording my data like it use to automatically.  What am I doing wrong?
```

---
## \#546 Posted by: bevilacqua Posted at: 2018-12-09T21:23:16.533Z Reads: 205

```
is the FW of the Metr updated?

2nd, do you have auto-records enabled?

I'll send a video/gif in a moment

EDIT:
http://gifsstore.com/public/upload/gifs/15444720241544472021.gif
```

---
## \#547 Posted by: Soflo Posted at: 2018-12-10T19:53:26.118Z Reads: 200

```
I'm having the same exact problem with having to unpair then re-pair every time I connect.  I reached out to the developer and got nothing.  
Now I've changed my esc from 4.12 to 6.6 and my battery reading bounces all over the place now
```

---
## \#548 Posted by: evoheyax Posted at: 2018-12-10T20:43:49.606Z Reads: 206

```
6.6 has issues man.
```

---
## \#549 Posted by: sayekim Posted at: 2018-12-10T21:56:03.306Z Reads: 215

```
I ran into a weird problem today. When I set a start up mode and then change modes after I switch on the board with the metr app on it applies the new mode but it leaves one motor behaving like it hasn’t run motor detection  yet. 
Only way to solve it for me was to run motor detection again with the desktop app and not use the start up mode since I narrowed it down that it only happens with this mode, and it does so every time. 

I’m using dual escapes with 3.40 firmware and the metr app for iphone. 

@rpasichnyk
```

---
## \#550 Posted by: Soflo Posted at: 2018-12-10T22:59:35.473Z Reads: 212

```
What kind of problems do the 6.6 have?  Is this documented?
```

---
## \#551 Posted by: ElectricCoast Posted at: 2018-12-11T01:48:29.134Z Reads: 213

```
It's a known issue from flipsky and the voltage fluctuations with the 6.6 FSESC from them.
```

---
## \#552 Posted by: rpasichnyk Posted at: 2018-12-11T09:25:33.789Z Reads: 212

```
Try the latest version of the metr app v3.4.8. If you still have the problem, send Settings -> Show Logs to support@metr.at
```

---
## \#553 Posted by: StefanMe Posted at: 2018-12-11T09:36:08.931Z Reads: 210

```
How it shows up? Just wired voltage readings? Problem with soft cut off because of wrong readings?
```

---
## \#554 Posted by: hiboute Posted at: 2018-12-12T12:31:18.574Z Reads: 208

```
It is like this:
https://metr.at/r/a91F7
```

---
## \#555 Posted by: hiboute Posted at: 2018-12-12T12:38:00.034Z Reads: 206

```
Regarding new functionalities, i really wish we were able to:
- combine multiple rides. On long rides, if i stop too long, this will create a new entry. The « solution » would be to set the stop time longer but not so convenient.
- ability to remove stop/idle time from data.
- to set the motor config per metr module. Currently If i have two different boards with two different metr module, the motor info is the same for the two. I have to change it between rides.
- renaming saved config in expert mode
```

---
## \#556 Posted by: amazingdave Posted at: 2018-12-12T13:00:38.386Z Reads: 199

```
That is some serious voltage sag. What batteries are you using?
```

---
## \#557 Posted by: hiboute Posted at: 2018-12-12T13:10:23.239Z Reads: 208

```
No sag, this is the flipsky 6.6.
The battery is a 10s4p samsung 30q.
Here is the same ride with focbox:
https://metr.at/r/BJml4
```

---
## \#558 Posted by: rpasichnyk Posted at: 2018-12-12T14:46:00.389Z Reads: 210

```
[quote="hiboute, post:555, topic:57780"]
* to set the motor config per metr module. Currently If i have two different boards with two different metr module, the motor info is the same for the two. I have to change it between rides.
[/quote]
This is supported. Connect your first board (make sure it is online) and make changes to Motor settings. Turn off your first board. Connect your second board (make sure it is online) and make changes to Motor settings. Turn off your second board. Turn on your first board and you will see settings change automatically.
[quote="hiboute, post:555, topic:57780"]
 * renaming saved config in expert mode
[/quote]
Long press on saved config and you will be able to rename it.
```

---
## \#559 Posted by: hiboute Posted at: 2018-12-12T14:57:18.419Z Reads: 199

```
Thank you!
```

---
## \#560 Posted by: amazingdave Posted at: 2018-12-12T21:03:55.297Z Reads: 209

```
That is not the same fluctuations that I have seen on the 6.6. 

It may not be your battery sagging but the fact that the voltage drops whenever the current rises suggests that their must be some resistance in the supply...
```

---
## \#561 Posted by: Gdunn416 Posted at: 2018-12-16T22:00:44.453Z Reads: 208

```
Is it possible to export the Metr app logs so that I can keep the odometer and top speed, etc., when I use a new device?
```

---
## \#562 Posted by: hexakopter Posted at: 2018-12-16T23:25:34.825Z Reads: 212

```
Are you using Android or iOS?

For iOS you can connect to iTunes and save all .s and .r record files from the metr app and import them afterwards for your new device. I think a iTunes device backup should also work to save all data. When the backup is not working its always good to have screenshots from all your stats and settings so you could change them on the device later manually.
For Android you can get the record files inside the metr app folder on the SD card or where you have installed it.
```

---
## \#563 Posted by: Friskies Posted at: 2018-12-22T13:03:51.939Z Reads: 217

```
Anybody else having problems with the metr pro working with the latest unity firmware? FW: 23.41

It won't send any info at all :(
```

---
## \#564 Posted by: dspx Posted at: 2018-12-22T13:19:21.758Z Reads: 211

```
Methinks it's still being developed for Unity
https://www.electric-skateboard.builders/t/focbox-unity-official/64944/1534?u=dspx
```

---
## \#565 Posted by: rpasichnyk Posted at: 2018-12-22T16:07:34.192Z Reads: 214

```
Working on it right now!

![computer-lego-notebook-3oz8xyg7F0uoJ5XxDO|690x388, 50%](upload://tpPGf6eTwT2U29rdirbtvEoKhuH.gif)
```

---
## \#566 Posted by: DavidC Posted at: 2018-12-24T09:40:01.225Z Reads: 210

```
@[rpasichnyk](/u/rpasichnyk) Regarding METR on Apple iOS : how to send data to an android smartwatch using Wear OS (ex Android Wear)?

I saw there was is an option in Miscellaneous but for Apple Watch.
```

---
## \#567 Posted by: murloc992 Posted at: 2018-12-24T09:40:06.505Z Reads: 210

```
Do we need to replace the original Unity module for Metr module? If not, then this is the best thing since sliced bread. :smiley:
```

---
## \#568 Posted by: StefanMe Posted at: 2018-12-24T09:41:11.850Z Reads: 202

```
I hope we can replace the original bl module... I want to use the free UART port for something else.
```

---
## \#569 Posted by: murloc992 Posted at: 2018-12-24T09:51:44.412Z Reads: 201

```
I hope @rpasichnyk just gonna add Unity module support. I want to keep my Unity as is. :smiley:
```

---
## \#570 Posted by: StefanMe Posted at: 2018-12-24T10:27:46.286Z Reads: 207

```
That would be awesome... but difficult with the payment. Now everyone paid for the expensive module and have to buy an extra app. 

I mean it would be super nice to use the original Modul, but I don’t believe it
```

---
## \#571 Posted by: Bjork3n Posted at: 2018-12-24T10:53:31.849Z Reads: 206

```
Guys if i want to be able to change settings on the focboxes with the pc without removing the enclosure do I need a bluetooth usb/card on my pc? 
Tcp bridge for example, does it require a bluetooth connection on the pc?
```

---
## \#572 Posted by: bevilacqua Posted at: 2018-12-24T11:20:49.908Z Reads: 213

```
no, just a wifi/ethernet connection, no BT.

You need a BT adapter/card IF you want to connect directly via Bluetooth to the vesc tool. This works with the Linux and Mac tool (the one modded by Roman). But if you got a metr pro I would stick to TCP, now its hella fast.

Alternatively you could change settings just via the Metr App on the "expert" section

![image|600x327](upload://cLJqpIBpfnU45s8FodWRrCpPYl.jpeg)
```

---
## \#573 Posted by: Bjork3n Posted at: 2018-12-24T11:57:11.290Z Reads: 210

```
Thanks for your reply! 
That's awesome! Will try once I get the module :)
```

---
## \#574 Posted by: StefanMe Posted at: 2018-12-24T23:24:23.975Z Reads: 209

```
Can u give us a small hint how u ll integrate the METR again? By using the UART port or are u able to use the original BL model from Enertion?
```

---
## \#575 Posted by: Jc06505n Posted at: 2018-12-24T23:56:18.708Z Reads: 215

```
Business wise, it wouldn’t make sense for him to make the BT on the unities work on METR. Espeically when 

A) The primary income for METR is from the sales of the modules

B) Enertion will not pay him for every unity Metrized

C) The Unity will become the primary dual VESC for the foreseeable future 

More than likely, and business wise, he would either have to make METR a paid app (which would be a loss in income compared to the module) or keep on the current module and jsut update the METR mods to work with the way the unity flirts with UART. This is all speculation of course, but anyone could see why it wouldn’t make sense for the unity to be meterized without some form of compensation to subsidized the app.
```

---
## \#576 Posted by: SeanHacker Posted at: 2018-12-25T00:39:14.307Z Reads: 210

```
[quote="Jc06505n, post:575, topic:57780"]
C) The Unity will become the primary dual VESC for the foreseeable future
[/quote]

I really doubt this. 2019 is upon us dude. 

*popcorn is being eaten right now* just be patient and watch before the pitchforks come out. ;)
```

---
## \#577 Posted by: Sn4pz Posted at: 2018-12-25T00:42:09.788Z Reads: 199

```
Do you have any information that proves otherwise ? Lmfao
```

---
## \#578 Posted by: SeanHacker Posted at: 2018-12-25T00:44:38.307Z Reads: 198

```
Ugh... The future dude. Tell me a year that went by when electronics didn't evolve. Not rocket science here.
```

---
## \#579 Posted by: StefanMe Posted at: 2018-12-25T00:46:19.733Z Reads: 201

```
I don't see why the paid app is a loss in income... no extra hardware cost, no repairs of module... just super quick payment by in app purchase. Selling a software (app) is so much easier than dealing with hardware. 

I mean for 98% of the people its totally fine to use the UART port. Its just one guys like me, who want to use two UART ports.
```

---
## \#580 Posted by: Sn4pz Posted at: 2018-12-25T00:55:56.083Z Reads: 198

```
Cool argument, keep fluffing your feathers in the name of *the future* 

Sometimes products are created and they stick in their environment, of course it's going to have competition via the Chinese and their insatiable hunger to clone things, but it's just silly to say that " because x exists, y will exist and sweep it away"
```

---
## \#581 Posted by: SeanHacker Posted at: 2018-12-25T01:15:38.772Z Reads: 199

```
This is silly. Good luck with that though. Just remember the days when @onloop was dissing hub motors and then the next year is making them. I'm going to stay with the forward thinking people and let those like yourself stay with the past. Considering the past in esk8 so far, I'd bet on the future. ;)
```

---
## \#582 Posted by: Sn4pz Posted at: 2018-12-25T01:17:19.213Z Reads: 196

```
Sure thing :+1:
```

---
## \#583 Posted by: jadatmag Posted at: 2018-12-25T01:51:41.740Z Reads: 196

```
How long has the focbox been the top dog?
```

---
## \#584 Posted by: SeanHacker Posted at: 2018-12-25T02:00:57.148Z Reads: 205

```
Does this have something to do with the electronics evolution? Because that's just an opinion as far as facts go. This is just another Apple and Android conversation for you dude.
```

---
## \#585 Posted by: Jc06505n Posted at: 2018-12-25T02:08:57.470Z Reads: 218

```
[quote="SeanHacker, post:576, topic:57780"]
I really doubt this. 2019 is upon us dude.
[/quote]

Hmmm I don’t know my dudes. 2018 saw a series of new ESC’s and even then the Focbox has stood on top because: 

* Trampa is Expensive
* Stewie’ is mia for the time being making the escapes and escape support severely limited
* Flipsky are for the cost you get them
* Maytech are Maytech 
* Focboxes work and have proven time and time again that they do. 

Now that they’re gone and more people will want to run an efficient system , so long as the unity’s switch system works with no problems , there’s very little that makes it not the optimal choice. 

[quote="StefanMe, post:579, topic:57780"]
I don’t see why the paid app is a loss in income… no extra hardware cost, no repairs of module… just super quick payment by in app purchase.
[/quote]

It’s not just the cost of hardware that goes into metr but the software  the support to catch and squash bugs, to help configurations and keep up with the latest release... a one time 4.99 a pop ain’t ganna cut it
```

---
## \#586 Posted by: jadatmag Posted at: 2018-12-25T02:35:37.681Z Reads: 215

```
[quote="SeanHacker, post:576, topic:57780"]
I really doubt this. 2019 is upon us dude.

*popcorn is being eaten right now*
[/quote]

That in combination with 

[quote="SeanHacker, post:581, topic:57780"]
This is silly. Good luck with that though. Just remember the days when @onloop was dissing hub motors and then the next year is making them. I’m going to stay with the forward thinking people and let those like yourself stay with the past. **Considering the past in esk8** so far,
[/quote]

and

[quote="SeanHacker, post:578, topic:57780, full:true"]
Ugh… The future dude. Tell me a year that went by when electronics didn’t evolve. Not rocket science here.
[/quote]

and

[quote="SeanHacker, post:581, topic:57780"]
I’m going to stay with the forward thinking people and let those like yourself stay with the past.
[/quote]

Made me wanne ask what the last years top vesc was. As it's just a simple question and you're kinda unnecessarily dissing someone in a demeaning way who has the side of history on his side. As this market is very small I wouldn't be to sure about "the electronics evolution" because only small vendors do the research and development at this moment.

Anyway. The Unity not having two uart ports makes me kinda sad. (Edit: it has 3 lololoool Edit agian: no it doesn't) I think the target audience for Metr Pro contains a lot of people who also want a remote with telemetry over uart, me included. I just ordered a Metr Pro and have a Unity on the bench. So I'm interested in what rpasichnyk will or won't do if the Unity really will be the top dog for the foreseeable future.
```

---
## \#587 Posted by: SeanHacker Posted at: 2018-12-25T03:09:14.643Z Reads: 207

```
What you're missing is that Enertion prior to the Unity has been taking others design's long before they found  @Deodand and the Unity. Not to mention, steals open source code without providing it back as legally required. @Blasto just made the design better. I can vouch for his work because I've been running two vesc-x's for two years that he personally fixed for me. I blew two FOCBoxes in a week the first time I ran them. Not to mention all the others with QC issues. I'm not dissing anyone. I'm stating the facts. This is a evolution. And whether Enertion takes the reigns , there will be evolution regardless.

If what I'm saying is wrong in 2019. I'll actually cut off my nipples and my fiancés in place of @brenternet's.
```

---
## \#588 Posted by: Deodand Posted at: 2018-12-25T03:21:35.576Z Reads: 209

```
Someone contact Sean's fiance and let her know he offered up her nipples on the esk8 altar before they were even married. Risky move.
```

---
## \#589 Posted by: SeanHacker Posted at: 2018-12-25T03:23:58.764Z Reads: 216

```
Done... ;)

![IMG_20181224_192259|375x500](upload://wS8zz25KW7IR04PO4rSrrTTmKz6.jpeg)
```

---
## \#590 Posted by: Deodand Posted at: 2018-12-25T03:26:17.585Z Reads: 209

```
Wish there was a mega heart button haha
```

---
## \#591 Posted by: SeanHacker Posted at: 2018-12-25T03:27:41.615Z Reads: 212

```
Just so you know dude. I love you. I'm really glad your on the Enertion team. You've done things that they didn't do in a year of begging them to. Open source. For real!

Edit- Duh. And the Unity. Which is amazing. That goes without saying.
```

---
## \#592 Posted by: Blasto Posted at: 2018-12-25T03:36:38.945Z Reads: 206

```
Unity has 3 uart port, ima go steal some code now
```

---
## \#593 Posted by: rpasichnyk Posted at: 2018-12-25T08:58:55.369Z Reads: 211

```
Support for UNITY stock BLE module is not planned at the moment. We discussed this option with Enertion and I am happy we tried. Unfortunately timeframes and resources were constrained and we couldn't come up with an agreement.

What we are working on with @hexakopter is adapting Metr Pro firmware and Metr App to the changes in UNITY code and making sure it all works well. We also have another project in the works, a smaller Metr Pro variant that can be fitted inside UNITY and replace the stock module.
```

---
## \#594 Posted by: Sn4pz Posted at: 2018-12-25T09:01:38.832Z Reads: 207

```
[quote="rpasichnyk, post:593, topic:57780"]
smaller Metr Pro variant that can be fitted inside UNITY and replace the stock module.
[/quote]

!!! Exciting! This is great to hear! Can't wait to pick one up :)
```

---
## \#595 Posted by: StefanMe Posted at: 2018-12-25T10:16:33.281Z Reads: 208

```
THIS is awesome. Great to hear that.

Thanks for the spoiler!
```

---
## \#596 Posted by: Friskies Posted at: 2018-12-25T10:28:18.295Z Reads: 210

```
How long till you will have the current units up and running with the unity? I have one board desperately waiting for you :frowning:
```

---
## \#597 Posted by: rpasichnyk Posted at: 2018-12-25T10:54:11.183Z Reads: 214

```
Soon™️

![IMG_3901|230x500](upload://fTLnQ7WVmZJNAfhUN8IiSUuGilF.jpeg)
```

---
## \#598 Posted by: BigBrit Posted at: 2018-12-25T11:08:18.157Z Reads: 209

```
Such a wise move....

If Enertion can't agree a deal you just make a replacement that any DIYer can change out.  Bravo
```

---
## \#599 Posted by: jadatmag Posted at: 2018-12-27T03:20:59.981Z Reads: 212

```
Where Can I find the other another spot to connect Metr pro. I installed the unity today.

The code stealing was sarcasm, was the other part also sarcasm? Did I use the term uart wrong? In drone boards it's actually quite common.
```

---
## \#601 Posted by: Blasto Posted at: 2018-12-27T03:27:10.742Z Reads: 211

```
There’s 2 ports that are not really accessible, under the cover on the 2X7 connector.
```

---
## \#602 Posted by: FredXanadu Posted at: 2018-12-27T21:09:38.767Z Reads: 216

```
Same boat... i'm looking to find a solution to plug my photon receiver and the metr module on my unity. Please help :slight_smile:
```

---
## \#603 Posted by: jadatmag Posted at: 2018-12-27T21:30:03.299Z Reads: 221

```
![image|281x500](upload://jMtF3TFiLj3chqzySElqpvIVF7g.jpeg) 
Picture by @pjotr47 

It won't be click-in and power on... I think this will require fine soldering.

@rpasichnyk
You have an estimated timeline for the custom smaller module? I might want to change my order for that new module. Soldering that would be much easier then wires. transac nr: 0XH86601T4183640N

Can we just stick in [those pointy wires](https://www.aliexpress.com/item/dupont-cable-jumper-wire-dupont-line-male-to-male-male-to-female-female-to-female-dupont/32854114982.html?spm=2114.search0104.3.66.1d193bc9uXWkDP&ws_ab_test=searchweb0_0,searchweb201602_2_10065_10068_319_5729915_317_10696_453_10084_454_10083_10618_10304_10307_10820_10301_10821_538_5730815_537_536_10843_10059_10884_10887_100031_321_322_10103,searchweb201603_51,ppcSwitch_0&algo_expid=c9f7fedc-8ea1-4050-8579-17a854b44ed9-9&algo_pvid=c9f7fedc-8ea1-4050-8579-17a854b44ed9) in the 2x7 connector? Not enough space though in most casings. It will be fiddly if you're not used to it.
```

---
## \#604 Posted by: hexakopter Posted at: 2018-12-28T09:54:05.256Z Reads: 218

```
[quote="jadatmag, post:603, topic:57780"]
You have an estimated timeline for the custom smaller module?
[/quote]


Don't expect it in the next weeks. It will take some time to test, program and source parts. I am in contact with @Deodand about getting a damaged Unity from the final production batch to see if the new smaller Metr Pro module would fit and work. 
Right now we don't have a final production Unity to test the module and there are also other factors that could delay ETA. We will let you know when we could estimate a date.

@jadatmag Your module would be shipped today, but we can also hold it. Please let us know ASAP if you want to cancel the order.
Its not a clean and nice option, but when you cut a hole in the orange silicone case of the Unity and build an adapter cable it could actually work. But I wouldn't recommend that "dirty hack" and see problems with loose connections.
```

---
## \#605 Posted by: jadatmag Posted at: 2018-12-28T11:55:22.065Z Reads: 214

```
Please hold it off for me.

Can I be be the first one to receive the special module? :heart_eyes:
```

---
## \#606 Posted by: hexakopter Posted at: 2018-12-28T17:29:35.840Z Reads: 219

```
I put you on the list that you want to buy one.
```

---
## \#607 Posted by: Eretron Posted at: 2018-12-30T17:10:42.594Z Reads: 218

```
![image|666x500](upload://p34L1Csc3iLaxB8McZ2VKWbo0dq.jpeg) 

Any thoughts on what's the best way to reattach antenna to the pcb?
```

---
## \#608 Posted by: bevilacqua Posted at: 2018-12-30T17:54:50.064Z Reads: 213

```
Buy a new one, plug n play.

I think there are links in this thread. The antennas should be the same as wifi router ones
```

---
## \#609 Posted by: StefanMe Posted at: 2018-12-30T18:35:32.592Z Reads: 217

```
U have to resolder the 0402 capacitor next to the antenna plug into the other direction to "activate" the PCB Antenna

0804 is for beginners
0603 is for intermediate
0402 is for ABSOLUTE PROS with microscope :rofl:

(its the SMD size of the components in 0.1mm)
```

---
## \#610 Posted by: rpasichnyk Posted at: 2018-12-31T09:10:59.491Z Reads: 214

```
- Get a new U.FL to SMA adapter (something like [this](https://www.banggood.com/U_FL-IPEX-IPX-to-SMA-RP-SMA-Female-Connector-Antenna-Cable-Adapter-p-1258127.html?utm_source=google&utm_medium=cpc_ods&utm_content=ysq&utm_campaign=RC-Sds-Feed&gclid=Cj0KCQiAmafhBRDUARIsACOKERMCyQPp4wyPbs-ASShTg8k7vs7JK1CnvbUbdhGB8dvDlsfobveiB38aAsmzEALw_wcB&ID=511528&cur_warehouse=CN))
- Cut the heat shrink and remove it, unplug broken adapter
- Plug the new adapter
- Wrap with a new heat shrink
```

---
## \#611 Posted by: Bjork3n Posted at: 2019-01-04T17:04:38.966Z Reads: 214

```
Just tried connect via tcp , works like a charm! 
Im so glad that i never have to remove my enclousure again to fix with the settings with vesc tool!
Amazing, just amazing! ::D
```

---
## \#612 Posted by: Eboosted Posted at: 2019-01-05T23:35:34.413Z Reads: 210

```
After years of hearing about this awesome module, I went ahead and purchase 2 for my builds.

Hope you guys could help me figuring out how to connect pair the module.

I tried to pair using PIN 0000 and 1234 but neither worked, if there a default  PIN I should use?
```

---
## \#613 Posted by: bevilacqua Posted at: 2019-01-05T23:36:21.437Z Reads: 204

```
There should be a sticker on every module
```

---
## \#614 Posted by: Eboosted Posted at: 2019-01-05T23:36:57.100Z Reads: 207

```
[quote="bevilacqua, post:613, topic:57780, full:true"]
There should be a sticker on every module
[/quote]

Damn, I'll have to crack open the enclosure. Thanks man!

Update: I was able to connect perfectly. Thanks for the input
```

---
## \#615 Posted by: Trdolan03 Posted at: 2019-01-08T04:58:24.821Z Reads: 204

```
I'm having an issue with my module> I try to connect via TCP and all 3 lights come on and are solid. The module then disconnects. I don't get any error or fault notifications though.
```

---
## \#616 Posted by: amazingdave Posted at: 2019-01-08T08:48:30.970Z Reads: 202

```
Is there any chance of having the VESC report demanded throttle to the app?
```

---
## \#617 Posted by: Jc06505n Posted at: 2019-01-09T21:44:00.675Z Reads: 201

```
Did the update that supported the unity but I still don't get telemetry.
```

---
## \#618 Posted by: Indiangummy Posted at: 2019-01-09T22:03:51.526Z Reads: 198

```
I think he's still working on it. I thank that update was for the phone app itself
```

---
## \#619 Posted by: sofu Posted at: 2019-01-09T22:15:11.726Z Reads: 198

```
I get telemetry on the unity... Make sure you have your baud rates and uart settings correct
```

---
## \#620 Posted by: Jc06505n Posted at: 2019-01-09T22:16:43.273Z Reads: 202

```
Ahhh I didn’t think of the baud rate , let me try that out now
```

---
## \#621 Posted by: Indiangummy Posted at: 2019-01-09T22:18:49.238Z Reads: 195

```
Idk even know what that is. I'll have to check again.
```

---
## \#622 Posted by: Indiangummy Posted at: 2019-01-09T22:19:55.301Z Reads: 199

```
Where is this setting? I can't find it
```

---
## \#623 Posted by: Jc06505n Posted at: 2019-01-09T22:20:15.859Z Reads: 199

```
Under UART tab in the Focbox tool

Changed baudrate to 9600 bps and I’m getting telemetry thanks @sofu @rpasichnyk
```

---
## \#624 Posted by: Indiangummy Posted at: 2019-01-09T22:43:03.931Z Reads: 207

```
Alright will try when I get home.
```

---
## \#625 Posted by: rpasichnyk Posted at: 2019-01-10T16:16:29.974Z Reads: 210

```
UNITY support is now live :slight_smile: We pushed it about a week ago!

https://giphy.com/gifs/snl-saturday-night-live-season-44-1zlnnuisxIwwaYsYGa
```

---
## \#626 Posted by: DAddYE Posted at: 2019-01-11T05:09:13.979Z Reads: 209

```
Is it possible to automatically start the app and record a session when I turn on my board?
```

---
## \#627 Posted by: Indiangummy Posted at: 2019-01-11T05:10:41.384Z Reads: 204

```
there is an option which you can enable to automatically start and record sessions based on speed.
```

---
## \#628 Posted by: DAddYE Posted at: 2019-01-11T13:27:49.392Z Reads: 205

```
But the app have to be open
```

---
## \#629 Posted by: rene Posted at: 2019-01-11T13:31:19.143Z Reads: 203

```
Sure has the App to be open and connected - how otherwise should it work?
```

---
## \#630 Posted by: DAddYE Posted at: 2019-01-11T13:38:55.762Z Reads: 197

```
Usually Bluetooth can “wake up” the phone and its  apps
```

---
## \#631 Posted by: rpasichnyk Posted at: 2019-01-11T13:40:29.705Z Reads: 202

```
You can have Metr app running in background. OS would freeze it, so it will consume no (or very little) resources. When you turn on your board, it will indeed "wake up" the app and everything should work just fine. Have you tried?
```

---
## \#632 Posted by: DAddYE Posted at: 2019-01-11T13:41:46.809Z Reads: 200

```
Yes, but doesn’t record. Should I keep location services always on on the app?
```

---
## \#633 Posted by: rpasichnyk Posted at: 2019-01-11T13:43:55.220Z Reads: 202

```
Do you have this option enabled?

![Untitled|316x470](upload://mesWbtj5HK4jDkXWEH7qAcnOQpN.png)
```

---
## \#634 Posted by: DAddYE Posted at: 2019-01-11T13:44:20.965Z Reads: 189

```
Yes sir! 10c
```

---
## \#635 Posted by: rpasichnyk Posted at: 2019-01-11T13:47:10.995Z Reads: 196

```
"Location services always on" is not required for this to work.. can you make a short test? Start the app, move it to background, start your board and press throttle, after 10 seconds the record should start. If you have Notifications enabled, your phone will also vibrate and show notification. If this is not happening, Settings -> Show Logs -> send to support@metr.at
```

---
## \#636 Posted by: DAddYE Posted at: 2019-01-11T13:47:44.898Z Reads: 196

```
Sure I will! Thanks mate
```

---
## \#637 Posted by: hiboute Posted at: 2019-01-11T14:25:40.749Z Reads: 194

```
I have the same issue. If i open the app in the morning. It will record my ride in the next hour. But if i ride a few hours later, it is like the app is closed. I have to reopen it.

Log: https://www.dropbox.com/s/pt4mx0906dr1nhm/log_2019-01-11.txt?dl=0

(I did a ride at 9am,  12h10pm, and 13h15)
```

---
## \#638 Posted by: amazingdave Posted at: 2019-01-11T14:26:46.499Z Reads: 196

```
Same goes for me.
```

---
## \#639 Posted by: rpasichnyk Posted at: 2019-01-14T14:22:33.146Z Reads: 196

```
@hiboute thanks for the log file! I just released v3.4.15 which should fix the issue. Metr Pro should wake up the app, when powered back on even after several hours. Don't force close Metr app, let it sit in the background. @DAddYE @amazingdave you have iOS too?
```

---
## \#640 Posted by: Pedrodemio Posted at: 2019-01-14T14:35:17.005Z Reads: 195

```
Mine always worked as long you connected the board with the app open once and then shut it down and leave the app on the background

If you open the app without connecting to the board and disconnecting it won’t start a record
```

---
## \#641 Posted by: DAddYE Posted at: 2019-01-14T15:49:28.791Z Reads: 196

```
Yes! 10 chars
```

---
## \#642 Posted by: amazingdave Posted at: 2019-01-14T18:40:05.281Z Reads: 193

```
Yes...
10 c
```

---
## \#643 Posted by: hiboute Posted at: 2019-01-14T18:40:43.612Z Reads: 199

```
It’s working! Thank you very much
```

---
## \#644 Posted by: mccloed Posted at: 2019-01-14T19:48:20.875Z Reads: 198

```
Should this work on the newest firmware for the Unity?
```

---
## \#645 Posted by: Jc06505n Posted at: 2019-01-14T20:04:34.555Z Reads: 207

```
https://www.electric-skateboard.builders/t/metr-pro-next-gen-bluetooth-module/57780/625?u=jc06505n
```

---
## \#646 Posted by: mccloed Posted at: 2019-01-14T23:44:58.216Z Reads: 212

```
Saw that. Problem is it works on the Beta with the older firmware but not on the new one with the new firmware. I'll double check my settings, I guess.
```

---
## \#647 Posted by: Indiangummy Posted at: 2019-01-14T23:54:32.451Z Reads: 214

```
I'm running it on the latest unity firmware just fine. or are you referring to the metr FW?
```

---
## \#648 Posted by: mccloed Posted at: 2019-01-15T00:10:48.405Z Reads: 219

```
No. I have updated the Metr app to the latest version. Haven't messed with the Metr firmware. Not sure I'd know how. :thinking:
```

---
## \#649 Posted by: rpasichnyk Posted at: 2019-01-15T04:39:57.921Z Reads: 224

```
@mccloed You go to Settings and click on the Blue gear :+1:

![ota|320x426](upload://rfnxb5rlMiS4T2EI3A6CarkAzgz.gif)
```

---
## \#650 Posted by: mccloed Posted at: 2019-01-15T15:08:20.576Z Reads: 221

```
Just that easy!:laughing: I'll try tonight. Thank you!
```

---
## \#651 Posted by: mccloed Posted at: 2019-01-17T15:24:04.024Z Reads: 227

```
Of course it worked! Thank you @rpasichnyk!
```

---
## \#652 Posted by: sofu Posted at: 2019-01-21T02:37:18.885Z Reads: 234

```
Is it possible to unplug the unity's integrated bluetooth and use the pins from that instead for the metr?

Edit: I went ahead and did it. Everything works,  firmware change required...

![image|666x500](upload://ts31ObXI8U6OITT2omyO4XbYfpP.jpeg)
```

---
## \#653 Posted by: Sn4pz Posted at: 2019-01-21T12:25:44.742Z Reads: 245

```
This is great to know, thank you!

I've been scratching my head as to how I can get a davega, metr, and feather style remote all functioning at the same time... This might be it 😁
```

---
## \#654 Posted by: sofu Posted at: 2019-01-21T20:42:47.574Z Reads: 247

```
If you want to get all three functioning at the same time, note that there are actually three tx/rx pairs in total. Looking at the esc landscape from the uart port, there's of course the "external" one, then counting from the top left on the "internal" header, pin 7/14 are rx/tx, 10/11 are rx/tx. So really the Unity includes one more uart port than a regular dual vesc which in my book makes an already leaps and bounds beyond esc even better 🤣 The internal pins are bound to 250k baud right now though, so you'll have to either ask @Deodand or wait for an updated tool where you can change the baud values of those
```

---
## \#655 Posted by: Sn4pz Posted at: 2019-01-21T22:16:42.703Z Reads: 251

```
Thank you thank you thank you!!! Great into 

@Deodand oh Mr. Dedoandddd 

please enable this for those of us who love to fiddle with bluetooth devices o3o
```

---
## \#656 Posted by: mishrasubhransu Posted at: 2019-01-22T12:59:55.285Z Reads: 237

```
@rpasichnyk, If I get the pcb version can I put the antenna later(in case I have connection problems)? I have a bunch of those antennas lying around.
```

---
## \#657 Posted by: hexakopter Posted at: 2019-01-22T17:09:52.906Z Reads: 237

```
Yes, that is possible with some soldering and an appropriate antenna cable. You can find the answer in the [FAQ.](https://metr.at/faq#q33)

_Yes, it is possible but requires some good soldering skills. You need to resolder the 0402 capacitor near the u.FL connector in a different position to change between internal PCB antenna and external antenna._
```

---
## \#658 Posted by: flyingox Posted at: 2019-01-24T19:14:17.923Z Reads: 230

```
Hope someone can help.  

Discovered this issue the other day when I was a long way from home and without a laptop resulting in a long walk back.

I configured vesc 0 using vesc_tool_0.95(linux) with via USB then vesc 1 same method and all works fine.  Side note, Bluetooth connection is discovered but doesn't work on Ubuntu8.04. 

Then out on the road decided to change mode connecting via  mobile Metr Pro.  Applied a different mode then immediately after vesc1 no longer responded.  I tried to recover using the expert settings, read the existing setting, change option to enable vesc1, wrote the change then found I was unable to use the remote control. 

When I got home I hooked up the laptop with vesc_tool to find the application and motor was all wrong.   Why would the mode change cause this issue?
    

metr pro version 3.4.14 firmware 3.65 Android 7.1.1 
Dual Vesc6 3.40 
hardware 60

Also I'm unable to connect using ESC monitor.  The app finds the connection, able to enter the security key but after that no data is shown.  Actually never been able to get this app to work with the metr module, tried several installs no luck, perhaps the app is no longer supported?
```

---
## \#659 Posted by: goldrabe Posted at: 2019-01-24T21:57:21.545Z Reads: 214

```
Did you read your settings before creating new modes?
If you don't read your settings before creating modes default values for motor detection etc. will be applied which will mess up your settings.
As for the ESC monitor app, I can not comment, haven't used it yet.
```

---
## \#660 Posted by: rpasichnyk Posted at: 2019-01-25T14:52:58.532Z Reads: 217

```
Sorry for this. Actually happened to me once as well, had to push about 2km back home, it sucked! I don't know the reason, but it never saw it again, it feels like the stars have to align for it to happen. I was never able to reproduce this issue. If you can, this will be great. Find the reliable way to recreate the problem and send logs!

About ESC monitor app. When we released Metr Pro, it was working. Then after some time it stopped. I don't know the reason and I tried to reach the developer for help, but got no reply. Unfortunately there is little we can do. You can try using the older apk, which should work.
```

---
## \#661 Posted by: sayekim Posted at: 2019-01-25T15:20:13.568Z Reads: 215

```
I think I nailed this issue a little over a month ago. 

https://www.electric-skateboard.builders/t/metr-pro-next-gen-bluetooth-module/57780/549?u=sayekim

I am running 3.38 now but not for this reason. Haven’t tried the start up mode with this firmware.
```

---
## \#662 Posted by: angeljmm Posted at: 2019-01-27T14:56:56.248Z Reads: 210

```
hi,
just finished a build with unity today (at least on the test bench, because still waiting for the board ;-)).
1) connected the metr.pro module without difficulty.
2) entered the pin code without problem
3) enterd all motor and config parameter without problem
4) tryed to update the module  (i'm using unity... so necessary!) with the blue icon
it says my firmware is 3.63 and that 3.65 ( unity 23.41 supporting, witch is my case) is avalaible
i click upgrade and...
start to download for 1 sec then

**Erreur SHA-256 mismatch.**

Any idea?
(blue led is ligthing and green blinking on the module)
```

---
## \#663 Posted by: angeljmm Posted at: 2019-01-27T15:38:13.164Z Reads: 203

```
And tryed the update one my other board equipped with metr.pro. 
(but with no working problem because not with unity!)
same issue using a iphone6

same error message. (but not same firmware)
**Erreur SHA-256 mismatch.**
```

---
## \#664 Posted by: rpasichnyk Posted at: 2019-01-28T07:05:32.610Z Reads: 203

```
Thank you for heads up. There was a problem with update server, this is now fixed! Please try again :slight_smile:
```

---
## \#665 Posted by: angeljmm Posted at: 2019-01-28T13:00:22.780Z Reads: 205

```
perfect and easy! update works fine now
```

---
## \#666 Posted by: Arzamenable Posted at: 2019-01-29T05:17:16.122Z Reads: 210

```
I’d just like to raise my hand and say I’m all for update that can read out 4 esc values.  I don’t think I can go back to 2wd. 🙋‍♂️

I run two unity’s with their own two receivers to a single Gt2b transmitter. I have two metr pros. I could be convinced to use canbus if that were needed, but I wouldn’t like it. 😬

Edit: I know, #firstworldesk8problems. Thanks for awesome hardware and software!
```

---
## \#667 Posted by: rpasichnyk Posted at: 2019-01-29T09:46:32.075Z Reads: 209

```
4wd support and dual UNITY is actually one of the things I am working on right now. Next week I will hopefully meet with @mackann at [Bioboards](https://www.bioboards.se/en/home/) workshop and we will fix things and go through the app and check that everything works smoothly👌
```

---
## \#668 Posted by: rene Posted at: 2019-01-31T18:37:05.145Z Reads: 217

```
I was just trying to set my both VESC 6 v3.40 to 140A motor amps - but it seems the max you allow me is 120A - total motor max is set to 150A.
```

---
## \#669 Posted by: pjotr47 Posted at: 2019-01-31T21:17:16.288Z Reads: 217

```
I have the old metr laying at home. Will this works with the unity?
```

---
## \#670 Posted by: kalebludlow Posted at: 2019-01-31T22:30:59.151Z Reads: 212

```
@rpasichnyk just to confirm, the Metr Pro works with Android Pie right?
```

---
## \#671 Posted by: Surfer Posted at: 2019-01-31T22:54:44.550Z Reads: 216

```
If you want to get the pro version, I don't mind to buy yours in the next group ride :)
```

---
## \#672 Posted by: sofu Posted at: 2019-02-01T08:56:21.591Z Reads: 219

```
Posting here for posterity, but for people wanting to use Metr + some other uart based peripheral, here's the link to the firmware file with internal ports running at 115200. This also has the low speed braking fix.

https://drive.google.com/file/d/1Ng-Gk0CU3XOB-D-ocXVkNCycbUTCykwM/view

Here's the pinout

![image|690x200](upload://xAv3R5dE3hGz15NaeyPIX05moec.png) 

This specific firmware is supposed to have UART2 enabled at 115200. I'm unsure if UART1 is running at 115200, it may still be at 9600.
```

---
## \#673 Posted by: Sn4pz Posted at: 2019-02-01T10:18:51.184Z Reads: 214

```
Saved! Damn thanks a bunch. All these knowledge little crumbs youre laying around are starting to come together in my head 😂😂
```

---
## \#674 Posted by: pjotr47 Posted at: 2019-02-01T11:32:58.631Z Reads: 209

```
Haha, i have also some boards running with focbox. So I can still use that in my other boards
```

---
## \#675 Posted by: PickSix24 Posted at: 2019-02-02T19:39:25.516Z Reads: 206

```
Can anyone help me with getting telemetry with a unity. I have the baudrate set to 9600 in the unity tool. I also made sure the metr was running the latest vertion. Metr shows as being connected but not seeing telemetry. 
Thanks !
```

---
## \#676 Posted by: mccloed Posted at: 2019-02-02T21:08:17.937Z Reads: 206

```
Change the baud rate to 115200 and it should work, I believe.
```

---
## \#677 Posted by: PickSix24 Posted at: 2019-02-03T21:17:05.547Z Reads: 201

```
Tried that, still not working. My green led is flashing so looks like it’s a baudrate issue. 
Anyone know what it should be set to ?
Any other settings that need to checked ?
```

---
## \#678 Posted by: Jc06505n Posted at: 2019-02-03T22:34:40.716Z Reads: 199

```
[quote="rpasichnyk, post:593, topic:57780"]
We also have another project in the works, a smaller Metr Pro variant that can be fitted inside UNITY and replace the stock module.
[/quote]

Thanks to @sofu’s build thread including 2 additional UART Ports I am pumped for this. If you can use the same pins (I Think their female , which ever one goes in) then it really is an easy swap on swap out.
```

---
## \#679 Posted by: Pantata Posted at: 2019-02-03T22:52:06.682Z Reads: 193

```
Can you please tell me what kind of a port it is for the external antenna? I got the module without it and wanna get one, though don't know what connector to look for at the end.
```

---
## \#680 Posted by: pookybear Posted at: 2019-02-04T00:52:08.140Z Reads: 189

```
Where do I sign up for this?
```

---
## \#681 Posted by: Jc06505n Posted at: 2019-02-04T01:16:40.802Z Reads: 189

```
You wait until he releases it
```

---
## \#682 Posted by: pookybear Posted at: 2019-02-04T01:26:52.997Z Reads: 194

```
I know. I was just showing my excitement about it. :wink::scream:
```

---
## \#683 Posted by: PickSix24 Posted at: 2019-02-05T00:52:35.676Z Reads: 206

```
Finally got my unity connected. I’ve got it set 10s. Can anyone tell me what’s going on with the battery voltage ? 
![image|230x500](upload://lV5YUWqlCxdKyJON4vme2N5jbUH.jpeg)
```

---
## \#684 Posted by: SeanHacker Posted at: 2019-02-05T00:56:54.308Z Reads: 209

```
You're not showing voltage in this screen shot. Percentage doesn't always add up. What's the actual voltage showing? 

Add the voltage so we can see it. Like this. I have mine right below percentage. 

![Screenshot_20190204-165516_metr|281x500](upload://bXCZRct4OmdtcPr3lQgM8Bp4ETs.png)
```

---
## \#685 Posted by: PickSix24 Posted at: 2019-02-05T01:08:40.906Z Reads: 207

```
Learn something new everyday. Didn’t know I could hold down and have those options !!
How do I make it bigger like the rest ? 
![image|230x500](upload://cimMgJICzMEWGA9l7Tpv2ncqKur.jpeg)
```

---
## \#686 Posted by: caustin Posted at: 2019-02-05T01:11:42.410Z Reads: 197

```
Hold the colored frame of the box you want to adjust. Then it can be moved and sized. Lit frame to show, dim to leave out of display etc.
```

---
## \#687 Posted by: Rod12579 Posted at: 2019-02-05T01:18:53.107Z Reads: 205

```
How did finally get the unity to connect?
```

---
## \#688 Posted by: PickSix24 Posted at: 2019-02-05T01:28:37.872Z Reads: 212

```
Make sure you have your Metr updated. From there I just set the baudrate and enabled UART in the unity tool.
```

---
## \#689 Posted by: PickSix24 Posted at: 2019-02-05T01:29:56.475Z Reads: 218

```
Now if I can get it working on my Apple Watch I’ll be a happy man. Pretty sure I just need to update the watch app. It was working before with my focboxes.
```

---
## \#690 Posted by: rpasichnyk Posted at: 2019-02-08T07:37:54.150Z Reads: 223

```
Support for 4WD VESC (as well as 4WD dual UNITY) has arrived. Get the latest Metr app and update Metr Pro firmware to v3.66 @mackann @Arzamenable @evoheyax

![IMG_3218|281x499](upload://5RiotZmMUlzEKdpm61cnfubCYKn.jpeg) 

Thanks to [Bioboards](https://www.bioboards.se/en/home/) for providing a test rig!
```

---
## \#691 Posted by: pookybear Posted at: 2019-02-09T22:45:55.105Z Reads: 217

```
Has anyone trouble turning off the dev mode? I tried it and can't turn it off now. No matter what I do.![Screenshot_20190209-144320|281x500](upload://zwretHLBfBlQsdDEPMgi0munvew.jpeg)
```

---
## \#692 Posted by: PickSix24 Posted at: 2019-02-09T23:06:47.095Z Reads: 197

```
Yeah same problem, I ended up closing the app and then I was able to get out of the mode
```

---
## \#693 Posted by: pookybear Posted at: 2019-02-09T23:07:54.994Z Reads: 200

```
I tried that. Right now it's stuck.
```

---
## \#694 Posted by: Jc06505n Posted at: 2019-02-09T23:28:13.676Z Reads: 202

```
btw, seems motor detection is now available for the unity, seems like my sensors are dead somehow lucky me
```

---
## \#695 Posted by: rpasichnyk Posted at: 2019-02-10T07:22:44.074Z Reads: 202

```
@pookybear Thank you for reporting this, I found a bug and update is on the way :+1:
@Jc06505n it is available, but I didn't have time to test it, please report how it went (also send logs if something isn't working)
```

---
## \#696 Posted by: PickSix24 Posted at: 2019-02-10T07:32:14.101Z Reads: 205

```
When using a unity , what should be enabled to get data from both motors ? Right now it shows both motors but only reporting data from one
```

---
## \#697 Posted by: pookybear Posted at: 2019-02-10T07:34:16.014Z Reads: 204

```
@rpasichnyk

Thanks!
```

---
## \#698 Posted by: Jc06505n Posted at: 2019-02-11T17:31:38.599Z Reads: 204

```
[quote="rpasichnyk, post:695, topic:57780"]
@Jc06505n it is available, but I didn’t have time to test it, please report how it went (also send logs if something isn’t working)
[/quote]

Seems to have gone well, your app let me know for sure that both my sensors were dead, have to find out why, is there any setting that allows me to change motor direction like in the FOCBOX UI tool ?
```

---
## \#699 Posted by: rpasichnyk Posted at: 2019-02-11T17:55:50.291Z Reads: 197

```
Yes, open Expert, click Read, input "Invert Motor Direction" in the omnibox, change, click Write :+1: 

![11|690x337, 40%](upload://s5BPAU7T0uU2OJyFCPZ9BnQa2Li.png)
```

---
## \#700 Posted by: Bjork3n Posted at: 2019-02-11T19:37:44.800Z Reads: 209

```
I have this issue with the app that it sometimes zooms in like crazy, i need to restart the app to get it normal looking again. 
Bug or wrong setting? ![Screenshot_20190211-203420_metr|281x500](upload://liwHmCI5R2Gkkl6TC6q2C1FLnYV.jpeg) 
![Screenshot_20190211-203441_metr|281x500](upload://5GvVQHpuTYWmZ4j7a17vo20F4Eu.jpeg)
![Screenshot_20190211-203457_metr|281x500](upload://cgzgpN5g3Km4htxkV7FndS5eWDg.jpeg)
```

---
## \#701 Posted by: rpasichnyk Posted at: 2019-02-11T19:50:48.153Z Reads: 198

```
Maybe it happens when you rotate the phone? Please send logs to support@metr.at
```

---
## \#702 Posted by: Bjork3n Posted at: 2019-02-11T19:57:11.879Z Reads: 192

```
👌 file sent
Can confirm that it happens when i tilt/rotate the phone.
```

---
## \#703 Posted by: rpasichnyk Posted at: 2019-02-11T20:26:12.030Z Reads: 194

```
I tried to fix it in v3.5.6 (up any second now), but if it still annoys you, you can disable UI scaling completely in Settings -> Miscellaneous
```

---
## \#704 Posted by: Bjork3n Posted at: 2019-02-11T23:08:30.217Z Reads: 190

```
Works great now, thanks 👍
```

---
## \#705 Posted by: PickSix24 Posted at: 2019-02-12T01:30:40.249Z Reads: 187

```
@rpasichnyk is there a specific option I need to select when using a unity to get data for both motors. I’ve got both motors showing but only one displays data.
```

---
## \#706 Posted by: rpasichnyk Posted at: 2019-02-12T07:50:15.667Z Reads: 184

```
Please screenshots, logs to :arrow_right: support@metr.at
```

---
## \#707 Posted by: Pantata Posted at: 2019-02-12T19:09:59.949Z Reads: 191

```
Hi, I have the bluetooth module and all aps work except for the ackmaniac... Not sure what to do anymore. It shows the connection, it gets connected but no data is displayed and when I click on add modes it says "esc not connected" but If I click on connect it will change the icon to connected. Any help please much appreciated
```

---
## \#708 Posted by: pookybear Posted at: 2019-02-12T19:19:25.690Z Reads: 193

```
I believe it was mentioned here before that metr pro does NOT work w ackmaniac app.

I could be wrong.
```

---
## \#709 Posted by: Pantata Posted at: 2019-02-12T19:49:34.461Z Reads: 192

```
I wanted to ask here because it specifically mentions ackmaniac esc tool. But I guess that is wrong info. Ackmaniac said his app doesn't have support for PIN modules. Wanted to make sure here. Thanks for the info. You can see it shown here. https://www.electric-skateboard.builders/t/metr-pro-next-gen-bluetooth-module/57780
```

---
## \#710 Posted by: rpasichnyk Posted at: 2019-02-12T19:59:45.934Z Reads: 185

```
@Pantata PIN pairing is done on Operating System level and not in the app. I don't think this is the reason. Also please check [my post](https://www.electric-skateboard.builders/t/vesc-monitor-android-app/20888/1093?u=rpasichnyk) in VESC Monitor thread.
```

---
## \#711 Posted by: Pantata Posted at: 2019-02-12T20:01:31.411Z Reads: 183

```
I am just repeating what Ackmaniac said. I thought so too... It is paired via system so it should work. Will have a look at your post. Thank you for the answer.
```

---
## \#712 Posted by: Pantata Posted at: 2019-02-12T20:07:27.652Z Reads: 186

```
Just sucks that ackmaniac esc tool is not working and vesc tool I can't use either as I am using ackmaniac firmware and it says I need to change to a different one in order to use it. Wanted to have cool video overlay but I guess not... Only the vesc app and ackmaniac has overlay.  On the other hand METR has cool Real time data.
```

---
## \#713 Posted by: rpasichnyk Posted at: 2019-02-12T20:13:12.574Z Reads: 189

```
Have you seen METR overlay?

https://metr.at/overlay

https://www.instagram.com/p/BgW4W0jDcWx/
```

---
## \#714 Posted by: Pantata Posted at: 2019-02-12T20:31:57.063Z Reads: 187

```
Yeah, just finished making a video. Very nice app and customizable. Only amperage is missing
```

---
## \#715 Posted by: Erniechan Posted at: 2019-02-13T10:19:47.366Z Reads: 187

```
Looks awesome!
```

---
## \#717 Posted by: amazingdave Posted at: 2019-02-13T18:06:33.208Z Reads: 196

```
Hey all,  this record shows a fault on my app but I’m dammed if I can find it... any ideas?

https://metr.at/r/dbWx7

![image|547x500](upload://e0RSqRqr1tzX3ZsSCUn3wzCxjoF.jpeg)
```

---
## \#718 Posted by: Sn4pz Posted at: 2019-02-13T19:03:37.499Z Reads: 184

```
Maybe that would be a feature for @rpasichnyk to include or maybe have a toggle-able switch for?

A "flag" on the map of where the fault happened(?)
```

---
## \#719 Posted by: bevilacqua Posted at: 2019-02-13T21:16:08.428Z Reads: 184

```
It is a fault code 4, let me look what it is... 

![image|545x101](upload://jYai6NCSj0PQ9fRrMZWdo76bKf0.png)

Got it: Over current fault,
```

---
## \#720 Posted by: sayekim Posted at: 2019-02-13T21:45:18.725Z Reads: 181

```
Okay... that was cool. 

Can you also tell where/when it happened?
```

---
## \#721 Posted by: amazingdave Posted at: 2019-02-13T21:54:23.274Z Reads: 180

```
Thanks for that!
```

---
## \#722 Posted by: bevilacqua Posted at: 2019-02-13T22:01:07.604Z Reads: 182

```
min 23 // 1380192ms
10char
```

---
## \#723 Posted by: bevilacqua Posted at: 2019-02-13T23:18:19.777Z Reads: 178

```
forgot to add where:
https://www.google.com/maps/place/52%C2%B045'36.0%22N+3%C2%B015'00.7%22W/@52.7600004,-3.2677095,14z/data=!4m5!3m4!1s0x0:0x0!8m2!3d52.76!4d-3.2502

Motor current of 130 might have triggered it. Seems like it was because you tried to climb something to steep @amazingdave ?
```

---
## \#724 Posted by: amazingdave Posted at: 2019-02-14T10:21:27.815Z Reads: 195

```
@bevilacqua thanks so much for that! How are you doing this wizardry?! 

Any idea why the current would go into over current instead of just limiting? Is it anything to do with traction control as that was kicking in a lot on the mud and gravel?

It’s a flipsky dual 6.6.  Do I just need to raise my absolute max figure?

These are my settings....

![image|230x500](upload://ukzKhugooyTTSgtdeOT7P3yyfQe.jpeg)
```

---
## \#725 Posted by: bevilacqua Posted at: 2019-02-14T10:35:24.691Z Reads: 186

```
I'm not sure how this happens, but I had it once too on 4.12HW vescs when I tried to climb a way to steep ramp. Probably rising the absolute current setting helps, but I am not sure what the absolute-max-rating of the MOSFETs in in FS6.6 vescs is.

Im working on a kind of longer paper (UNI work) where I analyze e-skate telemetry.  I have some scripts to automatically read all the values in Matlab.
```

---
## \#726 Posted by: Nubasaurus Posted at: 2019-02-15T21:15:58.681Z Reads: 182

```
Just got my Metr installed. Few questions. When I go into Expert and read. Is it reading both VESC or just the can ID i have set in settings?

In theory, would I change the settings for Master, go to settings, enable CAN FWD, change ID to slave, and go back to Expert to change settings for Slave?
```

---
## \#727 Posted by: rpasichnyk Posted at: 2019-02-16T06:06:25.993Z Reads: 189

```
It is reading the VESC that is currently selected on the top of the screen. To read another VESC, just select another one and click Read

![12|319x500](upload://wJ6GI42IYOxWDntLG1wDqqi0o80.png) 

CAN FWD is almost never needed and not recommended to use at all. Unless you are absolutely sure what you are doing. All Metr functions (Modes, Expert, Realtime, etc.) work just fine without enabling CAN FWD.
```

---
## \#728 Posted by: Nubasaurus Posted at: 2019-02-16T06:22:39.029Z Reads: 189

```
I tried this but when I try to read VESC 2, it appears to be the same as VESC 1. I scroll down and both list the same CAN ID. 

Example:
VESC 1 > Read > view CAN ID : 0
Go to VESC 2 > Read > view CAN ID: 0

Thoughts on how to correct this? Or possible bug?

Running dual FOCBOX 

I’m familiar with CAN FWD as that’s how I typically program my VESC from an externally accessible USB port. Just wasn’t sure if i needed to do somewhere here.

Edit: I should add that if I do back out to settings and enable CAN FWD, then read VESC 2, it will change to CAN ID: 1,  but if I go back to view VESC 1, it also updates to show ID 1.
```

---
## \#729 Posted by: rpasichnyk Posted at: 2019-02-16T06:35:57.020Z Reads: 182

```
It is a possible bug. Can you please disable CAN FWD, repeat your Example, go to Settings -> Show Logs and send to support@metr.at? Thanks!
```

---
## \#730 Posted by: Nubasaurus Posted at: 2019-02-16T06:52:59.845Z Reads: 179

```
Done. Thanks.
```

---
## \#731 Posted by: Nubasaurus Posted at: 2019-02-16T08:11:18.651Z Reads: 179

```
I did some more testing. I see what I did wrong. I have to hit read each time I switch between VESC 1 and 2. I had assumed it would act like tabs and show me the settings on each VESC so I could flip between them. 

Thanks for taking the time to address this for me.
```

---
## \#732 Posted by: amazingdave Posted at: 2019-02-17T15:11:30.323Z Reads: 183

```
I swapped connection from my board to my loan out board to check its battery and the record that was open seems to have been corrupted but just on the total distance ... it’s showing 29.9km where it should be 10km or less. Is there any way to look at the track record to get the actual distance I traveled?

Edit; link to record. 

https://metr.at/r/84Ami
```

---
## \#733 Posted by: bevilacqua Posted at: 2019-02-17T15:30:38.497Z Reads: 185

```
![image|690x388](upload://u5rhVpchPh8p5RegWY1w8T5YIy6.png) 

12,88km
```

---
## \#734 Posted by: rpasichnyk Posted at: 2019-02-17T16:42:32.974Z Reads: 188

```
Expert Tab 🎓 is getting some love. When multiple VESCs are connected via CAN, 
* Read button will read all configurations
* Write button will write all configurations
* Switching between configurations is like switching between browser tabs

https://gph.is/g/ap00jxa

This is how you would expect it to work, right?:grinning:
Thanks @Nubasaurus for the idea
```

---
## \#735 Posted by: Nubasaurus Posted at: 2019-02-17T18:54:56.530Z Reads: 187

```
![image|540x304](upload://djNAWe0mOAKm7UvtE7Nq7rcoL2B.gif)
```

---
## \#736 Posted by: Nubasaurus Posted at: 2019-02-18T02:04:17.733Z Reads: 183

```
@rpasichnyk I noticed Expert only saves the current VESC, and there's no way to rename or label master vs slave. Could you add either the naming of saved configs, or add VESC 1/2 to the default save name? I accidentally loaded my Master settings to my Slave which caused a bunch of havoc.

Edit: never mind. I see log pressing the file allows you to rename...
```

---
## \#737 Posted by: evoheyax Posted at: 2019-02-19T21:03:58.807Z Reads: 183

```
@rpasichnyk How do I get 4wd data? I see the option for dual data in the settings, but not for quad data...

Under the expert tab, I only see vesc ID's 1, 2 and 3, I don't see vesc 4.
The module is attached to ID 1.
PPM is on ID 2.
All 4 motors spin correctly together (via canbus) and I can see them all via the vesc tool via canbus. So I know it's a not a physical connection issue.
```

---
## \#738 Posted by: rpasichnyk Posted at: 2019-02-19T21:15:24.144Z Reads: 178

```
Please send log file to support@metr.at I will have a look
```

---
## \#739 Posted by: rpasichnyk Posted at: 2019-02-21T07:27:23.696Z Reads: 180

```

![19|300x300](https://media.giphy.com/media/3o6ZtbRh0xqwWzO8PC/giphy.gif) 

Metr app update is live and includes support for the latest VESC firmware v3.48 alongside with a better compatibility check. Metr Pro firmware v3.67 also live and needs to be updated over the air. Me and @hexakopter tried to test as much as we could, but you are always welcome to tell us if we missed something!
```

---
## \#740 Posted by: taz Posted at: 2019-02-21T09:01:38.307Z Reads: 181

```
https://tenor.com/view/who-is-the-man-you-are-the-man-you-got-it-all-you-gif-4392995
```

---
## \#741 Posted by: Bjork3n Posted at: 2019-02-21T18:53:33.654Z Reads: 178

```
Problem again..
I updated the metr pro firmware and now i get no data from the vescs.
It says its connected but no data is recived...
Anyway to go back to the old firmware?

Cant read motor values or any of the vesc settings either @rpasichnyk

Log sent to support@metr.at
```

---
## \#742 Posted by: rpasichnyk Posted at: 2019-02-21T19:00:27.188Z Reads: 172

```
Do these steps one by one until it helps:
* Turn bluetooth off and on (might be enough)
* Restart your phone
* Unpair and pair again with Metr Pro (last resort)
```

---
## \#743 Posted by: Bjork3n Posted at: 2019-02-21T19:06:46.804Z Reads: 171

```
Tried all.
Still no data from the vesc.
Just says connected but no data shows and i cant read any of the vesc.
```

---
## \#744 Posted by: rpasichnyk Posted at: 2019-02-21T19:11:27.102Z Reads: 172

```
Ok, I see in the logs that update went fine. Did you try to power cycle your board?
```

---
## \#745 Posted by: Bjork3n Posted at: 2019-02-21T19:12:41.762Z Reads: 174

```
Several times :confused:
```

---
## \#746 Posted by: rpasichnyk Posted at: 2019-02-21T19:14:26.478Z Reads: 172

```
Did you update VESC firmware too? (not needed, just wondering)
Can you check if green LED on Metr Pro turns ON when you power up?
```

---
## \#747 Posted by: Bjork3n Posted at: 2019-02-21T19:16:39.467Z Reads: 172

```
Nope, using ack 3.102. Worked perfectly with old metr pro fw. 
No i haven't unscrewed the enclosure yet to check
```

---
## \#748 Posted by: rpasichnyk Posted at: 2019-02-21T19:18:12.006Z Reads: 172

```
Oh I know what went wrong, hold on, I am working on it, no need to unscrew enclosure.
```

---
## \#749 Posted by: Bjork3n Posted at: 2019-02-21T19:19:13.671Z Reads: 173

```
😍👌 lovely thanks
```

---
## \#750 Posted by: rpasichnyk Posted at: 2019-02-21T19:22:03.175Z Reads: 175

```
Update Metr Pro firmware again to v3.68
```

---
## \#751 Posted by: Bjork3n Posted at: 2019-02-21T19:22:35.340Z Reads: 175

```
Ok i will try
```

---
## \#752 Posted by: Bjork3n Posted at: 2019-02-21T19:31:01.175Z Reads: 175

```
It seems to work now. Had the app freeze when using modes but after i restarted the app it worked again 👍
```

---
## \#753 Posted by: kalebludlow Posted at: 2019-02-21T22:07:46.998Z Reads: 169

```
Just ordered a Metr Pro, can't wait to add it to my build :grin:
```

---
## \#754 Posted by: mishrasubhransu Posted at: 2019-02-21T23:06:36.826Z Reads: 176

```
I got mine today, can't wait to put it on. 

@rpasichnyk, is it  going to be a lot of work to have more/configurable fields in the log? Say I want watts, or watthr/km. I can definitely open the log in Matlab or python and plot it myself, but would be nice to have it integrated into the existing setup.
```

---
## \#755 Posted by: SeanHacker Posted at: 2019-02-22T00:19:09.131Z Reads: 172

```
@rpasichnyk
 
Can we not use ack's firmware with this new update. No data here since the update?

I have the older modules in my boards.
```

---
## \#756 Posted by: NullReference Posted at: 2019-02-22T02:39:51.793Z Reads: 166

```
TCP bridge seems to not work correctly after I updated to the latest version of the app and Metr.Pro firmware. I'm getting a TCP timeout error 30 seconds after I attempt to connect on Vesc Tool.
```

---
## \#757 Posted by: Esk8enginneer Posted at: 2019-02-22T03:05:03.371Z Reads: 170

```
Can someone walk me through hooking up the Metr pro to the Unity and a DieBieMS.  I will be running this setup and just want to make sure I understand how everything is going to be hooked together.  Thanks guys sorry if this is a noob question.
```

---
## \#758 Posted by: rpasichnyk Posted at: 2019-02-22T07:41:01.747Z Reads: 164

```
@SeanHacker Yes you can! The fix for the older modules just arrived to Google Play v3.5.18, you will get it in a bit

@NullReference could not see your problem with my setup. Can you send logs to support@metr.at?
```

---
## \#759 Posted by: bevilacqua Posted at: 2019-02-22T09:27:52.433Z Reads: 159

```
Leave the diebiems CAN ID=10. For wirig check the diebiems thread, has been asked recently. 
Other than that default settings I think
```

---
## \#760 Posted by: janpom Posted at: 2019-02-22T20:51:26.188Z Reads: 159

```
Is it actually possible to export the recorded data? I haven't found the option for that and I looked really hard. :slight_smile:
```

---
## \#761 Posted by: SeanHacker Posted at: 2019-02-22T20:56:48.762Z Reads: 165

```
[quote="rpasichnyk, post:758, topic:57780"]
The fix for the older modules just arrived to Google Play v3.5.18
[/quote]

Did you already upload to the Play Store? Haven't got the update yet.
```

---
## \#762 Posted by: mishrasubhransu Posted at: 2019-02-22T21:06:28.808Z Reads: 168

```
@bevilacqua used them for his master's project. I just got my metr pro module. Haven't had a chance to explore it.
```

---
## \#763 Posted by: rpasichnyk Posted at: 2019-02-22T21:06:44.370Z Reads: 162

```
@SeanHacker I did upload it but forget to press Release button :flushed:
@janpom it is possible, using file manager and getting json app data from the phone, or by adding `?format=json` to the record url in the browser
```

---
## \#764 Posted by: mishrasubhransu Posted at: 2019-02-22T21:09:47.049Z Reads: 166

```
Hey @rpasichnyk, I know you are really busy fixing issues after the lastest vesc firmware update, but was wondering if you could talk about how hard it easy is it going to be to make logs configurable, when you are a bit free. To add extra fields etc.
```

---
## \#765 Posted by: rpasichnyk Posted at: 2019-02-22T21:22:43.161Z Reads: 168

```
It is already possible to calculate watts or watts/km using the data present in the record. What you are probably after is to display it in the browser, right? I will look at it :+1:
```

---
## \#766 Posted by: SeanHacker Posted at: 2019-02-23T04:04:04.136Z Reads: 172

```
@rpasichnyk

Latest Update works great with the old modules now. 

![37_2|373x500](upload://mL6XzLUXMKm6JpR2q01ZhGctezo.jpeg)
```

---
## \#767 Posted by: janpom Posted at: 2019-02-23T08:23:22.901Z Reads: 172

```
[quote="rpasichnyk, post:763, topic:57780"]
adding `?format=json` to the record url in the browser
[/quote]

Nice! I like the format. Very concise and comprehensible. I did quick parsing in Python. Here's a dump of one of my logs with the array data restricted to 10 points (taken from somewhere in the middle of the log) in case anyone else is interested in what kind of info is available.

```
ah: 2.34
ahRegen: 0.06
altitude: [196.2, 196.2, 196.2, 196.4, 196.4, 196.4, 196.4, 196.4, 196.7, 196.7]
appver: 3.5.4
consumption: [6.6, 6.8, 7, 7, 7.4, 7.5, 7.6, 7.6, 6.5, 7.6]
current: [5.3, 6.23, 6.12, 5.99, 5.38, 5.5, 5.52, 5.71, 5.48, 5.57]
distance: 17648.38
duty: [66.6, 67.1, 67.6, 66.3, 67.5, 68.9, 69.9, 69.1, 67.8, 68.3]
elapsed: [618623, 618806, 619065, 619339, 619567, 619772, 619954, 620158, 620389, 620635]
elapsedAh: [0.29, 0.29, 0.29, 0.29, 0.29, 0.29, 0.29, 0.29, 0.29, 0.29]
elapsedAhRegen: [0.02, 0.02, 0.02, 0.02, 0.02, 0.02, 0.02, 0.02, 0.02, 0.02]
elapsedDistance: [2730.8, 2730.8, 2730.8, 2730.8, 2739.3, 2739.3, 2739.3, 2739.3, 2739.3, 2746.8]
elapsedWh: [11.6, 11.6, 11.6, 11.6, 11.6, 11.7, 11.7, 11.7, 11.7, 11.7]
elapsedWhRegen: [0.8, 0.8, 0.8, 0.8, 0.8, 0.8, 0.8, 0.8, 0.8, 0.8]
end: 1550854003844
escCount: 1
faultCode: [0, 0, 0, 0, 0, 0, 0, 0, 0, 0]
faultsCount: 2
fw: 3.40 410
latitude: [49.17688, 49.17688, 49.17688, 49.17682, 49.17682, 49.17682, 49.17682, 49.17682, 49.17676, 49.17676]
longitude: [16.61679, 16.61679, 16.61679, 16.61687, 16.61687, 16.61687, 16.61687, 16.61687, 16.61692, 16.61692]
motorCurrent: [9.36, 10.81, 10.73, 10.6, 9.44, 9.42, 9.4, 9.75, 9.51, 9.59]
motorTemperature: [0, 0, 0, 0, 0, 0, 0, 0, 0, 0]
os: iOS 11.4
rpm: [29597, 29920, 29824, 29460, 29806, 30508, 30944, 30693, 30296, 30427]
speed: [26.78, 26.78, 26.78, 30.67, 30.67, 30.67, 30.67, 30.67, 29.81, 29.81]
start: 1550850465825
temperature: [27.6, 27.6, 27.6, 27.6, 27.6, 27.6, 27.6, 27.6, 27.6, 27.6]
version: 10
voltage: [39.6, 39.7, 39.7, 39.8, 39.7, 39.8, 39.7, 39.8, 39.6, 39.6]
wh: 88.77
whRegen: 2.44
```

@rpasichnyk What's `consumption`? The `version` is the version of the json format?
```

---
## \#768 Posted by: rpasichnyk Posted at: 2019-02-23T08:46:01.847Z Reads: 167

```
@janpom `consumption` is Wh per km value at the given moment. I do not display it yet on the web chart, but it is possible. Yes, `version` is a version of record format. Version 1 only had a few things, version 10 (current) has a lot more. This is one of the first records made on 29 October 2016 https://metr.at/r/NcF4o and it still displays fine because I have versioning in place :slight_smile:
@mishrasubhransu I added Power (Watts) to the chart, enjoy :slight_smile:
```

---
## \#769 Posted by: mishrasubhransu Posted at: 2019-02-23T09:40:51.407Z Reads: 165

```
Thanks Roman. You'll probably hate me for this, but wh/km is probably a better indicator if we are trying to be efficient. The reason I was requesting for that to be added to the chart is because, I want to learn my sweet spot in riding efficiency. :zipper_mouth_face:
```

---
## \#770 Posted by: rpasichnyk Posted at: 2019-02-23T10:43:17.039Z Reads: 156

```
I changed Watts to Wh/km (Wh/mi). I don't hate you :slight_smile: But now you have used all your wishes ;)
```

---
## \#771 Posted by: Pimousse Posted at: 2019-02-23T10:49:21.308Z Reads: 161

```
[quote="rpasichnyk, post:770, topic:57780"]
But now you have used all your wishes :wink:
[/quote]
@mishrasubhransu, I can sell you mines :smile:

Thanks, this info is also one I look the most at too. :pray:
```

---
## \#772 Posted by: mishrasubhransu Posted at: 2019-02-23T11:28:24.456Z Reads: 157

```
Haha, I'll take you up on it, if everything else fails.
```

---
## \#773 Posted by: Sn4pz Posted at: 2019-02-23T11:39:09.824Z Reads: 154

```
Very awe-struck at the level of efficacy that Roman has with his code... you make me jealous, I cant code like that! :rofl: 

How many years of practice do you have? @rpasichnyk
```

---
## \#774 Posted by: janpom Posted at: 2019-02-23T14:11:02.857Z Reads: 158

```
@rpasichnyk One more question, sorry. Do the `elapsedWh` and `elapsedAh` include the regenerated energy/current? I can see that there's `elapsedAhRegen`, but if I want the discharged Ah only it's not obvious whether it's `elapsedAh` or `elapsedAh - elapsedAhRegen`. Thanks.
```

---
## \#775 Posted by: Pedrodemio Posted at: 2019-02-23T14:44:18.691Z Reads: 160

```
Been waiting a lot for that, thanks Roman

Shouldn’t when negative current is flowing this value be negative? How much energy are you putting back at the battery at each kilometer?

And also the total average value considers the regenerated energy?
```

---
## \#776 Posted by: janpom Posted at: 2019-02-23T15:29:09.819Z Reads: 165

```
I played a little bit with Metr data in Jupyter notebok. I was mainly interested in the discharge curve for my battery pack (voltage vs. Wh), but since I was already at it, I looked at some other things, such as Wh / regenerated Wh vs. altitude to see whether regenerative breaking really works (it does! :slight_smile:) or how speed affects the energy efficiency (no strong conclusions there yet). Anyway, [here's](https://colab.research.google.com/drive/1glnV74xLNRwdulUe21U-H_lz2T46W0K8) what I have done. There's a lot of scary looking code at the top, but if you scroll all the way down, you'll see some charts.

![41|690x259](upload://mNoqTwX0lduacVxFqz91lJiIhYD.png) 

To analyze your own Metr data with the same notebook, do the following:
- download the notebook (`File > Download .ipynb`)
- upload the downloaded file back to Google Colab
- change the `METR_URL` at the very top
- `Runtime > Restart and run all...`

You can also add more charts to the notebook. I added a convenience `plot` function that's straightforward to use. Or, if there's some other data you'd like to see and don't know how to add it, you can ask me and I'll try to add it.

Thanks @rpasichnyk for doing such complete data logging. It's very useful.
```

---
## \#777 Posted by: Pimousse Posted at: 2019-02-23T15:39:39.256Z Reads: 158

```
I always wanted to draw the discharge curve of my battery however, my lack of Python skills made me give up.
Thanks a lot for sharing @janpom !
```

---
## \#778 Posted by: Pedrodemio Posted at: 2019-02-23T15:44:17.799Z Reads: 158

```
Really like it, well done

I’m trying to find out a way to take all my records and make a 2D plot of distribution of motor current vs rpm

The idea is to see what speed and torque range is most used for a given rider, this way I can optimize my DD motor to have peak efficiency at that predominant region
```

---
## \#779 Posted by: NullReference Posted at: 2019-02-23T16:08:20.222Z Reads: 154

```
Apparently it decided to fix itself. I fired it up today to get logs for you and it worked perfectly over TCP bridge.

I guess the universe just didn’t like me on Thursday.
```

---
## \#780 Posted by: janpom Posted at: 2019-02-23T16:28:52.235Z Reads: 172

```
Thanks. I tried plotting that in a scatterplot. Here's what the result looks like (more black = more frequent, logarithmic scaling):

![07|690x434](upload://ja83APaFWKcVonr1FDjicsdyuER.jpeg) 

I added it to the notebook. Not sure it's correct though. I would expect the more frequent points to be inside and less frequent outside, not the other way around.

Edit: Well, of course it's wrong because more brightness is more white. I'm such a genius. :smile: Corrected.

![11|690x436](upload://10HRykBTbFhUwtKvVDYqVYgDKGk.jpeg)

Edit2: A version with the `motorCurrent=0` data points excluded and with linear scaling for the brightness.

![44|690x460](upload://2saa5Bf73v8ZM4dRAX7I9OJ0TUG.jpeg)
```

---
## \#781 Posted by: bevilacqua Posted at: 2019-02-23T17:02:36.486Z Reads: 170

```
![image|690x387](upload://rgNm5GexX2cUgE4pXop3bpzCqVH.jpeg) 
V=0 and P=0 excuded || About 1M datapoints (still not enough)

Since I anayzed 9 to 13S boards I did it for power
```

---
## \#782 Posted by: Pedrodemio Posted at: 2019-02-23T17:46:54.696Z Reads: 165

```
@janpom thanks a lot, that’s exactly what I wanted  

@bevilacqua looking forward to the final results of your analysis, I think I have a few more points to send to you

The color scale is just and dimension less of the predominance?
```

---
## \#783 Posted by: bevilacqua Posted at: 2019-02-23T17:53:30.612Z Reads: 162

```
just a probability scala, the higher the more data points in that region. I'll post my work tomorrow, I found some typos :smile:... No so complicated data analysis, but well, I was totaly unexperienced so I learnt a lot
```

---
## \#784 Posted by: mishrasubhransu Posted at: 2019-02-23T17:58:47.523Z Reads: 164

```
I would love to see more of analysis and code in DD designing. I have been following your Feather thread. 

Also, good job @janpom.
```

---
## \#785 Posted by: rpasichnyk Posted at: 2019-02-23T18:59:22.703Z Reads: 165

```
`elapsedWh/Ah` does not include regen

@janpom @bevilacqua nice! 
![51|500x500,50%](https://media.giphy.com/media/bjx2nsum8nSYo/giphy.gif)
```

---
## \#786 Posted by: janpom Posted at: 2019-02-23T19:19:49.430Z Reads: 165

```
Thanks! I like how these are labeled in the new VESC app: "Wh out" and "Wh in". Short and very clear.
```

---
## \#787 Posted by: DavidC Posted at: 2019-02-23T22:39:00.451Z Reads: 166

```
I've got a problem with Metr Pro. I updated my FSESC 6 DUAL to latest firmware and Metr Pro to latest version.

But when I launch Metr Pro on androïd it changes master vesc motor setting to the old ones. Even if I don't touch to "Modes" or "Expert". A a result master and slave vesc have different motor current settings.
```

---
## \#788 Posted by: KrisKraanen Posted at: 2019-02-24T01:43:14.728Z Reads: 169

```
I have the problem that the metr pro works fine but then out of nowhere decided to stop and displays the message RT Timed out  in develepor mode, then is shows connected but no realtime data and no expert mode
```

---
## \#789 Posted by: KrisKraanen Posted at: 2019-02-24T03:18:55.521Z Reads: 165

```
It had some problems but now i starts but i can’t pair to it, everytime i enter the digits its led lights up
```

---
## \#790 Posted by: rpasichnyk Posted at: 2019-02-24T06:40:54.617Z Reads: 165

```
@DavidC clear Startup Mode. Check this post https://www.electric-skateboard.builders/t/configuration-and-telemetry-for-vesc-ios-android/13483/1243?u=rpasichnyk
@KrisKraanen go to bluetooth settings in your phone and forget (unpair) Metr Pro. Then try to pair again.
```

---
## \#791 Posted by: DavidC Posted at: 2019-02-24T06:53:36.159Z Reads: 161

```
Ok thank you very much! I'll try. I already removed the start up mode but I didn't push "Clear Startup Mode" as you show.
```

---
## \#792 Posted by: DavidC Posted at: 2019-02-24T07:01:36.648Z Reads: 176

```
The three vertical points where you click don't show. My board is shut down at the time. Do I need to be connected to Metr Pro module to be able to click "Clear Startup Mode" (and then when connected I'll loose my master vesc settings once more :open_mouth:)

![](https://media.giphy.com/media/8F9fPnn4qBkJ9DD2cP/giphy.gif)

![IMG_6075|375x500](upload://pRhiFWQwmVxTng5H248AbEpN4MY.jpeg)
```

---
## \#793 Posted by: rpasichnyk Posted at: 2019-02-24T07:28:03.958Z Reads: 164

```
Yes you need to be connected
```

---
## \#794 Posted by: DavidC Posted at: 2019-02-24T09:01:49.337Z Reads: 159

```
Thanks! Can I "Reset settings" in preferences to get rid of startup mode without connecting to module?
```

---
## \#795 Posted by: trampa Posted at: 2019-02-24T10:30:59.175Z Reads: 162

```
[quote="janpom, post:786, topic:57780, full:true"]
Thanks! I like how these are labeled in the new VESC app: “Wh out” and “Wh in”. Short and very clear.
[/quote]

It's also accumulated data over all ESCs. 
Problem about using data from only one ESC has been the accuracy. Heel side motors take 60 to 65% of the strain, while toe side motors are less stressed. The new code gives you quite precise values.
```

---
## \#796 Posted by: rpasichnyk Posted at: 2019-02-24T11:14:34.195Z Reads: 160

```
No, you can not. Startup mode is stored on the Metr Pro, not on your phone
```

---
## \#797 Posted by: KrisKraanen Posted at: 2019-02-24T11:51:10.722Z Reads: 159

```
Thats what im trying but now the 
Passcode which is on the back of the metr seems to be changed somehow
```

---
## \#798 Posted by: KrisKraanen Posted at: 2019-02-24T13:43:11.221Z Reads: 156

```
This is whats happening https://youtu.be/MAESLF_efNg
```

---
## \#799 Posted by: janpom Posted at: 2019-02-24T16:27:21.928Z Reads: 167

```
[quote="trampa, post:795, topic:57780"]
Heel side motors take 60 to 65% of the strain, while toe side motors are less stressed.
[/quote]

That's very interesting. Thanks for the info. I'll do the measurements on my boards. I'd be interested to know if there's really that much difference in the strain.
```

---
## \#800 Posted by: trampa Posted at: 2019-02-24T16:35:34.854Z Reads: 168

```
It is. Raptor 2 motor temp has been debated several times in Unity thread. Heel side glows, while the side is 25-30deg cooler. 
The big difference in strain taken by the two motors was a big issue for accurate RT-Data display. In consequence Benjamin coded the new VESC-Tool with accumulated values from all VESCs. Otherwise your values can easily be 15-20% off tge reality.
```

---
## \#801 Posted by: Pedrodemio Posted at: 2019-02-24T17:10:58.563Z Reads: 167

```
I think this may happen when you are traction limited, checks both vesc several time and energy consumption was almost identical between them
```

---
## \#802 Posted by: rpasichnyk Posted at: 2019-02-24T17:30:11.092Z Reads: 171

```
Thanks for the video. I guess I know what you are doing wrong. You should do the pairing in the Metr app and not in the phone bluetooth settings.

1) Unpair Metr Pro
2) Open Metr app and do pairing from there
3) If it didn't work, send logs to support@metr.at
```

---
## \#803 Posted by: KrisKraanen Posted at: 2019-02-24T22:33:58.040Z Reads: 164

```
where do i accure the logs? i can't seem to save the file from the app
```

---
## \#804 Posted by: KrisKraanen Posted at: 2019-02-24T22:37:00.785Z Reads: 168

```
when its says connected in the realtime window, although the password is wrong ( i think) and i go to modes to apply a mode it gives me the error: Firmware <= 2.18 can't apply
```

---
## \#805 Posted by: rpasichnyk Posted at: 2019-02-25T07:57:38.050Z Reads: 170

```
The PIN can not be wrong. Each module is tested before shipping. The PIN is alright. Did you do what I asked? 

[quote="rpasichnyk, post:802, topic:57780"]
* Unpair Metr Pro
* Open Metr app and do pairing from there
[/quote]

To get the log file in the Metr app, go to Settings -> Show Logs.
```

---
## \#806 Posted by: KrisKraanen Posted at: 2019-02-25T08:49:54.820Z Reads: 169

```
Yes i did it via the app, it connected then disconnected tried to reconnect again and this process repeated itself, everytime it "connected" the module goes red as in the video.
```

---
## \#807 Posted by: The_Dude Posted at: 2019-02-25T20:09:36.760Z Reads: 169

```
@rpasichnyk Hi Roman, I want to upgrade my metr to the metr pro module I bought some time ago. Does the metr pro use the ADC1-3 pins (metr doesn't) or can I use the pins for my own purposes?
```

---
## \#808 Posted by: janpom Posted at: 2019-02-25T20:37:47.924Z Reads: 171

```
I don't have any of the ADC connected and it still works.

You do need to connect both the 5V and 3.3V though, which caught me by surprise. I only connected the 5V first and it kinda worked but the BT connection was extremely unstable. After connecting 3.3V as well it works like a charm.

Edit: 5V actually doesn't need to be connected.
```

---
## \#809 Posted by: The_Dude Posted at: 2019-02-25T20:38:51.964Z Reads: 171

```
thx 10char
```

---
## \#810 Posted by: rpasichnyk Posted at: 2019-02-25T20:39:58.861Z Reads: 173

```
What @janpom said. ADC is free to use. 
 https://metr.at/faq#q32
```

---
## \#811 Posted by: janpom Posted at: 2019-02-25T20:42:37.816Z Reads: 176

```
Hm, so the 5V actually doesn't have to be connected?
```

---
## \#812 Posted by: The_Dude Posted at: 2019-02-25T20:53:21.478Z Reads: 180

```
Is the operating voltage of the metr pro different to the metr module?
```

---
## \#813 Posted by: rpasichnyk Posted at: 2019-02-25T20:54:18.570Z Reads: 181

```
@janpom no, 5V doesn't need to be connected
@The_Dude old modules 3.6V-6V, Metr Pro 3.3V
```

---
## \#814 Posted by: KrisKraanen Posted at: 2019-02-26T12:26:03.510Z Reads: 175

```
Yes i did this, a message popped up in the app, can’t connect cause of incorrect pin or passkey
```

---
## \#815 Posted by: KrisKraanen Posted at: 2019-02-26T12:26:49.692Z Reads: 173

```
Is there a way to  reset it to factory settings?
```

---
## \#816 Posted by: KrisKraanen Posted at: 2019-02-26T12:33:11.525Z Reads: 173

```
Found the problem, the android app was bugged, works fine on apple app, reinstalled the android app still error so i think there is a problem with the android app
```

---
## \#817 Posted by: Sooty Posted at: 2019-03-02T11:07:43.341Z Reads: 180

```
Can't seem to connect to my VESC6 anymore. Seems to show up in the logs but it never shows up while scanning...

![](https://dl2.pushbulletusercontent.com/foSbVyxT2ZCNN3oZApG0ZIqUksvR4l4t/Screenshot_20190302-105217.png)

https://pastebin.com/FU49aazn

Any suggestions?
```

---
## \#818 Posted by: rpasichnyk Posted at: 2019-03-02T15:30:47.456Z Reads: 167

```
What BLE module are you using? It says in the logs `name:VESC BLE UART` and not `Metr Pro` :confused:
```

---
## \#819 Posted by: Sooty Posted at: 2019-03-02T17:51:32.831Z Reads: 176

```
Ah looks like I'm using the trampa one. 

https://www.trampaboards.com/vesc-connect-wireless-dongle-p-25516.html

It used to work, so not sure what changed...
```

---
## \#820 Posted by: rpasichnyk Posted at: 2019-03-02T18:54:05.476Z Reads: 173

```
I am sorry, there is no way it worked with Metr app before. You have to purchase Metr Pro to be able to use the app.
```

---
## \#821 Posted by: rojitor Posted at: 2019-03-02T20:33:59.905Z Reads: 173

```
Mine stopped working this week. Xiaomi firmware update is to blame
```

---
## \#822 Posted by: SeanHacker Posted at: 2019-03-02T21:06:35.742Z Reads: 173

```
@rpasichnyk Where do we find the faults at in the app? Never had one before until today so I'm clueless.
```

---
## \#823 Posted by: rene Posted at: 2019-03-03T06:28:02.945Z Reads: 176

```
@rpasichnyk I tried to update my Vesc6 via the new VescTool Android App via MetrPro Module and it seems to have made a err somewhere. because it does not start the new FW. norbam I able to flash those via PC and Vesc Tool.

you maybe want to check this. 
I will need to use the St-link v2 next week.
```

---
## \#824 Posted by: janpom Posted at: 2019-03-04T21:01:20.470Z Reads: 183

```
[quote="trampa, post:795, topic:57780"]
Problem about using data from only one ESC has been the accuracy. Heel side motors take 60 to 65% of the strain, while toe side motors are less stressed. The new code gives you quite precise values.
[/quote]

I have done my own measurements today. Here's the data from my two VESCs on a ~10.5km ride. This was ca 7km of paved road and the rest pretty rough terrain in a forest, lots of steep hills (I didn't even think I would make it up on some :)). 12S 8Ah LiPo battery, 2x 6374-149kv SK3, MBS tires.

![41|690x211](upload://xrTAUQrsmkRUxr8S0jz5XtB0IeG.png) 

![50|498x208](upload://8ZauaW0VUCN6jzNC3WWYRac1MEC.png) 

![45|490x214](upload://c7IlebOR5qbpgFlq0QcDcwxnbao.png)

In my case, it was actually the toeside motor that took more strain (I double-checked I didn't get the readings reversed) and the difference between the two is not even 52/48, so 60/40 or even 65/35 seems exaggerated though I understand that YMMV.
```

---
## \#825 Posted by: mishrasubhransu Posted at: 2019-03-04T23:29:00.479Z Reads: 174

```
So to convert the board antenna to external antenna I have to move the 0 resistor from the board antenna side to external antenna side. But is it a 0R resistor or a capacitor?

"is it possible to change external/internal antenna afterwards?

Yes, it is possible but requires some good soldering skills. You need to resolder the 0402 capacitor near the u.FL connector in a different position to change between internal PCB antenna and external antenna."
```

---
## \#826 Posted by: rpasichnyk Posted at: 2019-03-05T06:19:36.382Z Reads: 172

```
It's a capacitor
```

---
## \#827 Posted by: pookybear Posted at: 2019-03-05T06:41:58.136Z Reads: 170

```
Any updates on the direct replacement BT metr version for the unity?
```

---
## \#828 Posted by: FredXanadu Posted at: 2019-03-05T11:07:22.258Z Reads: 164

```
yes i need this in my life :slight_smile:
```

---
## \#829 Posted by: rojitor Posted at: 2019-03-05T15:37:02.251Z Reads: 169

```
I said the same the first time i saw boobs.
```

---
## \#830 Posted by: hexakopter Posted at: 2019-03-07T01:36:25.607Z Reads: 173

```
[quote="pookybear, post:827, topic:57780, full:true"]
Any updates on the direct replacement BT metr version for the unity?
[/quote]


We will let you guys know when we have some updates to share. :smiley: I am very busy at the moment, so unfortunately not much time to work on it. I think it should be ready before summer, but no specific ETA at this point. Will keep you updated.
```

---
## \#831 Posted by: pookybear Posted at: 2019-03-07T01:57:35.133Z Reads: 176

```
It's hard for me to use this BT module with my feather remote. It uses the uart port. I could connect it to the extra uart ports inside the unity but I'd have to leave the cover off. Additionally, I need to be able the change the baud rates for those specific ports. I know sofu shared that special firmware but for some reason, the unity app doesn't recognize this version and disconnects. Im pretty much SOL.

This new BT direct replacement for the unity one fixes all my issues.
```

---
## \#832 Posted by: FredXanadu Posted at: 2019-03-07T10:37:32.604Z Reads: 166

```
i"m pretty sure the team are working hard on the new module, isn't it @hexakopter ?
```

---
## \#833 Posted by: mishrasubhransu Posted at: 2019-03-08T01:24:21.755Z Reads: 170

```
@rpasichnyk, probably you don't have a whole bunch of customers with DieBieMS, but it would be nice if we could configure some main settings form Metr app.
```

---
## \#834 Posted by: pookybear Posted at: 2019-03-08T03:42:49.543Z Reads: 170

```
I'm ok waiting. Not a big deal. I just wished unity app came w modes feature. The ability to be able to switch modes is really the only thing i use the most.
```

---
## \#835 Posted by: rpasichnyk Posted at: 2019-03-08T05:16:09.839Z Reads: 165

```
You can do it via Terminal option in Metr app
```

---
## \#836 Posted by: mishrasubhransu Posted at: 2019-03-08T19:32:54.597Z Reads: 173

```
How does one delete records from the app, to reduce clutter? Also everytime I do upload it goes into the metr server and creates a new link? Even if it is for the same log?

Any plans to upload the logs directly to google drive? so that I can keep all records in one place even when I uninstall the app.
```

---
## \#837 Posted by: rpasichnyk Posted at: 2019-03-08T21:09:10.345Z Reads: 173

```
* Swipe the record to the left to delete
* Same link when you upload again
* Some plans to do account / sync records but no ETA
```

---
## \#838 Posted by: mishrasubhransu Posted at: 2019-03-10T17:23:48.150Z Reads: 170

```
@rpasichnyk, requesting a feature
it would be nice if we can display the remaining range on the main screen. Of course this would vary, but we can have a configurabe setting under battery where we can set the worst-case/average wh/km.

The vesc tool mobile app does this based on the average consumption so far in a trip.
```

---
## \#839 Posted by: wafflejock Posted at: 2019-03-12T15:09:02.508Z Reads: 171

```
Having similar issue to @KrisKraanen on a Nexus 5X.  Was working great but some sort of system update or something seems to have broken the connection and now even when connecting from within the app I'm prompted for a pin (tried on two android devices) a bit stuck.  I can collect logs or whatever but would be good if there are known good steps to follow so my logs make some sense (I'll do what seems reasonable for now)  Tried rebooting the phone and uninstall/reinstall of app all results in same pop up message asking for pairing request and pin (tried 0000, or 1234, just loops back to prompt).
```

---
## \#840 Posted by: rpasichnyk Posted at: 2019-03-12T15:22:09.131Z Reads: 170

```
Q: Where is the PIN code for Metr Pro module?

A: You can find the PIN code on the back side of the module.

https://metr.at/faq#q4
```

---
## \#841 Posted by: wafflejock Posted at: 2019-03-12T15:24:52.606Z Reads: 172

```
:man_facepalming: as in DM you are correct sir, after putting in the PIN on the module I'm connected again thanks :)
```

---
## \#842 Posted by: rojitor Posted at: 2019-03-12T16:59:35.065Z Reads: 168

```
My app doesn't launch since the last xiaomi update. All i get is a black screen. Sucks. It was working so fine.
```

---
## \#843 Posted by: rpasichnyk Posted at: 2019-03-12T20:15:32.483Z Reads: 173

```
This is weird, but thank you for letting me know! I don't have xiaomi at hand but maybe you can collect some helpful information if you have computer which you can connect to your phone with USB.

- Install adb on your computer, enable Developer Mode on xiaomi
- Run "adb logcat"
- Start metr app
- Collect output of adb logcat and send to support@metr.at

If this is sounds too complicated, you can also try reinstalling the app, maybe it will work. Or wait until I get someone who has xiaomi and can help with this issue :bug::hammer:
```

---
## \#844 Posted by: rojitor Posted at: 2019-03-13T12:07:47.743Z Reads: 173

```
I reinstalled several times. No luck. I will try the pc thing when i have the chance
```

---
## \#845 Posted by: kalebludlow Posted at: 2019-03-14T22:51:15.536Z Reads: 172

```
Just received and installed my Metr Pro. Super easy to setup and use, no issues at all!
```

---
## \#846 Posted by: KrisKraanen Posted at: 2019-03-15T16:14:14.135Z Reads: 165

```
I had to reset my bluetooth in the phone some web page shows how to it with your phone, noe its working fine again
```

---
## \#847 Posted by: wafflejock Posted at: 2019-03-17T00:42:21.754Z Reads: 169

```
Yah have had this happen a few times too where I need to cycle the bluetooth on and off on the phone and scan again for it to connect but small inconvenience.  Main problem I'm having now is self imposed, after trying to flash firmware over bluetooth/tcp bridge I ended up putting my VESC in an unusable state.... managed to recover with an ST-Link but I still need to get the bootloader on there I beleive because the USB connection still doesn't work as is so I've been relying on the bluetooth module to update the firmware and configure things for the time being (all working at this point but think the bootloader is still missing so going to continue tinkering, figure I probably can't brick it more than I have already and seems recoverable with ST-link in the worst case scenario)
```

---
## \#848 Posted by: rojitor Posted at: 2019-03-17T19:41:09.134Z Reads: 163

```
i have sent you the data.
```

---
## \#849 Posted by: rey8801 Posted at: 2019-03-17T21:39:12.325Z Reads: 168

```
Guys one question. Would an old metr module work with a unity or only the pro one can do it? Thx
```

---
## \#850 Posted by: Pimousse Posted at: 2019-03-17T22:40:07.615Z Reads: 173

```
Did you erase the entire chip u der ST-Link software ?
Once done, flash the firmware and connect via VESC-Tool and burn the bootloader through it.
What's your computer OS ?
```

---
## \#851 Posted by: rojitor Posted at: 2019-03-17T23:01:07.898Z Reads: 171

```
It works again with your last update
```

---
## \#852 Posted by: Jc06505n Posted at: 2019-03-17T23:08:04.396Z Reads: 172

```
Unless the old meter module is updated , which I think only the pro is, then no. The unity has a different uart protocol then regular VESC’s
```

---
## \#853 Posted by: rey8801 Posted at: 2019-03-17T23:08:44.715Z Reads: 166

```
ah ok I thought so but was worth it to ask
Thanks for the info
```

---
## \#854 Posted by: wafflejock Posted at: 2019-03-18T02:35:26.803Z Reads: 186

```
Hey yah after trying to set modes in the app the vesc wouldn't respond (metr said VESC is running old firmware).  Once the disconnect happens from the module I tried hooking up over USB but no connection, so connected with stlink and cleared memory using windows and flashed hex file found searching the internet file with bootloader and firmware combined i think.  After flashing that way i regain connection via metr module but still no USB.  After that i tried bootloader upload via metr tcp bridge but same situation basically can consistently wipe and flash with st link but no flashing lights on boot seemingly no USB and can configure via metr module after flashing manually and then can update firmware but think bootloader is still botched.   I have access to windows ubuntu and mac os I've mostly been using windows to erase and flash but also tried with CLI make upload command and rougly same thing happening (flashing looks successful but no device in dmesg via regular usb only connected with st link)

Also things are working fine when configured over the tcp bridge but would be nice to be able to set modes on the fly again and just know whats going on with the USB connection so open to suggestions.
```

---
## \#855 Posted by: Skunk Posted at: 2019-03-18T02:41:21.727Z Reads: 180

```
[quote="Sn4pz, post:577, topic:57780, full:true"]
Do you have any information that proves otherwise ? Lmfao
[/quote]

Fast forward to the future @SeanHacker and guess what ..... you do have information that proves otherwise lol. But we'll keep that to ourselves lololololol
```

---
## \#856 Posted by: Sn4pz Posted at: 2019-03-18T03:13:11.620Z Reads: 181

```
Ah yes, I was wrong. Like a *human*. lmfao :roll_eyes:
```

---
## \#857 Posted by: Pimousse Posted at: 2019-03-18T07:42:41.342Z Reads: 179

```
I also had issues burning the bootloader through ST-Link software on Windows.
Erase fully the chip (all the table shall be filled with FFFF), then write ONLY the firmware.
If it doesn't work, check USB port integrity (I mean physically) and try another cable.
If you recover the USB connection, burn the bootloader via VESC-Tool.
```

---
## \#858 Posted by: willumpie82 Posted at: 2019-03-20T10:28:53.066Z Reads: 181

```
I have upgraded all firmwares of my VESC4.12 last weekend, since I'm unable to connect to them via the TCP bridge option and latest VESCtool for mac from your github, a connection attempt results in a firmware unknown error, I do see some bytes send, none received in metr.pro

Could this have to do with the vesc "app" configuration configured as just ppm or none, 
I have two vesc, the master has a ppm/uart solidgeek-ish receiver, The slave VESC connects to the Metr.pro, both VESCs and DieBieMS is connected via CAN (nothing electricly changed, worked fine before the fw upgrade)
```

---
## \#859 Posted by: rpasichnyk Posted at: 2019-03-20T10:50:14.169Z Reads: 177

```
Yes, VESC that is connected to Metr Pro **must** have UART enabled!
```

---
## \#861 Posted by: Hummie Posted at: 2019-04-01T19:02:57.368Z Reads: 168

```
Anyone have one of these for sale pronto? Like to get it in the next couple days. It’s a long thread

Looking for logging I can overlay with the moving background and not the white or black background
```

---
## \#862 Posted by: PickSix24 Posted at: 2019-04-02T00:29:27.142Z Reads: 168

```
@Hummie , I’ve got one if you are still looking
```

---
## \#863 Posted by: Bjork3n Posted at: 2019-04-04T18:25:13.266Z Reads: 165

```
Had a issue today with the metr recording. 
It seems like it recorded the speed but stopped record the voltage, duty, Amps after a while. Stopped record values at 18.23. Any ideas? Here is the record. 
https://metr.at/r/p5Ykb
```

---
## \#864 Posted by: TinnieSinker Posted at: 2019-04-07T07:53:36.446Z Reads: 158

```
since updating to the lasted vesc firmware, i can no longer change modes as the Metr app only recognizes one of the two Focboxs. 

is this a common bug that is being worked on or should this work? ( i have the latest Metr app)
```

---
## \#865 Posted by: Friskies Posted at: 2019-04-07T08:02:24.700Z Reads: 158

```
Have you updated the Metr firmware via the app @TinnieSinker
```

---
## \#866 Posted by: TinnieSinker Posted at: 2019-04-07T08:46:54.843Z Reads: 159

```
ummm firmware on the BT module? i have not, where is the option for that?
```

---
## \#867 Posted by: Friskies Posted at: 2019-04-07T08:47:46.532Z Reads: 173

```
https://www.electric-skateboard.builders/t/metr-pro-next-gen-bluetooth-module/57780?u=friskies

![](https://www.electric-skateboard.builders/uploads/db1493/original/3X/b/e/bef7c1a70c57e1ce441be1c0d872af473ff48fcf.gif)
```

---
## \#868 Posted by: TinnieSinker Posted at: 2019-04-07T08:59:42.571Z Reads: 168

```
thanks! i did not know that cog is a button haha
```

---
## \#869 Posted by: SimosMCmuffin Posted at: 2019-04-07T16:27:34.268Z Reads: 170

```
Can connect to Metr module, can update Metr firmware, but it can't detect VESC firmware or hardware and seems to be unable to communicate with the VESC to relay information to the Metr app.

I'm running dual VESC 6s over CAN bus, so I decided to update VESCs' firmwares manually from 3.34 to 3.54. When I got the master VESC flashed and got the settings configured (motor and app) the Metr app seemed to be working, got actually some live data running in the realtime window, but after I tried again after setting up the second VESC and got the CAN configured. Well now there is no life in the Metr app again, even though I can connect to the Metr module.

"Enable Permanent UART" is set to True and was not changed from default.

What do?

**SOLVED**: In VESC tool on the **MASTER VESC**; "App settings" -> "General" -> "APP to Use" needs to be set to "control signal and UART". In my case with GT2B PPM RC controller "PPM and UART". 

_I recommend adding this to the FAQ section on_ "https://metr.at/faq"
```

---
## \#870 Posted by: Hansg Posted at: 2019-04-10T15:35:50.598Z Reads: 166

```
Hello @SimosMCmuffin,

Could you let me to know how can I upgrade my firmware 3.34 to 3.54?
I am try to upgrade but I cant because it show me the error  "Status: Serial port error: The I/O operation has been aborted because of either a thread exit or an application request.". check this video.

https://tinytake.s3.amazonaws.com/pulse/hans-nserio/attachments/10337167/TinyTake10-04-2019-10-35-31.mp4
```

---
## \#871 Posted by: Bjork3n Posted at: 2019-04-10T18:12:54.998Z Reads: 165

```
This is normal to get this fault message in the end of the upload.
You get it because it reboots the vesc and i takes a couple of sec to get it connected again.

To Check if the fw is updated go to the firmware tab and check.
```

---
## \#872 Posted by: SimosMCmuffin Posted at: 2019-04-10T18:21:33.249Z Reads: 164

```
Just as @Bjork3n said

[quote="Bjork3n, post:871, topic:57780"]
This is normal to get this fault message in the end of the upload. You get it because it reboots the vesc and i takes a couple of sec to get it connected again.
[/quote]

I personally didn't even notice the disconnect message at the bottom of the VESC tool, as I was already expecting it to disconnect upon finishing the flashing and rebooting.
```

---
## \#873 Posted by: Hansg Posted at: 2019-04-10T18:41:40.291Z Reads: 169

```
@Bjork3n  When I go to the tab firmware the software is the old, never update :frowning:

Check this video: 

https://tinytake.s3.amazonaws.com/pulse/hans-nserio/attachments/10338594/TinyTake10-04-2019-01-40-16.mp4
```

---
## \#874 Posted by: Surfer Posted at: 2019-04-10T18:46:43.411Z Reads: 165

```
Did you updated before? When you don't have bootloader that's what happens
```

---
## \#875 Posted by: Hansg Posted at: 2019-04-10T19:51:20.726Z Reads: 166

```
yes, I updated the firmware to version 3.34 in November
```

---
## \#876 Posted by: pookybear Posted at: 2019-04-10T23:35:32.115Z Reads: 165

```
Vesc6 settings:

* 30
* -30
* 15
* -12

It feels very slow. I have the exact same settings using unit and focbox. It's significantly slower with vesc6. Any ideas why?

https://metr.at/r/vgX22
```

---
## \#878 Posted by: Andy87 Posted at: 2019-04-11T08:37:54.007Z Reads: 160

```
Seems like this thread is more active than you thought 😜
```

---
## \#879 Posted by: sayekim Posted at: 2019-04-11T11:25:54.175Z Reads: 161

```
I don’t think you are in the right thread.
```

---
## \#880 Posted by: rey8801 Posted at: 2019-04-14T17:37:36.103Z Reads: 164

```
@rpasichnyk hi! Just pulled the trigger on 2 metr pro modules. Super exited to finally have back telemetry with the Unity. I was waiting Enertion's app but will take too long I guess. One question that it's not totally clear to me. I know Metr works with Unity but it is possible to use it with the internal UART port? I read it somewhere but maybe now there is a more clear tutorial to follow. I would like to keep the external one for the remote or other device.
Thank you very much.
```

---
## \#881 Posted by: rpasichnyk Posted at: 2019-04-15T05:15:26.606Z Reads: 169

```
Yes, it is possible. You can check this post :slight_smile:

https://www.electric-skateboard.builders/t/sofu-s3-haya-12s4p-vtc6-modular-holders-surf-rodz-rkp-200mm-maytech-6880-190kv-unity-featherremote-18-20-33-100mm/79880/179
```

---
## \#882 Posted by: rey8801 Posted at: 2019-04-15T05:42:22.483Z Reads: 168

```
I saw the post I was hoping there was a step by step procedure since a lot of people are using unity by now. Maybe @sofu can you make a tutorial for it? A short on è is fine too. I was wondering the custom firmware allow you to chenge the interla UART baud rate or just change them to 115200 and you cna not play with it? Just to know which device will be compatible with the internal one since some modules use 9600, other 115200. Is the firmware still update or not there are new one? I have seen at least  2 official firmwares updates meanwhile.

Thank you
```

---
## \#883 Posted by: Bjork3n Posted at: 2019-04-17T20:50:16.289Z Reads: 168

```
On my ride to work today my board lost Power all of a sudden. I could still brake but nothing happend when i pushed to throttle forward. 
Any idea whats going on? 
Duty 111% accoding to the metr app ? :thinking: 
Dont know if its the bms acting up or something might be wrong with my batterypack..
https://metr.at/r/57Fwa?fbclid=IwAR3yNsFEb_7VPyRqmu2iCW39WDAJaErc4gMlmi0VtMDXqw_0T2xjBqRqKEM
```

---
## \#884 Posted by: sayekim Posted at: 2019-04-17T21:04:38.456Z Reads: 168

```
Which esc, esc fw, motors, battery, antispark, bms and how is it al wired up?

You got some weird readings at the end there. It goes over 100% duty a few times before the fault is logged. 

What did you do after it happened to get going again?

I had this happen to me once and I kick pushed to get home and while kick pushing it suddenly sprung back to life. 

Escapes fw3.38, maytech 6374 190kv, ali 12s bms bypassed or so I thought (discharge was connected to the charge lead, dumbass me), martinsp push to start v1, samsung 30q 12s6p.

https://metr.at/r/JvaJK
```

---
## \#885 Posted by: Bjork3n Posted at: 2019-04-17T21:10:56.654Z Reads: 164

```
Dual focboxes over can.
Besttech bms with e-switch and 10s4p 30q made by eskating. Bms is not bypassed. 
dual 190kv 6374

I noticed the board wouldnt accelerate but braking was fine, i just turned the board off and on and it worked fine for the 3km i had left to get to work.

This has happend to me once before on a diffrent ride.
```

---
## \#886 Posted by: sayekim Posted at: 2019-04-17T21:41:25.254Z Reads: 164

```
Which firmware version?
```

---
## \#887 Posted by: Bjork3n Posted at: 2019-04-18T03:42:14.460Z Reads: 166

```
Ackmaniac 3.102

I think i found the issue.. Its seems to be the on/off switch. I taped it up when heading home from work and everything worked fine. I will replace the switch since it lost that "click" when turning on and off.
```

---
## \#888 Posted by: hiboute Posted at: 2019-04-18T07:27:32.831Z Reads: 161

```
I had some issue yesterday, i tried to configure my remote over tcp bridge, but everytime i was activating rt/app on vesc tool, the metr is disconnecting. And i have to restart the board to connect back.
I’m on ackmaniac 3.103 and dual focbox.
```

---
## \#889 Posted by: mishrasubhransu Posted at: 2019-04-18T09:34:36.195Z Reads: 157

```
@rpasichnyk, do you have any plans to generate audio notifications from the Metr pro app for critical errors or even general info.. If people have their earphones on while riding that's a nice way of receiving information.

Like Jarvis. Haha.
```

---
## \#890 Posted by: rey8801 Posted at: 2019-04-18T09:59:30.523Z Reads: 157

```
It's actually pretty cool idea... The skate can get close to Kit car :heart_eyes:
```

---
## \#891 Posted by: rpasichnyk Posted at: 2019-04-18T10:16:25.823Z Reads: 160

```
It is already in the app 😉

![image|500x500](upload://jqtIWIdUmE55BLTjfBsjUD5mW9K.jpeg)
```

---
## \#892 Posted by: mishrasubhransu Posted at: 2019-04-18T10:34:14.207Z Reads: 155

```
Ohh it's perfect how did I miss it.
```

---
## \#893 Posted by: rey8801 Posted at: 2019-04-18T10:40:32.663Z Reads: 158

```
Hi. I got the message thst I am receiving the metr modules. Thank you for the fast shipping! Si c'è I will use them on Unity only, would be possible to make a more clear tolutorial to how to connect the module to the internal UART port? I understood the principle but that will avoid me too luck 2 hours for all the pin layout to be sure I don't do mistakes. I am pretty sure others will use it as well. I didn't know you where making the replacement module for the unity. Now too late :grin: if you manage to do it thank you very much.
```

---
## \#894 Posted by: rpasichnyk Posted at: 2019-04-18T11:00:11.284Z Reads: 159

```
We will not write this tutorial since we already making a special module for UNITY which will be easy plug and play. But you can be the hero :wink:
```

---
## \#895 Posted by: rey8801 Posted at: 2019-04-18T11:01:23.775Z Reads: 163

```
Damn I should have read before, now I got two new modules on the way. Well I guess I iwll have to figure it out. Thanks anyhow.
```

---
## \#896 Posted by: Sn4pz Posted at: 2019-04-18T11:19:16.753Z Reads: 165

```
I knew there was an secret message in that PM I sent you awhile back... 😂 

Glad I took your advice and am waiting! Can't wait to see what you make
```

---
## \#897 Posted by: mishrasubhransu Posted at: 2019-04-18T20:06:34.323Z Reads: 169

```
@rpasichnyk I have a DieBieMS that metr pro can talk to.  Would you know why there is a discrepancy between the battery % and the battery full empty indicator? Is it because it's taking the % from DieBieMS but 3.0Volts is set as the minimum for the capacity box?

![Screenshot_20190418-054224|281x500](upload://cvo5l4pZAfFZ4ecR1R5wn45GqrM.png)
```

---
## \#898 Posted by: Darkie02 Posted at: 2019-04-19T16:55:20.935Z Reads: 167

```
Any news to when you might be selling this?
```

---
## \#899 Posted by: mishrasubhransu Posted at: 2019-04-22T21:41:30.045Z Reads: 162

```
How does the app deal with 2 modules on 2 separate boards? When I open the app now, I can see the all time stats. Now is that going to be separate for separate boards?
```

---
## \#900 Posted by: rpasichnyk Posted at: 2019-04-23T06:12:02.628Z Reads: 162

```
@Darkie02 soon™️

@mishrasubhransu when  you switch between different boards, all the settings and stats will automatically switch too
```

---
## \#901 Posted by: LEE Posted at: 2019-04-23T23:46:35.126Z Reads: 160

```
![image|256x499](upload://6utOH44f8KmQy98f8WshSGwH9pD.jpeg) 

Baud rate 115200
FOCBOX Unity ver.23.43
iOS12.2

BT is connected but can not get data.
I uninstalled the app several times and deleted the BT, but the symptoms do not change.
Help me!😭
```

---
## \#902 Posted by: pookybear Posted at: 2019-04-24T00:09:30.698Z Reads: 149

```
Under App

Is ppm and uart enabled?
```

---
## \#903 Posted by: LEE Posted at: 2019-04-24T00:14:53.570Z Reads: 155

```
Yes it is enabled.
ppm and UART.
HM-10, eSkateVESC and Unity23.42.
There was no problem with this combination.
```

---
## \#904 Posted by: pookybear Posted at: 2019-04-24T00:17:43.763Z Reads: 155

```
Make sure your metr app and BT module is up to date.
```

---
## \#905 Posted by: LEE Posted at: 2019-04-24T00:20:42.909Z Reads: 163

```
![image|690x290](upload://gjkp761Oi3R10OfBYUoySLzSwP7.jpeg) 
The module was bought last month.  There are two, but both have the same symptoms.
The green and blue LEDs are on and not blinking.
```

---
## \#906 Posted by: pookybear Posted at: 2019-04-24T00:23:35.300Z Reads: 152

```
I assume your BT module is also up to date? If it is, could be your uart port that's defective?
```

---
## \#907 Posted by: pookybear Posted at: 2019-04-24T00:24:30.364Z Reads: 155

```
Based on my personal experience, the only time my metr doesn't show any numbers is when it needs to be updated.
```

---
## \#908 Posted by: LEE Posted at: 2019-04-24T00:28:34.964Z Reads: 156

```
As we were able to acquire data with Unity 23.42 and HM-10 and eSkate VESC, it is unlikely that there is a problem with the UART.
However, this also seems to be incompatible with the version from Unity 23.43.
```

---
## \#909 Posted by: pookybear Posted at: 2019-04-24T00:35:16.672Z Reads: 155

```
Well if you feel adventurous, you could downgrade to a working unity version to confirm this but I highly recommend inquiring unity folks about this to make sure you don't "brick" your unit.

Good luck.
```

---
## \#910 Posted by: LEE Posted at: 2019-04-24T02:47:24.972Z Reads: 162

```
![image|472x500](upload://l5VLnn3BRIJPQvB6qpXAlQjxkih.jpeg) 

With the help of @goldrabe, the firmware was found to be old.
Elementary mistakes.
I'm sorry to trouble.🙏
```

---
## \#911 Posted by: pookybear Posted at: 2019-04-24T02:49:31.919Z Reads: 155

```
Good for you! That usually happens when there's an update.
```

---
## \#912 Posted by: LEE Posted at: 2019-04-24T07:22:36.422Z Reads: 166

```
![image|230x500](upload://7g4W3lLoxKDVqZmhVZaLcENlcnE.jpeg) 
![image|230x500](upload://30AiOyvvY1KpcTSJBtq1Fm3OkGj.jpeg) 

I was able to connect.  Thank you!😆👍
```

---
## \#913 Posted by: Darkie02 Posted at: 2019-04-24T08:07:13.566Z Reads: 164

```
[quote="rpasichnyk, post:900, topic:57780"]
soon™️
[/quote]

🤔 Now with that response there’s no date to for any one complain about missing. How are we going to cope on forums with out bitching about things this is a catastrophe. your single handedly  GOING TO BRAKE THE INTERNET. Noooo 😭
```

---
## \#914 Posted by: hexakopter Posted at: 2019-04-24T21:17:12.611Z Reads: 164

```
[quote="Darkie02, post:913, topic:57780"]
your single handedly GOING TO BRAKE THE INTERNET.
[/quote]
:sweat_smile: :sunglasses:

https://giphy.com/gifs/eKCrMsVRbow2d2974s

![Metr_Pro_Unity|375x500](upload://47rOEAU1ADH8JnXHzpuVgUudppo.jpeg)
```

---
## \#915 Posted by: pookybear Posted at: 2019-04-24T23:17:58.512Z Reads: 161

```
Oh damn!!
10chat
```

---
## \#916 Posted by: murloc992 Posted at: 2019-04-25T10:17:11.847Z Reads: 160

```
![image|480x360](upload://nuPtmumXqn1VeTdPFsqpKQrkMi8.jpeg)
```

---
## \#917 Posted by: rey8801 Posted at: 2019-04-25T10:57:25.950Z Reads: 158

```
I waited years before buy a metr. Now I am using Unity, just got the metr pro today and the unity version is out :man_facepalming: Brilliant :sweat_smile:
![IMG_20190425_125452|281x500](upload://w0I8NIe8hBfy5NZT9tEoijA26B8.jpeg)
```

---
## \#918 Posted by: murloc992 Posted at: 2019-04-25T11:01:43.263Z Reads: 157

```
If you are in EU I might be interested in one. :wink:
```

---
## \#919 Posted by: FredXanadu Posted at: 2019-04-25T11:19:19.090Z Reads: 158

```
i sold mine yesterday :slight_smile:
```

---
## \#920 Posted by: rpasichnyk Posted at: 2019-04-25T11:31:46.340Z Reads: 158

```
You shouldn't be disappointed :slight_smile: We still have no final date / price for Unity version, it can take some weeks. Enjoy your Metr Pro while the weather is awesome ;)
```

---
## \#921 Posted by: rey8801 Posted at: 2019-04-25T11:34:12.310Z Reads: 160

```
I ma not disappointed with you :grin: It was just to laugh a bit with @pookybear about it. No problem I will try to use the internal UART port.
@murloc992 thanks but I wiil probably keep it. You better buy it from the website. It takes around 1 week to get to your place :wink:
```

---
## \#922 Posted by: Gerrycorrado Posted at: 2019-04-25T13:05:58.038Z Reads: 159

```
Instead of me shipping in my broken (by "ourselves") Metr Pro, i better wait for this one then haha (I have 1 legacy board left running non unity, but that is ticking on its lasts breaths too until when I get another Unity shipment in)
```

---
## \#923 Posted by: MikeDIY Posted at: 2019-04-25T14:22:43.051Z Reads: 160

```
Nood here :sweat_smile:

Will this bind up with my heltec loRa32 V2 ore ttgo loRa32 v2 ? :pray:
```

---
## \#924 Posted by: hexakopter Posted at: 2019-04-25T17:45:54.182Z Reads: 158

```
@MikeDIY When I got your question right, no it will not work. Your stated modules are not Bluetooth based.
```

---
## \#925 Posted by: MikeDIY Posted at: 2019-04-25T17:48:29.539Z Reads: 157

```
:sweat_smile::grinning:  Now i'am confuced :nerd_face:

http://www.heltec.cn/project/wifi-lora-32/?lang=en
```

---
## \#926 Posted by: hexakopter Posted at: 2019-04-25T18:00:05.541Z Reads: 153

```
Ok, looks like I found the wrong module... :sweat_smile: 
The Metr Pro modules are meant to pair to a computer or phone (iOS or Android) running the [Metr App](https://metr.at) or any other VESC communication app.
But when you want to challenge yourself and program a functioning code for the heltec module feel free to do it.
```

---
## \#927 Posted by: Rotko Posted at: 2019-04-27T15:11:35.102Z Reads: 152

```
Hi, 

Setting:
Metr pro,
Ackmaniac 3.102,
Huawei Honor 8 Adroid 8.0,
2x focbox

Problem:

App finds the module but doesn't ask for the pairing code. Blue led stays on while green led flashes.
I can connect the module to the device (app says so) but no telemetry datas are exchanged.
Any suggestions?
```

---
## \#928 Posted by: visnu777 Posted at: 2019-04-27T15:20:51.056Z Reads: 155

```
Afair you have to bind it with android, there you have to use the pin. After that you can easily connect it.
```

---
## \#929 Posted by: pookybear Posted at: 2019-04-27T16:14:54.111Z Reads: 160

```
This happened to me too. What I did was I paired it the first time w the ack app. It prompted me for the code. But for some reason it didn't work. I couldn't even pair it w metr app after that.

Here's what I did to fix it:
* Uninstall both apps
* Delete metr under phone system Bluetooth settings. (important step)
* Install metr app first
* Pair metr BT module using the metr app
* Type code 
* Confirm BT is connected successfully 
* Exit metr app
* Install ack app. It should not ask for the code since you have already inputted it. The phone system remembers it.
* Find BT module and connect.

As far as I know, this module does not support concurrent connections. Meaning you can't have both app open. One app needs to be closed/exited first to be able to use the other. 

Hopefully, this helps you.
```

---
## \#930 Posted by: Rotko Posted at: 2019-04-28T10:45:03.251Z Reads: 157

```
Thanks, 
I updated to Ackmaniac 3.103 and followed step by step your suggestions.
This time I was asked for the pairing code, green "+" on realtime screen but for the rest the screen shows a compilation of 0, app doesn't get any data from my vescs. 
Same behaviour with Ackmaniac app, it connects but doesn't get any datas. :disappointed_relieved:
```

---
## \#931 Posted by: pookybear Posted at: 2019-04-28T13:52:55.802Z Reads: 158

```
Edit:

Check for updates on metr. If there is, update the app as well as the module's firmware.
```

---
## \#932 Posted by: gmurad Posted at: 2019-04-28T14:52:30.722Z Reads: 162

```
You and me both! Just received 2 Metr Pros last week for future builds using Unity.... Did the metr team consider just making an adapter instead of a new module? Not sure what are the constraints there.

Hopefully someone will come up with a more streamlined way to use the internal UART port in the Unity. I want to use a Metr pro and a DaveGA at the very least and maybe a custom remote in the future(seems like you can't have more then 2 devices tho)

2018/2019 seems to be a year where a lot of "telemetry" options are available, I feel that the ecosystem as a whole has a lot of redundant efforts going on, imagine the same build using Metr pro, DaveGA and one of the Firefly variant remotes... It would be amazing is this was standardized in some way where you can get all of it in 1 solution.
```

---
## \#933 Posted by: trampa Posted at: 2019-04-28T19:32:16.111Z Reads: 156

```
Technically one NRF 51/52 module is enough
To get telemetry, connect to VESC-Tool and run a remote controller connection simoultaniously. 
The VESC code base is open source for a reason. Redundant module instalation is sort of silly from a technical point of view. If you start to run out of uart ports, you should ask yourself why that is the case.
```

---
## \#934 Posted by: gmurad Posted at: 2019-04-28T23:37:21.790Z Reads: 161

```
I totally agree and that's the point I'm making. I wonder what it will take to standardize or to reduce redundancy of the solutions. Metr is not open source but I feel it's the closest "entity" that could expand their efforts to provide an onboard telemetry screen and then eventually a remote controller receiver, a headlight/breaklight controller all in one pcb.
```

---
## \#935 Posted by: trampa Posted at: 2019-04-29T09:45:40.759Z Reads: 165

```
[quote="gmurad, post:934, topic:57780"]
I feel that the ecosystem as a whole has a lot of redundant efforts going on, imagine the same build using Metr pro, DaveGA and one of the Firefly variant remotes… It would be amazing is this was standardized in some way where you can get all of it in 1 solution.
[/quote]

The modules are pretty standard, it is a matter of the software/FW and/or purposely built in software locks. Technically there is no reason why a random NRF 51/52 module shouldn't be able to connect to your Phone/App, telemetry device, remote etc. 
You end up using two or more nearly identical BLE Modules for no other reason than a business strategy (e.g. Software only works with the hardware I sold you, UUID locked). 

We will try our best to offer FW updates for the Open Source-based NRF modules via VESC-Tool and we will bang on remote controller and telemetry solutions that work with a wide range of NRF modules available today. The idea is that you will only need one module and keep it updated FW wise. Benjamin Vedder spent quite some time on coding a FW that allows to use **one module** for **many purposes**, so that you can have a remote controller connection, VESC-Tool connection and telemetry at the same time via the same NRF module that can be upgraded via the VESC. 

In other words: **It is there already.** 

All you need is a open source NRF module solution and cheap small android skate phone in your pocket or strapped to the board.
```

---
## \#936 Posted by: taz Posted at: 2019-04-29T11:46:28.943Z Reads: 159

```
Any ETA on the new nrf based remotes?
```

---
## \#937 Posted by: drone001 Posted at: 2019-04-30T00:02:34.920Z Reads: 155

```
is it done yet....
is it done yet....
is it done yet....
is it done yet....
is it done yet....
is it done yet....
```

---
## \#938 Posted by: xsynatic Posted at: 2019-04-30T00:27:34.296Z Reads: 156

```
So is it worth it?

And did i get it right - I can program the whole VESC on the go and i can even program different speed modes and activate them via Smartphone. Even with the TB Vesc 410 (4.12)?
```

---
## \#939 Posted by: hexakopter Posted at: 2019-04-30T09:07:06.138Z Reads: 163

```
[quote="Rotko, post:927, topic:57780"]
Blue led stays on while green led flashes. I can connect the module to the device (app says so) but no telemetry datas are exchanged. Any suggestions?
[/quote]


Green LED flashing means that no UART connection is detected. Makes sure that you enable UART output of your VESC. You will see the green LED going solid when a UART connection is established which is necessary to receive data.
When I remember correctly some people reported that they have trouble with Ackmaniac 3.103 firmware so staying on 3.102 is maybe a good idea.

[quote="xsynatic, post:938, topic:57780, full:true"]
So is it worth it?

And did i get it right - I can program the whole VESC on the go and i can even program different speed modes and activate them via Smartphone. Even with the TB Vesc 410 (4.12)?
[/quote]
I would say it is worth it. :smile: Yes, you can program your VESC on the go, program different speed modes and activate them via smartphone and log all your rides via smartphone. Do you have a link to that hardware to be sure it is working? When it is VESC based (from the name it sound its based on the HW4.12) and has a UART port available it will work fine.
```

---
## \#940 Posted by: xsynatic Posted at: 2019-04-30T09:22:31.024Z Reads: 151

```
Well that sounds great.

The VESC i use is from torqueboard

[Product link](https:///products/torque-esc-bldc-electronic-speed-controller)
```

---
## \#941 Posted by: hexakopter Posted at: 2019-04-30T09:30:04.192Z Reads: 153

```
That's the normal VESC HW4.12 so it will work.:+1:
```

---
## \#942 Posted by: oyta Posted at: 2019-05-01T19:44:09.912Z Reads: 163

```
![image|290x500](upload://A7HhwuhUuaHoOXGtvxffvYY6JH5.jpeg) 

@rpasichnyk - I might be wrong about this, but I tried to understand. Look at the next post as well.
 
Not tried this before - but wanted to get the latest VESC FW on the VESC, which I believe is 3.55. Metr says I am up to date with version 3.39. Sholdn’t I be able to update to the newest version?
```

---
## \#943 Posted by: oyta Posted at: 2019-05-01T20:21:56.683Z Reads: 164

```
![image|281x500](upload://4L9BaMqrAEhbJN6NgPp7QoIpHfx.jpeg) 

So I am not sure what the log says, of course. But I am guessing :slight_smile: It may look like it is comparing the available VESC version 3.55 with the installed Metr Pro version 3.69? I could absolutely be misinterpreting this 😬
```

---
## \#944 Posted by: Rotko Posted at: 2019-05-02T06:55:22.518Z Reads: 159

```
Exactly, I thougt I had enabled PPM and Uart as the first thing but I didn't. Forgot to save the settings. My bad.
With 2x Focboxes and Ackmaniac 3.102 (didn't try 3.103) now works like a charm. Thank you.
```

---
## \#945 Posted by: xsynatic Posted at: 2019-05-02T08:54:54.709Z Reads: 157

```
Another thing. Benjamin veddar pointed out that he uses a 9$ Bluetooth module from aliexpress and published to corresponding code for it.

Would you say go for a plug and play but more expensive or diy but cheap.
```

---
## \#946 Posted by: bsb Posted at: 2019-05-02T20:28:31.969Z Reads: 162

```
Is there some documentation available about the android app? What happens or ought happen, when i press "upload" e.g.? Should i get a link?
```

---
## \#947 Posted by: sofu Posted at: 2019-05-04T05:13:43.596Z Reads: 165

```
@hexakopter @rpasichnyk I'm having this interesting issue with one of my modules. I can connect to it but I can't update the firmware on it. The app says installed firmware is 3.63 and that the module is up to date, but the latest firmware is 3.69 I believe. When the module turns on it flashes red once then the red turns off. I guess this is because it can't read the Unity. I did make sure the baud rate and uart output is turned on, but I think the unable to update firmware issue may be something else?
```

---
## \#948 Posted by: rey8801 Posted at: 2019-05-04T06:42:24.037Z Reads: 168

```
Guys. I am sure it's me, but new to Metr module. So I connected it to Unity. Baud rate 115200 (I think metr deal with TX, RX and baud rate alone). I get connected but no data. Something missing in the setting?

![app|281x500](upload://qPJSqxOggY5Kat7hqfn06uARuBy.png)
```

---
## \#949 Posted by: oyta Posted at: 2019-05-04T06:47:15.024Z Reads: 164

```
I had the same issue - see my two posts above. Seems like the version check has a bug? I manually updated the FW on my VESC 6.0 through USB for now though.
```

---
## \#950 Posted by: pookybear Posted at: 2019-05-04T06:52:22.118Z Reads: 163

```
Update firmware.
```

---
## \#951 Posted by: rey8801 Posted at: 2019-05-04T06:53:29.044Z Reads: 171

```
I have this firmware installed
![app|281x500](upload://idzxM4ADm9rsuxznHyuFX5pOVNF.png)
```

---
## \#952 Posted by: sofu Posted at: 2019-05-04T06:54:23.399Z Reads: 164

```
This is exactly the situation I have. Latest unity firmware and 3.63 on the Metr. Says latest Metr firmware installed but that's not true.
```

---
## \#953 Posted by: rey8801 Posted at: 2019-05-04T06:55:17.435Z Reads: 163

```
I am using Unity maybe that's the reason. I thought let's get installed and go for a ride.... Nope :sweat_smile:
```

---
## \#954 Posted by: pookybear Posted at: 2019-05-04T06:58:36.359Z Reads: 165

```
That's probably why. I'm on vesc6
```

---
## \#955 Posted by: rey8801 Posted at: 2019-05-04T07:04:58.515Z Reads: 165

```
I mean I thought it's compatible. This is the only reason why I got metr. Otherwise I would have kept my cheap hm10
```

---
## \#956 Posted by: pookybear Posted at: 2019-05-04T07:11:52.579Z Reads: 162

```
I'm sure the metr guys will have a fix soon. When I had my unity, it was flawless.
```

---
## \#957 Posted by: Nubasaurus Posted at: 2019-05-05T01:13:11.872Z Reads: 165

```
Metr page down?

Can’t seem to upload records. Log shows 

Documents/19-05-04-13-32-36-37.r', points=20033

[E 18:09:39.440] Login failed, err=Error: SSL handshake failed

[I 18:10:16.879] [records] exit

[I 18:10:16.899] [settings] enter
```

---
## \#958 Posted by: rpasichnyk Posted at: 2019-05-05T04:28:04.271Z Reads: 161

```
@Nubasaurus thanks, letsencrypt certificate expired and that’s why nothing was working properly :sweat_smile:  It is now fixed

@sofu @rey8801 please try again, you’re right, 3.69 is the latest. The server was down :arrow_up: 

@oyta VESC firmwares have some small issues and the latest is not available yet to update via Metr app. In more detail, now it generates a random CAN ID based on STM UUID. This was not the case before, where people used to have CAN IDs 0, 1, 2, etc. Because of it settings fail to restore after update and I consider the experience as not acceptable. I will fix this and VESC firmware updates will be available through the Metr app again
```

---
## \#959 Posted by: rey8801 Posted at: 2019-05-05T06:20:23.194Z Reads: 162

```
Yes it works. Thanks!
```

---
## \#960 Posted by: hexakopter Posted at: 2019-05-05T19:34:17.467Z Reads: 170

```
[quote="Rotko, post:944, topic:57780, full:true"]
Exactly, I thougt I had enabled PPM and Uart as the first thing but I didn’t. Forgot to save the settings. My bad. With 2x Focboxes and Ackmaniac 3.102 (didn’t try 3.103) now works like a charm. Thank you.
[/quote]


No problem. I am glad that it is working for you now.:smiley:

[quote="xsynatic, post:945, topic:57780"]
Would you say go for a plug and play but more expensive or diy but cheap.
[/quote]
I would go with the Metr Pro module. Maybe a bit biased because I am involved in it.:sweat_smile:

[quote="bsb, post:946, topic:57780"]
What happens or ought happen, when i press “upload” e.g.? Should i get a link?
[/quote]
When you are talking about your recordings, then yes you will get a link when you press the "Upload" button.
```

---
## \#961 Posted by: rey8801 Posted at: 2019-05-07T09:15:11.838Z Reads: 167

```
Hi, question. there is specific setting to apply to show correct data from the Unity? Meaning energy consuption ecc... since unity is actualy a dual vesc but with some shared parts so not sure how the software will work with it.
Maybe @sofu you have tested already and you know. I guess it's all about this setting page.

![app|281x500](upload://1D9XkJwAj7GFo75v0bp761Notsv.png) 

Ah last thing with motor poles do they mean the stator poles or number of magnets as for other software?
Thanks!
```

---
## \#962 Posted by: sofu Posted at: 2019-05-07T20:08:40.014Z Reads: 167

```
Measurements with one number are combined already and measurements that have two numbers are per motor. No settings to toggle. Here is some code from my Unity iOS app.

![image|643x500](upload://e3LRUVeDVRH96TTmnU7llboyZCt.png) 

You can see some stuff like motor temps are still split up but stuff like voltage, input current, etc are combined. Just trust in Metr, they automatically do the correct data display config.
```

---
## \#963 Posted by: rey8801 Posted at: 2019-05-07T20:10:48.269Z Reads: 170

```
Thank you for the explanation. Yes indeed I tried a small log today and it worked OK except my phone loosing GPS. Ow changed permission and the ride was ok.

https://metr.at/r/dbmPA
```

---
## \#964 Posted by: bevilacqua Posted at: 2019-05-08T15:12:39.550Z Reads: 164

```
@rpasichnyk Roman, I got a Batch-3 Diebiems, do I need a specific VESC-FW to make it work with metr-pro?

EDIT: Swapped CL-CH and now it works :sweat_smile: 

Any chance to implement live data of the Cell-Temperature(s)? :pray:
```

---
## \#965 Posted by: xsynatic Posted at: 2019-05-09T16:57:56.818Z Reads: 165

```
Can Somebody explain to me whats the difference between the Metr Pro and lets say the Flipsky Bluetooth Module?
```

---
## \#966 Posted by: rpasichnyk Posted at: 2019-05-09T16:58:45.168Z Reads: 163

```
Flipsky Bluetooth module does not work with Metr app
```

---
## \#967 Posted by: xsynatic Posted at: 2019-05-09T16:59:52.414Z Reads: 161

```
But with other VESC Apps?

EDIT: The problem is that i can't see the value in using the metr App compared to the vesc app or other if the functionality is the same? Or am i missing something?
```

---
## \#968 Posted by: rpasichnyk Posted at: 2019-05-09T17:25:45.489Z Reads: 165

```
Even if you are not using Metr app, you still get more benefits with Metr Pro:

* Encrypted bluetooth communication protected with PIN - only you can connect to your board
* Antenna for better signal
* Direct BLE connection from your Desktop computer

And you really want to try Metr app, because it has a lot of goodness!:heart:
```

---
## \#969 Posted by: Jc06505n Posted at: 2019-05-09T17:26:20.492Z Reads: 170

```
[quote="xsynatic, post:967, topic:57780"]
EDIT: The problem is that i can’t see the value in using the metr App compared to the vesc app or other if the functionality is the same? Or am i missing something?
[/quote]


Arguably Better Data Presentation and exportation, faster compatibles updates allowing the module to be used with vesc that don't follow the main VESC code (FocBox Unity) , protection pin,  and and ios application.
```

---
## \#970 Posted by: nirurin Posted at: 2019-05-12T04:27:02.094Z Reads: 164

```
I've read through a bunch of this thread, but before ordering I wanted to check a couple of things to see if this might work as a solution for me. 

I'm in the process of looking for a LCD screen to wire up to my bms, so that I can see my current battery level while riding, as well as monitor my battery while charging so I can make sure it's charging up to the correct voltages etc. Is the data from the Metr via the vesc able to provide accurate (or at least fairly accurate for my needs) voltage info even while charging? (I believe it can from what a couple people said, but I wanted to be sure before I invested). 

Also, are there currently any small board-mountable screens that people have used to display the data? If not, I'd be tempted to attempt something, it would seem all it would need is an android-powered touchscreen...
```

---
## \#971 Posted by: amazingdave Posted at: 2019-05-12T06:09:54.766Z Reads: 165

```
Have a look at this...

https://www.electric-skateboard.builders/t/davega-battery-monitor-odometer-speedometer/71509
```

---
## \#973 Posted by: nirurin Posted at: 2019-05-12T16:10:40.218Z Reads: 165

```
Yeh I had already looked at that, but from what the thread says there’s not currently any kits available, and it requires a bunch of soldering and programming arduino to get it working. Unless I buy the Flipsky clone, but I can 3d print my own enclosures for a lot less than they’re charging. The thread also doesn’t seem to say how it wires in, I assume it uses the same comms port though which means I wouldn’t be able to have both options, and having the gps and map tracking etc through the android apps gives me a lot more options.

I may be wrong on all of this, as I’ve not actually used either of these units lol. Just going by what the threads tell me.

Edit:
The Dual VESC I'm getting seems to have 3 communication ports, but as far as I can tell from what people on here say I need to use one specific port for these things to work? So I couldn't have both Metr and Davega working at the same time?
```

---
## \#974 Posted by: MiniChopper4Me Posted at: 2019-05-12T19:10:26.508Z Reads: 163

```
My understanding is that you can connect Metr into one VESCs UART port, and DaVeGa into the other VESCs UART port.  Metr allows you to see the data from both VESCs, while DaVeGa takes the data from the VESC it is connected to and multiplies it x2 where appropriate.  The VESCs talk to each other over the CAN bus, which is a different connector.  CAN bus is what you use if you get a DieBieMS, and that bus supports connecting multiple devices in parallel.

Where can you run into trouble? If you want to use a Metr, DaVeGa, and a Photon.  Those all use UART.
```

---
## \#975 Posted by: pookybear Posted at: 2019-05-13T02:48:03.485Z Reads: 175

```
I'm trying to change a value under "expert". 

Steps:
* Typed ramp on search bar
* Hit Read. Values show up
* Looked for PPM POS ramp
* Switched from 0.2 to 0.1
* Hit write.

App would try to write then it would give me signature check failed.

* Vesc 6
* Ack 3.102 modded firmware (brake fix) [This](https://www.electric-skateboard.builders/t/vesc-based-controllers-brakes-locking-at-low-speed-for-larger-wheels-in-foc-possible-unity-fix/73547/155) one.

Edit:
Do I need to turn on "untested firmware"? ESC beta firmware is on when trying to do the above but still failing.
```

---
## \#976 Posted by: rpasichnyk Posted at: 2019-05-13T05:34:26.582Z Reads: 172

```
No, do not change any settings in the Magic section. Please repeat the test and send your Settings -> Show Logs file to support@metr.at :+1:
```

---
## \#977 Posted by: pookybear Posted at: 2019-05-13T05:51:34.553Z Reads: 172

```
Will do.  10 char
```

---
## \#978 Posted by: pookybear Posted at: 2019-05-13T07:24:15.875Z Reads: 175

```
Error log sent.
```

---
## \#979 Posted by: Darkie02 Posted at: 2019-05-13T08:20:17.993Z Reads: 180

```
[quote="hexakopter, post:914, topic:57780"]
![Metr_Pro_Unity|300x400](https://www.electric-skateboard.builders/uploads/db1493/optimized/3X/1/c/1ce03f55a32a3fe0df69dfcdae20aa0226a97682_2_375x500.jpeg)
[/quote]


Any update on theses Unity Metr Pro’s or when thay might be for sale?

@hexakopter @rpasichnyk?
```

---
## \#980 Posted by: hexakopter Posted at: 2019-05-13T13:08:08.493Z Reads: 174

```
@Darkie02 There are some delivery delays regarding some parts. I can not guarantee, but I am pretty confident that we should get all missing parts before end of this month.
So I think the Metr Pro UNITY modules will be for sale around end of May/ early June.:grinning: 
Ready to be shipped next day when they hit the store.:blush:
```

---
## \#981 Posted by: nirurin Posted at: 2019-05-13T23:28:39.720Z Reads: 169

```
I thought the Metr Pro modules were designed to be universally compatible with every VESC? Is it only unity that requires a special module? I'm planning to get one of the new flipsky 4.20 duals, will this work with a standard Metr Pro?
```

---
## \#982 Posted by: kalebludlow Posted at: 2019-05-14T00:50:14.891Z Reads: 174

```
The Unity module is designed to be used on the internal UART port that is currently used by the stock bluetooth module. Your FSESC 4.20 Dual will work with the regular Metr Pro
```

---
## \#983 Posted by: rpasichnyk Posted at: 2019-05-15T19:43:42.001Z Reads: 177

```
We are pushing updates at a fast pace. The newest Metr app v3.6.3 landed to the Apple App Store and Google Play Store. Bug reports are being submitted (thank you!) and bugs are being fixed🤓

The latest VESC firmware v3.56 is now fully supported. And even ancient v2.18 firmware received quality fixes recently because some people are still using it :skull: 

![C65DD7D0-01D7-45B2-A636-9E653CFEA8A5|500x500](upload://lEPkzI5AeAuM5p8wtaawR1enfXM.jpeg) 

Metr Pro UNITY is on the way. Original Metr Pro is still our most important module and will receive firmware updates and be supported for long time :v:

![IMG_4010|577x500](upload://pmiEahg9VswMcYy7eS3ATSpQzze.jpeg) 

Android Q Beta on Pixel 3 is under testing. We are using bleeding edge tech here!

More cool stuff coming up🤓 This summer is going to be hot!
```

---
## \#984 Posted by: McErono Posted at: 2019-05-15T21:42:55.887Z Reads: 169

```
I have a metr pro in one of my boards and love just everything about it.

But I do not quite understand the unity metr module I think. Seeing bioboards using normal metr pro modules with their unitys what exactly is the benefit of a special unity module besides being integrated inside the unity?

Does the Enertion unity app still work beside the metr app?
```

---
## \#985 Posted by: caustin Posted at: 2019-05-15T22:21:09.621Z Reads: 170

```
Main benefit I see if freeing up the external UART port for use other than Metr Pro.  If that is not an issue (ie Proton remote or DAVEga), then normal Metr Pro works fine.
```

---
## \#986 Posted by: xsynatic Posted at: 2019-05-15T23:30:28.708Z Reads: 172

```
Where are you guys shipping from? Is Germany still on the 12€ fee?
```

---
## \#987 Posted by: rpasichnyk Posted at: 2019-05-16T04:19:34.433Z Reads: 175

```
The benefit of the Metr Pro UNITY is that it fits so well into the UNITY. You just pull out the built-in BLE module that comes with the UNITY and put Metr Pro instead:

https://giphy.com/gifs/eKCrMsVRbow2d2974s

[quote="caustin, post:985, topic:57780"]
freeing up the external UART port for use other than Metr Pro
[/quote]

And this is exactly the other benefit (more important one :slight_smile:) Otherwise it's the same Metr Pro (almost :wink: )! And you can even use it with all other VESCs - it will work just fine.

@xsynatic we ship from both Sweden and Germany. Me and @hexakopter have tight schedules and help each other wish shipping to supply you all with the modules in a timely manner :kissing_heart:
```

---
## \#988 Posted by: McErono Posted at: 2019-05-16T10:08:31.683Z Reads: 172

```
[quote="rpasichnyk, post:987, topic:57780"]
And you can even use it with all other VESCs - it will work just fine.
[/quote]

Didn't realize that! Cool!
```

---
## \#989 Posted by: rey8801 Posted at: 2019-05-16T10:25:41.664Z Reads: 176

```
Me neither! Damn it! :rofl:Well in case I have one not open metr pro from 2 weeks ago available for trade

EDIT: Meaning change it for an Unity one which will probably never happen since they are not released yet :sweat_smile:
```

---
## \#991 Posted by: niuva Posted at: 2019-05-16T16:58:31.690Z Reads: 175

```
Exited for the Unity module!
How about the reported Unity bluetooth module crashes on voltage spikes. Have you taken this into consideration?
https://www.electric-skateboard.builders/t/focbox-unity-official/64944/2592?u=scream

Anyway - can't wait to get my hands on one!
```

---
## \#992 Posted by: Balth81 Posted at: 2019-05-18T09:24:05.718Z Reads: 170

```
I just got my Metr Pro paired it to my unity and it’s only showing one motors amps?? I can’t seem to work it out re ran motor detection and sensors showing fine?
```

---
## \#993 Posted by: gmurad Posted at: 2019-05-19T12:19:08.540Z Reads: 174

```
Are you able to help/facilitate an adapter for the people that bought Metr Pro modules to use with the Unity before this dedicated version came out? I bought 2 of them. 
Seems to me that an adapter to plug normal metr pros into the special unity port would be very good for customers. (Instead of having to buy a brand new adapter)

Is it technically feasible? Would it require changes to to Metr pro firmware to make it work with those pins?
```

---
## \#994 Posted by: rey8801 Posted at: 2019-05-19T12:32:30.562Z Reads: 172

```
That would be great. I also recently got 2 metr pro that will go with Unity only.
```

---
## \#995 Posted by: xsynatic Posted at: 2019-05-19T15:48:12.857Z Reads: 170

```
Is it possible to programm a Cruise Control with the metr pro? vesc 4.12
```

---
## \#996 Posted by: Balth81 Posted at: 2019-05-20T12:19:35.865Z Reads: 178

```
@hexakopter has there been a change to the unity firmware which makes the metr no longer able to display both motors amps? No matter what I try I can’t get it working?![image|231x500](upload://qkNfkfHOd433L98C6LRbYcs9yjC.jpeg) ![image|231x500](upload://3x27Fr8w1mb0Up1uXWkLisKgoCh.jpeg) ![image|231x500](upload://ifuHitQLUbjFfC1i0coLs0iYWCL.jpeg)
```

---
## \#997 Posted by: sayekim Posted at: 2019-05-20T12:59:11.548Z Reads: 166

```
Do the batt amps display for both?

It might be the sensor itself that is at fault.
```

---
## \#998 Posted by: rpasichnyk Posted at: 2019-05-20T13:09:00.470Z Reads: 165

```
It’s a bug in the app, not in the firmware. We are working on it. Thx for the heads up!
```

---
## \#999 Posted by: Balth81 Posted at: 2019-05-20T13:54:28.762Z Reads: 162

```
@rpasichnyk thanks Roman I will keep an eye out for an updated version :) any eta?
```

---
## \#1000 Posted by: xsynatic Posted at: 2019-05-20T14:14:49.689Z Reads: 161

```
Any info on the cruise control Question i asked?
```

---
## \#1001 Posted by: bevilacqua Posted at: 2019-05-20T14:50:19.766Z Reads: 163

```
metr is not a remote, it logs telemetry, therefore no

You would need to get a remote that can do CC. Alternatively, I think that the mini-remote in combination with Ackmaniacs watt-control can do CC too.
```

---
## \#1002 Posted by: xsynatic Posted at: 2019-05-20T15:24:55.905Z Reads: 162

```
yeah thought so. Thats why i asked because speed modes are programmable too
```

---
## \#1003 Posted by: bevilacqua Posted at: 2019-05-20T15:29:07.304Z Reads: 160

```
Speed modes basically change the settings of your vesc. CC is more complicated than that since you have to control the vesc with a static PPM or change to PID-ccontrol
```

---
## \#1004 Posted by: Xenon Posted at: 2019-05-20T16:30:44.546Z Reads: 155

```
hi, is it possible to delete the standard boot modes?
My problem is that I want to use the metr.pro on a new vesc but the module sets after each reboot again and again all the values of the old vesc.
```

---
## \#1005 Posted by: rpasichnyk Posted at: 2019-05-20T18:58:54.330Z Reads: 155

```
Click on the 3 dots in Modes Tab -> Clear Startup Mode
```

---
## \#1006 Posted by: Xenon Posted at: 2019-05-20T19:23:15.417Z Reads: 161

```
 Thanks now it works.
```

---
## \#1007 Posted by: hexakopter Posted at: 2019-05-21T11:39:10.988Z Reads: 165

```
[quote="gmurad, post:993, topic:57780"]
Are you able to help/facilitate an adapter for the people that bought Metr Pro modules to use with the Unity before this dedicated version came out? I bought 2 of them. Seems to me that an adapter to plug normal metr pros into the special unity port would be very good for customers. (Instead of having to buy a brand new adapter)

Is it technically feasible?
[/quote]
I am sorry, but we will not sell an adapter that connects the standard Metr Pro module to the special internal UNITY port. As already said a while back (https://www.electric-skateboard.builders/t/metr-pro-next-gen-bluetooth-module/57780/604) it would be needed to cut a hole in the UNITY’s orange silicone case to have the space for the wires soldered to the 2.0mm 6pin pinheader you would plug into that port. The hole is also needed because there is no space inside the UNITY case for the standard Metr Pro module, so you need the wires to go outside the silicone case. I would also recommend glueing the adapter to the port so you don’t have trouble with a loose connection.

So it is technically feasible, but I think it is more a „dirty hack“ for DIY people than something that we want to sell. But feel free to build an adapter yourself and we will try our best to help you with upcoming questions and support the DIY spirit.:grinning:

[quote="gmurad, post:993, topic:57780"]
Would it require changes to to Metr pro firmware to make it work with those pins?
[/quote]

With an upcoming Metr Pro firmware update it will be possible to use the internal UNITY port without a special firmware for the UNITY itself.
```

---
## \#1008 Posted by: gmurad Posted at: 2019-05-21T11:42:15.356Z Reads: 166

```
[quote="hexakopter, post:1007, topic:57780"]
With an upcoming Metr Pro firmware update it will be possible to use the internal UNITY port without a special firmware for the UNITY itself.
[/quote]

Thanks, this would be enough for me. Looking forward to this update.
```

---
## \#1009 Posted by: Pimousse Posted at: 2019-05-21T11:55:12.760Z Reads: 165

```
Hi @rpasichnyk,
We updated @Manu39 's VESCs to latest FW 3.57.
On my side, no problem, but he bricked his VESC (the one connected to Metr Pro) when he applied a mode.

Unfortunately we couldn't use the other one to reprogram it (since Vedder added the Black Magic probe for SWG prog a bricked VESC with a working one).
So a STLink is on its way to him.

I'm really confused with the mode system. I already bricked a VESC the same way (that was with the old Metr module and a cheap Android phone).
I assume that needs to be fixed mostly on the FW side but cuold you have a look ?
```

---
## \#1010 Posted by: rpasichnyk Posted at: 2019-05-21T12:07:00.831Z Reads: 164

```
Yes, we can have a look. It would be really helpful to have a log file every time you report such a problem :+1:
```

---
## \#1011 Posted by: Pimousse Posted at: 2019-05-21T12:21:01.436Z Reads: 160

```
Sure !
I asked @Manu39 for it.
```

---
## \#1012 Posted by: Manu39 Posted at: 2019-05-22T06:51:21.831Z Reads: 161

```
Hey @rpasichnyk 
I sent you the LOG as a private message in the hope that it would help you.
Thank you. Thank you.
Manu
```

---
## \#1013 Posted by: Mainsedora Posted at: 2019-05-22T18:50:20.289Z Reads: 167

```
I have succesfully paired my metr pro with my pc, but I don’t know how to do it in the vesc tool.
```

---
## \#1014 Posted by: bevilacqua Posted at: 2019-05-22T20:05:06.743Z Reads: 163

```
windows? Linux? or mac?
```

---
## \#1015 Posted by: Mainsedora Posted at: 2019-05-22T20:05:51.845Z Reads: 167

```
Windows is my way
```

---
## \#1016 Posted by: bevilacqua Posted at: 2019-05-22T20:07:11.065Z Reads: 171

```
I think Vedder did not implement it for Windows, only Linux. MAC works thanks to @rpasichnyk, but I might be wrong and it has been implemented by now. 

Try TCP-bridge
```

---
## \#1017 Posted by: Mainsedora Posted at: 2019-05-22T20:09:11.686Z Reads: 169

```
It's mentioned in the first post. TCP Bridge is the odd way, I think.
```

---
## \#1018 Posted by: bevilacqua Posted at: 2019-05-22T20:11:40.330Z Reads: 162

```
its plenty fast with metr pro
```

---
## \#1019 Posted by: Mainsedora Posted at: 2019-05-22T20:17:24.323Z Reads: 168

```
btw I'm running on FW 3.56 on a Flipsky VESC 6.6. Should not be a problem though. But if it's not compatible for windows as clearly stated, then I have to run a linux vm or on a rpi3, what is flying around here. That sucks.
```

---
## \#1020 Posted by: rpasichnyk Posted at: 2019-05-23T05:47:20.797Z Reads: 177

```
Long story short: it's complicated between Vedder and Apple / Microsoft. But when compile VESC Tool with Microsoft compiler, it works pretty well including BLE.

You can grab the latest one here
https://github.com/rpasichnyk/vesc_tool/releases/tag/v1.13

Pair Metr Pro in Windows 10 first using System Settings


![Untitled|690x427](upload://wxJY0Kp0oebFJa7eHprUT1EnD8L.jpeg) 

![Untitled|432x500](upload://j8XZvSXjsxo5hkBNYRWSfVPnOH7.jpeg) 

Then connect in VESC Tool

![vt|690x469](upload://k3mEMyWVd31hD26mc64jUWrudA8.png)
```

---
## \#1021 Posted by: Mainsedora Posted at: 2019-05-23T05:56:15.518Z Reads: 165

```
Thx for the reply. Yesterday I tried to compile vesc tool for my rpi3 and installing qt is actually cancer. Maybe I release a rpi version on github
```

---
## \#1022 Posted by: Balth81 Posted at: 2019-05-23T12:13:08.407Z Reads: 172

```
@rpasichnyk I see there was an update yesterday for iOS to fix unity up now I don’t even get 2 readings it just one?? Am I doing something wrong? Dual mode is enabled.. ![image|231x500](upload://l0oRLwYZq8b6PAt1Fw86yAUYluR.jpeg)
```

---
## \#1023 Posted by: hexakopter Posted at: 2019-05-24T12:49:23.175Z Reads: 170

```
@Balth81 Are you running the latest Metr Pro firmware version? If not please go to Settings, in the list of devices click on the blue gear icon beside your Metr Pro module and see if an Metr Pro firmware update is available. 

![ota|320x426](upload://rfnxb5rlMiS4T2EI3A6CarkAzgz.gif)
```

---
## \#1024 Posted by: Balth81 Posted at: 2019-05-24T13:37:16.337Z Reads: 176

```
@hexakopter sure am ![image|231x500](upload://aWdgMyEaezfuTEZpTAQHrECxyPU.jpeg) ![image|231x500](upload://a74E5EX5gGAdKRVoaqlH7e5lQrY.jpeg)
```

---
## \#1025 Posted by: rpasichnyk Posted at: 2019-05-24T20:26:42.155Z Reads: 168

```
Motor amps - you should get 2 readings

Battery amps - 1 reading

Motor temp - 2 readings

ESC temp - 1 reading

All should be good🙂
```

---
## \#1026 Posted by: Balth81 Posted at: 2019-05-24T22:09:50.382Z Reads: 177

```
Thanks mate you know what I realised is that with the update my layout changed and the motors weren’t on there.. so once I actually enabled them all is good now .. I thought they were on by default before but maybe I was wrong and I didn’t realise there was extra info on  the front screen that you can turn on. Thanks for you help..![image|231x500](upload://7iicBoOGXrXTTPgHWyXVjuRaRHI.jpeg)
```

---
## \#1027 Posted by: mishrasubhransu Posted at: 2019-05-26T07:52:50.332Z Reads: 178

```
This is my second metr pro(This one has an antenna). I bought this one from a forum member. The issue that I am having is that the module just keeps restarting every 5 second or so. I am using the 5V supply to the module. I am able to connect to the metr pro app but it disconnects and connects every 5 seconds. 

When it disconnects on the app, all the leds go out on the module. So the module is physically turning off. @hexakopter and @rpasichnyk, any idea what's going on?'

I just have the 5V, Gnd, rx, tx connected. I flipped rx, tx to see if that's the problem, it didn't change anything. I know, I know it's auto detect, but just in case. 
I then tried to run the module with rx and tx both removed. It wouldn't even turn on. Is that supposed to happen?

EDIT: Fixed
Used 3.3V and it worked. Somehow 5V was making it restart. I confirmed by going back to 5V.
```

---
## \#1028 Posted by: murloc992 Posted at: 2019-05-26T08:39:08.051Z Reads: 167

```
5V regulator might be blown, I presume the module has it. :confused:
```

---
## \#1029 Posted by: hexakopter Posted at: 2019-05-26T08:57:03.445Z Reads: 178

```
As stated in the [metr.at FAQ](https://metr.at/faq#q31):

_What pins of the JST connector are necessary for Metr Pro to work?_

Only four pins: 3.3V, GND, TX and RX need to be connected. The cable uses 7 wires to match ESCs 7 pin connector. We can not provide a cable with missing wires and we don't really have time to remove them. **You can't power the module with 5V**.

So you need 3.3V to power the module.
```

---
## \#1030 Posted by: mishrasubhransu Posted at: 2019-05-26T09:26:09.118Z Reads: 176

```
Please consider putting NC on the silkscreen where it's not connected. I just didn't want to put the plug the 7pin directly because I wasn't sure how the 5V and 3.3V would interact. Also I am not sure what SWC and SWD are(no info on FAQ).
```

---
## \#1031 Posted by: Manu39 Posted at: 2019-05-28T16:18:25.427Z Reads: 174

```
@rpasichnyk  I just flaked my Escape and tested  metr.pro again, it seems to work..... I didn't use the mode change...
```

---
## \#1032 Posted by: rpasichnyk Posted at: 2019-05-28T18:25:44.939Z Reads: 177

```
https://metr.at/z/anniversary
```

---
## \#1033 Posted by: Pantata Posted at: 2019-05-28T22:17:03.705Z Reads: 175

```
Ever since I got the METR pro module, whenever I enter the modes menu or the expert settings menu, always after around 10-15 seconds it disconnects and reconnects again and I have to switch screens and go back. Seems like a bug or something. Any advice please? Second problem that PERIMETR doesn't find any bt connections for some reason (tried to reinstall, nothing), can't use it at all... Thirdly any update on the ackmaniac esc tool working with the METR pro module in the future?
```

---
## \#1034 Posted by: oyta Posted at: 2019-05-29T04:51:02.602Z Reads: 174

```
[quote="Pantata, post:1033, topic:57780"]
Second problem that PERIMETR doesn’t find any bt connections for some reason (tried to reinstall, nothing), can’t use it at all…
[/quote]
The standalone Perimetr app is done. Now it is integrated in metr. Look at the «Expert» option in the menu.
```

---
## \#1035 Posted by: Xenon Posted at: 2019-05-30T05:15:54.424Z Reads: 168

```
Hi, Yesterday I bought a  SmartWatch with android Wear OS but can not find the metr.at app anywhere.  has that been removed from the Playstore?
```

---
## \#1036 Posted by: rpasichnyk Posted at: 2019-05-30T06:03:48.698Z Reads: 168

```
They way it works is you install Android app on your phone and Wear OS counterpart is automatically installed on your watch
```

---
## \#1037 Posted by: Martin Posted at: 2019-05-30T06:50:37.130Z Reads: 164

```
Where can i order this ???
```

---
## \#1038 Posted by: rpasichnyk Posted at: 2019-05-30T07:01:57.443Z Reads: 174

```
You will find out! Wait for announcement, the countdown ends soon ;)
```

---
## \#1039 Posted by: rpasichnyk Posted at: 2019-05-30T18:00:29.331Z Reads: 178

```
https://www.electric-skateboard.builders/t/metr-pro-unity-bluetooth-module/95494
```

---
## \#1040 Posted by: Pantata Posted at: 2019-06-05T11:09:41.519Z Reads: 166

```
Any feedback on the reconnecting problem in the modes and expert menu? Everything works, but as mentioned, after 10-20 seconds I would say it always disconnects and immediately reconnects. ALso the wh/km reading is always higher than when I divide total wh / total range. The daily range doesn't reset after a day. Any thoughts on these flukes? Thank you (ackmaniac will not be working with metr ever?)
```

---
## \#1041 Posted by: rpasichnyk Posted at: 2019-06-05T11:52:59.594Z Reads: 167

```
@Pantata I don't think I ever saw reconnecting problem. Can you send logs?
Wh/km wrong reading is confirmed and being fixed. The range should reset after a day. Try to check tomorrow. The compatibility with ackmaniac, I really tried to make it work, I can see on my end that request is coming and reply is sent successfully for GET_VERSION command, but then the Android app just seems to ignore it :confused:
```

---
## \#1042 Posted by: Pantata Posted at: 2019-06-05T11:58:46.190Z Reads: 168

```
Thank you for the answers man :) Will send logs. It does it by itself, I don't even have to be reading the config. Just simply entering the modes tab and the expert menu triggers reconnection...
```

---
## \#1043 Posted by: ejastram Posted at: 2019-06-09T22:13:20.044Z Reads: 171

```
After a slightly messy bailout and a shattered IPhone screen, I have been using an old throw away Android phone to connect with my metr and check distance, motor temps, etc... with the throw away phone, I do not have a sim card and use wifi for any network needed.. When i attempt to upload my log files to view on a device with a larger screen, it just sits there and never uploads... in the application log, the error is an SSL Handshake error.. upon watching wifi traffic, no request is ever sent from the application. It seems that the software just kind of ignores the wifi connection and only uses cell.... it would be nice to be able to connect via wifi
```

---
## \#1044 Posted by: rpasichnyk Posted at: 2019-06-10T06:26:43.664Z Reads: 162

```
I just tested record upload on Moto G4 with Android 7.0 and it worked fine. The phone doesn't have a SIM card, only using Wi-Fi. Please do some more investigation, maybe connecting your phone with USB cable and running `adb logcat` will give you some hints
```

---
## \#1045 Posted by: ejastram Posted at: 2019-06-11T23:25:51.230Z Reads: 158

```
Logcat gave less useful information than the log files... I am happy just assuming my phones (running Android 4.4) are too old..
```

---
## \#1046 Posted by: ryanrauch Posted at: 2019-06-16T02:26:42.233Z Reads: 154

```
How do I share a recorded log (on my iPhone) to the forum here? 

I was thrown off my board earlier today, but was recording through the metr pro app when it happened, and wanted to see if anyone can help diagnose it so it won't happen again.
```

---
## \#1047 Posted by: ryanrauch Posted at: 2019-06-16T02:36:50.289Z Reads: 153

```
Nevermind, I figured it out
```

---
## \#1048 Posted by: McErono Posted at: 2019-06-16T20:44:10.231Z Reads: 149

```
If someone else is looking for an answer: records, choose record, upload, copy url in the opened browser window, paste url in forum (has to be supported).
```

---
## \#1049 Posted by: bsb Posted at: 2019-06-24T19:54:00.496Z Reads: 143

```
metr offers two options to record the speed and show it in the upload. One is by GPS data and the other is by RPM and number of poles of the motor and some calculation on wheel circumference. 
It would be very handsome if the raw eRPM or mRPM would show up as an individual channel on the uploaded graphic although the GPS speed is taken as reference. This feature would be helpful for all applications where you use a gearshift and also for propeller driven vehicles. Thank you.
```

---
## \#1050 Posted by: Darkie02 Posted at: 2019-06-24T20:08:24.041Z Reads: 146

```
So my auto record has stoped working over the last week but it’s turned on in the app. All works fine if I manually start recording.
```

---
## \#1051 Posted by: DAddYE Posted at: 2019-06-24T21:05:40.814Z Reads: 147

```
Same here. 10c
```

---
## \#1052 Posted by: rpasichnyk Posted at: 2019-06-25T12:08:50.202Z Reads: 144

```
@Darkie02 @DAddYE logs please?
```

---
## \#1054 Posted by: Darkie02 Posted at: 2019-06-25T16:15:10.666Z Reads: 149

```
Convinced ISO updated recently about the same time guessing that update broke things.
```

---
## \#1055 Posted by: PixelatedPolyeurthan Posted at: 2019-06-25T17:31:38.904Z Reads: 156

```
I am sorry if this is a stupid question but does this work if you pull out the UART connection out of my Evolve Carbon GT.
Does the GT need the UART plugged in to work?
Any way around this if not?

Thanks a million
```

---
## \#1056 Posted by: rpasichnyk Posted at: 2019-06-25T18:47:49.812Z Reads: 161

```
@Darkie02 @DAddYE go to Metr Settings and
* enable Use location (it may have been disabled)
* disable Prefer GPS

![image|281x499](upload://iifZyPjC5fJG6bURDp3f0maNGG0.png) 

also make sure Metr has location services on Always in iOS Preferences

![image|281x499](upload://2b2TafG8Oj3JbmLyAQEcXJXeWsa.png)
```

---
## \#1057 Posted by: DAddYE Posted at: 2019-06-25T20:20:54.540Z Reads: 152

```
After updating to iOS 13 I’m unable to test it (I think I might just need to give BT permission to metr)
```

---
## \#1058 Posted by: xsynatic Posted at: 2019-06-26T00:10:05.020Z Reads: 150

```
How would i use the metro pro and the flipsky vx1 remote which also connects via the uart port?
```

---
## \#1059 Posted by: ZachTetra Posted at: 2019-06-26T01:33:00.184Z Reads: 147

```
Someone has a splitter they're working on
```

---
## \#1060 Posted by: bsancken Posted at: 2019-06-26T02:31:52.033Z Reads: 150

```
https://www.electric-skateboard.builders/t/uart-splitter-for-vesc-based-escs/94552?u=bsancken
```

---
## \#1061 Posted by: xsynatic Posted at: 2019-06-26T06:19:04.480Z Reads: 145

```
Oh yes! Thanks for that. I hope the product is finished soon
```

---
## \#1062 Posted by: Darkie02 Posted at: 2019-06-26T06:56:35.790Z Reads: 151

```
Prefer GPRS was on all the other things were ok didn't need changing. Will give it a test later.

[quote="rpasichnyk, post:1056, topic:57780"]
* enable Use location (it may have been disabled)
* disable Prefer GPS
[/quote]

[quote="rpasichnyk, post:1056, topic:57780"]
also make sure Metr has location services on Always in iOS Preferences
[/quote]
```

---
## \#1063 Posted by: bevilacqua Posted at: 2019-06-26T08:19:21.138Z Reads: 147

```
@StefanMe is also using IOS 13, does your Metr App work Stefan?
```

---
## \#1064 Posted by: PixelatedPolyeurthan Posted at: 2019-06-26T12:30:41.088Z Reads: 144

```
Sorry but is my question above really that bad for no one to answer it 😬
```

---
## \#1065 Posted by: rpasichnyk Posted at: 2019-06-26T12:50:20.396Z Reads: 147

```
You must have [VESC®](https://vesc-project.com)-based ESC. If you have another controller, the app will not work for you. For example Boosted, Evolve, Meepo, WowGo, Backfire have another type of controller and are not compatible
```

---
## \#1066 Posted by: PixelatedPolyeurthan Posted at: 2019-06-26T16:31:42.650Z Reads: 147

```
@rpasichnyk thanks. Sorry again 😅
```

---
## \#1067 Posted by: ZachTetra Posted at: 2019-06-26T16:37:28.781Z Reads: 153

```
Has anyone tried a METR Pro with the FSESC dual 6.6 plus yet?
```

---
## \#1068 Posted by: McErono Posted at: 2019-06-26T19:48:14.017Z Reads: 152

```
@rpasichnyk auto record does still work here and just updated to 4.8
```

---
## \#1069 Posted by: rpasichnyk Posted at: 2019-06-27T05:32:37.228Z Reads: 159

```
Should work fine with FSESC dual 6.6

UART https://flipsky.net/collections/electronic-products/products/dual-fsesc6-6-plus-based-on-vesc6

![22|690x435,50%](upload://ltH6OHsnzJ1ub36d6B9V6aTO4sU.png) 

VESC6 https://metr.at/setup

![vesc|474x500](upload://jkys2Z2c0MGVXaqDKwDLtLugzkr.jpeg)
```

---
## \#1070 Posted by: keithcys Posted at: 2019-07-01T10:03:00.841Z Reads: 149

```
Sorry I'm new with vesc here.
Does it only works in certain fw?
I currently running  Dual FSESC6.6 with fw3.57
```

---
## \#1071 Posted by: Ricco Posted at: 2019-07-02T17:08:53.002Z Reads: 148

```
Where can I find the source code for the Metr Pro Firmware v4.8?
```

---
## \#1072 Posted by: McErono Posted at: 2019-07-02T17:29:50.115Z Reads: 150

```
Metr isn't open source...
```

---
## \#1073 Posted by: Ricco Posted at: 2019-07-02T17:34:51.819Z Reads: 150

```
The Metr Pro Firmware v4.8 is Firmware for VESC based ESCs right?
```

---
## \#1074 Posted by: McErono Posted at: 2019-07-02T17:35:42.081Z Reads: 153

```
4.8 is the firmware of the BT module not the ESC
```

---
## \#1075 Posted by: Ricco Posted at: 2019-07-02T17:38:01.937Z Reads: 150

```
Ok thanks for clarifying that :slight_smile:
```

---
## \#1076 Posted by: McErono Posted at: 2019-07-02T17:38:20.119Z Reads: 147

```
Should work with any vesc based firmware afaik.
```

---
## \#1077 Posted by: Goa Posted at: 2019-07-06T20:39:45.560Z Reads: 144

```
Just ordered the module. I am excited to add it to my work in progress kick scooter build!
```

---
## \#1078 Posted by: Jinra Posted at: 2019-07-07T07:32:21.834Z Reads: 146

```
Hey @rpasichnyk,

Using ackmaniac 3.102 with the metr pro module and the app freezes whenever I connect. Current on a Pixel 3 Android Pie. Before it connects I can navigate the menu and everything else, and yes I've tried a system reboot.
```

---
## \#1079 Posted by: rpasichnyk Posted at: 2019-07-07T07:44:46.506Z Reads: 141

```
Please connect your phone to computer and run adb logcat. Then repeat freezing. Collect the output of adb logcat and send to support@metr.at, thanks :slight_smile:
```

---
## \#1080 Posted by: Jinra Posted at: 2019-07-07T09:15:40.100Z Reads: 141

```
How exactly?
```

---
## \#1081 Posted by: Jinra Posted at: 2019-07-08T03:28:30.242Z Reads: 146

```
FWIW i tried two different modules and two different phones with the same result. I think it's an ackmaniac fw compatibility issue
```

---
## \#1082 Posted by: Jinra Posted at: 2019-07-08T20:37:19.592Z Reads: 146

```
Finally got it working with my pixel 2 (instead of my current pixel 3) but now it hangs on fw upload (the end is where it gets stuck).

https://photos.app.goo.gl/KA57stMK2SQ52jb77

EDIT: was able to update my OTHER module perfectly fine on my pixel 2, but the original module does what the video shows.
```

---
## \#1083 Posted by: vortek Posted at: 2019-07-08T23:10:28.207Z Reads: 147

```
Guys im using iPhone metr pro app and the modes keep disappearing. I create them and use them and then after a few minutes they are gone. ![image|230x500](upload://5ph6pAtTitPEPx6U6X6A6JOvgo1.jpeg)
```

---
## \#1084 Posted by: rpasichnyk Posted at: 2019-07-09T07:30:03.248Z Reads: 142

```
Interesting, thanks for video, can you please try again and then send logs to support@metr.at?

@vortek There was a bug with modes not being saved (already fixed), but app review takes a bit longer on App Store. You should receive an update (v3.8.18) soon :+1:
```

---
## \#1085 Posted by: Jinra Posted at: 2019-07-09T07:41:42.761Z Reads: 135

```
Could you provide instructions on how to get you those logs. What do i do about the module that can't even update
```

---
## \#1086 Posted by: rpasichnyk Posted at: 2019-07-09T07:53:01.600Z Reads: 136

```
Open Metr app, go to Settings -> Show Logs. Share the file via email. I will look at the upgrade logs first and then decide what to do with the module that you have :+1:
```

---
## \#1087 Posted by: Jinra Posted at: 2019-07-09T15:24:24.415Z Reads: 138

```
I just got to work and was going to do that... but then it started working (on my second module)! I'm not sure why, but I'll let you know if it happens again. I still can't get the other module working/updated though, I will email you about that.
```

---
## \#1088 Posted by: Jinra Posted at: 2019-07-09T16:51:50.405Z Reads: 140

```
Not sure if you take bug reports through here, but it seems that the "expert" panel shows my VESC as running sensorless even though it's sensored, perhaps just a quirk with non-official f/w?
```

---
## \#1089 Posted by: Goa Posted at: 2019-07-11T14:23:28.364Z Reads: 141

```
rpasichnyk Hello, am I supposed to receive order and tracking info in the mail? I'm not sure I got them.
Oh sorry i didnt realize you had FAQ on your website. Now i know you ship within 3 days of the order. 
Should be any moment now.
```

---
## \#1090 Posted by: rpasichnyk Posted at: 2019-07-11T17:51:00.196Z Reads: 136

```
Yes I am taking bug reports everywhere, can you please describe in more details (which firmware you have, screenshots and Settings - Show Logs to support@metr.at) Thanks!
```

---
## \#1091 Posted by: hexakopter Posted at: 2019-07-12T16:38:48.445Z Reads: 136

```
[quote="Goa, post:1089, topic:57780"]
Hello, am I supposed to receive order and tracking info in the mail?
[/quote]


You should receive a tracking number via PayPal. Orders were shipped today.
```

---
## \#1092 Posted by: Pantata Posted at: 2019-07-13T23:18:59.130Z Reads: 133

```
Ackmaniac ESC app never worked with this module.
```

---
## \#1093 Posted by: Jinra Posted at: 2019-07-13T23:48:58.771Z Reads: 129

```
Works for me
```

---
## \#1094 Posted by: rpasichnyk Posted at: 2019-07-14T07:12:12.394Z Reads: 130

```
Actually it did, at the time of Metr Pro release, Ackmaniac app worked just fine. But you are confusing things, Jinra is using Metr app with Ackmaniac ESC firmware for VESC, not Ackmaniac ESC app :stuck_out_tongue:
```

---
## \#1095 Posted by: Pantata Posted at: 2019-07-14T10:28:47.201Z Reads: 129

```
Oh, sorry confused the app with the FW. The ackaniac android app doesn't work with Metr module, though ackamaniac FW works with Metr module (metr app)
```

---
## \#1097 Posted by: pookybear Posted at: 2019-07-16T03:00:11.379Z Reads: 121

```
Ack app works w metr pro module. You just need a lower version of the app.
```

---
## \#1098 Posted by: caustin Posted at: 2019-07-16T03:19:50.523Z Reads: 127

```
What past version of the app worked with Metr module and how can we get it if we have long ago updated to more current versions?
```

---
## \#1099 Posted by: pookybear Posted at: 2019-07-16T03:21:35.368Z Reads: 125

```
Let me upload it. Give me one sec.
```

---
## \#1100 Posted by: pookybear Posted at: 2019-07-16T03:24:25.715Z Reads: 130

```

V1.101

Edit. 

Link no worky. Deleted. See post below.
```

---
## \#1101 Posted by: caustin Posted at: 2019-07-16T03:31:05.726Z Reads: 134

```
Hmm, what am I doing wrong?
![image|230x500](upload://hryXyKz5JubcR32hLdYjbo0L8DC.jpeg)
```

---
## \#1102 Posted by: pookybear Posted at: 2019-07-16T03:37:23.939Z Reads: 128

```
Let me double-check
```

---
## \#1103 Posted by: pookybear Posted at: 2019-07-16T03:41:04.925Z Reads: 129

```
@caustin 

I uploaded it to a different site. Ack app v1.101

[Here](https://we.tl/t-tmeGopnLph) you go. Let's try this again.
```

---
## \#1104 Posted by: caustin Posted at: 2019-07-16T19:20:57.495Z Reads: 122

```
Thanks, let me try this!
```

---
## \#1105 Posted by: drone001 Posted at: 2019-07-18T17:10:01.576Z Reads: 120

```
I'm interested in using these modes. is there like a web site that explains how these modes work?
```

---
## \#1106 Posted by: hexakopter Posted at: 2019-07-18T17:54:50.209Z Reads: 130

```
[quote="drone001, post:1105, topic:57780"]
is there like a web site that explains how these modes work?
[/quote]
It is explained in this thread. If you still have questions afterwards let us know.
https://forum./t/the-definitive-guide-to-metr-app/3109
```

---
## \#1107 Posted by: drone001 Posted at: 2019-07-19T03:16:43.186Z Reads: 131

```
thx bruh.....just what i needed.
```

---
## \#1108 Posted by: r3vilo Posted at: 2019-07-19T09:21:02.270Z Reads: 131

```
@rpasichnyk

I got the same problem. It hangs at the screen "Don't interrupt..." and I'm not able to upgrade fw. I will send you my log. Thanks for investigating.

By the way: Is with 4.8 the problem fixed, that people brick their VESCs since VESC fw 3.57 and the new, updated VESC tool? When I'm right, there was a problem with changing modes. Or was it when updating VESC fw via TCP bridge over metr? I don't know exactly. I did it via VESC mobile app and everything worked well. But also here I stuck now with VESC fw 3.57 and am not able to update to 3.58. There's another thread in this forum. More people have this problem.

Together with the problem now, that I'm not able to update metr.pro to 4.8. It all starts with 3.57 if you want so, but I don't think it's related.
```

---
## \#1109 Posted by: rpasichnyk Posted at: 2019-07-19T12:00:05.854Z Reads: 134

```
[quote="r3vilo, post:1108, topic:57780"]
Together with the problem now, that I’m not able to update metr.pro to 4.8. It all starts with 3.57 if you want so, but I don’t think it’s related.
[/quote]

No, this is not related. The upgrade from 3.69 to 4.8 was a major update that not only includes Metr Pro firmware but also new nordic softdevice and bootloader. This is why update process consists of 2 parts and it's very important not to interrupt it. However in some cases softdevice and bootloader update completes, but firmware is still 3.69. @taz had exactly this problem and we solved it using individual GUID based firmware update. Hope the same trick helps to you.
```

---
## \#1110 Posted by: sayekim Posted at: 2019-07-19T14:16:39.286Z Reads: 135

```
Will we ever see the dual motor records in the metr records as separate data when recording?

I needz this.
```

---
## \#1111 Posted by: r3vilo Posted at: 2019-07-19T22:52:01.256Z Reads: 136

```
Thank you, Roman. You helped me alot yesterday. I wrote you an E-Mail with logfile. After successful updating with my individual firmware I had to go to work. Sent you this logfile as well a few minutes ago. Sorry for the delay.
```

---
## \#1112 Posted by: sebaszz Posted at: 2019-07-31T21:34:18.477Z Reads: 126

```
[quote="rpasichnyk, post:94, topic:57780, full:true"]
I'm sure many of you would like to try VESC Tool with direct BLE connection to Metr Pro.
Here you can find the latest VESC Tool binaries for macOS and Windows.

https://github.com/rpasichnyk/vesc_tool/releases

In Windows, you first need to complete new device pairing procedure:
1. Press Start and type bluetooth. Open Bluetooth and other device settings.
![00|294x500,80%](upload://quYeSNojREiCnNWg9oBNafulpoG.jpg)
2. Click "Add Bluetooth or other device
![48|690x425,80%](upload://ArT4M0QgTQ9HmYoLEtNiZUZw0G.jpg)
3. Wait until you see Metr Pro, click on it and enter PIN code
![06|690x419,50%](upload://iDUzkuiIOdLAyNTiIkR0rmMuWEZ.png) 

After this you should be able to connect via VESC Tool
[/quote]

Any plans in releasing a new version based on the (windows) vesc 1.16 tool?
```

---
## \#1113 Posted by: krazor Posted at: 2019-08-05T09:15:50.696Z Reads: 115

```
I have it conne Ted to my phone the app says its connected but I have flashing blue and green light and all values in real time are zero?
```

---
## \#1114 Posted by: hexakopter Posted at: 2019-08-05T09:48:27.800Z Reads: 119

```
Make sure you have PPM + UART enabled on your VESC. Only when the green LED is solid lit, it detected the UART connection correctly.
```

---
## \#1115 Posted by: krazor Posted at: 2019-08-05T13:31:46.633Z Reads: 116

```
Thanks that was the issue
```

---
## \#1116 Posted by: krazor Posted at: 2019-08-12T08:57:35.001Z Reads: 109

```
a quick question since i  blew one of my foc boxes im looking at replacing my other one with this one here [Dual FSESC6.6 Based upon VESC6 with Aluminum Heatsink](https://flipsky.net/collections/electronic-products/products/dual-fsesc6-6-based-upon-vesc6-with-aluminum-heatsink)
```

---
## \#1117 Posted by: krazor Posted at: 2019-08-12T08:58:59.364Z Reads: 111

```
Wow seems like I never actually sent my previous message.. Well any ways I have my new vesc here flipsky 6.6. How abouts do I plug it in with metr cable that's supplied as it is missing a pin for it to fit?
```

---
## \#1118 Posted by: rpasichnyk Posted at: 2019-08-12T09:11:19.047Z Reads: 116

```
You can use the same cable, leave ADC3 pin unconnected
```

---
## \#1119 Posted by: krazor Posted at: 2019-08-12T09:18:36.802Z Reads: 120

```
Ah thought so I was cross referencing my focbox and it seems that's the only extra pin. I was also wondering if this will work from the slave vesc  on the flipsky duel 6.6 as I have the Firefly nanao remote i wnat to use that on the master side and the METR Pro on the Slave side is it possible?
```

---
## \#1120 Posted by: Pimousse Posted at: 2019-08-12T14:05:42.258Z Reads: 118

```
Yes.

10char
```

---
## \#1121 Posted by: Pantata Posted at: 2019-08-12T21:51:41.374Z Reads: 117

```
I have tried most of the versions available all the way to the oldest one. It does not work.
```

---
## \#1122 Posted by: caustin Posted at: 2019-08-13T01:17:07.026Z Reads: 110

```
Really, V1.101 didn’t work for you?
```

---
## \#1123 Posted by: Pantata Posted at: 2019-08-13T07:18:43.648Z Reads: 111

```
None of the versions, have had the module for over half a year, never managed to run the Ackamanic Esc app. It does show the module, it does "connect" but doesn't show any data and If I click on modes or anythig, it will say ESC is not connected. Does it work for you?
```

---
## \#1124 Posted by: pookybear Posted at: 2019-08-13T15:17:04.888Z Reads: 110

```
I'm using:

* Ack FW 3.102 ( [LINK](https://drive.google.com/drive/folders/1Ek1vL60n7eza7-dDqQeXCfLRhfMQXofg?usp=sharing) )
* Ack app v1.101  ( [LINK](https://drive.google.com/drive/folders/1QGyXueD_3qjdLBn_8hV8rTziXPBnKmaL?usp=sharing) )

This works for me. Make sure you set PPM+UART. Hope this helps.
```

---
## \#1125 Posted by: Pantata Posted at: 2019-08-13T15:31:42.921Z Reads: 112

```
I am not using ackmaniac fw as I have the unity. And 1.101 still does not work :(
```

---
## \#1126 Posted by: pookybear Posted at: 2019-08-13T15:33:22.730Z Reads: 112

```
Unfortunately, ack app only works WITH ack FW. Just use metr app. It's pretty robust.
```

---
## \#1127 Posted by: Pantata Posted at: 2019-08-13T22:00:08.580Z Reads: 110

```
Oh I am and always have been, it's great. The only thing extra were the gauges in the ackmaniac app.
```

---
## \#1128 Posted by: krazor Posted at: 2019-08-23T08:39:22.533Z Reads: 104

```
Is there a way to smooth out the battery voltage it jumps around a lot when idle
```

---
## \#1129 Posted by: xsynatic Posted at: 2019-08-23T12:35:27.032Z Reads: 107

```
Go to Settings → Battery → Smooth Voltage. If needed, adjust the margin.
```

---
## \#1130 Posted by: Toleg Posted at: 2019-09-07T23:31:21.175Z Reads: 101

```
does not work anymore with my android wear (install fails :( )
```

---
## \#1131 Posted by: Yegmesh Posted at: 2019-10-05T17:31:49.924Z Reads: 85

```
HI,

I would like to buy this, but i was wondering if i can get this without VAT as i am in Jersey channel islands and we don't have VAT. But there is no option to ship to jersey.

Thanks!
```

---
## \#1132 Posted by: hexakopter Posted at: 2019-10-07T19:13:30.756Z Reads: 83

```
Hi Thomas,

yes that should be possible. Please send us an email to support@metr.at and we will sort out the payment.
```

---
## \#1133 Posted by: ChristianT Posted at: 2019-10-07T20:42:09.839Z Reads: 83

```
Can someone explain me (with very little experience) what the Metr Pro is about?
What does it do and why is it so cool?

Sorry guys, I just don´t get it. Hope you can help me out ;)
```

---
## \#1135 Posted by: rpasichnyk Posted at: 2019-10-11T06:06:48.141Z Reads: 79

```
Here is a short manual with features (there are many)

https://forum./t/the-definitive-guide-to-metr-app-metr-pro
```

---
## \#1136 Posted by: krazor Posted at: 2019-10-26T10:44:01.525Z Reads: 65

```
Hello, I would like to find out some info beforei  purchase a couple Vesc6 from trampa. i already have the Metr Pro blutooth module as i was planning on using it with another vesc but it died during test any ways...   they have this Dongle on their site which i assume is just another blutooth module but at a fraction of the cost. i picked up the Metr pro module for its features but i would like to know if its usable in place of the Dongle. since i already have it and have used it a couple of times i really like the features and data it outputs and its ease of use. but im not sure what the difference is between the Trampa Dongle and the Metr Pro module. can i use the Metr Pro module in place of the Dongle. or do i need to use the Dongle and scrap the Metr Pro module i have?

Appologies for my ignorance. i am truely confused here about what i can use. just trying to save my self 20 pounds before making the purchase if i can is all since i already have the Metr Pro module. but i dont mind grabbing it incase i cant use the Metr Pro module if you know what i mean.

Thanks in advanced!
```

---
## \#1137 Posted by: rpasichnyk Posted at: 2019-10-26T10:56:43.163Z Reads: 68

```
You can use Metr Pro instead of Trampa Dongle. It supports all the functions and is more secure. But if you want to use their new remote Trampa WAND, you need Trampa Dongle.
```

---
## \#1138 Posted by: krazor Posted at: 2019-10-26T11:00:35.740Z Reads: 71

```
ah ok dam i was literly just about to ask about that as i was going to get the wand remote. guess ill hold off from the wand then. will metr pro be compatible with the Wand remote in the future or is it simpley pick 1 or the other. i like the feature on the wand remote which has safe reverse brakes for going down hill. basically makes the brakes work properly when going down hill without having reverse set up as i ride with forward/brake modes


Actually is it possible to use Both Metr Pro and the Trampa Dongle so i can get readings to the wand remote as well as record the data on my phone?
```

---
## \#1139 Posted by: rpasichnyk Posted at: 2019-11-26T17:13:34.812Z Reads: 53

```
If you missed Metr Pro updates, they are now posted on  forum. To read about latest new features and Black Friday announcement, follow this link

https://forum./t/metr-pro-updates/3105/419?u=rpasichnyk
```

---
## \#1140 Posted by: ElectricCoast Posted at: 2019-12-04T14:33:55.411Z Reads: 44

```
I just updated both of my FOCBOX Unitys to FW 23.46 and both of my stand alone regular Metr Pros and now I am getting this error.  I'm trying to change my settings via Metr Pro on my Unitys![Screenshot_20191204-083007_metr|236x500](upload://iv9sUjsUv7r3WDVzHfAWLwgD1xV.jpeg)
```

---
## \#1141 Posted by: webst Posted at: 2019-12-04T17:06:58.285Z Reads: 46

```
[quote="rpasichnyk, post:1137, topic:57780, full:true"]
You can use Metr Pro instead of Trampa Dongle. It supports all the functions and is more secure. But if you want to use their new remote Trampa WAND, you need Trampa Dongle.
[/quote]

Remote seems nice but this is fatal flaw.

[quote="rpasichnyk, post:1139, topic:57780"]
[https://forum ](https://forum)./t/metr-pro-updates/3105/419?u=rpasichnyk
[/quote]

This is not a valid address
```

---
## \#1142 Posted by: SeanHacker Posted at: 2019-12-05T01:50:55.750Z Reads: 47

```
Go here https://forum.        /t/metr-pro-updates/3105

Take the gap I made out (between the . and ) and you will have the link. This site doesn't let us post other forums because of racism or money or something... Jason's a fucking idiot.
```

---
## \#1143 Posted by: rpasichnyk Posted at: 2019-12-05T06:46:09.336Z Reads: 47

```
Check that you are running latest Metr app from Google Play Store.
```

---
## \#1144 Posted by: ElectricCoast Posted at: 2019-12-05T16:33:46.964Z Reads: 49

```
That fixed my issue.  Thanks so much for the superb customer service.
```

---
## \#1145 Posted by: Eretron Posted at: 2019-12-06T19:14:46.157Z Reads: 45

```
How to properly connect metr with diebiems?

I've tried searching forums but had no luck...

I am using flipsky dual 6.6 fesc.

Thanks
```

---
## \#1146 Posted by: rpasichnyk Posted at: 2019-12-09T09:55:14.778Z Reads: 47

```
1. Connect your DieBieMS via CAN to VESC
2. Connect USB cable to VESC
3. Use DieBieMS Tool on your computer and make sure it can access DieBieMS over VESC over CAN
4. Metr app should work out of the box after this. The only thing you need to change in Settings -> Battery -> Battery type to DieBieMS
```

---
## \#1147 Posted by: krazor Posted at: 2020-01-10T09:44:40.889Z Reads: 41

```
Hi i have issue with flashing blue and flashing green light i dont get any data sent to my app through the module i have vesc 6
```

---
## \#1148 Posted by: Pantata Posted at: 2020-01-26T19:05:21.897Z Reads: 31

```
ANy update on the constant freezes? It's been weeks now... I need 4.08 fw version so I can downgrade... Can you do that for me Roman If you can't fix it the correct way? I have almost no records in last weeks because of that... I did some testing and it has something to do with vertical/horizontal view change on the phone. There is a bug in it, I disabled horizontal view at all, will see If it stops freezing now.
```

---
## \#1149 Posted by: rpasichnyk Posted at: 2020-01-27T15:41:24.770Z Reads: 24

```
If you want 4.8 fw you have to send module back to us to reprogram. There is no easy way to downgrade the firmware
```

---
