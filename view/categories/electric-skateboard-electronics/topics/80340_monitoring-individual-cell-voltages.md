# Monitoring individual cell voltages

### Replies: 123 Views: 4257

## \#1 Posted by: janpom Posted at: 2019-01-08T23:14:39.477Z Reads: 390

```
I believe there's value in knowing the voltages of individual cells (or P packs) in a battery pack. If nothing else, knowing that your cells are well balanced and don't tend to drift away will give you a piece of mind.

I've been looking into what options there are. This is a write up of my findings. I hope this is useful info for some. I also hope for people to chime in and help to complete the list.

Possible solutions can be divided into two main groups -- measuring inside the enclosure and outside the enclosure.

## 1. Inside the enclosure
The cell voltages are measured by a device sitting inside the battery enclosure. The information is either wirelessly transmitted to a mobile phone or is viewed on a display that is a part of the enclosure.

### 1.1. [DieBieMS](https://www.electric-skateboard.builders/t/diy-6s-to-12s-bms-with-can-diebiems/2639) + [Metr Pro](https://www.electric-skateboard.builders/t/metr-pro-next-gen-bluetooth-module/57780)

These probably don't need any introduction. Great products made by community members. DieBieMS is a smart BMS that supports various communication interfaces. It integrates with the Metr Pro module, which can route the DieBieMS data to your mobile phone. Both Android and iPhone are supported.

https://media.giphy.com/media/3OC2r75I9xp9M2hdxa/giphy.gif

Pros
- tech support (products of active community members)
- Android, iPhone
- DieBieMS can be used as charge/discharge
- DieBieMS provides an e-switch

Cons
- fairly expensive
- DieBieMS is a big BMS
- DieBieMS is currently not easily available

### 1.2. [LLT Power Smart BMS](https://www.lithiumbatterypcb.com/product/13s-48v-li-ion-battery-pcb-board-54-6v-lithium-bms-with-60a-discharge-current-for-electric-motorcycle-and-e-scooter-protection-2-2-3-2-2-2-2-2/) + bluetooth module
Relatively cheap Chinese Smart BMS that supports UART communication and comes with a bluetooth module. An [Android app](https://www.lithiumbatterypcb.com/smart-bms-software-download/) that can display cell voltages as well as other useful information is available. It's a very basic app. The UI is by far not as polished as the Metr Pro, but it does provide all the info anyone may care about. There's also a number of configuration options.

https://www.lithiumbatterypcb.com/wp-content/uploads/2017/12/APP.jpg

There are three versions -- for 20A, 30A, and 60A discharge current. Probably not enough for e-skate application. It only makes sense to get the 20A as charge only.

The BMS is available for 10-15S. It's all the same hardware, which comes pre-configured for a certain number of cells. It can be relatively easily re-configured (I have done it) for a different number of cells. It requires a PC module, which costs additional ~$7 and the software only runs on Windows. The software configuration is straightforward. The hardware configuration is a trivial soldering task.

Pros
- cheap
- many features
- reasonably small
- supports 10-15S

Cons
- ~~Android only~~
  - Update: There's a 3rd party [iPhone app](https://itunes.apple.com/us/app/xiaoxiang-bms/id1375405426?mt=8) for $1. Thanks @lrdesigns for pointing this out.
- limited documentation / tech support

### 1.3. LLT Power Smart BMS + DIY

The smart BMS comes with a UART port and the communication protocol is [somewhat documented](https://www.lithiumbatterypcb.com/Protocol%20BMS%20EN.zip) (though deciphering the documentation is only marginally easier than reverse engineering the protocol :sweat_smile:). I managed to get it working with an Arduino, or more specifically, with my [DAVEga hardware](https://www.electric-skateboard.builders/t/davega-battery-monitor-odometer-speedometer/71509), which is essentially a simple Arduino with a display. 

![DSC01798|372x500](upload://yeA7ayiazn0dzozgDUrieVsdsCC.jpeg) 

It wouldn't be a problem to use an Arduino board (Nano or Mini) with a smaller display, such as the 128x32 OLED, which is small enough to be attached to a side of a battery enclosure (if someone designed a panel mount for it).

![IMG_1605%20(1)|690x213](upload://aVTCRvUgdSeqBqrKn9gqJHaynfS.jpeg) 

Also, the Smart BMS could be hooked up with a WiFi/Blueetooth enabled development board (ESP32 and ESP8266 dev boards are cheap and widely available) along with a simple mobile app in [Blynk](https://www.blynk.cc/). If you don't know Blynk, do check it out. It's awesome!

With ESP32 board and Blynk, an iPhone app for cell voltage monitoring would be easily available. I believe it can be done in less than one day.

We could also try to convince @rpasichnyk to integrate the LLT Power BMS with the Metr Pro, which doesn't seem that hard to do now that the DieBieMS integration exists. I can even provide some code snippets. What do you say, Roman? 

### 1.4. DIY cell voltage monitoring module

It would be really nice to have a module that only does one simple task -- read individual cell voltages and communicate the values over UART or I2C. This would likely be a tiny module, much smaller than any BMS. Similarly as the Smart BMS, it could be hooked up with DAVEga or with Arduino + OLED display or with ESP32 + Blynk. It could be an addition to a "dumb" BMS. The ones with li-ion packs who like to live dangerously could even skip the BMS completely. Some say that the li-ion batteries don't require balancing, though keeping an eye on cell voltages is recommended.

The question is what would be the best way to create such module. One option I discussed with @deucesdown in another thread is using a simple voltage divider along with ADC module with sufficient resolution/accuracy (possibly the ASD1115). Doing some experiments with this is on my TODO list.

https://i0.wp.com/henrysbench.capnfatz.com/wp-content/uploads/2015/09/Arduino-ADS1115-Module-Pin-Outs-Type-1.png?w=411

Another option that @deucesdown suggested is using a BMS chip without the BMS components not needed for voltage monitoring, which would likely result in a much smaller device than a traditional BMS. It doesn't seem trivial though.

### 1.5 Neptune Lite

[Neptune Lite ](https://www.speedict.com/product-page/neptune-lite) is a BT enabled cell voltage monitoring module with a very small footprint (41x35x7mm). It comes with a very cool looking Android app with a ton of features. Unfortunately no iOS (yet?).

### 1.6 Other smart BMSes

I don't know these, so I'll just put the links here (thanks @deucesdown).

- [Neptune 15](https://www.speedict.com/product-page/neptune-15)
- [Tiny BMS s516](https://www.energusps.com/shop/product/tiny-bms-s516-150a-750a-36)
- [IC GOGOGO 12-24S Smart BMS](https://www.aliexpress.com/item/Smart-Display-300A-8-24S-Cells-Lithium-Battery-Protection-Board-Balance-BMS-Coulomb-Meter-Lithium-iron/32827394534.html?tt=Copy+to+Clipboard&aff_platform=default&cpt=1547035003738&sk=bNQKo0G0&aff_trace_key=88a5bc79d31e4b19bfb10aba6522decb-1547035003738-04815-bNQKo0G0&terminal_id=290ac6e897e348138b9bb80b0d67ebf4)

## 2. Outside the enclosure

Routing balance wires outside of the enclosure opens many possibilities, such as using a balance charger or check cell voltages manually with a multimeter. It's a lot of wires to be routed. Let's first have look at how it can be done.

### 2.1. Wire routing

Many people use 12S batteries and that means routing at least 13 wires outside of the enclosure if you want to  measure individual cells or balance charge. The [SP21 IP68 connectors](http://www.weipuconnector.com/Product_show_25.htm) have up to 12 pins. I personally use one and I have seen @SkaterBoy58 [use one](https://www.electric-skateboard.builders/t/external-bms-and-charging-box/79444). The 12 pin version is rated 5A. 

![DSC01773|690x460](upload://ddRYzJSg4YBwCqWW8EDhWyghlNB.jpeg) 

This works for 10S (or 11S), but is one pin short for 12S. I found [these connectors](https://www.aliexpress.com/item/SD28-waterproof-connector-3-5-7-9-10-12-14-16-19-24-26Pin-IP67-Small/32919319661.html) on AliExpress, which also come with 14 pins, but those are already bit too bulky. Here's another [14 pin connector](https://www.ebay.com/itm/1Pc-Military-14-Pin-Twist-Male-Female-Connector-Plug/151106903634) (thanks @deucesdown); I haven't been able to find the dimensions for it.

Edit: The SP21 is also available with the [panel mount on the female part](https://fr.aliexpress.com/item/SP21-12pin-Ouverture-de-Sortie-Fiche-de-L-aviation-tanche-Montage-Sur-Panneau-prise-de-courant/32920827543.html), which is a better option since it reduces the risk of shorting out in case the connector gets damaged. (Also makes it harder for kids to create a dead short when they decide that it would be a good idea to stick some metal objects into the connector. :smiley:) 

@oriol360 pioneered the idea of using a [VGA port](https://www.electric-skateboard.builders/t/miami-electric-boards-diy-charger-how-to/4242) (15 pins) for balance charging. This has since been used by other people as well. 

@billappleton simply used [JST connectors and a cable cover](https://www.electric-skateboard.builders/t/hellboy-eboosted-enclosure-sector-9-meridian-board-focbox-unity-evolve-supercarve-trucks-psychotiller-6369-motors-unikboard-motor-mounts-pelican-bay-12s4p-battery-abec-107mm-wheels-hoyt-puck-remote/77933/30?u=janpom) on his Hellboy.

[Here's](https://youtu.be/O5gi35AtPSw?t=287) another use of JST connectors. Probably not exactly waterproof though.

### 2.2. Balance chargers

The easiest way to monitor individual cell voltages while charging is to use a balance charger. The problem is that balance chargers for 10S or even 12S are rare and expensive. They do exist though.

- [Chargery C4012B](http://www.chargery.com/C4012B.asp) is a monster 12S 1500W charger that you can feed directly from an AC supply. It costs astounding $350. I believe that @billappleton has one, so you can ask him if it's worth the money.
- [iCharger 1010B+](https://www.icharger.co.nz/icharger-1010b) is a 10S 300W charger for more reasonable $139. You need an additional DC power supply though.

https://www.icharger.co.nz/assets/full/I1010B.jpg

-  [EVPEAK A9](https://www.amazon.com/EVPEAK-1350W-Charger-Battery-Screen/dp/B01D4PORJW)  is a 12S 1350W charger and it costs around $200. It also requires a DC power supply (11-32V).

It's also possible to use two 6S balance chargers, which are widely available. It's critical to feed them from two isolated DC power supplies though, otherwise you'll short your battery over the common ground and you don't want to do that. Charging 12S with two 6S balance chargers is shown in the [same video I linked above](https://youtu.be/O5gi35AtPSw?t=267). The iMax B6AC chargers come with an integrated DC power supply and thus are safe for the purpose. You could just use any other chargers, though, as long as you feed them from two different DC supplies.

### 2.3. "Frankenstein" charger

@Luuke has built [this charger](https://www.electric-skateboard.builders/t/first-build-mono-6374-vesc-10s3p-bms-90mm-flywheel/37257/14?u=janpom), which is awesome. It's basically 10 independent single cell chargers.

### 2.4. External BMS

The BMS doesn't need to be inside the enclosure to be used for charging. @SkaterBoy58 is building [this impressive charger](https://www.electric-skateboard.builders/t/external-bms-and-charging-box/79444) using DieBieMS.

I'm working on [something similar](https://www.electric-skateboard.builders/t/cheap-diy-12s-balance-charger-idea/76695/64?u=janpom) with the LLT Power Smart BMS.

### 2.5. No balancing

Jehu Garcia claims in [this video](https://www.youtube.com/watch?v=tbaeMWdDlqY) that the li-ion batteries actually don't need to be balance charged. He specifically mentions that he doesn't use a BMS for his electric Volkswagen bus. And that's one hell of a battery.

He also mentions that checking individual cell voltages is worthwhile. It can simply be done with a multimeter if you have access to the balance wires. There's also a variety of cheap cell voltage checkers, such as [this one from HobbyKing](https://hobbyking.com/cz_cz/hobbykingtm-lipo-voltage-checker-2s-8s.html). One that I want to specifically mention is the [Chargery BS12](http://www.chargery.com/cellSaver12S.asp) since (1) it supports up to 12S, which is rare, and (2) it has a charge alarm that's triggered if any cell voltage exceeds 4.22V. This seems like a very handy thing to have when using a brick li-ion charger with no BMS since you get notified you should disconnect the charger.
```

---
## \#2 Posted by: deucesdown Posted at: 2019-01-08T23:19:54.383Z Reads: 285

```
didn't read yet, but I want to leave this here

https://www.instructables.com/id/1S-6S-Battery-Voltage-Monitor-ROS/

It's 6s, and he mentions using a 1:8 multiplexer IC to get up to18s (but no details). It's a voltage divider, so may have the passive drain issues you mentioned.

And generally, with respect to typical BMS functions, I believe I want to monitor cell voltages. I can balance as needed by whatever means -- I don't need to continuously balance. And I really don't like blindly trusting a no-feedback continuous balance system.
```

---
## \#3 Posted by: billappleton Posted at: 2019-01-08T23:29:25.092Z Reads: 266

```
Great post. I am a programmer and that influenced my decisions about charging. I wanted the charge system to be visible and the various components to be separate. The Chargery is expensive but very fast with nice display of information. It slows down as it approaches the target voltage, etc. I plan to use it for other boards too. I was really surprised at how hard it was to find a 12s charger! Seems like such a no brainer.
```

---
## \#4 Posted by: deucesdown Posted at: 2019-01-08T23:35:02.155Z Reads: 257

```
Jehu's pattern is:
- don't charge to full (saves cycle life, and don't need to be precise about termination)
- bottom balance occasionally (only if needed)  -- when pack is near 0%, cells should be in balance and not over discharged
- don't stress the cells out with close to max discharge (which tends to unbalance cells)
- for normal charge, don't balance charge. Just bulk charge to something like 90%.

Even if we don't do as he does, it's useful to think about it.
```

---
## \#5 Posted by: janpom Posted at: 2019-01-08T23:52:26.809Z Reads: 235

```
It's the same simple design as I have, so yes, it will have the same passive drain issues. I wonder if the multiplexer would really work though. I looked at the datasheet and didn't understand it (that's what usually happens to me with datasheets :slight_smile: ). I'll try again after I have slept on it.
```

---
## \#6 Posted by: monsterbuilder Posted at: 2019-01-09T02:57:43.961Z Reads: 227

```
Solid post.  Thanks for sharing all of your research with this community.
```

---
## \#7 Posted by: lrdesigns Posted at: 2019-01-09T03:23:22.361Z Reads: 233

```
I would really like to try 1.3 if you ever release the firmware. 

![image|690x376](upload://xC8e5xTP7zVdxinqyASRVBPQQxA.jpeg) 

I was planning on getting one of these smart bms anyway. but being able to check cell voltages without opening an app on my phone would be really nice. 

Also its not android only, there is an iphone app. Not sure the app name now though, a user on here told me about it a while ago. Might be "Xiaoxiang BMS" its $1usd.
```

---
## \#8 Posted by: deucesdown Posted at: 2019-01-09T03:54:15.116Z Reads: 224

```
Thanks @janpom great post. I've wasted an enormous amount of time with google on this topic.

[quote="janpom, post:1, topic:80340"]
There are three versions – for 20A, 30A, and 60A discharge current
[/quote]

I believe these guys are the OEM

https://www.lithiumbatterypcb.com/product-instructionev-battery-pcb-boardev-battery-pcb-board/ev-battery-pcb-board/smart-bms-of-power-battery/

The 60a version comes with aluminum top and bottom plate. The 20a/30a only have fets on top, and only has aluminum top plate. Bottom is fish paper. I like the physical protection of the 60a, and it's not that much more money.

They have a bigger version that can do more discharge, up to 100a. Oh and I see a bunch of new looking stuff with RS385, RS232, Can, SMbus. CAN would mean possible METR compatibility via vesc, like dbms?

There's also this 

https://www.speedict.com/product-page/neptune-15

Expensive (used to be cheaper) and the ES thread showed some concern for accuracy.

And this

https://www.energusps.com/shop/product/tiny-bms-s516-150a-750a-36

Also expensive, fairly well proven I think.

Connectors, @oriol360 showed us using a VGA port (15 pins) for balance and charge leads -- fine if you're doing low current.

I've also got m hands on a few of these types of thing

https://www.ebay.com/itm/1Pc-Military-14-Pin-Twist-Male-Female-Connector-Plug/151106903634

Comes in many sizes and shapes.

Balance charger for 10s/12s not a dual where you have to break the series connection, there's the Chargery ($$$) and

https://www.amazon.com/EVPEAK-1350W-Charger-Battery-Screen/dp/B01D4PORJW

The EVPEAK comes with the 12s breakout board. The company claims they have a 10s board for purchase but won't actually sell you one.

I think you can also use two 6s chargers if you use 2 different PSUs with the dc ground lifted.
```

---
## \#9 Posted by: mynamesmatt Posted at: 2019-01-09T09:36:55.582Z Reads: 195

```
![20190109_174620|666x500](upload://f3p6eCGLGLdCKk5aEXYbifuGZM9.jpeg)
if you zoom in on my board you can see my voltage meters. they're literally HobbyKing voltage testers hooked up to a switch. so i can see individual voltages at a flick of a switch
```

---
## \#10 Posted by: janpom Posted at: 2019-01-09T09:48:14.293Z Reads: 187

```
I like simple solutions like that. Can you turn them off, though?
```

---
## \#11 Posted by: Jumpman Posted at: 2019-01-09T09:49:12.453Z Reads: 183

```
There was also that cell checker that I think @Nowind used.  Can’t remember what the problem was with it.  I think his was called mttec or something similar, but looked like the Chargery BS12.
```

---
## \#12 Posted by: Surfer Posted at: 2019-01-09T09:52:05.118Z Reads: 180

```
This thread just made my day happier, thanks @janpom.

Bookmaked and in the waiting list.
```

---
## \#13 Posted by: mynamesmatt Posted at: 2019-01-09T10:55:21.813Z Reads: 183

```
![Screenshot_20190109-215106_Gallery|243x500](upload://xuJNPZSFZX8LpxLqeyLGhzA1B1k.jpeg)
up is off and down is on. the checker only does the front packs and the other checker does the back packs so i can quickly locate a problem. 
each checker cycles like this:
*switch on* "5Ce (5 cell), Total voltage (eg 21v bc its only measuring 5 cells) c1, (voltage), c2 (voltage), c3, (voltage), c4, (voltage), c5 (voltage)..... and then it repeats. *switches off*
(went over the top but idc)
```

---
## \#14 Posted by: pat.speed Posted at: 2019-01-09T11:11:36.895Z Reads: 170

```
Are you sure it’s actually turning off tho? I’ve had a similar checker and even after disconnecting the gnd pin it would still be on just the screen would dim slightly. In order to turn it off I had to disconnect the first 2-3 pins
```

---
## \#15 Posted by: mynamesmatt Posted at: 2019-01-09T11:12:45.992Z Reads: 166

```
yeah its dead off
```

---
## \#16 Posted by: mynamesmatt Posted at: 2019-01-09T11:13:13.325Z Reads: 166

```
i got the lights completely out to check and nup nothing at all
```

---
## \#17 Posted by: janpom Posted at: 2019-01-09T11:16:43.410Z Reads: 167

```
If the switch only cuts off the ground wire, there's likely still some passive drain even when it's off. It's probably small enough not to be a problem. I'm still curious to know how much it is (if anything at all). I have the same checker at home. I'll do some measuring on it.
```

---
## \#18 Posted by: Chrisjarram Posted at: 2019-01-09T11:30:04.777Z Reads: 162

```
Fantastic post - just getting round to this part of my build so really useful info!! Cheers
```

---
## \#19 Posted by: pat.speed Posted at: 2019-01-09T11:44:17.411Z Reads: 160

```
I just had a look at the bms modules and there doesn’t seem to be a 12s liion on the website, however it can be found on AliExpress for reasonably cheap
```

---
## \#20 Posted by: janpom Posted at: 2019-01-09T11:49:56.413Z Reads: 158

```
The product offer is a bit confusing. The 12S is only available for lifepo4 batteries. I'm not sure why. The BMS can definitely be configured for 12S li-ion.
```

---
## \#21 Posted by: Chrisjarram Posted at: 2019-01-09T11:53:21.834Z Reads: 149

```
Anyone got any experience with one of these?

￡87.26  17%OFF | 300A 8S 12S 24S Cell Lithium Battery Protection Board Smart Display Balance BMS Coulomb Meter lifepo4 Lipo li-ion APP Bluetooth
 https://s.click.aliexpress.com/e/bNQKo0G0

My build is 12s 12ah 50c max discharge - 2 x 6s lipo - dual maytech 6374s sealed with focbox unity - and wondered if this is going to be suitable?  Rated higher than I need but price difference is negligible so may as well over-spec.

Any disadvantages or is this the ideal solution for charging and battery protection in my case?

Extremely grateful for any advice! :)
```

---
## \#22 Posted by: janpom Posted at: 2019-01-09T11:56:38.556Z Reads: 143

```
Thanks @deucesdown for the additional information. Very useful! I added some bits to the original post. Will do more updates later when I have more time.
```

---
## \#23 Posted by: janpom Posted at: 2019-01-09T12:04:29.696Z Reads: 152

```
I'll definitely make the FW available. Note though that this won't be an additional functionality to the DAVEga. It only has a single UART port so you can either hook it up to a VESC or to a Smart BMS, but not both. Also even if I somehow figured it out, there's not enough flash memory for combining the two firmwares.

You could make an enclosure for dual DAVEga though. ;) The next obvious evelution step then is the DAVEga Unity! :smiley:
```

---
## \#24 Posted by: pat.speed Posted at: 2019-01-09T12:05:57.711Z Reads: 154

```
It looks huge and well over powered for our needs but if that doesn’t bother you I guess it’s fine
```

---
## \#25 Posted by: deucesdown Posted at: 2019-01-09T12:16:35.945Z Reads: 157

```
[quote="janpom, post:20, topic:80340"]
The 12S is only available for lifepo4 batteries
[/quote]

The guys at lithiumbatterypcb.com will customize the series count and settings for you, within limits of hardware (up to 15s)
```

---
## \#26 Posted by: Chrisjarram Posted at: 2019-01-09T19:15:44.665Z Reads: 157

```
Found this external 12s bms too in case it's useful to anyone..

￡83.63 | free shipping 300A BMS 2S - 16S LiPo LiFe Battery Management System TFT LCD Display Smart Lithium lifepo4 Li-ion Chargery BMS16
 https://s.click.aliexpress.com/e/bO2LQswk
```

---
## \#27 Posted by: ducktaperules Posted at: 2019-01-09T20:52:01.244Z Reads: 151

```
the post is great. well done @janpom

Personally your 1.3 solution looks great. If only we could hook this up to VESC and get the data through metr same as DieBieMS.

I believe the UNITY has spare serial ports accessible inside via headers, they are there for future modules like the BT module that's included. I believe they were planning on releasing the spec for these modules. 

Hooking charge only smart BMS directly to unity would be ideal :+1:
```

---
## \#28 Posted by: billappleton Posted at: 2019-01-09T21:18:25.814Z Reads: 142

```
external or internal? its 3 x 4 inches in size, supports regenerative breaking.  you could see that display from the deck no problem   :sunglasses:
```

---
## \#29 Posted by: Chrisjarram Posted at: 2019-01-09T21:20:14.436Z Reads: 141

```
External in the sense it has its own housing, but yeah I guess could be mounted internally too...

EDIT: doesn't have a balance function,  oddly - so it's a bust
```

---
## \#30 Posted by: monsterbuilder Posted at: 2019-01-09T21:26:02.481Z Reads: 142

```
Option #1.2 (LLT Power Smart BMS + bluetooth module) looks like the most builder & budget friendly option.  Has anyone else used this BMS with success?  I'm curious to know how many builders are using this product.
```

---
## \#31 Posted by: deucesdown Posted at: 2019-01-11T23:39:23.956Z Reads: 141

```
https://www.analog.com/en/products/ltc6801.html#product-overview

In my feeble mind this one looks pretty simple?

Ah nevermind, the output is just safe/no-safe indicator. But, things learned: there's probably an IC that does what we want, and this guy uses a MUX too. And, the boolean output is on a clock signal, so you can tell if it crashed/froze.

Clicking around on analog.com, found this video, didn't watch yet, but the title is nice

https://www.analog.com/en/education/education-library/videos/5849886030001.html

Oh, and [this](https://www.analog.com/media/en/technical-documentation/data-sheets/LTC6812-1.pdf) (15s, cell voltages, error less than 2.2mV, SPI). And it has balancing? But the diagrams look more complicated. $19 for the chip at [arrow](https://www.arrow.com/en/products/ltc6812ilwe-13zzpbf/analog-devices). Looks tiny!

Oh hey this is looking interesing now. Demo board:

https://www.digikey.com/product-detail/en/linear-technology-analog-devices/LTC6812ILWE-1-3ZZPBF/LTC6812ILWE-1-3ZZPBF-ND/9806657

Aaah there's a demo board but $150-200

https://www.digikey.com/catalog/en/partgroup/ltc6813-1-demonstration-board/75932

Did I mention I'm lazy? :)
```

---
## \#32 Posted by: janpom Posted at: 2019-01-14T18:43:49.292Z Reads: 135

```
The [Chargery BMS16](https://s.click.aliexpress.com/e/bO2LQswk) that @Chrisjarram has linked looks pretty cool for use as an external BMS. Unfortunately, I haven't been able to find any reviews. Does anyone have one?
```

---
## \#33 Posted by: deucesdown Posted at: 2019-01-14T20:05:27.144Z Reads: 132

```
Chargery is considered quality stuff, from reading various threads at ES. but I couldn't find much chatter about the brand!
```

---
## \#34 Posted by: Hummie Posted at: 2019-01-14T20:08:55.449Z Reads: 130

```
I want one!  I guess it has 6s balance plug slots on side. ?  I’ll be looking n likely ordering.  Seems to have more features and bigger price than needed for off board balancing
```

---
## \#35 Posted by: Jumpman Posted at: 2019-01-14T20:28:45.517Z Reads: 126

```
2x 8s, I guess.  Was considering it but was put off at the time by the requirement to use relays for charge and discharge.
```

---
## \#36 Posted by: janpom Posted at: 2019-01-15T04:31:28.633Z Reads: 125

```
Is it just that it uses relays instead of MOSFETs internally or do you need to provide external relays?
```

---
## \#37 Posted by: janpom Posted at: 2019-01-15T04:37:38.302Z Reads: 124

```
Looks like the latter. OK, that's indeed clunky. Better to stick with the LLT Smart BMS and make a nice case, display and beeper alarm for it.
```

---
## \#38 Posted by: Benjamin899 Posted at: 2019-01-15T11:43:40.288Z Reads: 121

```
i am tempted to buy the LLT smart bms, but why is it so much smaller than a bestech BMS. My 80A 10s bestech is almost 2,7cm high. The llt only 1,5cm.
```

---
## \#39 Posted by: janpom Posted at: 2019-01-15T11:53:52.307Z Reads: 129

```
Not my area of expertise, but I suppose it could have to do with the fact the LLT BMS is rated only 60A and that's only if you get the aluminium housing (as @deucesdown pointed out [here](https://www.electric-skateboard.builders/t/monitoring-individual-cell-voltages/80340/8?u=janpom)), which probably dissipates a lot of heat.
```

---
## \#40 Posted by: sk8l8r Posted at: 2019-01-15T12:12:07.245Z Reads: 131

```
I bought one of these , its WAY bigger than expected yet to setup and play with it but seems good value if you have the space

https://www.aliexpress.com/item/Bluetooth-smart-BMS-with-100A-constant-current-suitable-for-10S-36V-11S-12S-13S-48V-14S/32849172235.html

really like the amount of config 

![image|431x500](upload://6twrcdNiOT7SIFpDkzirtZ5jRVE.jpeg)
```

---
## \#41 Posted by: Benjamin899 Posted at: 2019-01-15T12:20:31.727Z Reads: 128

```
are the measurements given on their page wrong?
```

---
## \#42 Posted by: Benjamin899 Posted at: 2019-01-15T12:21:26.602Z Reads: 130

```
they have the smart bms up to 100A
https://www.lithiumbatterypcb.com/product/14s-bluetooth-lithium-e-bike-battery-pcb-board-with-30a-constant-charge-and-discharge-current-2/
```

---
## \#43 Posted by: sk8l8r Posted at: 2019-01-15T12:44:17.667Z Reads: 129

```
I just didn't pay enough attention to sizes :)
```

---
## \#44 Posted by: rojitor Posted at: 2019-01-15T12:48:05.508Z Reads: 128

```
I used that one. Yes, it's huge
```

---
## \#45 Posted by: janpom Posted at: 2019-01-15T12:54:07.019Z Reads: 124

```
There are two types.
- [20A-60A](https://www.lithiumbatterypcb.com/product/13s-48v-li-ion-battery-pcb-board-54-6v-lithium-bms-with-60a-discharge-current-for-electric-motorcycle-and-e-scooter-protection-2-2-3-2-2-2-2-2/); `108*65*10mm` (or `108*65*15mm` including the aluminum housing)
- [60A-100A](https://www.lithiumbatterypcb.com/product/14s-bluetooth-lithium-e-bike-battery-pcb-board-with-30a-constant-charge-and-discharge-current-2/); `138*105*15mm`
```

---
## \#46 Posted by: rojitor Posted at: 2019-01-15T13:44:02.077Z Reads: 123

```
I got the 100 amps version. Worth It yet huge
```

---
## \#47 Posted by: deucesdown Posted at: 2019-01-15T13:50:16.923Z Reads: 120

```
Are you using it for discharge too? No issues?

One thing I found in ES is that some (not all) don't go into the deeper sleep mode with bluetooth attached. If it doesn't sleep, the drain is fairly significant, enough to worry about. So I'm constantly checking my builds that use these BMS.
```

---
## \#48 Posted by: rojitor Posted at: 2019-01-15T14:03:15.124Z Reads: 119

```
I am still at the building stage. Didn't really use It. So...the bt module does not sleep? Damn.
Well i can use the pc and ignore the bt. All i really want is set 4.10 hvc
```

---
## \#49 Posted by: Benjamin899 Posted at: 2019-01-15T14:26:45.620Z Reads: 121

```
yes, exactly that
```

---
## \#50 Posted by: rojitor Posted at: 2019-01-15T15:59:02.546Z Reads: 120

```
The damn bt is not pairing anyway.
```

---
## \#51 Posted by: monsterbuilder Posted at: 2019-01-15T16:14:00.070Z Reads: 121

```
I was thinking about this the other day.  Wondering if it would be worth putting a connector on the BT that is accessible from the outside of the enclosure.  Would it be practical to only connect the BT to the enclosure when you need to change settings or check the individual pack voltage?
```

---
## \#52 Posted by: janpom Posted at: 2019-01-15T16:18:17.920Z Reads: 123

```
I would first do some measuring on how much power the BMS draws when idle with and without the BT connected. It can very well be that the difference is negligible. If there's a significant difference, though, then sure, you could definitely route the BT connector outside of the enclosure. It's 4 pin JST-XH and you could even change it to something waterproof.
```

---
## \#53 Posted by: janpom Posted at: 2019-01-15T16:23:01.890Z Reads: 124

```
The measuring may be a bit tricky though. I think it doesn't only draw power from the whole battery pack but from some sub-parts as well. Ideally you would put a multimeter on all balance leads. I only have two, one of which is this one. :smiley:

![IMG_1105|690x492](upload://k4s4VslnxkBjpDOMkUmS62gXkXA.jpg)
```

---
## \#54 Posted by: deucesdown Posted at: 2019-01-15T16:24:59.465Z Reads: 123

```
[quote="monsterbuilder, post:51, topic:80340"]
Wondering if it would be worth putting a connector on the BT that is accessible from the outside of the enclosure.
[/quote]

Yeah I had seriously considered putting a toggle switch in, and forgot :slight_smile:

[quote="janpom, post:52, topic:80340"]
measuring on how much power the BMS draws when idle with and without the BT connected
[/quote]

https://www.endless-sphere.com/forums/viewtopic.php?t=94522#p1384394 has some data

But I think different units seem to have different behavior.
```

---
## \#55 Posted by: deucesdown Posted at: 2019-01-15T16:34:36.239Z Reads: 121

```
[quote="rojitor, post:50, topic:80340, full:true"]
The damn bt is not pairing anyway.
[/quote]

When this happens to me I close the app, turn off bluetooth, start the app. app will start bluetooth, and usually can scan and bind.
```

---
## \#56 Posted by: rojitor Posted at: 2019-01-15T17:05:17.027Z Reads: 125

```
I do not have any led lit. WTF?
![ae_1547568689627|281x500](upload://1tm5RRALz7qBVqVx7nM6sIRGGl3.jpeg) 
Does It have leds or not?
```

---
## \#57 Posted by: Wisp Posted at: 2019-01-15T17:08:18.298Z Reads: 125

```
Can someone that has an LLT BMS confirm if the 'balance start voltage' cannot be set lower as 4.17? In the datasheet it says min 4.17, typical 4.2 and max 4.23. But I kinda hope that I could put it to 4.1 :slight_smile:

Same for over-discharge protection voltage.
```

---
## \#58 Posted by: deucesdown Posted at: 2019-01-15T17:10:44.210Z Reads: 122

```
I'm using one with A123, and have balance start set to 3.4v.

IIRC I attempted to convert a lithium ion 10s one to A123 15s (failed), and was able to change all the values.
```

---
## \#59 Posted by: billappleton Posted at: 2019-01-15T17:27:44.337Z Reads: 120

```
this conversation is why l like an external bms :)
```

---
## \#60 Posted by: deucesdown Posted at: 2019-01-15T17:36:13.313Z Reads: 120

```
Mr Smug. :slight_smile: I'll take a bit of the shine off ;)

One of the issues with a non-permanent balancing solution is the cycle life of the contacts for the balance leads.

For example JST-XH which is commonly used for lipo balance leads:

http://hansenhobbies.com/products/connectors/Connectors.pdf

[quote]
Terminals:
We highly recommend using only gold terminals for your connectors. Tin plated contacts usually have a life of about 10 cycles (a cycle being plugging in and unplugging) before the contact goes outside of its rated specs (possible specs being contact resistance and holding strength). Basically, the plating starts to rub off and the contact becomes prone to oxidation, and the contact(s) start to lose their springiness, increasing contact resistance. “Contact resistance” refers to electrical resistance, which can impede power going to the servo and possibly disrupt the servo signal. In most electronics applications the connector would be plugged in once and never touched again, so 10 cycles would be fine, but they’re simply not meant for the repeated use seen from hobbyists. Gold connectors have a life of 50-100 cycles, offer lower contact resistance, and are extremely resistant to corrosion. These numbers probably still seem low but keep in mind that the contact isn’t going to fail after 100 cycles, it will just gradually increase in contact resistance and decrease in holding strength (the springiness of the contacts is reduced). You might notice the same thing happening to the outlets near your kitchen counter. If your connector doesn’t plug in firmly anymore, that’s a good indication to replace it.
[/quote]
```

---
## \#61 Posted by: Benjamin899 Posted at: 2019-01-15T17:37:55.030Z Reads: 111

```
any recommendation?
```

---
## \#62 Posted by: billappleton Posted at: 2019-01-15T17:46:11.663Z Reads: 112

```
All of my jst connectors are intermediate and can be replaced, the charging cable too. But that is good info in your post.
```

---
## \#63 Posted by: Hummie Posted at: 2019-01-15T20:25:51.769Z Reads: 113

```
I skimmed the pdf and interesting but for the min cycles of the plug your stating (didn’t see it)I think they’re being used w a servo where the voltage drop from increases resistance over cycles could effect the communication w the servo but when used with balance wires it wouldn’t be a problem. 

Replacing the balance plugs the bare wires get so close I sure don’t want to ever do that.
```

---
## \#64 Posted by: deucesdown Posted at: 2019-01-15T20:33:48.826Z Reads: 115

```
When I'm messing around with my hobby chargers with "NIST traceable voltmeters", the voltages always seem a bit all over the place. Granted it's showing 3 digits of precision, and that third digit might as well be fiction. but we're trying to hit 2 digits of precision so the 3rd digit actually matters... And it always seems to be a little off from my "nice" multimeter.

Anyway, I feel like the balance leads are not consistently good connection. I'm always doubting what I see.

[quote="Hummie, post:63, topic:80340"]
didn’t see it)
[/quote]

Bottom of first page :)
```

---
## \#65 Posted by: Hummie Posted at: 2019-01-15T21:21:22.923Z Reads: 114

```
”
We highly recommend using only gold terminals for your connectors. Tin plated contacts usually have a life of about 10 cycles (a cycle being plugging in and unplugging) before the contact goes outside of its rated specs (possible specs being contact
resistance and holding strength). Basically, the plating starts to rub off and the contact becomes prone
to oxidation, and the contact(s) start to lose their springiness, increasing contact resistance. “Contact
resistance” refers to electrical resistance, which can impede power going to the servo and possibly disrupt the servo signal. In most electronics applications the connector would be plugged in once and never touched again, so 10 cycles would be fine, but they’re simply not meant for the
repeated use seen from hobbyists. Gold connectors have a life of 50-100 cycles, offer lower contact resistance, and are extremely resistant to corrosion. These numbers probably still
seem low but keep in mind that the contact isn’t going to fail after 100 cycles, it will just gradually
increase in contact resistance and decrease in
holding strength (the springiness of the
contacts is reduced). You might notice the same thing happening to the outlets near your
kitchen counter. If your connector doesn’t plug in firmly anymore, that’s a good indication to replace it.”

I’ve never replaced a plug on my kitchen counter and never heard of anyone doing that!  
I have had balance plugs break though but almost always from losing their connection to the battery, at that end.
```

---
## \#66 Posted by: jneumann Posted at: 2019-01-17T09:52:18.063Z Reads: 115

```
Question for those that have the smart BMS.Does it come with the balance cable? Also I'm tossing up between the 100a model and the 20a model. Still not sure if I want to go charge only or not. For those that have the 100a version did you struggle to fit it in your enclosure? It seems quite large
```

---
## \#67 Posted by: Andy87 Posted at: 2019-01-17T09:53:14.811Z Reads: 115

```
[quote="jneumann, post:66, topic:80340"]
Does it come with the balance cable?
[/quote]

Mine came with, like all bms I got from bestech had them included too.
```

---
## \#68 Posted by: janpom Posted at: 2019-01-17T10:25:53.444Z Reads: 113

```
Mine too came with a balance cable.
```

---
## \#69 Posted by: Ian-mountainboard Posted at: 2019-01-20T15:02:26.368Z Reads: 114

```
What are peoples thoughts on this bms
https://fr.aliexpress.com/item/Smart-Display-300A-200A-150A-100A-70A-Lithium-Battery-Protection-Board-Balance-BMS-Coulomb-Meter-Lithium/32826820690.html?spm=a2g0w.10010108.1000023.14.b50d2bbbUkjBeD
I'm hoping to use it in a mountain board so in would like to have a high current discharge.
```

---
## \#70 Posted by: Andy87 Posted at: 2019-01-21T11:38:14.684Z Reads: 111

```
I woud say it´s the same
https://www.electric-skateboard.builders/t/monitoring-individual-cell-voltages/80340/21?u=andy87
```

---
## \#71 Posted by: janpom Posted at: 2019-01-21T20:04:34.436Z Reads: 112

```
I just came across the [Neptune Lite](https://www.speedict.com/product-page/neptune-lite) and I like it a lot. It's not exactly a BMS. It merely monitors cell voltages and sends out the data via BT, but then again it's really small (41 x 35 x 7 mm). It comes with a very cool looking Android app with a ton of features. Unfortunately no iOS (yet?). Still, I wish I have known about it before I started routing all the balance wires out of my enclosure. :smiley:
```

---
## \#72 Posted by: Vanarian Posted at: 2019-01-22T13:31:23.981Z Reads: 109

```
Hey I'm gonna propose a scalable and working solution, it was a work made by an E-S member (**[AfdhalAtiffTan](https://endless-sphere.com/forums/memberlist.php?mode=viewprofile&amp;u=52772)**) back in the days. He called it an active battery balancer (compared to his previous passive dissipative one with shunt regulator). 

Claimed accuracy was 99.99% with him using various used laptop 18650 cells. It is built around 2S daisy modules between each cell so you can scale the voltage up as much as needed, no limit. 

Main con is : cost adds up quick for bigger batteries. 

Plugging in parallel if possible might be an efficient way to shave down price from expensive to super affordable (circa 40$ for 12s4p for example). But I don't know if it is doable or relevant? Is it how classic BMS usually work ?

Here is a link to his page :beers: 

http://www.afdhalatifftan.com/2017/06/low-cost-active-battery-balancer.html

Edit : This might deserve a separate build thread!
```

---
## \#73 Posted by: janpom Posted at: 2019-01-23T16:54:06.576Z Reads: 105

```
I looked at it and I don't understand it. Could anyone translate it to a 5-year-old language for me?

My (possibly wrong) understanding is that it can balance 2S by charging both cells by using the average voltage. So for example if one is 4V and the other is 3V it would charge at 3.5V and the charger voltage would gradually increase as the weaker cell is getting charged and it would converge to 4V. Right?

Now, how is that helpful for more than 2S? I also still don't quite understand how exactly the charging works.
```

---
## \#74 Posted by: Vanarian Posted at: 2019-01-23T21:11:06.063Z Reads: 102

```
In not exact terms, it kinda transfers exceeding energy from most charged cell toward less charged cell insured to balance it. Reference voltage is external voltage. 

So both will end up charged at same level ; under discharge I think it still does same job (balance is made at few mA current) but I was only interested in charging aspect.

You need 1x module "between" each cell in série. So 4s = 3 modules, 6S = 5, 12s = 11 etc...

It daisy chains. So your cells are always watched in regard of their immediate neighbor, which forms a group... 

Hope my half assed explanation is not too confusing (it is not a scientific description lol)
```

---
## \#75 Posted by: deucesdown Posted at: 2019-01-23T23:30:09.963Z Reads: 100

```
Does this mean all cells are being continuously balanced? This is not necessarily good. Hmmm but I guess that's the situation with cells in a parallel-group. Let me go into a hole and reconsider....
```

---
## \#76 Posted by: janpom Posted at: 2019-01-23T23:30:13.256Z Reads: 100

```
That's a great explanation. Thank you! That sounds really useful. Unfortunately nothing to do with measuring cell voltage, so somewhat misplaced in this thread. Thanks for sharing the link anyway. It's definitely an interesting approach to balancing cells.
```

---
## \#77 Posted by: janpom Posted at: 2019-01-23T23:45:25.439Z Reads: 101

```
I'm still unclear on a few things. IIUC, there's a buck converter for each 2 cells that acts as a charger. It charges at the voltage that's equal to the mean of the two cells. I guess it takes energy from the 2s pack and transfers it to one of the cells. Does it always charge the weaker cell though? It looks like it's hardwired to only one of the cells, so in case that cell is lower of the two, it can balance the 2s pack, but if it's the higher one it can't. Is that a wrong interpretation?
```

---
## \#78 Posted by: Vanarian Posted at: 2019-01-24T00:11:44.158Z Reads: 99

```
Well from what Adfhal told me back then, there was a minimum voltage thresold to reach before balancer triggers ON so under voltage thresold it will let cells charge first then balance on "top" :thinking: Positive aspect is : cells won't drift to overcharging state no matter what.
```

---
## \#79 Posted by: Vanarian Posted at: 2019-01-24T00:16:14.635Z Reads: 101

```
Not sure to have understood everything ; are you asking if it can bring a higher cell down to a lower voltage level (ex : 4.15 instead of 4.2) instead of just bringing both cells to higher cell voltage ? IIRC yes there is a way, need to dig in my ES PMbox to check infos. 

But basically it will try it best to bring down/up to reference voltage level so it might need to be set on charger firsthand.
```

---
## \#80 Posted by: janpom Posted at: 2019-01-24T00:24:01.688Z Reads: 98

```
Hm, so the buck converter is connected to the first cell of the 2s pack and it either charges it or discharges it to achieve balance with the second cell? That would make sense.

You would then need 11 buck converters for balancing a 12s pack and that would be pretty bulky, wouldn't it? A bit like the "Frankenstein charger"?
```

---
## \#81 Posted by: Vanarian Posted at: 2019-01-24T00:32:06.614Z Reads: 103

```
You got it right ! I'm sure a 2 layer PCB (up and down face) can be made the size of a coin for each 2S, problem is caps ; maybe tinkering with ceramic caps instead of electrolytic caps can help reduce further size if values are good ? 

Maybe a VESC / credit card sized PCB with soldering terminals can be achieved too. Should keep it compact and clean, just run balance cables through your pack with JST pins for example. Or a modular type (like you keep the tiny PCBs and you stack them all together on a "card" sized support) to keep scalability.
```

---
## \#82 Posted by: janpom Posted at: 2019-01-24T00:47:30.813Z Reads: 105

```
Right. Makes sense. It's an interesting design, but I'm not sure how much value there is. The thing is that you can buy tiny BMS-es for some $10. How would this buck converter thingie be better than that?
```

---
## \#83 Posted by: janpom Posted at: 2019-01-26T19:01:16.401Z Reads: 105

```
[Here's](https://gist.github.com/janpom/8e5c29092a473a62cbece80551568fe3) the code for my LLT Smart BMS display. This is mainly for @Andy87. 

![IMG_1636|333x500](upload://1UXrIthu7w8xsnTtEWlt5EBt6BF.jpeg) 

The code requires two files from the DAVEga repo to work. See the comment below the gist.

You can use the DAVEga as is and connect it to the Smart BMS UART port. However, **you must not connect the VCC**, since the BMS outputs 10V and that would fry DAVEga. Only connect GND, RX, TX, and either use another power source or put a 10V to 5V voltage regulator between the devices.

Alternatively, use the Arduino Nano (or any other arduino) with the 2.0" TFT DAVEga display. Nano has a built-in voltage regulator and you can safely feed it with 10V. Here's the [schema](https://www.electric-skateboard.builders/t/davega-battery-monitor-odometer-speedometer/71509/209?u=janpom) for wiring up the display to Nano (ignore the buttons; replace VESC with the BMS).
```

---
## \#84 Posted by: Andy87 Posted at: 2019-01-26T19:17:02.458Z Reads: 99

```
That’s an amazing work 👌👍
Gonna order an arduino nano now and hope it will arrive after my vacation 😌
```

---
## \#85 Posted by: Benjamin899 Posted at: 2019-01-29T18:43:10.833Z Reads: 92

```
I have a question towards the LLT Smart BMS. Is there a limit to the values you can set? I am not talking about the balancing/bleeding. I mean the charge Voltage per Cell. The Datasheet shows a min and max. So are we only able to chose in that spectrum or what?
Here the reference. Because if that is the case than this is not that great.
![PNG|559x499](upload://q3NUhCS5svI0VsFsY2l2Gvohsar.jpeg)
```

---
## \#86 Posted by: janpom Posted at: 2019-02-10T12:51:20.797Z Reads: 88

```
Yes, you can set various charge MOSFET cutoff limits, including max individual cell voltage and max total voltage. You can set it either using the mobile app or the PC app. Android app can be downloaded form the manufacturer's website. iOS app is available from the App Store for $1. I tested both. Both work well.
```

---
## \#87 Posted by: janpom Posted at: 2019-02-10T13:02:55.035Z Reads: 85

```
I have a bit of bad news regarding the LLT Smart BMS. The UART port outputs 10V but apparently it can only supply very small current. I assume it's just enough to drive the bluetooth module. I tried using it to power my NodeMCU board and it didn't work. That's a bit annoying. I will have to power my external BMS charger from the 10S battery using a DC-DC step-down converter. 

My first experiments with this didn't go well. I had [one of these](https://www.aliexpress.com/item/10A-DC-DC-6-5-60V-to-1-25-30V-Adjustable-Buck-Converter-Step-Down-Module/32861200188.html) on hand that I have never used before. I connected my 10S battery pack to the input and my multimeter to the output in order to set the correct output voltage. I got magic smoke after about 2 seconds. :frowning: Fortunately it looks like only the buck converter is dead. No other damage. After some googling it looks like the problem might have been that there was no load at the output. Ordered new buck converters. Will try again later.
```

---
## \#88 Posted by: Benjamin899 Posted at: 2019-02-10T13:17:14.173Z Reads: 84

```
I think you misunderstoof me. Is it possible to go outside of the Min/Max of the Datasheet i posted, because if not, then this BMS is not rly that great. I want for example to set the Max Charge per Cell to 4V, which would not be possible.
```

---
## \#89 Posted by: janpom Posted at: 2019-02-10T13:52:51.508Z Reads: 86

```
Ah, right, sorry. I just tested it and I can set the overvoltage protection threshold in the 4.0-4.3V range, so 4V would still work but no less than that. The overvoltage release threshold can be set in the 3.9-4.3V range.

BTW, it turns out you can't set these with the iOS app, only with the Android app.

I was also wrong saying that the overvoltage protection can be set based on total battery pack voltage. I though I saw that option somewhere, but couldn't find it now. At any rate, setting it based on cell level voltage makes more sense anyway.
```

---
## \#90 Posted by: Benjamin899 Posted at: 2019-02-10T13:57:06.875Z Reads: 80

```
weird, why do they not put it into the datasheet.
```

---
## \#91 Posted by: deucesdown Posted at: 2019-02-10T15:35:03.414Z Reads: 82

```
Sadly my 15s smart bms burned. I plugged in an unpowered charger, and when I powered it up I noticed voltage is very low. Phone app has a big red circle at top rigth with "IC" in it. I open up the board and the BMS is hot at the balance lead connection point, and it smells of burnt electronics. I've not inspected further. Sigh.

[quote="janpom, post:87, topic:80340"]
10S battery using a DC-DC step-down converter.
[/quote]

You might have better long term luck with a BEC/SBEC/UBEC from hobbyking? The dc-dc converter boards are usually terribly over-rated, and need supplemental cooling to stay alive at full load. And it's a big step down.

This one's pretty cool, dual voltage, pretty decent current but a little $$$. I bought one for lights and horn, but ended up not implementing the lights.

https://hobbyking.com/en_us/turnigy-multistar-twin-output-5-10-amp-6-50v-sbec-for-lipoly.html
```

---
## \#92 Posted by: janpom Posted at: 2019-02-10T16:13:16.171Z Reads: 82

```
Thanks for the tip. I'm sorry about your BMS. That sucks. Probably a bad piece. Mine has been working OK so far.
```

---
## \#93 Posted by: ducktaperules Posted at: 2019-04-15T12:45:23.254Z Reads: 78

```
@janpom I have been doing some reading regarding the LLT Smart BMS display and found some interesting things . . . 

It seems that the LLT Smart BMS is using the Atmel ATmega328P (same as most old arduinos) 
![](https://opensourceebikefirmware.bitbucket.io/development/images/57-1.png)

The board has a 6 pin standard programming header so that it can be easily reprogrammed.

Additionally it would seem that its using a well known and documented cell monitoring chip (Texas Instruments BQ76940) with working arduino example codes available https://github.com/nseidle/BMS .

Furthermore it seems like there are other projects that are using this BMS with custom open firmwares such as this Xiaomi battery mod https://github.com/BotoX/xiaomi-m365-compatible-bms in which they are using the LLT bms to emulate the original battery serial protocall.

BMS also has current measuring built in, could possibly be modified with a larger external shunt to do current monitoring whilst being used in a charge only bypass configuration.

Seems like this bms has:
 - 10s-15s opperation.
 - runs arduino compatible hardware 
 - capable of up to 60A discharge 
 - current monitoring
 - exposed serial port

Maybe we should be making our own firmware for this BMS so that we can use any known serial protocol rather than trying to reverse engineer theirs. It could easily share data with the vesc like DieBieMS does or tell a Focbox unity to limit power or gracefully shut down in a fault condition where you have single cell failure. Also with a custom firmware we could change cell charge and discharge voltage limits to whatever we wanted. Could even drive an i2c oled directly from bms if i2c pins are available or maybe using bit-banged i2c on the serial port.

What you think?

Ps. I just ordered one, i think this is worth investigating further :)
```

---
## \#94 Posted by: janpom Posted at: 2019-04-15T13:06:47.950Z Reads: 77

```
I'm aware of most of that and I agree that there's a lot of potential in that BMS. I have already used it for building an external BMS charger with a screen that displays individual cell voltages, charge current and other info:

https://www.electric-skateboard.builders/t/cheap-diy-12s-balance-charger-idea/76695/64?u=janpom

https://www.electric-skateboard.builders/t/no-words-just-pictures-delete-words/2992/9719

https://www.electric-skateboard.builders/t/no-words-just-pictures-delete-words/2992/9515?u=janpom

It would be cool to have a custom FW for the BMS. 

Alternatively, one could make an adapter for communicating with other devices. For example, you could make a simple CAN enabled gadget that plugs into the Smart BMS UART port and relays the information to the VESC emulating the DieBieMS protocol. That should be a lot easier than making a custom BMS FW. Also, the BMS doesn't have CAN.

I have already figured out how to read all available info from the BMS over UART. I just don't know how to send commands to it. I haven't found any documentation of that part of the protocol. Maybe that's not so important though.
```

---
## \#95 Posted by: ducktaperules Posted at: 2019-04-15T14:56:36.698Z Reads: 73

```
[quote="janpom, post:94, topic:80340"]
just don’t know how to send commands to it. I haven’t found any documentation of that part of the protocol.
[/quote]

This code seems to be able to write to control the mosfets https://github.com/bres55/Smart-BMS-arduino-Reader

he also links to this document describing some of the protocol https://drive.google.com/file/d/0B3UXptx89r4NZ3VLTHlVS1ZGTTQ/view

if we had custom firmware do you think it would be possible to pwm the charge fets and get user configurable charge current? would be great to use the same charger for trickle, standard or fast charge.
```

---
## \#96 Posted by: DougM Posted at: 2019-04-15T15:07:35.617Z Reads: 71

```
After my battery spot welder went iffy I started thinking about the same thing - what if a weld came loose and I lost one of the cels in a P pack.  This would be easy to identify if I could read the individual P voltage delta while riding.

But I don't want to know when the thing is running correctly, what I want is an alarm.  So I built a small board that monitors the voltage of each P pack with reference to the other packs (mean, probably, haven't coded it yet) and if one is significantly different than others display a message on a small OLED display (because I had a bunch of them lying around).

This board plugs into the charge port (conveniently my charge ports are external balance so all the balance leads are available)

So in terms of your model it might be helpful to add some sort of alarm capability if the thing gets too far out of wack.
```

---
## \#97 Posted by: janpom Posted at: 2019-04-15T17:25:29.128Z Reads: 72

```
[quote="ducktaperules, post:95, topic:80340"]
he also links to this document describing some of the protocol [https://drive.google.com/file/d/0B3UXptx89r4NZ3VLTHlVS1ZGTTQ/view ](https://drive.google.com/file/d/0B3UXptx89r4NZ3VLTHlVS1ZGTTQ/view)
[/quote]

That's what's available on the manufacturer website. It documents only reading from BMS, not writing into it.

[quote="ducktaperules, post:95, topic:80340"]
if we had custom firmware do you think it would be possible to pwm the charge fets and get user configurable charge current?
[/quote]

Sounds like that should work but I'm by no means an expert.

The million dollar question is who would do the custom FW coding. It's a lot of work and I already have a lot on my plate.
```

---
## \#98 Posted by: janpom Posted at: 2019-04-15T17:28:44.969Z Reads: 73

```
[quote="DougM, post:96, topic:80340"]
So I built a small board that monitors the voltage of each P pack with reference to the other packs (mean, probably, haven’t coded it yet) and if one is significantly different than others light up an LED.
[/quote]

I'm curious. How exactly have you done that? Did you use a voltage divider?

[quote="DougM, post:96, topic:80340"]
So in terms of your model it might be helpful to add some sort of alarm capability if the thing gets too far out of wack.
[/quote]

You may want to check out the [Chargery BS12](http://www.chargery.com/cellSaver12S.asp). It's a cell monitor and it has a buzzer for overvoltage/undervoltage alarm. The undervoltage threshold is configurable. I haven't had a chance to put my hands on one but the feature specs look promising.
```

---
## \#99 Posted by: DougM Posted at: 2019-04-15T18:18:59.055Z Reads: 74

```
[quote="janpom, post:98, topic:80340"]
How exactly have you done that?
[/quote]

Yes, a series of resistor dividers fed into a bunch of ADC's (on a Teensy 3.2).  The output is one of those little OLED displays that will be blank unless it detects an anomaly, then will display which P bank is having issues and what the current voltage is.

Basically the same as the Chargery BS12 you mention, but not as sophisticated.

I haven't written the code for it yet so I'm not sure how well it will work with this first rev of the hardware.
```

---
## \#100 Posted by: janpom Posted at: 2019-04-15T19:09:12.886Z Reads: 70

```
Cool. I tried doing [something similar](https://www.electric-skateboard.builders/t/cheap-diy-12s-balance-charger-idea/76695/68?u=janpom) but the resolution is too poor. I used the 10-bin ADC pins of the ATTINY-84. I planed to redo it with higher resolution ADCs but I never found the time for it.

Do you have a PCB design for yours and/or some pics?
```

---
## \#101 Posted by: DougM Posted at: 2019-04-15T21:20:15.477Z Reads: 73

```
[quote="janpom, post:100, topic:80340"]
resolution is too poor
[/quote]

I'm worried about that too.  I'll know for sure when the boards get here and I code it up, but it might be completely useless :slight_smile:

I'm happy to share both the schematic and the board layout, but the board will be completely useless to you unless you use the same charge port that I use, which is completely custom (the idea being that when I start my ride I plug the monitor board into the charge port for the duration of the ride)

Also, because I needed more analog lines than the Teensy 3.2 module provided, I ended up spinning my own custom Teensy implementation by buying the pre-programmed MLK04 from PJRC.
```

---
## \#102 Posted by: Ian-mountainboard Posted at: 2019-04-15T21:26:17.501Z Reads: 75

```
Sorry to interupt the chat but i just welded part of my battery together and the left cell is 13 degrees hotter then all the other ones. I dident short it out or anything.![15553633848031773625266|281x500](upload://1C1gtFIrXuLa6SA4IBZJ4DOxn6a.jpeg) just a bit confused
```

---
## \#103 Posted by: janpom Posted at: 2019-04-15T21:28:57.347Z Reads: 70

```
@Ian-mountainboard Please start a new thread if you need any help in that. This is about monitoring cell voltages. You're off topic.
```

---
## \#104 Posted by: janpom Posted at: 2019-04-15T21:32:16.605Z Reads: 72

```
[quote="DougM, post:101, topic:80340"]
I’m happy to share both the schematic and the board layout, but the board will be completely useless to you unless you use the same charge port that I use, which is completely custom
[/quote]

I understand. I don't think I would want to use it, but I would still like to see how you designed it. This forum is a lot about sharing ideas and getting inspired by each other.
```

---
## \#105 Posted by: DougM Posted at: 2019-04-15T23:40:29.714Z Reads: 75

```
Sure, here's the resistor dividers

![image|496x500](upload://fGrDQY6STisL2KMtMjRvOY46w2d.png) 

Here's the Teensy 

![image|620x500](upload://jZbXU7vcQDauktQoBvxxvXETsxa.png) 

And here's the board

![image|402x500](upload://sNud4z3NBj8BOELFbcAQ6GXdig6.png) 

Let me know if you need more detail
```

---
## \#106 Posted by: lrdesigns Posted at: 2019-04-16T11:09:48.654Z Reads: 70

```
I think I got a ticket to ride this train, how do I get on board? 

![image|666x500](upload://ve8W2X87GVzYP5eEWcE1HNW1k33.jpeg) ![image|666x500](upload://hnUiZJtYCfaZpApCfFfUgFfaUxD.jpeg) ![image|666x500](upload://uNzkEwEbKSD2WtdcSAEymM1qftU.jpeg) ![image|375x500](upload://rc92dk8cASK4Rc08adnaLc3VPen.jpeg) ![image|666x500](upload://2UXtYs1yXzh9OjdkYw88whRfUNg.jpeg)

There is a small amount of clear waterproofing over the IC’s, :+1: I will be adding more.
```

---
## \#107 Posted by: janpom Posted at: 2019-04-16T11:17:44.769Z Reads: 69

```
That depends on what exactly you're after. Do you want to get cell voltage readings on a small display? If so, the easiest thing to do is take a DAVEga (which you can now conveniently purchase at Flipsky :smile:), upload [this FW]( https://gist.github.com/janpom/8e5c29092a473a62cbece80551568fe3) and plug it into the BMS UART port. The only caveat is that you can't power it from the BMS. You must not connect the VCC. You need another power source.
```

---
## \#108 Posted by: janpom Posted at: 2019-04-16T11:19:11.628Z Reads: 69

```
BTW, why 14S?
```

---
## \#109 Posted by: lrdesigns Posted at: 2019-04-16T11:20:02.016Z Reads: 70

```
Backwards compatible with the future! Not any larger really.
```

---
## \#110 Posted by: janpom Posted at: 2019-04-16T11:23:29.395Z Reads: 71

```
Well, the only difference between 12S and 14S is in how it's set up, so unfortunately you just added more trouble to yourself by ordering the 14S if you're not going to use a 14S battery. You will need to reconfigure both the HW and the FW. Did you get the PC module? The FW can't be reconfigured without it. (Technically, it can be done be we would need to reverse engineer the communication protocol.)
```

---
## \#111 Posted by: lrdesigns Posted at: 2019-04-16T11:52:52.056Z Reads: 67

```
Oh train passes by :bullettrain_side: haha. 

I guess just use the phone then. ☺️

Was thinking 13s charged to 4.0, had to go up to 14. or if some high voltage vescs come out later.
```

---
## \#112 Posted by: janpom Posted at: 2019-04-16T12:05:56.533Z Reads: 66

```
[quote="lrdesigns, post:111, topic:80340"]
Was thinking 13s charged to 4.0, had to go up to 14. or if some high voltage vescs come out later.
[/quote]

That's not how it works. You have a single piece of HW that supports anything between 10S-15S. However, you need to configure it for given number of cells. If it's configured for 14S, you can't use it for 12S. You have to change the configuration first. The HW mod is simple. You just short some of the balance lead pins. The FW mod is actually also simple if you have the PC module. If you didn't get one you'll be best off ordering it now since it costs about $5.
```

---
## \#113 Posted by: lrdesigns Posted at: 2019-04-16T12:43:27.437Z Reads: 68

```
Oh $ thanks, what’s the hardware mod I can solder? It currently has 13-14 bridged. 

![image|281x500](upload://88S6KDcHM8QEHD679NeVUFowzpd.jpeg)
```

---
## \#114 Posted by: janpom Posted at: 2019-04-16T13:02:03.629Z Reads: 67

```
Look for the Texas Instruments BQ76940 datasheet. They have nice diagrams somewhere near the end of the document (IIRC).
```

---
## \#115 Posted by: lrdesigns Posted at: 2019-04-17T00:43:12.273Z Reads: 70

```
Thank you so much @janpom for leaving me enough bread crumbs to figure out how to use this BMS at 12s. Really sorry to clog up your thread. I checked the data sheet and found this :arrow_down: 

![Smart%20BMS%2012s%20short%20pins|690x335](upload://otZDx3ZKjmjDRx3AMPEQZDg133C.jpeg) 

http://www.ti.com/lit/ds/symlink/bq76940.pdf

I will still be ordering the PC programer but it wont come in time for my planed easter vacation building session.
```

---
## \#116 Posted by: deucesdown Posted at: 2019-04-17T00:57:31.634Z Reads: 70

```
So I attempted this kind of operation based on info in the endless sphere thread, and failed. I can't remember, but changing the solder bridges and tweaking software to change the series count. For me a few cells were reading very very low after the conversion. I'll try looking at that pdf to see if I missed anything.

Also, I fried 2 of these! Both times I plugged in a unpowered DPH5005 PSU into the charge port, and poof. The first unit survived a few of these I'm sure, but the second unit fried the first time I did this. I'm thinking the PSU has some caps on the output, and maybe the sudden inrush killed the bms. Weird, you'd think that's exactly the kind of stuff the bms would prevent. I just received my 3rd unit, and added a 5a fast blow fuse on the charge port. I'll try not to test it...

One day I'll try to figure out what blew and repair, but it'll be a long road for me, too much of a electronics n00b.

Oh btw I'm guessing a usb-ttl adapter will work for the pc app. Something like this:

https://www.amazon.com/JANSANE-PL2303TA-Serial-Console-Raspberry/dp/B07D9R5JFK

I acquired a few for playing with arduino stuff and the BT05/HM10 modules. I'll test it and report back.

Oh lol one more thing. In the PC app you can change a field, I believe "application name" -- on mine the value is "SZLLT". This name is also displayed in the xiaoxiang phone app. It's quite helpful if you have multiple boards with this BMS. I also tried to change the name of the bluetooth device using the usb-ttl thing, and failed. Some have reported newer versions of the bms use a cheaper BTLE dongle that's not configurable.

EDIT I keep remembering things after I hit save. If hooked up for discharge, I believe the BMS can be used as a power switch. There are solder points on the board, and the software has provisions. I believe the use case is to password lock the bms OFF via phone app for anti-theft. I'm not sure if all units have all the components populated though.
```

---
## \#117 Posted by: deucesdown Posted at: 2019-04-17T02:19:35.061Z Reads: 71

```
[quote="deucesdown, post:116, topic:80340"]
Oh btw I’m guessing a usb-ttl adapter will work for the pc app. Something like this:

https://www.amazon.com/JANSANE-PL2303TA-Serial-Console-Raspberry/dp/B07D9R5JFK

I acquired a few for playing with arduino stuff and the BT05/HM10 modules. I’ll test it and report back.
[/quote]

Confirmed, works perfectly.

The device renaming is mixed results. Setting "Device Manufacturer" in the pc app changed the title in phone app for one unit, but not for another unit.
```

---
## \#118 Posted by: janpom Posted at: 2019-04-17T05:08:41.828Z Reads: 73

```
[quote="deucesdown, post:116, topic:80340"]
Oh btw I’m guessing a usb-ttl adapter will work for the pc app.
[/quote]

I never thought of that. @LRDesigns, can't you just use the one you have for DAVEga? Connect GND, TX, RX pins to the BMS UART port. It's worth a try.
```

---
## \#119 Posted by: drone001 Posted at: 2019-07-29T03:51:45.667Z Reads: 52

```
I don't understand how you connect a 12s6p to this charger. The connector on the balance wires is a 13 pin connector. Are you happy with the purchase?
```

---
## \#120 Posted by: billappleton Posted at: 2019-07-29T17:28:07.007Z Reads: 50

```
there is a connection diagram on the build thread. let me know if that doesn't answer your question

https://www.electric-skateboard.builders/t/hellboy-eboosted-enclosure-sector-9-meridian-board-focbox-unity-evolve-supercarve-trucks-psychotiller-6369-motors-unikboard-motor-mounts-pelican-bay-12s4p-battery-abec-107mm-wheels-hoyt-puck-remote/77933
```

---
## \#121 Posted by: Jonisonvespa Posted at: 2019-07-30T00:04:14.764Z Reads: 46

```
Hello really interested in the 100a bms in this thred, what is the typical current draw using 2 motors worst possible case 270Kv
Thanks
```

---
## \#122 Posted by: drone001 Posted at: 2019-07-30T02:33:56.323Z Reads: 46

```
oh..you're hellboy...i mean your build was one of the builds that inspired my first DIY. I own a CGT, At first I planned to rebuild it with a FOCBOX Unity. but later decided on something else. Nice build by the way. back on subject...the diagram was what i needed thx.
```

---
## \#123 Posted by: drone001 Posted at: 2019-07-30T15:03:38.806Z Reads: 40

```
what would make a battery charge to a different voltage every time i charge. one day it'll go to 90% the other day 88%, 59%,70.... confirmed from xt60 reading, charger is at 50.4V confirmed. have not measured from the balance plug because i'm unable to remove the plug from the BMS. clearance issues. Any help would be greatly appreciated. thx
```

---
