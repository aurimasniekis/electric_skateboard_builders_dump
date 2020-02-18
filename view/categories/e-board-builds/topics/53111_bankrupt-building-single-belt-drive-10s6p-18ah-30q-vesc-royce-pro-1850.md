# &ldquo;Bankrupt&rdquo; (BUILDING!)/SINGLE BELT DRIVE/10S6P 18AH 30Q/VESC/ROYCE PRO/$1850

### Replies: 303 Views: 11903

## \#1 Posted by: legend27 Posted at: 2018-04-22T10:54:55.267Z Reads: 938

```
Hi everyone :slight_smile: 

Im planning to build my own electric skateboard when i have sold my current board. The board i have right now is a Huger Tech Travel board (feel free to contact me if you're interested. I live in Denmark).
I have already found all the parts so i wanted to know if i needed something more and if the setup is going to work.
I want the board to be around 1000$ and be able to upgrade it in the future (which i am definitely going to do) .

The parts:
-Enclosure: Knuckles from @psychotiller (https://psychotiller.com/product/knuckles)
-Battery: 10s6p samsung 30q battery pack by me with 10s 80a BMS from Bestech (https://eu.nkon.nl/samsung-inr-18650-30q-3000mah.html and https://eskating.eu/product/10s-bestech-bms-80a-10s4p/)
-ESC and remote: Cheap ESC and remote from @diyeboard (http://www.diyeboard.com/v11-dual-belt-motor-sine-wave-foc-esc-speed-controller-p-522.html)
-Motor, wheels, trucks, etc.: Cheap kit from @diyeboard (http://www.diyeboard.com/dual-belt-drive-1400w2-n5055-motor-power-truckfront-truck-kit-p-422.html)
-Deck: Cheap deck from SkateShred (https://www.skateshred.com/wholesale-blank-longboard-decks/downhill-kicktail-dark-walnut-deck.html)
-Charger: 4A charger from @fottaz (https://eskating.eu/product/4-amp-fast-charger/)

And a lot of extras such as wires, charging port, battery indicator, etc.



Thanks for reading my post and feel free to tell me your opinion on my upcomming board.
```

---
## \#2 Posted by: FredrikHems Posted at: 2018-04-22T11:29:32.489Z Reads: 819

```
Part list seems ok, but there is a few things I will recommend. 

Get a vesc instead of that esc. It feels much better, and you will be able to push a lot more power through. 
If you are going to build your own battery you will need a spot welder too. These are quite expensive, around $150.
Instead of going with the DIYeboard parts, I would have built a single drive board to start with and upgrade that later if you feel the need for it. This way you can get a much higher quality board, with both vesc`s and a better quality/ higher performance board
```

---
## \#3 Posted by: legend27 Posted at: 2018-04-22T11:33:38.119Z Reads: 788

```
Thanks for the help! I will definitely take the into my consideration.
And in terms of the spot welder i plan on making this spot welder: https://www.youtube.com/watch?v=b_kGgPVrcCI&t=305s
```

---
## \#4 Posted by: psychotiller Posted at: 2018-04-22T15:38:02.906Z Reads: 758

```
I'm curious how you're going to fit a 10s6p pack with a huge bestech bms in my knuckles enclosure..even double stacked it's going to be tight with the speed controller.
```

---
## \#5 Posted by: treenutter Posted at: 2018-04-22T15:40:30.086Z Reads: 736

```
[quote="legend27, post:1, topic:53111"]
-Deck: Cheap deck from SkateShred
[/quote]

I think it’s worth it, given all the other high quality components you’re using, to buy a good quality deck from a reliable source. The deck is the heart of your build, and will dramatically impact the feeling of your ride.
```

---
## \#6 Posted by: legend27 Posted at: 2018-04-22T16:34:31.578Z Reads: 718

```
Yes... hopefully i can fit everything... I might upgrade to a vesc which will also make some more free space in the enclosure.

I've made a sketch that shows how im going to place my parts:

![eboard above|690x299](upload://1cQGTQYD6y1xlajKrXHnwyVKLlb.png)

![eboard side|690x137](upload://fRe0FF4kdrymPWgIcKBjACfMJq2.png)
```

---
## \#7 Posted by: legend27 Posted at: 2018-04-22T16:45:22.240Z Reads: 682

```
I kinda see what you mean. But why should i go out and spend 100$ more on this deck https://loadedboards.com/cantellated-tesseract-longboard-skateboard when they almost look identical? I know there is some fiberglass and bamboo in the more expensive one but is that really going to change the ride quality much?
```

---
## \#8 Posted by: FredrikHems Posted at: 2018-04-22T17:45:13.040Z Reads: 652

```
Dont rate a deck’s quality by How it looks- on a picture from internet..
```

---
## \#9 Posted by: gee Posted at: 2018-04-22T18:01:06.211Z Reads: 644

```
@legend27 your battery is 10s6p but the charger say 12s only...AND are you sure you want 4A/fast charging? Slow charging is better if you want your battery to last.  
PLEASE DOUBLE CHECK YOUR DIMENSIONS, IT WILL SAVE YOUR A LOT OF $$$. That's my advice.
```

---
## \#10 Posted by: legend27 Posted at: 2018-04-22T19:05:39.518Z Reads: 631

```
Ohh fu*k i didn't even see that! thanks! I think i will be going with this charger instead https://eskating.eu/product/2-amp-charger-10-and-12-s/ and thanks for the advice. Im sure it will help me!
```

---
## \#11 Posted by: gee Posted at: 2018-04-22T19:33:04.655Z Reads: 614

```
just in case, for the voltage option pick the 42v one. Check and make sure what type of charging port the charger is, and buy the correct one. I think that's 5.5 mm x 2.1 mm. 
Let me know how much you spend on the DIY spot welder. If you spend more than $100 then might as well buy the arduino spot welder. 
BMS is label for 80A **10s4p**. You're getting 10s6p and with samsung 3000 mAh **15A** so wouldn't that be 90A continuous? If so then you might have to bypass the BMS.
```

---
## \#12 Posted by: b264 Posted at: 2018-04-22T19:47:24.083Z Reads: 581

```
@legend27 you can save a lot of space in the enclosure by bypassing the BMS and using a little BMS for charging only
```

---
## \#13 Posted by: FredrikHems Posted at: 2018-04-22T19:58:43.089Z Reads: 580

```
The 30Q can do 20A continious, so for a 10s6p= 120A continious.. The BMS can take max 80A continious, but there is no way you’ll ever draw that much current for a long period of time.. usually only a couple of seconds max
```

---
## \#14 Posted by: psychotiller Posted at: 2018-04-22T20:07:12.024Z Reads: 567

```
I'm glad you told me that! :roll_eyes: 

It's still going to be tricky fitting 60cells into an 18" long enclosure.
```

---
## \#15 Posted by: treenutter Posted at: 2018-04-22T22:36:20.977Z Reads: 553

```
[quote="legend27, post:7, topic:53111"]
know there is some fiberglass and bamboo in the more expensive one but is that really going to change the ride quality much?
[/quote]

I think it will, but no pressure man it's all good.
```

---
## \#16 Posted by: Sender Posted at: 2018-04-22T23:25:22.215Z Reads: 582

```
You could also spend a bit more and get a really bad ass deck.  There is this company, or custom builder rather, that makes really awesome decks.  It is called Red Ember Boards. @psychotiller makes some enclosures to fit his stuff specifically (The Altar Wedge), which would alleviate all space concerns.

  Hell, I think that custom deck master may even frequent the forum 😉.... what is his handle again...

Oh yeah.... @treenutter.... LOL 

I agree that a single drive with high quality parts would be the best route.  You already found @psychotiller stuff.  Skip the diyeboard stuff and stay on his site for your mechanical stuff.   Add the second motor/vesc later.  

I would take a nice single drive that I could upgrade later all day long over getting a dual with much less quality components.  

In the end you will be MUCH happier with the finished product.

Good luck on the build!
```

---
## \#17 Posted by: legend27 Posted at: 2018-04-23T14:03:47.274Z Reads: 538

```
I think you're right about the BMS. I didn't really spend that much choosing aw BMS so thanks!
And i will let you know how much i spend on the spot welder :slight_smile:
```

---
## \#18 Posted by: legend27 Posted at: 2018-04-23T14:08:35.520Z Reads: 539

```
But then it won't protect the battery from discharging too much, right?
```

---
## \#19 Posted by: legend27 Posted at: 2018-04-23T14:12:03.630Z Reads: 536

```
I will definitely consider upgrading the deck, thanks!
```

---
## \#20 Posted by: legend27 Posted at: 2018-04-23T14:20:32.956Z Reads: 548

```
Thanks for letting me know. I have never heard of them before but i don't think im going to get a longboard since i  live in the city and has to get around some corners easy and quick.

I think im going to go with single motor now since i can save som money and get high quality parts.

Thanks for your comment. It's nice hearing what other people think so it isn't just my opinion.
```

---
## \#21 Posted by: legend27 Posted at: 2018-04-23T18:12:14.939Z Reads: 542

```
**UPDATE #1**

I decided to go for a single drive instead with some higher quality parts. I still need to find some parts but here is the updated part list:
_**The board:**_

- **1x $40** - Deck & griptape: 9 plies of canadian maple with darkwalnut finish from Skateshred.com (https://www.skateshred.com/wholesale-blank-longboard-decks/downhill-kicktail-dark-walnut-deck.html)
- **1x $70** - Enclosure: Knuckles enclosure from @psychotiller (https://psychotiller.com/product/knuckles) 
- **1x $200** - Wheels, trucks, bearings, risers, mounting hardware, motor mount, pully, belt and drive wheel pully: Kit from @torqueboards (collections/single-motor-mechanical-kit/products/single-motor-mechanical-kit)
- 

_**Electronics:**_

- **1x $100** - Vesc from @torqueboards (collections/esc-speed-controller/products/torque-esc-bldc-electronic-speed-controller)
- **1x $120** - 6347 190KV Motor from @torqueboards (collections/electric-skateboard-motors/products/electric-skateboard-motor-6374-190kv)
- **1x $60** - Remote and receiver from @torqueboards (collections/remote-controller/products/torqueboards-2-4ghz-nano-remote-controller)
- **1x $45** - On/off switch from @fottaz (https://eskating.eu/product/anti-spark-power-switch/)

_**Battery:**_ 

- **65x $300** - Samsung 30q batteris from eu.nkon.nl (https://eu.nkon.nl/samsung-inr-18650-30q-3000mah.html)
- **2x $8** - 1 meter 0.10x0.15cm Nickel strip from eu.nkon.nl (https://eu.nkon.nl/nikkel-battijersoldeerstrip-10mm.html)
- **3x $10** - XT90 male and female connecter from @fottaz (https://eskating.eu/product/black-nylon-xt90-connectors/)
- **1x $5** - Charging port from @fottaz (https://eskating.eu/product/dc-in-battery-2-1mm-socket-with-dust-cover/)
- **2x $8** - 223mm heatshrink for the battery from @fottaz (https://eskating.eu/product/heat-shrink-for-esk8-lithium-battery-packs-1m-various-size-tailored/)
- **1x $10** - Battery indicator from @fottaz (https://eskating.eu/product/battery-percentage-lcd-display/)  
- **2x $4** - Insulation paper for the batteries from eu.nkon.nl (https://eu.nkon.nl/isolatie-papier-18650.html)
- **20x $15** - Random sizes of heat shrink for wires from @fottaz (https://eskating.eu/product/heat-shrink-tubing-10cm-4-various-size-tailored/) 
- **1x $30** - 42V Charger from @fottaz (https://eskating.eu/product/2-amp-charger-10-and-12-s/) 

_**Car battery spot welder:**_

_**Extra:**_

- **1x $5** - Waterproofing the battery case ish from @fottaz (https://eskating.eu/product/soft-black-gasket-for-enclosures-perimeters-1m-tailored/)
- **3x $4** - Velcro from @fottaz (https://eskating.eu/product/peel-n-stick-polyester-velcro-10cm4/) 
- **2x $12** - 20 units (2m) of black and red 12 AWG wire (https://eskating.eu/product/10-12-awg-silicone-wires-in-black-red-10cm-various-size-tailored/)
- **1x $9** - T-Tool from @torqueboards (collections/accessories/products/skateboard-t-tool-blue)
- **1x $8** - Metric hex tool from @torqueboards (collections/tools/products/metric-hex-folding-tool)
- **1x $7** - Sensor wires from @torqueboards (products/vesc-sensor-wires)
- **1x $2** - Male to male servo connector from @torqueboards (products/male-to-male-servo-connector)   

**_TOTAL:_** $1072 excl. shipping
-

Parts i still need to find:
- Foam pad for the battery
- BMS
- Parts for spot welder

I expect to pay $150 for shipping and $200 for the rest of the parts which will give me a total of:
$1422
-

I might downgrade some of my parts or find other solutions since its $400 more than i expected it to be.
```

---
## \#22 Posted by: legend27 Posted at: 2018-05-02T15:16:27.246Z Reads: 461

```
**UPDATE #2**

Hi everyone!
Thanks for all the help. I just bought the Royce Pro deck from BustinBoards.com. I got it for $105 including shipping. You can save 50% on the boards on this site (https://bustinboards.com/collections/bustin-factory-store-page) if you use the code: **Factorystore** at checkout.
And thanks @treenutter for recommending me to upgrade the deck :slight_smile:

edit: And thanks to @Adam0311 for posting the code on the forum!
```

---
## \#23 Posted by: legend27 Posted at: 2018-05-04T18:45:14.366Z Reads: 460

```
 **UPDATE #3**
-

Found all the parts for the spot welder and just some tools. Here are the parts:

**Spot welder:**
* **1x $9** - [Copper lugs](https://www.amazon.de/sourcingmap%C2%AE-Steckverbinder-Kabelschuhe-l%C3%A4uten-Durchreise/dp/B00843V5KE/ref=sr_1_1?s=diy&ie=UTF8&qid=1525458089&sr=1-1&keywords=cable+lugs+200a) from Amazon.de
* **2x $14** - [Copper cable](https://www.amazon.de/Schwei%C3%9Fkabel-Massekabel-Meterware-Ummantelung-hochwertiges/dp/B01GBQNQLQ/ref=sr_1_4?ie=UTF8&qid=1525458003&sr=8-4&keywords=welding%2Bcable&th=1) from Amazon.de
* **1x $10** - [Solenoid relay](https://www.amazon.de/MagiDeal-Anlasserrelais-Magnetschalter-Roller-Motorrad/dp/B01M35CE1S/ref=sr_1_1?s=automotive&ie=UTF8&qid=1525457034&sr=1-1&keywords=solenoid+relay+250cc) from Amazon.de
* **1x $8** - [On/off switch](https://www.amazon.de/FANGXIN-Klingeltaster-Drucktaster-Hupenknopf-Klingelknopf/dp/B01MY6T06H/ref=sr_1_4?ie=UTF8&qid=1525457353&sr=8-4&keywords=momentary+switch&dpID=41OvXy4GKRL&preST=_SY300_QL70_&dpSrc=srch) from Amazon.de
* **1x $7** - [Choc block](https://www.amazon.de/Dual-Row-Postions-Schraube-Terminal-Block-Streifen/dp/B00KLOU56E/ref=sr_1_fkmr0_3?ie=UTF8&qid=1525457755&sr=8-3-fkmr0&keywords=choc+block+60a) from Amazon.de
* **1x $15** - [Copper nails](https://www.amazon.de/Kupfer-Baum-Stumpf-Killer-Gro%C3%9Fe/dp/B01MUY26KX/ref=sr_1_1?s=diy&ie=UTF8&qid=1525457876&sr=1-1&keywords=copper+nails&dpID=51e90g7VGUL&preST=_SX300_QL70_&dpSrc=srch) from Amazon.de

**Battery:**
* **1x $3** - [Electrical tape](https://www.amazon.de/Tesa-Isolierband-schwarz-1-Rolle/dp/B004SQLWH2/ref=sr_1_1?ie=UTF8&qid=1525458255&sr=8-1&keywords=electrical+tape) from Amazon.de
* **1x $9** - [Heat resistant tape](https://www.amazon.de/Tinksky-Temperaturen-Hitzebest%C3%A4ndig-Polyimid-Klebeband/dp/B00OZ5FL0K/ref=sr_1_1?ie=UTF8&qid=1525458298&sr=8-1&keywords=heat+resistant+tape) from Amazon.de

**Tools:**
* **1x $9** - [Titanium scissor](https://www.amazon.de/Westcott-30450-Titanium-Softgrip-grau-gelb/dp/B002N1WYBM/ref=sr_1_3?ie=UTF8&qid=1525458519&sr=8-3&keywords=titanium+scissors) from Amazon.de

**Extra:**
* **1x $9** - [Glue for glue gun](https://www.amazon.de/Hankering-Heisskleber-Klebesticks-100mm-F%C3%BCr-Hei%C3%9Fklebe-Pistolen/dp/B074N8L7YP/ref=sr_1_4?ie=UTF8&qid=1525458325&sr=8-4&keywords=hot+glue) from Amazon.de

**TOTAL: $93 excl. shipping (GRAND TOTAL: $1165 excl. shipping)**
-

I still need to find a BMS and some foam pads for the battery
```

---
## \#24 Posted by: legend27 Posted at: 2018-05-05T14:23:40.007Z Reads: 423

```
**UPDATE #4**    
-

Orded all the parts i posted yesterday today. I payed $91.68 in total incl. shipping.

@gee I spent $64.36 on the spot welder incl. shipping and didn't have to buy a battery since i already have one :)

**TOTAL SPENT: $196.68**
-

The only things i haven't found yet is a BMS and money lol.
```

---
## \#25 Posted by: moon Posted at: 2018-05-05T19:04:24.175Z Reads: 401

```
I am basically making the same spotwelder

What spec battery is yours?
```

---
## \#27 Posted by: legend27 Posted at: 2018-05-05T19:18:50.252Z Reads: 403

```
Can’t find the battery right now but im pretty sure its a 12v 8ah 220a :slight_smile: I will update you when I find it.
```

---
## \#28 Posted by: legend27 Posted at: 2018-05-06T01:10:07.413Z Reads: 422

```
**UPDATE #5**
-
already? shit


After some research have i finally found a BMS. Im going to buy this BMS (http://www.batterysupports.com/36v-37v-42v-10s-100a-10x-36v-lithium-ion-lipolymer-battery-bms-p-390.html) from SuPower. Sadly there isn't enough space for the BMS in the Knuckles enclosure from @psychotiller so i might have to buy this (https://street-wing.com/product/fibreglass-enclosure-landyachtz-nine-two-five/) or this (https://street-wing.com/product/fibreglass-supermodel-enclosure/) enclosure from @DavidBanner if i can't find a solution.

I expect to receive the deck in a few days so i can do some measuring to know which enclosure will fit on the board.

I am also going to get this remote instead of the one from  (https://buildkitboards.com/products/mini-remote?variant=28691643845).

And thanks to all the help from the forum to make my board perfect :slight_smile:
```

---
## \#29 Posted by: psychotiller Posted at: 2018-05-06T01:56:21.757Z Reads: 370

```
Did you think about putting that bms on top of the battery?
```

---
## \#30 Posted by: legend27 Posted at: 2018-05-06T02:13:13.336Z Reads: 368

```
Yes but thanks :) The BMS is 20mm tall and the battery pack is at least 38mm which makes it 58mm tall and your enclosure is 40mm.
```

---
## \#31 Posted by: psychotiller Posted at: 2018-05-06T03:10:15.609Z Reads: 350

```
Should have got a smaller bms...
```

---
## \#32 Posted by: legend27 Posted at: 2018-05-06T07:18:14.200Z Reads: 356

```
I probably should but I don't know which one to get instead. Do you have any recommendations?
```

---
## \#33 Posted by: ARetardedPillow Posted at: 2018-05-06T07:30:38.679Z Reads: 363

```
Just a question, do you have a soldering iron, solder, bullet connectors, heatshrink, wires, assortments of nuts and bolts, connectors (xt), loctite, mulitmeter, etc

There are little things that people miss a lot of the time, most of it is cheap but buying it before may save you a lot of time and effort and also save money on "Expedited shipping"
```

---
## \#34 Posted by: legend27 Posted at: 2018-05-06T07:53:21.339Z Reads: 364

```
I don't have that many tools so i probably have to buy some when i start building. The only things you mentioned I don't have is bullet connectors, nuts, bolts and loctite. I plan on buying the nuts, bolts and loctite at a local hardware store but what am i supposed to use the bullet connectors for?
```

---
## \#35 Posted by: ARetardedPillow Posted at: 2018-05-06T07:59:13.205Z Reads: 363

```
The bullets come in handy when dealing with connecting individual wires, such as motor phase wires, the torque boards motor come with phase wires with bullets that match the vesc they sell so you would be fine. However is the phase wires are not long enough you may have to make extensions and such.

Many new builder start out with Sk3 motors with 4mm bullets and they use tb vescs which are 5.5mm bullets and get frustrated as shit when they don't fit and go batshit crazy waiting for bullets.
```

---
## \#36 Posted by: legend27 Posted at: 2018-05-06T14:15:58.978Z Reads: 386

```
**UPDATE #6**
-

I've changed some of my parts to save some money but not going down on quality. Here are my new parts:



* **1x $30** - [Remote](https://buildkitboards.com/products/mini-remote?variant=28691643845https://buildkitboards.com/products/mini-remote?variant=28691643845) from @JLabs 
* **1x $47** - [97mm wheels with bearings](https://buildkitboards.com/products/90mm-build-wheels?variant=5041515135006)s from @JLabs
* **1x $29** - [Motor mount](https://buildkitboards.com/products/motor-mount-1?variant=4993928953886) from @JLabs 
* **1x $90** - [6355 190kv motor](products/electric-skateboard-motor-6355-190kv?variant=712504606743) from @torqueboards
* **1x $4** - [Shockpads](products/longboard-shockpad-risers-3mm?variant=712549924887) from @torqueboards
* **1x $6** - [Deck hardware](products/1-5-deck-hardware-bolts?variant=712625487895) from @torqueboards  
* **1x $65** - [218mm caliber trucks](products/torqueboards-218mm-trucks?variant=712802992151) from @torqueboards
* **1x $8** - [Extra belt](products/265mm-htd5-12mm-belt?variant=712496807959) from @torqueboards
* **1x $47** - [Pulley kit](products/36t-abec-pulley-combo-kit?variant=1263681896471) from @torqueboards
* **1x $4** - [Spacers](products/bearing-spacers?variant=712270020631) from @torqueboards

**TOTAL: $330**
**MONEY SAVED: $110 :+1:** 
-
```

---
## \#37 Posted by: Ebisane9 Posted at: 2018-05-06T14:19:16.935Z Reads: 386

```
If you want to save even more money, get belts from vbeltsupply. Buy in bulk if you know it's the right length, then buy some more if you ever plan on changing gearing.
```

---
## \#38 Posted by: psychotiller Posted at: 2018-05-06T14:28:14.595Z Reads: 417

```
Bestech D140 Charge only - 10S BMS is really thin.

![2a69b08faf071946a249ddf6b079f9e1a659f525_1_491x499|491x499](upload://4bT6pfKt3tJucydegqJ38YTxYu8.jpg)
```

---
## \#40 Posted by: legend27 Posted at: 2018-05-06T14:54:26.866Z Reads: 407

```
What are the pros and cons of having a charge only BMS instead of a normal BMS?
```

---
## \#41 Posted by: psychotiller Posted at: 2018-05-06T14:56:29.044Z Reads: 390

```
Pros are you wont hit amp cutouts all the time. They take up a lot less room,
Cons are you will need a Mosfet switch.
```

---
## \#42 Posted by: legend27 Posted at: 2018-05-06T14:59:11.850Z Reads: 375

```
Is a mosfet switch an on/off button?
```

---
## \#43 Posted by: psychotiller Posted at: 2018-05-06T15:03:48.743Z Reads: 345

```
It's a pcb with mosfets on it. A rocker switch comes with them. 

I'm out right now, but will have a bunch in a week or so.
```

---
## \#44 Posted by: legend27 Posted at: 2018-05-06T15:06:24.205Z Reads: 337

```
Does a charge only BMS protect the battery from getting too low on power?
```

---
## \#45 Posted by: psychotiller Posted at: 2018-05-06T15:28:54.532Z Reads: 334

```
Your vesc's do that.
```

---
## \#46 Posted by: legend27 Posted at: 2018-05-06T15:33:34.826Z Reads: 323

```
@psychotiller The VESC monitors the whole pack and the BMS monitors each cell. So if one cell gets to low the whole battery pack is destroyed?
```

---
## \#47 Posted by: psychotiller Posted at: 2018-05-06T15:41:50.395Z Reads: 338

```
The bms monitors cell groups. Not individual cells, Same as the vesc. 

The low voltage cutoff in your vesc monitors voltage sag, If any cell forces your pack voltage below the cutoff the vesc shuts down. 

Hate to say it, but I've seen and read about more battery failures using charge/discharge bms's than packs running with no bms. 

I've also been doing alot of battery repairs lately for people with dead cells. all of those packs had charge/discharge bms's. 

Don't lay too much trust in a bms. You need to watch your percentage display, periodically check your cell balance levels, and make sure you turn your board off when you're not riding it.
```

---
## \#48 Posted by: legend27 Posted at: 2018-05-06T15:50:55.409Z Reads: 378

```
@psychotiller Okay. Thanks for the help. I think im going to buy a charge only BMS instead ([this bms](http://www.esk8life.com/bestech-d140-10s)) to save some money and space. But how am i going to connect the battery to the VESC? Number 1 or number 2?
![Screenshot_11|590x500](upload://b934OJfi6POYfelaOxfkH38LqSs.jpg)
![Screenshot_12|568x500](upload://jZosVYs4UauvL5yCt2gEqoi1kwI.png)
```

---
## \#49 Posted by: psychotiller Posted at: 2018-05-06T15:58:01.889Z Reads: 340

```
Your main Positive and Negative wires (10 or 12awg) go straight to an xt90. which you will plug into your vescs.

The bms is wired to the battery. It's only connection other than to the battery, is to the charge port.
```

---
## \#50 Posted by: ARetardedPillow Posted at: 2018-05-06T17:37:35.957Z Reads: 332

```
If you want to save a couple bucks on mounting hardware go to your local hardware store and get 10-32 nuts and bolts. This is for mounting the truck.
```

---
## \#51 Posted by: legend27 Posted at: 2018-05-06T18:20:51.193Z Reads: 339

```
**UPDATE #7**
-

I orded the [bms](http://www.esk8life.com/bestech-d140-10s) and [remote](http://www.esk8life.com/24ghz-mini-remote-controller) today. I payed $54.06 in total incl. shipping. Much less than I expected :slight_smile: 
I plan on ordering the trucks, wheeels, pulley, motor and vesc when I get my current board sold.

**TOTAL SPENT: $250.74**
-

Still waiting for the deck and spot welder parts to arrive. I will post some pictures when they arrive :slight_smile:
```

---
## \#52 Posted by: moon Posted at: 2018-05-06T18:27:59.435Z Reads: 326

```
Think you need 255mm belt
```

---
## \#53 Posted by: legend27 Posted at: 2018-05-06T18:47:26.573Z Reads: 326

```
hmmm.... I might buy 1 of each to make sure 1 of them will work. Thanks didn't think of that before :slight_smile:
```

---
## \#54 Posted by: legend27 Posted at: 2018-05-06T18:53:34.074Z Reads: 337

```
New sketch of the enclosure with everything in it.
![Screenshot_13|690x250](upload://6VZPjJol6O4hzp6Q9q864be4pxj.png)
![Screenshot_14|690x76](upload://fLB058fYptpwOxYPK3XFCAws3ZM.png)
```

---
## \#55 Posted by: moon Posted at: 2018-05-06T18:56:34.355Z Reads: 316

```
No problem

Want to pm me? I have a spare one I could sell;)
```

---
## \#56 Posted by: legend27 Posted at: 2018-05-06T18:57:35.767Z Reads: 310

```
I'll think about it :) Thanks
```

---
## \#57 Posted by: mmaner Posted at: 2018-05-07T01:59:48.481Z Reads: 341

```
[quote="psychotiller, post:47, topic:53111"]
I’ve also been doing alot of battery reapirs lately for people with dead cells. all of those packs had charge/discharge bms’s.

Don’t lay too much trust in a bms. You need to watch your percentage display, periodically check your cell balance levels, and make sure you turn your board off when you’re not riding it.
[/quote]

PREACH! 🤘
```

---
## \#58 Posted by: legend27 Posted at: 2018-05-09T15:02:08.236Z Reads: 374

```
**UPDATE #8**
-

I received the deck today and its awesome. PLUS it came with mounting hardware and risers FOR FREE!
![IMG_2764|666x500](upload://ctKDwD6g5p9X17pvhyQHnYQESYH.JPG)
![IMG_2765|666x500](upload://uN6M7wI5fD5a7GMAxRVprQgrJSg.JPG)
![IMG_2766|666x500](upload://rNTW2m6EWmKFYFRZNMNWdZW1xvB.JPG)


I also orded some [90mm 78a wheels](https://buildkitboards.com/products/90mm-build-wheels?variant=5041515102238), [motor mount](https://buildkitboards.com/products/motor-mount-1) and [screws to mount the motor](https://buildkitboards.com/products/m4x10-motor-mounting-bolts) from @JLabs. I payed $103.32 in total incl. shipping. Shipping was $33.39 but still cheaper than other places :slight_smile: 

**TOTAL SPENT: $354.06**
-
```

---
## \#59 Posted by: JLabs Posted at: 2018-05-09T15:14:44.586Z Reads: 353

```
Thanks for the support man! I will get them out tomorrow for you :slight_smile:
```

---
## \#60 Posted by: legend27 Posted at: 2018-05-09T17:41:17.094Z Reads: 352

```
**UPDATE #9**
-

Changing the [enclosure](https://psychotiller.com/product/knuckles) to [this one](https://eskating.eu/product/abs-enclosure-38x165x530mm/) from @fottaz to save some money on shipping.

**TOTAL: $82.93**
**MONEY SAVED: $23.07 :+1:**
-
```

---
## \#61 Posted by: Haimindo Posted at: 2018-05-09T18:17:07.586Z Reads: 344

```
Looking good! I have ordered the same deck. What is the length of the mountable area between the wheel wells?
```

---
## \#62 Posted by: legend27 Posted at: 2018-05-09T20:23:52.402Z Reads: 341

```
I will be able to tell you the exact lenght on monday but its about 10 cm :slight_smile:
```

---
## \#63 Posted by: legend27 Posted at: 2018-05-09T22:15:45.698Z Reads: 333

```
**UPDATE #10**
-
I still need to order parts for a total of $888 incl. shipping to finish the build. This will make the total:

**$1238.80 incl. shipping**
-

**THATS $183.2 LESS THAN I EXPECTED IN THE BEGINING! :+1:**

Looking forward to finish the build :slight_smile:
```

---
## \#64 Posted by: legend27 Posted at: 2018-05-10T13:24:59.873Z Reads: 335

```
**UPDATE #11**
-

Orded a lot of parts today. I payed $331.93 in total incl. shipping. I saved $40 on shipping THANKS @torqueboards

The parts i orded were: [vesc](products/torque-esc-bldc-electronic-speed-controller)**,** [skate tool](products/skateboard-t-tool-blue)**,** [metric hex folding tool](products/metric-hex-folding-tool)**,** [6355 190kv motor](products/electric-skateboard-motor-6355-190kv)**,** [218mm trucks](products/torqueboards-218mm-trucks)**,** [pulley kit](products/36t-abec-pulley-combo-kit)**,** [bearing spacers](products/bearing-spacers)**,** [servo connector](products/male-to-male-servo-connector) **and** [sensor wires](products/vesc-sensor-wires).

**TOTAL SPENT: $685.99**
-

I expect to be able to order the rest of parts in the begining of July.
```

---
## \#65 Posted by: Ebisane9 Posted at: 2018-05-10T16:22:06.896Z Reads: 312

```
You're running a single 6355? You might be starved for power. Actually you WILL be starved for power. How heavy are you? what's the terrain like?
```

---
## \#66 Posted by: legend27 Posted at: 2018-05-10T16:35:27.216Z Reads: 308

```
Haha. I don't wanna kill myself lol. I'm 14 years old so "live wild, die young" is not my slogan. I'm 132 pounds (60 kg) and I live in Denmark. Its really hard to find hills in Denmark and the steepest hill I know is probably 30%.
```

---
## \#67 Posted by: mmaner Posted at: 2018-05-10T16:43:35.644Z Reads: 302

```
At 132 a single 6355 is fine.  I'm just shy of 200 and I've ridden single 6355's for mile and miles and miles.  Those little guys will do a lot more than you think.
```

---
## \#68 Posted by: legend27 Posted at: 2018-05-10T16:48:14.840Z Reads: 295

```
I've gone 20mph on my current electric skateboard (Huger Tech Travel) and that's fast. Anything over 25 mph is probably too fast in my opinion.
```

---
## \#69 Posted by: Ebisane9 Posted at: 2018-05-10T16:52:41.559Z Reads: 303

```
must be the power-whore in me lmao. I had so little power before and now i crave all the power. @legend27 if @mmaner says it works, it does. He knows a lot :D

Edit: nice project for 14 btw. It's an excellent opportunity to learn a lot. wish i had this exposure when  was 14 tbh!
```

---
## \#70 Posted by: mmaner Posted at: 2018-05-10T16:57:18.613Z Reads: 311

```
people assume that a 6355 is not enough, in reality the only thing that suffers is the low end torque.  Top speed is only about 5% less with a single, but low end torque is about 60% with a single.  A 6374 delivers more torque in a single motor build but it uses more amps.  

A single is typically more efficient than a dual but delivers a lot less low end torque.
```

---
## \#71 Posted by: legend27 Posted at: 2018-05-10T17:13:41.703Z Reads: 301

```
**QUESTION #1**
-
How many amps should i set the fuse to on my [anti spark power switch](https://eskating.eu/product/anti-spark-power-switch/)?
```

---
## \#72 Posted by: mmaner Posted at: 2018-05-10T17:45:09.875Z Reads: 311

```
It depends on your max amps, if you have a max of 60 amps then use a 70 or 80 amp fuse.  I don't use a fuse at all as I'd rather have a dead switch than loose power going 30mph.
```

---
## \#73 Posted by: legend27 Posted at: 2018-05-10T17:49:56.937Z Reads: 331

```
Can i set the max amps in the VESC settings? And why is it posible to lose power going 30mph?
![Screenshot_11|690x482](upload://1oX9ugyT848JbnBIZIbZZb7bzcR.png)
```

---
## \#74 Posted by: mmaner Posted at: 2018-05-10T17:52:52.840Z Reads: 300

```
Yeah, that's the only place to set the max amps but remember it's doubled if your running dual motors.  You can lose power if the fuse blows...and it aint no fun :slight_smile:.
```

---
## \#75 Posted by: legend27 Posted at: 2018-05-10T17:57:02.107Z Reads: 304

```
So i can use a 70 amp fuse anti spark switch in case i want more power and set the max amps to 40 without any problems?
```

---
## \#76 Posted by: mmaner Posted at: 2018-05-10T18:18:21.560Z Reads: 304

```
NOOOOOOOO.  If you have dual motors/dual vescs and you have your MAX battery amps set at 35a, the minimum fuse value is 70, I would go to at least 80.  The fuse value needs to be higher than what your cumulative battery max is.
```

---
## \#77 Posted by: legend27 Posted at: 2018-05-10T18:58:13.360Z Reads: 290

```
So it dosen't matter if i use 100 or 40 amp fuse for 30 max battery amp?
```

---
## \#78 Posted by: mmaner Posted at: 2018-05-10T19:16:23.001Z Reads: 307

```
I seem to have lost you somewhere.  The fuse value needs to be higher than what your cumulative battery max is, at least 10% higher.

This means if you have x2 VESC's and the battery max on each is 30a, you have a cumulative battery max of 60a.  10% of 60a is 6a, so 60 + 6 rounded up is 70a.  So you need at least a 70a fuse

If you have x1 VESC and you battery max is 60a, its the same thing...70a fuse.  But if you battery max is 50, then 10% of 50 is 5, so 50 + 5 rounded up is 60a.  In this case you need at least a 60a fuse.

If you need at least a 70a fuse and use a 140a fuse, why use a fuse at all as you will never reach 140a if you battery max is set to a cumulative 60a.  You just want the fuse to be higher than the cumulative amps so that if something breaks on the battery side the fuse disconnects the current and hopefully saves your VESC's.

I, personally, would rather loose a VESC than all my teeth, and that is a distinct possibility if you loose all throttle (acceleration & brakes) at 30mph.
```

---
## \#79 Posted by: legend27 Posted at: 2018-05-10T19:23:41.190Z Reads: 285

```
Okay, thanks! I'm going to buy it with 60 amps fuse :slight_smile:
```

---
## \#80 Posted by: pixelsilva Posted at: 2018-05-10T20:22:41.679Z Reads: 281

```
...if you are setting 50 max battery amps.
```

---
## \#81 Posted by: legend27 Posted at: 2018-05-10T20:26:17.151Z Reads: 284

```
Im probably going to set it to 40 but i wanna be able to set it to 50 if i want some more power.
```

---
## \#82 Posted by: pixelsilva Posted at: 2018-05-10T20:27:57.625Z Reads: 289

```
Like all you detailed shopping list. Very valuable. :ok_hand:
```

---
## \#83 Posted by: legend27 Posted at: 2018-05-10T21:06:58.799Z Reads: 258

```
**QUESTION #2**
-

What wire should i use to connect the charing port to the battery?

Is 10 AWG wire strong enough to be used for connecting the battery to the vesc?
```

---
## \#84 Posted by: legend27 Posted at: 2018-05-10T23:08:54.592Z Reads: 269

```
**UPDATE #12**
-
Had to pay $8 more for shipping to Denmark since it wasn't calculated right. 

**TOTAL: $693.99**
-
```

---
## \#85 Posted by: ARetardedPillow Posted at: 2018-05-11T07:32:01.505Z Reads: 280

```
I would use 16 or 18 awg wire for the charge port, and 10awg wire Is great for connecting the batteries to the Vesc.

Your thread is so organized and you have everything documented. Thats awesome! Looking forward to your build.
```

---
## \#86 Posted by: legend27 Posted at: 2018-05-11T12:11:13.699Z Reads: 309

```
**UPDATE #13**
-
I've changed some of the parts to get more quanity. Its $53.5 more expensive but i will be able to make more battery packs in the future :+1:

**PARTS REMOVED:**
* **1.8 meter of each color $15** - [10 AWG wire](https://eskating.eu/product/10-12-awg-silicone-wires-in-black-red-10cm-various-size-tailored/) from Eskating.eu
* **Randon sizes $5** - [Heat shrink tubing](https://eskating.eu/product/heat-shrink-tubing-10cm-4-various-size-tailored/) from Eskating.eu
* **10 pack $13** - [Bolts to mount enclosure](https://eskating.eu/product/m4-bolts-for-enclosures-kit-of-6-pairs/) from Eskating.eu
* **0.5 meter $5** - [Velcro](https://eskating.eu/product/peel-n-stick-polyester-velcro-10cm4/) from Eskating.eu
* **2x female & 2x male $6** - [XT90 connector](https://eskating.eu/product/black-nylon-xt90-connectors/) from Eskating.eu

**TOTAL: $44 incl. shipping**
-

_-----------------------------------------------------------------------------------------------------------------------------------------------_

**NEW PARTS:**
* **1.5 meter of each color $13** - [AWG 10 wire](https://www.amazon.de/gp/product/B007DMW3IU/ref=ox_sc_act_title_10?smid=A16S8DGX6Q6F4I&psc=1) from Amazon.de (lol didn't save anything :frowning:) 
* **2.1 meter of each color $9** - [AWG 16 wire](https://www.amazon.de/gp/product/B07427NFJM/ref=ox_sc_act_title_9?smid=A16S8DGX6Q6F4I&psc=1) from Amazon.de
* **50pcs $5** - [Insert nut for M4 bolts](https://www.amazon.de/gp/product/B01MQIL9Q3/ref=ox_sc_act_title_8?smid=AQ1IBDB6G2RRD&psc=1) from Amazon.de
* **258 pieces $7.5** - [Random bolts incl. M4 bolts](https://www.amazon.de/gp/product/B00B22V8NI/ref=ox_sc_act_title_7?smid=A3JWKAKR8XB7XF&psc=1) from Amazon.de
* **560 pieces $11** - [Heat shrink tubing](https://www.amazon.de/gp/product/B071D7LJ31/ref=ox_sc_act_title_6?smid=A1BJ0HTATZOCK&psc=1) from Amazon.de
* **500 pieces $6.5** - [Random size washers](https://www.amazon.de/gp/product/B00B22VHOS/ref=ox_sc_act_title_5?smid=A3JWKAKR8XB7XF&psc=1) from Amazon.de
* **10 pieces 30cm*20cm $4.5** - [Foam sheets](https://www.amazon.de/gp/product/B00G28NL14/ref=ox_sc_act_title_4?smid=A3JWKAKR8XB7XF&psc=1) from Amazon.de
- **10x female & 10x male $13** - [5.5mm gold connectors](https://www.amazon.de/gp/product/B00NVMO1AY/ref=ox_sc_act_title_3?smid=A2I7JN4QZXZWJI&psc=1) from Amazon.de 
* **5x female & 5x male $15** - [XT90 connectors](https://www.amazon.de/gp/product/B00ON34RX6/ref=ox_sc_act_title_2?smid=A2I7JN4QZXZWJI&psc=1) from Amazon.de
* **10cm*1m $13** - [Velcro](https://www.amazon.de/gp/product/B01BY9Y15U/ref=ox_sc_act_title_1?smid=A33UO8CI5VEXSZ&psc=1) from Amazon.de

**TOTAL: $97.5 incl. shipping**
-

_-----------------------------------------------------------------------------------------------------------------------------------------------_

**NEW TOTAL: $1312.48 incl. shipping**
PARTS REMAINING: $630 incl. shipping
-

That's $110 less than I expected in the beginning.
```

---
## \#87 Posted by: sk8l8r Posted at: 2018-05-11T13:07:54.759Z Reads: 278

```
really like the detailed list of parts and costs really good for reference!
```

---
## \#88 Posted by: a67676767 Posted at: 2018-05-11T18:25:19.784Z Reads: 278

```
Thanks for detailing everything and the links .. helps me with ideas for mine.
```

---
## \#89 Posted by: legend27 Posted at: 2018-05-11T20:28:59.323Z Reads: 274

```
I'm glad you appreciate it. I was thinking that i maybe posted to many posts lol.
```

---
## \#90 Posted by: legend27 Posted at: 2018-05-11T20:34:28.529Z Reads: 281

```
Im glad you appreciate the costs. I wish some more people started to post the price of each item, so new people would get a good idea of the cost of building an electric skateboard and would take it into consideration as an alternative vehicle.
```

---
## \#91 Posted by: legend27 Posted at: 2018-05-11T20:37:47.103Z Reads: 261

```
I'm glad it helps you find inspiration :) When do you expect to start building your board?
```

---
## \#92 Posted by: legend27 Posted at: 2018-05-11T20:40:40.718Z Reads: 263

```
**OFF TOPIC UPDATE #1**
-

A guy has offered me $272 for my [Huger Tech Travel Board](https://www.indiegogo.com/projects/huger-powerful-affordable-electric-skateboards#/). I hope to get $320 for it but what do you think of the price? Should I sell it to him for that price?
```

---
## \#93 Posted by: a67676767 Posted at: 2018-05-11T21:06:55.837Z Reads: 256

```
I have 3 DIYeboard.com kits ordered .. one for me, one for my son, and one for my neighbor.  I think they will be here in about 2 weeks.  Looking at all the true builds that people are doing for what I'm sure will be my next build after that :slight_smile:
```

---
## \#94 Posted by: legend27 Posted at: 2018-05-11T21:22:39.038Z Reads: 251

```
Do you know what deck you are going to use?
```

---
## \#95 Posted by: legend27 Posted at: 2018-05-11T22:10:07.975Z Reads: 268

```
**UPDATE #14**
-
I need a mini usb cable for connecting the VESC to my computer.
- **1x $3** - [Mini USB cable](https://www.amazon.de/Mini-Kabel-Stecker-Mini-USB-B-Stecker-Schwarz/dp/B001M1L1NQ/ref=sr_1_4?ie=UTF8&qid=1526076371&sr=8-4&keywords=mini+usb+kabel) from Amazon.de

**NEW TOTAL: $1315.48**
-
```

---
## \#96 Posted by: legend27 Posted at: 2018-05-11T22:32:11.270Z Reads: 274

```
**QUESTION #3**  
-
Whats the max I can set my "Battery Current Max" in my VESC? My battery is going to be a 10S6P Samsung 30Q. I think the max I can set it to is 90 amps but is that correct?
```

---
## \#97 Posted by: Ebisane9 Posted at: 2018-05-11T22:34:06.546Z Reads: 271

```
you can set 60A per vesc, if your vesc can handle it? theoretically it should have a max continuous of 120A. Doubt you'd pull that much from the battery unless youre doing some crazy shit. I have a 4p and have 35 per vesc on the TB vesc. i could go 40 but i personally don't, if i had a focbox or vesc6 i would though...
```

---
## \#98 Posted by: legend27 Posted at: 2018-05-11T22:36:37.626Z Reads: 277

```
Im only going to use 1 motor and vesc. I want to get a lot of range so 25-40 amps is probably good enough for me. Thanks for your time and help!
```

---
## \#99 Posted by: legend27 Posted at: 2018-05-12T19:32:26.930Z Reads: 284

```
**UPDATE #15**
-
I need some [foam](https://www.amazon.de/Schaumstoffplatte-RG14-120cm-200cm-P035/dp/B00F8EWG3W/ref=sr_1_2?rps=1&ie=UTF8&qid=1526153152&sr=8-2&keywords=foam&refinements=p_76%3A419123031) to make sure the battery and vesc won't move around in the enclosure. THAT SHIT COSTS $16.5 HOLY FUCK!

**NEW TOTAL: $1331.98**
-
```

---
## \#100 Posted by: moon Posted at: 2018-05-12T19:53:28.613Z Reads: 294

```
Lol

It pays to order from Aliexpress and stock up
```

---
## \#101 Posted by: Eboosted Posted at: 2018-05-13T03:27:40.415Z Reads: 296

```
Don't focus on cost that much, enjoy the building process and get the best quality parts you can afford at the moment.

Building is one of my favorite parts of this hobby
```

---
## \#102 Posted by: a67676767 Posted at: 2018-05-13T05:57:56.198Z Reads: 320

```
I had planned to use a 43" longboard deck off of a long board I already have, but eyeing some others.  My neighbor is wanting to make some molds and build our own decks.  We may do that.  Here is the old board I had planned to use.  ![20180512_225033|281x500](upload://lHP5d2e96SgbjJnj6Qh4MXVlBDX.jpg)

![20180512_225025|281x500](upload://sNHohOxx0LtEso7YbvPrhbYkByw.jpg)

![20180512_225007|281x500](upload://qyCOAZZAyZowQFU2CNhYiAuaijK.jpg)
```

---
## \#103 Posted by: Westy Posted at: 2018-05-13T06:42:54.606Z Reads: 301

```
That Skateshred deck is actually a fairly nice deck. They're made by Ryan Ehlers from Ehlers Longboards. Granted I pretty much pulled a @whitepony on mine.  

![20180512_094448|374x500](upload://2yc34vJ3O2QbaXE3le7sYHeTMUM.jpg)
```

---
## \#104 Posted by: legend27 Posted at: 2018-05-13T08:07:49.220Z Reads: 303

```
@Haimindo, you asked about the mountable area. Now I have an exact answer:
![IMG_2769|375x500](upload://gxpqXwN3cLHB0TIinSahYNZcctu.jpg)
```

---
## \#105 Posted by: Haimindo Posted at: 2018-05-13T08:27:28.084Z Reads: 281

```
@legend27 nice, thanks a lot! 

So this enclosure would not fit, hmm hmm  https://eskating.eu/product/abs-enclosure-38x165x530mm/

Might have to get an adjustable two piece enclosure
```

---
## \#106 Posted by: legend27 Posted at: 2018-05-13T09:44:51.897Z Reads: 278

```
Im actually going to get this enclosure so hopefully lol. It will fit but there wil only be a 3 cm gap from the trucks to the enclosure.
```

---
## \#107 Posted by: Haimindo Posted at: 2018-05-13T09:48:12.866Z Reads: 274

```
Okay, keep me posted how it goes :sweat_smile:
```

---
## \#108 Posted by: legend27 Posted at: 2018-05-13T09:50:03.074Z Reads: 273

```
Sure! I'll do that!
```

---
## \#109 Posted by: legend27 Posted at: 2018-05-13T10:35:29.043Z Reads: 268

```
It won't actually fit :frowning: The outside dimensions of the enclosure are 57cm X 21.5cm. You have 50cm X 24cm to mount the enclosure :frowning:
```

---
## \#110 Posted by: legend27 Posted at: 2018-05-13T10:47:12.545Z Reads: 271

```
[This enclosure](https://eskating.eu/product/abs-enclosure-38x165x420mm/) will fit on the deck :slight_smile:
```

---
## \#111 Posted by: legend27 Posted at: 2018-05-13T19:00:40.961Z Reads: 289

```
**UPDATE #16**
-
Changed the [old enclosure](https://eskating.eu/product/abs-enclosure-38x165x530mm/) to [this one](https://eskating.eu/product/abs-enclosure-38x165x420mm/) also from @fottaz. Its almost the exact same the only difference is the lenght (The old one couldn't fit on the deck lol). I can still fit all the components in the new enclosure :slight_smile:  

**MONEY SAVED: $6 :+1:**
NEW TOTAL: $1325.98
-
```

---
## \#112 Posted by: legend27 Posted at: 2018-05-14T16:59:12.784Z Reads: 306

```
**UPDATE #17**
-
Received the [1 meter cobber cable](https://www.amazon.de/Schwei%C3%9Fkabel-Massekabel-Meterware-Ummantelung-hochwertiges/dp/B01GBQNQLQ/ref=sr_1_4?ie=UTF8&qid=1525458003&sr=8-4&keywords=welding%2Bcable&th=1) (not 2 meter as i wrote in Update 3), [electrical tape](https://www.amazon.de/Tesa-Isolierband-schwarz-1-Rolle/dp/B004SQLWH2/ref=sr_1_1?ie=UTF8&qid=1525458255&sr=8-1&keywords=electrical+tape), [heat resistant tape](https://www.amazon.de/Tinksky-Temperaturen-Hitzebest%C3%A4ndig-Polyimid-Klebeband/dp/B00OZ5FL0K/ref=sr_1_1?ie=UTF8&qid=1525458298&sr=8-1&keywords=heat+resistant+tape) and some [glue](https://www.amazon.de/Hankering-Heisskleber-Klebesticks-100mm-F%C3%BCr-Hei%C3%9Fklebe-Pistolen/dp/B074N8L7YP/ref=sr_1_4?ie=UTF8&qid=1525458325&sr=8-4&keywords=hot+glue) for my glue gun (pow pow)


![IMG_2770|666x500](upload://vGRieEuxNayxvWPqW1iPpjo8bGM.JPG)

![IMG_2771|666x500](upload://vZPcSoV4N3q7WrcRPtyfGz5oNjr.JPG)
```

---
## \#113 Posted by: FredrikHems Posted at: 2018-05-14T19:25:23.279Z Reads: 298

```
What is the cable for?
```

---
## \#114 Posted by: legend27 Posted at: 2018-05-15T12:39:16.588Z Reads: 302

```
 For making the car battery spot welder :slight_smile:

![Screenshot_15|539x500](upload://oNxFtBzaIhLGHXmepEsnlGa9fSo.jpg)
```

---
## \#115 Posted by: legend27 Posted at: 2018-05-15T13:24:35.083Z Reads: 299

```
**QUESTION #4**
-
Is it possible to limit the top speed in the vesc settings?

edit: solved
```

---
## \#116 Posted by: legend27 Posted at: 2018-05-16T14:47:33.370Z Reads: 297

```
**UPDATE FU*KING #17**
-
Received an import bill today... nice :rage:
I have to pay.. HOLD ON... $72.34 FOR THE FU**ING IMPORT OF A SKATEBOARD. $72!! THATS THE FUCKING PRICE OF THE BOARD! :rage:

I don't know when I will be able to order the rest of the parts (definitley not in July), but probably in August. When its almost winter again... :rage:

Hopefully i don't have to pay any fu*king import taxes again when i receive the 3 other packages from USA (im going to receive some more import tax bills. Calling it)

edit: I PAYED $30 FOR THE SHIPPING :rage:
```

---
## \#117 Posted by: moon Posted at: 2018-05-16T14:51:12.039Z Reads: 288

```
You should check the import tax laws in your country
```

---
## \#118 Posted by: legend27 Posted at: 2018-05-16T14:52:37.836Z Reads: 286

```
I already knew the import tax were insane in Denmark, but I have bought some other things from USA, without having to pay import taxes...
```

---
## \#119 Posted by: moon Posted at: 2018-05-16T14:53:28.968Z Reads: 284

```
Depends on the item value too

Some companies lie about this to save you some $
```

---
## \#120 Posted by: DeathCookies Posted at: 2018-05-16T14:54:58.893Z Reads: 287

```
[quote="moon, post:119, topic:53111"]
Some companies lie about this to save you some $
[/quote]
Mostly chinese companies because they dont care about laws. lol
```

---
## \#121 Posted by: moon Posted at: 2018-05-16T15:00:52.848Z Reads: 296

```
Very true they do like lying about it lol
```

---
## \#122 Posted by: legend27 Posted at: 2018-05-17T16:18:18.172Z Reads: 307

```
**UPDATE #18**
-
Received the [copper nails](https://www.amazon.de/Kupfer-Baum-Stumpf-Killer-Gro%C3%9Fe/dp/B01MUY26KX/ref=sr_1_1?s=diy&ie=UTF8&qid=1525457876&sr=1-1&keywords=copper+nails&dpID=51e90g7VGUL&preST=_SX300_QL70_&dpSrc=srch), [titanium scissor](https://www.amazon.de/Westcott-30450-Titanium-Softgrip-grau-gelb/dp/B002N1WYBM/ref=sr_1_3?ie=UTF8&qid=1525458519&sr=8-3&keywords=titanium+scissors) and [momentary switches](https://www.amazon.de/FANGXIN-Klingeltaster-Drucktaster-Hupenknopf-Klingelknopf/dp/B01MY6T06H/ref=sr_1_4?ie=UTF8&qid=1525457353&sr=8-4&keywords=momentary+switch&dpID=41OvXy4GKRL&preST=_SY300_QL70_&dpSrc=srch) today.

![IMG_2779|666x500](upload://cgHfC0RhOGKCvSPoSpFQvfrMZEh.JPG)
```

---
## \#123 Posted by: legend27 Posted at: 2018-05-19T12:43:21.897Z Reads: 303

```
**UPDATE #19**
-
Received the [BMS](http://www.esk8life.com/bestech-d140-10s) and [remote](http://www.esk8life.com/24ghz-mini-remote-controller). Haven't received the import tax bill yet lol.

![IMG_2785|666x500](upload://eXazTwbndKAEz8Gbdl6ZLwy0qvP.JPG)
```

---
## \#124 Posted by: legend27 Posted at: 2018-05-20T14:07:22.952Z Reads: 300

```
**UPDATE #20**
- 
Changed the [old enclosure](https://eskating.eu/product/abs-enclosure-38x165x420mm/) to [this one](https://pwrboards.com/products/pwr-case) from @OskarCastrone and ordered it :slight_smile: I payed $35 incl. shipping.

**TOTAL SAVED: $41 :+1:**
**TOTAL SPENT: $728.99**
**TOTAL SPENT INCL. TAXES: $801.33**
**NEW TOTAL: $1284.98**
**NEW TOTAL INCL. TAXES: $1357.32**
**PARTS REMAINGING: $560**
-
```

---
## \#125 Posted by: legend27 Posted at: 2018-05-20T19:16:36.240Z Reads: 290

```
**OFF TOPIC UPDATE #2**
-
Got my Huger Tech Travel board sold today! :grinning::+1::crazy_face::fireworks::sparkler::balloon::tada: He payed $268 in cold cash, so now im able to pay all the upcomming import bills! Thanks to the guy who bought it! You saved me!
```

---
## \#126 Posted by: legend27 Posted at: 2018-05-20T23:35:24.020Z Reads: 287

```
**UPDATE #21**
-
I found a pretty good name for my board today. "Bankrupt" is the name of my board. this is weird lol
```

---
## \#127 Posted by: GrecoMan Posted at: 2018-05-21T01:39:08.701Z Reads: 289

```
**esk8.builders**
*more addictive than crack since 1864*
```

---
## \#128 Posted by: legend27 Posted at: 2018-05-22T15:42:40.977Z Reads: 279

```
**OFF TOPIC UPDATE #3**
-
I made a video about the Huger Tech Travel Board. If any of you might be interested in buying the board, watch [this video](https://www.youtube.com/watch?v=XcDNeeehPfQ) before you do. Please don't buy the board.
```

---
## \#129 Posted by: legend27 Posted at: 2018-05-27T11:40:10.984Z Reads: 289

```
**UPDATE #22**
-
@gee

Decided to get a new battery for the spot welder. The old one was old and cheap. The [new battery](https://www.amazon.de/gp/product/B01N2ANL3F/ref=ox_sc_act_title_2?smid=A11WKGUFG1VZFJ&psc=1) im going to buy costs $46 and is from BulletBatt. This wil make the total cost of the spotwelder $100.36, which is still cheaper than a "plug and play" spot welder.

I also decided to get a [wire stripper](https://www.amazon.de/gp/product/B00CD24EAK/ref=ox_sc_act_title_5?smid=A3JWKAKR8XB7XF&psc=1) for $18, some other [velcro strips](https://www.amazon.de/gp/product/B0098LT9Z4/ref=ox_sc_act_title_3?smid=A2RCXAQDK3T42M&psc=1) for $5 and [2 brass clamps](https://www.amazon.de/gp/product/B002USHODG/ref=ox_sc_act_title_1?smid=A3JWKAKR8XB7XF&psc=1) for $7 (for the car battery)

**NEW TOTAL (will be incl. taxes from now on): $1433.32**
**PARTS REMANING: $636**
-
```

---
## \#130 Posted by: legend27 Posted at: 2018-05-28T14:20:38.445Z Reads: 307

```
**UPDATE #23**
-
Received the [enclosure](https://pwrboards.com/collections/enclosures/products/pwr-case) and [choc block](https://www.amazon.de/gp/product/B00KLOU56E/ref=oh_aui_detailpage_o04_s00?ie=UTF8&psc=1) today :slight_smile: I also got  some stickers, weird black glue? and sealing for the enclosure (isn't long enough).

![IMG_2811|666x500](upload://gaPozQ6pdpS0oNEpHBRUDcNvrxX.JPG)

![IMG_2799|666x500](upload://nHpRaB4OWIkIr3zYAc2sqdT9daD.JPG)

![IMG_2801|666x500](upload://9XZc3lCsGin5I24MdT0WUPmUGWt.JPG)

![IMG_2802|666x500](upload://r8CP8alYM9pM9Sj6OCm0EDerv9D.JPG)

![IMG_2812|666x500](upload://6oh3EvfXKpDXu7ExHSGTv9Oqx4c.JPG)

![IMG_2807|666x500](upload://ofzWJw3NhaGtd3CKFFJYuaNKRXT.JPG)

![IMG_2808|666x500](upload://liJcq5IxahnBeoRZ8ft8RHwJWVr.JPG)

![IMG_2809|666x500](upload://ntP4TXmbOaLdPWCQm77IbehtZFc.JPG)

![IMG_2803|666x500](upload://9AtrZmn3icDy7JrkVuHt3h6mO9v.JPG)

![IMG_2804|666x500](upload://qsdNmaPBMGwNrUgoEWjzMQmFWJO.JPG)
```

---
## \#131 Posted by: legend27 Posted at: 2018-05-28T16:52:36.661Z Reads: 288

```
**UPDATE #24**
-

I ran into a challenge (NOT PROBLEM!)... The enclosure isn't high enough to fit the battery pack. Any ideas on how to make it higher? I've seen one use some kind of plastic cardboard?

![Screenshot_17|690x206](upload://uv9Y0ZK8hrQgdHqsuxYLpq8wg2u.png)
```

---
## \#132 Posted by: dg798 Posted at: 2018-05-28T17:06:33.826Z Reads: 284

```
Maybe if u have a router route out part of ur deck to put the battery into kind of like a slot
```

---
## \#133 Posted by: Jc06505n Posted at: 2018-05-28T17:12:39.662Z Reads: 278

```
^ that plus a rubber grommet (hope I’m not getting I.T confused with a gasket) could also raise it, at most by half and inch.
```

---
## \#134 Posted by: rey8801 Posted at: 2018-05-28T17:21:48.246Z Reads: 273

```
It depends how much you need. I also had the same problem with my first enclosure (printed one, measured wrong :laughing: ). What I did was to use higher gasket or adhesive foam from both of the side, so sticked on the edges of the enclosure and on the board too. So you will get more room. Then it wasn't enough so I ended up by router out 5mm from the board. It depends on how tick is your board.
```

---
## \#135 Posted by: legend27 Posted at: 2018-05-28T17:43:58.375Z Reads: 267

```
I need it to be 1 cm higher. I could also take some plywood instead of the plastic cardboard? Have anyone tried doing that?
```

---
## \#136 Posted by: rey8801 Posted at: 2018-05-28T18:19:00.322Z Reads: 262

```
1 cm it's feasible just with the gasket. Like foam 3mm on the board and thick d shape gasket on the enclosure side.
```

---
## \#137 Posted by: legend27 Posted at: 2018-05-29T14:53:01.905Z Reads: 273

```
**UPDATE #25**
-
I payed another import bill today. $39 in total. I also found some [foam sheet](https://www.amazon.de/gp/product/B000OZL8ES/ref=ox_sc_act_title_2?smid=A3JWKAKR8XB7XF&psc=1) and [rubber gasket](https://www.amazon.de/gp/product/B016Q1BRKI/ref=ox_sc_act_title_1?smid=A3INC0B8PQWEWS&psc=1) which should make the enclosure 1cm higher.

**TOTAL: $1451.32**
**TOTAL FOR THE BOARD (no tools or extras): $866 excl.**
**shipping and taxes**
**TOTAL SPENT: $840.33**
-

edit: forgot to include the deck in the price for the board.
```

---
## \#138 Posted by: legend27 Posted at: 2018-05-30T12:19:19.925Z Reads: 285

```
**UPDATE #26**
-
Payed the last import taxes today for the parts from ! $113, quite expensive but whatever.

**TOTAL IMPORT TAXES: $224 holy**

I btw. also received the [90mm wheels and bearings](https://buildkitboards.com/collections/wheels/products/90mm-build-wheels?variant=5041475551262), [motor mount](https://buildkitboards.com/collections/parts/products/motor-mount-1), [screws for the motor mount](https://buildkitboards.com/collections/parts/products/m4x10-motor-mounting-bolts) and a cool sticker from @JLabs

![IMG_2814|666x500](upload://gjsDvQhVi7ghx4hkZZ6AN3OnYqU.JPG)

**TOTAL SPENT: $953.33**
-
```

---
## \#139 Posted by: moon Posted at: 2018-05-30T12:20:09.544Z Reads: 266

```
[quote="legend27, post:138, topic:53111"]
Payed the last import taxes today! $113, quite expensive but whatever.
[/quote]

$113 for what?!
```

---
## \#140 Posted by: JLabs Posted at: 2018-05-30T12:52:29.980Z Reads: 258

```
Yeah why was it so much? I think that’s more than the parts lol
```

---
## \#141 Posted by: legend27 Posted at: 2018-05-30T13:20:12.509Z Reads: 270

```
@moon @JLabs $113 for the parts I bought from . lol not from @JLabs. If it was then holy shit.
```

---
## \#142 Posted by: legend27 Posted at: 2018-05-30T18:49:54.403Z Reads: 281

```
**UPDATE #27**
-
Just ordered 21 items from Amazon.de. holy fuck... Hope i didn't forgot anything... I payed $261 incl. shipping for all the items and here they are:

* **3x $8** - [3mm sticky foam](https://www.amazon.de/dp/B07D22V5RC/ref=pe_3044161_185740101_TE_item_image)
* **1x $46** - [12V 40AH 340A car battery](https://www.amazon.de/dp/B01N2ANL3F/ref=pe_3044161_185740101_TE_item) @moon
*  **1x $9** - [16 AWG wire](https://www.amazon.de/dp/B07427NFJM/ref=pe_3044161_185740101_TE_item)
* **1x $14** - [10 AWG wire](https://www.amazon.de/dp/B007DMW3IU/ref=pe_3044161_185740101_TE_item)
* **1x $10** - [12mm rubber gasket for the enclosure](https://www.amazon.de/dp/B016Q1BRKI/ref=pe_3044161_185740101_TE_item)
* **1x $6** - [Insert nuts](https://www.amazon.de/dp/B01MQIL9Q3/ref=pe_3044161_185740101_TE_item)
* **1x $15** - [Digital multimeter](https://www.amazon.de/dp/B01N2NI76Y/ref=pe_3044161_185740101_TE_item)
* **1x $10** - [Solder arm](https://www.amazon.de/dp/B001BMSBD4/ref=pe_3044161_185740101_TE_item)
* **1x $8** - [Solder](https://www.amazon.de/dp/B000V8JZ2A/ref=pe_3044161_185740101_TE_item)
* **1x $30** - [Solder kit with a bunch of other stuff](https://www.amazon.de/dp/B072V3TY94/ref=pe_3044161_185740101_TE_item)
* **1x $3** - [Mini usb cable](https://www.amazon.de/dp/B002V9RMEK/ref=pe_3044161_185740101_TE_item)
* **2x $8** - [Foam pads](https://www.amazon.de/dp/B00GNAQ88O/ref=pe_3044161_185740101_TE_item)
* **1x $9** - [Battery clamp](https://www.amazon.de/dp/B002USHODG/ref=pe_3044161_185740101_TE_item)
* **1x $20** - [Wire stripper](https://www.amazon.de/dp/B00CD24EAK/ref=pe_3044161_185740101_TE_item)
* **1x $15** - [5 XT90 connectors](https://www.amazon.de/dp/B00ON34RX6/ref=pe_3044161_185740101_TE_item)
* **1x $15** - [10 bullet connectors](https://www.amazon.de/dp/B00NVMO1AY/ref=pe_3044161_185740101_TE_item)
* **1x $10** - [Lots of heat shrink](https://www.amazon.de/dp/B071D7LJ31/ref=pe_3044161_185740101_TE_item)
* **1x $9** - [A bunch of screws](https://www.amazon.de/dp/B00B22V8NI/ref=pe_3044161_185740101_TE_item)


Oh i forgot to buy a heat gun but my mom has a hair dryer :slight_smile:
btw. is it dangerous to have a car battery in your bedroom? lol

**TOTAL SPENT: $1214.33**
**REMAINING PARTS: $453**
**TOTAL: $1667.33 (10650 DKK just to make it more extreme. BUT STILL CHEAPER THAN A BOOSTED BOARD!)**
-
```

---
## \#143 Posted by: moon Posted at: 2018-05-30T18:51:35.891Z Reads: 261

```
[quote="legend27, post:142, topic:53111"]
btw. is it dangerous to have a car battery in your bedroom? lol
[/quote]

I don't think so...

I havent thought about it much but I have left my car battery/soon to be spot welder for a couple of months

Man... those are really expensive parts on amazon

I got my spot welder nearly sorted. Just waiting for a few things
```

---
## \#144 Posted by: legend27 Posted at: 2018-05-30T18:53:55.131Z Reads: 253

```
You might be right about the price but I don't know were else to buy them.
```

---
## \#145 Posted by: moon Posted at: 2018-05-30T18:55:11.642Z Reads: 269

```
Well ebay will always be slightly cheaper than amazon just because of seller fees etc.

I am making pretty much the same spot welder but different battery same company. I'll show you some pics now, one moment.

![IMG_20180530_195252|375x500](upload://rDVmkjwNG7knc49Fa99Wv26204q.jpg)
```

---
## \#146 Posted by: legend27 Posted at: 2018-05-30T19:04:37.017Z Reads: 257

```
Thats a cool spot welder! How many amps is your battery?
```

---
## \#147 Posted by: moon Posted at: 2018-05-30T19:07:41.460Z Reads: 251

```
265amps. I think its enough I saw darkkevind with 250a in one of his videos.

(removed gif- stupid crop)
```

---
## \#148 Posted by: legend27 Posted at: 2018-05-30T19:08:46.388Z Reads: 244

```
Yea, that should be enough. Mine might be a bit too high.
```

---
## \#149 Posted by: moon Posted at: 2018-05-30T19:09:10.635Z Reads: 248

```
darkkevind now uses a 330amp one now so I think its fine
```

---
## \#150 Posted by: moon Posted at: 2018-05-30T19:12:01.673Z Reads: 265

```
https://i.imgur.com/YfTHqyb.gifv

I think you've seen the GIF by now but.. :)
```

---
## \#151 Posted by: linsus Posted at: 2018-05-31T15:03:38.438Z Reads: 258

```
[quote="legend27, post:142, topic:53111"]
btw. is it dangerous to have a car battery in your bedroom?
[/quote]

Avoid Sunlight, also if its a lead acid then it exhaust fumes when charging that are quite deadly in big doses.
```

---
## \#152 Posted by: legend27 Posted at: 2018-05-31T16:18:24.797Z Reads: 278

```
**UPDATE #28**
-
Recived a lot of parts today :slight_smile:

**:**
* [VESC](products/torque-esc-bldc-electronic-speed-controller)
* [Sensor wires](products/vesc-sensor-wires)
* [Male to male](products/male-to-male-servo-connector)
* [T-Tool](products/skateboard-t-tool-blue)
* [Metric hex tool](products/metric-hex-folding-tool)
* [6355 190kv motor](products/electric-skateboard-motor-6355-190kv)
* [218mm trucks](products/torqueboards-218mm-trucks)
* [Pulley kit](products/36t-abec-pulley-combo-kit)
* [Bearing spacers](products/bearing-spacers)

**Amazon.de:**
* [Solenoid relay](https://www.amazon.de/gp/product/B01M35CE1S/ref=oh_aui_detailpage_o06_s00?ie=UTF8&psc=1)
* [Copper lugs](https://www.amazon.de/gp/product/B00843V5KE/ref=oh_aui_detailpage_o05_s00?ie=UTF8&psc=1)

![IMG_2815|666x500](upload://dEs6sDYe2y4aFrHuGHmoOv5LamT.JPG)

![IMG_2817|666x500](upload://vaUYzeS6XpFGFZlcVQYzN4mtHrU.JPG)

I also put 1 of the trucks on the board. The board already looks like a tank with those big trucks lol

![IMG_2818|666x500](upload://AszWh1JZlPuxQ19UL9cr5X8kkOl.JPG)

![IMG_2819|666x500](upload://12qeEG4Mjn05a1zEziU0qb9ZRCA.JPG)

![IMG_2820|666x500](upload://aBIHvI0lbAH7ocpYhLhZQTEAuSH.JPG)
```

---
## \#153 Posted by: moon Posted at: 2018-05-31T16:53:17.806Z Reads: 249

```
Have the same relay.

Does it smell really bad?  Like toxic chemicals
```

---
## \#154 Posted by: legend27 Posted at: 2018-05-31T16:59:57.779Z Reads: 251

```
Yes lol. A lot
```

---
## \#155 Posted by: legend27 Posted at: 2018-06-01T22:24:19.388Z Reads: 273

```
**UPDATE #29**
-
Yesterday and today has probably been the most productive days i've had in a while. Yesterday I made the wheel pulley fit in the wheel.

![IMG_2823|375x500](upload://qQn9s3UpRrE82MEW3uJDQSUVSUu.JPG)

![IMG_2824|375x500](upload://nqfvAXV272T3g0tLCuPaxyNviXp.JPG)

And today I sanded down the one of the trucks to make the motor mount fit.

![IMG_2827|666x500](upload://6vvl9ReAmNps61chnRfOcfvKAzb.JPG)

![IMG_2828|666x500](upload://wBTPZb624nHYbFlIp0ceEnj2MMo.JPG)

And then it was time to put the wheels, trucks, motor mount and motor together.

![IMG_2825|666x500](upload://9Q0TZWCnWKT0S6vqvPzLxLm2kBM.JPG)

![IMG_2826|666x500](upload://5z1vdYW2TiDH1Fgqn1Mqina1mJS.JPG)

![IMG_2829|375x500](upload://xOwtHUBdTQkwWCKU6RRVIf4Exp9.JPG)

![IMG_2830|375x500](upload://x5viM3olhZdgZbAKnk7jLKb6aw0.JPG)

![IMG_2835|375x500](upload://sLupeJpsrrQuKDwWFkYn2C7gLMC.JPG)

![IMG_2831|666x500](upload://sCHc58fSwC07Jy37pyFWUoUinL3.JPG)

![IMG_2833|666x500](upload://yFIYvWXTSwOf1ljBvjteYPRCFne.JPG)

![IMG_2834|666x500](upload://2UaVa5QoES0EaF3jH6NsCDnVnTc.JPG)

I have to buy 2 more risers so I won't get any motor bites.

![IMG_2832|666x500](upload://5HGHqfqaeRC1KPxrM7UWZ4wpHl9.JPG)

---

I also received a lot of parts from Amazon.de:

* [Digital multimeter](https://www.amazon.de/dp/B01N2NI76Y/ref=pe_3044161_185740101_TE_item)
* [Solder arm](https://www.amazon.de/dp/B001BMSBD4/ref=pe_3044161_185740101_TE_item)
* [Solder](https://www.amazon.de/dp/B000V8JZ2A/ref=pe_3044161_185740101_TE_item)
* [Solder kit and a bunch of other things](https://www.amazon.de/dp/B072V3TY94/ref=pe_3044161_185740101_TE_item)
* [Mini USB cable](https://www.amazon.de/dp/B002V9RMEK/ref=pe_3044161_185740101_TE_item)
* [Battery clamps](https://www.amazon.de/dp/B002USHODG/ref=pe_3044161_185740101_TE_item)
* [Wire stripper](https://www.amazon.de/dp/B00CD24EAK/ref=pe_3044161_185740101_TE_item)
* [5x XT90](https://www.amazon.de/dp/B00ON34RX6/ref=pe_3044161_185740101_TE_item)
* [10x 5.5mm bullet connector](https://www.amazon.de/dp/B00NVMO1AY/ref=pe_3044161_185740101_TE_item)
* [Heat shrink tube](https://www.amazon.de/dp/B071D7LJ31/ref=pe_3044161_185740101_TE_item)
* [A bunch of screws](https://www.amazon.de/dp/B00B22V8NI/ref=pe_3044161_185740101_TE_item)

![IMG_2837|666x500](upload://bFRqcHqeNel20RE2nVkTOdSO7n9.JPG)
(Forgot to put the heat shrink tubes and screws in the picture)

![IMG_2836|666x500](upload://rq0Xa7n5HSeQDe30lTqrLaW8399.JPG)
```

---
## \#156 Posted by: legend27 Posted at: 2018-06-03T16:39:17.879Z Reads: 269

```
**UPDATE #30**
-
Ordered a few (not that few) parts today :slight_smile: I payed $159.24 incl. shipping. Only parts remaining to order is the [batteries](https://eu.nkon.nl/samsung-inr-18650-30q-3000mah.html), [nickel strip](https://eu.nkon.nl/nikkel-battijersoldeerstrip-10mm.html) and [insulation paper](https://eu.nkon.nl/isolatie-papier-18650.html)!

Aliexpress:
* **3x $4.32** - [3mm riser pads](https://www.aliexpress.com/item/1-pair-6mm-3mm-Skateboard-Riser-Pads-Longboard-Highten-Pads-for-Skate-board-Shock-Pads-Cushion/32832437600.html?spm=a2g0s.9042311.0.0.2ed84c4dEsfi1l)
* **1x $7.74** - [100 pcs M5x10mm insert nuts](https://www.aliexpress.com/item/M4-M5-M6-M8-M10-Furniture-Pass-through-Drive-Unhead-Threaded-Nut-Color-Zinc-Plated-Carbon/32835710899.html?spm=a2g0s.9042311.0.0.2ed84c4dEsfi1l)
* **1x $2.79** - [Solder cleaner](https://www.aliexpress.com/item/1pc-Welding-Soldering-Accessories-Mayitr-Solder-Iron-Tip-Cleaner-Ball-Holder-with-Steel-Wire-Sponge/32825960896.html?spm=a2g0s.9042311.0.0.2ed84c4dEsfi1l) 

Eskating.eu:
* **1x $3.5** - [Thread locker](https://eskating.eu/product/thread-locker-for-pulleys-and-bolts-medium-strong/)
* **1x $60** -  [Anti spark power switch](https://eskating.eu/product/anti-spark-power-switch/)
* **1x $8** - [Battery LED](https://eskating.eu/product/battery-percentage-voltage-lcd-display/)
* **1x $5** - [Charge port](https://eskating.eu/product/dc-in-battery-2-1mm-socket-with-dust-cover/)
* **1x $29** - [42V 2A charger](https://eskating.eu/product/2-amp-charger-10-and-12-s/?attribute_voltage=42V)
* **2x $7** - [180mm heat shrink](https://eskating.eu/product/heat-shrink-for-esk8-lithium-battery-packs-1m-various-size-tailored/?attribute_width=180mm&attribute_color=Black)


The 265mm belt I received from  is a little bit too big. PWRBoards.com told me the wrong dimensions of the enclosure, but have given me a free 255mm belt as a "We're sorry" gift :slight_smile: If anyone wants the 265mm belt and pays the shipping then message me. I live in Denmark.

![IMG_2838|666x500](upload://7gs268RcikaBtvJq7BbiIRrmiY6.JPG)

![IMG_2839|666x500](upload://3UHDLqDHWspJk8rU0zJYbKEix44.JPG)

**TOTAL REMAINING: $310**
**TOTAL SPENT: $1373.57**
-
```

---
## \#157 Posted by: JLabs Posted at: 2018-06-03T16:55:48.005Z Reads: 252

```
How long did it take you to sand the trucks? When your set in on where your placing them you could get some matte black spray paint to cover up the sanding marks.
```

---
## \#158 Posted by: legend27 Posted at: 2018-06-03T17:00:02.328Z Reads: 249

```
I spent between 2 hours plus minus sanding them down. I took it slow and easy to make sure I wouldn't fuck anything up. And I don't really care about the sanding marks. That can be a project in the future to make it look much cooler :slight_smile: I might do that. What spray paint do you recommend?
```

---
## \#159 Posted by: legend27 Posted at: 2018-06-05T10:40:45.209Z Reads: 265

```
**UPDATE #31**
-

Received my car battery today. It came with some water in the bag and was soaked completely? Don't know if it was water cause it smelled a bit sour? There is also water inside the battery? Is the battery defect or is this normal?

![IMG_2842|666x500](upload://gqsP2qMTq7oCKJgyIG0TvqH8xfZ.JPG)
![IMG_2841|666x500](upload://554Iurdfo1LdEj5lPUKYbKkxwsq.JPG)
![IMG_2844|375x500](upload://eClIPQzwXyCVhdYPFU9OBsmPAko.JPG)![IMG_2843|375x500](upload://CaQSqJnRonCJmtAfYfH2lZvXGM.JPG)
![IMG_2845|375x500](upload://4gSWq56WRaPGAJNvAmRvCfRljP3.JPG)
```

---
## \#160 Posted by: moon Posted at: 2018-06-05T10:48:45.379Z Reads: 238

```
I think that will be lead acid, that whats inside car batteries.
```

---
## \#161 Posted by: legend27 Posted at: 2018-06-05T10:49:51.425Z Reads: 235

```
So the battery has been damaged if so? And is it dangerous?
```

---
## \#162 Posted by: FredrikHems Posted at: 2018-06-05T11:10:21.354Z Reads: 238

```
You should contact the seller. Seems abit wierd.
```

---
## \#163 Posted by: legend27 Posted at: 2018-06-05T11:20:59.003Z Reads: 250

```
Think I know what it is now. It's the lead acid from the battery as @moon said that comes out from these holes

![IMG_2846|374x500](upload://kcSY31gXbatklqflnDL0z4It0Ex.JPG)

On the box it says that the battery should be transported a special way and they might not have done that...

![IMG_2847|375x500](upload://p2mMe774J2w971AWCYfwOPhZUga.JPG)

The lead acid isn't dangerous but you should was it off your hands. If not done then your hands might get a bit dry. Nothing else.
```

---
## \#164 Posted by: legend27 Posted at: 2018-06-05T11:25:14.370Z Reads: 244

```
Also got a replay back from the seller:

Hello Legend27,

Thank you for your request.

Occasionally, a small amount of leakage comes out of the vent holes of the battery. Please follow these steps:

1. Carefully clean the batteries, taking care that no acid touches your hands or clothing. Please do this outside by wearing suitable protective clothing.

2. Check for physical damage.

3. If no physical damage occurs, please use batteries as usual and monitor their performance. We state that the batteries are primarily overfilled in the first place to avoid low leakage during transport.

4. If you have any problems, please contact us immediately. Your warranty period is not affected.

Best regards




Edit: btw. thanks a lot for the help @moon
```

---
## \#165 Posted by: legend27 Posted at: 2018-06-05T14:34:37.390Z Reads: 249

```
Progress

![IMG_2848|666x500](upload://hx2X1iwc3N47pF8wBJmTM2NDUXv.JPG)

![IMG_2849|666x500](upload://yqVmflHMRAOeFy38zpuxCLppqUi.JPG)
```

---
## \#166 Posted by: legend27 Posted at: 2018-06-05T15:12:27.308Z Reads: 251

```
**UPDATE #32**
-
The spot welder is done! Thanks a lot to @darkkevind for making this amazing spot welder! I don't have any nickel strip to test it with.
Here is a short video of it: https://youtu.be/6MbLlSevb2Y

![IMG_2850|666x500](upload://pRddxo9k2vv7SMdcNsOd8SDc2IB.JPG)

![IMG_2851|666x500](upload://gevU2cLNLjraGh7kbhMkgP52Lec.JPG)

![IMG_2852|666x500](upload://nglEdrSX0OD6x6hlXmzkJSLshOx.JPG) 

![IMG_2854|375x500](upload://nI6rMBsPSkaxCpJ8uispH3a1U1w.JPG)

![IMG_2855|666x500](upload://3vV6yEIpq3qV4b8AjdDX6lSOPfB.JPG)
```

---
## \#167 Posted by: rey8801 Posted at: 2018-06-05T15:23:11.930Z Reads: 228

```
Nice you could tet it on a cutter blade. Usually nickel + cutterblade is a good test for a spot welder. For the moment just try on a cutter blade to see if it is working. I also made an sport welder but using a microwave trasformer and an arduino...
```

---
## \#168 Posted by: legend27 Posted at: 2018-06-05T15:25:40.423Z Reads: 233

```
Microwave transformer wow
```

---
## \#169 Posted by: rey8801 Posted at: 2018-06-05T15:31:33.603Z Reads: 238

```
It's full of tutorial online. I just didn't want to spend anything on it and I had a old microwave so...I called the "Frankenstein Spot Welder" for how ugly it is. You can see it in the first post of my build http://www.electric-skateboard.builders/t/first-build-the-avenger-jet-spud-dual-hubs-motors-custom-10s3p-30q-maytech-vescs/52437?u=rey8801 :smiley: The tricky part was to get a good welding because by just using a momentary button was to strong :rofl: then the arduino help since you can actually program the duration of the pulses.
```

---
## \#170 Posted by: legend27 Posted at: 2018-06-05T18:19:16.091Z Reads: 236

```
**UPDATE #33**
-
The spot welder didn't work that well. The welds wasn't good and it started to fall apart lol. Have to make it over again an other time. Might also have to get some clamps that actually fit. That might fix the bad welds problem. But at least i got most/all of the parts :slight_smile:
```

---
## \#171 Posted by: rey8801 Posted at: 2018-06-05T18:35:55.385Z Reads: 228

```
For a good welding you really have to be able to push your pins on the surface. With a certain pressure to ensure a good contact. To do that you need to right build a proper pins holder and arm because it get hot around the pins and it will fall apart if it's only taken in place by tape or similar materials.
```

---
## \#172 Posted by: Itsmedant Posted at: 2018-06-05T18:43:00.463Z Reads: 222

```
I purposely didn't track how much money I was dumping into my board.....I would be driving myself crazy! Good luck with the rest of the build!
```

---
## \#173 Posted by: sk8l8r Posted at: 2018-06-06T08:31:42.076Z Reads: 228

```
[quote="Itsmedant, post:172, topic:53111"]
I purposely didn’t track how much money I was dumping into my board
[/quote]

I started out tracking my costs, at least until it started to stress me now I just track what I have left to get ;)
```

---
## \#174 Posted by: Itsmedant Posted at: 2018-06-06T13:50:11.243Z Reads: 226

```
I know the feeling! Maybe one day I'll go back and add everything up once its done! I just gotta get my batteries now and then my build can proceed....that and make a new deck since the one I was planning on using is too bendy!
```

---
## \#175 Posted by: legend27 Posted at: 2018-06-14T19:16:09.532Z Reads: 248

```
**UPDATE #34**
-
Hello again everyone :slight_smile: I haven't made that much progress but im moving forward. Received the [riser pads](https://www.aliexpress.com/item/1-pair-6mm-3mm-Skateboard-Riser-Pads-Longboard-Highten-Pads-for-Skate-board-Shock-Pads-Cushion/32832437600.html?spm=a2g0s.9042311.0.0.36e64c4dvgZq2N), [sticky foam](https://www.amazon.de/gp/product/B07D22V5RC/ref=oh_aui_detailpage_o03_s00?ie=UTF8&psc=1) and [foam](https://www.amazon.de/gp/product/B00GNAQ88O/ref=oh_aui_detailpage_o05_s02?ie=UTF8&psc=1) a few days ago. AND 2 FREE 255mm(250mm?) belts from pwrboards.com! Thanks guys!

![IMG_2863|666x500](upload://yYdNlQqxNfxHS3krGz53ObFC82O.JPG)

![IMG_2866|666x500](upload://9MF41f3jILfvucsU8SvOjFMmQ59.JPG)

Belt tension seems perfect!

![IMG_2873|666x500](upload://xpxPaPx8fRPYmdp21qG4N8lV0vw.JPG)

![IMG_2874|666x500](upload://3tnG0jwFgtXbMWajH4FZt9fijVK.JPG)

![IMG_2860|375x500](upload://agAKgr8WWloUGwMKOZP16A0F7Ir.JPG)

There is just one issue. I tried installing 3 pairs of 3mm riser pads, but the motor mount still hits the deck, when I make really sharp turns. I don't know if I am going to turn that sharp but do you have any ideas on how to fix it? And is that enough room for the trucks to stay mounted?

![IMG_2875|666x500](upload://354VXu1ryYOG0wr0hLHokH8AALo.JPG)

![IMG_2879|666x500](upload://zOdTgp7diSfgVrhG8IpDIGdV2vf.JPG)

![IMG_2877|666x500](upload://99L1obOoKpgB6HMND62eTwC7njO.JPG)
(1cm-1.5cm clearance)

![IMG_2881|666x500](upload://8qG7CsIVDtNQKDPKDmMQnrQZ4TF.JPG)
(motor mount hits deck

And just some pictures of the board
![IMG_2869|666x500](upload://om5mvOazReCbbOXgDDK5j8wudcT.JPG)

![IMG_2868|666x500](upload://scqm71mvE3WamlSwxgANoAT4VlW.JPG)

Thanks for all the help guys and reading this post. Im getting to the point where this project is getting boring since everything takes weeks before arriving and I feel like im running into issues all the time (Im not really but it feels like)... Hopefully things get funnier when they start working and it dosen't feel like a bad prototype.
```

---
## \#176 Posted by: Toughook Posted at: 2018-06-14T19:45:12.350Z Reads: 226

```
Hey don't worry about the time taken so far ! I spent 4 months of dithering about before getting to a rideable stage, and I didn't need to do half as much as you are doing in your build - by which I mean I bought a ready made battery as wasn't confident in welding my own like you are doing.

All I can say is that rushing any job will lead to mistakes, often costly, and with your detailed budgeting (something I dare not EVER think about regarding my own board!!!!) it'll only serve to frustrate you more ... Lol

Seriously though, your build is great and your links and costing show you are going to succeed with this eventually. 

Looking forward to seeing the finished board 👍👍👍
```

---
## \#177 Posted by: threebysix Posted at: 2018-06-14T20:05:05.534Z Reads: 211

```
Maybe try to angle the motor mount so it's more parallel with the ground? That's what I did to gain more clearance between motor and deck.
```

---
## \#178 Posted by: legend27 Posted at: 2018-06-14T20:16:08.262Z Reads: 208

```
Wow man thanks! Don't know what you did, but that just gave me a lot of hope! That's why I love this forum! It's full of friendly people that helps you in a magical way like you. And wow your board looks so clean and awesome!
```

---
## \#179 Posted by: dg798 Posted at: 2018-06-14T20:17:18.292Z Reads: 205

```
I’m almost a year in to my board and have only gotten it working for a few weeks. I am on my 3rd motor and getting my 3rd vesc. And I’m on my third deck and third BMS. I am also on my 2nd battery.
I have wanted to give up so many times but people on this forum provide real inspiration for me to continue.
```

---
## \#180 Posted by: legend27 Posted at: 2018-06-14T20:22:00.871Z Reads: 209

```
[quote="dg798, post:179, topic:53111"]
I have wanted to give up so many times but people on this forum provide real inspiration for me to continue.
[/quote]

It's so true! I feel like the community is 50% of electric skateboard, so if this community didn't exists, I think the eskate community would be much smaller.
```

---
## \#181 Posted by: dg798 Posted at: 2018-06-14T20:22:45.710Z Reads: 223

```
Totally agree.
Keep going.
Never give up.
It will all be worth it in the end
```

---
## \#182 Posted by: dg798 Posted at: 2018-06-14T20:25:08.266Z Reads: 228

```
This was in the very beginning of this long expensive journey:
![image|690x482](upload://71R7Fnnh90Hbx0h4qSrTHQIIF4M.jpeg)
```

---
## \#183 Posted by: legend27 Posted at: 2018-06-14T20:26:21.768Z Reads: 208

```
And how does it look now?
```

---
## \#184 Posted by: dg798 Posted at: 2018-06-14T20:35:58.404Z Reads: 205

```
Everything is taken apart right now so I have nothing really atm but should have it up and running by the beginning of next week.
Will post pics.
```

---
## \#185 Posted by: legend27 Posted at: 2018-06-14T20:38:16.912Z Reads: 213

```
Yea man please post some pictures. Would love to get some more inspiration! And good luck putting everything back together.
```

---
## \#186 Posted by: dg798 Posted at: 2018-06-14T20:39:55.087Z Reads: 224

```
Thanks I will need it.
I’m actually in middle of doing a mad monkey mod. This is the gt2b disassembled:
![image|375x500](upload://wf7LEVidwXX4ucJsupBgHSIfFpr.jpg)
I’m happy I don’t screw anything up disassembling it.😉
```

---
## \#187 Posted by: GrecoMan Posted at: 2018-06-14T21:04:35.874Z Reads: 205

```
i give it like an 80% chance that you fuck up the usb port lol
```

---
## \#188 Posted by: Mattmccrary8 Posted at: 2018-06-14T21:34:53.411Z Reads: 201

```
Lmao your an ass hole 😂😂😂😂
```

---
## \#189 Posted by: dg798 Posted at: 2018-06-14T22:39:53.042Z Reads: 206

```
how rude.
when im done i will post a pic and prove you wrong
```

---
## \#190 Posted by: pat.speed Posted at: 2018-06-14T22:58:04.306Z Reads: 205

```
Haha I think he’s joking, cos that’s what a lot of people stuff up.
```

---
## \#191 Posted by: GrecoMan Posted at: 2018-06-14T23:27:04.895Z Reads: 206

```
lol i only said that cause i did it the first time...

psa for everybody: plz don’t take anything i say seriously unless i specify that i’m being serious
```

---
## \#192 Posted by: Apolo Posted at: 2018-06-14T23:32:13.310Z Reads: 207

```
Mjolnir bruh
```

---
## \#193 Posted by: moon Posted at: 2018-06-14T23:34:14.205Z Reads: 205

```
Haha thanks

@legend27 did you get your spot welder working
```

---
## \#195 Posted by: Zac13 Posted at: 2018-06-15T02:16:59.823Z Reads: 212

```
"You need to watch your percentage display, periodically check your cell balance levels, and make sure you turn your board off when you’re not riding it."

How often do you check your cell balance levels?
```

---
## \#196 Posted by: psychotiller Posted at: 2018-06-15T02:32:43.063Z Reads: 206

```
Anytime I need to take off my enclosure, or if the board is behaving differently. Could be every month or so.
```

---
## \#197 Posted by: legend27 Posted at: 2018-06-15T03:38:51.986Z Reads: 210

```
Not yet. I'm waiting for new battery clamps and lugs to arrive from amazon. What's the status of your spot welder?
```

---
## \#198 Posted by: moon Posted at: 2018-06-15T11:07:44.367Z Reads: 206

```
Stuff still coming. Should be here soon
```

---
## \#199 Posted by: Blitz Posted at: 2018-06-16T16:41:13.279Z Reads: 202

```
[quote="GrecoMan, post:191, topic:53111"]
psa for everybody: plz don’t take anything i say seriously unless i specify that i’m being serious
[/quote]

seriously...?

Edit: If you said something bad you will be held accountable for it, there are no excuses.
```

---
## \#200 Posted by: GrecoMan Posted at: 2018-06-16T16:48:14.415Z Reads: 199

```
lol i’m just trying to save you guys from getting buthurt because you don’t understand the jokes
```

---
## \#201 Posted by: legend27 Posted at: 2018-06-18T07:53:54.722Z Reads: 215

```
**UPDATE #35**
-
Just paid an import bill on $25 for the f**cking BMS and controller I received 30 days ago. It took them 14 days to send the bill and 14 days for me to receive it.

**TOTAL SPENT: $1,425.69**
**TOTAL REMAINING: $310**
-
**TOTAL: 1,735.69**
This is the total incl. tools. Compared to what the new Boosted Board Stealth would cost for me ($2,123.75) then it's not really that expensive :slight_smile: I've also got a lot of knowledge I wouldn't had got by buying a complete board. 
-
```

---
## \#202 Posted by: legend27 Posted at: 2018-06-23T15:22:54.864Z Reads: 219

```
**UPDATE #36**
-
Made this diagram :slight_smile:
Question: Is the charge port wired correctly? (and everything else)

![board|690x388](upload://2VO1QiwnJKwIMeh8200h5LtaFZv.jpg)
```

---
## \#203 Posted by: legend27 Posted at: 2018-06-26T17:17:20.089Z Reads: 241

```
**UPDATE #37**
-
Hi again everyone :slight_smile:
I've made some progress since last time.
  
Received a few items some days ago. Here they are :slight_smile:

**Amazon:**
* [Rubber gasket](https://www.amazon.de/gp/product/B016Q1BRKI/ref=oh_aui_detailpage_o01_s00?ie=UTF8&psc=1) (not on the picture)
* [16 AWG cable](https://www.amazon.de/gp/product/B07427NFJM/ref=oh_aui_detailpage_o02_s00?ie=UTF8&psc=1)
* [10 AWG cable](https://www.amazon.de/gp/product/B007DMW3IU/ref=oh_aui_detailpage_o02_s00?ie=UTF8&psc=1) (didn't really get this cable. They had sent me a 18 AWG cable instead. They let me keep the 18 AWG, now im just waiting for the 10 AWG to arrive.)

**Aliexpress:**
* [Threaded nuts](https://www.aliexpress.com/item/M4-M5-M6-M8-M10-Furniture-Pass-through-Drive-Unhead-Threaded-Nut-Color-Zinc-Plated-Carbon/32835710899.html?spm=a2g0s.9042311.0.0.3c154c4dAj80BX)

**Eskating.eu:**
* [Thread locker](https://eskating.eu/product/thread-locker-for-pulleys-and-bolts-medium-strong/)
* [Anti Spark Power Switch](https://eskating.eu/product/anti-spark-power-switch/)
* [Battery percentage LED](https://eskating.eu/product/battery-percentage-voltage-lcd-display/)
* [Charge port](https://eskating.eu/product/dc-in-battery-2-1mm-socket-with-dust-cover/)
* [42V 2A charger](https://eskating.eu/product/2-amp-charger-10-and-12-s/?attribute_voltage=42V)
* [180mm heat shrink](https://eskating.eu/product/heat-shrink-for-esk8-lithium-battery-packs-1m-various-size-tailored/?attribute_width=180mm&attribute_color=Black)

![IMG_2888|375x500](upload://ngV0f2ogVrQj7x94NWC8Vxgm5rw.JPG) 

Now to what i've done to the board/parts (the more exciting part)
I've put the rubber gasket on the enclosure and put the 3mm foam on the board
-

![IMG_2911|666x500](upload://rjMWy7fpTEaaRbQCqNyGkrGMrKP.JPG)

![IMG_2912|666x500](upload://g62dAeanB9ecGxtfHJ0jpdwe1AV.JPG)

![IMG_2913|666x500](upload://da8zfUFPg1VtyePtAQkbeQrcEO9.JPG)

![IMG_2907|375x500](upload://xlMRLBJ6WGa9uoGuYg9ze7qTU00.JPG)

![IMG_2908|666x500](upload://ag5Siv5QXu9l2NL03YEcwZhv2AB.JPG)

![IMG_2910|666x500](upload://zOrDCy4h0a0mQbxt0hOYMcBtPkF.JPG)

![IMG_2909|666x500](upload://sVDemZk8dP4KD1Wf9FjRpbTrtwR.JPG)

Put thread locker on all the bolts
-

![IMG_2914|666x500](upload://zCKwO7RUhYmOqTBARHkxbvguMX6.JPG)

And the least important thing (noone probably cares but I do!)
I've cleaned my "workbench"
![IMG_2917|666x500](upload://6LU2Zre8O1tB0GVfpYyyvE9ytji.JPG)

![IMG_2916|666x500](upload://tL7e8O0C0eNrqfMa73qJHJNhBWt.JPG)

![IMG_2918|666x500](upload://7bKS58kwItVjZaPeayQhD6EiKVn.JPG)

Fun fact: This is what my board parts look like when I don't want them to get dusty
![IMG_2915|666x500](upload://hOrmdb6AV3S8mOCe1deDR9PJQR7.JPG)
```

---
## \#204 Posted by: legend27 Posted at: 2018-06-30T18:36:55.822Z Reads: 246

```
**UPDATE #38**
-
I have ordered some parts :slight_smile: Here they are:
(all the prices are including shipping)

**Aliexpress:**
* **1x $1.9** - [HM-10 Bluetooth module](https://www.aliexpress.com/item/Freeshipping-HC-06-Wireless-Bluetooth-Module-With-baseboard-Slave-Wireless-Serial-Port-for-arduino-with-Dupont/1568545615.html?spm=a2g0s.9042311.0.0.5cf94c4dGQhvS1)
* **1x $3.22** - [7 pin cable](https://www.aliexpress.com/item/10pcs-Micro-JST-Mini-2-0-PH-2-3-4-5-6-7-8-9-10/32868201984.html?spm=a2g0s.9042311.0.0.5cf94c4dGQhvS1)
* **1x $1.88** - [Battery holder](https://www.aliexpress.com/item/Mayitr-Battery-Holder-2pcs-10x-Cell-Plastic-18650-Battery-Holder-Cell-Spacer-Cylindrical-Cell-Bracket-for/32863340138.html?spm=a2g0s.9042311.0.0.5cf94c4dGQhvS1)
* **1x $0.38** - [22 AWG cable (white)](https://www.aliexpress.com/item/Tinned-copper-22awg-cable-1007-electric-wire-PVC-insulated-22-awg-Electric-cable-LED-Lighting-Strip/32789815353.html?spm=a2g0s.9042311.0.0.5cf94c4dGQhvS1)
* **50x $9.45** - [M5 screws (25mm, 30mm, 35mm lenght)](https://www.aliexpress.com/item/M5-Bolt-Stainless-Steel-Hex-Socket-Cap-Screws-304-Stainless-Allen-Bolt-DIN912-M5-6-8/32815262851.html?spm=a2g0s.13010208.99999999.261.33f83c00SbOijk)

**Ebay:**
* **1x $19.90** - [Fish paper](https://www.ebay.com/itm/192184288680)

**Amazon:**
* **1x $7.5** - [Battery clamp](https://www.amazon.de/gp/product/B01LBL21BW/ref=oh_aui_detailpage_o00_s00?ie=UTF8&psc=1)
* **1x $7.5** - [Lugs](https://www.amazon.de/gp/product/B01E75BEM6/ref=oh_aui_detailpage_o00_s00?ie=UTF8&psc=1)

**NEW TOTAL: 1,787.42 (only 300 above expected pfffff)**
-

**Enough of parts and money. Let's take a look at what i've done to the board!**
-

I think im going to lay the parts in the enclosure like this:

![IMG_2920|375x500](upload://ulxGgR0fNGftDdLTyoMRHatjlup.JPG)

![IMG_2919|375x500](upload://tqgJd1oUNHqKaoC9wzQE9Cj1cqH.JPG)

**QUESTION TIME:**
**Can i put 2mm foam on all the sides of the enclosure without any of my parts are going to overheat?**
-


Back to the board:
Today I added some more foam on the board to make the enclosure lay flat. Turned out pretty good!

![IMG_2945|666x500](upload://67q1vqzokxiz3dLqqQeXCzR9kwC.JPG)

![IMG_2940|666x500](upload://wYpKjxfu5tRMyNOBBTfcsxWuxFP.JPG)

![IMG_2947|666x500](upload://wWmI6S0jK9Jx8iG2fwP134ApIef.JPG)

![IMG_2941|666x500](upload://zHS9Imgny6EON0V3AG2bQoCS6yX.JPG)

![IMG_2942|666x500](upload://yHJDkDEKrnfNA6CbWt8xMoLCVsm.JPG)

![IMG_2944|666x500](upload://vglQn0WfeN2fSRelfuHBUefaHt7.JPG)

![IMG_2946|666x500](upload://yPLUpXJ4nEq5dI32jtuv3Tikoss.JPG)
```

---
## \#205 Posted by: legend27 Posted at: 2018-07-04T15:12:31.954Z Reads: 233

```
***from the "Noob question thread"***

Hi everyone :slight_smile:
Im going to make a 10S6P samsung 30Q battery but I don't know how to weld the pack together. I have two options. Which one is the best? Maybe why? Any other suggestions?

**OPTION 1:**
-
I use 10mm X 0.15mm nickel strip. If there are two lines, that means im putting 2 nickel strips instead of 1. (not my picture from the side view)
![battery1|690x388](upload://r86JPGRoyAiAHtwJNxBbaRhAA16.jpg)

--------------

**OPTION 2**
-
I use 10mm X 0.15mm nickel strip. All the read lines are 2 nickel strips on top of each other.
![board|690x388](upload://2VO1QiwnJKwIMeh8200h5LtaFZv.jpg)
```

---
## \#206 Posted by: legend27 Posted at: 2018-07-09T18:37:34.730Z Reads: 223

```
**UPDATE #39**
-
Currently waiting for a lot of china parts to arrive. At the time they arrive, will I order the batteries and the build will be done soon after. One important thing I have learned and I think everyone should know is: Always order parts from China before ordering anything else.

**Aliexpress:**
* **1x $3** - [Plastic box](https://www.aliexpress.com/item/Mayitr-10-15-24-Slots-Compartment-Organizer-Plastic-Storage-Box-Case-Container-Adjustable-Jewelry-Box-Display/32820395015.html?spm=a2g0s.9042311.0.0.7edb4c4daRnVQq)
* **1x $1.15** - [Double sided tape](https://www.aliexpress.com/item/Practical-Auto-Acrylic-Foam-Double-Sided-Attachment-Tape-3M-10mm-3844/32381641996.html?spm=a2g0s.9042311.0.0.7edb4c4daRnVQq) 
* **1x $5.50** - [Dual lock (really really really strong velcro)](https://www.aliexpress.com/item/3M-brand-tape-SJ3550-dual-lock-self-adhesive-fastener-3M-tape-250-type-mushroom-black-15/1000001467327.html?spm=a2g0s.9042311.0.0.7edb4c4daRnVQq)
* **Random sizes $6** - [Cable glands](https://www.aliexpress.com/item/High-Quality-IP68-PG16-10-14MM-Waterproof-Nylon-Cable-Gland-No-Waterproof-Gasket-Plastic-Waterproof-Connector/1986015521.html?spm=a2g0s.9042311.0.0.7edb4c4daRnVQq)
* **Random sizes $1.57** - [Cable sleeve](https://www.aliexpress.com/item/1M-Black-Braided-Expandable-Cable-Sleeve-Tight-PET-High-Density-Wire-Sleeve-Sheathing-PC-Cable-Organizer/32860329441.html)

**Ebay:**
* **1x $10** - [Battery terminal adapters](https://www.ebay.com/itm/Japanese-Car-Battery-Terminal-Post-Adapters-Small-Post-Conversion/362003348200?ssPageName=STRK%3AMEBIDX%3AIT&_trksid=p2060353.m2749.l2649)

**NEW TOTAL: $1814.64**
-
```

---
## \#207 Posted by: Grozniy Posted at: 2018-07-09T23:18:38.889Z Reads: 219

```
I used that dual lock, the genuine one and wasn't impressed. The dial lock is so strong that it rips the whole strip from the surface, the "glue" on it is weaker than the dual lock ahaha but maybe in your case, it will work better
```

---
## \#208 Posted by: legend27 Posted at: 2018-07-11T21:46:04.962Z Reads: 247

```
**UPDATE #40**
**_10-07-2018:_**
-

Ordered some more stuff from China. Of course I got some fish paper from ebay that cost me $19 and today I just found some fish paper from AliExpress for $2.5...

**AliExpress:**
* **2x $2** - [Fish paper for positive battery site](https://www.aliexpress.com/item/100pcs-1S-18650-Battery-Insulation-Gasket-Barley-Paper-Battery-Pack-Cell-Insulating-Glue-Patch-Positive-Electrode/32827000489.html?spm=a2g0s.9042311.0.0.5d254c4dyZbqhR)
* **2x $4.60** - [Fish paper with adhesive](https://www.aliexpress.com/item/1m-120mm-18650-Battery-Insulation-Gasket-Barley-Paper-Li-ion-Pack-Cell-Insulating-Glue-Patch-Positive/32827522392.html?spm=a2g0s.9042311.0.0.5d254c4dyZbqhR)
* **1x $1.07** - [Fish paper for positive site of the battery but with a little thing to glue you're balance lead on](https://www.aliexpress.com/item/70pcs-1S-18650-Battery-Insulation-Gasket-Barley-Paper-Battery-Pack-Cell-Insulating-Glue-Patch-Positive-Electrode/32851824498.html?spm=a2g0s.9042311.0.0.5d254c4dyZbqhR)

**NEW TOTAL: $1,822.27**
-

Im also going to order some fish paper from Nkon when ordering the batteries. Then i'll do a quality test (me touching the fish paper and see what feels best. ALSO SETS IT ON FIRE :open_mouth: )

------------------

I received the [7 pin cables](https://www.aliexpress.com/item/10pcs-Micro-JST-Mini-2-0-PH-2-3-4-5-6-7-8-9-10/32868201984.html?spm=a2g0s.9042311.0.0.5cf94c4dGQhvS1) so if anyone wants 1 or 2 of them, hit me up. Shipping from Denmark costs around $5...
And the foam: I found it on the streets while crusing around on my bike. One mans trash is another mans treasure :white_check_mark:

![IMG_2958|666x500](upload://z0803nYtiqxO2sEa96Udhb6it08.JPG)

![IMG_2959|666x500](upload://qt95tUpsY0pUVjUbEDDPS7U3cqA.JPG)

----

I also found this cool diagram of the VESC 4.8.
- **Canbus**: connect another VESC.
- **P1: HALL SENSOR**: Connect the motor sensor wire.
- **P2: SWD**: No idea
- **P3: UART**: Connect bluetooth module.
- **3 wires in left corner**: Connect the receiver for the remote.
![vesc-diagram_1530326294055|585x500](upload://jViFxl8Vn2AxeVhTsMBjuvRbcQn.png)

-----

**_11-07-2018:_**
-

I received an [apdapter](https://www.ebay.com/itm/Japanese-Car-Battery-Terminal-Post-Adapters-Small-Post-Conversion/362003348200?ssPageName=STRK%3AMEBIDX%3AIT&_trksid=p2060353.m2749.l2649) for my car battery to make the clamps fit :slight_smile: Put everything back together and BAM everything works! 
Well that's not really what happend... I tried welding 2 peices of metal together but instead of welding them together it made a lot of sparks. Don't know whats the issue? Does anybody know? @darkkevind @moon
On the bright side: Now it dosen't feel like a prototype and everything dosen't fall into pieces when im touching it.

![IMG_3058|666x500](upload://lDdACRyZehhda9gXofOamXTPMlQ.JPG)

![IMG_3059|666x500](upload://4zTGE4h54EwhBSSeEOJbDsqg3Uy.JPG)

![IMG_3060|666x500](upload://mmHgIu42hhN3Bb2U0R2usZUZKXv.JPG)

![IMG_3066|666x500](upload://t8RxHWCEHo9FOfHhj63NLmG4JFn.JPG)

![IMG_3062|666x500](upload://gHdpEkIMi6fvUqTDQ4sgzXGxHPr.JPG)

![IMG_3061|666x500](upload://nGPCGDoKPWy3PQDmCkL4qB6o0ao.JPG)

![IMG_3064|666x500](upload://ohH7xrHCOWNv7H3ofCnEh7g3oz7.JPG)

![IMG_3065|666x500](upload://jLoGgrBgpbhwQFplCnEgQ7Qb9uS.JPG)

![IMG_3063|666x500](upload://aERHznP3r8vp8lF18wDXmXs9XvU.JPG)
```

---
## \#209 Posted by: mmaner Posted at: 2018-07-12T00:53:09.705Z Reads: 213

```
The diagram is for the VESC 4.12.  I made a typo and didn't see it until days later, by the then it was too late to edit.
```

---
## \#210 Posted by: legend27 Posted at: 2018-07-12T09:41:06.257Z Reads: 226

```
**My thoughts about the spot welder**
-

The 2 metals pieces I tried welding together is around 0.5mm thick and is bend everywhere. Could the problem be that the spot welder dosen't have enough power to weld them together. And the sparks come because the metal isn't touching properly? I don't have any razor blades to test it with but is there something else I can test it with instead?

![IMG_3068|666x500](upload://gcuL9iO5Qg2tr9xibJWpxi75bk9.JPG)

![IMG_3069|666x500](upload://5lenPYSLbVXxzjBDj6DwgxRvITj.JPG)

![IMG_3070|666x500](upload://A49Y5bjWrlYlQJ0XiQZx2QWkdtF.JPG)

![IMG_3071|666x500](upload://kjngQzzO959KVvhilmM0rhVKMXo.JPG)
```

---
## \#211 Posted by: moon Posted at: 2018-07-12T11:05:00.175Z Reads: 203

```
I think this problem occurs because of the tips. Just try different configurations? I am not sure.

Is the nickel pure?

I accidentally bought my terminal blocks from a Chinese ebay seller so I can't test alongside with you and give you my thoughts

Also 0.5mm is quite a lot

@legend27 any chance you got any spare junction boxes? My button came today so I wired that up, at least the relay works :slight_smile:
```

---
## \#212 Posted by: legend27 Posted at: 2018-07-12T15:08:51.073Z Reads: 218

```
@moon Is that a junction box?

![IMG_3075|666x500](upload://bNvdLhAJro40ZRa0h9KueclM0Nh.JPG)

And if you need some new battery clamps I got 2 in spare.

![IMG_3076|666x500](upload://pZ07LvlgRFb53c486PnLSw9Hz6M.JPG)

It's just a piece of metal
```

---
## \#213 Posted by: moon Posted at: 2018-07-12T15:12:24.808Z Reads: 195

```
Yeah thats a junction connector, I dont know why I said box.
```

---
## \#214 Posted by: legend27 Posted at: 2018-07-12T15:16:57.359Z Reads: 196

```
How many do you need? Shipping is $5
```

---
## \#215 Posted by: moon Posted at: 2018-07-12T15:18:41.969Z Reads: 192

```
I will need one, It might not take that long to ship from China so I might wait it out. Il go local hardware shop see if theres anything too

Did you try the spot welder again?
```

---
## \#216 Posted by: legend27 Posted at: 2018-07-12T15:20:21.200Z Reads: 187

```
Okay :slight_smile: tell me if you want one
```

---
## \#217 Posted by: legend27 Posted at: 2018-07-12T17:17:24.338Z Reads: 224

```
I'm currently making a pen for my welder. I like the idea that I can do it one handed this way.

![IMG_3079|666x500](upload://6zZTXZ4kb4EIpKe96fNv4CORir.JPG)

![IMG_3080|666x500](upload://fYfBYJffvt3NMMvyl42cECwwb1O.JPG)

Just don't know how practical it is. What do you think is most practical?

![IMG_3077|666x500](upload://7Qmhmj5qLknqqMik2J08qgsR3p6.JPG)

![IMG_3078|666x500](upload://dPESJ8gFiq5APXq834e4gGaKy2M.JPG)


(Found the design in another thread about a spot welder. Think it's in the boss welder thread)
```

---
## \#218 Posted by: moon Posted at: 2018-07-12T19:59:01.789Z Reads: 200

```
The design looks great

I am also trying to make it one handed. Thats why I added an arm to my spot welder.

I dont know where to place my button though
```

---
## \#219 Posted by: legend27 Posted at: 2018-07-12T21:31:22.732Z Reads: 204

```
I placed it on the wood plate I made. If it's on the top then it's hard to press fast.
```

---
## \#220 Posted by: moon Posted at: 2018-07-12T21:40:27.341Z Reads: 198

```
Have you got it working?
```

---
## \#221 Posted by: legend27 Posted at: 2018-07-12T21:49:36.583Z Reads: 195

```
Not yet. Im going to continue tomorrow. Have you made any progress on yours since last time?
```

---
## \#222 Posted by: JamesNothing Posted at: 2018-07-12T22:20:21.674Z Reads: 194

```
"sweet" welder :smiley:
I love this kind of builds where ppl build things to build other things to put in things they're building! keep up the good job!
```

---
## \#223 Posted by: moon Posted at: 2018-07-12T22:24:39.945Z Reads: 197

```
Unfortunately not, I wish I did, but I am working on my gear drive and my own esc 6. But I can't complain, I like learning and designing new things, so in the meantime wont bother me.

I hope the welder works for you, and me :slight_smile:

All I am really waiting for is those junction connectors :)
```

---
## \#224 Posted by: RedEagle Posted at: 2018-07-12T22:51:35.667Z Reads: 185

```
[quote="legend27, post:208, topic:53111"]
**P2: SWD** : No idea
[/quote]

P2 is for programming.
```

---
## \#225 Posted by: moon Posted at: 2018-07-15T00:33:07.913Z Reads: 185

```
Made a pretty cool contraption with the things I had at home. Just need to find some copper nails because the things I was using before we're not good enough.

The contraption includes 5.5mm bullet connectors and m4 screws, and a bunch of tape. I'll get some pictures later
```

---
## \#226 Posted by: moon Posted at: 2018-07-15T12:51:21.713Z Reads: 213

```
![IMG_20180715_121430|375x500](upload://z9MWgKJiJEUPiHVqSYG2CQ3tkj5.jpg)![IMG_20180715_134841|375x500](upload://tAHLXZ3ZUxpMgJZ9V2AEaMSioQY.jpg)![IMG_20180715_134935|375x500](upload://2tGxc1QmziUBgfvuNNpZmJ9txVW.jpg)![IMG_20180715_131119|375x500](upload://m2GpwTHJcOXDs1eV8AJIKh6CofL.jpg)![IMG_20180715_131233|375x500](upload://j2BNyb3l9sYKunULdTMRGDHbm9e.jpg)
```

---
## \#227 Posted by: legend27 Posted at: 2018-07-16T23:06:06.264Z Reads: 212

```
**UPDATE #41**
-
Hi everyone! @moon Finally got my spot welder working yesterday!

I ended up spending $135 in total on the spot welder. You can get the Sunkko 787A+ spot welder for $140 incl. shipping.

**PROS:**
* Can be cheaper than a finished spot welder.
* You become really happy when it finally works.

**CONS:**
* Same price as a not DIY spot welder if you don't have a car battery.
* Not programmable 


![IMG_3094|666x500](upload://8gSUIqsVw5e562iEqgQU5YIelNl.JPG)

![IMG_3097|666x500](upload://AlWep93j86EolBF5wQQ0aZTHZll.JPG)

![IMG_3098|666x500](upload://iDyIuspcdi1wtnhUQW5TkpZBKGT.JPG)

![IMG_3096|666x500](upload://wigbnagC5H1raUtV28spqWRFt8W.JPG)

![IMG_3095|666x500](upload://lzz8VtRkNIYRWQV1PQmV9SpR8PQ.JPG)


Here is a video of a really bad weld. Forgot to take a picture of a good weld...
https://www.instagram.com/p/BlQ9QpagcPg/?taken-by=legend271_
```

---
## \#228 Posted by: moon Posted at: 2018-07-16T23:23:13.076Z Reads: 199

```
Thats sick!

I decided to ditch the spot welder arm for now, if I start making more battery packs I will just put it back on.

I tested my spot welder with really shitty tips I could find and it worked too, I am just waiting on copper nails that I bought from ebay.

[quote="legend27, post:227, topic:53111"]
**PROS:**

* Can be cheaper than a finished spot welder.
* You become really happy when it finally works.

**CONS:**

* Same price as a not DIY spot welder if you don’t have a car battery.
* Not programmable
[/quote]

Agreed, you can always find the parts that you need to fix it too. For example just stock up with a spare solenoid, buy it from aliexpress it only costs a couple of dollars.

You could also implement an timer.
```

---
## \#229 Posted by: rey8801 Posted at: 2018-07-17T03:26:43.092Z Reads: 188

```
Nice! I like the solution you came up with. My DIY spot welder was really ugly. In my defense I was in a hurry to start building and I used parts I ready had it :joy: 
Now time to build your battery pack! Which battery are you gonna make?
```

---
## \#230 Posted by: legend27 Posted at: 2018-07-17T10:27:48.006Z Reads: 182

```
10s6p Samsung 30q 648wh - 28.5cm X 13cm X 3.8cm
```

---
## \#231 Posted by: rey8801 Posted at: 2018-07-17T10:31:06.697Z Reads: 179

```
Limitless range. Cool!
```

---
## \#232 Posted by: legend27 Posted at: 2018-07-17T10:33:14.092Z Reads: 181

```
Yea almost. And you went for a 10s3p? How far can you go on a charge?
```

---
## \#233 Posted by: rey8801 Posted at: 2018-07-17T10:42:55.050Z Reads: 182

```
The specs say 29 km, but I would say that with my set up and I going full throttle as much as possible, plus some hills, I reach 20km at 20 left battery so not that much left. If you cruise normally then closer to 30 is possible. 6p is a lot yuu can always think at 11s to gain a bit more power or 12s.
```

---
## \#234 Posted by: legend27 Posted at: 2018-07-20T18:50:53.403Z Reads: 204

```
**UPDATE #42**
-
Hi everyone. Today I ordered some more parts...

**Aliexpress:**
* **1x $7.99** - [Battery charger](https://www.aliexpress.com/item/NEW-LiitoKala-lii-100-lii-202-lii-402-1-2V-3-7V-3-2V-3-85V/32813235933.html?spm=a2g0s.9042311.0.0.27424c4dfL36o0)
* **1x $2.56** - [Washers](https://www.aliexpress.com/item/M3-M4-M5-M6-M8-M20-Large-Flat-Washer-304-Stainless-Steel-Big-Metal-Gasket-Meson/32847105986.html?spm=a2g0s.9042311.0.0.27424c4dfL36o0)
* **1x $3.02** - [Ski googles](https://www.aliexpress.com/item/1pc-Skiing-Eyewear-Ski-Glass-Goggles-5-Colors-Snowboard-Goggles-Men-Women-Snow-Glasses-Ski-Googles/32595462231.html?spm=a2g0s.9042311.0.0.27424c4dfL36o0)

I also received my dual lock :+1:
![IMG_3074|666x500](upload://5R6eJV9Zhnc3wexwKrZ8O9vyrF7.JPG)![IMG_3073|666x500](upload://fPphGcHbzu1nymJMBKPslx3UbyE.JPG)

![IMG_3072|375x500](upload://vFWF37W8Jp7G8npU4HxNLA1C10a.JPG)

--------------

**NOW TO THE COOL PART!!!! (it's really cool)**
-

Yesterday I went to the library (yea.. belive it or not) to get a belt cover 3d printed ([link for belt cover on thingiverse (I printed the Cover_Final.stl file)](https://www.thingiverse.com/thing:2246770)). They got 2 really cool 3D printers (Ultimaker 2 and Ultimaker 3 extended). I payed $5 for it and it's made out of PLA (plastic). It took 8 hours to print. It didn't fit with the 90mm wheels so I had to cut a bit off. Now that it's all good it looks amazing. Really happy about how it turned out! :slight_smile:

**BEFORE CUTTING:**
-

![IMG_3165|666x500](upload://w77Ce1vP0Udl7ZJu1HqoxrO9orh.JPG)

![IMG_3168|666x500](upload://vGCGzg9EAz7OlWFdBpoIZx1o9H9.JPG)

![IMG_3167|666x500](upload://aAWYGAgLktyxcqxomHsVreWphZ0.JPG)

![IMG_3166|666x500](upload://2tFAbz6gXpjlIHJfGQUTWqSuD15.JPG)

![IMG_3172|666x500](upload://rnDbhamU1wgIsbXWepRjvhd5Svg.JPG)

![IMG_3169|666x500](upload://vvJvKcTWjtUxcxXoODmNdx5frfS.JPG)

![IMG_3171|666x500](upload://y6PXaCHKRZfY3qhM2OOrJUfoIkJ.JPG)

**AFTER CUTTING:**
-

![IMG_3174|666x500](upload://4T91lZMhaZ4YGLs0pt1B8kB3AxP.JPG)

![IMG_3173|666x500](upload://ia92MD9YCIo7ptg6m8fdXNYQIBL.JPG)

![IMG_3176|666x500](upload://8QDfu9WWkJTnqCi8xg0umr1y5J2.JPG)

![IMG_3175|666x500](upload://n1yKBsfRBTxqMUCiBFAtIwKXv89.JPG)

![IMG_3178|666x500](upload://sk4LgLMBLhWW7K3MqHbK6qzNr99.JPG)

![IMG_3177|666x500](upload://3LwEAmWea4evPcYxBTaYfXx04v0.JPG)

![IMG_3179|666x500](upload://qTyhUTecCcZc8Az1adCU7KXVbFE.JPG)

-------

**And here are some updated pictures of the board:**
-

![IMG_3187|666x500](upload://gbpYhz9jbSaI1y6VHofgkPusEK4.JPG)

![IMG_3181|666x500](upload://q8Gc2BMOOyRMsm1JtEoysK29BwH.JPG)

![IMG_3186|666x500](upload://SJqQG27IZoEvWy1JK5ONHvVYjG.JPG)

![IMG_3183|666x500](upload://xG9ZtDuTwvXlY6kLSYSuwu4X1Yx.JPG)

![IMG_3184|666x500](upload://kZoIRgHxazUPwO48pO22LXoLRY0.JPG)

![IMG_3180|375x500](upload://elJlzkEBg0fNGFHosooarfof0Gb.JPG)

![IMG_3185|666x500](upload://gwEkavlalM3EB3ObCZ29L35Tv6v.JPG)

![IMG_3182|375x500](upload://hrm8K5s02rbyslhT6n0jMEvqAMy.JPG)
```

---
## \#235 Posted by: JamesNothing Posted at: 2018-07-20T20:46:29.066Z Reads: 191

```
that's a great print! 8hrs @0.1mm layer height? I printed mine @0.2mm to gain some time, but 100grit sandpaper, some filler primer and 600grit wet sanding and black paint got me at this point.![IMG_7678|375x500](upload://irT4IOOrWKww4X4YV02ZVioNNPp.JPG)![IMG_7679|666x500](upload://tbw9bXvG5aLS2mF6Fb4VzMq6O1Q.JPG)!
and then I hit a rock with it :frowning: I think I'll probably reprint it in some black pla and anneal it to make it more resilient or I'll have it made by my business in sls nylon eventually 

![IMG_7680|666x500](upload://lPWiPEQzFCMBQl1YsNiZED5wAeI.JPG)
```

---
## \#236 Posted by: legend27 Posted at: 2018-07-20T21:11:18.417Z Reads: 179

```
That looks good! Yea 0.1mm layer hight :slight_smile:
```

---
## \#237 Posted by: JamesNothing Posted at: 2018-07-20T21:32:26.524Z Reads: 182

```
It came out really smooth, but I don't really like the model. I'll get a different model next time or I'll make it myself Your model is much nicer than the one I printed.
with 0.1 layers I think you can skip the 100 grit and o straight to high build filler primer and 600grit wet sanding. Then 2-3 layers of paint and voilà! approx 1hr of work in total if you're really slow :smiley:
```

---
## \#238 Posted by: legend27 Posted at: 2018-07-20T21:59:22.174Z Reads: 178

```
I'll paint mine when my build is done and I got some money in spare. Thanks for the guide!
```

---
## \#239 Posted by: moon Posted at: 2018-07-20T23:03:07.222Z Reads: 176

```
How did you solve this?

I know that usually all the problems come from the copper tips
```

---
## \#240 Posted by: legend27 Posted at: 2018-07-21T07:49:00.497Z Reads: 178

```
I think it was the copper tips. After making the pen everything worked. Think it might have been bad connection.
```

---
## \#241 Posted by: moon Posted at: 2018-07-21T15:26:12.751Z Reads: 182

```
Ok I guess I will wait for the junction connectors before I make any other changes
```

---
## \#242 Posted by: legend27 Posted at: 2018-08-01T20:19:48.628Z Reads: 185

```
**UPDATE #43**
-
Hi everyone!
I just ordered the last parts for my board today!

**FINALLY!**
-

Nkon.nl didn't have any nickel strip or battery insulators in stock so I had to order it from eskating.eu. They will have more in stock on 22. August. I didn't wanna wait that long time (obviously lol?)

**NKON.nl:**
- **65x $278.93** - [Samsung 30Q 3000mAh](https://eu.nkon.nl/samsung-inr-18650-30q-3000mah.html)
- **3x $6.82** - [Fish paper adhesive](https://eu.nkon.nl/isolatie-papier-blank.html) 

**Eskating.eu:**
- **4x $13.94** - [1 meter 10mm X 0.15mm Nickel strip](https://eskating.eu/product/pre-cutted-pure-nickel-0-15mm-10mm-various-size-tailored/?attribute_quantity-length=1meter)
- **2x $4.64** - [Fish paper for positive battery](https://eskating.eu/product/insulation-paper-positive-1x-sheet-of-40pcs/)

**TOTAL: $304.33**
**AND THE FINAL COST OF THIS BUILD INCL. TOOLS (didn't have any in the beginning): $1850ish**
-

All there is left to do is wait and then BUILD!
```

---
## \#243 Posted by: moon Posted at: 2018-08-02T19:16:01.334Z Reads: 181

```
Well the final part for my spot welder came today so I decided to test it out. It was a little frustrating at first, but every issue I came across was to do with the copper tips.

So after experimenting a little I spot welded single layers on both sides of my cell. I can do it really quick now, no problems - except that I can't get a solid two layer connection yet. Probably to do with the tips, they kept wearing out for me which is annoying.

But I think I am going to buy/make those 18650 PCBs to save some headache as I have to make another pack after this.

I don't know why I post on this thread lol. But its the first thing I think of when I have done something with my build
```

---
## \#244 Posted by: legend27 Posted at: 2018-08-02T19:46:12.481Z Reads: 168

```
Nice to hear that it actually works! The tips also wear out for me. I tried sanding them a bit to make them more flat and that worked. When I get my nickel strip I'll try to put to on top of each other and see if it works for me. What PCB's are you talking about?

What battery do you have?

Good luck!
```

---
## \#245 Posted by: moon Posted at: 2018-08-02T19:52:11.244Z Reads: 188

```
I have 30qs and 25r, making two packs. 

Tips wore out very quick and sanding didn't really help. But I am using slightly thinner copper nails than you. That could be the issue too.

I couldn't really get any good welds nickel to nickel. But battery to nickel had no issues apart from copper nails.

![image|637x500](upload://xrY2FGOeqTZ1t2eGVUFt5wvkoeP.jpg)
![image|375x500](upload://qV5tD7KxM0u22LEl8ZyfViUtF6s.jpg)

Pictures from @Rob69de
PCB made by @Kug3lis  


![image|375x500](upload://84tzu2PyA5IVQeiA5058HHbPucx.jpg)

![image|375x500](upload://mbNzhXSm9NIL9Uj1VNWR5EilF83.jpg)

![image|500x500](upload://bbwd2Adpk3NzaYCeGyO6QLSDkli.jpg)

I think the original idea was from @Blasto and I should probably ask him some questions if he is kind to answer  :star_struck: 

Many people have designed a PCB like this. I need to do more research first though- the positives the negatives. Whether I can use 12/10awg to solder the pcb to the cells ( i got some sexy looking 12awg wire so hoping I can use that).

 The PCBs are super cheap so hoping someone needs them since shipping is not cheap lol. I will be ordering 20 for myself, probably some extra and then hopefully someone is also interested in this cool idea.
```

---
## \#246 Posted by: legend27 Posted at: 2018-08-02T20:01:34.068Z Reads: 170

```
Ahhh those. I meant what car battery do you have? And do you have a picture of your welds?
```

---
## \#247 Posted by: moon Posted at: 2018-08-02T20:06:19.119Z Reads: 170

```
Ill get some pictures really soon.

So with the copper nails I would get ugly looking welds but functional - but unreliable 
Switched to those thick copper strands and I got reliable welds and cleaner welds. For the second layer, it would stick but I could still pull it apart.

265amp car battery, made by the same company as yours. https://www.tayna.co.uk/car-batteries/bulletbatt/054/

Problem could probably be solved by holding onto the button for a little longer. Thats another thing, I saw that video that darkkevind made and he was emphasising the importance on pressing the button quickly. I felt like a pro when I was doing that, no issues there :laughing:
```

---
## \#248 Posted by: legend27 Posted at: 2018-08-02T20:10:48.246Z Reads: 167

```
Be careful if you hold the button a little longer. It makes the battery hot.

The problem could maybe also be your car batterys amps? My battery has 340 amps. Ill give you an update when i get my nickel strips.
```

---
## \#249 Posted by: moon Posted at: 2018-08-02T20:13:44.511Z Reads: 163

```
Could be the battery, but darkkevind was using a weaker battery than mine in some of the videos.

I am not bothered if it can do 1 layer reliably since those PCBs were on my mind before today.

Yeah sometimes I would make the battery a little warm, I wouldnt say hot though
```

---
## \#250 Posted by: moon Posted at: 2018-08-02T20:40:05.856Z Reads: 165

```
Actually I forgot about this, I did make double layers quite easily with new copper tips on thee negative side. Then I realised I don't need to to do that. And I couldnt get the copper tips close enough because the junction connector was so wide
```

---
## \#251 Posted by: moon Posted at: 2018-08-02T21:19:24.701Z Reads: 190

```
![IMG_20180802_164828|375x500](upload://eLucBEUOyJeQEwuRjPUjn06ZP93.jpg)![IMG_20180802_205725|375x500](upload://jilKF4FgHGsxhMNaElFrdwcfvRT.jpg)![IMG_20180802_151130|375x500](upload://iHdbXdxx2YI8h5UA7aUfzccMMjo.jpg)

What i found on my phone - the last picture was my first weld
```

---
## \#252 Posted by: legend27 Posted at: 2018-08-04T18:18:00.119Z Reads: 177

```
Hi again everyone. Quick update. I bought way less nickel strip than I need. I ordered 4 meters and after some math, I figured I'd actually need 11 meters. I contacted Alberto and ordered some more so now it's all good. Just want everybody to know that you are probably going to need more nickel strip than you think. DO THE MATH! I ended up getting 13 meters in total. Can't belive i've spent $45 on fucking nickel strip lol.
```

---
## \#253 Posted by: legend27 Posted at: 2018-08-06T21:53:26.523Z Reads: 191

```
**UPDATE #44**
-
**_Before 06-08-2018:_**
Received parts.
![IMG_3188|666x500](upload://d6xAxjCdvQeLtfRDorqAcvt3zTt.JPG)

![IMG_3189|666x500](upload://aao1oEXLiDj9dujcYOktoJKSyz3.JPG)

![IMG_3190|666x500](upload://wIGfPgEwqNjCxj9BrFwV14KIvEn.JPG)

------------
Made HM-10 bluetooth module.

![IMG_3192|666x500](upload://6HF8PcNcefsZMCQYIY9B4b9UhPh.JPG)

![IMG_3193|666x500](upload://8alTQmOsbki7FVyL9uBoKlLsZaR.JPG)

![IMG_3194|666x500](upload://hJg0UHYsLsUh8BZ6J5A5gFQEYA8.JPG)

![IMG_3191|375x500](upload://aiLR4CyKWfl8IY3ojOjM6qjo6tc.JPG)

------
Put some cable sleeves around my motor cables

![IMG_3239|666x500](upload://wcPlC0jNK33TgwLkKwFHTdkG9lk.JPG)

-----------------

**_06-08-2018:_**
-
Hi everyone!
Today I received my batteries and started working on my battery. My nickel strip got shipped today so i'll probably have it in 3-4 days! I would appreciate if I could get some feedback on my battery design :slight_smile: 

----
Crazy unboxing
![IMG_3218|666x500](upload://r4YSJdjdJGBMKH9uiDU2fAaeXGC.JPG)

![IMG_3220|666x500](upload://2c0SZSaveEtkHbua0nElXkyClXQ.JPG)

![IMG_3219|666x500](upload://oH5W2BOXNNXM7cnxFRYrjiOEMGA.JPG)

-----
Measured all battery voltages. They were pretty close to each other (3.41V-3.43V).

![IMG_3223|666x500](upload://du7vZcwFmi3Ds2AXHQ2B2QxxFZ1.JPG)

![IMG_3221|666x500](upload://clo533h86mGaW5bPFazsb3FLMHO.JPG)

-----
Realized I had got some other parts. I did the "try to lit the fish paper on fire by holding a lighter under it" test. The fish paper from ali lasted the longest but I don't think the adhesive is that good.

**I used the battery insulators from ali on my batteries and they started to fall off. Is that normal or should I get some new battery insulators?**
-

![IMG_3226|666x500](upload://kou2wO0p7j46JZ7XXEL4L4bKUle.JPG)

([Fish paper from aliexpress](https://www.aliexpress.com/item/1m-120mm-18650-Battery-Insulation-Gasket-Barley-Paper-Li-ion-Pack-Cell-Insulating-Glue-Patch-Positive/32827522392.html?spm=a2g0s.9042311.0.0.a6164c4dia7FQp))
![IMG_3225|666x500](upload://97Mn76sGlDXpbeJUzvJvrYEyPVW.JPG)

([Fish paper from eu.nkon](https://eu.nkon.nl/isolatie-papier-blank.html?___SID=U))
![IMG_3224|666x500](upload://1O34APPEiiKMVuu2VatGNmWIEMz.JPG)

--------
Put the battery insulators on the positive site of the batteries. The fish paper started falling off? As mentioned above: Is that normal or should I get some new?

![IMG_3228|666x500](upload://q4wsmzfQzRV0kEPjlFSby61tP2Y.JPG)

![IMG_3230|666x500](upload://drq7UfCwRenHJdHlaoJgsty9rFY.JPG)

--------
Glued all cells together in packs of 3. All the cells fitted in the enclosure! really nice :+1: 

![IMG_3231|666x500](upload://oh79T7SpnQle0wsfucr4AFjq6ot.JPG)

![IMG_3233|666x500](upload://jNWn8YwWolecp5WwWNoCsjzoPkc.JPG)

-----------------
Glued all the packs of 3 together in packs of 6.  Really nice! Did some more test fitting with all the parts.

**Im going to put fish paper around my parralel packs. Is that stupid? Should I use kapton tape instead?**
-

![IMG_3236|666x500](upload://lr77qgPjJyvbqvDZH0joYK4qxEH.JPG)

![IMG_3237|666x500](upload://eZcujVVkgbghQxTTObRJFwUgDEP.JPG)

--------
Also got a new helmet today. I like it! REMEMBER TO USE A HELMET!
![IMG_3241|666x500](upload://ieCO85qH2ODPkTjILeQYRK29gMo.JPG)![IMG_3240|666x500](upload://8nmzo4FDBC2qKflhoQA98I0GzIc.JPG)
```

---
## \#254 Posted by: legend27 Posted at: 2018-08-22T18:05:18.661Z Reads: 182

```
**UPDATE #45** 
-
It's been a while. It's time for an update.
Ditched the DIY spot and bought a Arduino Spot welder for $185. It arrived yesterday and it works great. Much easier to handle and im not afraid that the battery explodes.

![IMG_3286|666x500](upload://sVSeHmJ8phxyDQkne6hvnWrPZjf.JPG)

![IMG_3287|666x500](upload://t4ziFm6nn7fVUNpymP9fHsuh1bn.JPG)

![IMG_3288|666x500](upload://KWrv5nOWcUGvwhzitInbYDhNcz.JPG)

![IMG_3290|666x500](upload://blfSQRFe7X2F24wiGkc9Ru2gSYC.JPG)

![IMG_3285|666x500](upload://umTDtI5LZYcmt3xVPLEXg3CZ76k.JPG)
(This came in the box as protection. love that he actually filled all the words in :smile:)

Today I used the spot welder to weld all of my packs. They are not done yet because I got some problems welding nickel to nickel.

I used 24ms when welding nickel to battery (steel) and 55ms when welding nickel to nickel. I think 55ms is a bit too much because I blew a hole in the nickel strip and I had to pull it off.

I also tried setting the pulse time to 47ms and it worked much better (no explosions) but im afraid the welds won't be strong enough.

Ended up stopping after the nickel strip exploded so I wouldn't fuck anything up in my "WHY DOES IT NOT WORK?!?!" mood. Glad I did that.

My plan tomorrow is to complete all the parallel packs and then I'll see how much time I've got left. Hopefully the board will be done in 2 weeks (hopefully before lol). Thanks for reading till the end and following my build thread. Enjoy some pictures of the welds.

![IMG_3292|666x500](upload://iiftGjrHVfzU0aecoc3h8cbNp1b.JPG)

![IMG_3293|666x500](upload://pEquwMr25uwVVN6Z9Iz5rIKmR3n.JPG)

![IMG_3291|666x500](upload://sGfVGwblW183RQteKggrXACf3NG.JPG)
```

---
## \#255 Posted by: legend27 Posted at: 2018-08-23T18:52:35.329Z Reads: 175

```
Quick and irelevent update. Isn't that what this forum is used to?

Got all my packs welded done today. I used 47ms and the welds seem pretty good. Think I shorted a cell really quick cause it made a spark. I put a lot of pressure on a nickel strip to see how strong the weld was and there came a spark. Measured the volts and no damage was made.

Thanks for reading.

![IMG_3296|666x500](upload://nl5D4CPWSnywJ66L0ucKVNfJerm.JPG)

![IMG_3295|666x500](upload://zurXEOJ8UUBniJxb9qSY6WQegEF.JPG)

![IMG_3297|666x500](upload://vEkdZs82QjAe27ShqryrzxtmshP.JPG)

![IMG_3294|666x500](upload://oHBunMMudajWc8SqKd8uZlfMRaI.JPG)
```

---
## \#257 Posted by: legend27 Posted at: 2018-10-03T15:42:26.879Z Reads: 173

```
Okaaaaaay... I've made very little progress but it's time for an update!

**UPDATE #46**
-
Glued my pack together, put some tape around it and cut some nickel

![IMG_3303|666x500](upload://rIRtADEn7SoI2mqwuWYb050cgMR.jpeg) 

![IMG_3310|666x500](upload://sSzPBXF4Tc2zWYX9XmwN3MJV2WM.jpeg) 

![IMG_3311|666x500](upload://lcfQA7zBuJQkFV5wtIkMSL1LhIQ.jpeg)

My old 340A car battery was not strong enough to make good welds so I had to get a new one. Got this for free but turned out it lost too much power after each weld. The welds was also not strong enough.

![IMG_3331|666x500](upload://pjwkD60zC8nEWbYzNk5Dpv6OmgO.JPG)

![IMG_3321|666x500](upload://hhbIg38TY7nhgudyKlzuUFEmU3p.jpeg) 

Okay. Got a new big 700A car battery! NOW WE'RE WELDING! right? Well, turns out the battery had a lower output than 700A. Great! I have sent it to repair and I am currently waiting to get the battery back or a new one. They said a week, but it's now been 8 days and no battery. Enjoy the pictures :slight_smile: 

![IMG_3335|666x500](upload://wVOVJNfaaxEil8ZcjIaV7oj3WH7.jpeg)

![IMG_3337|666x500](upload://4wB3STqxyrlKXxE5HbGxDM0EQXf.jpeg)

![IMG_3340|666x500](upload://7LVPXWH7regQmjKZsSZg2Zxjdhw.jpeg)

![IMG_3341|666x500](upload://fn9BmB2btuf5o93QJPCIgQTmCmH.jpeg)

![IMG_3344|666x500](upload://1XHFKiRw7VVBvS7QBxgTYgufLBj.jpeg)

![IMG_3353|666x500](upload://uqgRhelc6tHvsYxXHUM5LJvXDpC.jpeg)

![IMG_3355|666x500](upload://aPvfLVFPXjGTASV7OytzYYedhRO.jpeg)

![IMG_3366|666x500](upload://34C5OHrjjc2qNdZgMjSCFpPBuqd.jpeg)

![IMG_3367|666x500](upload://x2hpd8JoegSA82gKbHj7eS1X95a.jpeg)

![IMG_3368|666x500](upload://27TYoo4212cgzpJNqtNhZ97kXl7.jpeg)

My original plan for the series connections looked like that

![hard2make|666x500](upload://wUzbGS6EFl9ETqZvJ2h1ugbxEw5.jpeg)

They were pain in the ass to get perfect but I found a solution. Just lay them like this instead. Much easier!

![easy2make|666x500](upload://dH4OVVf1hFVHHwaSVGUbF40MalV.jpeg) 


Ohh yea.. Also shorted my battery. Think everything is fine. The nickel strip acted like a fuse. Just some burn marks.

![IMG_3377|666x500](upload://7K7EgvUK58LrGSHuU2MFfl9vsWy.jpeg) ![IMG_3378|666x500](upload://k80HL425d6hmGKVGyLVDCyqIb31.jpeg) 

To avoid the same thing happening to you always insulate positive and negative. If it had been the main leads it would probably had started a fire. I was lucky. Learn from other peoples mistakes and when you think "it's not gonna happend to me" it is going to. As good old friend Crazy Russian Hacker says "Safety is number one priority"

![IMG_3379|666x500](upload://s9mqDvUb0OKSGeE17QXzhVujmk3.jpeg)
```

---
## \#258 Posted by: legend27 Posted at: 2018-10-04T15:42:19.067Z Reads: 155

```
**UPDATE #47**
-
Finally got answer from where I bought the car battery. It got denied and they told me nothing is wrong with the battery. Great... Can't get my money back from the car battery and it dosen't work properly.

What im going to try and do now is see if the spot welder is broken. I don't think so but it's worth it trying. I've messaged a couple of guys on the forum about their car battery specs to contradict the shops claim that the battery is fine and to have some kind of proof.

Luckily I still have my old 340A battery and im pretty sure I measured the amps to be 380A. Which is 40A over the rated. Which means that if thats still the case, the 700A battery is broken and the spot welder works fine. Great!

Thanks for reading and remember to never let the challenges stop you.
```

---
## \#259 Posted by: legend27 Posted at: 2018-10-29T19:25:02.484Z Reads: 162

```
**UPDATE 48**
-

Time for an update! Only 25 days since last and no progress made on the skateboard!

So what has been going on?
Well I placed an order on Amazon for a new car battery and it said "Usually dispatched within 2 to 3 days" and me be like "great! I get a battery from a well known source and I will have it in a few days. Two weeks later without the battery has been dispatched I contact them and gets told "we have some problems with our system so the item is not actually in stock and we don't know when it will be again". GREAT AMAZON! THANKS FOR WASTING 2 WEEKS WITHOUT EVEN TELLING ME ABOUT IT! 

Then I needed to find another place to buy the battery. Luckily the place I bought my 340A battery (Tayna Batteries) had it in stock and shipping time was only a few days. On October 24. I bought the battery and I received it today. It was well packaged and had no acid in the bag. Voltage was 12.56V.

![IMG_3440|666x500](upload://84ipgo1Sl7p5lkvCvXvVCv5Uw5R.jpeg) 

![IMG_3442|666x500](upload://bI1bzVzCymjcosq4GJb2ptCPzgn.jpeg) 

![IMG_3443|666x500](upload://lue4pKiPVFij3gOexf9GC4AwlIv.jpeg)
```

---
## \#260 Posted by: legend27 Posted at: 2018-11-09T22:51:26.114Z Reads: 154

```
**UPDATE #49**
-

Finally! Got my pack welded and connected. The motor run! Still haven't hooked up the bms and shrink wrapped it.

![IMG_3493|666x500](upload://rNAjgmYR3ObZbzpDzjKSMdrM2W1.jpeg) 

![IMG_3504|666x500](upload://xUuhBGiylnGvxJCdMx37xY4MBpZ.jpeg) 

![IMG_3502|666x500](upload://iJ5sZYFxigHRiBf24CZSAdLx0tU.jpeg) 

![IMG_3509|666x500](upload://g7bplIxDcHa1yPk3GRoan4pFwiP.jpeg) 

![IMG_3511|666x500](upload://gr6iLTaWlb8WCRpTJYw5C03wXlK.jpeg)

 ![IMG_3513|666x500](upload://h8xANPi477gADzJrI97vLefRJ6D.jpeg) 

![IMG_3515|666x500](upload://tjhxMZmljSOgPaIvDKND6r5Zy5V.jpeg) 

![IMG_3517|666x500](upload://t1CYS1yslwKMIVl3EuHaQEj1mCH.jpeg)

 ![IMG_3518|666x500](upload://1BlbVLWgQPejCQkbRwjWniT7wY6.jpeg) 

![IMG_3524|666x500](upload://mvSZKrRpmi1YnLnDuiVhSQuFwk8.jpeg) 

![IMG_3520|666x500](upload://sSCExaLUyv7tShrk079TCVmK7lD.jpeg)

 ![IMG_3485|666x500](upload://uqQLNj65CTseGnmxXZ6E5rxYdf4.jpeg)

 ![IMG_3491|666x500](upload://xdEk5cT7poWIHWjRaSWZTa9JXpE.jpeg)

 ![IMG_3487|666x500](upload://99pIp25ue370LUDFFTEBgDPZJGM.jpeg)

 ![IMG_3532|666x500](upload://rtZeMriTPE19JILfYfRnW3epW16.jpeg) 

![IMG_3486|666x500](upload://b5LaH3IS0b7QZNF95dP6Qt8wRnj.jpeg)

 ![IMG_3534|666x500](upload://kVcWYzFLF7hFMrbBlKuI0QIOnIm.jpeg) 

![IMG_3523|666x500](upload://bqRJSGTVxzpmVx82jC8RonSimD3.jpeg) 

And today I finally turned on the board and tested the motors.

Video: https://instagram.com/p/Bp-chgYhjyu/

![IMG_3537|666x500](upload://tAg3sL17xwCDWxumvxmA7hrBzxW.jpeg)

![IMG_3541|666x500](upload://fjvotLxZCecLOfdNIqCJSC0xRtt.jpeg)
```

---
## \#261 Posted by: legend27 Posted at: 2018-11-10T17:17:48.604Z Reads: 153

```
**UPDATE #50** 
-

Got my vesc set up and WOW! It's much more powerful!

(Not even close to full power :smiling_imp:)
https://youtu.be/RCxMl-TYf-c

Got my BMS connected but can't charge the battery yet. The charger outputs 42.4V and pretty sure that's too much. I've sent an email to Alberto and will hopefully will get an answer tomorrow. 

![IMG_3543|666x500](upload://i6EBq9wrfcEojDYA2eGRHOgQLQL.jpeg) 

![IMG_3544|666x500](upload://9VSVm4IYe0dJG9axngMqWL2Abbt.jpeg) 

![IMG_3545|666x500](upload://jDQXhpHLfkUIAnZc2uhgcjAxP0G.jpeg) 

![IMG_3546|666x500](upload://aQ14hcXloxjJMLnTp18iqocjjvA.jpeg) 

![IMG_3542|666x500](upload://9s8IPfKeM8bm4CHidxNJCMLmrC0.jpeg)
```

---
## \#262 Posted by: legend27 Posted at: 2018-11-10T17:28:55.203Z Reads: 150

```
Wait... Just realized one thing. When the charger outputs 42.4V each cell will be at 4.24v fully charged, correct?

> 3. Standard charge: CCCV, 1.50A, 4.20 ± 0.05 V, 150mA cut-off

That means each cell potentially can be at 4.25V safely?

Which means the conclusion would be that the charge output is correct and the battery pack won't be overcharged?

edit:
The BMS has a overcharge voltage detection of 4.28V. That means the charging will be interrupted when the voltage of a cell exceeds 4.28V. The 30Q max charge is 4.25V, doesn't that mean the cell will be damaged before the bms turns off?

![IMG_3552|645x500](upload://iGADm4taycDNsB1MXoXmf0bYk1M.png)
```

---
## \#263 Posted by: legend27 Posted at: 2018-11-10T18:58:42.538Z Reads: 144

```
I turned on the charger. And look at that! It's charging! I will probably turn it off when it reaches 40V.

![IMG_3554|666x500](upload://oZDVwMAvZSM96bDlSD772Ppaf3m.jpeg)
```

---
## \#264 Posted by: Sn4pz Posted at: 2018-11-10T19:35:18.358Z Reads: 135

```
I think you should be fine*, but ill bump for more opinions :)

*as long as you use that charger specifically, as its set to 42.4
```

---
## \#265 Posted by: pat.speed Posted at: 2018-11-10T21:08:48.662Z Reads: 135

```
It will be fine, it most likely won’t even reach that voltage once under load. I would expect it to reach 41.9-42.1v. I know that my adjustable charger I set to 50.5v and my 12s gets balance perfectly to 50.4 once removing the charger
```

---
## \#266 Posted by: Sooty Posted at: 2018-11-10T22:41:13.404Z Reads: 132

```
European building seems to be a lot more expensive than in the USA. I'm in the UK and these extra taxes and shipping fees look prohibitively expensive!
```

---
## \#267 Posted by: brenternet Posted at: 2018-11-10T23:26:40.380Z Reads: 135

```
I did the math recently and on my first build, after making a few mistakes and ordering most items from overseas I ended up spending over £700 on shipping, import taxes and fees.

There are some pretty decent builds on the forum for £700 haha. We get abused.
```

---
## \#268 Posted by: Sn4pz Posted at: 2018-11-10T23:37:07.335Z Reads: 130

```
thats fucked :sweat_smile: :laughing:

buy a plane ticket and come pick them up by hand :P
```

---
## \#269 Posted by: lrdesigns Posted at: 2018-11-10T23:43:04.417Z Reads: 132

```
I think it’s normal the BMS should bleed off any extra voltage as heat to balance them down to 4.2. You could check after the first full charge.
```

---
## \#270 Posted by: legend27 Posted at: 2018-11-10T23:50:24.383Z Reads: 139

```
@lrdesigns  Will do!

![IMG_3555|666x500](upload://2mzZPv1oEwOIvgyHPwqvvTJCbA0.jpeg) 

Definitely also need a new charger. 5 hours since I plugged it in and only at 39.3V so far.
Just don't know which one of these two to get. Any suggestions?

https://www.aliexpress.com/item/36V-4A-charger-Output-42V-4A-aluminum-case-charger-Used-for-36V-Li-ion-battery-charging/1731012609.html?spm=2114.search0104.3.3.597f7626zbHSa1&ws_ab_test=searchweb0_0,searchweb201602_3_10065_10068_319_317_10696_5728811_10084_453_454_10083_10618_10920_10921_10304_10307_10820_10821_537_10302_536_5733215_5733315_328_10059_10884_5731015_5733115_10887_100031_5733415_321_5730015_322_10103_5733515_5729015_5733615,searchweb201603_1,ppcSwitch_0&algo_expid=2969d992-cd13-4e07-acf6-7d559df058c2-0&algo_pvid=2969d992-cd13-4e07-acf6-7d559df058c2

https://www.aliexpress.com/item/42V4A-Charger-10S-36V-li-ion-battery-Charger-Output-DC-42V-With-cooling-fan-Free-Shipping/32760909127.html?spm=2114.search0104.3.19.239d7626hYOQob&ws_ab_test=searchweb0_0,searchweb201602_3_10065_10068_319_317_10696_5728811_10084_453_454_10083_10618_10920_10921_10304_10307_10820_10821_537_10302_536_5733215_5733315_328_10059_10884_5731015_5733115_10887_100031_5733415_321_5730015_322_10103_5733515_5729015_5733615-5733315,searchweb201603_1,ppcSwitch_0&algo_expid=3fc549ae-7e7d-44ab-9ff7-b20a67513952-2&algo_pvid=3fc549ae-7e7d-44ab-9ff7-b20a67513952
```

---
## \#271 Posted by: pat.speed Posted at: 2018-11-11T01:23:28.797Z Reads: 134

```
For the same price or cheaper you could buy a cc/cv boost converter and watt meter giving you a fully adjustable charger able to charge any voltage batteries up to 80v and all you need is a 12-24v input supply for powering it. @skatardude10 is using the same thing as me and I think he’s using it for a portable charger.


Here’s a pic of it currently powering a bt speaker im making

 ![image|375x500](upload://owCGbkFmXR1ldq0BkLf8i9hRvnx.jpeg)
```

---
## \#272 Posted by: skatardude10 Posted at: 2018-11-11T01:25:52.287Z Reads: 128

```
Yep, works great! Charging my 10S battery at 4 amps easy, and it's adjustable
```

---
## \#273 Posted by: legend27 Posted at: 2018-11-11T08:20:21.861Z Reads: 125

```
Only problem is I don't have a 12-24v input. I only have a wall socket.

But good idea for road charging or instead of having to buy 2 different chargers for 10a and 12s!
```

---
## \#274 Posted by: pat.speed Posted at: 2018-11-11T08:26:12.297Z Reads: 123

```
Yeah that was my thoughts, I have a 10 and 12s board and to buy two 4-5a chargers it costs about $120
```

---
## \#275 Posted by: legend27 Posted at: 2018-11-11T10:02:49.343Z Reads: 132

```
Still going! Don't worry, didn't leave it on all night.
Going to charge it to 42V and then the next charge around 41V for longer lifespan.
![IMG_3556|666x500](upload://4Dc3R2xSz4mbzvcTZtRnZkSlpMX.jpeg)
```

---
## \#276 Posted by: legend27 Posted at: 2018-11-11T10:59:30.512Z Reads: 128

```
Almost there!
![IMG_3559|666x500](upload://w5kRYxYsPZ9T8WXMNFul9XCVVvX.jpeg)
```

---
## \#277 Posted by: Grozniy Posted at: 2018-11-11T11:24:51.716Z Reads: 125

```
That's what she said
```

---
## \#278 Posted by: legend27 Posted at: 2018-11-11T11:37:45.739Z Reads: 132

```
And it's done. Finally! Only took 9 hours. Glad I bought a new charger.

![IMG_3560|666x500](upload://gUlrm5hF2ihyL8u12oCqjCe5EdO.jpeg)
```

---
## \#279 Posted by: Grozniy Posted at: 2018-11-11T11:41:27.702Z Reads: 130

```
And no explosions
```

---
## \#280 Posted by: legend27 Posted at: 2018-11-17T16:55:18.812Z Reads: 135

```
**UPDATE #51**
-

I fully charged my battery, put some foam on it to make it flat and heatshrinked it. Battery is done (Actually all electronics are done now :partying_face: ).


![IMG_3563|666x500](upload://wZQjbaSaxST5jiDiXc3CqmZxbTs.jpeg)

![IMG_3570|666x500](upload://tRzNwgGQJM95vMI9qfBRzAV4H1Y.jpeg) 

![IMG_3575|666x500](upload://svU6Qn8B6xItHHcsuVQ2VMqwT2E.jpeg)

I drilled and cutted holes in my enclosure. It looks like a smiley :smile: 

![IMG_3567|666x500](upload://n9RGvx4f5d2HB80fCorRshCKX8M.jpeg)

![IMG_3568|666x500](upload://eZzZE5DKUgXtZM44MaXWYxJxpcA.jpeg) 

Mounted everything in the enclosure with velcro and dual lock (vesc and antispark is not in the picture)

![IMG_3584|666x500](upload://yBAFj9oGCZpCowcq3YDkDYcfGIq.jpeg)

![IMG_3583|666x500](upload://yN6PGZNRR0KgJkq4wty0WpzGFD7.jpeg) 

**TO DO:**
- Make inserts to mount enclosure
- Mount enclosure
- Drive

Now the more challenging part. I'm currently trying to put the inserts in the deck. I made 3 holes in the deck but when screwing the bolts in, the pressure on the enclosure is too much and it will crack over longer time.

![IMG_3582|666x500](upload://zDY93T92XNOhTklGDcBkhvoxb2e.jpeg)

![IMG_3580|666x500](upload://7reqoLG8Om5aW0iGoedvMTYRBrt.jpeg)

![IMG_3581|666x500](upload://tE0TWY4tdHnbhV9OAWVYiN5HGaq.jpeg)

There is a medium gap between the deck and enclosure. When the enclosure is mounted down, it will fill in the gap. Don't worry, it's just pressing down the foam on the battery, not the actual batteries.

![IMG_3585|666x500](upload://al6AHKDtuJXuhnKUGJrv3UChDGm.jpeg)
 
![IMG_3586|666x500](upload://qlzh2J1TfShjJRBywTuUT5AXZVP.jpeg)

Luckily for me two of the holes I drilled might actually be okay to mount the enclosure. The only hole that's off is the one in the front. I will have to fill that with fiberglass filler and then drill a new hole next to it.


![IMG_3588|666x500](upload://aiLfR0k66WpplvjzoBsXtHxAM69.jpeg)


Pro tip I saw in another thread:
Screw your insert nuts in with a little slant towards the inside of the enclosure **IF YOUR ENCLOSURE HAVE SOME FLEX**. If they slant away from the inside of the enclosure, a lot of pressure will be put on the thin edge of the enclosure and it will break over longer time.

----

I also have some motor sensor problems. When accelerating really slowly or when putting pressure on the wheels the sensors start acting weird. Does anyone know what could cause the problem?

https://www.youtube.com/watch?v=vJRmkAuGdhs


Thanks for reading all the way to the end and I hope you are having a great weekend!
```

---
## \#281 Posted by: Grozniy Posted at: 2018-11-17T16:58:02.470Z Reads: 127

```
Another option
https://www.electric-skateboard.builders/t/epoxy-pools-of-flatness/48399?u=grozniy
```

---
## \#282 Posted by: murdomeek Posted at: 2018-11-17T17:45:18.184Z Reads: 122

```
love your bike bell mod! XD
```

---
## \#283 Posted by: legend27 Posted at: 2018-11-17T20:48:36.947Z Reads: 124

```
Thanks a lot man! Gonna go with that option instead. I'm gonna make a higher edge on the deck for the inserts and leave space in the middle for battery.
```

---
## \#284 Posted by: legend27 Posted at: 2018-11-18T10:56:43.178Z Reads: 127

```
**Small update**

Im gonna go with the option @Grozniy suggested. It seems easier and I think I will get the best end result. Thanks @Grozniy!

I ordered the same epoxy @squishy654 used. The one he used is only available in the US, but luckily Hobbyking has the same, but from a different brand ([link](https://hobbyking.com/en_us/finish-cure-20-min-epoxy-glue-4-5-oz.html)). I ordered x4 packs so in total 4 bottles of hardener and 4 bottles of epoxy.

I also ordered 25 meters of the cheapest [foam](https://www.aliexpress.com/item/1Roll-200-2cm-EVA-Single-Sided-Adhesive-Tape-Weather-Sticky-Stripping-Sponge-Foam-Rubber-Strip-Neoprene/32818859998.html?spm=a2g0s.9042311.0.0.47bc4c4d5b8WNs) on Aliexpress to make some walls for the epoxy.

Thanks for reading till the end and I hope you are having a great sunday so far!
```

---
## \#285 Posted by: legend27 Posted at: 2018-11-18T12:05:40.676Z Reads: 135

```
Ready for the first ever test ride :smile: :+1:

![IMG_3592|666x500](upload://kW6AgsBT0g2WB1egInJQLGo6j3g.jpeg)

![IMG_3594|666x500](upload://x6iWPWhC5GjiGsuiCVRB3wFShL9.jpeg)
```

---
## \#286 Posted by: Grozniy Posted at: 2018-11-18T12:19:38.610Z Reads: 133

```
Looks totally safe XD
```

---
## \#287 Posted by: legend27 Posted at: 2018-11-18T12:34:57.586Z Reads: 140

```
First test went pretty good. I'm gonna go do a longer test really soon. Is it normal for the TB vesc to make a beep sound when brakeing? See video below.

https://youtu.be/RtoqqC2JDHs
```

---
## \#288 Posted by: legend27 Posted at: 2018-11-18T16:13:06.632Z Reads: 141

```
First real test ride over. Pretty fucking fun and worth all the time I've spent. I rode 7km and still had 94% battery left! I got to 41km/h but I'm not sure how accurate it is. Definitely didn't feel like 41 more like 30. Wh/km was around 9wh. Great!

I got an error the the Xmatic app when trying to save my ride so it didn't save.

The trucks are pretty tight but I am still able to make sharp turns. I also have the kick tail. I didn't get any speed wobbles and felt really safe and secure on the board. Also going 41. Much better than my old board.

After my ride the motor pulley had moved a bit so it made a clicking sound. It also started cutting in to the motor mount. Fixed it pretty easy by cleaning the pulley and screwing it back again with lots of loctite.

![IMG_3597|666x500](upload://2RbvHdf2AgktpRZblq99k2Wjz64.jpeg) 

![IMG_3598|666x500](upload://tSLuTUC8octbkt16jtM4MYrKEdA.jpeg) 

Tightened all the screws. The only one that was loose was the trucks.

edit:
Ohh yea. Nothing fell off even though it doesn't look safe.
```

---
## \#289 Posted by: legend27 Posted at: 2018-11-18T18:43:49.440Z Reads: 139

```
I won't be able to mount the enclosure within the next few weeks so I decided to make it a bit nicer. I actually think it's waterproof :+1: (not gonna test it :joy:)  

![IMG_3600|666x500](upload://dnfsqxKVCAT7yE2SskicB2Qn78g.jpeg) ![IMG_3601|666x500](upload://zbhkvnqM4Sqq5Z2iZdH0IaRCduz.jpeg) ![IMG_3602|666x500](upload://4R4WSqagt3LLJBJdM4r4eMDvpGO.jpeg)
```

---
## \#290 Posted by: legend27 Posted at: 2018-11-22T17:20:52.705Z Reads: 143

```
**UPDATE #52**
-

Took the board for another ride to go and pickup a package. Wow! It's so much fun. I totally forgot the feeling of riding an electric skateboard. Also the reaction from people. A car honked at me and some kids were just staring at me. There was also this smaller girl that yelled something at me I couldn't hear.

![IMG_3609|281x499](upload://zjN57XKO88yzEEUmNKSg1HnQHrw.png)

I went over a lot of bumps and a few bad roads that made a lot of vibrations. When I came home, I opened the enclosure and everything still looked good. Only thing that had moved around was the actual enclosure because it was not mounted that well.

![IMG_3605|666x500](upload://jIVnh3oJZQNy3NJpoN3kclksKQQ.jpeg)

The package contained the epoxy from Hobbyking. I also ordered some LED strips that I will be putting inside the epoxy so I get some really cool light effects. Thanks for mentioning that idea in the "epoxy thread" @squishy654
 
![IMG_3606|666x500](upload://qtcsnoK47n7W1Lrls55dZrzBXTW.jpeg) 

![IMG_3608|666x500](upload://rffbG6q4vzNmVYq26sxqWnNI8m.jpeg) 

Thanks for reading till the end!
```

---
## \#291 Posted by: Sooty Posted at: 2018-11-27T20:46:18.363Z Reads: 130

```
Will you do a final pricing post?
```

---
## \#292 Posted by: legend27 Posted at: 2018-11-28T05:34:26.764Z Reads: 129

```
Yes :slight_smile: I will do one including all the tools I bought and then another one with only the parts used to build the board :slight_smile:
```

---
## \#293 Posted by: legend27 Posted at: 2018-12-29T01:47:47.532Z Reads: 130

```
**UPDATE #53**
-

Hi again everyone!

I have been playing around with the LED srips and the front and rear light. I have also removed the paint on the deck where the epoxy will be.

https://youtu.be/YQEoTFeyvVo

![IMG_3695|666x500](upload://xqJnCYcjzp1pag2bU6fMpl19VhF.jpeg) 


Then I made the support for the epoxy but after a day it somehow had got fucked up. Had to remove it again because it would leak epoxy..

**Before:**
![IMG_3699|666x500](upload://k01mOI7hr9OfepQPOMDd805ZLHl.jpeg) 

![IMG_3697|666x500](upload://qIEfQmfK5C8vcb2kWhOupfcEmNw.jpeg) 

![IMG_3698|666x500](upload://jQPDREBU92Mju2GCmORT3MFgNgD.jpeg) 

**After:**
![IMG_3703|666x500](upload://vYU6fv8Ce1MpRViRkQgRbhSVsQ3.jpeg)

![IMG_3705|666x500](upload://jNbO0NOl544yA0dlbt9n48IVgoE.jpeg)

**Then I removed it...**
![IMG_3704|666x500](upload://u6llFERTUXHKqYkhuBvmObGrFPU.jpeg)

I also need some way to turn on/off my lights and since I don't have a fancy app or some cool way of doing it, is the only way buttons.

**Made some more holes in my enclosure and added the buttons**
![IMG_3702|666x500](upload://9yoFMa30ruyc4glhNvryrEWG3RM.jpeg) 

**The front and rear light**
![IMG_3709|666x500](upload://Avw5L53ifVfiOCX2jgq6R803TfF.jpeg)

I ordered some new bolts from AliExpress and since they probably won't show up within the next couple of weeks and I really wanna get out riding, did I decide to "finish" the board. I can now ride the board and I don't expect to get it 100% done within the next months unless the weather is really bad because I'm lazy AF and hate working with epoxy.

I will make a full pricing with tools, shipping, taxes etc. when I get bored.

Wait a second... I can't ride my board yet. I got some new bushings for Christmas but only enough for one of the trucks. I ordered some for the other truck and will have them on the 2. January 2019. THEN I WILL FINALLY BE ABLE TO RIDE!!! (if the weather is good)

Enjoy the pics and happy New Years in two/three days!

**Bushings:**
- RipTide KranK Canon 87A (front and rear
- RipTide Pivot Cups 96A (Caliber II) (front and rear)
- flat washer front and round washer bottom
Will do an update on how they feel when I get out riding. And thanks for helping me find the right bushings @Alphamail! 
![IMG_3707|666x500](upload://yULTzIIvDPdkcb9sirkCxNiDuu5.jpeg) 

(don't know how I managed to fit everything in the enclosure)
![IMG_3721|666x500](upload://mCfkewIhiKoweA9ly3KFeLrejbE.jpeg)

(It was at this moment I realized the board drove backwards and had to remove the tape and do it all over again :expressionless:)
![IMG_3723|666x500](upload://xnUWAO6nPT2zL8hYhfQkqLM8e5z.jpeg)

![IMG_3724|666x500](upload://btRCRdO8X3uJaXkCq1XiFUOwN1H.jpeg) 

(Made the board go forward and here it is "finished")
![IMG_3726|666x500](upload://8N2Ko43zdA4EN4cLkJQZY9LQ1As.jpeg)
```

---
## \#294 Posted by: briman05 Posted at: 2018-12-29T01:57:03.730Z Reads: 121

```
The board is looking good
```

---
## \#295 Posted by: dg798 Posted at: 2018-12-30T00:41:31.985Z Reads: 114

```
@legend27  what lights are those
```

---
## \#296 Posted by: legend27 Posted at: 2018-12-30T03:43:12.943Z Reads: 111

```
What are you referring to? :thinking:
```

---
## \#297 Posted by: tardyparty7 Posted at: 2018-12-30T04:32:07.094Z Reads: 112

```
i think he means the "led sign" ones on the first or second pic.
```

---
## \#298 Posted by: legend27 Posted at: 2018-12-30T04:36:13.791Z Reads: 113

```
@dg798 @tardyparty7

Ahhhh.... that's the switch for the "F"ront light, "LED" light and "R"ear light.
```

---
## \#299 Posted by: dg798 Posted at: 2018-12-30T21:26:01.117Z Reads: 104

```
The actual led lights
```

---
## \#300 Posted by: pjotr47 Posted at: 2018-12-30T21:50:02.941Z Reads: 102

```
I am also looking for the front light... This is the back light I think...[Rear light](https://nl.aliexpress.com/item/12V-Red-LED-Car-Styling-Third-Brake-Light-Bar-External-Light-Source-Fog-Stop-Truck-Tailgate/32777824737.html?spm=a2g0z.10010108.1000014.3.6a3d20beSTWKic&pvid=e76009aa-b371-4c49-ab81-3b253c816679&gps-id=pcDetailBottomMoreOtherSeller&scm=1007.13338.80878.000000000000000&scm-url=1007.13338.80878.000000000000000&scm_id=1007.13338.80878.000000000000000)
```

---
## \#301 Posted by: legend27 Posted at: 2018-12-30T23:05:00.561Z Reads: 103

```
@dg798 ahhh, you wrote "lights" not signs :joy:
- [ LED lights](https://nl.aliexpress.com/item/SMD-5050-RGB-LED-Strip-Waterdicht-5-m-300LED-DC-12-v-24-v-CCT-RGBCCT/32903257649.html?spm=a2g0s.9042311.0.0.27424c4dlNkJOw) (don't know if I would recommend them. Had some issues with mine showing the wrong color. Ended up resoldering the strip and now they work just fine. You need to wire them like this to show the right color
|> - 12+
R - R
G - B
B - G
W - W

(controller - strip)

- [Bluetooth LED controller (Bluetooth RGBW)](https://nl.aliexpress.com/item/DC-5V-12V-24V-Mini-Bluetooth-WiFi-LED-RGB-RGBW-Controller-iOS-Android-APP-24Key-IR/32815415160.html?spm=a2g0s.9042311.0.0.27424c4dlNkJOw)
- [Splitter](https://nl.aliexpress.com/item/RGBW-5-Pin-Wire-Connector-1-to-2-Female-to-Female-Splitter-Connector-Extension-Cable-for/32816369026.html?spm=a2g0s.9042311.0.0.27424c4dlNkJOw)
- [Step down converter](https://nl.aliexpress.com/item/DC-DC-Converter-Adjustable-Power-Supply-DC-DC-Step-Down-3A-LM2596HVS-LM2596HV-DC-Step-Down/32485142548.html?spm=a2g0s.9042311.0.0.27424c4dlNkJOw) 

@pjotr47 Exactly. [This (14 led)](https://nl.aliexpress.com/item/12V-Red-LED-Car-Styling-Third-Brake-Light-Bar-External-Light-Source-Fog-Stop-Truck-Tailgate/32777824737.html?spm=a2g0s.9042311.0.0.27424c4dinqLkG) is the rear light I am using. Wouldn't really recommend it though, since it feels really cheap, not very waterproof and not very robust.
The front light I am using is [this (spot version)](https://nl.aliexpress.com/item/1-Stks-2-Stks-18-w-DRL-LED-Spot-Flood-Werk-Werklamp-9-32-V-4WD/32835112621.html?spm=a2g0s.9042311.0.0.27424c4d0neMXt). It feels much more robust and waterproof since its made out of some kind of metal/aluminium. Would defenitly recommend it, but its a PITA to mount it. I used some double sided tape but down known how long it will last. Im planning to mount it with some epoxy.
```

---
## \#302 Posted by: dg798 Posted at: 2018-12-31T01:52:22.051Z Reads: 89

```
Thanks man!
```

---
## \#303 Posted by: legend27 Posted at: 2018-12-31T09:10:05.674Z Reads: 88

```
Forgot to mention that I got the waterproof RGBW strip. You will also need some switches to turn on/off the lights.
```

---
## \#304 Posted by: Chrisjarram Posted at: 2018-12-31T09:28:05.287Z Reads: 92

```
Just to be the 300th post :)
```

---
## \#305 Posted by: legend27 Posted at: 2019-01-11T14:54:20.399Z Reads: 87

```
Don't feel like writing an essay but just want to give a quick update. After changing the bushings it's an whole other board. Really. I have also though people over-reacted when they got new bushings but they really don't. I now feel comfortable going 40 km/h.
The issue I'm facing right now is that my battery is a bit unbalanced also after charge.
I have been able to go 27.7km on a charge with still 60% left. (around 38V). My wh/km was 9.4.
```

---
## \#306 Posted by: legend27 Posted at: 2019-01-11T16:04:35.559Z Reads: 87

```
@pjotr47 and anybody else that might want to use the same front light I used:
Remember to put loctite on the bolts that hold the light in place. If you don't they will fall out (talking for experience).
I also suggest to upgrade to some M5 bolts with max length of 16MM. ![IMG_3765|666x500](upload://7YQZmIPU5L8ZhuIqoTtUoeWzLlf.jpeg)
```

---
## \#307 Posted by: pjotr47 Posted at: 2019-01-11T16:05:46.795Z Reads: 82

```
Haha will do, loctite is something important :slight_smile:
```

---
