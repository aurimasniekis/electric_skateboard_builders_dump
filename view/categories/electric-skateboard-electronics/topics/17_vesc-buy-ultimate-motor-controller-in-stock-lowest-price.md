# VESC - Buy Ultimate Motor Controller - In Stock &amp; Lowest Price

### Replies: 132 Views: 28276

## \#1 Posted by: onloop Posted at: 2015-07-12T04:07:25.063Z Reads: 768

```
[<img src="/uploads/db1493/original/2X/9/93e44d7810e9b81981a6dd41b89b056aea21e14d.png" width="690" height="333">](http://www.enertionboards.com/electric-skateboard-parts/FOCBOX-programmable-brushless-motor-controller/)

VESC TECHNICAL SPECIFICATIONS:

The hardware and software is open source. Since there are plenty of CPU-resources left, the customization possibilities are almost endless.
STM32F4 microcontroller.
DRV8302 MOSFET driver / buck converter / current shunt amplifier.
IRFS3006 MOSFETs (other FETs in the same package also fit).
5V 1A output for external electronics from the buck converter integrated on the DRV8302.
Voltage: 8V – 60V (Safe for 3S to 12S LiPo).
Current: Up to 240A for a couple of seconds or about 50A continuous depending on the temperature and air circulation around the PCB.
Firmware based on ChibiOS/RT.
PCB size: slightly less than 40mm x 60mm.
Current and voltage measurement on all phases.
Regenerative braking.
Sensored or sensorless operation.
A GUI with lots of configuration parameters
Adaptive PWM frequency to get as good ADC measurements as possible.
RPM-based phase advance (or timing/field weakening).
Good start-up torque in the sensorless mode (and obviously in the sensored mode as well).
The motor is used as a tachometer, which is good for odometry on modified RC cars.
Duty-cycle control, speed control or current control.
Seamless 4-quadrant operation.
Interface to control the motor: PPM signal (RC servo), analog, UART, I2C, USB  or CAN-bus.
Wireless wii nunchuk (Nyko Kama) control through the I2C port. This is convenient for electric skateboards.
Consumed and regenerated amp-hour and watt-hour counting.
Optional PPM signal output. Useful when e.g. controlling an RC car from a raspberry pi or an android device.
The USB port uses the modem profile, so an Android device can be connected to the motor controller without rooting. Because of the servo output, the odometry and the extra ADC inputs (that can be used for sensors), this is perfect for modifying an RC car to be controlled from Android (or raspberry pi).
Adjustable protection against When the current limits are hit, a soft back-off strategy is used while the motor keeps running. If the current becomes way too high, the motor is switched off completely.
Low input voltage
High input voltage
High motor current
High input current
High regenerative braking current (separate limits for the motor and the input)
Rapid duty cycle changes (ramping)
High RPM (separate limits for each direction).
The RPM limit also has a soft back-off strategy.
Commutation works perfectly even when the speed of the motor changes rapidly. This is due to the fact that the magnetic flux is integrated after the zero crossing instead of adding a delay based on the previous speed.
When the motor is rotating while the controller is off, the commutations and the direction are tracked. The duty-cycle to get the same speed is also calculated. This is to get a smooth start when the motor is already spinning.
All of the hardware is ready for sensorless field-oriented control (FOC). Writing the software is the remaining part. However, I’m not sure if FOC will have many benefits for low inductance high-speed motors besides running a bit quieter.
```

---
## \#2 Posted by: cmatson Posted at: 2015-07-19T03:09:17.779Z Reads: 535

```
I've read a lot of the ES posts regarding VESC's, but am still kinda confused on the setup. Do you need to tinker with it, and change setting based on your motor, gearing, etc? Or can you just hook it up and run it stock? I know there are all sorts of cool things the vesc allows you to do, but to be honest, I wouldn't really tap into that unless it was super easy and seamless. I also don't have a computer running linux, so I don't see how I would be able to change the settings. I haven't even seen a receiver lead on a vesc, so how do you control the beast?
```

---
## \#3 Posted by: onloop Posted at: 2015-07-23T00:17:56.597Z Reads: 527

```
The setup is what scares most people, originally you needed linux on your PC. Then you needed to follow about 20 steps to configure it, which was actually fairly straight forward. I had never installed linux, but within about an hour i had it setup and had the vesc configured.

However, all that is in the past. There has been windows & mac versions of the software developed so now you just install from your normal PC.

The VESC does need to be configured specifically for your motor, but that is why it is so good! It knows the parameters of your motor so it can perform at max efficiencies. The configuration is automated. Basically you connect the motor & press a button, it gives you some numbers which you type into a screen & click update.

There is also an android app being developed.

You are right the VESC has lots of features that are not important to most people. But what is important are:
1. Its open source, so people will be able to work on it and constantly make it better. like FOC
2. It is actually really compact, so it makes building a slim eboard easy.
3. It doesn't get hot. So don't need big fans or heat sinks
4. The performance is very good. You can start from stationary with non-sensor motors.
5. It is also hall sensor compatible, if you have them installed into your motor it will auto detect them and use them to further improve start up torque performance.
6. The brake functions really nicely. Very progressive & feels well balanced.... it doesn't feel like your going to get sling-shot off the board because you tapped the brake slightly too hard.
7. Last but not least, it has built in safety features. Temperature & Current control. this is the single biggest advantage. It is easy to blow your motors pulley to many amps... It can't happen with the VESC. 

Basically it is the best ESC ever made. Well at least that is what the creator Ben Vedder set out to achieve when he started building it.
```

---
## \#4 Posted by: onloop Posted at: 2015-07-23T00:20:41.815Z Reads: 423

```
**WARNING - VESC PRICE RISE**
Due to production cost increases and the diminishing value of the Australian Dollar

VESC - ADVANCED OPEN SOURCE MOTOR CONTROLLER
The VESC is becoming a world wide hit amoungst RC & DIY Enthusiats & It is our mission to ensure as many people as possible can get there hands on one of these 'Pre-Assembled' open source motor controllers at a great price.

Currently we offer "pre-assembled" VESC for purchase online at www.EnertionBoards.com
USD $115
EURO $105
POUND $74
AUD $154.60 (New Price $169.00)
Shipping in August.




AUD PRICE WILL RISE 10% IN 24 HOURS
-----------------------------------


[BUY NOW & LOCK IN PRICE][1]


  [1]: http://www.enertionboards.com/electric-skateboard-parts/vesc-beta-membership/?setCurrencyId=1
```

---
## \#5 Posted by: onloop Posted at: 2015-08-07T05:18:02.646Z Reads: 405

```
<img src="/uploads/db1493/original/1X/2137d2dc849e7d6e0dd91e7de0cd6317e013c31e.jpg" width="666" height="500"> 
<img src="/uploads/db1493/original/1X/607073c92f0eafc9dbe5f6c11d3c0ae31314bde5.jpg" width="666" height="500">
```

---
## \#6 Posted by: Wanderer Posted at: 2015-08-09T02:02:52.985Z Reads: 371

```
Not one for the electronics side of the spectrum (will have to learn eventually), but this looks seriously sexy! Looking forwards to strapping them under my current build!
```

---
## \#7 Posted by: Wanderer Posted at: 2015-08-09T02:03:47.133Z Reads: 374

```
On a side note, are you planning on any sort of enclosures for these beauts?
```

---
## \#8 Posted by: onloop Posted at: 2015-08-09T04:51:44.503Z Reads: 370

```
I did design a 3D printed enclosure, however I don't have a 3D printer & it was really expensive to print. I think Shrink tube is suitable for now.
```

---
## \#9 Posted by: lowGuido Posted at: 2015-08-09T06:49:21.335Z Reads: 358

```
[quote="onloop, post:1, topic:17"]
Wireless wii nunchuk (Nyko Kama) control through the I2C port. This is convenient for electric skateboards.
[/quote]

Can you please clarify this for me? does that mean that this VESC does not need an arduino board to use the nunchuck. The nunchuck can interface directly to the ESC?
```

---
## \#10 Posted by: elkick Posted at: 2015-08-09T09:21:12.465Z Reads: 346

```
You only need the Nunchuk receiver to be connected to  I2C, the rest is built into the VESC. No Arduino anymore :-) 
Works great! 

I still think that the nRF solution might add security  and since Benjamin already implemented it into the VESC FW I'm going to try it as well. Nunchuk has to be modified with an Nano & nRF though, testing it at the moment. Jacob seems to be a little bit further though I guess with this approach.
```

---
## \#11 Posted by: lowGuido Posted at: 2015-08-09T10:28:34.703Z Reads: 343

```
Thats one big selling point right there.
```

---
## \#12 Posted by: Wanderer Posted at: 2015-08-09T16:38:07.694Z Reads: 339

```
Fair enough. 
What are the overall dimensions of the vesc? Just to get an idea of how much space it will take up under my board.
```

---
## \#13 Posted by: elkick Posted at: 2015-08-09T19:32:06.663Z Reads: 349

```
40x60mm without the capacitor. It depends how the battery cables are placed. It might add another 20mm. The motor wires could be skipped also and the connectors could be soldered directly to the board. <img src="/uploads/db1493/original/1X/f14c610e4b8944fcbddfe27e7080da2ab4b34b87.jpg" width="666" height="500">
```

---
## \#14 Posted by: Wanderer Posted at: 2015-08-09T20:27:46.359Z Reads: 334

```
Cool thanks a lot, wont take up much room at all than.
```

---
## \#16 Posted by: csfrasher Posted at: 2015-08-26T14:40:55.882Z Reads: 325

```
@onloop do you mind posting that design. I have a buddy who has a 3d printer and i could probably make a few and put them on here for pretty cheap.
```

---
## \#17 Posted by: onloop Posted at: 2015-08-26T22:04:39.861Z Reads: 322

```
The case I designed is not very good... it is not a finished product
```

---
## \#18 Posted by: onloop Posted at: 2015-10-19T07:04:21.725Z Reads: 324

```
**VESC v4.10 OCTOBER BATCH SOLD OUT**


next batch due mid november
===========================
```

---
## \#19 Posted by: yendi Posted at: 2015-10-19T19:44:30.365Z Reads: 317

```
As the VESC are in "beta" should we be worried of some PCB changes? Or is the hardware design definitive ?
```

---
## \#20 Posted by: Quickfeet Posted at: 2015-10-19T20:24:23.418Z Reads: 318

```
I ordered 2 from your site last night...the page said still October release. Please tell me I missed the cut off
```

---
## \#21 Posted by: onloop Posted at: 2015-10-19T21:57:28.272Z Reads: 310

```
Actually I sold out about one week ago. 

So lots of people missed the cutoff.
```

---
## \#22 Posted by: cmatson Posted at: 2015-10-20T01:26:48.313Z Reads: 268

```
darn, that means I missed the cutoff :sob:

next one won't be for a month or two I'm assuming...
```

---
## \#23 Posted by: disastorm Posted at: 2015-10-20T21:32:19.974Z Reads: 265

```
@onloop Did mine make it before the cut off?
```

---
## \#24 Posted by: locktight Posted at: 2015-10-21T18:14:44.714Z Reads: 266

```
@chaka sells vescs if you missed the cutoff I believe they are still in stock
```

---
## \#25 Posted by: onloop Posted at: 2015-10-21T23:44:04.629Z Reads: 265

```
if your order number is greater than 1133 you likely missed out on this vesc batch. don't worry the next batch will follow very quickly as we have ironed out lots of issues with this current batch.
```

---
## \#26 Posted by: emotiva Posted at: 2015-10-22T03:27:25.777Z Reads: 263

```
What kind of issues are you having with this batch?

Edit: Never mind, I misread that.
```

---
## \#27 Posted by: onloop Posted at: 2015-10-22T03:35:33.467Z Reads: 268

```
getting them made quickly!
```

---
## \#28 Posted by: onloop Posted at: 2015-10-22T03:36:58.323Z Reads: 278

```
halting production half way, re-making different PCB, making new stencil for PCB, fucking around doing stupid shit....

blah blah blah... FUCK

the fun of manufacturing...
```

---
## \#29 Posted by: onloop Posted at: 2015-10-30T03:09:19.425Z Reads: 295

```
VESC VERSION 4.10 - FINALLY READY
=================================

One month overdue! :sob: sorry for all the people who have been patiently (& the impatient ones too) waiting

it will take a few more days before they get shipped out to you.

1. So they are going to ship today from factory to me, that can take 3-5 days (not including weekends)
2. I need 1-2 days to testing & firmware loading
3. 1-2 days for packing orders
4. 2-5 days shipping to your address. 
Best case 7 days Worst case maybe 14 days. I suspect it will be around 10 days. this is assuming no other major hold up with customs or act of god.

<img src="/uploads/db1493/original/1X/771487b9592c4b3b44a982a7df82e7bed8e70a6a.jpg" width="375" height="500"><img src="/uploads/db1493/original/1X/ab01977357bdb2a79931b9b56bbafaf0a1efd23f.jpg" width="375" height="500"><img src="/uploads/db1493/original/1X/c3d0c29496f878a4d4c1c00bed4e4085390f7358.jpg" width="666" height="500"><img src="/uploads/db1493/original/1X/2cff17d833fa69916fbed7787493cdccd54dfdb0.jpg" width="375" height="500"><img src="/uploads/db1493/original/1X/5da67cdd36254e28895fa3abff3ba98665815842.jpg" width="666" height="500">
```

---
## \#30 Posted by: cmatson Posted at: 2015-10-30T04:25:13.163Z Reads: 258

```
lol, when will the next batch start shipping?

yes, I'm that guy...
```

---
## \#31 Posted by: onloop Posted at: 2015-10-30T04:26:48.590Z Reads: 252

```
each batch should take about one month each. so in theory late november

i am hoping quicker now that the issues have been ironed out...
```

---
## \#32 Posted by: onloop Posted at: 2015-10-30T04:31:06.571Z Reads: 255

```
also.. much-much-much quicker if i didn't have to spend time answering emails asking when stuff would be ready :stuck_out_tongue: :)
```

---
## \#33 Posted by: disastorm Posted at: 2015-10-30T05:23:39.126Z Reads: 250

```
Congrats thats good to hear the VESC issues have been solved
```

---
## \#35 Posted by: BigAl Posted at: 2015-10-30T17:11:39.274Z Reads: 243

```
I placed my order this week, its order #1315, am I in this batch?

Technically this is not the same as asking "when stuff would be ready :stuck_out_tongue: :smile:".

Thanks
Al...
```

---
## \#36 Posted by: Jeff Posted at: 2015-10-30T17:21:45.653Z Reads: 237

```
According to @onloop, order #1133 was the cutoff for this batch.
```

---
## \#37 Posted by: BigAl Posted at: 2015-10-30T17:32:37.970Z Reads: 247

```
just saw that, thanks

oh darn, waiting patiently...

Al...
```

---
## \#38 Posted by: longhairedboy Posted at: 2015-10-30T17:36:55.794Z Reads: 233

```
I really just need to order a few of these and be done with it. I've been waiting for revisions to slow down and the batch process to iron out a little more so that the wait times weren't as bad, but i think i'm just going to bite it next month and get a small batch. I think things are about as ironed out as they're going to get for a while.
```

---
## \#39 Posted by: onloop Posted at: 2015-10-30T22:43:12.840Z Reads: 266

```
I'm taking drastic steps to ensure that demand no longer outstrips supply.......

I would really like a board to ride too.... if it makes you all feel better I also have not had a vesc now for several months as I have had to keep selling the personal ones that I set aside.

The biggest problem is people hitting the site ordering in lots of 10, 12 etc. I had like 4 or 5 orders like this happen in a few days of each other... it totally wiped out the stock. It takes one month to get a batch made... so when you sell a months worth in a few days and it takes a month to get more you are now 2 months behind... so i need to order like 3 or 4 months worth.... thats a hell of an upfront investment 

So I am waiting also... patiently
```

---
## \#40 Posted by: chaka Posted at: 2015-10-31T10:08:40.699Z Reads: 285

```
I made my oshpark V4.10 VESC file public today for anyone wanting to build one of their own. It can be a fun little project assembling these little gems.

[vedder's_esc_4.10][1]

<img src="/uploads/db1493/original/1X/add1e090cc5a1cf278658629f899ede089a1fe73.jpg" width="370" height="500">


  [1]: https://oshpark.com/shared_projects/NNzfrwPG
```

---
## \#41 Posted by: kai Posted at: 2015-10-31T12:52:27.201Z Reads: 289

```
So with the board capacitors and wires, what is the full dimensions? With the regular jst plugs and wires not right angle ones. I would like to start building my enclosure this week. Would you guys suggest a seperate enclosure for space cell and another for the dual vesc? Or just one enclosure? I would like to run my motor wires in parallel to the vesc not in a big wad.
```

---
## \#42 Posted by: chaka Posted at: 2015-10-31T14:32:48.764Z Reads: 273

```
The whole assembly with capacitor board measures 110mm long with a 5mm gap between the two and 40 mm wide. 

For the enclosure my only advise is to be sure you can access the usb ports of the VESC's easily and allow for some passive ventilation, it doesn't take much.
```

---
## \#43 Posted by: kai Posted at: 2015-10-31T14:42:14.953Z Reads: 274

```
Thanks for the advice.  what about height off the deck with jst ph plugs in? I guess the only way to provide easy access to the usb because i am running two would be to run them long ways and not side by side. Do you typically mount the vesc directly to the board?
```

---
## \#45 Posted by: onloop Posted at: 2015-11-02T06:05:37.033Z Reads: 278

```
<img src="/uploads/db1493/original/1X/e5ec87b13eadca390a652e55a58eb46e9d2f7bab.jpg" width="690" height="388"><img src="/uploads/db1493/original/1X/f2640d3722d8d76fa1ef64d067cef54d9de0e8bf.jpg" width="690" height="388">

VESC finally arrived.

Busy next few days.... Try not to bother me too much ;)
```

---
## \#46 Posted by: Batou Posted at: 2015-11-03T13:43:23.838Z Reads: 260

```
Nice ! Thank you very much, I m looking forward to receive it !

On another forum, a guy noticed the UART port has now 7 pins. Does anyone know how to wire the Nyko Kama dongle in this configuration ?
```

---
## \#47 Posted by: disastorm Posted at: 2015-11-05T02:03:00.983Z Reads: 308

```
> Nice ! Thank you very much, I m looking forward to receive it !

> On another forum, a guy noticed the UART port has now 7 pins. Does anyone know how to wire the Nyko Kama dongle in this configuration ?

Can anyone answer this? I bought the 6-pin connectors thinking that would be good enough. Its a good thing I didn't solder them to the Nyko Receiver yet. What kind of connectors do we need now ?
Is this what we need: http://www.ebay.com/itm/JST-2-0-PH-7-Pin-Female-Connector-with-Wire-and-Male-Connector-x-10-Sets-/121367876323?hash=item1c4216d2e3:g:OvoAAOxyKsZRy55z ?

  [1]: http://Link
```

---
## \#48 Posted by: jacobbloy Posted at: 2015-11-05T13:48:14.353Z Reads: 312

```
Hi mate, you don't need a 7pin connector, I use a 6pin connector still, the end pin is 5v don't need it, <img src="/uploads/db1493/original/1X/e6452b92323accccd88b313d269d7b3942db96d9.jpeg" width="666" height="500">

But the extra pins are for connecting a nrf24 chip not the nyko kama so you will be fine any way.
```

---
## \#49 Posted by: chaka Posted at: 2015-11-05T14:32:32.197Z Reads: 303

```
I have 7 pin connectors. I am going to make some adapters with the Nunchucky breakout board if anyone is interested. I'll have a listing up in my online shop soon.
```

---
## \#50 Posted by: Batou Posted at: 2015-11-05T15:05:53.248Z Reads: 300

```
@jacobbloy : thanks for the answer, it's a relief :smile:
@chaka : For now I have the Kama dongle, but apparetly it may loose connection so I will probably check your website.
```

---
## \#51 Posted by: chaka Posted at: 2015-11-05T15:09:55.039Z Reads: 290

```
You still use the dongle, it just makes it easy to connect the dongle to the vesc. If you have some soldering skills it is best to solder directly to the dongle's PCB.
```

---
## \#52 Posted by: disastorm Posted at: 2015-11-05T18:42:29.293Z Reads: 299

```
[quote="jacobbloy, post:48, topic:17"]
Hi mate, you don't need a 7pin connector, I use a 6pin connector still, the end pin is 5v don't need it,
[/quote]
Thanks for the info. I don't know much about connectors, so all 6 pin JST-PH connectors should fit the 7 pin socket right, they are standardized ? This is the one I have http://www.ebay.com/itm/JST-2-0-PH-6-Pin-Female-Connector-with-Wire-and-Male-Connector-x-10-Sets-/111386693164?hash=item19ef2a0e2c:g:HYgAAOxyRHdRy55H

Just wanted to verify before i solder it.
```

---
## \#53 Posted by: Batou Posted at: 2015-11-05T18:58:45.088Z Reads: 287

```
@chaka : Ok I got it. For some reason I thought the nunchucky was a different brand of wireless nunchuck. But in your opinion is it realy hard to solder the dongle directly to the VESC? Do you solder the thin dongle wires that are already there ?
```

---
## \#54 Posted by: jacobbloy Posted at: 2015-11-05T20:18:48.129Z Reads: 273

```
Correct that is right
```

---
## \#55 Posted by: chaka Posted at: 2015-11-05T21:17:18.371Z Reads: 273

```
You can, it is really personal preference. I like to use connectors first and once it is confirmed as working I then solder it in
```

---
## \#56 Posted by: lowGuido Posted at: 2015-11-06T01:45:54.796Z Reads: 288

```
Yeah I like that idea. Test with plugs and then solder.
I wouldn't run a skateboard with plugs or adapters because it's just one more point of failure added to the mix. None of this stuff is designed to withstand the amount of shock and vibration of skateboarding.
```

---
## \#57 Posted by: disastorm Posted at: 2015-11-07T05:42:48.711Z Reads: 293

```
Hey @jacobbloy @chaka or anyone, can you tell me if the diagram from this guide is correct ?? Looking at the VESC pinouts i think it might be outdated now? http://www.electric-skateboard.builders/t/vesc-faq-connect-the-nyko-kama-wireless-wii-nunchuck/139

Here are the VESC pinouts https://raw.githubusercontent.com/vedderb/bldc-hardware/master/design/PNGs/3D_back.png

the 3 bottom pins ( left most in the diagram ) are ADC2,RX,TX while the forum thread guide shows them as RX_SCL, TX_SDA, ADC_EXT

Is the guide outdated ?
```

---
## \#59 Posted by: disastorm Posted at: 2015-11-07T06:17:25.130Z Reads: 307

```
[quote="chaka, post:58, topic:17, full:true"]
ADC2 was added in the latest hardware update, the rest of the pinouts are the same. If I get a chance I will wire up a v4.10 with a dongle and confirm.
[/quote]

Thanks for confirming. That is what it looks like to me as well. @jacobbloy's comment confused me since he mentioned the 5v

[quote="jacobbloy, post:48, topic:17, full:true"]
Hi mate, you don't need a 7pin connector, I use a 6pin connector still, the end pin is 5v don't need it, <img src="/uploads/db1493/original/1X/e6452b92323accccd88b313d269d7b3942db96d9.jpeg" width="666" height="500">

But the extra pins are for connecting a nrf24 chip not the nyko kama so you will be fine any way.
[/quote]

so @jacobbloy must have made resoldered a new connector for 4.10 ? If he was reusing his old 6-pin theres no way that position in that photo would work right ?

*edit I just took a look at some of the older diagrams and the schematic on Vedders site and it does look like you are right, the pinouts are the same with the addition of the ADC2
```

---
## \#60 Posted by: disastorm Posted at: 2015-11-07T06:52:31.523Z Reads: 304

```
crap i just noticed my Nyko Kama receiver doesn't match the one from the guide either... have any of you guys seen this variant of the nyko kama receiver?
<img src="/uploads/db1493/original/1X/f3e8641ab8b752a14b420309bcf4a2d757384733.jpg" width="375" height="500">
<img src="/uploads/db1493/original/1X/b99a8554cb39b4b70c5430e27f11230beffea291.jpg" width="375" height="500">
*edit nevermind I found a diagram of the wii socket pins and was able to map this version of the nyko kama to the correct pins
```

---
## \#61 Posted by: jacobbloy Posted at: 2015-11-07T07:04:24.358Z Reads: 286

```
I was simply demonstrating that the 6pin plug works if the wires don't match you can do a pop and swap of the wires in the plug.
```

---
## \#62 Posted by: disastorm Posted at: 2015-11-07T07:17:34.012Z Reads: 276

```
ah i see, that makes sense.
```

---
## \#63 Posted by: trbt555 Posted at: 2015-11-07T07:58:06.938Z Reads: 269

```
Do you have a source for that pinout ?
```

---
## \#64 Posted by: disastorm Posted at: 2015-11-07T08:53:07.330Z Reads: 282

```
I actually have the little converter pcb thing in this post:
http://duino4projects.com/wii-nunchuck-arduino-tutorial/

So that labelled the pins for me before I cut the wires to the head.

Heres a random diagram from google images that seems to be consistent with the convert pcb thing:
<img src='/uploads/db1493/original/1X/a5cebf02b5022f8c5d7da7ab4bf471bcb4f80641.jpg'>

Keep in mind this view is looking at it from the front. When you look at it from the back ( the part will you will cut the wires ) the left and right will be opposite.
```

---
## \#65 Posted by: lowGuido Posted at: 2015-11-07T08:56:18.766Z Reads: 266

```
Wow. Thats a crazy large nyko kama reciever. I have not seen one like that before.
```

---
## \#66 Posted by: disastorm Posted at: 2015-11-07T09:15:34.156Z Reads: 272

```
Well the pinout image is not the nyko kama, thats just the standard wiimote pinout i found on a site. I don't know what device that is. Or are you referring to my actual photos with me holding the pcb ?

Anyway I just finished soldering it to the connector.  I don't have the vescs yet so can't test it out, hopefully my soldering wasn't too bad lol.
```

---
## \#68 Posted by: onloop Posted at: 2015-11-29T21:45:59.297Z Reads: 255

```
NICE!.... vesc art!.. looks cool.
```

---
## \#69 Posted by: onloop Posted at: 2015-12-03T06:55:20.241Z Reads: 243

```
A post was split to a new topic: [THE DUAL VESC | Integrated Design - 2 Motor Controllers 1 PCB](/t/the-dual-vesc-integrated-design-2-motor-controllers-1-pcb/640)
```

---
## \#70 Posted by: Braylon31 Posted at: 2015-12-03T08:46:24.104Z Reads: 253

```
Can you post a dia gram with the 7 pin connecter as im sure being able to see it will cuase less confusion because its not much mention and i would hate to fry my vesc cuase of wrong  wiring  @jacobbloy if you understand can you please post pic im checking diagrams jus wanna be sure of rite connection who woula thought one pin could mean so much i have no ifea what a adc2 is scares the hell outta me lol
```

---
## \#71 Posted by: jacobbloy Posted at: 2015-12-03T10:41:05.416Z Reads: 265

```
What are trying to connect to the vesc, nrf24 or nyko Kama.<img src="/uploads/db1493/original/2X/a/ad55baa7eda3e832d2497067f4edc6b5acb7772e.png" width="281" height="499">

NRF24.      VESC
PIN8 IRQ      -> not connected
PIN7 MISO   -> PIN7 SCL_RX_MISO
PIN6 MOSI   -> PIN6 SCL_RX_MOSI
PIN4 CSN     -> PIN5 SDA_TX 
PIN5 SCK     -> PIN4 SCK_ADC_EXT
PIN1 GND    -> PIN3 GND
PIN3 CE       -> PIN2 VCC (3v)
PIN2 VCC    -> PIN2 VCC (3v)
         NONE -> PIN1 5v
```

---
## \#72 Posted by: Braylon31 Posted at: 2015-12-03T17:10:38.690Z Reads: 244

```
Im using just the nunchuck... so vcc is 3.3v i need for power and the triangle is ground?  and i dont use pins 7.. 4... 1 correct?
```

---
## \#73 Posted by: Blasto Posted at: 2015-12-03T18:19:39.936Z Reads: 246

```
I've tried figuring this out for myself but have been unsuccessful so far, how can one turn the regen/brake feature off?

I am communicating by PPM and i wish to have this behavior: Reverse, Coast, Foward.
```

---
## \#74 Posted by: onloop Posted at: 2015-12-03T20:56:43.021Z Reads: 255

```
[quote="Blasto, post:73, topic:17"]
how can one turn the regen/brake feature off?
[/quote]

http://www.electric-skateboard.builders/t/vesc-faq-regen-braking-configuration-bldc-tool-brake-force/353
```

---
## \#75 Posted by: jacobbloy Posted at: 2015-12-09T15:07:05.117Z Reads: 247

```
just so every one knows FOC is know available for the VESC, with FW2.3.
Windows and OS X versions have been updated to 2.3 also.
```

---
## \#76 Posted by: chaka Posted at: 2015-12-09T22:45:48.704Z Reads: 259

```
Be sure to update your VESC before updating the BLDC-Tool. Seems to be having some issues the other way around.
```

---
## \#77 Posted by: tomtnt Posted at: 2015-12-10T23:16:49.337Z Reads: 266

```
looks like vedder just released 2.4 to fix FOC bugs
```

---
## \#78 Posted by: chaka Posted at: 2015-12-11T00:55:28.007Z Reads: 289

```
A little update for everyone. We have Vedder's spark switch set for production and will be offering it as a pre-wired package in combination with the VESC. It will come with a high quality sealed  push button switch and auxiliary xt-60 charge port. As always the actual configuration is completely customizable by request.
<img src='/uploads/db1493/original/2X/5/5fdc1040dcea36709b28a40a424e806da05dc5f8.jpg'>
```

---
## \#79 Posted by: NNGG Posted at: 2015-12-11T04:32:40.362Z Reads: 278

```
When can I buy this?
```

---
## \#80 Posted by: chaka Posted at: 2015-12-11T14:32:26.440Z Reads: 289

```
I will have the first batch completed in a week, waiting on the pcb's. If you already have an order for a vesc I can send an invoice for the upgrade.
```

---
## \#81 Posted by: elkick Posted at: 2015-12-17T11:38:48.346Z Reads: 297

```
@jacobbloy, thanks again for your continuously updating. 

It seems, that the mc_config_&_FW.zip is currently missing 2.4, also the OSX_BLDC_Tool_FW 2.3 FOC contains actually the BLDC-Tool V2.4....
```

---
## \#83 Posted by: jacobbloy Posted at: 2015-12-17T21:42:19.618Z Reads: 274

```
I basically scraped 2.3 as Vedder did some big bug fixes that he recommends every one to use, also you can get the fw file from git hub if your desperate I just haven't had time to get every thing sorted.
```

---
## \#84 Posted by: elkick Posted at: 2015-12-17T22:39:37.832Z Reads: 269

```
No problem and I'm not desperate since I'm using Ubuntu and github anyway. 

I was just asked by others not present here due to language constraints who are using the google drive solutions. But that's ok.
```

---
## \#85 Posted by: Sharkface Posted at: 2015-12-18T00:10:42.302Z Reads: 261

```
The moment i get my servers back im just gonna setup a build cluster. I can even get access to some certs to sign the code so windows dont freak out about the app ever
```

---
## \#86 Posted by: lowGuido Posted at: 2016-01-24T05:59:13.471Z Reads: 244

```
just looking at that photo @chaka, I quite like the look and slim form of the VESC without any headers on it.
got me thinking half the headers on there are not gonna get used, I might as well take them off.

like what are they all for anyway? 
the one on the baseline is for hall sensors right? well I'm never gonna use that.
then there is the can bus, well i might link 2 together.. but only need 2 of the pins so I could just solder 2 wires.
when my new Kama's arrive i'll use the 7 pin header to connect the dongle, but again only 4 of the 7 pins used..
If im using the kama then theres no need for the PWM pins.. 
whats the other one for? flashing? I can do that with the USB. so probably don't need that one either.

now that I think about it i'd rather have no headers and just solder to the pads that I do need.
```

---
## \#87 Posted by: chaka Posted at: 2016-01-24T15:36:28.780Z Reads: 242

```
You are correct! If you have a hot air station you can pull them off fairly easily I also stock right angle jst connectors  to port them out the sides. keeps the whole assembly about as thick as the fets.
```

---
## \#88 Posted by: onloop Posted at: 2016-02-04T10:09:35.082Z Reads: 266

```
**NEW VESC BATCH HAS ARRIVED!..** 

Original estimated shipping date of 17th FEB is now invalid, everyone gets VESC much sooner, shipping starts tomorrow! 

**It's great to be ahead of schedule! We have plenty of stock for sale & immediate shipping! But It won't last!**

https://www.instagram.com/p/BBW-3meAW3I/?taken-by=enertionboards
https://www.instagram.com/p/BBXCrP1AW6-/?taken-by=enertionboards

Some notes about this batch.
 - Comes with 5.5mm Connectors, Great for R-SPEC motors.
 - Wires have Silicone Insulation Rated for 200c
 - Firmware Pre-Loaded
 - R-SPEC motor parameters pre-configured.
 - Motor spin testing on all VESC before shipping.
```

---
## \#89 Posted by: chaka Posted at: 2016-02-08T17:46:45.819Z Reads: 259

```

I wanted to announce how we are handling the latest hardware update to version 4.12. Vedder recently added another capacitor above C18 to address a fault occurring in FOC mode, in effect doubling the capacitance at C18

Every VESC leaving our shop now comes with a C18 modification on v4.11 hardware. We opted to use a higher rated capacitor instead of stacking two 2.2uf caps. I was worried the stacked caps could end up tearing the pads on the pcb due to the added leverage and the small footprint. We also have version 4.12 PCB's in fab so those will be available soon but are essentially the same as 4.11 with a higher rated cap at C18.
<img src="/uploads/db1493/original/2X/8/805964f85e4398c00ab412e39ffebf7362727c79.png" width="296" height="500">
```

---
## \#90 Posted by: onloop Posted at: 2016-03-14T10:36:28.617Z Reads: 235

```

Beginners intro to VESC.
https://www.youtube.com/watch?v=tOzTdqe6TVc
```

---
## \#91 Posted by: chaka Posted at: 2016-03-18T18:03:29.081Z Reads: 243

```
Dual heat sinked VESC's mounted on a single aluminum base with vertical usb ports for ease of access.  It is the most compact dual VESC available measuring under 80mm wide.

<img src="/uploads/db1493/original/2X/1/15dd01a513b76cff42bff695eefa87a18984ce32.jpg" width="667" height="500">

I also made some custom mounting plates for a Losi 6IX. Lots of possibilities when it comes to the VESC.

<img src="/uploads/db1493/original/2X/c/cb6f82ca871b046518ada90cc7475de62d937589.jpg" width="690" height="440">
```

---
## \#92 Posted by: torqueboards Posted at: 2016-03-18T19:09:52.988Z Reads: 240

```
Getting closer to a completed batch. PCB's done and assembly should be completed within the week.

<img src="/uploads/db1493/original/2X/2/228dfd99cadbffd5548e002aaa7c924f4058ae76.png" width="690" height="417">
```

---
## \#93 Posted by: Kaly Posted at: 2016-03-18T23:27:18.559Z Reads: 237

```


Hello Dexter 
Nice to see your VESC coming along :sunny:

Do you have the VESC parameters for your sensored Motor 6355 230KV 2650W ?
```

---
## \#94 Posted by: torqueboards Posted at: 2016-03-19T02:41:56.085Z Reads: 243

```
@Kaly - I don't. Not yet.

Yeah, they look great. Excited to get them.
```

---
## \#95 Posted by: onloop Posted at: 2016-03-30T08:26:31.845Z Reads: 241

```
FINAL PRODUCTION SAMPLE FROM NEW USA SUPPLIER

photo for peer review
<img src="/uploads/db1493/original/2X/e/e337040863f2a018a57cb2b0bb53fae45f5bfdaf.jpg" width="649" height="50
```

---
## \#96 Posted by: onloop Posted at: 2016-03-30T22:09:46.727Z Reads: 236

```
Here are my final thoughts about production.

No 5.5mm bullet connectors. Prob just some motors wires..
Only install header plugs for CAN & Sensor Ports.
Caps & Power wires with xt60 will be installed.
Can't find a compatible vertical USB receptacle, so it's just the standard USB receptacle from BOM (unless someone can tell me the part #)
```

---
## \#97 Posted by: cmatson Posted at: 2016-03-31T03:14:37.895Z Reads: 234

```
[quote="onloop, post:96, topic:17"]
No 5.5mm bullet connectors. Prob just some motors wires..
[/quote]

I'd put the bullets just for the plug-and-play lovers.. having the Space Cell, VESC, and R-SPEC combo require no soldering would be a huge plus. 

Also if the 2.4ghz remote came with a servo cable to attach it to the VESC, people wouldn't need anything extra at all.
```

---
## \#98 Posted by: onloop Posted at: 2016-03-31T03:19:30.723Z Reads: 242

```
No Soldering would be great, but the bullets mounted direct to PCB seem to be an issue for some people. It's not really design for that so one knock & it can damage the PCB. In the long run the VESC needs to be completely modified so that it has better motor connections. 

I suppose I could put the 5.5mm connectors on 1inch of wire, then it will eliminate the stress problems.

Yeah the 2.4ghz remote was meant to have the servo cable... never came with it... Nothing in this world is easy!
```

---
## \#99 Posted by: Michaelinvegas Posted at: 2016-03-31T07:47:04.092Z Reads: 242

```
Servo cable to control the bomb bay doors on your down hill bomber lol
```

---
## \#100 Posted by: malik Posted at: 2016-04-08T13:52:28.608Z Reads: 239

```
Hello, 
i ordered a vesc for the 31st of March batch. i still have no information about shpping. 
Thank you
```

---
## \#101 Posted by: claudiofiore88 Posted at: 2016-04-09T22:29:00.412Z Reads: 260

```
@malik 

http://www.electric-skateboard.builders/t/enertion-vesc-delay/2158
```

---
## \#102 Posted by: harpie Posted at: 2016-04-27T11:26:34.424Z Reads: 236

```
I am a electronic engineer from South Africa keen to get my hands on a vesc for some experimentation. Think torture testing with some oscilloscopes, smoke, ect... Instead of buying a ready made vesc I will be buying bulk components and boards for a run of 10 to bring the cost down. I would like to sell around 8 of them (working of course) to make up the cost. I estimate around 150$ each. Would there be interrest or should I stick to a run of 2 for myself only?
```

---
## \#103 Posted by: onloop Posted at: 2016-04-27T14:08:11.328Z Reads: 248

```

hey harpie, welcome to the fourm, unfortunately, there is a new rule that you have to be level 2 before you can talk about arranging group buys or selling items...

So please hang around for a some more time & reply to posts & integrate into the community, you will reach level 2 soon.

http://www.electric-skateboard.builders/t/new-rule-group-buy-for-sale-topics-level-2-user-only/2601/8
```

---
## \#104 Posted by: chaka Posted at: 2016-05-03T14:22:42.173Z Reads: 243

```
I have been wanting to share this project for a long time. They unveiled the ROV and finished qualifying last week.  If you look close you can see the motor controller placement in the rendering, they might look familiar. 
https://www.youtube.com/watch?v=r9y_yW9snug


<img src='/uploads/db1493/original/2X/2/275a486f9ff09ca4b68f0d89b38b399e01111478.jpg'>
```

---
## \#105 Posted by: joaoalmeida Posted at: 2016-05-03T19:26:27.763Z Reads: 217

```
Does a turnigy aerodrive sk3 430kv motor brushless outrunner motor work on the mono  drive kit and for the board? Please help
```

---
## \#106 Posted by: claudiofiore88 Posted at: 2016-05-03T19:28:57.203Z Reads: 214

```
No, the kv is way too high.  You want to get the largest motor possible like an sk3 192kv 6374.
```

---
## \#107 Posted by: joaoalmeida Posted at: 2016-05-03T19:32:57.186Z Reads: 209

```
Thank you, and whats the best esc for the sk3 192kv 6374 motor?
```

---
## \#108 Posted by: claudiofiore88 Posted at: 2016-05-03T19:40:26.293Z Reads: 213

```
You have a couple choices for the "BEST" esc.  You can get the VESC which are hard to come by at the moment (@torqueboards @chaka @onloop sell them).  You can also get the 12s Torqueboards ESC from @torqueboards again.
```

---
## \#109 Posted by: joaoalmeida Posted at: 2016-05-03T19:45:48.308Z Reads: 210

```
Which is the best and most powerfull motor "sk3 6374-192 kv brushless" or "sk3 5055-280 kv brushless"?
```

---
## \#110 Posted by: Blasto Posted at: 2016-05-03T19:47:19.239Z Reads: 205

```
They misted a great opportunity to have a hot girl mess around with their water drone.
```

---
## \#111 Posted by: claudiofiore88 Posted at: 2016-05-03T19:48:34.811Z Reads: 202

```
The sk3 192kv 6374 because it's a way bigger motor.  6374 means that the motor is 63mm in diameter and has a 74mm long can, and 5055 means that motor is 50mm in diameter and a 55mm long can.
```

---
## \#112 Posted by: joaoalmeida Posted at: 2016-05-03T19:56:52.958Z Reads: 201

```
Alright thank you very much
```

---
## \#113 Posted by: joaoalmeida Posted at: 2016-05-03T20:08:25.808Z Reads: 204

```
Is the 120 A esc the same as a 12s esc?
```

---
## \#114 Posted by: claudiofiore88 Posted at: 2016-05-03T20:32:14.925Z Reads: 205

```
No, that esc can handle up to a 6s Lipo, while the other can handle up to a 12s Lipo.
```

---
## \#115 Posted by: joaoalmeida Posted at: 2016-05-03T21:07:54.644Z Reads: 202

```
Does the space cell pro enclosure come with a charger?
```

---
## \#116 Posted by: claudiofiore88 Posted at: 2016-05-03T21:24:00.660Z Reads: 208

```
The spacecell from enertion comes with the charger as far as I know. @onloop would be able to confirm.
```

---
## \#117 Posted by: joaoalmeida Posted at: 2016-05-04T13:01:16.964Z Reads: 210

```
Does a sk3 6364 mm motor  fit in the mono drive kit?
```

---
## \#118 Posted by: chaka Posted at: 2016-06-15T21:01:44.339Z Reads: 210

```
Big thanks to @JTAG for the suggestion. Our VESC's now come with a larger capacitor on C37, definitely makes for a more robust build. We have been implementing this change for the past few weeks so some of you already have this upgrade on your VESC. ;)

<img src="/uploads/db1493/original/2X/6/6e4b77b0eba0a4d358fdcb3ced67203cc263c997.jpg" width="666" height="500">
```

---
## \#119 Posted by: Qwiksand Posted at: 2016-06-15T21:56:07.870Z Reads: 205

```
@chaka I love how quickly you guys can turn these hardware updates into reality. Top notch!
```

---
## \#120 Posted by: Pablo_702 Posted at: 2016-06-15T22:25:14.446Z Reads: 205

```
Can i use a solid state switch instead that way would be no spark anywhere
```

---
## \#121 Posted by: chaka Posted at: 2016-06-15T22:33:09.453Z Reads: 207

```
This upgrade has nothing to do with anti-spark. 

Vedder has designed an in-rush controller that works very well if you want to use a switch rather than unplugging your battery to power on and off. 

[SparkSwitch BOM](https://github.com/vedderb/SparkSwitch/blob/master/SparkSwitch_BOM.ods)

[Upgraded Gerber Files - OshPark](https://oshpark.com/shared_projects/XuqJkZzU)
```

---
## \#122 Posted by: flatsp0t Posted at: 2016-06-15T22:35:06.863Z Reads: 197

```
yes, the vedder antispark is just a solid state switch.
see the esk8.de shop, they have it.
```

---
## \#123 Posted by: Bender Posted at: 2016-06-16T01:05:21.704Z Reads: 203

```
Do you know the difference between vedder's and torqueboar's
```

---
## \#124 Posted by: delta_19 Posted at: 2016-06-16T02:15:15.593Z Reads: 215

```
both are solid state, just different pcb layouts.
```

---
## \#125 Posted by: chaka Posted at: 2016-06-17T15:34:09.355Z Reads: 222

```
Give it up for Vedder! Looks like it wont be long till v5 is released. Lets hope everything goes smoothly and don't forget to send him some support, he has been hard at work!

<img src="/uploads/db1493/original/2X/b/bc47bc62d7041bf4950b6129d23a4d66332af76e.jpg" width="560" height="500">
```

---
## \#126 Posted by: Jinra Posted at: 2016-06-17T15:40:33.047Z Reads: 212

```
That's quite some real estate! Does the v5 eliminate the drv8302 altogether?
```

---
## \#127 Posted by: chaka Posted at: 2016-06-17T16:05:38.540Z Reads: 208

```
On the flip side you will see the drv8301 footprint.
```

---
## \#128 Posted by: Kaly Posted at: 2016-06-17T16:55:20.184Z Reads: 214

```
Here we go !!
Mr. vedder guy is a MONSTER :thumbsup: :thumbsup: :slight_smile: :slight_smile: 
We all need to chip in on this :money_with_wings: :money_with_wings:
```

---
## \#129 Posted by: Ulfberht Posted at: 2016-06-17T19:12:28.696Z Reads: 214

```
So the one on the left is the current style and the one on the right the V5? That is a huge size difference! Also, the VESC on the right has VESC 6.0 on it. Is that V6? :grinning:
```

---
## \#130 Posted by: Jinra Posted at: 2016-06-17T19:17:34.825Z Reads: 217

```
It's so good, we're skipping v5!
```

---
## \#131 Posted by: Qwiksand Posted at: 2016-06-17T20:40:31.457Z Reads: 226

```
@chaka how quick do you plan to tool up for production once vedder releases/shows a fucntioning prototype? Significant cost difference as far as you can tell at this point?
```

---
## \#132 Posted by: chaka Posted at: 2016-06-17T22:22:08.870Z Reads: 234

```
@Ulfberht @Jinra v5 was populated on two separate pcb's but vedder opted for a single pcb so v6 was born.

@Qwiksand  Vedder likely won't release the gerbers until it he knows it is fairly stable but once he does we should have some ready for beta testers within 2 weeks. They will be a little more expensive due to the milling services needed to produce the aluminum enclosure but they will also be a better match for larger motors.
```

---
## \#133 Posted by: Ulfberht Posted at: 2016-06-17T23:39:52.343Z Reads: 228

```
@chaka
  So can i just start a tab? :wink::beer: Seriously, I'll just give you my credit card # and call it a day! :grinning:
```

---
## \#134 Posted by: quinnyt2015 Posted at: 2016-07-25T09:16:20.665Z Reads: 217

```
Whats the status of the VESC settings for these motors? :) Edit: The sensored 6355 230KV 2650W ones
```

---
## \#135 Posted by: torqueboards Posted at: 2016-07-25T16:36:22.413Z Reads: 221

```
@quinnyt2015 What do you mean? I'd just run the motor detection, apply on your bldc tool.
```

---
## \#136 Posted by: Ultimat3ging3r Posted at: 2016-09-23T01:05:54.365Z Reads: 171

```
Where did you find that diagram? I have the same one you have and I'm a bit wire tarded.
```

---
## \#137 Posted by: disastorm Posted at: 2016-09-24T02:20:05.735Z Reads: 174

```
> Where did you find that diagram? I have the same one you have and I'm a bit wire tarded.

unfortunately, it actually ended up not working after i tried it.
```

---
## \#138 Posted by: Redfire1 Posted at: 2018-04-14T05:43:19.919Z Reads: 61

```
@onloop morning I am desperately trying but can’t rap my head around it I am using a 5056 racestar motor with a 5 pin sensor to connect to 6 pin vesc,in my pic I think the Orange wire is the temp that’s the one they said I should leave so I am going to connect the black to black,red to red,white to white,yellow to yellow and finial blue to green.does that sound right ![image|409x499](upload://GkgNv8bqT20btmDJhONhI7lk6R.jpeg)![image|679x500](upload://xNEWmDFUhUPqgQ8BG5Tptwt9UgN.jpeg)
```

---
