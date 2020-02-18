# VESC HM-10 bluetooth wiring

### Replies: 70 Views: 14350

## \#1 Posted by: rodrigovolkmer Posted at: 2016-11-10T22:28:15.674Z Reads: 998

```
Hey guys, 

just bought a HM-10 module to connect the VESC to the iOS BLDC tool app, just wondering if someone could help me with the wiring and first connection?



photos of the VESC and HM-10 wiring would be most appreciated.

thanks
```

---
## \#3 Posted by: rodrigovolkmer Posted at: 2016-11-11T00:25:25.062Z Reads: 926

```
I was thinking on getting simple jumper leads to connect the pins, but what the heck are those 1k and 2k ohm and in a T junction ? sorry the stupid question, I'm a newbie in electronics...

can I buy that ready or need to assemble myself?
```

---
## \#4 Posted by: Pimousse Posted at: 2016-11-11T11:21:54.048Z Reads: 905

```
Not sure you can buy it ready to use.
Resistors are here to lower the signal level from 5V (level of VESC) to 3,3V (level of HM10) only for the RX pin of HM10.
BTW, some guys don't use them and it  works. But no idea how long it will last.

For JST pins connection, see Vedder schematic :
https://github.com/vedderb/bldc-hardware/blob/master/design/BLDC_4.pdf
```

---
## \#5 Posted by: DeathCookies Posted at: 2016-11-11T12:05:32.498Z Reads: 885

```
[quote="Pimousse, post:4, topic:12838"]
Resistors are here to lower the signal level from 5V (level of VESC) to 3,3V (level of HM10) only for the RX pin of HM10.
[/quote]

It depends on each module. My module is safe up to 6V i think but the old ones are only safe up to 3,3V
```

---
## \#6 Posted by: rodrigovolkmer Posted at: 2016-11-11T12:30:51.409Z Reads: 846

```
If I'm not mistaken my VESC has 3.3v output as well as the 5v. Its written down on the pcb. 

Will test it before plug it in and let you know
```

---
## \#7 Posted by: Pimousse Posted at: 2016-11-11T12:59:29.504Z Reads: 830

```
Are you talking about power supply or RX/TX level ?
Mine is safe also up to 6V... for power supply ! Not for RX/TX level.

@rodrigovolkmer : yes, for power supply, not for TX/RX level.
```

---
## \#8 Posted by: DeathCookies Posted at: 2016-11-11T13:20:40.170Z Reads: 810

```
Power Supply but i do not know my rating of the rx/tx
```

---
## \#9 Posted by: PB1 Posted at: 2016-11-11T15:08:51.320Z Reads: 804

```
I'm using an HC-05 module without resistors for tx and it works fine. Powered by 3,3v off the VESC UART port. 

Don't know yet about the HM-10 module, still waiting for it.
```

---
## \#10 Posted by: Pimousse Posted at: 2016-11-11T19:40:09.365Z Reads: 792

```
Should be 3,3V as HC05 is 3,3V.
There are some boards workinf with a power supply because manifacturers add their PCB with DC/DC converter to be accept 5/6V.

BTW, 5V on the RX seems to be supported by the HC05.
I lowered it to 3,3V for the peace of mind. :slight_smile:
```

---
## \#11 Posted by: chinzw Posted at: 2016-11-12T02:06:37.046Z Reads: 752

```
Don't feed 5v to the RX of an HC05. It wont short straight away, but it will eventualy, the RX port of the HC05 is 3.3v rated.  Most modules allow for higher vcc, but not on the pins.

The ideal hookup to the vesc would be gnd and 3.3v rail
```

---
## \#12 Posted by: JTAG Posted at: 2016-11-13T12:00:53.019Z Reads: 725

```
The VESC has a STM32 operating @3V3, why would the serial port communicate @5V? As far as I know the signal levels on the VESC are 3V3. Does anybody know where the 5V info comes from?
```

---
## \#13 Posted by: chinzw Posted at: 2016-11-13T17:44:40.009Z Reads: 725

```
[quote="JTAG, post:12, topic:12838"]
Does anybody know where the 5V info comes from?
[/quote]

Arduino confusion, since they have 5v signals that need to be reduced with a voltage divider.
```

---
## \#14 Posted by: Pimousse Posted at: 2016-11-13T18:51:14.941Z Reads: 706

```
My fault.
I was sure that TX level of VESC was 5V...
BTW it's possible to directly use 5V Arduino TX level on RX pin of the VESC.
http://vedder.se/forums/viewtopic.php?f=6&t=214
```

---
## \#15 Posted by: chinzw Posted at: 2016-11-13T20:33:17.370Z Reads: 690

```
Its so easy to add 2 resistors to the TX pin of the arduino that its just not worth the risk of blowing up an ic
```

---
## \#16 Posted by: Pimousse Posted at: 2016-11-13T20:36:20.026Z Reads: 676

```
100% agree.
```

---
## \#17 Posted by: Eboosted Posted at: 2017-02-16T01:44:52.002Z Reads: 664

```
Hello guys, this wiring was not very clear for me, hope to get help to this.

On the VESC there is no indication on what pins of the UART are what, only on the bluetooth module.

Does anyone has a picture with the HM-10 connected?
```

---
## \#18 Posted by: Deakbannok Posted at: 2017-02-16T10:40:45.043Z Reads: 691

```
I have HM-10 bluetooth installed on my VESC-X.
It works good, no problem.

Post a photo of your vesc I'll show.
You only need to 4 connection wires.
On the HM-10
TX
RX
Grnd
VCC or 3-5 voltage
```

---
## \#19 Posted by: Pimousse Posted at: 2017-02-16T10:52:03.555Z Reads: 698

```
Sorry, previous wiring diagram was not clear (even wrong with the resistors).
Here is a better one :slight_smile:
[img]http://img4.hostingpics.net/pics/995016847251VESCHCconnection.jpg[/img]
Just replace HC-05 by HM-10 (same pin layout)
```

---
## \#20 Posted by: Eboosted Posted at: 2017-02-16T14:44:58.133Z Reads: 670

```
Just to add a little bit more clarification for future users:

1. On the back of THE VESC UART port is an indication of what pin is what
2. You need to plug in this layout otherwise Bluetooth will connect but no data will be displayed:
VCC - 5V
GND -  GND
TX - RX
RX -  TX
3. Connect HM-10 cables to master VESC UART port
4. Change application from PPM to PPM and UART

If these steps were written somewhere, it would have saved me 2 hours at least
```

---
## \#21 Posted by: Blasto Posted at: 2017-02-16T15:21:04.563Z Reads: 637

```


[quote="Eboosted, post:20, topic:12838"]
If these steps were written somewhere, it would have saved me 2 hours at least
[/quote]

there's always a learning curve ;)
```

---
## \#22 Posted by: Blasto Posted at: 2017-02-16T15:26:09.827Z Reads: 611

```
[quote="Pimousse, post:19, topic:12838"]
Sorry, previous wiring diagram was not clear (even wrong with the resistors).Here is a better one :slight_smile:
[/quote]

is the EN pin pulled up on the module? i've seen some that are actually pulled down, so you need to short the EN pin to VCC
```

---
## \#23 Posted by: Pimousse Posted at: 2017-02-16T15:51:12.166Z Reads: 594

```
No need.
At least on mine, it works well without doing anything with (just a shrinktube on it ;) )
```

---
## \#24 Posted by: Eboosted Posted at: 2017-02-16T17:14:16.700Z Reads: 583

```
Thanks @Blasto, the typo was fixed!
```

---
## \#25 Posted by: flyboywebb Posted at: 2017-04-06T13:14:56.990Z Reads: 563

```
 So, once you have it connected and powered up is there anything you need to do in settings to make it work with the BLDC app?
```

---
## \#26 Posted by: flatsp0t Posted at: 2017-04-06T13:21:32.561Z Reads: 558

```
Maybe check out the post 5 posts above yours.
```

---
## \#27 Posted by: flyboywebb Posted at: 2017-04-06T13:52:19.134Z Reads: 553

```
Thanks! Misssd the ppm and uart part.
```

---
## \#28 Posted by: flyboywebb Posted at: 2017-04-14T16:42:36.377Z Reads: 540

```
 Anyone know of a DIY ble remote control
```

---
## \#29 Posted by: jaykup Posted at: 2017-04-14T20:26:59.770Z Reads: 551

```
[quote="flyboywebb, post:28, topic:12838, full:true"]
Anyone know of a DIY ble remote control
[/quote]

Active work in process - 

https://www.radicalcreation.com/forums/viewtopic.php?f=6&t=35
```

---
## \#30 Posted by: emcauliff Posted at: 2017-09-09T01:28:40.888Z Reads: 460

```
What app is everyone using for iOS?
```

---
## \#31 Posted by: rpn314 Posted at: 2017-09-15T21:42:45.673Z Reads: 459

```
metr and perimtr are you're only really options (same guy, does different things). He requires that you buy his bluetooth module though. I think most of us on iOS just don't, sadly.
```

---
## \#32 Posted by: cody00 Posted at: 2017-09-18T04:12:54.809Z Reads: 460

```
@emmaanuel created one for iOS 
http://www.electric-skateboard.builders/t/new-ios-app-eskate-vesc-for-standard-and-ackmaniac-fw/32340
```

---
## \#33 Posted by: rpn314 Posted at: 2017-09-19T17:22:51.773Z Reads: 434

```
Thanks fantastic! I hadn't seen that post yet, thanks for the heads up!
```

---
## \#34 Posted by: danielz Posted at: 2017-10-11T01:58:39.559Z Reads: 405

```
Thank you, reading i had to enable uart helped me. I had to set baud to 9600 too
```

---
## \#35 Posted by: jalapeno_ninja Posted at: 2018-04-16T04:33:26.508Z Reads: 313

```
Hi All,

I installed the HM-10 module and used it / got a read out on the app, now it's stopped. Looking around the pins of the HM-10 + heat shrink I applied, there's white clouding. I'm guessing that I've got the 5V to 3.3V issue.

Can anyone please explain what resistors are required and how/where to solder them in? (Complete beginner here to resistors etc)

Much appreciated!
```

---
## \#37 Posted by: jalapeno_ninja Posted at: 2018-04-16T04:43:39.583Z Reads: 295

```
Yep I did, but the posts that followed that said it was incorrect? (And I'm not sure what 1K ohm / 2K ohm resistors are to buy).
```

---
## \#38 Posted by: ZackoryCramer Posted at: 2018-04-16T04:54:00.790Z Reads: 300

```
[quote="jalapeno_ninja, post:37, topic:12838"]
Yep I did, but the posts that followed that said it was incorrect?
[/quote]
Can you reference the post? The resistors assembled in a T junction is a simple method of cutting down voltage which that guy didn't seem to understand. :smile:

[quote="jalapeno_ninja, post:37, topic:12838"]
what 1K ohm / 2K ohm resistors
[/quote]

Resistance is the only main parameter that defines a resistor. Any new resistor with that resistance will do. :grinning:
```

---
## \#39 Posted by: jalapeno_ninja Posted at: 2018-04-16T04:58:39.713Z Reads: 285

```
Reference post: http://www.electric-skateboard.builders/t/vesc-hm-10-bluetooth-wiring/12838/19?u=jalapeno_ninja
```

---
## \#40 Posted by: ZackoryCramer Posted at: 2018-04-16T05:04:35.383Z Reads: 284

```
oh wait ur right. Didn't see that coming. But I would highly doubt its the overvoltage causing the trouble. 
I had problems like that in the past and what I would do is restart my phone and it works again. :stuck_out_tongue_winking_eye:
```

---
## \#41 Posted by: Acido Posted at: 2018-04-16T05:14:11.165Z Reads: 288

```
Check your wires, maybe you did not solder them very well and somehow something broke???

Hm10 modules usually work on 5v...
```

---
## \#42 Posted by: driver Posted at: 2018-04-26T18:15:12.978Z Reads: 292

```
Mine was working, but now it stoped... i updated both vescs to 3.101 (Ackmaniac).
I set the PPM and UART, 9600bps
BT Modul is blinking slowly, my phone finds a "unknown device", but i cant connect to it.

![2018-04-26 20_05_24-ESC Tool|690x438](upload://5DizM2HZY46BJPAT4UpSa17numa.jpg)
```

---
## \#43 Posted by: louwii Posted at: 2018-04-26T22:23:48.370Z Reads: 274

```
Android phone? Android 8 has issues with a lot of HM10 bluetooth modules.
```

---
## \#44 Posted by: mmaner Posted at: 2018-04-27T02:13:00.328Z Reads: 274

```
I got some new hm-10s from @JLabs, they work with my Android 8 phone.  The metr adaptor still doesn't. Not sure what the issue is but I'm sticking with the @Ackmaniac app I guess.
```

---
## \#45 Posted by: driver Posted at: 2018-04-27T05:30:00.623Z Reads: 267

```
Its 8.0. :-/
I Heard about the restrictive bt protocol in 8.0.

Thanks for the Tipp! I am in Germany, so ordering from the US is time and cost intensive. So I'd like to buy it in the EU. 
 Do you know how I know which Modul will work?
```

---
## \#46 Posted by: mmaner Posted at: 2018-04-27T11:49:38.555Z Reads: 258

```
You'd have to ask @JLabs, I have no idea where he sourced them.
```

---
## \#47 Posted by: rey8801 Posted at: 2018-04-27T11:59:23.071Z Reads: 256

```
You can try to ask here HM-10 Transparent Serial Port Bluetooth 4.0 Modules Bluetooth Serial Port With Logic Level Transformation
 http://s.aliexpress.com/FJBJJ3qI?fromSns=Copy to Clipboard to the seller if it is actually original. Based on the post https://blog.yavilevich.com/2016/12/hm-10-or-cc41-a-module-automatic-arduino-ble-module-identification/ it seems legit. Of course more expensive than the clone.
```

---
## \#48 Posted by: tm0587 Posted at: 2018-05-07T17:10:27.078Z Reads: 243

```
Just want to clarify, do I or do I not need the resistors to cut down 5V to 3.3V? If yes, which is the right wiring? I see two diagrams in this thread, but the first one was declared wrong, and the second one did not contain any resistors. Any help appreciated!
```

---
## \#49 Posted by: Pimousse Posted at: 2018-05-07T20:12:53.607Z Reads: 239

```
No need of resistors.
```

---
## \#50 Posted by: tm0587 Posted at: 2018-05-07T23:36:51.769Z Reads: 234

```
Awesome, thanks! You just saved me a bunch of money, the HM-10 modules are ridiculously cheap on Taobao, like $1 each.
```

---
## \#51 Posted by: Pimousse Posted at: 2018-05-08T03:53:26.310Z Reads: 230

```
I may want to buy original HM10 module, not cheap copies.
We have tons of issues with copies and lzst versions of Android.
```

---
## \#52 Posted by: tm0587 Posted at: 2018-05-08T06:18:59.999Z Reads: 226

```
Hmmm anyway to tell them apart? Besides the price, of course.

Though at $1 a piece, there's little risk to buying one to try.
```

---
## \#53 Posted by: Pimousse Posted at: 2018-05-08T07:01:21.079Z Reads: 218

```
$1 modules won't work for sure with Android 8 without a workaround (or a firmware upgrade of the chip which is a bit tricky).
```

---
## \#54 Posted by: tm0587 Posted at: 2018-05-08T07:49:07.094Z Reads: 214

```
I would think most Android phones are stuck with older versions of Android and that Android 8 is abit of a rarity.

I don't think it'll be an issue for me, I have at least 1 phone still running Android 7, so I can use that for now.
```

---
## \#55 Posted by: Pimousse Posted at: 2018-05-08T09:11:09.159Z Reads: 215

```
Sure Android 8 is not well deployed yet. But it will more and more.
Is it worth saving $5 on a $1000+ build for an already obsolete device ?
My advice : buy an official HM-10 and drink a beer less. it's worth it. ;)
```

---
## \#56 Posted by: Drehfeld Posted at: 2018-06-15T14:16:42.203Z Reads: 197

```
I think now I tried everything to get one of the common apps working to monitor the VESC.
But I still do not get communication. I do find the bluetooth device (tried different ones HM-11,10 older green ones) but it does not matter what I do, the app (vesc connect pro & vesc Monitor) does not response. 
I do have a maytech clone (e-greenmotion), installed the bootloader and new firmware (13.04.2018) changed the settings to PPM and UART. I crossed the RX and TX wires (also flipped this 2 for testing) and do power the bluetooth module with 3,3V. I did read the whole treat but could not find my mistake.
Did I miss something or does not one of the 4 bluethooth moduls work for this simple task? 
"No firmware Read response" sometimes pops up.
Thanks for your help.
```

---
## \#57 Posted by: rey8801 Posted at: 2018-06-15T14:29:29.983Z Reads: 191

```
Which module do you have (how do they hsow up on your phone? Which phone do you have?
I power the module with 5V but also with 3.3V I tried and it works.
```

---
## \#58 Posted by: Drehfeld Posted at: 2018-06-15T16:00:44.316Z Reads: 190

```
HMSoft is written in the list of my huawei P9.
Changed to 5V but still the same problem.
I did get a totally new one that is HM-10 from keyestudio Bluetooth 4.0 V2
VESC Firmware is 3.38 HW 410
```

---
## \#59 Posted by: rey8801 Posted at: 2018-06-15T16:11:21.943Z Reads: 199

```
Definetely the bluetooth module should work. Really wierd. At which step you see the problem adn which app are  you trying to use?

Edit:
Can you post a pic of the wiring on the module and the JST connector? Also the uart port on your vesc
```

---
## \#60 Posted by: Drehfeld Posted at: 2018-06-17T16:15:46.563Z Reads: 207

```
Thanks for your help. I made a picture but I´m sure there is no misstake. It also the same like on [this pic](http://www.electric-skateboard.builders/t/vesc-hm-10-bluetooth-wiring/12838/19?u=drehfeld).
The app is VESC Connect by jacob bloy.
In the app I do find the module but can not communicate (I can not read the config, start the motor...)![IMG_20180617_180914|374x500](upload://uBZMHCMYPde3cnU54Qf0j2dvV6K.jpg)
```

---
## \#61 Posted by: Minim Posted at: 2018-06-17T18:52:23.575Z Reads: 211

```
Does something else need to be done to find the bluetooth module with my phone? I've wired it up to a Escape (vesc6) with tx/rx crossed and gnd/5v to the gnd/vcc pin of the HM10 module. HM10 is speced for 3.6-6volts so I use the 5v pin on the escape and not the 3.3v vcc pin since it's to low. The bluetooth module is blinking red with 1hz approx and I can't find it when searching with my phone.

Edit. forgot to add that I use a ebay genereic HM10 module with metr and petimetr app on Iphone X.
```

---
## \#62 Posted by: mmaner Posted at: 2018-06-17T19:18:26.008Z Reads: 210

```
Metr won't see the generic module. It has to be the metr module. With the generic hm-10 set the baudrate to 9600bps, download the @Ackmaniac app.
```

---
## \#63 Posted by: Minim Posted at: 2018-06-17T19:21:28.252Z Reads: 204

```
I found it with a bluetooth scanner so it's prolly the issue. Is the ackmaniac app the "eskate VESC" app that's paid?

Edit:

Working with the paid eskate app.. Neat! Thanks @mmaner
```

---
## \#64 Posted by: rey8801 Posted at: 2018-06-17T21:55:30.224Z Reads: 200

```
Yeh if the wiring is correct and you set PPM + UART in the VESC tool then you try to use another phone or another module. There isn't that much more do it. If already tried that can be the VESC the problem. If you have access to a 4.12 hardware you could give it a try. One thing you can try immidiately is download a BLE app like BLE SCANNER, find your module and connect to it. You should see the red blinking led become fixed once connected. If that works than you app should work too. If that doesn't work than you have a problem and usually is the module, but you can easily try with another phone too.
```

---
## \#65 Posted by: achatham Posted at: 2018-07-12T04:02:19.811Z Reads: 181

```
Where and what is the cable that connects the hm-10 to the vesc? Thanks.
```

---
## \#66 Posted by: Travo Posted at: 2018-08-13T19:24:21.678Z Reads: 153

```
I've received my bt module (3.6v - 6v) and I have the necessary cables to attach it to the vesc. Do I have to do any programming to the vesc via vesc tool to get this to work or can it just plug and play
```

---
## \#67 Posted by: Travo Posted at: 2018-08-13T19:24:54.873Z Reads: 150

```
Jst 6 pin I believe is what it's called
```

---
## \#68 Posted by: nuttyjeff Posted at: 2018-08-14T02:06:29.879Z Reads: 149

```
Jst-ph 5, 6 or 7 pins will work with the hm-10.
```

---
## \#69 Posted by: b264 Posted at: 2018-10-05T18:59:53.657Z Reads: 112

```
For those landing here, the image above is no longer working, but try https://www.electric-skateboard.builders/t/bt05-a-wolf-in-hm-10-clothing/45243?u=b264
```

---
## \#70 Posted by: QGruschkof Posted at: 2018-11-26T17:34:12.231Z Reads: 96

```
Hez which FW are zou using on your VESC. I connected everything set everything up but my Android app still says esc not connected. What do you think is the problem?? I have a VESC HW 4.12 and the FW 3.40 installed and everything setup (baud rate, PPM and UART) Thanks
```

---
## \#71 Posted by: ricoghardforth Posted at: 2018-12-14T16:34:49.097Z Reads: 91

```
Me in my infinite wisdom have encased my Vesc in a aluminium enclosure and don't really want to hack out a slot in the case to poke out my HM10 PCB antenna.  

I was thinking if I cut the PCB trace and solder on a wire wip antenna from a broken  2.4ghz FS-GR3E rc receiver.  Then I could then just simply drill a small hole and poke the wire out.   Would this work its only got to transmit as far as my pocket.   What length should I use vaguely to remember something about quarter the wave form or something. 

While I'm on the subject could I do something similar to the rc receiver of the Winning remote which doesn't have a wire antenna.  I've had to swap this with my sons mini remote which has the wire antenna so I can poke it out of the enclosure.

Thanks

Rich
```

---
## \#72 Posted by: ricoghardforth Posted at: 2018-12-15T17:02:13.078Z Reads: 75

```
Turns out the HM10 transmits fine through my enclosure and for a few metres not just a few feet so I needn’t of worried.  
May have to try the winning remote receiver and see if that works as well.
```

---
