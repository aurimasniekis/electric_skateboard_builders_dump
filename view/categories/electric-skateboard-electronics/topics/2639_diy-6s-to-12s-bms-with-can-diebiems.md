# DIY 6S to 12S BMS with CAN - DieBieMS

### Replies: 1107 Views: 62975

## \#1 Posted by: JTAG Posted at: 2016-04-27T01:49:42.280Z Reads: 2114

```
Now that I am addicted to my electric skateboard with the nice performance of the VESC I feel that the only thing missing is a decent and competent BMS for a wide configuration of cells. Therefore I would like to start a long term project which I will document here, both to keep myself motivated + maybe implement some great ideas that arise in this topic. I think and hope that this forum is the right place for this new hobby project :smiley:, feel free to point me to a problem you think I didn't adres that is a bottleneck for the current available BMS's. 

Please note that my goal is not to make a cheap or affordable BMS, my goal is to make the most competent BMS for e-skateboard applications. 

It will have the following features straight away:
*Soft power switch input with LED on / off / charge indicator.
*Charge input -> switched (high side) -> to charger input (to disable charger if a cell reaches the max voltage)
*Discharge input -> switched (high side)-> to motor controller / VESC (to disable the load when a cell reaches the min voltage)
*CAN bus interface for cell voltage monitoring and charger detection, status monitoring + more with future updates (like state of charge / state of health).
*Charge current sensing (future capacity measurement)
*Discharge current sensing (future capacity measurement)
*Pre charge for high capacitive load (with short detection, in case the motor controller is shorted / dead / wrong polarity)
*USB interface for serial communication and flashing (no need for a programmer -> HW serial bootloader is used)

Future features:
*mAh / Wh counting + soc + soh calculation.
*option to connect a [cheap oled display](http://www.ebay.nl/itm/0-96-I2C-IIC-Serial-128X64-OLED-LCD-LED-White-Display-Module-for-Arduino-Screen-/161836161890?hash=item25ae2fdb62:g:n9MAAOSw7NNUK-pv) for soc / soh display
*firmware update over can (trough VESC maby?)
*Chrome based configuration interface (+ firmware upgrades)

So far in my pre investigation I think I will be going with the following chipset:
BQ76200 [For high side N-FET switching + precharging](http://www.ti.com/product/BQ76200)
LTC6803-4 [Battery stack monitor](http://www.linear.com/product/LTC6803-2)
CP2104 [USB serial interface](http://www.silabs.com/Support%20Documents/TechnicalDocs/cp2104.pdf)
STM32F303K8 [uC with HW floatingpoint](http://www2.st.com/content/st_com/en/products/microcontrollers/stm32-32-bit-arm-cortex-mcus/stm32f3-series/stm32f303/stm32f303k8.html)
LM5165 [Power supply](http://www.ti.com/product/lm5165) with [744043151](http://nl.farnell.com/wurth-elektronik/744043151/tpc-inductor-4828-150uh-sat-0/dp/2082517)
ISO1050 CAN [Transceiver isolated](http://www.ti.com/product/ISO1050)
BF1 [Series fuse](http://www.littelfuse.com/products/fuses/automotive-passenger-car/high-current-fuses/bf1-58v.aspx#) 

Tracked in github (still in a very early stage):
https://github.com/DieBieEngineering/DieBieMS

Schematic can be found [here](https://github.com/DieBieEngineering/DieBieMS/raw/master/Project%20Outputs%20for%20DB10005_DieBieMS/DB10005_DieBieMS.PDF) (UPDATED). 

Thanks for your time :).

https://drive.google.com/file/d/1cAlaAxA7yCMaTV4SlLBUlxvXA49OH1vI/view
```

---
## \#2 Posted by: Mobutusan Posted at: 2016-04-27T02:15:40.466Z Reads: 1671

```
Most of this lingo is above my pay grade, but it sounds like a great idea. Having just shorted one of my Lipos, I'm liking the idiot (me) proof single plug bms scenario more and more. Good luck!
```

---
## \#3 Posted by: laurnts Posted at: 2016-04-27T02:22:00.328Z Reads: 1659

```
@JTAG Man this is 4am in the morning and you're still awake lol!

Yes this is a very cool project, to be widely acceptable I hope this BMS works with either lipo / 18650 packs! The capacity measurement is very cool, really hard at the moment to really test how much is exactly 5000mah after several cycles.

Btw I am not quite sure, but with Dual VESC configuration the CAN port is being used for traction control. Not sure if CAN bus could be branched, but since it's a bus its probably possible. I am not an electrical engineer, so I don't know how CAN bus works.

Finally some contribution from The Netherlands! Happy Kingsday @JTAG
```

---
## \#4 Posted by: harpie Posted at: 2016-04-27T06:32:01.859Z Reads: 1500

```
Awsome, i had a similar idea. Instead I was thinking of using one of the intersill battery management ic's with i2c. The vesc would then directly control the bms through i2c without the need for another microcontroller in the system. I might be mistaken, but I think there should be enough processing power left on the vesc.
```

---
## \#5 Posted by: Blasto Posted at: 2016-04-27T14:00:28.298Z Reads: 1385

```
With boundary scan? ;)
Nice project, what ecad you plan on using?
```

---
## \#6 Posted by: JTAG Posted at: 2016-04-27T14:35:01.395Z Reads: 1348

```
Yeah happy Kingsday to you as well :), finally the weather is getting better.

The CAN bus should have lots of capacity left to communicate with other stuff. Not really looked into the firmware of the VESC yet but I am pretty sure its possible.

@Mobutusan is saw your post! It looked nasty, but luckily no fire :). Especially the no more sparking and soft switching is what I like. I would really like the amount of PCB's in a board as low as possible.

@harpie Hmm I havent looked into Intersil yet thanks for the tip! Yeah the VESC has plenty of processing capacity left, but there is a chicken egg problem. The powermanagement of the vesc is not suitable to be always connected to the battery, this takes away the opportunity to utilize it. I would also like it to stay universal to be used with other BLDC's.

@Blasto nice one :), no, no JTAG. Just SWD should be sufficient :smile:. I am using Altium. 

Once I made all libraries Ill start composing the schematic and share it!
```

---
## \#7 Posted by: longhairedboy Posted at: 2016-04-27T14:46:25.202Z Reads: 1182

```
Its about goddamned time. 

When the time comes, i will tell you to shut up and take my money.
```

---
## \#8 Posted by: harpie Posted at: 2016-04-27T14:47:57.746Z Reads: 1154

```
Good point with the chicken egg problem. Looking forward to see progress. Is it going to be open source? Hope it gets an oled display!
```

---
## \#9 Posted by: JTAG Posted at: 2016-04-28T11:48:15.157Z Reads: 1128

```
@harpie  Yes ofcourse :slight_smile:! As soon as I start the schematic ill keep track in an open github repo.
```

---
## \#10 Posted by: Bender Posted at: 2016-04-28T12:39:00.380Z Reads: 1081

```
This is a fantastic idea!
I will be following this project with great anticipation
```

---
## \#11 Posted by: chaka Posted at: 2016-04-28T13:12:42.407Z Reads: 1028

```
I have been working on a non IC BMS, How much current will you be designing this to handle? It would be great if you used KiCAD for this project.
```

---
## \#12 Posted by: Blasto Posted at: 2016-04-28T14:14:35.416Z Reads: 1017

```
[quote="chaka, post:11, topic:2639"]
It would be great if you used KiCAD for this project.
[/quote]

Speaking out of experience, it's really hard for someone to go from Altium to Kicad, I tried and failed miserably. Felt like a complete Ecad noob.

Especially if he has a nice big library that is already built, building a library is a long and tedious process.
```

---
## \#13 Posted by: chaka Posted at: 2016-04-28T14:47:41.719Z Reads: 963

```
I suppose your right but you lose the people who only work on projects based on open source tools, myself included. I will just have to be happy sitting on the sideline cheering this project on!
```

---
## \#14 Posted by: JTAG Posted at: 2016-04-28T14:53:57.520Z Reads: 1038

```
Unfortunately indeed once you are used to a powerful CAD tool you get easily annoyed and lose motivation quickly ( for a costumer of mine I have to work in Eagle, it is HORRIBLE, I can sum the disadvantages but the list is so long I wont even start ). I need about 1/3 of the time in Altium than I would in Eagle. 

And next, if someone would like the branch and go in another direction with the project it is very likely the change would be significant and one would restart the pcb design completely (in the CAD program he/she feels comfortable). 

The weather is getting nicer by the day & parts are arriving -> there is lots of motivation to finish fast :D. Luckily the software of the BMS is orders of magnitude simpler than the VESC ^^.
```

---
## \#15 Posted by: JTAG Posted at: 2016-04-28T23:11:20.790Z Reads: 1034

```
HA someone had a similar idea! Nice one @onloop !  

https://www.youtube.com/watch?v=EHE5EMvVAiw&feature=youtu.be&t=344
```

---
## \#16 Posted by: Blasto Posted at: 2016-04-29T02:18:00.600Z Reads: 1042

```
But no mcu ;)

http://www.electric-skateboard.builders/t/the-troll-enertion-cf-deck-dual-tbs-6355-sensor-10s-build-completed/1491/17

Still in testing phase, some small issues to iron out
```

---
## \#17 Posted by: JTAG Posted at: 2016-04-29T21:32:49.975Z Reads: 1046

```
Aaaah how could I have missed that thread :hushed:? Nice build! Did you design this BMS? What chip do you use?

OK the project that kept me from making progress on the BMS is finally working! Here is the victory picture:
<img src="/uploads/db1493/original/2X/e/e1f9f13ffdafeb88ef431d91955a2870c7806bd1.jpg" width="675" height="499">

This weekend I fully dedicate to the BMS, let the progress begin :grin:!
```

---
## \#18 Posted by: Blasto Posted at: 2016-04-29T21:52:11.494Z Reads: 1000

```
It's based on the bq77pl900 ic from TI. It's a standalone chip, could be used in a host enviroment. Wanted to keep things simple
```

---
## \#19 Posted by: JTAG Posted at: 2016-04-29T22:07:50.567Z Reads: 1003

```
5 to 12S nice, with charge and discharge fet driver. Nice and affordable all in one solution indeed!
```

---
## \#20 Posted by: laurnts Posted at: 2016-04-30T02:32:48.930Z Reads: 1014

```
@JTAG I didn't read it as part of the features, but normally BMS are relative to cells count and the voltage. It would be nice if you can use various power supply voltages ranging from 12v up to lets say 50v.
```

---
## \#21 Posted by: JTAG Posted at: 2016-04-30T15:20:09.444Z Reads: 1014

```
Yes I could enable the BMS to support a "regular" power supply, It will need some sort of CC/CV supply or regulation. I did a project a while ago for a 12S system but never came around to finish the small and compact version of it:
<img src="/uploads/db1493/original/2X/f/f0806b7ccaf880c8647eee2792c7d3a426edae5e.jpg" width="666" height="500">

https://www.youtube.com/watch?v=kEH5Yj2vRCU

However I would like to add this as an option later (would have added 15 euro to the cost of the BMS for a 100W CC/CV or double for 250W).

The smaller version is still a hacky prototype xD:
<img src="/uploads/db1493/original/2X/7/732c305c8faa6a2ebecdb8df2205d31aa770fadd.jpg" width="666" height="500">
```

---
## \#22 Posted by: JTAG Posted at: 2016-05-01T02:15:34.892Z Reads: 958

```
Huge progress today. Was able to make most of the library components and started to compose the schematic. The schematic so far can be found on Github ( see opening post ). Its far from done but we are getting somewhere!

<img src="/uploads/db1493/original/2X/9/936a1b5f7d726a2ef7ef475f7c3dac35ade0e1e8.png" width="690" height="389">

Microcontroller will have a lot to "manage" :smile:.
```

---
## \#23 Posted by: laurnts Posted at: 2016-05-01T02:26:35.810Z Reads: 907

```
Nice progress man. Well i think the micro controller in VESC still have plenty of room to process data. However I hope it doesnt make it run hotter or hitting over heating issue.
```

---
## \#24 Posted by: JTAG Posted at: 2016-05-02T00:25:01.337Z Reads: 970

```
Next update and bringing an end to the sprint for this week. I forgot to add a SWD/Debug interface and switched the current / voltage monitoring to a dedicated chip ( [ISL28022](http://www.intersil.com/content/dam/Intersil/documents/isl2/isl28022.pdf) ) for the job making the focus of today remapping all IO / peripherals to the uC and implementing it in the schematic:
<img src="/uploads/db1493/original/2X/1/14a3f9fe458985be714d653beb647fde8887e346.png" width="542" height="499">

And implemented most of the power switching elements:
<img src="/uploads/db1493/original/2X/d/d1a5d3bafb8826e158616b790462dcf769e17f7d.png" width="690" height="311">

Finally I started playing with the components layout, this are the results so far: 

<img src="/uploads/db1493/original/2X/1/1cc33a35d15c04131e9389d127f2cb4ebe9fae87.png" width="690" height="413">

<img src="/uploads/db1493/original/2X/b/b3568c32a547af25cd4cef9bbcfe6f3590a90f19.png" width="690" height="357">
```

---
## \#25 Posted by: laurnts Posted at: 2016-05-02T00:41:33.009Z Reads: 872

```
Slick! Do you have an estimated dimensions? Please post more common data for normal people like me. Charging voltage? Charging current? Discharge current? Would it be customizable like VESC? I mean more general information :D it will trigger interest!
```

---
## \#26 Posted by: JTAG Posted at: 2016-05-02T00:51:57.138Z Reads: 904

```
Ah yeah of course! For now I design it with the following specs:

6S to 12S
Charge current: 15A (up to 20A depending on heat)
Discharge current: 120A (up to 160A burst a 10seconds isch depending on heat buildup)

I added a fancy feature that lets the BMS turn on when a charger is connected, The discharge contact will remain off (keeping the ESC powered down) in this state but the OLED display will show general information and the digital WS2812 LED shows a pattern indicating that its charging. 

On first instance only the trivial stuff will be configurable:
Number of cells
Max discharge current
Max charge current
max cell voltage 
min cell voltage

I am planning on making a simple chrome app to do this configuration stuff. Cross platform and needs minimal installation + auto updates :D.
```

---
## \#27 Posted by: Michaelinvegas Posted at: 2016-05-02T05:55:41.629Z Reads: 818

```
I feel like I should wear one of those full body non-static suits when I read this thread
```

---
## \#28 Posted by: Ulfberht Posted at: 2016-05-02T06:11:06.225Z Reads: 814

```
@JTAG You are freaking awesome!! This is a great thread! I can't wait to see where this is going! 
Cheers, Danny!!
```

---
## \#29 Posted by: Blasto Posted at: 2016-05-02T15:04:55.377Z Reads: 820

```
Good stuff!

You don't want to use the JST XH familly for your balance connector? don't forget to route your shunt signals as a diff pair.
```

---
## \#30 Posted by: JTAG Posted at: 2016-05-04T00:46:57.456Z Reads: 894

```
I don't really like the regulator balance connectors, they feel really cheap and are easy to accidentally break (exposing unfused thin wires to the battery, very scary). I also want two temperature sensors on the pack and this connector solves both of these issues/desires. 

And little progress on the schematic / board. I finally figured out how to reuse / implement multiple equal schematics for the cell balancing circuits:
<img src="/uploads/db1493/original/2X/6/6b79714b0fd19d01b4233fd78fc1a65428639068.png" width="690" height="343">

<img src="/uploads/db1493/original/2X/1/1c79737468de9c8e2a39848fbdaf3ef09c034ade.png" width="690" height="345">
```

---
## \#31 Posted by: laurnts Posted at: 2016-05-04T02:30:42.027Z Reads: 836

```
Nice progress man. Hey btw I just realized this. If your BMS is needing alot of computational power, would it be possible to utilize the power of the 2nd STM processor on dual VESC build? Otherwise just add extra STM processor for better flexibility of ur bms. One chip only cost 5 - 10 euro in mouser if I am not mistaken.

Just across my mind. At this moment balance charging system is quite in efficient according to my perspective. Is there any possibility to improve the charge rate for the last 20% of the capacity? I noticed my balance charger are slower when battery reaches about 90%.
```

---
## \#32 Posted by: Tarzan Posted at: 2016-05-04T08:57:36.475Z Reads: 807

```
That is some impressive work you do there.
I don't understand the magic behind it, but the numbers I do understand sound pretty awesome.
Keep up the great work an make this masterpiece available :smiley:
```

---
## \#33 Posted by: korryh Posted at: 2016-05-05T00:31:24.023Z Reads: 840

```
@JTAG This is great! always wondered how the magic works in a BMS - still not 100 percent on how it works but it is cool seeing your progression.  I dont mean to hijack the thread but you seem to be the person to ask about BMS stuff, after reading a bit I was curious if you could control sections of a battery with CAN - low voltage/high voltage cut off and have those sections controlled by the main PCB.  Basically take your cell balancing circuits and daisy chain them with CAN bus.  This way the battery can be modular so easy to replace sections and easy to wire (just daisy chain tx/rx- similar to is really quick rendering. <img src="/uploads/db1493/original/2X/7/7a8e9d1627eba3ab894689e0c0178963433aa1ed.jpg" width="690" height="439">
```

---
## \#34 Posted by: JTAG Posted at: 2016-05-05T00:39:41.589Z Reads: 819

```
What you seem to desire is having multiple battery voltage monitor pcb's (one per pack), them all connected to a CAN bus communicating with a master module that is in control of enabling or disabling the charge/discharge current. This is actually the most used method in electric vehicles / large battery systems.  There are a few open github projects with this exact topology.

However, this is not the path I would like to go with my design, although it is possible it would become crazy expensive since 70% of the cost is in the power switching components and not at voltage monitoring. Also electric skateboards (and in most other system that I know are needing a BMS are max 12S).
```

---
## \#35 Posted by: korryh Posted at: 2016-05-05T00:44:33.362Z Reads: 774

```
Thanks for the info. Cant wait to see where your BMS goes.
```

---
## \#36 Posted by: DeathCookies Posted at: 2016-05-05T11:21:11.983Z Reads: 789

```
Another question:
When You build a 12S3P pack it would Monitor and balance  12x 3 Batteries (3x) . Could it be that one battery is unbalanced because it checks the voltage of all three Batteries instead of every one individually ?  Just a Crazy example: 3V 3V 6,6V
```

---
## \#37 Posted by: chaka Posted at: 2016-05-05T12:20:42.022Z Reads: 772

```
All cells in a parallel group will self balance and the bms module will treat them as a single cell.
```

---
## \#38 Posted by: lowGuido Posted at: 2016-05-06T10:21:22.566Z Reads: 767

```
Mmmm I love Altium.

----------
```

---
## \#39 Posted by: korryh Posted at: 2016-05-31T21:19:15.997Z Reads: 762

```
@JTAG- any update on your BMS
```

---
## \#40 Posted by: JTAG Posted at: 2016-05-31T21:37:56.903Z Reads: 795

```
Yeah but nothing exiting, should post an update indeed, here is a small summary (ill make a bigger update soon):
*I worked on the power enabling / switching (managing how en when the BMS should turn on). I still need to check all voltage levels everywhere.
*I just received a LTC6802 evaluation board and had a little play with that, seems all nice and straightforward.

Next big thing todos are:
*Fix circuit around LTC.
*think of a way to safely configure the bms for the different battery configurations.
```

---
## \#41 Posted by: korryh Posted at: 2016-06-01T04:25:12.409Z Reads: 707

```
Thanks for the update. Let me know when you need a beta tester.
```

---
## \#42 Posted by: rpn314 Posted at: 2016-06-01T14:06:09.538Z Reads: 693

```
I'll second @korryh. This is fantastic work @JTAG
```

---
## \#43 Posted by: DeathCookies Posted at: 2016-06-02T13:32:45.905Z Reads: 717

```
Can you estimate the final price for getting such a bms?
Can you estimate a date for a beta test?
```

---
## \#44 Posted by: longhairedboy Posted at: 2016-06-02T19:27:58.146Z Reads: 734

```
@JTAG when can you shut up and take my money? lol

i'm itching for a compact high powered 12S, as well as a 10S variant. These monstrosities i've been using are great but they take up a lot of room and prevent any sort of super-stealth build.
```

---
## \#45 Posted by: JTAG Posted at: 2016-06-02T23:42:11.661Z Reads: 808

```
Sorry man, there is just loads of trash talk towards you guys te keep me structured :smile:.

Also motivation raised to a new level:

1. Got a decent laptop now (T440P) that lasts long enough to make long train rides productive again.
2. I have a functional but hacky personal electric longboard with no BMS that forces me to walk sometimes because I suck at charging it in time -> no state of charge indication XD.
3. I extended my student Altium licence with one year, I am at the latest version now hopefully getting rid of some annoying bugs.
4. SUMMER HAS COME.

**Cost**
A cost estimate calculation is boring to make and might be a little confronting, let me first build a prototype and judge on what components to go the cheap route. Some current / voltage monitoring stuff might be simplified in the final design to reduce cost.  

**Firmware**
Some of the never ending developments like feature adding will be realized in firmware and companion software, at some point I hope that others will jump into the SW development boat and help make the BMS even cooler. Because of the more luxurious (lazy) BMS hardware route the software development becomes doable for everyone (even for a hardware engineer like me) and add lots of features that in some regard might dazzle commercial boards. I hope that when(if) more of you end up with this BMS software development will make a jump and utilize all hardware features :smiley: (and mature into something as cool as the VESC). 

**Progress**
The latest progress is mainly focused on the circuit that controls when the power is enabled and the microcontroller can take control. There are many things to take into consideration and I might have overlooked some (that what makes the prototype stage fun^^). The main problem lies in the fact that when the BMS is disabled the current draw from the battery pack should be as low as possible demanding the powerstate control electronics to be low power but still be 'intelligent' (else a device that is made to protect and control the pack will end up breaking it when in storage mode for a long time). I also want many thing to trigger the enable state and even more challenging that once the power is enabled the microcontroller can detect 'what' made the BMS to turn on.

I want that the following items to enable the BMS:

* **Power button**
This will be a "soft" power button, so only push( being a momentary switch) opening possibilities for integrated rubber (boosted like) and small waterproof switches + making it possible to serve other roles/tasks ->. This will not only function as a power button but also to control the menu structure on the OLED/eINK display (when either of them is installed*). 
* **Microcontroller**
Since the power button is only a momentary switch the controller should also be able to keep the power (and therefore itself) enabled :evergreen_tree:.
* **Power applied to CAN bus connector**
In some applications where I fancy this BMS the usage will be on a remote location. In these applications a 3G modem will be present to relay telemetry data to the manager of the system. This 3G modem will have its own power supply ( something like the [particle electron](https://docs.particle.io/guide/getting-started/intro/electron/) ), the modem could trigger on request or at a set interval applying power to the CAN bus enabling the BMS and request SOC / cell voltage data (notifying the administrator in case of failures / low battery).
* **Power being applied on charge input (detect that a charger is connected)**
In order to track the state of charge, state of health and most importantly keep the cell voltages between set limits the BMS should detect when a charger is connected and act accordingly. One can also choose to keep the rest of the skateboard in power down (applying no power to the VESCs) during charging.
* **A computer being connected trough the USB connector**
In case of firmware upgrade or configuration the BMS should remain on.

*In the future I would like to get rid of the whole display and communicate all the data trough the CAN interface to the VESC which in his turn relays is to a phone or smart remote (evolve like). Because of the VESC versatility and the communities effort this is a REAL big and sensible option.

In the current design all of this should be possible. If it all works as intended the display could give very useful information:

* How many hours left to charge to battery to full.
* How much of the capacity is used ( in total / trip) and available in mAh and/or percentage.
* All measured data (max current / average current / cut off reasons / cell voltages and all the other stuff controlled by the already available button).

In case you omit the display I opted to support a digital WS2811 style LED to indicate the power states.

I updated the latest progress to Github and will update the PDF shortly (done).
```

---
## \#46 Posted by: Ulfberht Posted at: 2016-06-03T01:32:11.386Z Reads: 654

```
Thank you, Danny!! You are really contributing a lot here! Big respect, bro!
```

---
## \#47 Posted by: DeathCookies Posted at: 2016-06-03T06:42:30.044Z Reads: 659

```
Did you think about a remote power switch? It would be a great idea to start the engine (BMS) with a button on a remote!
```

---
## \#48 Posted by: Maxid Posted at: 2016-06-03T07:11:36.547Z Reads: 668

```
[quote="DeathCookies, post:47, topic:2639, full:true"]
Did you think about a remote power switch? It would be a great idea to start the engine (BMS) with a button on a remote!
[/quote]

Wouldn't the receiver constantly be using power? Not sure I want this on my battery.
```

---
## \#49 Posted by: DeathCookies Posted at: 2016-06-03T07:50:47.626Z Reads: 657

```
[quote="Maxid, post:48, topic:2639"]
Wouldn't the receiver constantly be using power? Not sure I want this on my battery.
[/quote]

Yeah, thats true. Another idea died :D
```

---
## \#50 Posted by: JTAG Posted at: 2016-06-03T11:34:48.931Z Reads: 630

```
Unfortunately the receiver would need continuous power indeed, that is not that big of a deal since there is a freaking huge battery connected and transceivers nowadays can operate with extremely low power. However the power management needs significant extending (add a power supply to make constant 3.3V ). So sure its possible and would indeed be cool, maybe if many like or want it we could add it (maybe as an optional board or something). 

It might also become a little scary when a kid grabs the remote and a 3kw+ beast awakens :P.

With the current setup an auto power off function when the remote is inactive or turned off is easy to realize.
```

---
## \#51 Posted by: DeathCookies Posted at: 2016-06-03T11:39:31.167Z Reads: 629

```
[quote="JTAG, post:50, topic:2639"]
Unfortunately the receiver would need continuous power indeed, that is not that big of a deal since there is a freaking huge battery connected and transceivers nowadays can operate with extremely low power.
[/quote]

Well if you put your board into a corner of your room and do not use it for a long time your battery will be drained... It does not happen that often but is annoying. 
A better idea is that everything is shut down and when you pull the transmitter out of a holder from the eboard it could power the receiveron and wait until the transmitter is on starting the main power. When you put it back into the holder the BMS detects it and will power off the receiver. That would be a freaking cool idea. But somehow the BMS has to detect if the transmitter is in the holder of the eboard.
```

---
## \#52 Posted by: Maxid Posted at: 2016-06-03T12:08:50.534Z Reads: 624

```
[quote="DeathCookies, post:51, topic:2639, full:true"]
When you put it back into the holder the BMS detects it and will power off the receiver. That would be a freaking cool idea. But somehow the BMS has to detect if the transmitter is in the holder of the eboard.
[/quote]
Well that you can simply do yourself with a switch - just modify the momentary switch @JTAG wants to add to the BMS anyway.
```

---
## \#53 Posted by: DeathCookies Posted at: 2016-06-03T12:16:20.635Z Reads: 628

```
[quote="JTAG, post:50, topic:2639"]
With the current setup an auto power off function when the remote is inactive or turned off is easy to realize.
[/quote]

Just keep attention that you do not set the "auto shut off timer" too low. If a transmitter fails and needs to be restarted the board should not turn off ;)
```

---
## \#55 Posted by: JTAG Posted at: 2016-06-13T01:02:41.832Z Reads: 656

```
It took a bit of fiddling around but finally all components are on board! The rough placement is done :smiley: . 

<img src="/uploads/db1493/original/2X/8/8eb95ea6087c172c092cf48e69ce8f55f8dcdf78.png" width="690" height="331">

Now the routing starts, the part I love the most ^^.
```

---
## \#56 Posted by: Tarzan Posted at: 2016-06-13T07:01:43.963Z Reads: 638

```
Awesome! I wish I could contribute anything to your project, but that's another level of building stuff.
Keep up the good work and make this masterpiece available for the community.
```

---
## \#57 Posted by: Ulfberht Posted at: 2016-06-13T07:38:50.333Z Reads: 631

```
Incredible! I really like the direction you are heading with this! :thumbsup:
```

---
## \#58 Posted by: JTAG Posted at: 2016-06-15T01:30:24.368Z Reads: 700

```
Thanks for the support! It helps me to keep motivated ^^!

Had a couple or routing hours:
<img src="/uploads/db1493/original/2X/1/1a965b32c96795c2b12426fc77f596da07833b74.png" width="690" height="299">

<img src="/uploads/db1493/original/2X/2/28214ac06891f1c62c709db2e27285141f5c6030.png" width="690" height="293">

<img src="/uploads/db1493/original/2X/2/2c80d0415fa3e5f6cc94521248bbe219e4636bb8.png" width="690" height="296">

Got a lot of work done, still quite a bit to do trough, we are getting there :D.
```

---
## \#59 Posted by: hexakopter Posted at: 2016-06-15T14:32:26.387Z Reads: 663

```
Nice idea. Looking good as far as I can tell. :grinning:

But what are the dimensions? Looks like something around 5,5cm x 12,5cm now.
And what charging voltage do you plan to use?
```

---
## \#60 Posted by: Arzamenable Posted at: 2016-06-15T14:48:20.175Z Reads: 655

```
I'd like to contribute too, but this seems out of my league. I guess I could offer sutures if things get out hand 😉👍
```

---
## \#61 Posted by: Ulfberht Posted at: 2016-06-15T21:52:44.473Z Reads: 653

```
@JTAG I'd love to test a couple of these out.  
For science! :wink: 
You are raising the bar on what can be done DIY. I just want to support what you do!!
```

---
## \#62 Posted by: DeathCookies Posted at: 2016-06-15T23:36:15.092Z Reads: 605

```
Me too. I would like to buy some for test purpose too
```

---
## \#63 Posted by: korryh Posted at: 2016-06-16T00:13:34.215Z Reads: 617

```
Ditto. This means I will probably buy some batteries and a spot welder as well. 

I think I may have a problem. Hi, my name is Korry and I am an esk8aholic.
```

---
## \#64 Posted by: Krudte Posted at: 2016-06-16T00:50:02.225Z Reads: 640

```
@JTAG this is looking so good! I'm definetly also interested! your work is taking esk8 to the next level, keep it up man :D :chestnut:  :chestnut:
```

---
## \#65 Posted by: JTAG Posted at: 2016-06-16T23:21:22.465Z Reads: 722

```
Thanks guys (as I assume there are mostly guys around here)!

Once we are confident everything operates safely we will be offering complete prototype boards (very limited). Functionality will gradually grow since up until now it seems I will have to make the software as well :P ( any volunteers? It will first only be embedded software and in the future something with a chrome app "cleanflight" UI style ). 

In the meantime today I was able to finish the rough routing, tomorrow ill do a little tweaking, polishing and designrule error solving and then its up to the PCB fab :smiley:!

<img src="/uploads/db1493/original/2X/7/737e13f561ef54958ffaab9a79951ded222de2e7.png" width="690" height="293">

<img src="/uploads/db1493/original/2X/e/e663c3493860d3ff8f04c2abc858a24f1b4c47b7.png" width="690" height="279">

 <img src="/uploads/db1493/original/2X/5/5302a5e6c323b401e7edce5b3f909f4d6ed625c0.png" width="690" height="275">

I did a minor update to the schematic, we should now be able to detect if the main fuse is broken / has failed. Lets hope that this all works!

Somehow I completely missed all the request for dimensions :o. The dimensions are:
<img src="/uploads/db1493/original/2X/0/054a8372d766ac1d459ffc60639bce675d8e4842.png" width="374" height="330">

And the height approximately 15mm including the bolts to mount the wires. This can be lowered if you find a different way to bolt the cables to the enormous press fit sockets xD.

If you wanna have a play with it in 3D, you can import this [STEP file](https://github.com/DieBieEngineering/DieBieMS/raw/master/DB10005_BMS.step) into for example Solidworks.
```

---
## \#66 Posted by: Kaly Posted at: 2016-06-16T23:26:20.054Z Reads: 648

```
Nice this is so exciting :slight_smile: 
this is great work man thank you !!
```

---
## \#67 Posted by: JTAG Posted at: 2016-06-18T22:03:09.752Z Reads: 682

```
Ok production files are ready and send to the factory!

<img src="/uploads/db1493/original/2X/1/14bb5626b8c19bc102bbfdc8363e6f339bd0bfa0.png" width="690" height="307">

I cant wait to touch it in real life ^^....

<img src="/uploads/db1493/original/2X/1/13391c1ea42ad993f45b49f4f82d4b9d0ca62f6b.png" width="690" height="357">
```

---
## \#68 Posted by: Ulfberht Posted at: 2016-06-18T22:11:28.213Z Reads: 619

```
@JTAG Fantastic!! Just beautiful to look at... 
Great work!!! You are one talented dude!! :v:
```

---
## \#69 Posted by: Bender Posted at: 2016-06-18T22:16:05.529Z Reads: 604

```
When can I get one?😀
```

---
## \#70 Posted by: rpn314 Posted at: 2016-06-18T22:51:03.899Z Reads: 604

```
Looks fantastic!
I'd definitely be available and interested to be a tester
```

---
## \#71 Posted by: Menwaylo Posted at: 2016-06-18T22:51:39.871Z Reads: 602

```
Put me down for one!!!Man that is talent to just whip up a bms in your spare time, while your at it just add dual vesc's a reciever and charger if you come across some more spare time. That would be a nice plug and play system..:slight_smile:
```

---
## \#72 Posted by: Kaly Posted at: 2016-06-18T22:52:52.283Z Reads: 583

```
Put me down as a tester.
```

---
## \#73 Posted by: cmatson Posted at: 2016-06-18T23:45:18.319Z Reads: 584

```

I've been following this and literally can't wait.. This is going to be sweet
```

---
## \#74 Posted by: mason Posted at: 2016-06-19T00:07:43.595Z Reads: 597

```
My god this is awesome. I would love to try this out ASAP.
```

---
## \#75 Posted by: lox897 Posted at: 2016-06-19T00:28:33.968Z Reads: 614

```
This is epic. I've also been following the progress of this BMS. Can't wait to see what it looks like.
```

---
## \#76 Posted by: JTAG Posted at: 2016-06-19T14:56:22.579Z Reads: 640

```
Thanks :D! But calm down guys, its still a prototype :sweat:. There is still some hardware verification to be done + some software to write (luckily the latter can be very simple at first).

In comparison to our hacky VESC setup:
<img src="/uploads/db1493/original/2X/2/27d2016c31d51b7879f38c454d08eb9607e6f81f.jpg" width="375" height="500">

In the future when the VESC 5.0 / 6.0 (whatever it is called) is matured I might squeeze VESCs + caps in the same footprint as the BMS allowing for a nice and compact DIY buid ^^.
```

---
## \#77 Posted by: emepror Posted at: 2016-06-20T22:31:29.774Z Reads: 611

```
I'd like to jump on the list for one once their available, I can also try my hand at hardware debug (just got out of school as an electrical engineer, gotta put it to good use!)  if needed, slightly lacking tools right now though 😞. 

Not sure if it's mentioned above, didn't see it the last time I ran through, but what's the current rating ? Also thoughts on how to handle that directly on the PCB. I.e trace widths etc
```

---
## \#78 Posted by: Blasto Posted at: 2016-06-21T00:55:56.632Z Reads: 601

```
@JTAG  knows what he's doing, i have my doughts about the 150A fuse on the silkscreen. But i'm sure it can handle a good amount of continuous current.
```

---
## \#79 Posted by: emepror Posted at: 2016-06-21T01:27:45.540Z Reads: 597

```
ohh yeah his work is awesome, not doubting that, i've been starting to work with some higher current designs and i'm looking for some opinions from others.
```

---
## \#80 Posted by: Blasto Posted at: 2016-06-21T01:47:45.606Z Reads: 632

```
I'll try not to hi-jack the thread here, personnally i use Saturn pcb tool kit for trace width calculations and what not.

http://www.saturnpcb.com/pcb_toolkit.htm

If you look closely at the top layer, you will see hundreds of vias, to transfer heat to the other layers, to get as much copper as possible in the smallest footprint possible. Copper weight is another big factor, but that will affect the rest of the pcb. On this design it seem that the smallest track to track width is 10mil, could have 4oz of copper on the external layers, but it will be pricey and a bitch to reflow the smt components
```

---
## \#81 Posted by: JTAG Posted at: 2016-06-24T11:29:19.003Z Reads: 657

```
Parts are delivered slowly :smiley:.

<img src="/uploads/db1493/original/2X/6/6614bed08c12057ec85ac40c23b61ffd54ae49cd.jpg" width="666" height="500">
```

---
## \#82 Posted by: harpie Posted at: 2016-06-24T11:33:58.260Z Reads: 616

```
Really cool! Good name (DieBieMS). Has a whole other meaning when pronounced in English. Hope you added lots of LEDs!
```

---
## \#83 Posted by: zeno Posted at: 2016-06-25T10:58:36.797Z Reads: 601

```
I'd like to pitch in to help with the software part! :)
```

---
## \#84 Posted by: JTAG Posted at: 2016-06-29T17:46:01.683Z Reads: 617

```
@zeno nice :D! Thanks for the offer!

If the hardware is verified I'll look into how to tackle the software.

The latest news: PCBs came in!

<img src="/uploads/db1493/original/2X/0/093a166a93bf7fd5aeac467640c43e0b18320d88.jpg" width="281" height="500"> <img src="/uploads/db1493/original/2X/5/5aabb1f3dc0b9f304ebc486ab8dfca1e5178ec5f.jpg" width="281" height="500">
```

---
## \#85 Posted by: zeno Posted at: 2016-06-29T18:00:12.785Z Reads: 583

```
Whoop! :slight_smile:

_btw, I'm the guy that picked up that vesc last sunday ;)_
```

---
## \#86 Posted by: JTAG Posted at: 2016-06-29T18:14:29.712Z Reads: 593

```
Haha nice! I already had that suspicion :smile:.
```

---
## \#87 Posted by: JTAG Posted at: 2016-06-30T08:02:37.799Z Reads: 642

```
<img src="/uploads/db1493/original/2X/8/8d1a620917ab66aa4556c729224c525820441a6b.jpg" width="666" height="500">

<img src="/uploads/db1493/original/2X/2/2a214c123fd32a8db227d0f38ad8ef1456a0ebbf.jpg" width="666" height="500">

<img src="/uploads/db1493/original/2X/3/39755663255e27b58ebed3b96c122ee093f1a3d5.jpg" width="370" height="499">

I had a little time to mount most of the components. There are still a few important parts missing but this is a nice start ^^.
```

---
## \#88 Posted by: scoobiext Posted at: 2016-07-01T00:01:33.077Z Reads: 578

```
Absolute work of art.  Definitely on my wish list, can't wait.
```

---
## \#89 Posted by: Pantologist Posted at: 2016-07-01T04:43:47.734Z Reads: 575

```
Ehhh I am holding off buying from Bestech because I want to have this so badly! :D 

Any rough estimates on pricing or when some prototypes boards will be available for testing?
```

---
## \#90 Posted by: Nordle Posted at: 2016-07-02T11:39:33.218Z Reads: 575

```
Can you add a buzzer,and make an option to let it beep instead of cutting power. If for example a cell drops to low or when overcurrent is reached. This would still allow controll over the board.
```

---
## \#91 Posted by: MrEpiquad Posted at: 2016-07-05T14:50:58.812Z Reads: 575

```
@Nordle There is already a buzzer just below the usb connector, it's just not soldered on yet.
```

---
## \#92 Posted by: appelton Posted at: 2016-07-05T15:04:54.951Z Reads: 564

```
What are the exact dimensions of this beauty ?
```

---
## \#93 Posted by: Stevemk14ebr Posted at: 2016-07-06T01:48:10.266Z Reads: 562

```
eta? Looks really cool
```

---
## \#94 Posted by: JTAG Posted at: 2016-07-10T22:11:26.985Z Reads: 617

```
Ill answer you all soon! I was too busy with solar boat racing last week :). 

A teaser for the progress I made today:
* USB <--> serial works.
* SWD interface is correctly connected :blush:.
* Blinky works.
* Pre-charge circuit works.
* Main output switch works.
* The whole powermanagement and charger detection works :smiley:! 

Main output switch:
https://youtu.be/d3oHv81YU4E

Pre-charge:
https://youtu.be/aMyzXU0MiL0
```

---
## \#95 Posted by: Stevemk14ebr Posted at: 2016-07-11T01:12:38.197Z Reads: 571

```
Looks great! Any chance the software will be open source? I'd love to take a look and contribute (im a cs major).
```

---
## \#96 Posted by: Michaelinvegas Posted at: 2016-07-11T02:11:15.993Z Reads: 585

```
Bravo @JTAG

👏🏻
--------------
```

---
## \#97 Posted by: JTAG Posted at: 2016-07-17T11:23:46.341Z Reads: 623

```
@Stevemk14ebr yes! Most of the drivers and basic functionality is done but still a bit hacky, once I feel confident ill push it to github. First I want to ride a damn skateboard with it, then ill clean the code :).

@Nordle you will have all the freedom to configure an allowed lowest cell voltage, the idea behind a BMS however is to **protect** (protect against low and high cell voltages) the battery against abuse and to make it easy to use (simple 2 wire charging). Once all hardware/software drivers are written ill start to implement a module that will hopefully keep track of an accurate state of charge, if you use the SOC info correct you will never end up with an empty :innocent:. And like @MrEpiquad said there is a buzzer on the board (however for a long time it was unpopulated):
<img src="/uploads/db1493/original/2X/e/eed8c27d04989836fd36c2d43f093edddfdf07e2.jpg" width="666" height="500">

@Pantologist I hope that this BMS in combination with a dual vesc setup + future fancy remote will create the boosted board like experience. All this fancy stuff makes it mode pricey than chinese BMSes, on the +side there are lots of customization possibilities (and allowed high current).

@appelton dimensions are 140*60mm.

Here I have a static dual VESC setup to test pre-charging (anti spark), switch the main current path (bypassing pre charge and allow the full current to flow) and simultaneously measure pack current + voltage:
https://www.youtube.com/watch?v=bUREnOEL0cg&feature=youtu.be

Here the same but now with me sitting on the board:
https://www.youtube.com/watch?v=WuTpSgyIEc0&feature=youtu.be

Demonstrating turning the board on/off:
https://youtu.be/5D9kg96CN14
```

---
## \#98 Posted by: JTAG Posted at: 2016-07-24T17:56:30.536Z Reads: 595

```
<img src="/uploads/db1493/original/2X/1/1e5f606f561836352b570236a644ccc2569b740a.jpg" width="666" height="500">
<img src="/uploads/db1493/original/2X/6/687b83287560d0d4d5ab3bb2d80b59668e9fb60f.jpg" width="666" height="500">

Display is alive :D!
```

---
## \#99 Posted by: Blasto Posted at: 2016-07-24T18:55:48.620Z Reads: 564

```
Looks clean!👌
```

---
## \#100 Posted by: boards Posted at: 2016-07-25T05:44:38.867Z Reads: 569

```
The work you are doing is insane!

I plan on trying your encoder method and soldering up BMS once it's finished.
```

---
## \#101 Posted by: JTAG Posted at: 2016-08-06T01:07:51.007Z Reads: 608

```
Some good news, I just got the battery stack monitor working (LTC6803-2)! It took some time since I first wanted to make the general firmware buildup universal and "neat". It is far from finished but the software for now is very clear and easy to understand + most importantly easy to extend. There is no real useful functionality yet (because the lack of cell voltage information so far) but now that this chip is working that should not take to long. 

<img src="/uploads/db1493/original/2X/5/5ec9ebb65a4f4bb7c55167d474e62950b86662ad.png" width="690" height="376">
STM has this freaking awesome tool that enables you to look inside the chips memory "realtime" trough the debugger without interrupting the code. This makes for a powerful debugging tool. In this screenshot you can see an accurately measured pack voltage & current namely packState.packVoltage and packState.packCurrent measured by the ISL28022. The packState.loadVoltage is a voltage measurement done by the micro controller and thus much less accurate, this voltage is only used to verify the output voltage during precharge, it will give the OK to enable the main current path if the output voltage is within 85% of pack voltage, if for a certain time the output does not reach this threshold the BMS goes to error mode (probably because the output is shortened or initial load is to high).

You can also see all 12 measured cellvoltages being displayed. I deliberately use a very unmatched pack to test my software (and safety features). Current setup 12S 18650:
<img src="/uploads/db1493/original/2X/0/0dc095a7d12312cbe78c14f79ddedc4cc140607b.jpg" width="666" height="500">
```

---
## \#102 Posted by: JLabs Posted at: 2016-08-06T01:40:26.602Z Reads: 566

```
This is amazing.. I literally sat here and read this hole thread wanting more... This is great!! Keep it up!
```

---
## \#103 Posted by: cjoliver Posted at: 2016-08-06T05:55:49.539Z Reads: 558

```
If you ever run into any problems there's another project similar 

https://github.com/Teslafly/OpenBMS
```

---
## \#104 Posted by: Stevemk14ebr Posted at: 2016-08-06T16:27:43.904Z Reads: 544

```
That project seems cool but it's very incomplete and the code is absolute spaghetti (that means messy for non coders)
```

---
## \#105 Posted by: cjoliver Posted at: 2016-08-06T19:50:08.462Z Reads: 536

```
Lol the code is formatted correctly and has detailed comments on nearly every line of code, very neat. And if you followed the thread the creator made he successfully made a modular BMS that allows up to 96 cells. I love what JTAG is doing here but if he ever ran into problems this is an incredible resource to look at
```

---
## \#106 Posted by: Stevemk14ebr Posted at: 2016-08-06T20:36:01.097Z Reads: 526

```
having proper indentations and comments is not what make code clean. I agree it's a great resource, it's just not clean code
```

---
## \#107 Posted by: cjoliver Posted at: 2016-08-06T21:02:36.010Z Reads: 513

```
Mind explaining why its ugly code then?
```

---
## \#108 Posted by: Kaly Posted at: 2016-08-06T21:05:55.127Z Reads: 511

```
@cjoliver @Stevemk14ebr 

Please guy, let use PM for that conversation.
thank you in advance for your cooperation ;-)
```

---
## \#109 Posted by: cjoliver Posted at: 2016-08-06T21:45:27.724Z Reads: 519

```
Lol


tenchars
```

---
## \#110 Posted by: Ulfberht Posted at: 2016-08-06T21:50:49.201Z Reads: 531

```
[quote="JTAG, post:101, topic:2639"]
STM has this freaking awesome tool that enables you to look inside the chips memory "realtime" trough the debugger without interrupting the code
[/quote]

This is incredible news! Thanks for posting the pics. It really illustrates the concepts well. :thumbsup:
```

---
## \#111 Posted by: reynex Posted at: 2016-08-10T04:52:20.063Z Reads: 533

```
As a student, this is very inspiring! our design project is the same as this, BMS with active cell balancing 48volts for e-vehicle applications. Right now, we only have little idea on how to do it. How do you guys learn how to design BMS in its hardware and software? can you recommend me some books to read? I am not that knowledgeable at this moment but I am very willing to learn to know how it works to be able to design a BMS. From choosing the right microcontroller, IC, and other parts up to implementing the software. Any help from all of you guys is very much appreciated. Thanks. God bless. And hoping to hear from you all soon. :slight_smile:
```

---
## \#112 Posted by: sl33py Posted at: 2016-08-11T00:24:54.486Z Reads: 521

```
@JTAG - wow man this is really amazing.  I'd love to be an early tester if you still need one.  I'm on the fence on BMS and have been kicking around the idea of adding one to my boards - this looks like the ultimate BMS to me.

Let me know when there is a pre-order option and how i can help support!
```

---
## \#113 Posted by: Blasto Posted at: 2016-08-11T00:32:57.409Z Reads: 519

```
Go on ti.com, choose a chip, read a fuck ton of app notes
```

---
## \#114 Posted by: boards Posted at: 2016-08-20T06:08:55.554Z Reads: 522

```
Do you think it's a safe bet to start buying components, or do you think you are going to have to do some major hardware revisions?
```

---
## \#115 Posted by: JTAG Posted at: 2016-08-20T09:57:51.471Z Reads: 566

```
[quote="boards, post:114, topic:2639"]
ardware revisio
[/quote]

Hi, there is a hardware revision upcoming to improve ease of manufacturing and a few small component value changes. There is also a small conducted emission.immunity test coming that should show any major design flaws if any.

Small update:
The BMS was capable of balancing the pack (with mismatches like the previous screenshot) to this new state in just 4 hours :blush: :
<img src="/uploads/db1493/original/2X/0/0bda0e452704fc08fba652621cc2b63a15097424.png" width="690" height="373">

I am now working on a command line interface over serial, this should make configuration doable as long as there is no real ui.
```

---
## \#116 Posted by: NAF Posted at: 2016-08-20T10:41:41.296Z Reads: 522

```
@JTAG You are sitting on a gold mine here. Just make it into final production, and we all are going to buy this piece of art from you !!
```

---
## \#117 Posted by: Ulfberht Posted at: 2016-08-20T23:26:14.637Z Reads: 502

```
@jtag Brilliant!!! :sunglasses::+1:
```

---
## \#118 Posted by: Pedrodemio Posted at: 2016-08-25T04:49:59.657Z Reads: 545

```
Amazing work @JTAG, count me in too, already have the space reserved in my next build

Do you have any ideia on how the fuel gauge algorithm will work? I've been sketching some ideas but none seen reliable to give an acurate state of charge across all available energy. I was going to design it to gather the energy consumed from VESC via uart on an arduino

The main problems I found:
- how to account for battery degradation?
- since most discharges are only partial (in my case maybe in will never use all the energy in one take) you can't average the total energy from a few full discharge cicles and make that the 100% state of charge
- In you design i understood that the current and voltage are measured charging and discharging, the integration errors over a lot of charge/discharge cicles is negligible? But even so I don't see a way of estimating the loss from degradation without doing a complete full discharge from time to time

Of course all of the above aims toward a ultra precise fuel gauge, maybe for our boards just using a 100% charge energy value a little bit below than the real capacity and integrating charge/discharge energy will do

I wil take a look at the Tesla open patents, from all I've seen they do do a pretty good job on the fuel gauge, even so considering that most of the people will never do a full discharge on the lifetime of the car
```

---
## \#119 Posted by: Heavy1 Posted at: 2016-08-25T06:28:43.352Z Reads: 510

```
Is it ridiculous to ask a ballpark $ on what this BMS will be? :)
```

---
## \#120 Posted by: JTAG Posted at: 2016-08-25T13:31:45.011Z Reads: 528

```
I don't know what algorithm I am going to implement yet. I just know I know everything that is realistically measurable about the pack (individual cell voltages, pack current and temperatures on two places in the pack) . Once all the basic functionality is done ( already done ) and safety cut off systems( almost done ) ill start looking at research papers that focus on this topic.

I haven't summed up all components. but expect a price close to 150 euro.
```

---
## \#121 Posted by: Garfield Posted at: 2016-09-08T11:42:49.062Z Reads: 554

```
@JTAG

Have you been heard from a technic called "Power Pump Cell balancing" (name from TI)? This technic discharges the stronger cell and use this energy to charge the weaker cell so there aren´t isn´t so much energy wasted into head during balancing. With this technology it is also possible to balance the cells during discharge to squeeze all energy out of the pack. Unfortunally all ICs which are designed for the technic are not recommendet for new designs (see BQ78PL116). Here is an [Application Report](http://www.ti.com/lit/an/slua524b/slua524b.pdf) from TI which describes the principle a lot better than I could do.

Disadvantages are you need more components and the PCB would grow.

Perhaps you could think about adding this feauture to your BMS Version 2.

But in any case I  would love to see a BMS from you which I could use for my two wheeled balancing scooter. I would use the BMS on my battery and the CAN connected to an Teensyduino 3.1 on the Teensyduino there are two VESCs on the hardware serial ports 1 and 2 and some sensors and LEDs for battery level indication and things like that. So the Teensyduino would be the head and only needs to read out the BMS.

I would love to see a charging Mode also so that I could integrate everything I need to charge the battery into the vehicle.

Please have a look an the following [article](http://blog.chromium.org/2016/08/from-chrome-apps-to-web.html) and think about using a chrome app.

Best Regards
```

---
## \#122 Posted by: Nordle Posted at: 2016-09-08T12:27:20.695Z Reads: 489

```
Would you mind willing share your ''Teensyduino-project''? :)
```

---
## \#123 Posted by: Garfield Posted at: 2016-09-09T12:43:46.632Z Reads: 498

```
I wouldn´t mind it is planned to share the project but there is only one feauture missing before I share the code. I will implement the feauture that the Teensy is capable of getting the actual VESC config over UART and uses the actual in the VESC configured parameters for max and min current and voltages. So that I don´t have to set the currents and voltages three times (first time in VESC1 second time in VESC2 and the third time in the Teensy). I hope I find time in the next two weeks to implement and test this so that I could document and share my code.
```

---
## \#124 Posted by: zeinstra Posted at: 2016-09-14T12:32:26.804Z Reads: 498

```
Al those electrical engineering art looks like magic to me.
Very nice work!
```

---
## \#125 Posted by: Pantologist Posted at: 2016-09-24T14:44:35.162Z Reads: 474

```
@JTAG Would it be possible to add a 5 LED battery voltmeter to this via the port for the OLED? 

I think it would be easier to implement and read on a longboard. Similar to what Boosted now has. 

Bestech also has it on their higher end boards. It indicated charging too. 

https://snag.gy/wAFpdg.jpg
```

---
## \#126 Posted by: IDVert3X Posted at: 2016-10-12T13:37:33.955Z Reads: 444

```
Port for the display is I2C bus which has 2 data wires, VCC and GND.
It can't be used for this purpose, but it's not a big deal to add a few solder pads for the LED wires.
He would have to redesign the PCB and assemble a new one. Implementation in SW would be really easy.
Maybe we could expect it in the new HW version?
```

---
## \#127 Posted by: B4Me Posted at: 2016-10-12T13:58:46.559Z Reads: 451

```
One could also make a I2C to LED pcb, with some smd LEDs on, using the same or another I2C ID, then it could just send data to both IDs, and ignore if one of then isnt connected.. or check on boot which ID is attached, and only send data to one of them
```

---
## \#128 Posted by: stealth71 Posted at: 2016-10-12T15:58:13.027Z Reads: 460

```
Cool project.
```

---
## \#129 Posted by: JTAG Posted at: 2016-10-17T22:57:46.391Z Reads: 506

```
Hi all, 
Sorry for the long delay, I had some awesome other projects to work on xD.

The LED battery indicator desired is actually VERY easy to implement :stuck_out_tongue:. For example this one has I2C and can be connected directly to the Display connector on my BMS:
http://www.dx.com/p/battery-style-digital-tube-led-battery-level-display-module-for-arduino-avr-arm-pic-blue-340914#.WAVVa-h96Hs

<img src="/uploads/db1493/original/3X/9/8/982f70fc25117b054cfe5f73613011bdde75933e.jpg" width="500" height="500">

This display would need only minimal software support. 

Other progress:
<img src="/uploads/db1493/original/3X/d/f/df73a4206b0a5141b65bd8ac89a2ba7eda3ec616.jpg" width="668" height="500">
<img src="/uploads/db1493/original/3X/6/e/6edb745ca67bdb627135bd184c1470672ec0ca44.jpg" width="668" height="500">
<img src="/uploads/db1493/original/3X/f/6/f6706c61d833b86c710ccc71d1f0276e873c2e84.jpg" width="666" height="500">
<img src="/uploads/db1493/original/3X/c/f/cf644194f8adea0fb5dcd5e7894762c3b4ff6629.jpg" width="666" height="500">
<img src="/uploads/db1493/original/3X/d/4/d4e31c8f6cddf3847bf8bb6ca047933e6478daef.jpg" width="668" height="500">

I finally found the time + motivation to connect the BMS and Meanwell charger to my 6S longboard. Next ill try to hack a SD card holder to the BMS to start logging cell voltages + current in order to develop and evaluate a state of charge / health algorithm.
```

---
## \#130 Posted by: laurnts Posted at: 2016-10-17T23:00:10.704Z Reads: 459

```
The board looks very beatup! used alot :smiley:
```

---
## \#131 Posted by: JTAG Posted at: 2016-10-17T23:16:07.520Z Reads: 455

```
YES! The board is used every day :kissing_closed_eyes::heart_eyes:.
```

---
## \#132 Posted by: atKa Posted at: 2016-10-18T10:22:06.110Z Reads: 451

```
@JTAG Wow, can´t wait to try one. Seems like its almost  ready for production :)
```

---
## \#133 Posted by: Pantologist Posted at: 2016-10-18T13:05:30.041Z Reads: 452

```
Speaking of production, how did you assemble yours? Did you use a reflow oven or did you use a hot air station and a soldering iron?

Also price per PCB is around $40 on OshPark. I think that is pretty good pricing. Not sure about BOM pricing yet.
```

---
## \#134 Posted by: longhairedboy Posted at: 2016-10-18T14:08:39.064Z Reads: 435

```
i want 10 of these. Seriously.
```

---
## \#135 Posted by: Pimousse Posted at: 2016-10-18T15:47:56.737Z Reads: 443

```
I follow this project since a while, it's good to see HW seems to be ready.
What about SW ?
Do you have a feature list ?
How do you plan to connect it to the VESC ?

Making both BMS and VESC communicate allow tons of awesome features !!
```

---
## \#136 Posted by: Pantologist Posted at: 2016-10-18T16:53:59.099Z Reads: 430

```
Via CAN bus I'm pretty sure.
```

---
## \#137 Posted by: Stevemk14ebr Posted at: 2016-10-18T17:54:33.645Z Reads: 434

```
Bms to vesc communication would be insane. Could setup custom performance profiles for battery charge, statistics streaming through vesc. More data available to vesc the better!
```

---
## \#138 Posted by: Pimousse Posted at: 2016-10-18T21:02:51.312Z Reads: 437

```
According to the thread title, that make sense :smile:
I'm an idiot. :grin:
So the plan would be to have VESC as master and BMS (and second VESC if dual setup) as slaves ?
```

---
## \#139 Posted by: Pantologist Posted at: 2016-10-18T21:06:03.928Z Reads: 443

```
I'm not entirely sure about that. Don't worry I'm an idiot too :confused:

I screwed up my battery now I am desperately trying to make a decent battery and BMS setup again.
```

---
## \#140 Posted by: Kaly Posted at: 2016-10-18T22:08:54.470Z Reads: 466

```
@JTAG nice work on this. 
One thing i that will be nice to have is a **storage mode** to give the battery pack a longer life by avoiding the chemical reactions that take place when the pack is charge +75% and is not use within a couple of days. 

This can be implemented with a 96hr counter that gets activated when the board is power off. After the 96hr the BMS will check the cell voltage and if +75% capacity it will discharge the cells until reaches the storage voltage for the current chemistry. 

Even if the discharge load apply by the BMS it will help avoid the reactions and give longer life to the pack.
```

---
## \#141 Posted by: Pantologist Posted at: 2016-10-18T22:17:55.226Z Reads: 454

```
It would be pretty easy to implement through software I would think. I'd rather have a selectable mode on a bluetooth connect smartphone app. 

My idea is to have a way to talk and get info from both the Vesc and DieBie with one Bluetooth receiver and have an app available to calculate speed, controller data and BMS settings and data. Having charge percentage and notifications popup on the app would be great too.
```

---
## \#142 Posted by: Pimousse Posted at: 2016-10-19T06:43:22.349Z Reads: 417

```
That would be a great feature.
But a discharge mode requires a load (like a resistor) and need some hardware changes and heatsinks I guess.
```

---
## \#143 Posted by: Kaly Posted at: 2016-10-19T13:36:36.261Z Reads: 435

```
It may need just a small heat sink, because the same balancing load can be use for this purpose. 

Even a small load will produce great benefits, because the strategy is for the ions to move to prevent metal plating inside the cell, it's not meant to be a fast process but ratter a continuous one that will stop at storage voltage.
```

---
## \#144 Posted by: JTAG Posted at: 2016-10-19T17:53:39.439Z Reads: 463

```
@atKa
Normally the prototypes I make are 95% ready for production. I only need to fix small bugs + BOM list. So when I think everything is ready (I verified that all the desired functionality is possible) the step to production is small.

@Pantologist
I assembled these two with paste + stencil followed by a reflow oven indeed. Really simple but the result is awesome. Pricing is not bad indeed.

@longhairedboy
You fall in love way to easy, what I showed so far is BORING, the awesome stuff is coming upcoming weeks (I hope).

@Pimousse
Indeed trough CAN. As far as I can see the VESC does broadcasts, the BMS can do the same. The master VESC or any other master on the CAN bus can use all available information to do awesome stuff. Let met do the awesome stuff first, ill start the awesome stuff later :slight_smile:.

@Kaly
Nice thought! For this however the BMS would need a mechanism to turn itself on, currently the uC (and all other stuff) is disabled when the BMS is off (to prevent battery drainage when the battery is stored for a couple of months). For this to work I need to add a system that periodically enables the system. Ill look into this, this periodically enabling the system would allow a lot more than bring the battery to storage level.

@All
The BMS has balance resistors that are designed to drain the battery. It would take several days (depending on the battery capacity) to bring the cell voltages to their nominal voltage but since we can assume the battery isn't going to be used for several days this is no problem.

(My apologies for the bad writing, I am on a train and not focused, ill correct it later).
```

---
## \#145 Posted by: longhairedboy Posted at: 2016-10-19T18:59:51.023Z Reads: 421

```
i'm a sagitarius. everything is glorious or terrible; emotions run high.
```

---
## \#146 Posted by: Pimousse Posted at: 2016-10-20T06:19:40.815Z Reads: 424

```
Awesome news ! :smile:
Can't wait !
```

---
## \#147 Posted by: webst Posted at: 2016-10-22T00:45:57.701Z Reads: 453

```
[quote="longhairedboy, post:145, topic:2639"]
i'm a sagitarius. everything is glorious or terrible; emotions run high..
[/quote]
excuse off topic but, as much it feels home, this is engineering topic on the internet and you just used zodiac

https://d.justpo.st/media/images/2014/01/0a4b9f87176ff8da7134c675e205fbd1.jpg

take no offense, somebody had to do it and i'm gemini :joy:
```

---
## \#148 Posted by: JTAG Posted at: 2016-11-01T20:18:01.682Z Reads: 458

```
Ok lots of progress:

<img src="/uploads/db1493/original/3X/7/1/71205b89a40e3553fc757bdb62d4e7f6759a1a2e.jpg" width="374" height="500">

Me and my brother now both have a BMS mounted to (me) or insite (my brother @MrEpiquad  ) our longboard and are testing it in our everyday commutes. 

Small video of the charging / on / off modes. I even implemented an extremely simple state of charge indicator based solely based on 100%*(consumed Ah)/(battery capacity Ah):

https://youtu.be/dPrGB-z_9Pw
```

---
## \#149 Posted by: MrEpiquad Posted at: 2016-11-01T20:53:11.024Z Reads: 463

```
It's working like a charm so far ! 
No more usage of dangerous cheap chargers from hobbyking.

And it came pretty well together along with the vesc in one enclosure. 
I din't put the bms in the battery enclosure since I want to make the battery modular but with out having to put a bms in each battery pack. :slight_smile:

Here is the bms mounted on a aluminium plate next to the two VESC.
<img src="/uploads/db1493/original/3X/8/d/8db15bf75c610fe6b624e6b7d5b26f81238c50ad.jpg" width="668" height="500">
```

---
## \#150 Posted by: Pimousse Posted at: 2016-11-01T21:12:18.879Z Reads: 442

```
Love to see that !!
How far is the development ? Is the software and hardware ready or do you have still features to add ?
```

---
## \#151 Posted by: Ulfberht Posted at: 2016-11-02T23:38:29.186Z Reads: 435

```
:fist:The Bokma brothers rock! :fist:
Can't wait to see more!
```

---
## \#152 Posted by: boards Posted at: 2016-11-03T05:09:58.604Z Reads: 431

```
Man, I just want to start buying the components now.
```

---
## \#153 Posted by: notger Posted at: 2016-11-08T09:21:50.592Z Reads: 438

```
Holy, shit, i just came across this thread, and this great build.

Respect, i guess thats what may of us are waiting for, at least spoken for me.

Will you announce it here if some "prototypes" are up for grabs ?
Or actually does the BMS allready work as it should without major-changes needed?

One thing that would be nice for me for future developement on the BMS would be that the PCB either gets the Dimensions of the old (4..) or new (5,...6,...) VESC.
That would make it easier to fit and arrange them nicely on (my) board.

thanks for that work 

Notger
```

---
## \#154 Posted by: Garfield Posted at: 2016-11-12T21:19:08.352Z Reads: 426

```
@Nordle My Teensyduino-project is uploaded here is the link https://github.com/RunningPenguin/TeensyWay

@JTAG very nice project glad to see it working. I need one for my self balancing scooter which I build lately. It uses two VESCs and an teensyduino. To get the control software to work I used lead acid batterys but in the future I would update to LiPo or LiFe and need a BMS for that and yours looks really good. I would be very exited to hear from you.

Regards
```

---
## \#155 Posted by: DeathCookies Posted at: 2016-11-24T12:32:13.395Z Reads: 423

```
@JTAG Maybe you want to update your first post?
How is your project going?
Could you implement a feature to level the cells only when the drift is more than 0.5V?
```

---
## \#156 Posted by: JTAG Posted at: 2016-12-07T19:41:30.009Z Reads: 442

```
Sorry for the lack of updates, I had lots of other projects. 

The BMSes are working nicely on our esk8's I did update/added a few things:
* Added SD card holder for logging / debugging -> mainly to develop / evaluate SoC algorithm.
* Added an extra shunt to allow for higher discharge currents -> for future use in EV / solar boat.
* Added a safety shut off -> If the LTC looses its configuration due to a uC brownout or misbehavior the LTC automatically shuts off the power stage.

<img src="/uploads/db1493/original/3X/4/5/45dbd5815a27933fa7bebc452b5115eb39994105.png" width="690" height="302">

<img src="/uploads/db1493/original/3X/1/d/1db9f1190c5325bb7e81354a6413f10538f4ed79.png" width="690" height="298">

I will be sending this design to the fab this week, should be in before xmas :smiley:.
```

---
## \#157 Posted by: FLATLINEcustoms Posted at: 2016-12-07T20:59:37.079Z Reads: 413

```
Beautiful @JTAG
```

---
## \#158 Posted by: Ulfberht Posted at: 2016-12-10T04:58:07.844Z Reads: 418

```
Very Nice indeed...
:robot::v:
```

---
## \#159 Posted by: Garfield Posted at: 2016-12-10T16:56:37.220Z Reads: 429

```
Looks really nice to me.
```

---
## \#160 Posted by: ACIN Posted at: 2016-12-10T17:08:50.833Z Reads: 444

```
http://images-cdn.9gag.com/photo/99823_700b.jpg
```

---
## \#161 Posted by: Garfield Posted at: 2016-12-10T18:59:29.948Z Reads: 433

```
@JTAG Looks very clean to me. Great work.
```

---
## \#162 Posted by: B4Me Posted at: 2016-12-13T07:50:47.889Z Reads: 409

```
Is it a safety shutoff if you're on an esk8, and it gets a brownout.. now you cant brake anymore :open_mouth:
Shouldn't it be possible to choose the corresponding safety state of the switch ?
```

---
## \#163 Posted by: ThomasRBK Posted at: 2016-12-13T08:11:35.441Z Reads: 403

```
@JTAG First time I see this thread but what you did so far is amazing man, keep up the good stuff! When they're available for sale I'll get one for sure :slight_smile:
```

---
## \#164 Posted by: JTAG Posted at: 2016-12-13T08:31:41.795Z Reads: 404

```
I got scared and a little bit more cautious due to the recent BB battery fires xD. I is a watchdog controlled safety, so no direct (cell based) voltage switching happening.
```

---
## \#165 Posted by: B4Me Posted at: 2016-12-13T10:00:13.032Z Reads: 392

```
Awesome, just got a littel worried, as burning batteries is better than dead skater ;)
```

---
## \#166 Posted by: WrinklyWink Posted at: 2016-12-15T17:11:47.408Z Reads: 398

```
ordered a bms, got lost in the mail, got refunded, now I see this. I would like to purchase, How much and when?
```

---
## \#167 Posted by: psychotiller Posted at: 2016-12-15T17:23:05.060Z Reads: 405

```
I just read this whole thread. Super amazed and intrigued.

Nice work!!!
```

---
## \#168 Posted by: bjorntsc Posted at: 2016-12-22T00:02:37.631Z Reads: 403

```
Looks awesome!
How close are you to testing the newest board?
Any Idea when you may be ready to sell a few for testing?
```

---
## \#169 Posted by: JTAG Posted at: 2016-12-22T00:36:53.121Z Reads: 452

```
The new PCB's just arrived! I have lots of people to answer, please be patient I am quite busy te lasts weeks :sweat:.

Some pictures for amusement:
<img src="/uploads/db1493/original/3X/b/f/bfeee9024636567ab17b243e3de78717450f4acb.jpg" width="666" height="500">
<img src="/uploads/db1493/original/3X/0/c/0c1fd25b4f96147fd9f612048a06670d64fbf0bb.jpg" width="666" height="500">
<img src="/uploads/db1493/original/3X/f/f/ff3d42793928d40a50925dccc1aea642081266ed.jpg" width="666" height="500">
<img src="/uploads/db1493/original/3X/6/6/6682cfcb205dd975324ec5b14b5029c8f3c3a672.jpg" width="666" height="500">
```

---
## \#170 Posted by: bjorntsc Posted at: 2016-12-23T11:07:17.900Z Reads: 408

```
That looks really clean!

Happy Holidays/Christmas!
```

---
## \#171 Posted by: JTAG Posted at: 2017-02-16T15:04:47.636Z Reads: 398

```
Is there an admin around? Why cant I update/edit my opening post?
```

---
## \#172 Posted by: Maxid Posted at: 2017-02-16T15:30:17.936Z Reads: 383

```
when the topic gets too old you can't change it anymore.
```

---
## \#173 Posted by: laurnts Posted at: 2017-02-19T21:13:19.409Z Reads: 382

```
@JTAG What do you need help for? :D
```

---
## \#174 Posted by: JTAG Posted at: 2017-02-21T09:11:37.451Z Reads: 387

```
Thanks for the reply, I wanted to update the link to the schematic in the OP, I now fixed it on Github, so no need for an update anymore. 

(not towards you but):
I still find it undesired that I cant update posts from the past since I might change specifications a little or would like to make some things clearer. It seams that I have to live with it :stuck_out_tongue:.
```

---
## \#175 Posted by: laurnts Posted at: 2017-02-22T09:35:48.019Z Reads: 377

```
I believe its because people already read that before and it's "kind of unfair" if they read and you change it without the past reader knowing the content has changed. Discourse its a partial blog, so its also weird if you have a past and then you changed that. Than all of the comments / discussions underneath it becomes irrelevant. I dont know how best explained it, but I think you understand what I meant.
```

---
## \#176 Posted by: fuelre Posted at: 2017-02-22T10:11:18.044Z Reads: 372

```
it would make sense to refer from in the first post to the postnumber with the updated spec/news. or place a link to the post
```

---
## \#177 Posted by: Gromok Posted at: 2017-03-04T09:05:37.073Z Reads: 372

```
Your BMS is on my shopping list.

Will order one, once it is in production and out of beta.
```

---
## \#178 Posted by: mt37 Posted at: 2017-03-07T22:29:29.912Z Reads: 377

```
@JTAG Are you taking pre-orders ? :slight_smile:
```

---
## \#179 Posted by: Brad Posted at: 2017-04-09T09:42:24.815Z Reads: 377

```
Update on current status? On hold or ?
```

---
## \#180 Posted by: Okami Posted at: 2017-04-09T23:08:44.613Z Reads: 410

```
yeh, post some more info! @JTAG  

And also update the topic's name, please, if it is still possible.. The topic was here all the time but only now I managed to read it after @tomtom13 stirred up the situation :D 

Though.. im sure you will create a new topic maybe.. once you get to the 'distribution' part for these bms's.. 

**Do you have an estimate how much they might cost per unit?**
```

---
## \#181 Posted by: tomtom13 Posted at: 2017-04-09T23:15:55.953Z Reads: 457

```
Just, anybody don't take my crapy topic as a means of diverting you from @jtag BMS. It has a lot of stuff that I would be looking for in BMS (looks like it has a distribution unit - some people call it soft switch). So it's a lot better than my crack pipe dream of bms with esp :)
```

---
## \#182 Posted by: JTAG Posted at: 2017-04-10T01:42:34.582Z Reads: 491

```
@Okami the estimate cost is 100 euro each when you make 6. 

Small update:

We made 6 BMS's for evaluation, we plan to mount them on our skateboards and electric scooters:
<img src="/uploads/db1493/original/3X/c/7/c7acda7f7b8ba9373a564c9dc2784e3638ac05f5.jpg" width="666" height="500">

<img src="/uploads/db1493/original/3X/4/1/4102648c09b09f2ef66c54c1a85ef0ef64567769.jpg" width="666" height="500">

<img src="/uploads/db1493/original/3X/2/b/2bfdc15bf6304ce45fff8b06092d311b24826a07.jpg" width="666" height="500">

<img src="/uploads/db1493/original/3X/8/2/828561a5057b827e9b5f7a2f52bb48d51e0608f7.jpg" width="666" height="500">

<img src="/uploads/db1493/original/3X/7/9/793cf79b638918f9c226c80f6a4ff8a314735713.jpg" width="666" height="500">

<img src="/uploads/db1493/original/3X/8/d/8d8e2fc96e57e2ca437bba46b9bbde7749dc31b1.jpg" width="666" height="500">

<img src="/uploads/db1493/original/3X/2/4/24c3aa5bd3b614dba602ea7d90259ea844acc222.jpg" width="666" height="500">

<img src="/uploads/db1493/original/3X/b/7/b78943b1ebea5dcbb9a9f9d2395e05903bec8c9d.jpg" width="666" height="500">

I have no plans on commercially selling these BMS's now or in the future. I just like sharing everything such that maybe someone else can benefit from it. Maybe in the future if my redesign of the VESC 6.0 is going to work I might join a webshop and start producing esk8 electronics, but so far the financial risk is to high for this :pensive:.
```

---
## \#183 Posted by: Stevemk14ebr Posted at: 2017-04-10T02:40:38.880Z Reads: 445

```
Setup a liscensing deal with a manufacturer on here. Something simple, you get X% of profits with contingency you are not liable and have no responsibility to provide upgrades, fixes, or otherwise do further work. If you wish to allow others on here to enjoy your work that's an easy win, win. If not still good stuff here
```

---
## \#184 Posted by: PXSS Posted at: 2017-04-10T02:49:54.746Z Reads: 442

```
Are you planning to open source it atleast so maybe a few of us can build our own?
I would be interested in DIYing a couple or myself and my gf.
```

---
## \#185 Posted by: JTAG Posted at: 2017-04-10T03:02:46.698Z Reads: 446

```
It's open source:

From the OP:
Tracked in github (still in a very early stage):
https://github.com/DieBieEngineering/DieBieMS
```

---
## \#186 Posted by: chsknight Posted at: 2017-04-12T07:18:25.869Z Reads: 424

```
How's version .4?  Is it good it enough to make a board or two or does it need more testing?
```

---
## \#187 Posted by: katodo Posted at: 2017-06-12T15:14:42.139Z Reads: 384

```
Hi, how can I build a pcs?
```

---
## \#188 Posted by: katodo Posted at: 2017-06-14T06:51:54.059Z Reads: 386

```
Hi, How can I try to build source code? I've founded it on https://github.com/DieBieEngineering/DieBieMS-Firmware

Can I build it with Eclipse and GCC or "System Workbench for STM32" suite ?
```

---
## \#189 Posted by: Minim Posted at: 2017-06-18T22:01:03.547Z Reads: 386

```
This really looks like the perfect BMS system. Is anyone going to order a bulk of these assembled? If so im up for it and I don't mind a early beta software if I can contribute with the code myself also. 

An idea I have that isn't mentioned yet (as I can see) is to have an option to use storage mode that limits the charge. I'm not thinking about a discharge circuit but more like a software feature. It can be a feature you activate when you know you are going to leave the board for a while and then you can ride it to discharge it (warning will be sent at XX%) and then when it's charging again it will stop at storage voltage. I do this manually with my Tesla now and keep charge state between 50-80% to keep the battery good shape longer. When doing long trips I charge to 100% right before departure so it never sits at 100% over a long period. 

Another feature if a braking resistor was added is the possibility to have better brakes at high SOC and limit overvoltage to the battery by letting it go into heat. Would also make it possible with auto storage mode. It will take up a lot of space tho with heat sink, therminals, components and whatnot so prolly not worth it since space is often a problem.
```

---
## \#190 Posted by: Pantologist Posted at: 2017-06-18T22:57:43.837Z Reads: 355

```
I asked him about adding a braking resistor and I think he said it was not worth the extra space to add it but it would be easier to implement into the ESC rather than the BMS.
```

---
## \#191 Posted by: Brad Posted at: 2017-07-11T11:21:46.404Z Reads: 368

```
I read through this thread and could not find an answer on whatever the balancing is only done when the charge limit is reached. 

One of the only downsides to partial charging is that many inexpensive battery management system (BMS) circuits will only do active bleed balancing of the cells when they are at or near the full charge voltage of 4.2 V/cell. 

This means that with partial charge profiles that don’t reach that voltage, the BMS circuit will never be able to re-balance cells if they are drifting apart. This issue it can be easily remedied by occasionally (like once every month or two) leaving the pack connected to a 100% charge cycle overnight. I just would rather not have to do that if I can help it!

Over time you may have less available capacity from the pack as certain cells will hit the low voltage cutoff on discharge well before others.

Would your DieBie BMS do charge balancing immediately? Good quality programmable BMS circuits will usually attempt to balance the cells whenever they see more than a certain voltage spread between the highest and lowest cell in the group, and in that case there is no problem with partial charges.
```

---
## \#192 Posted by: longhairedboy Posted at: 2017-07-11T12:32:24.172Z Reads: 366

```
I want to participate in this beta if it happens. This is something that is desperately needed.
```

---
## \#193 Posted by: jos Posted at: 2017-07-11T12:52:11.032Z Reads: 369

```
It is happening as we speak:
http://www.electric-skateboard.builders/t/diebie-jtag-12s-bms-gauging-interest-nonprofit/20947

If you are quick I think there's still time to get in on the action :slight_smile:
```

---
## \#194 Posted by: lock Posted at: 2017-07-11T13:14:35.692Z Reads: 369

```
[quote="Brad, post:191, topic:2639"]
Would your DieBie BMS do charge balancing immediately?
[/quote]
Just looking at the source code. There's a `cellBalanceStart` config parameter, and it looks like no balancing is performed till a cells voltage exceeds this. Cells are sorted so that the highest voltage cells are discharged first, it also seems to limit the number of cells discharging at any one time (another config param). I'm sure there's a good reason why you don't want to be discharging too many cells at once?

Not quite sure what setting the `cellBalanceStart` to a low value would do. Slow the charging process, flames?

[quote="Brad, post:191, topic:2639"]
Good quality programmable BMS circuits will usually attempt to balance the cells whenever they see more than a certain voltage spread between the highest and lowest cell in the group, and in that case there is no problem with partial charges.
[/quote]

From a software point of view it seems it would be very easy to do something like this. The function that does this already has an array of the cell voltages, you'd just need to change an `if` statement.
```

---
## \#195 Posted by: JTAG Posted at: 2017-07-11T13:18:21.246Z Reads: 377

```
When the charger is connected balancing starts when a cell voltage exceeds "defaultConfig.cellBalanceStart" and when the mismatch is more than "defaultConfig.cellBalanceDifferenceThreshold" . On all my electrical transportation vehicles where I use my BMS the balancing part takes about 20 minutes (the display indicates balancing during that period), once the displays indicates charged all cells are balanced. 

So yeah, I start balancing quite early ( in my opinion >3,8V cell is early ) and once stated "charged" all my devices have a full cell voltage matched pack (<5mv mismatch). When you leave the system connected to the charger even when it states charged the bms will balance even further.

You could start balancing even earlier (for example always when charger is connected), this will backfire you since you will be discharging cells that would eventually ended up to being matched (but are brought to imbalance by your attempt to balance), so there is a sweet spot (that isn't at the end and isn't at the beginning). The whole problem we attempt to solve with balancing is (when you started witch a matched pack & in my opinion) -> compensate for the temperature mismatched you had during charging and discharging + the imperfections you have in your cells (that converts either charge/discharge currents to heat). As long as the imperfections are minimal balancing will be easy since the mismatch created by the temperature imbalance are minimal. The imperfections (caused by defects in the cell) are a bitch, they will need a big effort (balancing time) to compensate since their impact can be huge (cause a big energy imbalance). 

The worst parallel cell combination determines the total Ah of your pack, it is thus key to have all imperfections matched (this its the case with new cells or cells that all had the same abuse :stuck_out_tongue: ), (same energy capacities), (every cell should have the same state of health). A BMS will not fix a crappy battery pack, a BMS will do its best to protect a pack against the environment to prevent it to become crappy by abuse from its user :smiling_imp:. The BMS will tell to user the lowest cell voltage is under a limit, you should no push your board you lazy basterd! Even when you don't like to push.

TLDR;
The main goal of a BMS: make a battery pack save enough (protect it against a user) to be used as a energy storage media (prevent). Every other benefit is just a bonus :grin:. 




	defaultConfig.noOfCells 																=	4;														// 4 Cells in series
	defaultConfig.batteryCapacity														=	80.00f;												// 80Ah battery
	defaultConfig.cellHardUnderVoltage											= 2.40f;												// Worst case X.XXV as lowest cell voltage
	defaultConfig.cellHardOverVoltage												= 4.45f;												// Worst case X.XXV as highest cell voltage
	defaultConfig.cellSoftUnderVoltage											= 2.70f;												// Normal lowest cell voltage 2.7V
	defaultConfig.cellSoftOverVoltage												= 4.10f;												// Normal highest cell voltage 4.10V
	defaultConfig.cellBalanceDifferenceThreshold						=	0.005f;												// Start balancing @ 5mV difference, stop if below
	defaultConfig.cellBalanceStart													= 3.80f;												// Start balancing above 3.8V
	defaultConfig.cellBalanceUpdateInterval									= 4*1000;												// Keep calculated resistors enabled for this amount of time in miliseconds
	defaultConfig.maxSimultaneousDischargingCells						= 5;														// Allow a maximum of 5 cells simultinous discharging trough bleeding resistors
	defaultConfig.timoutDischargeRetry											= 4*1000;												// Wait for X seconds before retrying to enable load.
	defaultConfig.hysteresisDischarge 											= 0.02f;												// Lowest cell should rise 20mV before output is re enabled
	defaultConfig.timoutChargeRetry													= 30*1000;											// Wait for 30 seconds before retrying to enable charger
	defaultConfig.hysteresisCharge													= 0.01f;												// Highest cell should lower 10mV before charger is re enabled
	defaultConfig.timoutChargeCompleted											= 30*60*1000;										// Wait for 30 minutes before setting charge state to charged
	defaultConfig.timoutChargingCompletedMinimalMismatch 		= 6*1000;												// If cell mismatch is under threshold and (charging is not allowed) wait this delay time to set "charged" state
	defaultConfig.maxMismatchThreshold											= 0.020f;												// If mismatch is under this threshold for timoutChargingCompletedMinimalMismatch determin fully charged
	defaultConfig.chargerEnabledThreshold										= 0.2f;													// If charge current > 0.2A stay in charging mode and dont power off
	defaultConfig.timoutChargerDisconnected									= 2000;													// Wait for 2 seconds to respond to charger disconnect
	defaultConfig.minimalPrechargePercentage								= 0.80f;												// output should be at a minimal of 80% of input voltage
	defaultConfig.timoutPreCharge														= 300;													// Precharge error timout, allow 300ms pre-charge time before declaring load error
	defaultConfig.maxAllowedCurrent													= 120.0f;												// Allow max 120A trough BMS
	defaultConfig.displayTimoutBatteryDead									= 5000;													// Show battery dead symbol 5 seconds before going to powerdown in cell voltage error state
	defaultConfig.displayTimoutBatteryError									= 2000;													// Show error symbol for 2 seconds before going to powerdown in general error state
	defaultConfig.displayTimoutSplashScreen									=	1000;													// Display / INIT splash screen time
	defaultConfig.maxUnderAndOverVoltageErrorCount 					= 5;														// Max count of hard cell voltage errors
	defaultConfig.notUsedCurrentThreshold										= 0.5f;													// If abs(packcurrent) < 500mA consider pack as not used
	defaultConfig.notUsedTimout															= 30*60*1000;										// If pack is not used for longer than 30 minutes disable bms
	defaultConfig.stateOfChargeStoreInterval								= 60*1000;											// Interval in ms to store state of charge information
```

---
## \#196 Posted by: JTAG Posted at: 2017-07-11T13:34:38.943Z Reads: 363

```
[quote="lock, post:194, topic:2639"]
Cells are sorted so that the highest voltage cells are discharged first, it also seems to limit the number of cells discharging at any one time (another config param). I'm sure there's a good reason why you don't want to be discharging too many cells at once?
[/quote]

Hahaha, yeaaaaaaaaah there is xD, I found out the hard way; balance resistors convert energy to heat, in the worst case (4.2^2)/15=~1.2W of heat times 11 cells = 13.2W of heat. This is an awfully lot if enclosed in a small space, the area is just to small. In my early stage of software development discovered that some sort of throttling is desired.

I made this max amount of active balance resistors configurable to allow for different environments (temperatures) and other values of resistors. Maybe in to future it could become a self learning parameter since there is a temperature sensor inside the LTC, but hey self learning is scary, the current solution works and there are more important / fun things to engineer. 

You might think: well, if your board gets to hot with to much resistors enabled why don't you use a larger resistor? Will this will increase in either size or cost. 

The other reason; only a small amount of cells will be out of balance (for all of my 12S packs always the same 4 cell are mismatched, but you want them to discharge / match fast, hence the desire for the lower resistance). You will always be bypassing / discharging the same limited amount. Only in limited circumstances you need to discharge more, for example when you just connected a new pack, then it will only take more time. 

Again a place/case where there is no perfect situation / solution, I however tried to approach the best case.
```

---
## \#197 Posted by: Brad Posted at: 2017-07-12T01:41:11.139Z Reads: 340

```
Starting the balance at 3.8 volts would be fine cos I just wanted to stop charging at 4.1 volt for battery longevity.

Your post was an interesting read.
```

---
## \#198 Posted by: JTAG Posted at: 2017-07-31T23:52:14.020Z Reads: 371

```
Ok, I found some time again to put a few extra features to onto the BMS.

* The bootloader button was useless, I read the documentation wrong with the first iteration and wrongly assumed that my chosen uController had a hardware bootloader on UART2, it doesn't so the boot button could go (I will port the VESC bootloader to the BMS).
* I removed the holes that could have been used to mound the OLED display. I discovered that it was useless since I never used it since the display if any will go into the cover / enclosure.

<img src="/uploads/db1493/original/3X/0/2/02002c471a6e5d50116e86a1b6152f8a814b1a2a.png" width="690" height="320">

<img src="/uploads/db1493/original/3X/e/3/e3731620b2284e09175945c2e73a6ff7cc060ece.png" width="690" height="320">

* I added a NTC close to the switching transistors to protect them from overheating when the hi-amp power draw is to long.
* And for me the long awaited optional feature: A sub-ghz RF tranceiver :D :D :D (I want to design a remote in the future).

This one in 915 MHz:
https://www.anaren.com/air/products/868mhz-solutions
```

---
## \#199 Posted by: Pantologist Posted at: 2017-08-01T05:29:20.421Z Reads: 339

```
Will these revisions be updated for @fedestanco 's group buy?
```

---
## \#200 Posted by: fedestanco Posted at: 2017-08-01T11:09:48.380Z Reads: 339

```
Yes. Jtag contacted me in advance telling me to wait few more days for getting the new production files.
```

---
## \#201 Posted by: JTAG Posted at: 2017-08-01T11:12:02.368Z Reads: 341

```
Yes that's the plan!

But without the transceiver, that part is costly and is still in the development stage, even for me. Once it's useful you can add/solder it on later. 

I hope to finish the BOM and design rule check today.
```

---
## \#202 Posted by: fuelre Posted at: 2017-08-01T16:20:16.333Z Reads: 314

```
@JTAG:
the 915MHz band is only in America a ISM band -> not allowed to use it in the rest of the world except you have a HAM licence
other than that - nice BMS!
```

---
## \#203 Posted by: JTAG Posted at: 2017-08-01T17:13:36.089Z Reads: 317

```
For other countries there are other module of the same type:

https://www.anaren.com/air/products/air-proprietary-rf-apps

All have the same footprint.
```

---
## \#204 Posted by: karma Posted at: 2017-08-17T12:35:07.367Z Reads: 312

```
@JTAG Will there be a beta for this project ? :)
```

---
## \#205 Posted by: JTAG Posted at: 2017-08-17T14:24:38.456Z Reads: 318

```
I personally wont be producing / selling the BMS on the short term, maybe in the future :sweat_smile:.

There might appear other that produce it like these:
http://www.electric-skateboard.builders/t/diebie-jtag-12s-bms-gauging-interest-nonprofit/
```

---
## \#206 Posted by: chinzw Posted at: 2017-08-18T17:07:08.270Z Reads: 305

```
@JTAG quick question, will the bms allow to charge a pack with higher voltage than the charger? Like if i want to charge 12s pack with 25.2v charger ?
```

---
## \#207 Posted by: JTAG Posted at: 2017-08-18T21:20:30.272Z Reads: 319

```
Nope, the charger has to have a higher (about 3V isch) voltage than then battery, preferably at all times. The BMS does not boost the voltage.
```

---
## \#208 Posted by: JTAG Posted at: 2017-08-18T21:40:05.004Z Reads: 349

```
Latest PCB came in!

<img src="/uploads/db1493/original/3X/c/2/c2c73686fdd50a19ce0e8056c7c6b096919925dc.jpg" width="666" height="500">

<img src="/uploads/db1493/original/3X/d/a/dae28508b27e2cffb140122322d3b11e86ad84be.jpg" width="666" height="500">

<img src="/uploads/db1493/original/3X/e/b/ebd4156b15a4b3539eb9bc701cd3510143b140c3.jpg" width="666" height="500">

<img src="/uploads/db1493/original/3X/4/c/4c834c550654a7c5cddd7661981454c006874f8f.jpg" width="666" height="500">
```

---
## \#209 Posted by: chinzw Posted at: 2017-08-18T21:52:17.484Z Reads: 315

```
@JTAG hmm, so i'd need a 60v give or thake charger for 12s then?
```

---
## \#210 Posted by: JTAG Posted at: 2017-08-18T22:25:49.445Z Reads: 315

```
Any 48V PB battery charger will do. 48V battery charges (all will be oriented to charge 4 lead acid batteries in series) will have a high enough open clamp voltage to trigger the charger detect mechanism on the BMS. This is what I use on my E-Scooter. 

The minimal open clamp voltage to automatically detect the charger with a full battery will be 12*4.2+3=53.4V. A voltage between 53.4V and 60V will be fine.
```

---
## \#211 Posted by: lock Posted at: 2017-08-18T23:11:44.650Z Reads: 314

```
Or 3.6*12+3 = 46.2 if your batteries max out at 3.6v? Hoping this is modifiable via settings 😬
```

---
## \#212 Posted by: JTAG Posted at: 2017-08-19T00:08:58.013Z Reads: 327

```
[quote="lock, post:211, topic:2639"]
es m
[/quote]

Yes, exactly! All voltages are configurable.

In my example I assumed the most common li-ion isch voltage. What chemistry do you use?
```

---
## \#213 Posted by: lock Posted at: 2017-08-19T01:57:11.460Z Reads: 334

```
Cool, this was one of the main reasons I really liked this BMS; it'll support my current chemistry and any others if I change my mind in future. Battery pack is a 12S2P A123 26650 LiFePO4 setup.
```

---
## \#214 Posted by: JTAG Posted at: 2017-09-04T17:47:13.817Z Reads: 359

```
Ok, I finally had time to build and evaluate my latest design, I found a very small improvement and fixed it right away (I had the wrong value resistor next to the NTC) in the design. So for everyone that wants to make a DieBieMS; you are good to go!

This latest revision has an NTC close to the switching logic (to intervene with possible overheating of the switching logic) and an optional Anaren transceiver that could be used as a receiver for a remote :grin: (I really like this optional feature).

I tested the NTC and the communication to the transceiver and they both seem to work. 

This board is not fully populated, I couldn't find the parts for the sections of the board with missing parts (TVS diodes and the display connector), those sections however did not change and were already proven to work in the previous versions.

I couldn't find the tool to insert the press fits all the way but really wanted to start testing. Once all components are in and I pressed the pressfits all the way ill post a pic (again, this has no influence on the functionality).

Thanks for everyone's patience so far!

<img src="/uploads/db1493/original/3X/7/3/731368326c17205736901043489aa7187203d1b4.jpg" width="666" height="500">

<img src="/uploads/db1493/original/3X/5/8/584ac4e53ab75143d471828600982f477336eb63.jpg" width="666" height="500">

<img src="/uploads/db1493/original/3X/b/a/ba48ff7760ca09746001785cb841c634224f51bf.jpg" width="666" height="500">

<img src="/uploads/db1493/original/3X/b/a/bab6f2172fca4946993716553700ca083a35b07f.png" width="690" height="310">

<img src="/uploads/db1493/original/3X/9/e/9e641978b0e62a505237174a9c5b8e3d8e5f7f0f.png" width="690" height="308">
```

---
## \#215 Posted by: Johnj143 Posted at: 2017-10-22T19:33:15.123Z Reads: 311

```
@fedestanco are these boards still available to buy? Will you be making another order?
```

---
## \#216 Posted by: JTAG Posted at: 2017-10-23T08:54:15.924Z Reads: 320

```
[quote="JdogAwesome, post:228, topic:20947, full:true"]
Hey @JTAG your devolpment on these things is just amazing, great work! I'm just curious on why you opted for a STM32F4 microcontrollers instead of something like a F1 or even a small 8 bit IC because of the low CPU load a BMS has? Also you should go with the IRFS7730 instead of the 7734 it's RDSon is only 1.7-2 instead of the like 3Mohms the 34 has. Other than that it looks awesome and I think the DIY community really needs a good DIY BMS.
[/quote]

In my latest design I use the 7730, I might have used the other FET in older designs/prototypes but the 7730 should be in the new.

What is the benefit of having a F1 instead of the F4? You have freedom now to implement almost everything you want. In the future features might be added ( like a receiver as on my latest design ) and maybe logging (also possible on my latest design ). The added cost and power usage was in my opinion negligible compared to the value of more computational power (but that is just my opinion, I might have overlooked something).

Thanks for analysing and help!

This was a reply in this topic:
https://www.electric-skateboard.builders/t/diebie-jtag-12s-bms-gauging-interest-nonprofit/20947
I wil try and aim to keep most of the technical information here else everything might get scattered around.
```

---
## \#217 Posted by: JdogAwesome Posted at: 2017-10-23T15:22:55.079Z Reads: 301

```
That makes sense, similar reason to Vedders choice of the F4 for the VESC. And the only benefit of the F1 or other smaller microcontollers was price and power consumption but for this application I suppose it doesn't really matter. Though on that topic what is the standby power of this BMS? Im assuming the F4 has a very low power sleep state and thats what its in most of the time yes? Anyways thanks for responding!
```

---
## \#218 Posted by: JTAG Posted at: 2017-10-23T16:38:19.419Z Reads: 312

```
Look at the schematic, once powered down the whole board except for a couple of multi meg ohms is disconnected. The sleep power of the MCU doesn't matter since its completely disconnected from the batter :heart_eyes:.
```

---
## \#219 Posted by: Johnj143 Posted at: 2017-10-31T05:19:00.970Z Reads: 321

```
When will the next batch of BMS’s start up?
```

---
## \#220 Posted by: JTAG Posted at: 2017-11-13T23:43:08.802Z Reads: 357

```
Hi Everyone!

I have been crazy busy working on more projects than I can handle :sweat:. The resent developments with the group buy, some of my friends I sold a BMS to for their skateboard asking to configure / customize it and a personal project (efoil) had me to focus for the last two days on implementing a basic way of status reporting and customizing the BMS trough a UI.

And with the help of the world of opensource I represent to you; a crudly simple way to configure the BMS (for now). Of course I (or we :innocent:) will be realising a decent UI but for now this should provide basic functionality:

<img src="/uploads/db1493/original/3X/a/8/a8898a4466c8a1727f1fff00b2a1ed410024698b.png" width="690" height="434">
The firware version is incorrect, but I have to set it like this to trick the VESC-Tool to allow me to use the terminal.

I implemented the communication style of the VESC, this will make it crazy easy to (in the future) configure all esk8 electrical components over the same CAN bus, for now only USB is supported (no CAN, no firmware upgrade, no UI yes) in collaboration with the VESC-tool and its terminal. I am eager to start implementing firmware upgrade and CAN functionality but I simply was unable to finish it on time for the group buy to start shipping (sorry guys :sweat:).

I was however able to implement cell voltage status report generation over terminal:
<img src="/uploads/db1493/original/3X/f/9/f9ac402f8a6ac35010be310ce270ed7f485a8a05.png" width="690" height="469">

Battery summary report:
<img src="/uploads/db1493/original/3X/7/d/7de9753617586c358260e5229353e6e9c5b76169.png" width="461" height="500">

Change settings:
<img src="/uploads/db1493/original/3X/e/e/ee7b4d0ed1ac297f3575e41abdb7cdf9fbfbc2a3.png" width="626" height="500">

Like:
pack amp hours
cells in series
soft and hard under and over voltages (determines the (dis)charge enable moments and error states).
can id (for the future)
cell voltage threshold to start balancing
cell mismatch balance start threshold

And reports a help info block:
<img src="/uploads/db1493/original/3X/c/c/ccc0919805cf10574f3b6bb1aad2c7e8c8d6af41.png" width="516" height="500">

More to come! Thanks for you patience everyone :blush:.
```

---
## \#221 Posted by: Pedrodemio Posted at: 2017-11-13T23:50:29.872Z Reads: 320

```
@JTAG Would be possible to port your firmware to @raphaelchang BMS? At least part of it? If you say so I think I will try that since Raphael vanished and left us with non working boards
```

---
## \#222 Posted by: lock Posted at: 2017-11-14T00:13:06.407Z Reads: 314

```
Oh man. This hack is even more epic than the hack I posted over in the other thread 😂. I love it!
```

---
## \#223 Posted by: Pimousse Posted at: 2017-11-14T05:17:23.220Z Reads: 315

```
About @raphaelchang 's BMS, perhaps is there someone n the shadow working on it ? ;)
I'm mean, "in the shadow" is even not true because he keeps people updated and asked for support ;)

Anyway, the VESC Tool trick is an amazing idea.
I keep this idea in the corner "in case of".
Really nice work !
```

---
## \#224 Posted by: Pedrodemio Posted at: 2017-11-14T11:24:27.187Z Reads: 311

```
I really hope, i planned to help put things moving, but since the connection for debugging is only working on mac i've put it aside and ordered a cheap BMS from aliexpress

@JTAG do you have the schematic somewhere? the link is not working and i couldn't find on GitHub

thanks
```

---
## \#225 Posted by: JTAG Posted at: 2017-11-14T12:30:25.490Z Reads: 307

```
https://github.com/DieBieEngineering/DieBieMS/blob/master/DB10005_DieBieMS.pdf
```

---
## \#226 Posted by: Pimousse Posted at: 2017-11-14T12:53:11.721Z Reads: 325

```
No worries. ;)
I'm a early beginner into C coding so it's a big amount of work to train myself (reading books or studiyng other codes like @JTAG or Vedder's's one ) and to gain knowledge (or remembering as I had some lithium batteries courses at university) about the way to manage charging/balancing.

ATM, I wrote A LOT of code (including charge/balance storage, CAN bus with VESC, UI, SoC, voltage SAG calculation and so on) but I'm still in the process of building a bench to try all this fresh and non-debugged code with safety.

Sorry JTAG for this off topic. :slight_smile:
```

---
## \#227 Posted by: chsknight Posted at: 2017-11-14T17:52:05.801Z Reads: 327

```
Should we be using the IRFS7730 instead of the IRFS7530 found in the latest BOM?
```

---
## \#228 Posted by: lock Posted at: 2017-11-15T04:40:20.577Z Reads: 331

```
There's a serial port under the board. Would it be possible to wire up one of those HM-10 Bluetooth modules?
```

---
## \#229 Posted by: chinzw Posted at: 2017-11-15T06:07:31.406Z Reads: 341

```
the board has can bus, so yes
```

---
## \#230 Posted by: JTAG Posted at: 2017-12-11T19:44:37.490Z Reads: 348

```
<img src="/uploads/db1493/original/3X/7/b/7be94fdb91e2f9ab437f5971f963b404ad057341.jpg" width="690" height="239">

<img src="/uploads/db1493/original/3X/f/0/f04299634f584cd628b87dea4776ba09906c96d4.png" width="690" height="341">

<img src="/uploads/db1493/original/3X/b/5/b5addc011b0cfb1911ccb8f6393436b608bdbeb3.png" width="690" height="348">

<img src="/uploads/db1493/original/3X/5/7/57f573f763348473f4f055f276d01dff6f1947e2.jpg" width="690" height="242">

By a customer's request; a shield that adds 6 temperature sensors, a DC - DC converter (for 12V on the can bus), 4 fans with rpm control, buffered IO, relay driver, additional pre-charge method and shunt to allow currents up to 250A :heart_eyes:.

This will be perfect for applications that require a bit more power or "MoreAmps" :sunglasses:.

Once the design is tested and my customer is OK with it ill opensource as well.
```

---
## \#231 Posted by: banjaxxed Posted at: 2017-12-31T13:53:50.430Z Reads: 323

```
Superb thanks for your contributions @JTAG 

I'm hamfistedly putting together a small case for the bms, I'm almost certertain that I should make room for an anti-spark there too? My electrics are in vesc cases by @Kug3lis and cells in nese cases by @agniusm
```

---
## \#232 Posted by: JTAG Posted at: 2017-12-31T14:09:07.242Z Reads: 327

```
[quote="banjaxxed, post:231, topic:2639"]
lls in ne
[/quote]

No need for anti spark, it is all build into the BMS, the pre-charging and the switching :innocent:.
```

---
## \#233 Posted by: banjaxxed Posted at: 2017-12-31T14:14:49.945Z Reads: 326

```
Oh man so cool thanks
```

---
## \#234 Posted by: banjaxxed Posted at: 2017-12-31T16:08:48.507Z Reads: 329

```
Fumbling, ta for the scad & yes the XLR is going to be replaced by laptop charge port

<img src="/uploads/db1493/original/3X/5/4/546012d7d7ffe0a55c7b1f6a5e38f027c0b6a0af.png" width="550" height="500">
```

---
## \#235 Posted by: JTAG Posted at: 2017-12-31T21:32:17.880Z Reads: 328

```
Fancy! 

XLR can be used as a charging plug, a friend of mine did it and it worked fine.

It is unclear to see but the balancing leeds might need some more room to get into a right angle radius, this gets me as well sometimes.
```

---
## \#236 Posted by: banjaxxed Posted at: 2017-12-31T23:24:24.071Z Reads: 318

```
I decided to make 2 holes and n front of the balance lead port, I will split the leads into two silicone tubes running up the 'spine' of @agniusm's packs

The xlr panel was too large, by itself it would raise the enclosure height another 5-10mm so reverted back to a laptop port 5.5mmx2.5mm iirc, the thread for this should be about 10mm so that's what I'm printing right now HNY!

Ps: all being good once design is acceptable I will publish and link here my feeble attempt 👌☘️
```

---
## \#237 Posted by: banjaxxed Posted at: 2018-01-01T13:43:04.238Z Reads: 316

```
Will be delayed prototyping as printer has a bed problem and have to leave for work tomorrow so HNY all will have something by next weekend

If delay is bad I picked up the initial case design on thingiverse
```

---
## \#238 Posted by: banjaxxed Posted at: 2018-01-04T22:13:44.243Z Reads: 330

```
I managed a print of the bottom shell before my printer crapped out..too small, I need to work in scaling and fixing the problems 

i.e. Moving the holes for the balance wires closer together 

Added can comms port

Changed xlr port to 10mm threaded hole

12mm switch threaded hole

<img src="/uploads/db1493/original/3X/9/3/9333deb2f081c64556603c9aafeefb03ab5c9a95.JPG" width="666" height="500"><img src="/uploads/db1493/original/3X/0/d/0dd908a3d04847997c679ad74b5e9d107c02e502.JPG" width="666" height="500">

It glows in the dark...crappy iPhone
```

---
## \#239 Posted by: lock Posted at: 2018-01-04T23:56:59.006Z Reads: 322

```
Quick question...

When wiring up do you connect the main battery +/- then the balance cables (or vice versa)?

I know some BMSes are a little sensitive to the order in which this is done.
```

---
## \#240 Posted by: fedestanco Posted at: 2018-01-06T02:22:01.957Z Reads: 335

```
<img src="/uploads/db1493/original/3X/1/f/1f42dc5e2c47e1605f5bb689d7fcb1f465ac0988.png" width="690" height="330">

DO NOT SCREW THE CONNECTION UP!! I did it and had to replace a couple resistors.
To be 100% sure, double check with the multimeter: you should see increasing voltage from c1 to c12; this way the diodes can do their job.
```

---
## \#241 Posted by: lock Posted at: 2018-01-06T02:41:27.565Z Reads: 331

```
Thanks for that figure. I was 90% sure that was the way it was intended, nice to be 100% 👍. And yes, I'll definitely go over it with a multimeter first.

BUT, when I'm connecting the wires to the BMS should I first connect the battery main +/-, then the balance connectors? It possibly doesn't matter with this BMS, but does with some others.

Another question too... I wasn't planning on using the temperature sensors right now; can I simply leave T1, T2, and the "GND FOR NTC's" disconnected? Or do I need to hack it and include some conventional resistors I have lying around (ohms?)
```

---
## \#242 Posted by: lock Posted at: 2018-01-06T12:01:26.073Z Reads: 323

```
Heh, it's a bit of a rabbit hole... Just started looking at the other parts that need to be wired up; power button and the oled display.

I should be able to figure out the oled display, I have 4 labeled pins on the oled PCB (GND, VCC, SCL, SDA) and the schematic for the BMS. I don't know which pin is number 1, but one end is 3v and the other ground so that should let me figure out which is SDA/SCL.

Power button gets a bit more complicated; showing off my lack of electronics background. Even if I knew which pin was what I still have little idea how it should be wired. eg; when the button is pressed is the circuit completed from the "PushButton" pin to ground pin or 3v pin. Similarly the smart LED; except that gets a little more complicated as polarity matters.

lil help would be much appreciated. 😬

Anyway, it's Saturday night here and a few beers means it's time to put the soldering iron away.
```

---
## \#243 Posted by: banjaxxed Posted at: 2018-01-06T13:47:21.842Z Reads: 304

```
Presumably the anti spark facility of the board allows for the balance wires first the the mail battery +/- otherwise you would not be able to have a battery quick disconnect @JTAG
```

---
## \#244 Posted by: banjaxxed Posted at: 2018-01-06T20:44:25.937Z Reads: 337

```
Printing at the minute so please wait for my results, also I was planning on making the top much fancier
Edit: removed thing, the scaling is still wrong :(

Update: I'm mid-print on another and looking good so releasing again
https://www.thingiverse.com/thing:2748550

Came out ok, could mate be scaled back another mm in length/width
<img src="/uploads/db1493/original/3X/e/8/e83c5c633f5b6c770066d9f2f5c1c49f822c2fb4.JPG" width="375" height="500">

Panel mounts need very small file work to get to fit

**Update:** Problem with one of the panel mounts interfering with the switch port, need to move panel mount 3mm, will update soon. Also the 'gasket' interfact between top and bottom shells is not a perfect watertight fit, going to recut that....for the moment removed the bottom shell design.

On the plus side with a plain top the enclosure will be 30mm tall ;)

To anyone printing or thinking of please know this is a living doc but is not perfect by any means open to any guru improving it and doing a spinoff on thingiverse
```

---
## \#245 Posted by: chinzw Posted at: 2018-01-09T16:04:57.477Z Reads: 317

```
I'll try and take a picture of my wiring tonight. You can connect the battery in any order as far as I know, first balance then terminals and vice versa.
```

---
## \#246 Posted by: lock Posted at: 2018-01-13T15:05:34.769Z Reads: 329

```
Spent the last 2hrs watching my battery pack being balanced by this BMS :joy:

Ok, so I did manage to do something productive in that time...
![diebiebms_wiring|690x339](upload://g1MozQD3E7qqwo5egVSjSyPHBRq.jpg)

The above figure should be pretty straight forward, but use at own risk. Please let me know if you see anything wrong with it.

I wired up the power button first, and wasn't sure how it should behave. In my playing around I may have held it down a little long and reset its settings. I then left it on charge for a little while. After wiring up the OLED display it was showing that my battery was flat, whereas the multimeter was saying otherwise. Checked out the settings in the VESC tool, and found it was setup for LiIon (and not LiFePO4). High cell was only charged to 3.61v, so no damage done. After you wire it up I'd definitely suggest either confirming settings via VESC tool, or watch with a multimeter before leaving alone for a while.

Took all of 2min to reconfigure the BMS in the VESC Tool (needs to be v0.82), and now it's been chipping away at the cell imbalance for the last couple hours. It's really kind of cool. The watt meter I have on my charger shows the BMS switching between discharging the high cells, then bulk charging the pack. At the same you can check out how the balancing is going in the VESC tool on a cell-by-cell basis.

@JTAG and @fedestanco thanks again for all the effort you've put into this, it shows 🙌
```

---
## \#247 Posted by: fedestanco Posted at: 2018-01-13T15:26:23.625Z Reads: 308

```
Thanks for the diagram! 
I was like 100% sure to have uploaded your custom firmware to your bms. 
If you found the wrong firmware maybe now somebody else has your Lifepo4 firmware on his bms :frowning: .
What values (max cell voltage....) did the vesc tool show before you changed them?
```

---
## \#248 Posted by: lock Posted at: 2018-01-13T15:41:00.585Z Reads: 312

```
[quote="fedestanco, post:247, topic:2639"]
maybe now somebody else has your Lifepo4 firmware on his bms :frowning: .
[/quote]

Yeah, good point. This is what it was set to before.

    ---   BMS Configuration   ---
    NoOfCells                  : 12
    batteryCapacity            : 10.00Ah
    cellHardUnderVoltage       : 1.800V
    cellHardOverVoltage        : 3.950V
    cellSoftUnderVoltage       : 2.100V
    cellSoftOverVoltage        : 3.700V
    cellBalanceStart           : 3.800V
    cellBalanceDiffThreshold   : 0.010V
    CAN ID                     : 10
    --- End BMS Configuration ---
```

---
## \#249 Posted by: banjaxxed Posted at: 2018-01-13T15:48:37.061Z Reads: 299

```
So there are two wires attached to pack negative thanks for heads up @fedestanco
```

---
## \#250 Posted by: fedestanco Posted at: 2018-01-13T15:54:56.851Z Reads: 304

```
This values aren't even appropriate for liions... Maybe the custom firmware was defective by itself. I will try to double check the 12s-lifepo firmware again and see whats written on it.
```

---
## \#251 Posted by: lock Posted at: 2018-01-17T14:41:11.866Z Reads: 325

```
Been looking at communication with the DieBieMS via a command line app over the last few days. Started off as something really hack'ish, and now it's a little cleaner and better documented so figure it may be of use to others. Could do with some more error checking, unit tests, etc.

https://github.com/lachlanhurst/diebiems-cmd-terminal

It's a command line app written in Python that will run DieBieMS terminal commands. No need for the VESC Tool, although it's possibly still the preferred option for those who like a GUI.

Install and usage details can be found over on the repo. Hopefully once up and running it should be easy enough to use.

To list available serial ports run:
`python dbmscmdterminal.py -l`

To run a DieBieMS command run something like (will print DieBieMS command help), you will need to replace <MY_SERIAL_PORT> with a serial port found by the above command:
`python dbmscmdterminal.py -sp <MY_SERIAL_PORT> -c help`

You'll need quotation marks around space separated commands. For example;
`python dbmscmdterminal.py -sp <MY_SERIAL_PORT> -c "config_set_cells 12"`

There's a record mode that runs continuously polling the BMS and writing out cell voltages, percent charge (and all other available params) to a set of CSV files.
`python dbmscmdterminal.py -sp <MY_SERIAL_PORT> -r`

The only thing it won't do is upload a new firmware (yet), but on the upside you don't need to track down a special version of the VESC Tool to setup your DieBieMS.

@jtag please don't feel you need to maintain any level of backwards compatibility for this. I've invested very little time in it so far so if it gets broken, and is never used, then I really don't mind. However, I am interested in what your thoughts are going forward. Is the client side/desktop stuff something that you'd like to focus on, and should we hold off on investing more time and doing anything 'prettier'?
```

---
## \#252 Posted by: Mike_Lemon Posted at: 2018-03-09T17:30:25.977Z Reads: 306

```
Hi there, 

I've also been starting to make the "perfect BMS" and looking at your design raised me with some questions: 

1) Why didn't you use this IC? bq76pl455a

it can balance AND monitor up to 16 cells 

2) why did you go south the standard JSP XH connector? most battaries use that already.

3) I see you use the DF13 connectors which are realy great worked with them alot as a drone engineer I think you should be following the pichawk hardware format when pinning them.

4) is the charge port isolated when no voltage applied at the input? If there is voltage at all times the physical port may short sins it's usually exposed and live so consider addind an isolation along with some reverse polarity protection.

Thanks for paying attention keep me updated if you want to work together on this project.
```

---
## \#253 Posted by: Mike_Lemon Posted at: 2018-03-09T17:37:25.097Z Reads: 306

```
Also I don't know what about you guys but I've found the 3P GX-16 to be the ideal connector for charging sins it's small and can carry just enough current for everything and it also have that locking nut feature which it great!

I already featured it in my swap able battery pack(Yes I know it's 4P instead of 3P was too lazy to model the 3P one):

 ![12S2P_18650_pack v34 v4|690x388](upload://pxDrEPB1gnfK49zjefCrgTFc9Jh.jpg)
```

---
## \#254 Posted by: JTAG Posted at: 2018-03-09T18:24:57.119Z Reads: 312

```
1, Bacause: "Monitors and Balances 6-to-16 Cells per Device" and I want to go lower (although the title says 6 to 12S I can do 4S(havent tested lower yet) to 12S). But having a system that can do up to 14S is on my desires list, TI has quite a broad choice but nothing 4 to 14S as far as I know.

2, because they suck balls(mechanically), are to wide for 12S + sensors, existing batteries rarely go to >6S in a single pack, they don't have temp sensors and most dedicated skateboard builders will build their own packs. 

3, They are Molex Picoblade / wurth WR-WTB 1.5mm. What do you mean with that I should follow their wiring / hardware format? Does a FC have the same type of interfaces that I do? 

4, Read the schematic or the thread to find out :grimacing:.

No thanks.

GX-16 is what old people use on CB radios :roll_eyes: also mechanically crap, modern people go for mini XLR, XLR, neutrix power con, BINDER, PoPD rosenberger or regular DC jacks, one might even go for the modern industrial M12.
```

---
## \#255 Posted by: Mike_Lemon Posted at: 2018-03-09T19:12:59.747Z Reads: 302

```
1) 4S is a whole other category can't imagine people even go under 10S with their built sins it's just not efficient in terms of current handling in relation to power.

2)You could fit it there easily along the width on the PCB just look around most batteries use that connector. just make a separate connector that will go in parallel to the balance one (Should use some 2.54mm spaced one) sins most people don't have a temp sens installed on their pack yet if they might even want it.

3) NVM thought that was a DF13

4) to save some time from learning about the more that million ic's available it'd be nice to get a summery on the system overall features.

Right XLR might be suitable but it's used alot in the music industry unlike GX16 which I could hardly find any product use for expect some soldering iron handles that use the 5P ones.
```

---
## \#256 Posted by: JTAG Posted at: 2018-03-09T19:48:11.332Z Reads: 286

```
Feel free to change anything you like and implement it any way you want. I don't see any of your motivations as a reason for me to change anything, but it's opensource so you are free to do so 😇.
```

---
## \#257 Posted by: Mike_Lemon Posted at: 2018-03-09T20:59:19.886Z Reads: 293

```
Just offering a few suggestions and asking a few questions to expand my knowledge that's all.
```

---
## \#258 Posted by: fedestanco Posted at: 2018-03-09T21:57:01.613Z Reads: 291

```
You see Mike I am always open to consider any suggestion regarding the production, IF it's reported in a polite and constructive format.
"why don't you go for X brand for the diodes? they are just as good and cheaper" -this is constructive.

"I am not going to pay this much for this stuff, how about half price?"- this is, you know...,retarded
```

---
## \#259 Posted by: banjaxxed Posted at: 2018-03-12T15:31:01.302Z Reads: 285

```
anyone thinking of printing an enclosure head over to @lock's design posted in his build thread, better design and should fit together properly unlike my abomination
```

---
## \#260 Posted by: PXSS Posted at: 2018-03-13T11:22:37.722Z Reads: 290

```
[quote="fedestanco, post:258, topic:2639"]
You see Mike I am always open to consider any suggestion regarding the production, IF it’s reported in a polite and constructive format.
[/quote]

Are we reading two different posts? All of his posts appear very polite and friendly to me.
```

---
## \#261 Posted by: fedestanco Posted at: 2018-03-13T13:01:41.776Z Reads: 295

```
Maybe its just because of the language barrier (english is not my first language) but this comment [quote="Mike_Lemon, post:386, topic:20947"]
90 euro?! How did it get so expensive?

I’d be comfortable to pay 50Euro for one piece and 40 for bulk,
[/quote]
felt a bit arrogant. I may be wrong though, for this reason I answered in detail to his question.
```

---
## \#262 Posted by: DeathCookies Posted at: 2018-03-13T13:12:30.034Z Reads: 293

```
[quote=“Mike_Lemon, post:386, topic:20947”]
90 euro?! How did it get so expensive?

I’d be comfortable to pay 50Euro for one piece and 40 for bulk,
 [/quote]

I had the same Feeling when reading his sentence. I think it is very rude of him!

I am just happy that he has published it so anybody can make it on their own.
```

---
## \#263 Posted by: PXSS Posted at: 2018-03-14T22:30:32.934Z Reads: 285

```
Ah. That was on a different thread. Not here.
```

---
## \#264 Posted by: Kug3lis Posted at: 2018-03-19T17:38:28.892Z Reads: 289

```
@JTAG have you had any thoughts about controlling charging current on BMS itself? I am thinking what is a possibility for this, as I do not want to get another module to limit the current power supply for charging.
```

---
## \#265 Posted by: JTAG Posted at: 2018-03-19T17:59:02.516Z Reads: 293

```
Any option to transform an external constant voltage supply either by implementing a buck or boosting converter to the BMS will limit its functionally/universality for the type of battery pack ( voltage ), charge power ( DC DC current ) and increase cost.

Or where you suggesting something else?
```

---
## \#266 Posted by: lock Posted at: 2018-03-20T04:21:18.869Z Reads: 292

```
@JTAG how far along did the CAN stuff get? I see there's a 'CAN enabled' firmware in the GitHub repo.

With a bluetooth module hooked up to a VESC, and DieBieMS CAN support (??), I could presumably just connect the new VESC tool (assuming I hack around the version checking) with Bluetooth support to the VESC and use CAN forwarding to get at the DieBieMS stats/config?
```

---
## \#267 Posted by: JTAG Posted at: 2018-04-18T23:11:40.641Z Reads: 273

```
@lock yes there was a moment where I had CAN operational but after a bit of testing in combincation with two vesc's I discovered that I had a bug where the high bus load communication generated by the vesc's influenced the BMS firmware. I therefore disabled the CAN functionality in software to first focus on other higher priority stuff. BUT! I am now actively developing and expect to have CAN back up and running soon!

To everyone; my apologies for the lack of firmware updates and response, I was incredibly busy with other stuff. The last weeks however have been more focused to the BMS and a list of firmware features I would like to add. Once this revision is tested on my vehicles for a couple of days ill release it for all of you!
```

---
## \#268 Posted by: lock Posted at: 2018-04-19T01:38:25.675Z Reads: 273

```
Awesome, I might order a few cables given they'll take weeks to arrive. Do [these ones (Molex Pico Picoblade 1.25mm Cable 5 Pin)](https://www.banggood.com/FrSky-5p-JST-XH-1_25mm-Cable-5-Pin-Receiver-Wire-for-XSR-2_4G-ACCST-Receiver-p-1115427.html?rmmds=buy&cur_warehouse=CN) look ok?

It'd be great if you could bump the VESC firmware version number it pretends to be so it'll work with the latest VESC Tool. Main reason being the inbuilt Bluetooth support.

I'll stop with the feature requests now :wink:. What we have right now is a really quite nice, fully functional BMS. If you were to stop developing it and forget all about it then I'd still be happy, anything that comes later is just a bonus.
```

---
## \#269 Posted by: JTAG Posted at: 2018-04-19T08:14:46.590Z Reads: 298

```
Completely forgot to mention that just pushed a new version (V0.7) of the hardware to Github, there are no amazing / spectacular new features, just three that are worthy to state.

**NTC Power stage**
I added an option for the NTC of the power stage to be placed even closer to the switching / charging logic:
![image|690x312](upload://3Mq40VdsN5K7iqHjD4AwdkxNktY.png)
You can now chose between either of the two locations, not both :).

**NTC on LTC changes**
All previous versions that are produced of this BMS (pre V0.7) contain an error in the pullup resistor value of the NTC's. I mistakenly assumed that the LTC would be capable of driving a dual 10k pullup / NTC combination from its internal voltage regulator. After me attempting to implementing the battery NTC and reading the datasheet of the LTC I learned that this impedance is to low. These are the resistors:
![image|434x500](upload://mZyKOpEeXYlCqCBq0Y22rk4zCvQ.jpg)

And in the schematic:
![image|690x427](upload://6eCQO8AJEJiM5LstTcqqVObqCCE.png)

As seen the new pullup values should be 100kOhm. You will only need to change these resistors if you plan to implement the external temperature sensors for the battery pack. 

**Power switch options**
In a few applications (like my electric scooters) I have a main "ignition" switch that does not behave as a pulse switch but like a continuous switch. I really started to desire supporting a continuous switch as a power switch but struggled with thinking of an implementation where the BMS would still be able to power itself completely down in an extreme condition (like forgetting to power it of or when the battery is extremely empty -> below hard under voltage level).

All versions of the hardware (with the upcoming new version of the firmware) will support the continuous switch as a means of power on/off however only from V0.7 and up will the BMS be able to turn itself completely off.

The hardware changes on the board are here:
![image|690x305](upload://nxp0VAbgMYARyDjsPEV30vX8iEO.png)

And the schematic changes are these:
![image|690x348](upload://16Z2ZZEkCdG2r2MiSqhfRodU4YO.png)

It is a high pass filter construction but with the benefit that there is minimal leakage current when a switch is closed.
```

---
## \#270 Posted by: JTAG Posted at: 2018-04-19T08:20:35.459Z Reads: 267

```
This is the connector used on the PCB:

https://www.molex.com/molex/products/datasheet.jsp?part=active/0532610571_PCB_HEADERS.xml

So yes de description sounds good but something tells me that the FRSky connector style is different (but the drone hobby is very old so my memory could be wrong :stuck_out_tongue: ).
```

---
## \#271 Posted by: Samau18 Posted at: 2018-04-21T04:36:14.454Z Reads: 279

```
Hi all,

I will make small batch of v0.7 (20pcs). Will keep 5pcs for myself, so 15bare pcb or finished pcba up for grabs after we tested 2pcs successfully in the coming weeks.  PM me if interested, I will provide more details.

Thank you Danny for creating the project.

Sam
```

---
## \#272 Posted by: JTAG Posted at: 2018-04-28T21:26:12.157Z Reads: 283

```
![image|687x500](upload://3L0JnjSR5YiZ0WG3YHUzj2sTaJJ.png)

Disclaimer: Nu functionality yet! But I am really close to start and implementing that :). I am impressed by all the amazing work Benjamin had put in the VESC tool and the tools he made to adapt the tool. I am first going for VERY basic functionality like configuring most of the important stuff and later on I will add stuf to upload custom pictures to the OLED display.

And OFCOURSE it will be opensource :smiley:!
```

---
## \#273 Posted by: lpasselin Posted at: 2018-04-29T17:43:57.390Z Reads: 269

```
I have some experience with SOC algorithms that are more complex than the simple coulomb counting method.

Is there anyway you could send me some data from the SD card? All CV, current, Temperature (?), motor commands, etc.

I would start working on this after may 15th, so no rush.

Also, I'd like to build the BMS. At least one. Would anyone be willing to sell me a couple of PCB? If you have some that are already populated or have spare parts, it would be even better. I'll pay of course.
```

---
## \#274 Posted by: ekman Posted at: 2018-04-29T23:11:26.644Z Reads: 267

```
@Samau18 I'd be interested in a V.0.7 finished PCB.
```

---
## \#275 Posted by: Ethanstone Posted at: 2018-04-29T23:13:37.458Z Reads: 274

```
Hi,
I have a Hobby King 6s BMS that I am going to charge my 6S batteries with. How much power do I need to give the BMS to have it charge my batteries. 
Thanks
```

---
## \#276 Posted by: Samau18 Posted at: 2018-04-30T03:56:19.521Z Reads: 290

```
Just getting them tested now. 

![diebiems07back|375x500](upload://i5ar5XbqeyZ3WWw1KyVecjJjQfg.jpeg)![7|375x500](upload://duIdA2vR5rTGh6djykjLaAWrdM3.jpg)
```

---
## \#277 Posted by: Peakon28 Posted at: 2018-05-23T12:50:05.278Z Reads: 284

```
Where did you order PCBs from?
```

---
## \#278 Posted by: JTAG Posted at: 2018-05-24T05:53:36.568Z Reads: 323

```
I normally order trough Multi-CB, but recently discovered JLC PCB makes decent enough PCB's as well!
```

---
## \#279 Posted by: Samau18 Posted at: 2018-06-02T06:37:01.242Z Reads: 341

```
It seems I would need a Level3 account to create the groupbuy account. 

I hope Danny don't mind me starting a sale here.  Please keep all inquiries to my PM to avoid messing up this thread.  I will try to create a separate post also, but not sure if the admin allows for sales post in other categories.

I will assemble and sell 15 pcs of DiebieMS v0.7. 

The deliverable are as followings:
1 x DiebieMS v0.7 assembled. (SD Card and RF module NOT mounted).  Components I have stayed true to the original design. 
5 red and 5 black  x wire connectors (non-crimped) for battery and VESC 4x. 
1x Male 16P connector 
20 pcs non-crimped terminal for balance cables (some are spares)
1x Momentary switch
1x OLED 0.96 Display
4x single end male connector with cable (JST 1.25mm 5p, 10mm) (Display, switch, canbus)
1x single end male connector with cable (JST 2mm 4p, 10mm (VESC side can bus) 
6x M5x14 spacer screws
1x 80A Fuse 

Asking for 120USD/pc shipped to major cities around the world via Hong Kong Post with tracking Number.  (~8-10 days) destination tax and duties not included.  PM if interested, I will create PayPal invoices.
Will take ~2 weeks for completion, I have most of the parts already. 

![IMG_4942|375x500](upload://xeCnHSdLeVrKLgHO7Dj1QpJ2v4S.JPG)![IMG_7860|375x500](upload://c88wOher6fCvycANDI896cZjVx6.JPG)

Canbus test (*note I am using Ackmaniac firmware on my vesc, that's why there is a warning)
https://www.youtube.com/watch?v=bizQ7BjiMUQ

Current list: 
@uigiroux (1x Confirmed)
@Giga (2x confirmed)
@DeathCookies (3x confirmed)
@PXSS (2x confirmed)
@chsknight(2x confirmed)
@Rene（2x confirmed)
@Jumpman(1x confirmed) 
@bflan(1x confirmed) 
@PatRocks (1x confirmed)

All sold, please message me you email for PayPal invoice if you haven’t done do.  That was quick .
 
I want to let you all know it may be a while until I can make another run with this type of quality built.  As a manufacturer, I was able to get limited quantities of the parts.  But my suppliers would likely impose a minimum quantity for my next request.  It won't be easy to make another batch unless I get "a lot" of orders.  So don't miss the chance to pick one or a few of these beauties up. 

A little background about myself.  I own a electronic factory in China  (smart home).  So I was able to use my resources to make this run possible.   

Finally, I must thank Danny for the design.  Really awesome BMS.
```

---
## \#280 Posted by: chuttney1 Posted at: 2018-06-03T00:15:49.311Z Reads: 298

```
You would have to make a new thread offering this for sale. But the post is related and on topic with the title.
```

---
## \#282 Posted by: bflan Posted at: 2018-06-03T00:22:59.000Z Reads: 304

```
If there are still two left I would love to get in for 1.

Let me know, thx.
```

---
## \#283 Posted by: deucesdown Posted at: 2018-06-04T01:02:50.631Z Reads: 296

```
Dammit too late. One of these days I'll get my hands on one of these...
```

---
## \#284 Posted by: MaartenvanEls Posted at: 2018-06-04T09:55:49.191Z Reads: 297

```
If someone is making an another batch i'm really interested!
```

---
## \#285 Posted by: Mihkel Posted at: 2018-06-04T10:16:36.660Z Reads: 294

```
Look few posts back. @Samau18 plans to make a small series
```

---
## \#286 Posted by: Samau18 Posted at: 2018-06-06T07:20:52.957Z Reads: 305

```
https://www.youtube.com/watch?v=R0Py4Y1DiP8

Here is the included momentary switch and LCD screen.  

If you are interested, please send me a PM. I will make another run if I have received enough queries. 

Sam
```

---
## \#287 Posted by: SORRENTINO Posted at: 2018-06-06T19:29:08.907Z Reads: 285

```
@Samau18 can you make a new post to see if we can get a big group buy for this. I would love to get one if possible :slight_smile:
```

---
## \#288 Posted by: Samau18 Posted at: 2018-06-07T05:32:45.886Z Reads: 275

```
I am not level3 yet.  Will see how I can start one
```

---
## \#289 Posted by: agniusm Posted at: 2018-06-09T09:11:51.977Z Reads: 273

```
@JTAG Do you have board outline CAD with mounting holes or drawingvwith dimensions? I have been asked to do My NESE enclosure to fit your BMS. Also, how many power connectons is there? I see 5 but common - and pack - should be the same ?
```

---
## \#290 Posted by: banjaxxed Posted at: 2018-06-09T10:13:36.613Z Reads: 291

```
There is a step file of the design in the GitHub repository

https://github.com/DieBieEngineering/DieBieMS/blob/master/DB10005_BMS.step

I would love to utilise your design with the NESE cellpacks
```

---
## \#291 Posted by: agniusm Posted at: 2018-06-09T10:26:46.202Z Reads: 287

```
Thanks mate. How do i buy one?
```

---
## \#292 Posted by: moon Posted at: 2018-06-09T13:41:35.830Z Reads: 286

```
https://www.electric-skateboard.builders/t/diebiems-v0-7-2nd-batch/58327
```

---
## \#293 Posted by: agniusm Posted at: 2018-06-09T14:10:21.566Z Reads: 276

```
Could this bms be used standalone without vesc(programmed)? If it can, sign me up for one. Where do i pay?
```

---
## \#294 Posted by: moon Posted at: 2018-06-09T14:13:23.856Z Reads: 270

```
Click on the thread I linked. He will answer your questions. I don't know if I can answer your questions right now :)
```

---
## \#295 Posted by: Samau18 Posted at: 2018-06-09T14:28:00.828Z Reads: 263

```
You will need to configure initially with the vesc-tool terminal or the new bms tool Danny is working on.   Basically set 6-12S and capacity.  Then you are set.
```

---
## \#296 Posted by: Taliesin Posted at: 2018-06-09T14:43:10.032Z Reads: 253

```
How do I get one of these?
```

---
## \#297 Posted by: Samau18 Posted at: 2018-06-09T14:47:32.148Z Reads: 258

```
I am getting interest for a 2nd round.  I could put you on the list if you are interested.
```

---
## \#298 Posted by: banjaxxed Posted at: 2018-06-09T16:26:40.930Z Reads: 266

```
$120 shipped from @Samau18 based in HK in thread above
```

---
## \#299 Posted by: Taliesin Posted at: 2018-06-09T22:49:36.380Z Reads: 278

```
Yes add me to the list please
```

---
## \#300 Posted by: uigiroux Posted at: 2018-06-10T14:25:01.007Z Reads: 285

```
Forgot to ask, will this come with a fuse?  I'm not sure exactly what type I would need to get that is used in this design.

![Screenshot_20180610-093018|527x312](upload://itVgCym0e1G0PencOWSTT8Xl5S4.jpg)
```

---
## \#301 Posted by: Samau18 Posted at: 2018-06-10T14:55:39.450Z Reads: 281

```
Yes, I have included an 80A fuse, to match the the silkscreen value.
```

---
## \#302 Posted by: Silverline Posted at: 2018-06-10T16:14:30.782Z Reads: 280

```
What type og fuse is that. So i could buy a spare one
```

---
## \#303 Posted by: lock Posted at: 2018-06-10T16:21:50.340Z Reads: 277

```
Littelfuse bf1 58v
```

---
## \#304 Posted by: agniusm Posted at: 2018-06-10T19:29:59.483Z Reads: 287

```
Could you elaborate on wiring? Most protection boards and BMS'es i had would have a negative, charge negative and load negative + sense wires going to BMS/PCM. This one has like 5 power connectors. 
Are they all need to be connected or say pack - and common - are the same?
I would like to fit it to my modules but i have 4 power ports.

[img]https://i.imgur.com/Jtt0qeI.jpg[/img]

[img]https://i.imgur.com/oRgZ0R5.jpg[/img]

Thanks
```

---
## \#305 Posted by: Samau18 Posted at: 2018-06-11T01:38:06.675Z Reads: 272

```
Load+ and common goes to vesc(s)

Pack+ and pack-(Linked to common internally) goes to pack.  *so you can save a cable opening, but will gain some connector height total height.  Worst if you are using two packs.

Charge+ and common to charger.

You will also need the sensor/balance, canbus(s) , display and power connector to be exposed.
```

---
## \#306 Posted by: willumpie82 Posted at: 2018-06-13T08:28:36.552Z Reads: 270

```
@jtag, great design imo, just ordered one from @Samau18 :smiley: 

I do have a question, how is an overcurrent (or other error) handled? The most obvious way should be disconnecting the load. but in that case the VESC is powered down and (on a esk8) you would be even unable to brake. 

What if the error could be handled by telling the VESC to limit or cut the power/throttle gracefully before cutting the load completely in a specified amount milliseconds?

Of course current and temperature thresholds should apply where the load is cut of anyway
```

---
## \#307 Posted by: Samau18 Posted at: 2018-06-14T09:40:20.422Z Reads: 271

```
Was going see if @jtag would answer it, but seems like he is busy.   I would say you should always set some margins  (VESC max current + safety margins =  BMS max current), so the VESC can still have power to handle before the BMS is at it's limits.
```

---
## \#308 Posted by: Samau18 Posted at: 2018-06-14T09:43:13.217Z Reads: 265

```
Guys a quick update.  Still setting up SMT machine, I am pushing for completion asap.  Will update again when I start testing.
```

---
## \#309 Posted by: banjaxxed Posted at: 2018-06-14T09:45:36.922Z Reads: 270

```
[quote="Samau18, post:305, topic:2639"]
will gain some connector height total height
[/quote]
Ring terminals with a 90deg offset make this ok I think
```

---
## \#310 Posted by: chinzw Posted at: 2018-06-14T17:07:36.278Z Reads: 273

```
That's correct.
```

---
## \#311 Posted by: Samau18 Posted at: 2018-06-21T06:14:38.982Z Reads: 278

```
Waiting on the loading resister still.  Should be here soon.  Will flash firmware later today. 

![image|666x500](upload://qRyVUeeo9us10UrdAU6tlqU3w2p.jpeg)
```

---
## \#312 Posted by: uigiroux Posted at: 2018-06-21T17:34:08.592Z Reads: 267

```
Beautiful! :heart_eyes:
```

---
## \#313 Posted by: deucesdown Posted at: 2018-06-21T17:51:09.768Z Reads: 279

```
Gonna throw some questions out that I didn't see solid answers for in the original thread.

I saw in the original thread @JTAG said charger should be 3v higher than pack max voltage. So for example 12s full is 50.4v. We need a cc/cv source at 53.4v? This is not typical, and means we cannot use 12s bulk chargers?  Am I misunderstanding something?

Does anyone know what happens when limits are hit? Like cell or pack overvoltage when braking?

And are heatsinks necessary with say dual 6374 with like 12s4p or 10s5p riding it with spirit? I think its borderline?
```

---
## \#314 Posted by: JTAG Posted at: 2018-06-22T01:09:34.346Z Reads: 280

```
Well it depends. 

It all has to do with the power on state of the BMS. The BMS is designed such that when not used for an configurable amount of time it will turn off to a state where the microcontroller cannot recover out of on its own. In this state, the normal "off" state the BMS will enable by any of the following external events:

1. The power button is pushed.
2. 5V is fed into the usb port (a computer is connected to the usb port).
3. 5V is applied to the can enable pin on the can connector.
4. the charge port input is 3V higher than the pack voltage.

So if you want the convenience of having the BMS to automatically turn on when a charger is connected then the charger (CC/VC) voltage should indeed be 3V higher than the pack voltage.This is how I use my BMS in almost all applications.

But recently however I added the  (configurable) functionality to allow charging during the normal (discharge enable) state. So if you have a charger that has a voltage of 0.6V (charger input diode drop) higher than the battery voltage then the battery wil charge as normal without the need of the extra 3V.

If you also want to get rid of the diode drop of 0.6V you can bridge it by putting a solder blob on these pad's:
![image|690x307](upload://9210KXI6kAfKJ0Ny54OlnEm9hIP.jpg)

But be careful when doing this! When you bypass the charge input diode you can discharge out of the charge input due to the parasitic body diode in the charge FET. So male charge connectors will become a no no, the charger will be energised when attaching it with the connector (will spark due to the output caps of the charger when the charger has a lower voltage than the battery on its output).
```

---
## \#315 Posted by: deucesdown Posted at: 2018-06-22T02:47:20.173Z Reads: 264

```
Wow, thanks for the detailed explanation. I'll try to read code for the rest, maybe learn something. Really excited!
```

---
## \#316 Posted by: JTAG Posted at: 2018-06-22T07:20:14.056Z Reads: 266

```
No worries, need to write a manual as well and therefore I can reuse what I write :stuck_out_tongue:.
```

---
## \#317 Posted by: Samau18 Posted at: 2018-06-25T13:57:47.707Z Reads: 274

```
![image|374x500](upload://k7CEV8U6xsyf2QxrbCRrng7OR2F.jpeg)

Arrived!
```

---
## \#318 Posted by: willumpie82 Posted at: 2018-06-25T14:11:22.526Z Reads: 266

```
what is it? some kind of mega wirewound resistor?
```

---
## \#319 Posted by: Samau18 Posted at: 2018-06-25T14:21:24.492Z Reads: 269

```
Is a huge resistor to simulate 4000w loading.  50v*80A.  Quick testing of the boards before I sent them out.

Sam
```

---
## \#320 Posted by: willumpie82 Posted at: 2018-06-25T14:27:30.889Z Reads: 268

```
fine piece of kit
```

---
## \#321 Posted by: deucesdown Posted at: 2018-06-25T15:36:26.710Z Reads: 263

```
quick video plz... omg lol.
```

---
## \#322 Posted by: JTAG Posted at: 2018-06-26T11:07:20.813Z Reads: 262

```
The torture :sob:.
```

---
## \#323 Posted by: Hanok Posted at: 2018-06-27T13:41:10.855Z Reads: 262

```
Interested.
Are you still available?
I live in Korea.
```

---
## \#324 Posted by: DeathCookies Posted at: 2018-06-27T16:47:43.583Z Reads: 261

```
So excited about the resistor test. It is so nice that you make some load Tests!
```

---
## \#325 Posted by: willumpie82 Posted at: 2018-06-28T06:30:07.436Z Reads: 265

```
All that smart goodness that we are putting on our boards gives me lots of ideas :smiley:
 
@JTAG, would it be possible to startup the board (enable pack power to the VESC) by means of pusing the board (like some commercial boards)

When I push my board, the VESC led lights up, hence there is a little 5v generated. if this 5v rail is connected to the CAN power enable pin,... could that trigger the powerup sequence of the BMS?

If integration between VESC, DieBieMS and @solidgeek simple nrf remote goes further, a power-on/off feature could also be realised from the remote control.
```

---
## \#326 Posted by: JTAG Posted at: 2018-06-28T07:16:33.499Z Reads: 269

```
Wow never seen this feature 😲, I like it! It might only need a very small hardware and software update 🤐.
```

---
## \#327 Posted by: Samau18 Posted at: 2018-06-29T11:34:20.319Z Reads: 281

```
![IMG_4323|666x500](upload://hKIQAdbz6RkIEFg7HAad2V1A1JQ.JPG)
![IMG_4331|375x500](upload://aIuDTJiXQrXzfVGHzY8zLYmmTfO.JPG)

Ok a quick update. 
I have 17 pcs tested working.  2 more waiting for replacement parts. 

Although I have the giant load tester ready, I realise I don't have good enough of a battery source to test it at 80A.  I have a couple layers of pure nickel strips on my 12s4p pack, but I fear it may still be not enough for a "semi" continuous 80A test.  Not wanting to make you guys wait any longer; I will leave it to my batch 2 to have my fun with it(will take video).  

So my estimated ship day is early next week, when I have the final ones fixed.  Sorry it took a while, but there are a lot of testing to be done without automatic tools to tests.  Each pcs was tested manually. 

Testing sequence
1) 12S, ESC loaded
2) Power up
3) plug BMS USB
4) read State (Should be load enabled)
5) Test pack charge (55V, 2.4A) 
6) read operating state (should read charging)
7) Test ESC loading (run motor) 
8) Test Canbus access to DBMS

*Note I am unable to fully test the balancing capability of each board, please test charging your pack initially with caution.
```

---
## \#328 Posted by: JTAG Posted at: 2018-06-29T12:24:20.656Z Reads: 261

```
Wow, this looks fancy :heart_eyes:.
```

---
## \#329 Posted by: Holyman92 Posted at: 2018-06-29T13:01:10.224Z Reads: 262

```
@Samau18 u said 120 shipped? I am interested for round 2
```

---
## \#330 Posted by: Samau18 Posted at: 2018-06-29T13:42:11.158Z Reads: 265

```
No problem, will put you on the list
```

---
## \#331 Posted by: uigiroux Posted at: 2018-06-29T14:12:36.531Z Reads: 278

```
These look so great, I can't wait til next week!! :smile:
```

---
## \#332 Posted by: JTAG Posted at: 2018-07-01T14:58:33.298Z Reads: 279

```
IT HAPPEND:

https://www.youtube.com/watch?v=D7UNELBKQmk
(my display is water damaged, I removed it, that's why you can look trough the window and see the LED's on the BMS)

I can now enable my board by using the power button OR by kicking against the wheel OR by just placing it on the ground and start pushing the board once (like those kids or sporty people do) xD.

And exactly what you described; I already had the VESC CAN bus and +5V + GND connected to the BMS for firmware updates and acces to the BMS trough the Metr bluetooth module and the VESC, I only connected the CAN_ENABLE to the +5V and made a small firmware update (to go to normal mode instead of external mode when an external power on signal is applied) and the video shows the result!

This day ( 1-7-'18 EU date method :stuck_out_tongue: ) will be the day the power button died and will no longer be implemented in my new builds.
```

---
## \#333 Posted by: deucesdown Posted at: 2018-07-01T15:13:26.274Z Reads: 269

```
[quote="JTAG, post:332, topic:2639"]
power button died and will no longer be implemented in my new builds.
[/quote]

Wait, you rely 100% on auto sleep for turning the board off? My inner fear monger is getting anxious. :)
```

---
## \#334 Posted by: JTAG Posted at: 2018-07-01T15:15:12.747Z Reads: 262

```
I just got it working 30 minutes ago, but it works so good that I was willing to state that ^^.

No more awkwardly leaning forward to enable the board, such life hack, such improvement :blush:.

Edit: ( it has no sleep, it just powers off completely when not used for a configurable amount of time )
```

---
## \#335 Posted by: banjaxxed Posted at: 2018-07-01T15:33:30.488Z Reads: 264

```
That is a killer feature thanks for it @JTAG
```

---
## \#336 Posted by: willumpie82 Posted at: 2018-07-01T16:34:13.876Z Reads: 267

```
That is so awesome! now I seriously can't wait to receive my diebieMS
```

---
## \#337 Posted by: uigiroux Posted at: 2018-07-01T20:29:27.427Z Reads: 264

```
So I'm set to receive one of the new DieBieBMS and wanted to know, for that push to start, what would I need to upload and do to the hardware of my BMS to implement that?
```

---
## \#338 Posted by: willumpie82 Posted at: 2018-07-02T06:12:28.305Z Reads: 264

```
@JTAG Just looked up the board dimensions in this thread, is 140x60mm still accurate? I measured my [custom pla-printed](https://thingiverse.com/thing:2937580) battery/electronics enclosure and it should fit (barely :thinking:)
```

---
## \#339 Posted by: Samau18 Posted at: 2018-07-03T07:32:50.709Z Reads: 266

```
Great news!!.   Any update to the PCB?  I am ready to order the new boards for batch 2. 

Batch 1 ready to be sent to Hong Kong.  Will provide tracking as soon as I have them. 

![image|375x500](upload://mwczg5Lk2ZJaC0kXFyuextf4Ob2.jpeg)
```

---
## \#340 Posted by: Samau18 Posted at: 2018-07-03T08:25:00.391Z Reads: 254

```
Just measured again 140x 60, but you need to account for the balance cable sticking out to one side
```

---
## \#341 Posted by: Zimnismoboy34 Posted at: 2018-07-03T09:17:49.163Z Reads: 245

```
Hi .. also keen for a board as well how do I get one
```

---
## \#342 Posted by: uigiroux Posted at: 2018-07-03T11:25:55.492Z Reads: 246

```
Why do they need to be sent to Hong Kong
  I thought they were ordered from there, and then you did some work on them and then they were finished.?
```

---
## \#343 Posted by: moon Posted at: 2018-07-03T11:38:10.825Z Reads: 246

```
Shipping forwarder is probably in HK
```

---
## \#344 Posted by: Samau18 Posted at: 2018-07-03T11:44:11.475Z Reads: 246

```
yup. pricey to ship from my China factory.

Usually we direct ship if we have like thousands of them..  20 pcs, not fun to fill out all the paperwork in china.
```

---
## \#345 Posted by: uigiroux Posted at: 2018-07-03T11:45:39.171Z Reads: 246

```
Sweet, so about a week till we get em then?
```

---
## \#346 Posted by: Samau18 Posted at: 2018-07-03T11:46:17.600Z Reads: 247

```
more or less, depending on the mood of the postal guys.. but out of my hands from that point haha. good luck..
```

---
## \#347 Posted by: uigiroux Posted at: 2018-07-03T11:47:26.563Z Reads: 248

```
Lol, ok cool, thanks so much for making these!  They look fantastic and the packaging is top notch!
```

---
## \#348 Posted by: Samau18 Posted at: 2018-07-03T11:50:55.141Z Reads: 250

```
No problem, learn lots myself along the way..  By the way, two or more pcs buyers we bubble wrapped and bulk packed it for the reduced size.
```

---
## \#349 Posted by: sayekim Posted at: 2018-07-03T14:46:27.722Z Reads: 254

```
Pretty cool well done. I worry about one thing which is when the battery is empty on a ride and this push to switch on is enabled, won’t this continue to drain the battery when you then wish to continue push kicking the board?

How is this handled?
```

---
## \#350 Posted by: Peakon28 Posted at: 2018-07-04T09:07:34.292Z Reads: 245

```
How did you flash the bootloader?
```

---
## \#351 Posted by: Samau18 Posted at: 2018-07-04T09:31:27.475Z Reads: 237

```
I preflashed it already.   If you want to you can use jlink or stlink to flash it again.
```

---
## \#352 Posted by: uigiroux Posted at: 2018-07-05T14:00:29.567Z Reads: 238

```
Will we get a tracking number from the Hong Kong forwarding company?
```

---
## \#353 Posted by: moon Posted at: 2018-07-05T14:29:03.703Z Reads: 234

```
From DHL or other western companies
```

---
## \#354 Posted by: Samau18 Posted at: 2018-07-05T14:44:13.668Z Reads: 240

```
Using Hong Kong post, will have tracking
```

---
## \#355 Posted by: banjaxxed Posted at: 2018-07-05T14:52:18.955Z Reads: 245

```
Dn't forget to house your goodies folks, you have two published nice quality cases to choose from

@lock's one
https://github.com/lachlanhurst/locks-esk8/tree/master/cad/bms

And @agniusm's one  
http://18650.lt/wp-content/uploads/2018/06/DieBieMS_nese.stl
```

---
## \#356 Posted by: deucesdown Posted at: 2018-07-05T15:03:10.061Z Reads: 235

```
I'm still awestruck that github has a built-in stl viewer.
```

---
## \#357 Posted by: uigiroux Posted at: 2018-07-05T15:05:53.559Z Reads: 241

```
@agniusm isn't finished yet with his.  He waiting to get the BMS in hand so he can complete it with the proper openings for cables etc...  That's what he told me last time at least.  Hopefully won't be too long after getting it till it's completed :slight_smile:
```

---
## \#358 Posted by: chinzw Posted at: 2018-07-05T20:22:31.985Z Reads: 237

```
I designed an enclosure for this BMS as well, ill upload it tonight if i have some time.
```

---
## \#359 Posted by: wafflejock Posted at: 2018-07-05T20:32:52.247Z Reads: 243

```
Wild they even support diffing on the stls apparently and can use their viewer code with a script tag: https://help.github.com/articles/3d-file-viewer/

Let's see how long it takes for MS to mess this up ;)
```

---
## \#360 Posted by: webst Posted at: 2018-07-12T17:33:47.717Z Reads: 247

```
Hi there! Have you managed to compile some kind of manual yet? If not could you just paste what you have into Summarize this topic field? If you have no time I will soon look through the thread, choose the important information and paste it there.
```

---
## \#361 Posted by: deucesdown Posted at: 2018-07-18T04:15:08.171Z Reads: 257

```
Thanks for linking. And @lock for the design.

![IMG_20180718_001012|666x500](upload://p3elN4AKENtcGFPRi6aB6pxmQeD.jpg)

Not sure yet if I'm going this way.
```

---
## \#362 Posted by: lock Posted at: 2018-07-18T06:09:00.193Z Reads: 251

```
Ha, that's awesome... Kind of never really expected anyone else to print one. 

I should really upload the Fusion360 files so people can move the holes around a bit more easily. At the moment they are kind of randomly scattered around where I needed the cables to come out.
```

---
## \#363 Posted by: deucesdown Posted at: 2018-07-18T11:18:43.978Z Reads: 244

```
Thank you! The cad files are already in your github folder. I modded the lid to make the top flat to make it easier to print :)
```

---
## \#364 Posted by: Angelesen Posted at: 2018-07-18T18:21:25.432Z Reads: 237

```
I'm planning a setup where i mainly need the regen braking. How is this units overcharge protection? Would it be possible to redirect the surplus power to another load?
```

---
## \#365 Posted by: JTAG Posted at: 2018-07-18T20:00:05.464Z Reads: 239

```
Well this is an interesting question, currently, no there is no alternate path for power than the battery. 

In the future I would like to add regen power dissipation in a resistor. This will become an add on. I am also curios on who will need it :sweat_smile:.
```

---
## \#366 Posted by: Angelesen Posted at: 2018-07-18T20:51:55.607Z Reads: 249

```
Would this feature require much work? :roll_eyes: 

I would like to test the use of regen braking to add variable resistance and braking to rollerskis. Currently you order wheels with set resistance and you to skid to brake resulting in heavy tire wear.
```

---
## \#367 Posted by: PatRocks Posted at: 2018-07-20T13:13:48.440Z Reads: 261

```
I f-cking PROMISED myself I wouldn't do this, but (-sigh-) can someone help me understand the balance wiring for two 6s lipos with 6 black and 1 red balance wires per pack? I'm looking at the github now, Ive read the diagrams thread, my instinct and research leads me to think it is column "c" below:![20180720_060328|690x388](upload://kxiYR0w3VkG4l6bGmDNRjascmYb.jpg)

I'm a complete idiot, and I'd rather not eat-it here. Input is respected and appreciated, thanks you-people
Edit: @JTAG @deucesdown @Namasaki
```

---
## \#368 Posted by: JTAG Posted at: 2018-07-20T14:59:22.873Z Reads: 251

```
Haha I can imagine the frustration 🤗.

Balance wire mounting is always the biggest frustration.

Could you please draw the main current wires as well? 

For the lowest pack you do need to connect the gnd wire of the balance Leeds. For the top pack you can indeed leave the gnd(with respect to the top pack) wire open.
```

---
## \#369 Posted by: uigiroux Posted at: 2018-07-20T15:13:11.029Z Reads: 251

```
I'm also quite confused about setting up the balance wire connector..

There is 2 grounds GND, and I don't know what the T1, and T2 are
```

---
## \#370 Posted by: JTAG Posted at: 2018-07-20T15:20:54.925Z Reads: 259

```
At the top end (close to c12) of the balance connector there are GND T1 and T2, there are optional battery temperature sensors. You don't need to connect them.

You start numbering/connecting from the lower end ( the GND close C1.

So in every battery all cells will have both sides connected to the BMS trough the balance Leeds. Also there are two main big wires that carry main current connected between the main terminals of the battery and the pack- and pack+ of the BMS.
```

---
## \#371 Posted by: PatRocks Posted at: 2018-07-20T15:21:08.108Z Reads: 269

```
The MAN himself!! Thanks for taking the time to reply. So in this "c" column, wire 1 of 14 is gnd 1 on pcb, wire 2 is c1... wire 7 is c6, wire 8 flops around unprotected lol, wire 9 is c7... w14=c12? 
Edit: better lighting 
![20180720_082453|281x500](upload://8x2wxvz3qM2SQmuA0MC021oyzfj.jpg)
```

---
## \#372 Posted by: JTAG Posted at: 2018-07-20T16:17:55.110Z Reads: 244

```
No problem! Column B and C are both ok, but C has my preferende.

Column A will result in smoke 😎😎.
```

---
## \#373 Posted by: deucesdown Posted at: 2018-07-20T16:20:10.757Z Reads: 242

```
This looks good to me (column C).

I usually build harnesses and adapters so I can split the pack and use hobby chargers to check capacity/health and rebalance. But it takes more space and is more delicate.

 rofl is that a penis?
```

---
## \#374 Posted by: PatRocks Posted at: 2018-07-20T16:42:43.145Z Reads: 236

```
Shown actual size too
```

---
## \#375 Posted by: JTAG Posted at: 2018-07-20T16:47:06.668Z Reads: 251

```
Before connecting the balance connector to the BMS please please check with a multi meter with the black lead on the GND and the red stepping from C1 to C2 to C3 to C........ whether you get incrementing voltages.
```

---
## \#376 Posted by: deucesdown Posted at: 2018-07-20T17:14:39.796Z Reads: 249

```
[quote="PatRocks, post:374, topic:2639, full:true"]
Shown actual size too
[/quote]

Haha if it's to scale you don't need a multimeter to check voltage
```

---
## \#377 Posted by: PatRocks Posted at: 2018-07-20T23:24:42.629Z Reads: 253

```
Better penetration and resolution (sensitivity lol)

@JTAG @deucesdown and a phone call from @Namasaki , your input has been enlightening. Collectively you have bridged the gap between what I was pretty sure of and what I'm pretty confident of. Hopefully my understanding will help somebody else in the future! Thanks guys
```

---
## \#378 Posted by: PatRocks Posted at: 2018-07-22T21:35:35.452Z Reads: 256

```
@JTAG I have a question about the precharge circuit on this bms. I am using a huge capacitor pack, which is 23Farads. Is that going to be problematic for the circuit? Just wondering if there's a limit to what the e-switch can handle
```

---
## \#379 Posted by: JTAG Posted at: 2018-07-23T00:02:19.647Z Reads: 251

```
23Farads? On the load side? Or as a battery?

23Farads it not an intended load for this bms XD you might have to upgrade to a higher values pre charge resistor and change the pre-charge timeout value in the source.
```

---
## \#380 Posted by: PatRocks Posted at: 2018-07-23T00:07:33.593Z Reads: 249

```
Lol, yeah they are rather ridiculous. I had a feeling that might be a problem. I'll probably use something smaller with the bms. What size resistor would work for this cap pack? Or maybe about a 7F pack?
```

---
## \#381 Posted by: JTAG Posted at: 2018-07-23T06:48:30.325Z Reads: 246

```
What are you doing with Farads as caps on the load side of the BMS (picture! :stuck_out_tongue: )? why are they there?
```

---
## \#382 Posted by: PatRocks Posted at: 2018-07-23T23:23:23.995Z Reads: 256

```
I do not have the bms installed yet. The capacitor pack is inline between my batteries and esc's (as close to the esc's as possible). LOL, you're right to question that though, definitely not the right place to put them.
```

---
## \#383 Posted by: lock Posted at: 2018-07-24T01:27:29.983Z Reads: 269

```
Updated my wiring diagram to show the intended power LED switch wiring. Ignore other versions of this figure in above posts, I'd change them but can't edit my old posts. The issue was that I *had* the LED between 3v and LED Smart, when it should have been between LED Smart and GND. This worked, but the LED does the opposite to what jtag intended (it's actually not as bad as it sounds :wink:).

![diebiebms_wiring|690x339](upload://6jbTeKDw7eAOqj2tN2RhjzNZIIL.jpg)
```

---
## \#384 Posted by: rpasichnyk Posted at: 2018-07-28T09:04:44.979Z Reads: 263

```
Another happy DieBieMS user here. Such amazed!

https://www.electric-skateboard.builders/t/no-words-just-pictures-delete-words-use-pm/2992/6240?u=rpasichnyk

Can we have new firmware (binary file) with push to start (external CAN power up)? Will be adding support to Metr app and need a little help @JTAG ;) When charger plug is connected do not shut down VESC (make this configurable). Please please

https://giphy.com/gifs/cat-kitten-please-4u8WdgQEMVaj6
```

---
## \#385 Posted by: JTAG Posted at: 2018-07-28T21:16:20.288Z Reads: 259

```
Yes yes, will make this available asap (I am currently on a holiday in the UK and am only allowed minimal "hobby" time (she is asleep now, sshhhh dont tell her!))! As soon as I am back at my man(only)cave I will build and test a version specific for esk8 (recently I added a bunch of stuff to make it useful for an e-foil, I will need to retest everything when that is all disabled). Directly after releasing that ill finish the user interface for the computer and that will allow you to possibly implement some of those interfaces in your app, and man that would be freaking awesome!!!! :heart_eyes::heart_eyes:

Yes charging during discharge is already coded into the firmware and is configurable ^^, I actually wrote it to allow me to use the TCP - bluetooth - vesc - can - bms bridge :blush:.
```

---
## \#386 Posted by: PatRocks Posted at: 2018-07-31T01:59:31.281Z Reads: 244

```
@JTAG about the large capacitor pack, and the precharge circuit, if I were to use an anti-spark connector (as150) between the bms (load+ terminal) and the capacitor pack and esc's, would that serve to "bypass" the precharge circuit on the bms? For example, I would power-on the bms, then connect the bms to the caps&esc's via as150..? Just curious, don't want to damage anything on the pcb
```

---
## \#387 Posted by: JTAG Posted at: 2018-07-31T19:07:37.383Z Reads: 239

```
So you are using caps for the ESC that are rated with a value in farads? Unless they are as big as a couple of times the size of your battery they are most likely nog suited for a high current buffering application that an ESC needs. Can you share a type number just to make sure?
```

---
## \#388 Posted by: PatRocks Posted at: 2018-07-31T19:37:28.681Z Reads: 245

```
https://emperformanceproducts.com/product/ripple-voltage-filter-energy-booster-cap-pack-23500-uf-12s-max-volt-8awg-wire/

These are the ones that I'm running
EDIT: mine is 23500 uF version
```

---
## \#389 Posted by: JTAG Posted at: 2018-07-31T19:46:53.236Z Reads: 249

```
Ah ok, looks like this might work without any changes straight on the output of the BMS. 

This does not seem to be a cap(bank) that totals in the farad range, it is 23.5 mili farad :sweat_smile:.
```

---
## \#390 Posted by: PatRocks Posted at: 2018-07-31T20:28:07.695Z Reads: 249

```
Lol, you are correct sir! Hahaha, I am an idiot. I forgot to check my symbols. That's great news (except the me being an idiot part) thanks for the enlightening reply
```

---
## \#391 Posted by: walleywalker Posted at: 2018-08-08T04:41:37.097Z Reads: 250

```
I just received my DieBieMS today! I'm amped to get working on it. 

One question, do the MOSFETs put off heat from both sides? The heatsink side is facing towards the board, but I'd like to add an additional external heatsink on the top side of the MOSFETs as shown. 

[img]https://i.imgur.com/QI8Sb9X.jpg[/img]
[img]https://i.imgur.com/te0M7va.jpg[/img]
```

---
## \#392 Posted by: linsus Posted at: 2018-08-08T07:17:50.422Z Reads: 244

```
The heat dissipates from the "back" of the mosfet, meaning you're heatsink in that Picture isnt very effective
```

---
## \#393 Posted by: JTAG Posted at: 2018-08-08T09:21:18.675Z Reads: 243

```
Ha! amped :sunglasses:.

Fancy looking!!

Well normally with this small style of skateboards I rally doubt that you would need any heat sinking. 

But if you really want to than the best method is cooling from the bottom and then go to somewhere where you can get rid of the heat.  That said, getting rid of any heat will always help, so from the top will help as well. Just make sure to keep som distance between the wire terminals.

One extra thought, be sure to take into account the space balance leads might take up.
```

---
## \#394 Posted by: willumpie82 Posted at: 2018-08-08T09:30:48.990Z Reads: 240

```
cool design, I think your battery layout is a bit tricky to wire up though
```

---
## \#395 Posted by: walleywalker Posted at: 2018-08-08T14:46:10.011Z Reads: 238

```
Glad I asked!
```

---
## \#396 Posted by: walleywalker Posted at: 2018-08-08T14:50:03.315Z Reads: 244

```
lol I hadn't realized I dropped a pun till now. 

Is there a reason that most traditional BMS systems have huge heat sinks on them, and the DieBieMS doesnt? At first glance (from a non-electrical engineer perspective) is it that the DBMS takes a more efficient, 'smarter' approach to battery management vs the traditional chips? 

Would sinking to the bottom of the PCB actually have any direct heat conduction path from the FETs? I don't believe the copper goes from one side of the PCB to the other, correct? 

Maybe I'm just completely over thinking this whole thing and don't need to remove heat at all. I'll be maxing my system out at probably 70A pull from the battery.
```

---
## \#397 Posted by: walleywalker Posted at: 2018-08-08T14:51:27.316Z Reads: 241

```
For sure! It's going to have some weird wiring paths, but after like 4 iterations I think it'll be the most space efficient setup with 26650 cells to avoid the case from hitting the ground on the flexy vanguard board.
```

---
## \#398 Posted by: walleywalker Posted at: 2018-08-10T17:47:20.666Z Reads: 249

```
Another question pertaining to building a battery pack with fuse wire to avoid fires. 
[img]https://i.imgur.com/q4luTbn.png[/img]
```

---
## \#399 Posted by: deucesdown Posted at: 2018-08-10T17:55:48.514Z Reads: 253

```
IMO the only thing BMS can see is how voltage changes more rapidly when charging and discharging on that P group. Can be extrapolated out to how much total energy goes into (or out of) the pack before one P group hits cell high (or low) voltage cut-off.

Temperature sensors could also help, as that p group will likely run hotter if you're running the pack at high loads.

I'm just thinking out loud though...
```

---
## \#400 Posted by: willumpie82 Posted at: 2018-08-13T06:45:21.374Z Reads: 253

```
Hey, I received the BMS last friday and have build it into my board, it just fits :+1:
(currently the load power cable and CAN wires are bundled in a mesh sleeve)

< LongPostWarning >
A wiring diagram should really help, now I have searched the schematic and figured out pin 1 of the connectors with a multimeter

I have also been struggling a bit with the balance connection, The labeling C0+ and C0 on the connector layout is a bit misleading. after a few trails i found that C0 is the absolute minus of the balance chain. 

Now i connected everything including CAN, it works, I can communicate with Metr.pro via the VESC and read cells. I connected the CAN_Enable directly to the CAN_5v but i can't get it to power-on with a push. at some point I got it to charge but it won't do that anymore. and also when powered the "smartled" blinks and goes off (the board stays powered)

Also remember to setup and store the settings cells & capacity with "config_write"

![IMG_20180812_175612|666x500](upload://kL9chy3Wjl7cyav7mZ74XbNAhLc.jpg)
```

---
## \#401 Posted by: JTAG Posted at: 2018-08-13T09:07:36.636Z Reads: 242

```
Push to start will be enabled in the new firmware. In the current firmware the BMS should only briefly turn on and go off immediately after pushing.

Yes I can imagine that the numbering is confusing, I have tried different schemes bus connecting balance wires keeps a frustrating job. 

A manual writing will follow directly after the BMS Tool development
```

---
## \#402 Posted by: willumpie82 Posted at: 2018-08-13T13:34:27.073Z Reads: 256

```
thanks. if you are looking for beta testers, I'll volunteer ;-)

Until the manual is ready, a pictorial guide how to connect the balance cable for the early adopters :smile: 

(please correct me if i'm wrong)

![diebiemsbalance|666x500](upload://cRY9nfZ9XKMxqMvnSWZzZ5aTdsj.png)

note: A Cell could consist of one or more parallel cells
```

---
## \#403 Posted by: PatRocks Posted at: 2018-08-13T19:10:01.154Z Reads: 246

```
That balance wire connector is a little off. C0 is below c1, and the last balance wire is c12. There are 13 total balance wires (c0, c1..c12)
Edit: i think...
```

---
## \#404 Posted by: JTAG Posted at: 2018-08-13T20:00:34.655Z Reads: 250

```
Looking good!

A new project just popped up, and I am crazy exited about it..... the USB-C PD standard!!!!

And look what I just found on Farnell:
![53|690x387](upload://auD8DqV9FyJp7cApahgBrnH7AQZ.jpeg)

A freaking waterproof USB-C connector!

WHAT IF: You could charge your esk8 with ANY USB-C PD that can source power? And if that same esk8board can also act as a power source? 

Then you could charge your board with the same power supply as your future notebook, or your notebook from your skateboard or charge your skateboard from your notebook xD.

Oh man I really dig this standard, this will be on any future battery powered device, and this should also become the standard for our skateboards :slight_smile:.
```

---
## \#405 Posted by: deucesdown Posted at: 2018-08-13T20:08:40.123Z Reads: 239

```
[quote="JTAG, post:404, topic:2639"]
USB-C PD
[/quote]

But... 100w max, at 20v? No needs a pretty big boost too?

https://en.wikipedia.org/wiki/USB_(Physical)#PD

Still, pretty awesome!
```

---
## \#406 Posted by: JTAG Posted at: 2018-08-13T20:30:03.755Z Reads: 235

```
Well 100W is still impressive, only 2.5Hours to charge a (my) board from completely empty to full, but realistically how often would you like to charge your board to completely full right after you emptied it? I need at leas 2 hours of recovery beer after that :stuck_out_tongue:. 

Yeah a boost from any of the USB PD voltages would be preferred, I would like to charge even from a 5V 3A charger :heart_eyes:. Would take 16hours with that phone like charger  but is still acceptable.

We could even implement the charge throttling mechanism of this BMS in the boost converter
```

---
## \#407 Posted by: oyta Posted at: 2018-08-13T20:36:12.482Z Reads: 236

```
[quote="JTAG, post:404, topic:2639"]
A new project just popped up, and I am crazy exited about it… the USB-C PD standard!!!
[/quote]

And I am super excited about you being super excited about that! Hehe 😄

It is definitaly a good way to go. Less charger standards makes = less charger needed :slight_smile: 100W is also good enough.
```

---
## \#408 Posted by: willumpie82 Posted at: 2018-08-14T06:29:34.583Z Reads: 226

```
I took the balance connector layout from the gerbers, the bottom right pin is connected to GND (through a resistor), in other photos (older gerbers on C0- is labeled GND. The balance terminals are labeled in programmers style, starting from zero ;-)

@JTAG, USB-c for the win! I already own a 75W satechi usb-c PD charger with additional "old-school" charge ports (very handy to charge my macbook and other gadgets and need bring just a single charger)
```

---
## \#409 Posted by: fraannk Posted at: 2018-08-14T08:14:54.061Z Reads: 225

```
Well, if USB-C happens, I'll definitely switch to a (this) BMS...
```

---
## \#410 Posted by: Andy87 Posted at: 2018-08-14T08:35:34.693Z Reads: 225

```
Would it mean if I get a powerbar with a 3a output instead of 2a, I could charge my board battery?🤔 maybe even while driving? Just theoretically?
```

---
## \#411 Posted by: JTAG Posted at: 2018-08-14T08:55:33.572Z Reads: 236

```
Hahahaha, yes you could :smile:.

Then you could conveniently carry extra storage for your board, and it would even be useful for your other devices.

If I would design a USB PD charger / control board it would be universal, not specific to this BMS (however some features like charge throttle and convenient auto turn off/on would likely be specific to this BMS) and would work with 80% of the existing boards (will depend on battery voltage but covering the 6S to 10S batteries is doable, 12S might be a challenge).
```

---
## \#412 Posted by: chocol4te Posted at: 2018-08-14T19:54:08.599Z Reads: 223

```
This is exactly what I started to work on; if I'm carrying around a several hundred watt hour battery, surely I can use it charge my phone and laptop, and USB C makes it even better. Very exciting!
```

---
## \#413 Posted by: AresTech Posted at: 2018-08-15T08:25:30.271Z Reads: 225

```
What program is are you using for the project? Kicad, eagle or something else?
```

---
## \#414 Posted by: JTAG Posted at: 2018-08-15T10:48:05.443Z Reads: 233

```
For the hardware; Altium designer.
```

---
## \#415 Posted by: JTAG Posted at: 2018-08-15T11:47:12.930Z Reads: 265

```
Ok guys, the first version of the DieBieMSTool is finally available! 

There is still a really long todo list (like adding the realtime data for analysis and having more stuff configurable like custom logos :) ) but the first step is made!

You can find the project here:
https://github.com/DieBieEngineering/DieBieMS-Tool

I am a Qt novice so I didn't yet figure out on how to make a static build (with only an .exe output without the need for all de dll's), so for now you need to download the complete zip and extract it and run the exe from that folder. 

I assume a windows user and that you have the BMS with a firmware that states 3.38 (if I am correct this is the firmware that was delivered with the group buy's, the controller should also have the bootloader programmed). In the steps below I first flashed this ('old') firmware to match the BMS like it is from the group buy.

Version 3.38 does not support the reading and writing of the config trough the tool (only trough the terminal), that is why you need to update the firmware. Setting the firmware version to 3.38 was done back then to allow you to use the VESCTool to interface trough the terminal, the new version will be 0.18 and only works with the DieBieMS.

**Step 1**
Download the .zip ( https://github.com/DieBieEngineering/DieBieMS-Tool/tree/master/Builds )  and extract it to a folder. Yeah I know it is stuffed with files, I still need to learn on how to compile it statically :sweat_smile:, teach me @Ackmaniac :smiling_imp: .

**Step 2**
Connect the USB with the USB cable to the computer and install the drivers for com port (should happen automatically ). Open the .exe go to connections and hit auto connect (or select the correct com port). It should detect the BMS and connect to it:
![image|689x457](upload://yOUeDUzI1HjFu1cvptDMjuDfBEt.png)

**Step 3**
Go to firmware, select the DieBieMS_default.bin and hit update firmware:
![image|690x459](upload://6nLY9d60vb6Vj2Ti8Yke8sOB2Dn.png)

And wait until the firmware is written.

**Step 4**
With the 3.38 firmware the bootloader is not automatically triggered (was not yet implemented back then, it is now with 0.18 and forward), so we need to trigger it manually:

![image|690x452](upload://sftjtVCCTmsqGgnxCLz7CvmCMZ5.png)

Go to the terminal, make sure you are still connected and type bootloader_jump followed by Enter. The status LED on the BMS will now go from regular blinking to intermittent fast blinking. 

**Step 5**
If all went OK the main application will start to run and the LED blinks (either slow or normal). The defaults of the main application are set to a 10S pack, if this is the case the BMS will work normally and if not it goes to an error state. But don't be scared! If you are connected trough USB you can still configure it :slight_smile: in the error state.

When the BMS is in the error state it really badly wants to power down, the connection by USB however will force it to stay on.

Optional step:
Now go back to the firmware and hit this button:
![image|690x447](upload://z9CyTPeX1l80QJDW2AUDGVNOsws.png)

Confirm that the FW version now reads 0.18. If not repeat the previous steps. If still not lets discuss.....

**Step 6**
Go to cell management and hit read configuration:
![image|690x451](upload://kb283GmB1WdUo7bp9mVBmi23Udl.png)

Depending on how the **active configuration** matches the connected battery pack the BMS could go from normal operation (slow blinking on the bms and showing a battery on the display) to an error state (fast blinking just wanting to turn off ). The BMS wont recover by updating the config, you will need to update the config, store it in flash to the correct version to recover. If you are connected trough USB you will always be able to interface with it. 

* On first startup (after firmware update) the BMS loads the default config and stores that in **flash**.
* On every following startup it wil read the config from **flash** and use that as the **active configuration**.
* You can load the default configuration to the DieBieMS tool with the "Read default BMS configuration" button. 
* **this differs from the VESC** You can change the **active configuration** by changing a value in  the DieBieMS tool followed by hitting "Write BMS configuration". This change will be used directly (but as said it wont recover from an error state, only a reboot will do that)! So if you change a voltage limits or cells configuration wrongly it will go to an error state. The **active configuration** will be lost if you dont store it to **flash**.
* **this differs from the VESC** You can store the **active configuration** to **flash** by hitting this button:
![image|689x448](upload://idPUBHWd4ckDFMZzxrCFesZ2nBV.png)

**Step 7**
Now power cycle the BMS by removing the USB connection and turning it off and on. If you configured and stored it correctly it will now power on and activate its load output.

**You are done**

You can still check the status the old way:
![image|690x333](upload://eFFldtbDOOaIVyA1jAbkXD2Fg1c.png)

Now my focus will be on making a shiney enviroment for the realtime data where you can see cel voltages and currents and stuff. Learn how to statically build the application and build it for linux and mac. Still a lot to be done but this is a good step in the right direction.
```

---
## \#416 Posted by: oyta Posted at: 2018-08-15T17:23:31.078Z Reads: 232

```
👏🏼👏🏼

Good job! I am looking forward to get it up and running!
```

---
## \#417 Posted by: sebaszz Posted at: 2018-08-15T20:31:33.911Z Reads: 232

```
wow! this really great!

thank you very much for all your effort and sharing it with the community
```

---
## \#418 Posted by: willumpie82 Posted at: 2018-08-17T18:33:11.573Z Reads: 236

```
Wow, nice job, but I have a slight challenge, since I put everything together to and connected the CAN bus via the VESC, and the VESC is accessible via Bluetooth. 

If you create a new firmware version in the future (push to start -wink-wink-) can I still program it via vesctool?

Another question, would it be possible to compile for Mac (vesctool has an unofficial Mac release)
```

---
## \#419 Posted by: JTAG Posted at: 2018-08-17T19:23:28.663Z Reads: 244

```
Yes I have this same challenge :stuck_out_tongue:.

With this firmware and ui you should still be able do everything over CAN and trough a VESC, you can also still do everything with the terminal. 

There is however one big BUT, the current firmware's default configuration is written for 10S, and will therefore not enable the output after the firmware update if you pack has any other configuration then 10S, trough USB you would be able to change the cells, do a reboot and you would be OK, but trough CAN you cant acces the BMS after the FW update since the VESC's wont turn on anymore. I have 6S in my board and can just like you only acces the BMS trough CAN, so I have the same issue. 

Thus one thing on my todo list just became higher in priority: _Doing automatic cell count detection!_ 

This will solve 70% of the wrong configuration mistakes, so expect this feature soon :nerd_face:.
```

---
## \#420 Posted by: willumpie82 Posted at: 2018-08-17T19:50:49.468Z Reads: 230

```
I'll wait for one of the next versions that will add some features ;)

But if you need beta testers, please let me know :smile:
```

---
## \#421 Posted by: myreala Posted at: 2018-08-17T20:27:23.676Z Reads: 235

```
[quote="JTAG, post:419, topic:2639"]
Doing automatic cell count detection!
[/quote]

Oh my gawd, that would be perfect!
```

---
## \#422 Posted by: uigiroux Posted at: 2018-08-17T21:00:07.025Z Reads: 234

```
Sorry that confused me a bit, lol.  I'm gonna be running 12s, so what will I need to avoid doing, or do after an update.
```

---
## \#423 Posted by: deucesdown Posted at: 2018-08-17T21:07:50.910Z Reads: 233

```
Basically, if you're not running 10s you need to do first time (just first time) configuration via usb.
```

---
## \#424 Posted by: uigiroux Posted at: 2018-08-17T21:32:28.848Z Reads: 231

```
Ahh, got it, thanks!  :wink:
```

---
## \#425 Posted by: JTAG Posted at: 2018-08-19T21:43:33.510Z Reads: 239

```
![19|690x474](upload://gK13VPReyJcTPdqMRhPkmpBK5Gk.jpeg)

Text based realtime data works! Soon the graph for current/ voltage, temperatures and a bar graph for the cells will be made and the auto cell count detection will be implemented.
```

---
## \#426 Posted by: Pimousse Posted at: 2018-08-20T07:20:16.327Z Reads: 230

```
Well done !
I also customized VESC Tool for my own purposes. Vedder did an amazing work, it's so easy to rearrange parameters and pages, even when we're not used to Qt.
However, I'm struggling finding how to add telemetry in the dark grey squares as you did.
Could you point me the file to change ?

Thanks !
```

---
## \#427 Posted by: JTAG Posted at: 2018-08-20T12:17:08.512Z Reads: 231

```
Yes I really appreciate all the work vedder has put in and the aids he made to facilitate the development of the tool itself.

The text boxes are filled / changed in a widget: widgets/Sources/rtdatatext.cpp 

Good luck!
```

---
## \#428 Posted by: AlexBE Posted at: 2018-08-20T23:48:13.782Z Reads: 238

```
This is certainly awesome, and I will include it in some of my products for sure, but for Battery voltages>20V, you will need a fairly large boost converter somewhere. Very very unlikely that is going to be inside your board.
```

---
## \#429 Posted by: Samau18 Posted at: 2018-08-23T01:52:17.068Z Reads: 233

```
Hi Guys, 

If you are happy with your unit, please help get me some reference by voting for me below.  

https://www.electric-skateboard.builders/t/trusted-sellers-and-builders-these-people-will-not-rip-you-off/48508/58

Sam
```

---
## \#430 Posted by: DeathCookies Posted at: 2018-08-23T11:56:01.507Z Reads: 230

```
You got my thumb up! Deserved!
```

---
## \#431 Posted by: angeljmm Posted at: 2018-08-23T12:02:15.881Z Reads: 234

```
+1 
10char...
```

---
## \#432 Posted by: Trdolan03 Posted at: 2018-08-23T17:03:16.813Z Reads: 251

```
I'm having a hard time finding a price and how to order. Whats the going rate on these?
```

---
## \#433 Posted by: oyta Posted at: 2018-08-23T17:07:29.089Z Reads: 256

```
Check out the new group buy:

https://www.electric-skateboard.builders/t/diebiems-v0-8-batch-3/65313?u=oyta
```

---
## \#434 Posted by: Trdolan03 Posted at: 2018-08-23T17:13:24.053Z Reads: 250

```
Oh man. I don't think I can afford $120 right now. Some day
```

---
## \#435 Posted by: webst Posted at: 2018-08-24T05:40:33.254Z Reads: 250

```
I got this strange error
![image|690x153](upload://36sOjBfstEtISmw48SrhlIdDWDV.jpeg)
```

---
## \#436 Posted by: Samau18 Posted at: 2018-08-24T06:55:59.998Z Reads: 241

```
Thanks for letting me know.  Someone else told me also, may be your account is too new?
```

---
## \#437 Posted by: Jumpman Posted at: 2018-08-24T14:12:37.193Z Reads: 234

```
Same here.
```

---
## \#438 Posted by: webst Posted at: 2018-08-24T22:05:36.874Z Reads: 235

```
There has to be something else. My account will have 2y soon.
```

---
## \#439 Posted by: DeathCookies Posted at: 2018-08-25T08:14:59.789Z Reads: 229

```
Maybe because you are not regulars?
I would think so to prevent scammers taking the lead.
```

---
## \#440 Posted by: JTAG Posted at: 2018-08-26T00:22:54.507Z Reads: 241

```
Strangely enough even I can't vote xD.

In other news!
I have all graphs operational, one example of the temperature graph:
![image|690x388](upload://fRlGPQTakxmOK2BRXzACJkUt3SS.png)

Will push and build a release asap! For now I am starting to read on the plotting of bar graphs xD.
```

---
## \#441 Posted by: chinzw Posted at: 2018-08-26T00:36:02.217Z Reads: 228

```
Great work JTAG! Can't wait to put all the new features on my board!
```

---
## \#442 Posted by: oyta Posted at: 2018-08-26T06:15:26.511Z Reads: 242

```
[quote="JTAG, post:415, topic:2639"]
Learn how to statically build the application and build it for linux and mac.
[/quote]
@rpasichnyk has experience building the VESC Tool for MacOs 😊
```

---
## \#443 Posted by: craigthemachine Posted at: 2018-08-26T17:53:06.826Z Reads: 244

```
I know you guys explained the CAN Bus connection several times. However for the sake of clarity, kindly explain which wires from the BMS side is which. 

Obviously the Focbox has 4 pins , and the BMS has 5. 

5v
cAn L
cAn H
GND 

Noting the colors, which is which ?
```

---
## \#444 Posted by: craigthemachine Posted at: 2018-08-26T17:54:18.159Z Reads: 247

```
![image|375x500](upload://22uX0EnllQIORq0F0lJAcoeVllD.jpeg)
```

---
## \#445 Posted by: oyta Posted at: 2018-08-26T18:44:12.039Z Reads: 245

```
I have tried to go through the documentation. Would be good if someone could verify it:

![image|690x260](upload://rYPuv6ahePSFbDIcY5A0x559KMI.jpeg)

This is from the schematics of DieBie MS. 

![image|393x500](upload://2e8Du4n0VdVXbzrWOl6ndSs9vze.jpeg)

And this also. I have numbered the pins. So number

1. is Enable CAN,
2. is CAN 5V, 
3. is CAN L (low), 
4. is CAN H (high)

Not sure about the VESC though. Haven’t done it myself yet. Thereof please someone with experience should verify it 🙂
```

---
## \#446 Posted by: craigthemachine Posted at: 2018-08-26T19:20:37.258Z Reads: 228

```
This helps 👊🏽, thanks a million
```

---
## \#447 Posted by: JTAG Posted at: 2018-08-26T19:38:02.280Z Reads: 229

```
This is correct! 

The can connector has 5 pins however :stuck_out_tongue:, last pin, pin 5 is gnd.

Sorry guys for the missing manual. Now that the bms tool is getting useable I will start to focus on the manual.
```

---
## \#448 Posted by: JTAG Posted at: 2018-08-27T09:29:48.042Z Reads: 235

```
Finally able to plot bar graphs:
![image|690x377](upload://3lpod35HyymQ9kXTumeiNNwDSc4.png)

This is just dummy data to test the graph plotting but it looks good already. Will now attempt to make the BMS send the individual cell voltages to the bmstool.
```

---
## \#449 Posted by: JTAG Posted at: 2018-08-27T22:50:25.563Z Reads: 235

```
![image|690x376](upload://CJ9xSYchCjWHBSKtDZ6K3dus65.png)

Bar graphing works! Now with real data :heart_eyes::heart_eyes::heart_eyes:.

Anybody have a suggestion on how to intelligently and automatically zoom without the range changing all the time :sweat_smile:, can't think of a good method right now.
```

---
## \#450 Posted by: Giga Posted at: 2018-08-27T23:10:25.165Z Reads: 226

```
[quote="JTAG, post:449, topic:2639"]
how to intelligently and automatically zoom without the range changing all the time
[/quote]

Fixed scale based on cell chemistry/cut off settings? (e.g. for LiPo form 3.7 to 4.2)
otherwise for cell drift maybe with minimum interval + cell status (e.g. steps depending on drift, but can't go below 0.05V and range is depending on overall soc)
```

---
## \#451 Posted by: bevilacqua Posted at: 2018-08-28T09:14:09.720Z Reads: 224

```
Hello Danny (@JTAG), 

witch kind of NTC Thermistors should we utilize? 

If I'm not mistaken there is room for two? 

Is there any command to test if they work? or will the SW implementation come later on?

Thank you for your help :)
```

---
## \#452 Posted by: JTAG Posted at: 2018-08-28T11:32:56.354Z Reads: 233

```
Yes you can use up to two NTC sensors, preferably use 100kOhm @25 degree C type sensors. 

You can configure the beta value here:
![image|689x375](upload://sYF4Rnt4eH5Ep0rT9NA3bNtfJPS.png)

When you connect the NTC and configured it you can enable it by setting the "Temp sensor enable mask Battery" to 3 if you connected both sensors on the balance connector. Set it to 1 if you have only connected a sensor to NT0 and set it to 2 if you have only a sensor connected to NTC1.

You should now be able to see the value in the realtime window:
![image|690x375](upload://aaGnJ5jWlu7lsqRejDztQ5Yzatj.png)
```

---
## \#453 Posted by: bevilacqua Posted at: 2018-08-28T11:45:51.748Z Reads: 228

```
great! Thank you for the detailed explanation :D
```

---
## \#454 Posted by: rpasichnyk Posted at: 2018-08-28T20:22:56.577Z Reads: 238

```
@JTAG you rock!!! :open_mouth:

In order to have a single executable on Windows, you need to compile static build of Qt. The easiest way I can recommend is to use these awesome scripts https://github.com/martinrotter/qt5-minimalistic-builds and tweak them a little bit. Remove `-skip qtconnectivity` and  `-skip qtserialport` because you need that and follow instructions.

Also, I compiled DieBieMS-Tool for mac. When you are ready to do it yourself, let me know if you need any help :slight_smile: 

https://github.com/rpasichnyk/DieBieMS-Tool/releases

Please do not put DieBieMS-Tool builds in git, it hurts me a little :sweat_smile: You can use GitHub Releases for that ;)
```

---
## \#455 Posted by: JTAG Posted at: 2018-08-28T21:29:31.866Z Reads: 224

```
Thanks thanks, I will try that!

Yes master I'll change my life and be a better man on github :nerd_face: (soon).
```

---
## \#456 Posted by: SpeedyGonzales Posted at: 2018-09-02T02:24:20.427Z Reads: 215

```
You might consider to post about your BMS on Endless Sphere forum.
You can start a new thread and update all changes on your first post.
Also you can put your BMS for sale on ITEMS FOR SALE - NEW page.
```

---
## \#457 Posted by: Jc06505n Posted at: 2018-09-02T02:46:07.305Z Reads: 216

```
[quote="SpeedyGonzales, post:456, topic:2639"]
your BMS
[/quote]

Jtag’s******
```

---
## \#458 Posted by: SpeedyGonzales Posted at: 2018-09-02T03:41:58.458Z Reads: 215

```
Is that some kind of code?
Who do I contact to buy one of these wonders (BMS)?
```

---
## \#459 Posted by: Jc06505n Posted at: 2018-09-02T03:51:28.306Z Reads: 219

```
You buy them from @Samau18, but it’s @JTAG who designed and created it
```

---
## \#460 Posted by: Wraith Posted at: 2018-09-02T05:01:42.674Z Reads: 227

```
Get in on the 3rd batch! 

https://www.electric-skateboard.builders/t/diebiems-v0-8-batch-3/65313?u=wraith

Sign the form and sit tight cause production will begin once the 50 interested orders are in!
```

---
## \#461 Posted by: SpeedyGonzales Posted at: 2018-09-02T15:21:11.784Z Reads: 209

```
Just did, Thanks.
```

---
## \#462 Posted by: SpeedyGonzales Posted at: 2018-09-02T15:56:10.377Z Reads: 212

```
BTW: I ordered one, but can order second if this will make the difference. 
Keep us posted. Maybe others will order more so we get it going.
Do we have some kind of manual or YouTube video how to?
```

---
## \#463 Posted by: guilhem74 Posted at: 2018-09-02T19:24:37.596Z Reads: 206

```
Did you run any test on how much amps it can handle ? 
I might be interested for a unit.
```

---
## \#464 Posted by: Wraith Posted at: 2018-09-02T22:38:55.056Z Reads: 209

```
I believe it would make a difference in order to get production going.

Both @Samau18 and @JTAG have some Youtube videos that you can reference for setup
```

---
## \#465 Posted by: Wraith Posted at: 2018-09-02T22:50:04.005Z Reads: 211

```
I can’t recall the exact number but it was over 100 amps. You could look it up here
```

---
## \#466 Posted by: Superflim Posted at: 2018-09-03T12:56:34.257Z Reads: 220

```
I don’t mean to be rude or anything but why is this better than say a bestech bms? My knowledge about bms’s is still in a very very early stage...

Just looking for a quick answer
```

---
## \#467 Posted by: Wraith Posted at: 2018-09-03T12:58:19.700Z Reads: 217

```
Lots of good features and can handle higher amps to safely be used without bypassing for discharge afaik
```

---
## \#468 Posted by: Klaerke91 Posted at: 2018-09-03T14:54:05.734Z Reads: 216

```
1. Its configurable from 6-12s setups
2. Has CANBUS support so you can connect and talk to the vesc
3.  its own config tool
4. Future addons like USB-C PD (Use you laptop/mobile charger)
```

---
## \#469 Posted by: Superflim Posted at: 2018-09-03T14:59:12.942Z Reads: 222

```
Would you recommend me getting this? 
Is the Diebiems something like focbox unity, only for super high-end systems? So basically anyone exept people with a crazy build are going to benefit from it.

This is my build
https://www.electric-skateboard.builders/t/the-reborn-in-progress-focbox-6473-200kv-10s4p-first-build/66111
```

---
## \#470 Posted by: Wraith Posted at: 2018-09-03T15:01:16.106Z Reads: 210

```
You dont need super high end build to use this bms. Its more expensive but thats because its a robust all in one system so no need for anti-spark anymore. Everything you’ll need is on the board and like the previous posts mention, its highly configurable to suit any build from 6s-12s.
```

---
## \#471 Posted by: Superflim Posted at: 2018-09-03T15:17:19.185Z Reads: 208

```
Thank you for the explanation.
Also thank u @Klaerke91.

I'm going to stick with a bestech bms since it's half price.
```

---
## \#472 Posted by: Wraith Posted at: 2018-09-03T15:20:33.383Z Reads: 208

```
No problem. Bestech is a good brand as well! Should suit your build fine
```

---
## \#473 Posted by: oyta Posted at: 2018-09-03T16:53:05.192Z Reads: 210

```
So I do not have the cable to connect CAN between the DieBie MS and the VESC. Are the connectors JST <s>2 mm</s> 1.25 mm pitch 5 pin on the DieBie MS and JST 2 mm pitch 4 pin on the VESC? I haven't been successful finding these cables complete. <s>Anyone selling these or having spare?</s> Edit: Never mind. I will buy and make some.
```

---
## \#474 Posted by: Samau18 Posted at: 2018-09-04T00:00:30.081Z Reads: 218

```
I have included them in.  5pin connectors with cable and 4pins connectors with cable.  You will just need to solder them up.  I didn’t make a premade 5p to 4p cable since the length is quite customized.

Sam
```

---
## \#475 Posted by: SpeedyGonzales Posted at: 2018-09-04T03:00:40.182Z Reads: 218

```
@Samau18 and @JTAG
Guys, it looks like you build a premium product and you are selling it at a premium price, but if you hope to sell a lot of it, and God forbid, make a back or two, please, please, please provide good instructions and description. What I see on YouTube is just not good. You will get many more people buying your product once you build consumer confidence. That's no brainer I think.
Guys that already used DieBieMS, can you please give back to the community and write some feedback?
```

---
## \#476 Posted by: MrEpiquad Posted at: 2018-09-04T09:08:57.083Z Reads: 230

```
@SpeedyGonzales  I'm not sure what you are trying to get out of this criticism and if you understand that it is  actual not a product but a open source project. 
No one is actual saying you should buy it or is advertising the bms, and I am pretty sure that the people who are buying it actual are involved enough to understand how the BMS works. And even if they don't they understand it's an open source project and not a ''Premium product''. Also the title of the this topic says enough '' DIY 6S to 12S BMS with CAN'' and not ''Premium 6S to 12S BMS you should buy". 
In the beginning of the very first vesc there were also not clear instruction or fancy a interface but over time the community and Vedder created to what it is today. 

The ''Premium price'' as you describe it is almost cost price and if you would actual be aware of the components prices you could already see that it's actual quite cheap.
```

---
## \#477 Posted by: SpeedyGonzales Posted at: 2018-09-04T15:58:42.905Z Reads: 233

```
What I'm trying to get out of it is very simple. I would like to painlessly put that BMS into my battery pack and make it work like a charm. I would like to see it rise to the level of VESC so everyone who is buying FOCBOX will buy one of these BMS. I think that this is that cool. Do you have a problem with that? 
I already ordered one and willing to buy more. I don't care what the price is. I can afford anything. I understand that this is still early, but it is definitely more than DIY. That title is meaningless by now. 
![Battery%20pack-1|690x388](upload://aErTqnWz0LupGSHj1IonfwBW1y.JPG)
```

---
## \#478 Posted by: rpasichnyk Posted at: 2018-09-04T18:19:55.514Z Reads: 235

```
Damn @SpeedyGonzales you are so cool! Can you afford 25 DieBiez so we can close the third group buy? Also with 25 Metr Pro modules, cause they are gonna work sweet together!

![mov|331x499](upload://p9iArLP0UU6WlXmTLgP4qKeM9x9.gif)
```

---
## \#479 Posted by: Jc06505n Posted at: 2018-09-04T18:38:43.035Z Reads: 222

```
How?! Explain this wizardry ! Is the Metr mod taking info from the vesc's that's connected to the bms via canbus?
```

---
## \#480 Posted by: rpasichnyk Posted at: 2018-09-04T18:43:27.591Z Reads: 229

```
Metr module talking directly to the BMS via CAN bus. Oh, not directly, but through UART. CAN bus works in a such way that there is literally two signal wires connected through everything (that's why it is called bus). Same two wires, CANH and CANL and you can connect multiple things to them, for example 4 VESCs, 1 remote and 1 BMS. Each thing can receive and send the data.
```

---
## \#481 Posted by: deucesdown Posted at: 2018-09-05T05:48:06.114Z Reads: 226

```
Geez @rpasichnyk it's working, I won't be able to hold out...  which vesc6 firmwares does this mighty combo work with?
```

---
## \#482 Posted by: Pimousse Posted at: 2018-09-05T06:56:02.719Z Reads: 238

```
https://media.giphy.com/media/yidUzHnBk32Um9aMMw/giphy.gif

@SimosMCmuffin is working on his BMS also. I guess if both project share the same protocol, it won't be so difficult to make your app compatible with both.

BTW, how does your VESC counter script differentiate VESC from BMS ?
Does it need to be for instance ID #200 or some high value ?
```

---
## \#483 Posted by: bevilacqua Posted at: 2018-09-05T07:14:10.322Z Reads: 232

```
ID 10
10char
```

---
## \#484 Posted by: JTAG Posted at: 2018-09-05T09:41:29.898Z Reads: 235

```
Such animation much future :nerd_face:.

:sparkling_heart: @everyone : 
https://www.youtube.com/watch?v=UaYiNzV8UX0
```

---
## \#485 Posted by: willumpie82 Posted at: 2018-09-05T13:11:54.292Z Reads: 228

```
@rpasichnyk, w00w that looks so nice! 

@JTAG now we need DiebieMS to forward CAN-ID over uart so we can connect the metr.pro to the BMS instead of the VESC (makes more sense during charging to keep the VESC off)

metr.pro (UART) ==> (UART) DieBieMS (CAN) ==> (CAN) VESC1) || (CAN)VESC2
```

---
## \#486 Posted by: SkaterBoy58 Posted at: 2018-09-05T23:27:18.860Z Reads: 232

```
@JTAG  Danny - just about to put one of your great BMS units in service - ( from Sam batch 2 ) 
Could you please confirm start-up actions as below

Use DieBieMSTool 0.20Windows 
Connect PC to BMS usb
power up BMS from battery pack +ve and -ve
from tool - download FW 0.20 to BMS 
Configure settings from tool and download to BMS
Connect balance and charging leads 

Thanks
```

---
## \#487 Posted by: SkaterBoy58 Posted at: 2018-09-06T00:04:09.181Z Reads: 229

```
@rpasichnyk  Roman - does this mean that if the DieBie BMS has a metr-pro module connected to its usb port ( and no vescs involved) the metr app can see the bms and provide real time cell voltages ?

Cheers
```

---
## \#488 Posted by: walleywalker Posted at: 2018-09-06T03:43:58.169Z Reads: 226

```
Question - How does the power switch integration work on the DieBieMS when matched with a FocBox or similar that utilizes it's own anti-spark switch? 

Does the BMS signal the ESC to power up or vice versa?
```

---
## \#489 Posted by: Pedrodemio Posted at: 2018-09-06T13:35:22.774Z Reads: 229

```
Second this!
```

---
## \#490 Posted by: rpasichnyk Posted at: 2018-09-08T14:18:13.243Z Reads: 238

```
I was watching how my DieBieMS is charging. So beautiful. I was watching and watching, and then strange thing happened: the cell voltages switched places or something for a split second

![mov|600x382](upload://4mKchGLjtiwcK4SBgBr79nJNWoM.gif)

Afterwards it jumped back. This looks like a bug @JTAG or I don't understand something?
```

---
## \#491 Posted by: DeathCookies Posted at: 2018-09-08T14:19:44.751Z Reads: 231

```
Seems like it gets sorted for a Split second
```

---
## \#492 Posted by: rpasichnyk Posted at: 2018-09-08T14:29:20.373Z Reads: 232

```
Also getting pretty hot right now with 4A charger
![15|318x126,50%](upload://2Z9XNGzq1P3TMV2ErJzxxUp5DwK.png)
Is it safe? Will it stop at some point?
```

---
## \#493 Posted by: JTAG Posted at: 2018-09-08T14:33:55.239Z Reads: 227

```
Yes that is a bug: https://github.com/DieBieEngineering/DieBieMS-Firmware/issues/1

It is fixed in my current code but this with some changes still need to be released.

That looks high indeed, strange, I charge my skateboard with 8A and it doesn't get that hot. Did you change the "Max enabled balance resistors" value in the balancing tab? Should be max 5.
```

---
## \#494 Posted by: rpasichnyk Posted at: 2018-09-08T14:38:42.484Z Reads: 219

```
Yes I have 5. Here is my configuration, I use mostly defaults http://codepad.org/oweiony8
My BMS has no airflow, packed very tight in the enclosure
```

---
## \#495 Posted by: JTAG Posted at: 2018-09-08T14:52:16.917Z Reads: 225

```
You only have the LTC temperature sensor enabled ( tempEnableMaskBMS 4 ), so the read temperature comes from the heat of balancing. It might indeed be the very compact build and the high thermal resistance why it gets so hot. You could try to lower the “Max enabled balance resistors” and therefore reduce the heat.

Regulating this automatically is still on my desired feature list :).
```

---
## \#496 Posted by: JTAG Posted at: 2018-09-08T14:53:01.521Z Reads: 234

```
typedef enum {
TEMP_EXT_LTC_NTC0 = 0, //1
TEMP_EXT_LTC_NTC1, //2
TEMP_INT_LTC_CHIP, //4
TEMP_INT_STM_NTC, //8
TEMP_EXT_ADC_NTC0, 
TEMP_EXT_ADC_NTC1, 
TEMP_EXT_ADC_NTC2, 
TEMP_EXT_ADC_NTC3, 
TEMP_EXT_ADC_NTC4, 
TEMP_EXT_ADC_NTC5, 
TEMP_INT_ADC_NTC6, 
TEMP_INT_ADC_NTC7, 
TEMP_INT_SHT 
} modPowerElectronicsTemperatureSensorMapping;

You can enable an extra sensor (TEMP_INT_STM_NTC, this NTC sits next to the switching electronics) by setting the tempEnableMaskBMS  to (4+8=) 12.
```

---
## \#497 Posted by: bevilacqua Posted at: 2018-09-13T18:09:16.538Z Reads: 239

```
Hi, I've got one problem and Im not able to figure out why: 

- Redid the balance connectors
- Charged form 3,4V/cell to 4,1V @ 10S 
- *Is preconfigured to 12S (Recieved it like that) 


After I power it on, it shows me the start screen and a crossed battery symbol. Then it just turns off. 
Im not able to connect it to my computer (Mac and Win. tested). 

It behaves lake this with and without balance connector attached. 

Any idea why? @Samau18 thought it maybe was because of the low voltage (34V @ 12S**) But now at 41V nothing has changed. 

one of the LED's also blinks when the USB is connected + the LCD shows "bye"....


http://gifsstore.com/public/upload/gifs/15368611571536861142.gif

![telegram-cloud-file-2-246227574-387211-7724610070488373603|690x419](upload://8OwyLandBQ4GRXtZXxBXULqbme4.jpg)
```

---
## \#498 Posted by: JTAG Posted at: 2018-09-13T19:09:55.572Z Reads: 235

```
Ok so the bms turns on when you connect the computer. 

Do you maybe have to install some additional drivers? the chip is a CP2102, there should be driver available for every OS. Can you check this?

After that you can update the firmware as described earlier and you should be able to configure it to your pack. 2.8V per cell is low but not so low that this warning should occur (depends on the voltage configuration).
```

---
## \#499 Posted by: bevilacqua Posted at: 2018-09-13T19:21:17.389Z Reads: 234

```
I'll try it right now, thanks :)

Edit: It worked!
```

---
## \#500 Posted by: SkaterBoy58 Posted at: 2018-09-14T01:35:22.203Z Reads: 239

```
@JTAG  Danny  I have slight problem with BMS not enabling charging 
Have a 10S 10Ah pack and are using BMS for charging only.
Pack is connected with 40.6V  - all cells are below the soft cutoff , it is balancing , the power light is off and a 45V charger is connected . 
Could be something to do with 100% SOC disabling charger?   Have set pack Ah to 100 but SOC stays at 100% . Any way to ignore SOC for charger enabling?

Many thanks
![2018-09-14_9-28-30|690x343](upload://3N9euBXXecPNz2uN1ONPu6qHs7z.jpg)
```

---
## \#501 Posted by: JTAG Posted at: 2018-09-14T08:47:22.697Z Reads: 234

```
Can you enable / use it in discharge mode (is it just charging that isn't working?)?
```

---
## \#502 Posted by: SkaterBoy58 Posted at: 2018-09-14T09:45:43.074Z Reads: 230

```
@JTAG  Danny I am only using BMS for charging
What are the conditions that need to be true for enabling charging?
Cheers
```

---
## \#503 Posted by: JTAG Posted at: 2018-09-14T10:06:12.000Z Reads: 227

```
Wow that are quite a few :stuck_out_tongue:.

Mainly these:

* Charger voltage >= 2V+battery voltage but preferably a bit higher.
* Charger current should be above the "Charger enable threshold"
* highest cell voltage should be below the soft over voltage and below the hard over voltage
* The amount of cells should match the pack.

(state of charge is ignored, it is only for indication)
```

---
## \#504 Posted by: SkaterBoy58 Posted at: 2018-09-15T12:06:34.515Z Reads: 229

```
@JTAG  Danny thanks for that - good to know that SOC is indication only

Still having trouble keeping BMS charging above 40V

current condition with charging off is
45V charging voltage 
V Pack = 40.93V
CVHigh = 4.110
CVLow = 4.096
Condition Status-- Power Down""
Have Charger enable threshold set to 0.50A 
Cell Hard Overvoltage set to 4.35V
Cell Soft Overvoltage set to 4.20V
Charge hysteresis set to 0.01V

Is there any way the power switch can be changed to a latched switch to keep BMS charging

or any other clues?

Many Thanks
```

---
## \#505 Posted by: rpasichnyk Posted at: 2018-09-15T14:29:39.655Z Reads: 228

```
I am having a hard time shutting my board down :sweat_smile:

https://youtu.be/11k6X4RlK00

Is it maybe because VESC capacitors keep them alive for a second and wake up BMS after it shuts down?
```

---
## \#506 Posted by: JTAG Posted at: 2018-09-15T14:56:13.816Z Reads: 226

```
What current do you use for charging? What kind of charger is it? Could you try powering it up with the button and then apply the charger? 

@rpasichnyk hahaha it is fighting you I see :stuck_out_tongue:. It does seem a bit like a re power loop indeed. Good thing is that it will eventually power down. I will try to recreate it and build a delay mechanism to prevent this oscillation. What ESC's do you have dual/single? Or do you know the total capacity?
```

---
## \#507 Posted by: rpasichnyk Posted at: 2018-09-15T17:56:24.931Z Reads: 224

```
Single FOCBOX
```

---
## \#508 Posted by: SkaterBoy58 Posted at: 2018-09-16T02:52:05.087Z Reads: 226

```
@JTAG  I am using a DPS5015 CCCV charging module set to 45V 5A 

without charger or usb connected and the balance wires connected - when the pack voltage is applied - pushing power push-button switches it on and the switch led comes on for 5 seconds and then it goes off and BMS goes to Power Down mode .
 Its as if it is waiting for something during that 5 seconds. Pushing the power pushbutton after the five seconds does not switch is back on again and it stays in Power down mode.

 Thanks for your assistance
```

---
## \#509 Posted by: JTAG Posted at: 2018-09-16T08:18:09.327Z Reads: 223

```
Fancy module! I should still buy one of those...

Well the reason why it is unable to stay on by itself is one of the reasons why it won't charge. Ill pm you and we will dive into this. Later when it is resolve ill share the reason back here.
```

---
## \#510 Posted by: bevilacqua Posted at: 2018-09-16T21:22:53.984Z Reads: 221

```
I wired all 4 of the CAN cables to the BMS and bridged Can-Enable and 5V to test the “push to start” feature: it did not work 😅

Does 0.2 FW support it? Do I have to change anything on the settings? 

Cheers, Mathias
```

---
## \#511 Posted by: JTAG Posted at: 2018-09-16T21:37:59.380Z Reads: 226

```
You probably mean V0.20 ? Yes that one should support it. Can you enable it the regular way by use of the push button? 

I kick the wheel with my foot, you should spin the motor quite a bit but it should work! Does the power led on the BMS turn on when you quickly turn the wheel (this should happen)? The same should happen on the VESC itself.
```

---
## \#512 Posted by: sebaszz Posted at: 2018-09-17T06:55:06.339Z Reads: 238

```
Can somebody help me out. 

First of all. I made stupid mistake by slipping out postive battery lead out of my hands while connecting.
Argghhh I was so carefull all the time, by double checking, measuring etc.
However it made very short contact with GND pin of the canbus transceiver creating a tiny spark.
There is no visual damage to the traces or components as far as I can see.
If I look at the schematics there are no components in the lowest resistance path during the short circuit so maybe nothing is damaged.

![611D1469-41D3-41B0-9DE4-0D4E9FE3EE3D|666x500](upload://zdgD1YYxsX0rFB7Y5oFLxeO9r1Z.jpeg)![03B77A36-5FD8-4979-B156-6473CA5F743B|666x500](upload://uhZJyvmpXZAEMx3vPn0CZqjYG6U.jpeg)

Now the issue.
I can only power up the bms by re-connecting usb
The bms keeps in power down state, so starting up, showing eventually message "bye"
In the real time tab there is not fault
however temperatures of the bms is fluctuating to minus values

![Capture1|690x345](upload://pnKRlbi4G873XUwTFuoT8K1OJcc.JPG)![Capture|690x347](upload://yDyQaOck95u0qruBDZXMDiVm9Hm.JPG)


What I did
I’am able to connect to the diebiems tool.
Update firmware to 0.20
Execute bootloader_jump via terminal
Read default config
Adjust battery pack to 12S
Write to BMS and save to flash
Reboot by disconnecting usb cable

When I re-connect the display shows V0.15 or V0.17  ( don't remember, unable to check) instead of V0.20 in the tool.
If I read the config in the tool after rebooting. It shows the change to 12S and V0.20
I know there is big mismatch in the cell, I need to check if this is really the case, Battery is completely new.
It was balanced couple weeks ago.

Also updated drivers, disabled temp setting etc. to get it out of the power down state.

Am I missing something or is the PCB broken?

Gr

Sebastiaan
```

---
## \#513 Posted by: bevilacqua Posted at: 2018-09-17T08:09:09.763Z Reads: 222

```
yes, push button works fine. I tried to spinn it really fast. Its a 200kv 5055, maybe the back_emf is to weak?
```

---
## \#514 Posted by: Devilmycry Posted at: 2018-09-19T02:59:03.683Z Reads: 222

```
Just see this 
How many A the bms can take for discharge thank you
```

---
## \#515 Posted by: Pantologist Posted at: 2018-09-19T03:22:43.589Z Reads: 225

```
https://www.electric-skateboard.builders/t/diy-6s-to-12s-bms-with-can/2639/26?u=pantologist
```

---
## \#516 Posted by: Pmac Posted at: 2018-09-19T07:33:15.239Z Reads: 221

```
amazing work!  I just came across this post (sadly after I have already purchased a BMS).  This is amazing.  A lot of it went over my head but from what I understood, it is amazing.

When I get some funds I will have to upgrade my BMS to this model.

I have a few questions.
Is there a way without plugging in the USB to change settings to balance the pack at ~3.7v for storage when the board won't be used over the winter period?  Can this be done over CAN with bluetooth plugged into a VESC?
```

---
## \#517 Posted by: JTAG Posted at: 2018-09-19T09:49:19.213Z Reads: 219

```
Currently that functionality is not there (yet), maybe in the future. On the shorter term I will implement a mechanism for the balance resistors to function as regenerative bleed resistor in combination with a buffer capacity of the battery (to go downhill for long even trough it was just charged). 

The desired discharge to storage voltage has close ties to this functionality, that might be added quickly after that.
```

---
## \#518 Posted by: Wraith Posted at: 2018-09-19T10:02:31.071Z Reads: 220

```
@Samau18 has a 3rd batch group buy going on now. you can get in on it as early as now as it seems like getting to the target of 50 orders is taking a while anyway. just in case you were interested :slight_smile:
```

---
## \#519 Posted by: Samau18 Posted at: 2018-09-19T10:56:42.734Z Reads: 219

```
35 pcs now
```

---
## \#520 Posted by: Pmac Posted at: 2018-09-19T12:56:34.660Z Reads: 221

```
That would be really good.  It would add a lot of safety to the board to be able to brake as soon as you jump on it.  Keep up the great work.

How do we Tip you for your great work?  As when I purchase one I will definitely have to spend a few extra dollars towards the brains behind it.

Also how is that additional piece going for the 250amp model?  I would of loved if it was expandable to 16s with the huge currant draw option as my brother wants me to electrify his quad bike and I was planning to go 16s with a 250 amp ESC on a 7-9kw (maybe 13kw if budget allows) motor.  I can definitely see there is no huge need for it with esk8 though as it would just make it bulkier for no good reason.
```

---
## \#521 Posted by: Pmac Posted at: 2018-09-19T12:59:29.793Z Reads: 210

```
You talked me into it.  I'll sign up for it tomorrow.
```

---
## \#522 Posted by: Wraith Posted at: 2018-09-19T13:01:34.949Z Reads: 218

```
[quote="Pmac, post:520, topic:2639"]
How do we Tip you for your great work? As when I purchase one I will definitely have to spend a few extra dollars towards the brains behind it.
[/quote]

Once the GB is finalized and production is started a portion of all payment goes to @JTAG for all the effort He's put in and continues to put into this awesome project :smile:
```

---
## \#523 Posted by: rpasichnyk Posted at: 2018-09-19T13:39:51.274Z Reads: 217

```
[quote="Pmac, post:516, topic:2639"]
Can this be done over CAN with bluetooth plugged into a VESC?
[/quote]


Everything that can be done via USB, can be done via bluetooth as well using latest DieBieMS Tool. I did it with a bluetooth module that is connected to VESC and VESC is connected to DieBieMS via CAN.
```

---
## \#524 Posted by: bevilacqua Posted at: 2018-09-19T13:44:57.110Z Reads: 213

```
Hi Roman, do you have "push to start" wired on your board?
```

---
## \#525 Posted by: SkaterBoy58 Posted at: 2018-09-19T13:45:13.385Z Reads: 217

```
@rpasichnyk  So Roman -Any way you can put a blue tooth module in DieBie BMS to talk to DieBie BMS tool or metr app without involving any vesc?
```

---
## \#526 Posted by: rpasichnyk Posted at: 2018-09-19T13:58:00.535Z Reads: 218

```
@bevilacqua Yes, push to start works for me with 6364 single motor.
@SkaterBoy58 no way
```

---
## \#527 Posted by: walleywalker Posted at: 2018-09-19T18:47:33.146Z Reads: 217

```
Sorry for the continued newb questions here but - How does this 'smart' BMS work when it comes to new smart VESCs like the FOCBOX Unity? 

They both have built in power switches, they both have push-to-start capabilities, and such. So how do you establish control of these types of features between the two? Does it become a case of one master and the other in a slave configuration over CAN similar to how two regular FOCBOXes would interact? 

:thinking:
```

---
## \#528 Posted by: Jc06505n Posted at: 2018-09-19T18:51:51.594Z Reads: 220

```
[quote="walleywalker, post:527, topic:2639"]
So how do you establish control of these types of features between the two? Does it become a case of one master and the other in a slave configuration over CAN similar to how two regular FOCBOXes would interact?
[/quote]


This would be better asked on the Focbox unity thread since i recall seeing a post about this on there or something similar. Good question though, @Deodand, is the unity's canbus port a simply plug in for the diebiebms?
```

---
## \#529 Posted by: JTAG Posted at: 2018-09-19T19:17:27.797Z Reads: 215

```
No problem! 

I wonder just as wel on what would be the best way to implement the Unity with the BMS, on protocol level there wont be a problem, on the power electronics side there might be, I have no idea how they implemented the switch but there will very likely be a neat way for them to collaborate.
```

---
## \#530 Posted by: Deodand Posted at: 2018-09-19T19:20:25.618Z Reads: 217

```
Yep we will get it sorted and share! Should be fairly straightforward to figure out.
```

---
## \#531 Posted by: fedestanco Posted at: 2018-09-19T19:22:29.239Z Reads: 231

```
I saw they implemented high side switching witch lm5060 which I also considered for my switch. It would be sufficient to tie the enable pin of this ic  to gnd and have the bms to cope with all of the power functions.
```

---
## \#532 Posted by: Devilmycry Posted at: 2018-09-20T00:50:48.919Z Reads: 230

```
I need on of this where I can get it and how much shipping included to US
```

---
## \#533 Posted by: Wraith Posted at: 2018-09-20T00:58:09.769Z Reads: 233

```
You can still get onboard :smile: not sure how much shipping to the US is though. @Samau18 may be able to answer that

https://www.electric-skateboard.builders/t/diebiems-v0-8-batch-3/65313?u=wraith
```

---
## \#534 Posted by: Devilmycry Posted at: 2018-09-26T02:22:54.594Z Reads: 226

```
Charge current is only 15A 
Question 
My setting for my battery min is 15 2 motor 
This mean if I break really hard I have 30A come to my battery I believe this bms will not work correct ?????
```

---
## \#535 Posted by: JTAG Posted at: 2018-09-26T06:56:37.349Z Reads: 223

```
You will be charging trough the discharge/load port (as you should), this will be no problem at all!
```

---
## \#537 Posted by: willumpie82 Posted at: 2018-09-28T07:52:11.732Z Reads: 228

```
I just read the thread about the metr.pro upgrade, just awesome progress! 

But now, the VESC is kind of the CAN master when using metr.pro and need to be powered on before the communication gets active. I prefer not having my VESCs energized for an hour or longer during charge.

Does the D.B.MS forward CAN data? if so I would be able to connect the metr.pro to the BMS serial port instead of to the VESC. 
This would open up some possibilities:
- The VESC would not have to be powered-on to monitor the charge process or battery state. 
- Metr.pro would be able to send push messages when charge is done or if there is an issue
- With push-2-start I would be able to check my battery state before rolling off
- At some point the BMS could also store VESC logging to the SDcard.
```

---
## \#538 Posted by: Trdolan03 Posted at: 2018-10-08T06:50:00.748Z Reads: 213

```
So I might have missed it but what is the current amp capacity for discharge of the unit?
```

---
## \#539 Posted by: Eretron Posted at: 2018-10-08T21:12:03.354Z Reads: 223

```
So I am waiting for my DieBie to arrive. What is the recommended charger for a 12s setup? What are you guys using. 

If I have read correct info. It is recommended that charger is about 3V higher than the full charged voltage of battery.
```

---
## \#540 Posted by: totalgeek9224 Posted at: 2018-10-11T13:19:54.895Z Reads: 222

```
[https://www.meanwell.com/productPdf.aspx?i=327](https://www.meanwell.com/productPdf.aspx?i=327)

https://eu.mouser.com/ProductDetail/MEAN-WELL/HLG-480H-48A?qs=u4fy%2FsgLU9PVn6yM5LRg%252bg%3D%3D

Ive read that these could be good for the DieBieMS. Could be useful fo you :)
```

---
## \#541 Posted by: Trdolan03 Posted at: 2018-10-11T17:07:40.198Z Reads: 217

```
So what is the status of the phone app? Is there one for IOS?
```

---
## \#542 Posted by: willumpie82 Posted at: 2018-10-15T06:30:35.380Z Reads: 219

```
metr.pro works like a charm, not for configuration though

https://www.electric-skateboard.builders/t/metr-pro-next-gen-bluetooth-module/57780
```

---
## \#543 Posted by: willumpie82 Posted at: 2018-10-15T06:38:32.790Z Reads: 218

```
damnz, those meanwell's are expensive :anguished:

for my 10S setup I use an aliexpress power supply, 42v 3A, I paid something in the range of 25€
just search for "10s lithium charger"
```

---
## \#544 Posted by: totalgeek9224 Posted at: 2018-10-15T06:46:25.437Z Reads: 213

```
Right, I've just bookmarked those because @JTAG had mentioned them somewhere.  
Additionally, I believe you need an extra 3v on top of your nominal voltage for your charger, so having the adjustable Voltage and Amperage so those are nice for that flexibility
```

---
## \#545 Posted by: Eretron Posted at: 2018-10-15T08:27:40.176Z Reads: 212

```
What do you mean? You are not able to configure VESC via metr app?
```

---
## \#546 Posted by: willumpie82 Posted at: 2018-10-15T08:43:15.409Z Reads: 216

```
Metr.pro is designed for VESC and works great for logging and configuration!

They are currently integrating DieBieMS features (state of charge with fancy animation), no configuration page for DBMS (jet?)
you can still do so via the terminal and CAN fwd (ID:10) in the app.
```

---
## \#547 Posted by: totalgeek9224 Posted at: 2018-10-21T07:09:01.882Z Reads: 211

```
@JTAG would you reccomend cell level fusing in use with this?
```

---
## \#548 Posted by: malJohann Posted at: 2018-10-24T00:50:02.534Z Reads: 210

```
@JTAG didn’t see it anywhere, but would this work with Hobbywing Max6 ESCs and off the shelf Turnigy cell packs? Do I need to have a Vedder based ESC?
```

---
## \#549 Posted by: totalgeek9224 Posted at: 2018-10-27T10:33:43.687Z Reads: 206

```
Any update on this project?! Looks like it would be amazing for some of us :)
```

---
## \#550 Posted by: Giga Posted at: 2018-10-28T01:07:50.361Z Reads: 207

```
[quote="JTAG, post:265, topic:2639, full:true"]
Any option to transform an external constant voltage supply either by implementing a buck or boosting converter to the BMS will limit its functionally/universality for the type of battery pack ( voltage ), charge power ( DC DC current ) and increase cost.

Or where you suggesting something else?
[/quote]

What about simple PWM?

I am not really familiar with switching losses, heating and stuff. But in my understanding a buck converter is only a PWM switch with additional smoothing by caps and coil. And for buck converters efficiency rises for low voltage differences (vin vs vout). So if I am right, the losses at high dutycycle switching should be small and from ~55V to 36V you are always above 65% duty, for Lipos even above 80% duty. 
And even if there is some heating, you could always regulate the charge current down according to the temperature of the closest NTC. So you do not have to have a CC/CV powersupply but a CV is sufficient (like the cheap ledstrip powersupplys)

So what do you think, could a simple software 40kHz PWM regulate the input current?
```

---
## \#551 Posted by: rene Posted at: 2018-10-28T16:11:27.788Z Reads: 215

```
Hey Guys,

I need you help. @JTAG 

Just attached the DieBieMS  to my 2 x 12s5p == 12s10p.
The balance cables and PACK +/- are connected.

- DieBieMS does power up. HW V0.7
- DieBieMS-Tools can connect to the MS states FW 0.16
- FW Upload does work.
- But after reboot - it is still 0.16
- Can NOT read / NOT write values with the DieBieMS-Tool
- only Terminal commands.
- Strange "State of charge" - 1.5% - at 12s with 48.97V it should be above 90%

What am I doing wrong?

Please find all data below.


-------    BMS Info   -------
Firmware: V0.16
Hardware: V0.3
Name    : DieBieMS
UUID: 33 00 3E 00 10 57 34 56 36 30 33 20
------- End BMS Info  -------


-----   Cell voltages   -----
Cell voltage 0             : 4.088V
Cell voltage 1             : 4.089V
Cell voltage 2             : 4.080V
Cell voltage 3             : 4.089V
Cell voltage 4             : 4.089V
Cell voltage 5             : 4.089V
Cell voltage 6             : 4.089V
Cell voltage 7             : 4.088V
Cell voltage 8             : 4.089V
Cell voltage 9             : 4.089V
Cell voltage10             : 4.089V
Cell voltage11             : 4.083V
Cell voltage high          : 4.089V
Cell voltage low           : 4.080V
Cell voltage average       : 4.088V
Cell voltage mismatch      : 0.009V
----- End Cell voltages -----
 
-----Battery Pack Status-----
Pack voltage          : 48.97V
Pack current          : 0.02A
State of charge       : 1.4%
Remaining capacity    : 0.57Ah
Operational state     : External (USB or CAN)
Load voltage          : 0.00V
Cell voltage high     : 4.089V
Cell voltage low      : 4.082V
Cell voltage average  : 4.088V
Cell voltage mismatch : 0.008V
Discharge enabled     : False
Charge enabled        : False
---End Battery Pack Status---


---   BMS Configuration   ---
NoOfCells                  : 12
batteryCapacity            : 41.00Ah
cellHardUnderVoltage       : 3.400V
cellHardOverVoltage        : 4.250V
cellSoftUnderVoltage       : 3.300V
cellSoftOverVoltage        : 4.250V
cellBalanceStart           : 4.100V
cellBalanceDiffThreshold   : 0.010V
CAN ID                     : 10
--- End BMS Configuration ---
```

---
## \#552 Posted by: rene Posted at: 2018-10-28T20:26:46.278Z Reads: 198

```
OK @JTAG  - read the whole thread again and found the part where you describe the bootloader_jump command.

Now it says v0.21 in the DieBieMS-Tool - but the LCD states v0.17 at boot.

Is this normal?
```

---
## \#553 Posted by: JTAG Posted at: 2018-10-28T20:31:48.472Z Reads: 216

```
Hi guys!

Sorry for the lack of response from me lately I have been very busy. But also busy on adding new features to the BMS and the interface. The most important thing I am working on is a self test feature to test the BMS after production and changing the hardware to add test pads for a test fixture.

I will soon take time to answer all unanswered questions soon! 

And for the last question, I am sorry that might indeed be a bug :stuck_out_tongue: . I still have to automate incrementing the firmware version on every place in the firmware automatically.
```

---
## \#554 Posted by: rene Posted at: 2018-10-28T20:35:02.470Z Reads: 219

```
DieBieMS is now managing 12s10p of 20700B.

Wow - this is just the coolest BMS around!
Thanks @JTAG from Hamburg.  

![image|666x500](upload://o3bHZaSvyAESO6UUxRKjTRS3rFm.jpeg)
```

---
## \#555 Posted by: totalgeek9224 Posted at: 2018-11-02T20:29:43.259Z Reads: 216

```
@JTAG anything buddy?
 :slight_smile:
```

---
## \#556 Posted by: Klaerke91 Posted at: 2018-11-02T20:31:57.758Z Reads: 218

```
you can maybe still get one here

https://www.electric-skateboard.builders/t/diebiems-v0-8-batch-3/65313
```

---
## \#557 Posted by: totalgeek9224 Posted at: 2018-11-02T20:33:06.691Z Reads: 214

```
Was actually referring to the "More amps shield" that he was (or is) developing,
Thanks though!!
```

---
## \#558 Posted by: skatardude10 Posted at: 2018-11-02T21:11:55.049Z Reads: 212

```
It'd be great if someone would do a large run to keep these in stock. I don't need one right now, but in the future it'd be great to have to option to buy it outright instead of waiting on a GB. I could see this becoming the new standard if it we're more available.
```

---
## \#559 Posted by: Samau18 Posted at: 2018-11-03T08:55:24.139Z Reads: 213

```
I made extras with this run. 

Sam
```

---
## \#560 Posted by: malJohann Posted at: 2018-11-04T10:15:13.419Z Reads: 215

```
@JTAG didn’t see it anywhere, but would this work with Hobbywing Max6 ESCs and off the shelf Turnigy cell packs? Do I need to have a Vedder based ESC?
```

---
## \#561 Posted by: Klaerke91 Posted at: 2018-11-04T17:22:25.194Z Reads: 213

```
you dont need a vesc, but some of the functions will not work without it
```

---
## \#562 Posted by: evoheyax Posted at: 2018-11-13T06:37:23.281Z Reads: 227

```
@JTAG

Thank you so much for this great work. I've been loosely following your progress from the beginning and I'm catching up now on what I've missed lately and it's a lot.

I have 2x the V0.8, and reading back, I saw you mention the MoreAmpsShield last December (2017). I haven't seen anything about this since then. Do you have any idea when I could expect more from this?

I'm debating what to do right now as 80a is just not enough for me (was trying to do 200a+, as I run 4wd). I read before the plan was to allow this to support 140a in theory as it is. Have you tested this yet? Is there a 140a fuse that will fit nicely?

Charging wise, limit is 15a, correct?

I'm a bit confused on the charge current. You said to detect charge, it needs to be 3v above pack voltage? So it won't detect a charge if say my pack is at 49v and the charge current is 50.4v? Do I need to set it to 53.4 then?

I'm still confused about the canbus connection to the vesc, but hopefully I find something that clarifies this soon (still not done reading all of the topics and every message, soooo much to read, haha). Do you just need to connect CAN L BMS -> CAN L VESC and CAN H BMS to CAN H VESC?

The manual would be great. I might through something together in the mean time for others, because it's not efficient for everyone single person to read all of these lengthy threads. Already been about 4 hours and I still have at least 2 more to go through.

Thanks again for this amazing piece of work. Would love to use the full power potential of my setup though (200a+, could even set each vesc to 80a for 360a total in theory). I think it's worth limiting my power output for the time being and using this instead of not using a bms, since I'm now using a 25ah lipo pack. But would love to get this running at higher amps.
```

---
## \#563 Posted by: evoheyax Posted at: 2018-11-13T06:52:46.765Z Reads: 228

```
In general, the ESC should have no effect on the bms. They are separate, compartmentalized systems. This bms has a canbus port, which the vesc also has, and it seems there's some firmware stuff being implemented so the VESC and BMS can be blended together nicely. But this is the icing on the cake.

Personally, I would recommend a VESC, especially a VESC 6. I've tried pretty most vesc's out there and the only ones standing still are the official VESC 6 (damn you Frank for charging so much!!! I know how cheap your BOM is now!) and the Axle and Chaka Vesc 4.12's. It pays in the long term to use quality parts (remember, electric skateboarding can be deadly, especially if you experience electrical failures at the wrong time).
```

---
## \#564 Posted by: willumpie82 Posted at: 2018-11-14T07:59:00.531Z Reads: 223

```
**Charge voltage:**
should 0,7v above pack voltage to be able to fully charge (due to protection diode 

**the CAN connection:**
VESC1  | VESC2 | BMS
canH     | canH     | canH
canL      | canL     | canL
--            | 5v         | 5v CAN
--            | 5v         | Enable Can  (<-- connect to 5v for push2Start)
GND      | GND     | GND

5v_CAN is mandatory to power the primary can circuit on the dbMS
Enable_Can  is optional connected to 5v_VESC for push2Start


pinout of the dbms
![image|690x260](upload://wEYr27n5RVwHoRjwqSnL5Peh2j3.jpeg)
```

---
## \#565 Posted by: rene Posted at: 2018-11-15T07:39:11.378Z Reads: 211

```
Do you guys also realized that the two chips between the positiv ports do get HOT?
And that every other BMS got heat sinks but DieBieMS does not.

Did someone worked on this?
```

---
## \#566 Posted by: evoheyax Posted at: 2018-11-16T21:36:34.210Z Reads: 210

```
@rene Do you or anyone one else have any adivce on crimpting the J12 connector? Maybe the wire I'm using is too large or something, but I'm having a hard time getting those little legs to clip. It looks pretty clen and narrow, but when I pull it out, the legs look bent inward and I have to use tweezers to pull them back out. But everytime I try to insert it, the pins get pushed in and stay, they don't spring back out and get connected, even though I get the entire pin in.

Any advice is much appreciated as it's driving me crazy to where I want to just de solder the port and solder directly. to the pcb haha. But I'm trying to restrain myself.

Does anyone know of the proper name for this connector? I wouldn't mind even picking up a pre-crypted cable with the port on it. All I can find on the schematics and BOM is J12.
```

---
## \#567 Posted by: hexakopter Posted at: 2018-11-16T22:44:04.416Z Reads: 211

```
[quote="evoheyax, post:566, topic:2639"]
Does anyone know of the proper name for this connector? I wouldn’t mind even picking up a pre-crypted cable with the port on it. All I can find on the schematics and BOM is J12.
[/quote]
Its a WR-MPC3 connector that should be used with 20-24AWG wire. At least that is the conclusion I came to. :sweat_smile:

[quote="hexakopter, post:253, topic:58327"]
I see that a WR-MPC3 connector is used for the balance leads and that 20 crimp terminals are already within the package. I don’t have the BMS near me right now and would like to order some silicone wires now, but the Würth website tells me there are two types of crimp terminals available. [http://katalog.we-online.de/de/em/MPC3_3_00_MALE_CRIMP_TERMINAL_662X0213722 ](http://katalog.we-online.de/de/em/MPC3_3_00_MALE_CRIMP_TERMINAL_662X0213722)
Are the ones we received the ones for 20-24AWG wire or the ones for 26-30AWG wire?
[/quote]
https://www.electric-skateboard.builders/t/diebiems-v0-8-2nd-batch-total-48pcs-closed/58327/262
```

---
## \#568 Posted by: evoheyax Posted at: 2018-11-17T23:55:57.948Z Reads: 203

```
So this wiring diagram unfortunately doesn't help with the latest gen of switches. They have the following listed names: C, NO, NC, LED, and A.

Doesn't anyone know the correct wiring?

I would love to get this bms working. I'm just finding it hard as information gets old and then theirs no documentation for most of what I'm have to do as the end user to get this running.
```

---
## \#569 Posted by: evoheyax Posted at: 2018-11-18T00:07:26.149Z Reads: 211

```
What would have been amazing for future groups buys would be if cables were pre-crimped and wires pre soldered to the switch. I would pay an extra $30 to not have to guess and break stuff trying to figure out what is what.

So far, I likley blew the first one because I got frustrated with this stupid balance plug.

The second one is like the first, in that I plug it into the computer and windows chimes and it shows under devices. But it doesn't find it when I used the DieBieMS tool. Both are v0.8. I get no lights on the bms, either. I connected my battery to it and tried to use the switch, but nothing works. It's been over 15 hours now I've spent trying to get this bms working and I'm ready to just throw it in the trash and move on.

Update: So the second one I was able to get the firmware updated, and it now powers on when I plug in the usb. But it shows 0 volt for the battery pack. It this because I don't have the battery balance wires plugged in? It shows the bms temp correct (I activated rt data).
```

---
## \#570 Posted by: Prism Posted at: 2018-11-18T01:02:04.826Z Reads: 215

```
The correct wiring for the switch is: 
C and NO for the switch. That is the red and black wire. 
LED and A is for the LED. The green and the blue wire. 
The yellow one is not used. Same with the NC contact of the switch. 
![bms_switch|690x339](upload://9UbmCOnlcnhq6xOpzHVq30LYqsS.jpeg)
```

---
## \#571 Posted by: chocol4te Posted at: 2018-11-18T11:11:13.508Z Reads: 213

```
Hello!

My BMS has been working great in my board, but I have been trying to plug it in to my computer over USB to change some settings and have encountered some issues. If I plug it in, lights do not come on, but it does appear as SLAB_USBtoUART in vesc_tool, Ackmaniac's tool and DieBieMS tool, but after trying to connect in all 3, I get a `No firmware read response` error. I get the same issue when using CAN forwarding to connect to it.

I also cannot seem to flash it using my STLinkV2 using the debug connector on the side of the board, it is apparently not recognised or connected, even after I double checked all the connections.

Any ideas?

Edit: My debug connection wasn't as good as I thought, I soldered it and manually flashed the bootloader and firmware to the correct addresses using OpenOCD, but still getting the `No firmware read response` error :(

Edit 2: I tried flashing the VESC boot loader, and the older DieBieMS firmware, using a different machine and still no luck :(
```

---
## \#572 Posted by: tsr Posted at: 2018-11-19T08:45:26.756Z Reads: 201

```
Don't know which is the correct thread anymore, so i used this one;) Can I still order the DieBieMS somewhere?
```

---
## \#573 Posted by: Eretron Posted at: 2018-11-19T08:51:14.465Z Reads: 199

```
Try here. I think there are some extras made. 

[https://www.electric-skateboard.builders/t/diebiems-v0-8-batch-3/65313](https://www.electric-skateboard.builders/t/diebiems-v0-8-batch-3/65313)
```

---
## \#574 Posted by: chocol4te Posted at: 2018-11-19T19:36:49.086Z Reads: 201

```
@evoheyax May I ask what firmware versions you used, and the steps you took to be able to use it over USB? I think I have the same problem :(
```

---
## \#575 Posted by: evoheyax Posted at: 2018-11-19T22:00:17.771Z Reads: 201

```
I tried my best to wire up the based on what I knew at the time to do the power switch. Hooking it up to my battery, and then pressing the switch turned it on (with the usb).

I have the switch weird up correctly now. Working on the display and waiting for pre crimped wires so I hopefully can get them to fit into the connector for the balance wires.
```

---
## \#576 Posted by: evoheyax Posted at: 2018-11-19T22:08:48.461Z Reads: 199

```
Thank you for the diagram!

I wired up the switch correctly and it seems to work. The bms turns off after a few seconds though. I'm assuming this is because I only have batt - and batt + connected, with no balance cable yet?

Also, when I plug the screen in, nothing happens on the screen, but the power switch blinks a few times before it turns off. Unplugging the display returns the power switch to the state above (no fast blinking before turning itself off).

EDIT: Solved! If you mess up the wiring, it will I guess it will blink before shutting off! Glad it doesn't just blow up! Now it shows a battery with and x, then says bye and shuts off, haha.

I guess this is all normal since I don't have balance wires connected yet.
```

---
## \#577 Posted by: evoheyax Posted at: 2018-11-19T22:40:09.462Z Reads: 195

```
The other thing I'm wondering if any can answer is...

Is this really bms limited to 80 amps (as the silk screen infers)? That is to say, If I put a 130 amp fuse, would that be an issue? (JTAG originally said 140a theoretically)

Also, I saw this asked before, but I didn't see an answer, as to what is the type of fuse these are called? Trying to find replacements but not sure. I have been running 120 amp across 4 vescs and was very happy with the performance. If I could keep that and not have to put this bms in parallel, I would love this bms that much more!
```

---
## \#578 Posted by: Ckarg Posted at: 2018-11-20T01:35:07.117Z Reads: 199

```
@JTAG @Samau18, mostly the same question as above: would these work? 
https://www.littelfuse.com/~/media/automotive/datasheets/fuses/passenger-car-and-commercial-vehicle/bolt-down-fuses/littelfuse_bf1_58v_datasheet.pdf

Looking at the 125 amp available from Digikey:
https://www.digikey.ca/product-detail/en/littelfuse-inc/142.7010.6122/F11191-ND/5234200
```

---
## \#579 Posted by: evoheyax Posted at: 2018-11-20T02:26:08.358Z Reads: 196

```
If that works, looks great. If theoretically 140a is the true amp, 125 would be a nice in between. Since I’d want to limit it 10 amps lower than the fuse so I don’t blow fuses during hard accelerations.
```

---
## \#580 Posted by: Ckarg Posted at: 2018-11-20T02:31:12.748Z Reads: 198

```
That is exactly what my thinking was. I am building two 12S6P packs using samsung 25r's. So this would fit nicely; especially paired with either the Unity or FSESC dual.
```

---
## \#581 Posted by: evoheyax Posted at: 2018-11-20T02:34:32.445Z Reads: 194

```
Yep that sounds about right. I ride 4wd, so it’s tough to get a bms that can power 4 vescs to their full potential. That and I just built a 12s 25ah lipo pack (a bit over a kilowatt of juice) that could easily do 400 amps con. 120 ish is still limiting, but ok for now until the more amps shield is ready.
```

---
## \#582 Posted by: Ckarg Posted at: 2018-11-20T02:43:24.074Z Reads: 193

```
It's too bad that the development of the more amp Shield has gone silent! Till then I'm just paralleling my my two DieBieMS's for the 200 amps I'm looking for.
```

---
## \#583 Posted by: chocol4te Posted at: 2018-11-20T11:44:24.795Z Reads: 200

```
Hmm, now the lights come on, but still no communication with any tools :frowning:

I don't suppose anyone could use an STLink to download their entire flash so that I can write it? I can't think of anything else to try :confused:
```

---
## \#584 Posted by: JTAG Posted at: 2018-11-20T12:02:57.368Z Reads: 207

```
The firmware can be found here:
https://github.com/DieBieEngineering/DieBieMS-Tool/tree/master/res/firmwares/DieBieMS

First erase the chip, Pick the default firmware and flash it, and when communication works with the BMS be sure to upload the bootloader with the BMS tool for the next firmware update with the BMS tool.
```

---
## \#585 Posted by: JTAG Posted at: 2018-11-20T12:06:51.617Z Reads: 220

```
![IMG_20180830_143052|666x500](upload://7zk7WksIgF0ilWtqWQ7DAANfGtQ.jpeg) 

![IMG_20180830_142725|435x500](upload://zfecB52lV4DFln2Fa0tXh7gh7oE.jpeg) 

We are doing tests with it, but 150A is ALOT, and are still improving.
```

---
## \#586 Posted by: chocol4te Posted at: 2018-11-20T12:30:21.165Z Reads: 211

```
So I used `st-flash erase`, then `st-flash write DieBieMS_default.bin 0x08000000`, then unplugged the debugger and plugged in the USB cable.

It shows up, but I'm still getting `No firmware read response`, regardless of whether my battery pack is connected, whether the debugger is providing power or not, nothing. Flashing or not flashing the boot loader to 0x08032000 makes no difference.

Do you have any other debugging steps I can try?
```

---
## \#587 Posted by: Friskies Posted at: 2018-11-20T13:44:08.550Z Reads: 205

```
Wait did @JTAG just tell us that the BMS can handle 150 amps discharge???
```

---
## \#588 Posted by: Ckarg Posted at: 2018-11-20T14:00:05.840Z Reads: 205

```
If you look closely at the second picture it is a DieBieMS with the more amps shield. 🤔 So it's still up in the air about just the DieBieMS. Though heart pumping to see the elusive more amp shield in the wild 😍
```

---
## \#589 Posted by: JTAG Posted at: 2018-11-20T15:03:18.639Z Reads: 204

```
Does the LED blink a couple of times? 

Did it ever work or just suddenly stop? I believe that every thing including the usb was tested during the production, so at some point it should have worked.
```

---
## \#590 Posted by: JTAG Posted at: 2018-11-20T15:06:19.641Z Reads: 202

```
Yes it is doing 150A but only for 15 minutes ( then the temperature raised to 70 degree C and the battery itself became warm and we stopped ).

But at 150A and 15 minutes the battery was also almost drained
```

---
## \#591 Posted by: Surfer Posted at: 2018-11-20T15:30:16.029Z Reads: 202

```
Hallo @JTAG, just curious if you did consider to build a charging only BMS with very small footprint, smart enough to work with metr.pro?
Dank u!
```

---
## \#592 Posted by: chocol4te Posted at: 2018-11-20T16:14:56.996Z Reads: 206

```
It always worked, I had it in my board for a few months, but wanted to set up CAN forwarding, so I disassembled my board and hooked it up only to find it no longer connecting. It still charged, and discharged correctly, until I flashed firmware (but that is most likely due to the default being 10 cells not 12). Now when powered it slow blinks, then after a while goes off with the second LED always remaining lit. Neither LED turns on when only connected via USB.
```

---
## \#593 Posted by: evoheyax Posted at: 2018-11-20T17:36:58.638Z Reads: 213

```
@JTAG Ahhh great to see you still around and testing the more amps shield. Do you not recommend trying to do more than 80 amps then with out the more amps shield?

I'm tempted to get that 125 amp fuse and see what happens. If it's a bad idea, would love to be told off before I blew it up, haha.
```

---
## \#594 Posted by: SkaterBoy58 Posted at: 2018-12-04T05:07:32.702Z Reads: 202

```
Anyone by any change got the dimensions between the four mounting holes on PCB?
```

---
## \#595 Posted by: AlexBE Posted at: 2018-12-04T05:46:29.984Z Reads: 200

```
@JTAG, I'm wondering how the bootloader is programmed onto the device in the first place? Do you purchase the chips preprogrammed?
```

---
## \#596 Posted by: Joon Posted at: 2018-12-04T12:45:29.964Z Reads: 199

```
Yeah, the pattern is **90 mm x40 mm** measured from the centres of the holes which should have a diameter of **3.2 mm**. 
in case you wanna know more dimensions and you haven't seen the link, [here's the Github link for the 3D files.](https://github.com/DieBieEngineering/DieBieMS/tree/master/3DFiles) I also double checked the dimensions by hand and it's correct.
```

---
## \#597 Posted by: SkaterBoy58 Posted at: 2018-12-05T03:47:16.384Z Reads: 195

```
@Joon Thanks a lot
```

---
## \#598 Posted by: JTAG Posted at: 2018-12-05T19:34:53.549Z Reads: 193

```
They are programmed trough the SWD debug connector on the bottom, when DIY assembling you have to do that yourself. You could first flash the main application followed by the bootloader either trough the DieBieMS tool or directly with the debugger. Notice that this bootloader works different than the arduino style bootloader (the BMS has the same style as the VESC).
```

---
## \#599 Posted by: JTAG Posted at: 2018-12-05T19:39:34.474Z Reads: 197

```
I am thinking about designing a small and compact one, but that is still a very long time away.... What functionality would you like to get rid off? only discharging or would you also accept slow balancing?

@evoheyax As a very short pulse it might handle it, but not sure for how long :stuck_out_tongue:. I could to a small test and film it with the Flir and webcam, I do have to find a suitable battery and wiring trough.....

@Joon Thanks! We sould put the mechanical drawings in the manual as well :....
```

---
## \#600 Posted by: totalgeek9224 Posted at: 2018-12-05T20:13:46.034Z Reads: 200

```
How far off... ;) 
Like how could we get you to design a compact bms that could be suitable for high discharge. Like we need something like the DBMS but higher discharge, even if it sacrafices the size a lil.

What do you think? Do we need to hire you? ;)
```

---
## \#601 Posted by: Surfer Posted at: 2018-12-05T20:18:47.093Z Reads: 200

```
That's a good news!!! Thanks :p
For what most I would like it is for monitoring with metr.pro, if it's doing also balance even better, doesn't matter if is slow balancing.
 For my liking it will be 10s-12s, charge around 4-5 amps, UART, balancing and small, kind of 3 or 4p 16850 size.
Thanks !!!
```

---
## \#602 Posted by: JTAG Posted at: 2018-12-05T20:57:40.584Z Reads: 197

```
5A 12S should be doable, will look into it next year, I won't be promising anything :stuck_out_tongue:. Some things just might need to go, and be a little less fancy... this might suppress the cost  and benefit size. But enough projects for now :nerd_face:.

For a small footprint high discharge BMS would you accept a narrow but long (30 times 160mm) BMS that needs to be mounted on a strip of aluminium? What would be an acceptable method of mounting the wires (avoiding press fits)?
```

---
## \#603 Posted by: AlexBE Posted at: 2018-12-06T06:09:26.344Z Reads: 194

```
Ahh thanks, I missed that connector in the schematic.
```

---
## \#604 Posted by: AlexBE Posted at: 2018-12-06T06:11:26.615Z Reads: 192

```
For those after a smaller size, I am considering modifying the layout and putting the cell balancing on the bottom of the board, 140mm is a little too wide for my build. If I do it, I will post the modified files so others can build the smaller PCB.
```

---
## \#605 Posted by: totalgeek9224 Posted at: 2018-12-06T12:40:01.492Z Reads: 191

```
[quote="JTAG, post:602, topic:2639"]
would you accept a narrow but long (30 times 160mm) BMS that needs to be mounted on a strip of aluminium
[/quote]

I dont see why not. As it stands the DBMS is large but people still use it for its functionallity. That being said, 160mm it a bit long, as even something like @Eboosted DS enclosure is about 152 mm (i think, Alan? how far off am i?) I think you might be able to get away with trading the length for thickness, producing someething like a double pcb BMS that could be stacked or something. 

OH! That makes me wonder, whats the feasability of having a charge only bms module (small) that could be upgraded with a high discharge portion, depending on the need of the user?
```

---
## \#606 Posted by: JTAG Posted at: 2018-12-06T12:54:36.470Z Reads: 183

```
Just looking for the mechanical limits :P . 160mm are 8 times a 18650 with 20mm center to center, that's why I thought it would be reasonable. 

Yes external discharge switch is absolutely doable but complicate dings a whole lot when explaining and debugging. I am not super negative, just sceptical....
```

---
## \#607 Posted by: totalgeek9224 Posted at: 2018-12-06T12:58:57.548Z Reads: 188

```
[quote="JTAG, post:606, topic:2639"]
just sceptical…
[/quote]

I think skepticism is appreciated, especially when talking about something where you clearly have more experience. Maybe 160mm isn't that absurd, and i think at the end of the day it would depend on the way that the final product is designed that will dictate wether or not it would make sense to use. I would like to imagine a system where the bms and VESC are both mounted on a heatsink(s) and are easy to integrate, so, would love to see what you have in mind either way!
```

---
## \#608 Posted by: Itsmedant Posted at: 2018-12-06T17:25:14.175Z Reads: 202

```
Was there ever a full manual and diagram for this written up? I'm about to wire it all up to the new battery I'm making and want to make sure I'm doing it 100% correctly.

I've found various pictures of people drawing out how to hook up the switch and the charging port, but still didn't see an official manual. (or is it all just the info thats posted throughout this thread and I need to extract it?)

Also, this is my first ever BMS that I'm wring up so I'm a total noob here.
```

---
## \#609 Posted by: evoheyax Posted at: 2018-12-06T19:00:31.126Z Reads: 211

```
So not too much need to be done to wire it up. I'll see if I can compile a quick guide here:

First, easy enough to wire up the power switch and screen

![image|690x339](upload://u2U1qkFnxgyl4grO9V6aUJy40yW.jpeg)

_____________________

Then the balance plug is simple:

![image|666x500](upload://gfSjDB7tu8NPt93XLzCdcudbDsl.png) 

If you want to use temp sensors, which btw I think everyone should since it's implemented and a huge safety feature, then connect 1 side of the temp sensor to the gnd, and the other to t1. For the second temp sensor, again, connect 1 side to gnd and the other to t2. Remember, temp sensors are variable resistors. So as they heat up, they change their resistance and the BMS simply measures the resistance to figure out what temp it is. Pretty nifty, eh?

If not using temp sensors, leave gnd, t1, and t2 empty.

If you need temp sensors, I'm using these: https://www.amazon.com/gp/product/B06XR1TG5N
And if you need wire's pre-crympt, I'm using these: https://www.mouser.com/ProductDetail/710-662100124015
_______________

Then, the actual wiring:

Pack + -> Positive of the battery
Pack - -> Negative of the battery
Charge + -> Positive of the charger
Load + -> Positive of the VESC or other ESC (You'd better use a VESC *shakes fist in anger*)
Common - -> Negative of the VESC or other ESC **AND** negative of the charger

__________________

For the canbus, here's how to wire up with the vesc:

(Please note, CAN H and Can L are the center 2 pins of the VESC CANBus Port)
(on the 4.12: CAN H is the center pin, closer to the FETs, and CAN L is the other center pin, closer to the big external caps, 5v is the pin closest to the FET's, and GND is the opposite side)

All Vesc's CAN L -> BMS CAN L
All Vesc's CAN H -> BMS CAN H
1 Vesc's 5v -> BMS 5v CAN **AND** Enable Can (Enable Can is for push to start)
All Vesc's GND -> BMS CAN GND

By Default, The ID of the BMS for CanBus purposes should be 10.

That should be everything condensed into one post that should get you up and started.
```

---
## \#610 Posted by: Itsmedant Posted at: 2018-12-06T19:12:00.636Z Reads: 188

```
Awesome, yea having it all condensed here makes it alot easier!!!!

Thanks so much man! I'm excited to get this going and running.
```

---
## \#611 Posted by: evoheyax Posted at: 2018-12-06T19:15:04.139Z Reads: 187

```
As am I, haha. I still haven't done the final wire up or the balance plug. I had a nightmare getting those pins crympted for the balance cable's port, so I ended up ordering some from mouser pre-crypmt.

If anyone has the same issue, here's a link to ones that will fit (I've already tested and confirmed they are a perfect match): https://www.mouser.com/ProductDetail/710-662100124015
```

---
## \#612 Posted by: Itsmedant Posted at: 2018-12-06T19:18:57.138Z Reads: 182

```
Ah crap, I forgot about that. I wonder if my regular crimpers will work. Or maybe I'll just buy these.
```

---
## \#613 Posted by: evoheyax Posted at: 2018-12-06T19:23:09.496Z Reads: 185

```
Trying to use crimpers was a nightmare for me and I couldn't get them all the way in.

I found their shipping was very fast. But the wires are complete shit IMO, not a good soft silicon wire. But it should get the job done.
```

---
## \#614 Posted by: Itsmedant Posted at: 2018-12-06T19:36:46.102Z Reads: 185

```
I may still have my old crimper for old serial connectors, it would work, but not sure if I still have it or not.

Oh well, small issue in a bigger adventure!
```

---
## \#615 Posted by: Prism Posted at: 2018-12-06T23:13:43.992Z Reads: 200

```
On the topic of crimping the balance cables. I used a crimping tool for AMP MODU IV contacts that I have access to at the place I work at. 
https://www.distrelec.de/Web/WebShopImages/landscape_large/5-/40/te-connectivity-169481-1.jpg
the WR-MPC3 contact is very similar to the AMP MODU IV crimp contact on the wire side. 

WR-MPC3:
https://www.distrelec.de/Web/WebShopImages/landscape_large/63/74/66200113722DEC.jpg

AMP MODU IV:
https://asset.conrad.com/media10/isa/160267/c1/-/de/1094787_LB_00_FB/te-connectivity-crimpkontakt-ampmodu-mod-iv-polzahl-gesamt-1-167024-3-1-st.jpg?x=520&y=520

It worked quite well so I thought I'd share my experience.
```

---
## \#616 Posted by: Prism Posted at: 2018-12-07T13:40:40.667Z Reads: 199

```
Since this thread is about the DieBieMS and my DIY battery uses one I'm gonna ask here.

I build my pack a few weeks ago. The rest of my project (not a skateboard, I'm putting it on my scooter) isn't finished so I can't use it yet. I have it sitting on my desk, do some testing and configuration changes with it and my vesc from time to time. 
Today I turn it on and got the battery with an X on the display. I immediately checked the pack voltage but it dtill was at 41 volts (pack is 10S3P). So I connected it to my pc and fired up the DieBieMSTool to check the individual cell voltages and I see this: 
https://puu.sh/CdXnI/debd14beea.png

C3 and C5 have dropped quite a bit and I have no idea why. Anyone here has an idea? 
I really hope I don't have bad cells. 
I really don't want to have to take the pack apart and search for broken cells.
The cells I used are new LG HG2 18650.
```

---
## \#617 Posted by: Trdolan03 Posted at: 2018-12-07T15:47:44.045Z Reads: 190

```
I would definitely say bad cells. Most likely 2 bad cells in c5 and 1 in c3
```

---
## \#618 Posted by: JTAG Posted at: 2018-12-07T16:05:59.520Z Reads: 197

```
This can be caused by several things:

1. One or more cells in your parallel group of groups (C3 and C5) got disconnected for some reason and now those groups have a lower capacity, therefore discharged faster and now have a lower voltage.(medium bad because now you have to reweld them / resolder them). I had exactly this happen to me but than with a single group multiple times (I wasnt skilled at welding yet), but because I have a 6S4P pack and only discharge slowly I only noticed it when my board cut of (by the bms) instead of throttling back (VESC), but one will only notice that when you have it configured correctly (the VESC) and use the board often.
2. some of your balance leads came lose and therefore the reading of the BMS is wrong. However normally when this happen two cells right next tho each other have a strange reading instead of in your case where two readings are wrong with a healthy in the middel, therefore I think this isn't the case.
3. Some of the main current carrying connections between the parallel groups opened resulting in large voltages across the cell balance inputs of the BMS (this could be bad). This is very annoying to debug.

Some things you could do to diagnose further:

1. Measure the parallel group voltages individually on the balance connector.
2. Measure the parallel group voltages on the batteries directly (but be sure not to accidentally apply pressure on the nickel that cause a broken weld to attach to the cell again :P , I say thay because I had that trap for young players happen to me more often than I prefer :( ).
3. turn everything on and try to load the system a bit by slightly running the motor, if this works the connection between your parallel groups are likely to be OK.
```

---
## \#619 Posted by: Prism Posted at: 2018-12-07T19:50:19.968Z Reads: 181

```
Thanks for the replies. 

I checked all welds and balance lead connections and they seem fine. Nothing looks or feels loose. 
Measuring the cells in question directly on the nickel strip, I get 3,72V on C3 and 3,19V at C5. Just like the BMS reports in the software. 

The pack was never in use so it didn't experience any mechanical stress from vibrations. Highest electrical load was 3A maybe 4A max. from spinning my motor without any load. 

Should I just try to charge the two p-groups manualy and see if they discharge on their own again?
```

---
## \#620 Posted by: DeathCookies Posted at: 2018-12-07T19:59:44.179Z Reads: 188

```
[quote="Prism, post:619, topic:2639"]
Should I just try to charge the two p-groups manualy and see if they discharge on their own again?
[/quote]

Good idea! Try to Balance the Pack manualy and inspect it carefully. It is worth a try before you are going to disassemble sth.
```

---
## \#621 Posted by: JTAG Posted at: 2018-12-07T20:27:00.459Z Reads: 188

```
All welds are ok and the battery isn't used? Are the cells used or reused? Was it balanced when you assembled them? 

If those two cells groups discharged themselves this  could be because of bad cells ( never happens two times in the same pack ), or the BMS got damaged and is now leaking current ( can happen when you connected it wrong and fixed it later ) or the BMS was faulty from the start. I have only seen this happen once in maybe 50 boards, but then only on one group and not two.
```

---
## \#622 Posted by: Prism Posted at: 2018-12-07T21:02:26.202Z Reads: 192

```
Cells are all new and arrived with 3,5V. After assembling my pack I was at 35V. 
I double checked all balance leads both physically and electrically before plugin in the balance connector.
The only mistake I made was not plugging in the ground of the balance connector but after seeing a to low voltage on C0 in the tool I fixed that. Afterwards I charged it with 42V and 2A till it was fully charged. 

I'm gonna charge the two p-groups manually and see if they discharge on their own again. That way I can rule out the BMS as the problem.
```

---
## \#623 Posted by: JTAG Posted at: 2018-12-07T22:32:52.171Z Reads: 192

```
That all sounds good and you did all you could have done. You could indeed charge them and measure with a couple hours intervals whether they are discharging.
```

---
## \#624 Posted by: Joon Posted at: 2018-12-07T23:37:05.470Z Reads: 197

```
@Itsmedant 
Up to January I'll be getting a DieBieMS system ready for use in an electric boat (together with some fellow students and the help of @JTAG) and one for my skateboard. The BMS in the boat needs some proper documentation as it will be used by other people with varying knowledge of electrical systems. We might as well kill two birds with one stone and also help other users of the DieBieMS!

I'll write a manual which is intended for novice and upwards builders. A starting DIYer without electrical engineering knowledge (but with some common sense) should be able to hook the BMS up with the manual without getting into too many details. Once that is finished it can be expanded with more advanced sections. Hopefully @JTAG could check whether the draft is correct so you can be sure you're getting the right information once the first part is completed. I'll also try my best to add the right references to schematics and photos and credits where due.

I don't think this forum is the best place for a manual. Posts easily get lost in this thread and it takes a long time to find the information you're looking for, if it even can be found at all. The [DieBieMS Github](https://github.com/DieBieEngineering/DieBieMS) might be more suitable. 

If you have any feedback or questions, please let me know. I'll be happy to answer :slight_smile:
```

---
## \#625 Posted by: Wraith Posted at: 2018-12-08T00:28:33.840Z Reads: 185

```
This sounds like something I could definitely use! I'll be getting my DieBieMS in a few weeks time and I have no background in electrical engineering so this could be a life saver!
```

---
## \#626 Posted by: Prism Posted at: 2018-12-09T19:17:56.540Z Reads: 186

```
I charged my cells and let them sit without anything connected for a while and unfortunately the slowly discharge themselves. 

Good news: the BMS is not the problem
Bad news: I have to take apart my newly build battery pack and put new cells in

Can anyone give me advise on how to safely break up spotwelded connections so I can spotweld to the good cells again? Do I just pull the strips of and sand down the rest?
```

---
## \#627 Posted by: JTAG Posted at: 2018-12-09T19:39:29.866Z Reads: 182

```
New cells that discharge themselves? Wow that is VERY scary.... Where did you get them?
```

---
## \#628 Posted by: Prism Posted at: 2018-12-09T19:47:52.389Z Reads: 188

```
nkon.nl
I don't think I got bad cells. They arrived with 3,5V each and held that voltage till I built my pack a few weeks later.
I suspect that I did something wrong while building my pack. It's my first battery after all. 
I used the car battery + starter solenoid spotwelding technique.
```

---
## \#629 Posted by: Prism Posted at: 2018-12-09T22:18:01.441Z Reads: 191

```
![20181209_231022|690x388](upload://AkB3YwbXQmF2AGSRA2tkpuyMXk4.jpeg) 

What a sad day. :frowning_face:

But at least I could confirm that my welds were nice and strong. It took quite a bit of force to pull the nickel strip away from the contacts.
```

---
## \#630 Posted by: JTAG Posted at: 2018-12-09T22:25:46.473Z Reads: 187

```
Aaaawh, poor battery :frowning: . Good look in repearing and making it that good looking again....

We have used nkon many times, we ordered 100s of cells and never had issues. I hope you discover why it happend.
```

---
## \#631 Posted by: Prism Posted at: 2018-12-09T22:30:22.680Z Reads: 187

```
I'm gonna let the cells sit like that till tomorrow and check the voltage again.
That way I'll know if it's the p-groups themselves or if the problem was my series connections.
```

---
## \#632 Posted by: Eretron Posted at: 2018-12-09T22:42:53.490Z Reads: 187

```
I'm still waiting for DieBie to arrive, I would like to make button free board, so my idea is to make it only push to start...

Is there anything I should know that's gonna bother me once I try to make it happen?

It will be used with flipsky dual 6 esc and metr 

Thanks
```

---
## \#633 Posted by: Prism Posted at: 2018-12-10T01:22:25.772Z Reads: 187

```
Well, you'd have no way to manually turn off your board. 
The only thing turning off your board would be the timeout in the bms. If that doesn't bother you I don't see a problem.
```

---
## \#634 Posted by: Surfer Posted at: 2018-12-10T07:28:35.561Z Reads: 194

```
I can recommend this pliers with the idea of taking apart you pack, you will destroy them, but you will have the pack done in no time, if you don't have that one buy 2, it's really handy tool to have.
Btw In Ali is quite cheap
![_SR300%2C300|300x300](upload://ujzf3rstWA5DsxiHW26RY0sIWOp.jpeg)
```

---
## \#635 Posted by: chocol4te Posted at: 2018-12-10T20:57:05.253Z Reads: 193

```
Finally had time to do more work, now when I turn it on, I get ERROR PRECHARGE on the display. I'm looking through the code, but do you have any ideas as to what could cause it? Should I be able to connect over serial when it displays "bye"? That is the only time the serial port appears on my system.
```

---
## \#636 Posted by: JTAG Posted at: 2018-12-10T21:34:36.047Z Reads: 195

```
In any state you will be able to connect and communicate with the BMS trough USB. Can you try the following:

* Reflash the firmware to the latest (this resets the default config to something known).
* Disconnect the load
* Change the cell configuration to match your pack (wrong cellcount can lead to this precharge error because it is not expecting the minimal voltage withing a reasonable time), make sure to write and store the config.

And retry to enable. You can also do this by hitting reboot in the BMS tool.
```

---
## \#637 Posted by: chocol4te Posted at: 2018-12-11T19:04:27.325Z Reads: 197

```
I still cannot connect over serial. I have now built the firmware myself and manually changed the default config in the source, and flashed it. Now I get an empty battery image, and holding the power button does not turn it off. It does power off if I remove the the ground lead and leave the balance connector and positive cable connected.

Connecting and disconnecting load has no effect.

CAN forwarding does not work, giving the same error as serial.
```

---
## \#638 Posted by: Prism Posted at: 2018-12-12T18:35:45.987Z Reads: 205

```
I found my two offending cells. 

![20181212_185139-1|690x199](upload://9z3v5X7CN7ZDt3krNEEbCBXTpR5.jpeg)  
as you can see, C6.2 and C4.1 are slowly dropping in voltage while the rest stays at the same level.
 
![20181212_192459|690x388](upload://95spsNs3KrZn2aBIZoAso66h91k.jpeg) 
curren status of my pack (sad)

I'm not looking forward to removing the leftover pieces from spotwelding from the good cells.
```

---
## \#639 Posted by: chocol4te Posted at: 2018-12-12T18:39:28.156Z Reads: 196

```
Update:
Connecting to the serial port with an external USB-serial adapter gives a different error: "The firmware on the connected DieBieMS is too old. Please update it using a programmer.". But since I *just* built from master that seems unlikely.
```

---
## \#640 Posted by: Prism Posted at: 2018-12-12T18:52:18.892Z Reads: 200

```
I'm no expert, but did you check if you can see the bms in your device manager when connected to your pc?
It should look something like this:

https://puu.sh/CgAGO/f5c22ad52c.png

if not, download the driver from the silicon labs website, install it and try again. 
I got the “The firmware on the connected DieBieMS is too old. Please update it using a programmer.” error on a windows 7 laptop. Manually downloading and installing the driver fixed it for me.
```

---
## \#641 Posted by: JTAG Posted at: 2018-12-12T19:44:41.266Z Reads: 196

```
LOOK! That is progress! 

That means that it can read the firmware version. It also means that it didn't upgrade properly if you just did an upgrade. That could be because of a missing bootloader. Right after uploading the firmware it will jump to the bootloader and the LED should start blinking quickly. If the fast blink doesn't happen the bootloader is missing or your are at an extremely old version of the BMS firmware and should do the jump manually (described a long while back)
```

---
## \#642 Posted by: chocol4te Posted at: 2018-12-13T16:46:24.593Z Reads: 192

```
Hmm, after flashing the boot loader again I get fast blinking followed by slow blinking, then off, so I am pretty sure it is flashing correctly. Both the latest firmware in the diebiems-tool repository and the firmware I built give the same error "The firmware on the connected DieBieMS is too old. Please update it using a programmer.” over the external USB-serial connection. I'm trying to manually send 0x02, 0x01, 0x00, 0x00, 0x00, 0x03 over the serial port (This is the version request packet?) to see what is actually being sent back.
```

---
## \#643 Posted by: chocol4te Posted at: 2018-12-13T19:10:13.003Z Reads: 201

```
After flashing the boot loader I get the following displayed on the screen (with quick flashing lights followed by the DieBieMS splash screen and then "bye"):

```
Bootloader V0.1
Size...Error-wrong
ERROR!
```
```

---
## \#644 Posted by: JTAG Posted at: 2018-12-13T19:15:55.763Z Reads: 202

```
This is what is happening in the bootloader when you see this message:

yAxisOffset += 8;
libGraphicsSetCursor(0,yAxisOffset);
libGraphicsWrite('S');  
libGraphicsWrite('i');  
libGraphicsWrite('z');  
libGraphicsWrite('e'); 
libGraphicsWrite('.'); 
libGraphicsWrite('.'); 
libGraphicsWrite('.'); 			

if(newAppSize == 0)
	bootloaderStateNext = BOOT_SIZE_ZERO;
else if(newAppSize > NEW_APP_MAX_SIZE)
	bootloaderStateNext = BOOT_SIZE_WRONG;
else
	bootloaderStateNext = BOOT_SIZE_OK;

So the new firmware that is loaded is more than the max size, which is wierd and should never happen.
```

---
## \#645 Posted by: PXSS Posted at: 2018-12-16T06:16:58.871Z Reads: 192

```
@JTAG Any differences in HW between 0.7 and 0.9? I'm opening up my board and was planning to do updates if need be.
```

---
## \#646 Posted by: JTAG Posted at: 2018-12-16T12:50:21.800Z Reads: 196

```
You have a 0.7 PCB and want do do modifications to make it 0.9? Well I think that between these revisions there were only component changes to simplify the bom and I moved the PCB NTC a bit closer to the switching components, so nothing worth changing or patching!

PS. @chocol4te his problem seem to be resolved after an erase and rewrite of the firmware.
```

---
## \#647 Posted by: PXSS Posted at: 2018-12-16T14:16:04.401Z Reads: 197

```
Perfect. Then I'll just do a firmware upgrade.
For the push to start feature I just need to connect enable_CAN to the 5v_CAN correct?
```

---
## \#648 Posted by: JTAG Posted at: 2018-12-16T14:40:47.376Z Reads: 197

```
Yes that is correct!
```

---
## \#649 Posted by: mishrasubhransu Posted at: 2018-12-19T02:48:26.497Z Reads: 191

```
@JTAG,  I can safely use a 50.4 volts charger for charging a 10S battery, or should I go for 42V charger?
```

---
## \#651 Posted by: JTAG Posted at: 2018-12-19T10:56:03.840Z Reads: 201

```
Using a 50V charger on a 10S will work, no problem, just make sure to configure the correct soft and hard over voltages, but that should be done for every charger. 

The minimum charger voltage for 10S when configuring the max voltage to 4.2V is:
* (10*4.2+0.7)=42.7V for charging when the BMS is already on.
* (10*4.2+3)=45V when you want the BMS to turn on automatically when the BMS is of.

So 50V would do it as well.
```

---
## \#652 Posted by: mishrasubhransu Posted at: 2018-12-19T12:00:36.604Z Reads: 207

```
Perfect!  Thanks.

BTW, if anyone else is looking for a 50.4V 4A charger then here's [one](https://www.aliexpress.com/item/XINMORE-50V-4A-Battery-Charger-For-44-4V-lithium-Battery-Electric-bicycle-Power-Electric-Tool-for/32829835683.html) from aliexpress that I got for $20(when including seller's discount $2 and instant discount for using paypal $5). I just got one, so should work for you all too.
![image|487x487](upload://4vxqLbJ7xmIhCUpBG5Wcbes7Iy2.jpeg)
```

---
## \#653 Posted by: willumpie82 Posted at: 2018-12-19T14:46:42.029Z Reads: 208

```
( just deleted my (mis infomed) post ) 

How does the BMS handle the CV part of CC-CV? Hence how does DieBieMS create 42v (ish) from 50v, there is no charge voltage disipation or buck regulator on the board right?
Normally the "Constant Voltage" is limited by the charger (= max cell voltage * number of cells ).

![afbeelding|690x474](upload://ezjgoPFOoqJS4QOQ2jJf2r1RMe2.jpeg)
```

---
## \#654 Posted by: JTAG Posted at: 2018-12-19T15:03:03.615Z Reads: 204

```
No problem! Thanks for helping answering the questions, the community helping saves me al lot of time and helps me alot. I am currently hard at work on realising a new version of the firmware that can also test the cell connections (does a minimal impedance check of the balance wires) for production testing but also to verify whether all wires are still connected, this took and takes more time that I thought but will be finished soon.

The BMS does indeed not change the voltage, it just disconnects the charger from the battery when the highest cell voltage has reached the configured threshold. Therefore it is ok to have a charge with a higher open clamp voltage, the drawback of that is that you are not utilising the full power that a charger can deliver but that is not a problem.
```

---
## \#655 Posted by: mishrasubhransu Posted at: 2018-12-25T09:00:32.081Z Reads: 198

```
So i was going to follow your direction for running the **tool** on windows but i see that in the present commit the build folder is missing. Whats the best/easiest way to get this running? I have access to both **linux** and **windows** computer.
```

---
## \#656 Posted by: JTAG Posted at: 2018-12-25T10:32:30.880Z Reads: 194

```
You should go to releases nou on the BMS GitHub. I didn't knew that by tthen but that is the recommended way of releasing software.
```

---
## \#657 Posted by: mishrasubhransu Posted at: 2019-01-03T05:58:39.247Z Reads: 206

```
Solved now
with this
[quote="JTAG, post:415, topic:2639"]
Go to the terminal, make sure you are still connected and type bootloader_jump followed by Enter. The status LED on the BMS will now go from regular blinking to intermittent fast blinking
[/quote]

Before solution:
Connected the bms with 10S battery with 10Ah capacity. was able to connect to the diebieMS_tool(and also vesc-tool) using the terminal. However rest of gui doesn't work for me. no realtime data, can't read the present config etc.  It is charging though. The voltage across the charger has dropped to a bit above 38.42 Volts. Is that expected? 

Also why does the status say that the state of charge is 100% even though the pack voltage is 38.11 volts

-------    BMS Info   -------
Firmware: V0.16
Hardware: V0.3
Name    : DieBieMS
UUID: 31 00 24 00 04 57 34 57 30 39 36 20
------- End BMS Info  ------

---   BMS Configuration   ---
NoOfCells                  : 10
batteryCapacity            : 10.00Ah
cellHardUnderVoltage       : 2.300V
cellHardOverVoltage        : 4.400V
cellSoftUnderVoltage       : 2.500V
cellSoftOverVoltage        : 4.250V
cellBalanceStart           : 3.800V
cellBalanceDiffThreshold   : 0.010V
CAN ID                     : 10
--- End BMS Configuration ---

-----Battery Pack Status-----
Pack voltage          : 38.11V
Pack current          : 0.32A
State of charge       : 100.0%
Remaining capacity    : 10.00Ah
Operational state     : Charging
Load voltage          : 0.00V
Cell voltage high     : 3.829V
Cell voltage low      : 3.795V
Cell voltage average  : 3.810V
Cell voltage mismatch : 0.034V
Discharge enabled     : False
Charge enabled        : True
---End Battery Pack Status---

-----   Cell voltages   -----
Cell voltage 0             : 3.818V
Cell voltage 1             : 3.809V
Cell voltage 2             : 3.819V
Cell voltage 3             : 3.818V
Cell voltage 4             : 3.812V
Cell voltage 5             : 3.812V
Cell voltage 6             : 3.810V
Cell voltage 7             : 3.812V
Cell voltage 8             : 3.812V
Cell voltage 9             : 3.812V
Cell voltage high          : 3.819V
Cell voltage low           : 3.809V
Cell voltage average       : 3.813V
Cell voltage mismatch      : 0.010V
----- End Cell voltages -----
```

---
## \#658 Posted by: mishrasubhransu Posted at: 2019-01-03T08:04:27.034Z Reads: 179

```
Everything work but I have one last question(hopefully). How do I set the max charge current or something to that effect, so that my charger doesn't hit it's limit. All i could see was charge throttle settings. But from the description what I understand is that it controls the final charge current.
```

---
## \#659 Posted by: SkaterBoy58 Posted at: 2019-01-03T08:56:19.045Z Reads: 181

```
no control over charge current from the bms
the bms fires a charge mosfet that acts like a switch
current control needs to come from the cccv charger
```

---
## \#660 Posted by: mishrasubhransu Posted at: 2019-01-03T12:38:32.353Z Reads: 190

```
Gotcha. That's what I concluded. But having a max current(input & charge)could be a desirable feature for couple of reasons. 
1. Say you have a monster power supply, a max current can prevent high charge rates and hence prolong the battery life. 
2. Say you have a supply with a rated fuse(or ability) , you don't have exceed that current limit. 

The charge throttle is already implemented for end of charging, so I don't see how that's a lot of work. Am I getting something wrong?
```

---
## \#661 Posted by: Pmac Posted at: 2019-01-03T13:31:37.151Z Reads: 198

```
Hi @JTAG,

Can you please confirm if I get a charger of 53.4V or there abouts, will that be fine to use on a 10S and 12S battery using your BMS?  Or would it be preferable to have a 45V and 53.4V charger for each battery pack.

I can only ride one board at a time so a single charger is fine (if possible) and would mean i can get a better quality one and not skimp.

Cheers,
Patrick
```

---
## \#662 Posted by: Wraith Posted at: 2019-01-03T13:36:26.943Z Reads: 198

```
I also want to ask if this power supply would be fine for 10s![image|375x500](upload://h3pN5cf0wpoNnlA32XsKsdTevOs.jpeg) 
I used the potentiometer and measured DC output voltage and I can tune it anwhere from 38v to 50v. I’m thinking of setting it to 45v as @jtag does in order to enable bms power on from plugging in the charging cable but want to know if this power supply will not break the BMS.

I understand that as long as it can regulate a constant current while providing enough voltage(even over as diebiems has over voltage cutoff) then this should work for me?
```

---
## \#663 Posted by: JTAG Posted at: 2019-01-03T13:57:58.656Z Reads: 193

```
Yes will be fine.
```

---
## \#664 Posted by: JTAG Posted at: 2019-01-03T14:03:38.994Z Reads: 201

```
I think this is a constant voltage power supply (that doesn't limit the current, but just switches of on overload), but you can always try an see the current in the BMS tool, if it switches of than it is not a current limiting power supply and isn't suitable for battery charging.

The voltage of the charger should at least be 1V higher than the battery voltage when it is fully charged to charge the battery to full. 

If you also want to have the bms to turn on automatically you have to have a charge that provides a voltage that is at least 3V higher than the battery voltage when it is full.
```

---
## \#665 Posted by: Wraith Posted at: 2019-01-03T14:06:35.154Z Reads: 189

```
Thanks for the detailed response @jtag! What cc/cv can you recommend me in case the bms doesnt power on when I plug in the power supply?
```

---
## \#666 Posted by: JTAG Posted at: 2019-01-03T14:35:11.737Z Reads: 189

```
You can power it on manually with the power button, after that it will charge as well. You will just not have the convenience of it auto powering on.

Uhm well, cant point one out directly, I prefer the meanwell LED power supplies that have a configurable voltage / current, but there are many options out there.
```

---
## \#667 Posted by: mishrasubhransu Posted at: 2019-01-04T10:58:58.975Z Reads: 184

```
@JTAG,  I am not sure if you read my question above. It was directed at someone else, but you are THE person to answer it best. In short the question is:

If charge throttle is already implemented for end of charging scenario, why not use it for limiting input or charge current? Or is the throttling done not done fast enough to qualify as current limiting?

Advantage would be to improve battery life by restricting charge current. Secondly, one can use any charger(even the one that shuts down when current limit is hit)
```

---
## \#668 Posted by: JTAG Posted at: 2019-01-04T11:27:36.857Z Reads: 192

```
Yeas I read it bus was unable to respond to it yet :sweat_smile:, am hard work at work on more things than I can handle xD.

charge(and discharge) throttling is functionality that can be implemented to charge as fast as possible and discharge as long as possible. Because if you limit the currents at either the full and empty state you can do it longer (discharge it more and charge it longer). The BMS knows the cell voltages and therefore knows the worst case, it can however not control the charge / discharge current directly other than just stop it, so it emits a percentage on the can bus that can be used by the motor controller or the charger. This is used I a different application than a skateboard for a client of mine. In the future when I make a USB-PD adaptor this charge throttling will also be used to throttle charging. I hope in the future to implement it in the VESC code as well (to make the VESC throttle back instead of the battery cutting out and throwing you of the board), but the need is not high enough for me to make that a priority yet (I still have an enormous list of todo's of much awesomer things :stuck_out_tongue: ).

Edit: To answer your question, if your are able to implement the throttling in the charger than you should, however that rarely happens since you don't easily have acces to that in the chargers available (I implemented it in an external controller next to a meanwell charger that supports dimming).
```

---
## \#669 Posted by: Prism Posted at: 2019-01-04T22:31:02.100Z Reads: 193

```
my pack is back together. I also ordered some heat shrink for the pack with my new cells. 

![20181228_114412|690x388](upload://eCcho6IkFotq8DtSUkVURKVCe0M.jpeg)
```

---
## \#670 Posted by: mishrasubhransu Posted at: 2019-01-06T03:49:21.128Z Reads: 200

```
[quote="JTAG, post:668, topic:2639"]
so it emits a percentage on the can bus that can be used by the motor controller or the charger
[/quote]

Thanks for the detailed explanation. It's very interesting. I understand how that can be implemented on the charger(with CAN) side. 

so the bms can only control on or off when it's comes to charging, but if done fast enough does it just average out a certain value of current. Same way how the VESC produces a desired phase voltage?

**BTW:** 
I burnt my R36 resistor (for cell 1-5) somehow while I was working to connect canbus to vesc. Using a multimeter they read 5k, 11k, 2.9k , 1.8k, 112, 100, 100, 100, 100, 100, 100, 100.  Power tools touching balancing wires, copper dust,... i don't know what did it. diebiems tool just went crazy with the voltage readings for those cells. Looked through the schematics to locate what could cause the erroneous readings and a closer look(under microscope) showed **tiny brown marks** on those resistors :sob: 

![IMG_20190105_225508|666x500](upload://jQSjoNhIxFx4WdZb9JHmamqCh3h.jpeg) 
![image|690x306](upload://5GnwQTxjjSlCJvGxJ22dHWuQ4L9.png) 
![image|690x481](upload://1dynyS4rm5QKERr0DAAtlRRXEVK.png)
```

---
## \#671 Posted by: JTAG Posted at: 2019-01-06T15:30:16.800Z Reads: 189

```
Aaaawh nice one! Yes these resistors tend to go as described above somewhere (or I don't know exactly really where) when the main power leads are disconnected but when the load is connected and the load is enabled. Then part of the energy to the load is provided trough the balance leads into the BMS, this circuit is only ment for measuring and balancing to can't handle that current. I have rarely had this happen (compared to the amounts of succes), but all of the times it was due to either incorrect wiring of the balance wires or not / bad main power lead wiring.

On request by @Samau18 I added some new functionality to the BMS tool / firmware that is able to test these resistors. I will give an example in a sec.
```

---
## \#672 Posted by: mishrasubhransu Posted at: 2019-01-06T21:40:50.269Z Reads: 188

```
[quote="JTAG, post:671, topic:2639"]
when the main power leads are disconnected but when the load is connected and the load is enabled
[/quote]

OMG. That is exactly what happened. I am using a case for the bms and the assembly procedure makes you disconnect the power first and then the balancing port. At some point I connected the usb to see the cell readings and that when it started the bms without the main battery leads connected. Somehow it needs to be made fool proof, either in software or hardware. I think it can be fixed in software because, I burned 5 of those resistors. 5 is the number of discharge resistors active at a time. 

I don't know the exact pathway of the current but 2 of  the discharge mosfets got destroyed too(they were on even when the bms was off). I finally have everything working again by using ghetto jumper wire replacing the defective visas and transplanting the discharging mosfets from cell 11 & 12 to 1 and 2.
```

---
## \#673 Posted by: Arek Posted at: 2019-01-08T22:24:57.410Z Reads: 180

```
Let's say I have your BMS, is there a way to increase the current handling?
I need 160A continous and 240A burst.
What's the limiting factor, is it the thermals?
Adding some cooling would give me more current?
Or I need to biggyback solder secondary mosfets?
```

---
## \#674 Posted by: AlexBE Posted at: 2019-01-09T01:36:14.320Z Reads: 179

```
What on earth do you need 160A continuous for? I would love to see that build. Seriously though, at those currents, I would just bypass the BMS and use it for charge only.
```

---
## \#675 Posted by: JTAG Posted at: 2019-01-09T09:54:00.257Z Reads: 183

```
160A is not easy, and I am afraid you are indeed better off bypassing the bms. Maybe in the future ill design a smaller bms build in multiple layers that is a bit more modular but with a small footprint that is capable of carrying this type of current, but that will take a while I am afraid.
```

---
## \#676 Posted by: AlexBE Posted at: 2019-01-09T10:39:14.410Z Reads: 180

```
Alternately you could use an external contactor and drive that from the FET gates. This is what gokarts and evs do.
```

---
## \#677 Posted by: Arek Posted at: 2019-01-09T10:50:31.074Z Reads: 181

```
Yeah I was also thinking about external MOSFETs.
I can't just bypass it, I need the battery protection :stuck_out_tongue:
Maybe it's not like 160A all the time but maximum continuous when for example going uphill full speed.
```

---
## \#678 Posted by: AlexBE Posted at: 2019-01-09T11:32:52.250Z Reads: 182

```
Maximum continuous is not a thing. What battery do you have, work back from that. If your battery can't do 160A continuous you don't need the BMS to do it.
```

---
## \#679 Posted by: rene Posted at: 2019-01-09T12:47:39.152Z Reads: 183

```
Well 160amps continous battery usage on a skateboard with dual motors I would strongly doubt.


[Test drive 15% steep Hamburg](https://metr.at/r/OnBan)

That ride is uphill in hamburg the steepest street we got. But it was a cold and wet day - so I did not rush uphill. Between the cars.
```

---
## \#680 Posted by: Arek Posted at: 2019-01-09T13:55:30.245Z Reads: 188

```
I only know I'll use Samsung 30Q or ncr18650ga, how many in parallel I don't know, because I start with the motor and then workout the battery.
So you're saying I'll never exceed the ratings of diebiems in a real world use?
I chose 2x SK8 6374 192kv from hobbyking and focbox unity.
```

---
## \#681 Posted by: Giga Posted at: 2019-01-09T14:25:32.207Z Reads: 187

```
[quote="Arek, post:680, topic:2639"]
I chose 2x SK8 6374 192kv from hobbyking and focbox unity.
[/quote]
Then you will never exceed the ratings :smiley:

Maybe if you try pulling your car uphill, but before you will overload the BMS your 6374 will just burn with 60A cont.
```

---
## \#682 Posted by: Arek Posted at: 2019-01-09T16:08:01.193Z Reads: 187

```
What if I put some ferroliquid between the stator and rotor and get extra cooling and so be able to push much more? :smile:
```

---
## \#683 Posted by: Giga Posted at: 2019-01-09T16:43:15.954Z Reads: 183

```
Sure go on. Same result. Ferrofluid will only work for RPMs <<1000, otherwise your fluid is elsewhere and your motor will still overheat. Never wondered why it only works for direct drive hub motors at bikes? Doesnt work for geared hub or mid drive systems exactly because of this...
```

---
## \#684 Posted by: rene Posted at: 2019-01-09T18:12:20.961Z Reads: 186

```
My Setup is 12s10p of 20700B fine with 15A each == 150A easy possible battery amps.

My Motor max ams are set to 120A each.

Never reached my battery max.
```

---
## \#685 Posted by: Arek Posted at: 2019-01-09T18:58:07.275Z Reads: 180

```
So you have like 5kg just in cells xD
OK OK OK I will run currents that DieBieMS offers and see if I actually need more.
So now just wait for 4th batch of these...

[mishrasubhransu](https://www.electric-skateboard.builders/u/mishrasubhransu) It's not end of the world, you should be able to replace these resistors.
```

---
## \#686 Posted by: rene Posted at: 2019-01-09T18:59:41.669Z Reads: 180

```
The battery box weight is 10,4kg incl. Pelican Box. 
Somewhere you find a picture in this thread.
```

---
## \#687 Posted by: Arek Posted at: 2019-01-09T19:03:53.287Z Reads: 190

```
Ohh right these are not standard 18650, that makes sense.
What's the advantage of these Sanyo 20700B?

[JTAG](https://www.electric-skateboard.builders/u/JTAG) I read above that regen charge(when braking with vesc) is not supported, is that correct?

Also if my battery pack goes low and diebiems shuts it down, will it be enabled again as the voltage rises due to no load and let me ride very slowly few more kilometers?

Any idea when it will be available back again for purchase?
```

---
## \#688 Posted by: mishrasubhransu Posted at: 2019-01-09T21:43:50.195Z Reads: 190

```
Oh I replaced them, right away. I even mention that. I also destroyed mosfet and one discharge resistor. All replaced and everything's working fine.

My main concern was how to make it fool proof.
```

---
## \#689 Posted by: evoheyax Posted at: 2019-01-12T21:53:22.726Z Reads: 188

```
Has anyone been given a "error percentage"?

Just finally connected everything for the first time, but this is what I get... I pre configured it via the tool for 12s... I don't understand

Edit: So I looked into it some more... It appears that the settings are getting set back to default every time it's turned off. If I save and disconnect and reconnect, then read, the settings are in tacked... Any ideas?
```

---
## \#690 Posted by: evoheyax Posted at: 2019-01-12T22:12:25.054Z Reads: 179

```
I updated the firmware, but no luck with that. I'm guessing the error is due to the wrong cell count.
```

---
## \#691 Posted by: bevilacqua Posted at: 2019-01-12T22:13:01.754Z Reads: 179

```
You have to flash the memory of the BMS, look at the right side of the tool
```

---
## \#692 Posted by: evoheyax Posted at: 2019-01-12T22:20:23.929Z Reads: 178

```
Ah perfect!

But now now it shows an empty battery... Is there something else I could b missing in settings?

It show 3.7ish for every cell in the realtime data tab and voltages look good.
```

---
## \#693 Posted by: bevilacqua Posted at: 2019-01-12T22:22:23.789Z Reads: 183

```
Maybe check the balance connector?
```

---
## \#694 Posted by: evoheyax Posted at: 2019-01-12T22:25:41.112Z Reads: 182

```
Balance connector looks good. Like I said, voltages are showing up normal for every cell in the diebiems tool.
```

---
## \#695 Posted by: evoheyax Posted at: 2019-01-12T22:33:18.436Z Reads: 189

```
![image|690x355](upload://ivaw8JDAb8PMTAb73XhVDPdMTBV.png)

![image|375x500](upload://yIJjuq5p4dyfeoK8IZvUBM38F82.jpeg)
```

---
## \#696 Posted by: bevilacqua Posted at: 2019-01-12T22:37:08.337Z Reads: 180

```
Ahh now I get it, just use the battery normally and after 1/2 charges it will show the percentage bar
```

---
## \#697 Posted by: evoheyax Posted at: 2019-01-12T22:40:36.817Z Reads: 183

```
Ah, so it needs to be used charged before it'll show. Got it! Thanks!
```

---
## \#698 Posted by: evoheyax Posted at: 2019-01-12T23:41:34.482Z Reads: 188

```
So now the question is getting it to work with mtr pro. Currently, it shows me nothing.

Anyone know what settings need to be set? I selected "enable status over can" on the bms. I wired it as described above. I get temp data from the vesc, so it's connected. But I don't get anything for battery. Uart and correct baud rate are selected on focbox the module is plugged into. Also updated to the latest vesc firmware. What am I missing?

@rpasichnyk
```

---
## \#699 Posted by: rpasichnyk Posted at: 2019-01-13T09:33:07.551Z Reads: 182

```
Status over can is not needed. Did you check what CAN ID your BMS has?
```

---
## \#700 Posted by: evoheyax Posted at: 2019-01-13T16:08:56.485Z Reads: 183

```
It’s the default 10. I’m wondering if it needs the pos and neg for canbus to come from the same vesc as the module is plugged into.

There’s no special firmware for this either?
```

---
## \#701 Posted by: JTAG Posted at: 2019-01-14T02:20:12.624Z Reads: 184

```
You need to connect all CANH's and CANL's together of the bms and the two vescs for the communication. To power the isolated CAN transceiver you should also connect the power of it, that is the ground and 5V that are on the same connector as the CAN of the BMS. You connect it to either one of the ESC's doesn't matter which.
```

---
## \#702 Posted by: evoheyax Posted at: 2019-01-14T03:43:53.090Z Reads: 184

```
hmm... This is exactly how I have it wired. Assuming the diagram that you verified above as correct is correct. I have the pin 1 and 2 together, connected to 5v from the one of the focbox's can. And pin 5 connected to gnd on the same focbox's can. This is focbox id 3, which also has the remote's receiver. The metr pro is plugged into focbox id 2. 1 and 4 have no accessories and just can L and can H are connected to the rest of the cans L and H (both bms and all 4 focbox's).
```

---
## \#703 Posted by: JTAG Posted at: 2019-01-14T03:47:58.151Z Reads: 188

```
Then it should work....

Your VESC's are already (and still) working together right? 

For the config of the BMS is for CAN ID style still VESCStyle selected?
```

---
## \#704 Posted by: evoheyax Posted at: 2019-01-14T03:48:58.192Z Reads: 182

```
Let me prod that real quick and see, but I believe yes. I know have send status over can enabled on the bms.
```

---
## \#705 Posted by: evoheyax Posted at: 2019-01-14T04:10:34.091Z Reads: 186

```
I can communicate to all of the other 3 vesc's via canbus in the vesc tool from 1 vesc. So it seems canbus is working for them. It also turns on the bms when I turn on the VESCs (I have the vesc's and bms in parallel so I can discharge 200 amps).

Yes, Can ID is set to VESCStyle, and also id is 10. I disabled the "send status over can", and restarted afterwards. Nothing. Just shows 0 for voltage on the metr pro app.

I'm using FW 3.40 no limits.
```

---
## \#706 Posted by: JTAG Posted at: 2019-01-14T04:27:17.542Z Reads: 187

```
Could you connect your PC to a vesc usb and open the BMS tool, set can forward Id to 10 enable can forward and try to connect ( so trough a vesc over usb over can to the BMS)?
```

---
## \#707 Posted by: evoheyax Posted at: 2019-01-14T06:10:09.615Z Reads: 190

```
Does not connect... Pretty sure I had the connections right, especially since the focbox has the pins labeled on the outside.
```

---
## \#708 Posted by: evoheyax Posted at: 2019-01-14T06:18:53.043Z Reads: 195

```
Just double checked and the wiring is correct.

![image|375x500](upload://5xFbd4DxUHI9fb438APlT8wMBvy.jpeg) 

A little hard to see but pin. 1 and 2 are connected to the red wire, which is can pos on the focbox.

Pin 3 starts out yellow and turns black, which is can L.

Pin 4 starts out green, turns yellow, which is can H.

Also, just measured the voltage and sure enough, there is 5.1v across the can lines from the focbox to the the bms.
```

---
## \#709 Posted by: evoheyax Posted at: 2019-01-14T06:52:24.786Z Reads: 183

```
Also, Strangely enough, one of my canbus ports on one of my focbox's just stopped working. Everything is wired correctly, I don't understand.
```

---
## \#710 Posted by: JTAG Posted at: 2019-01-14T11:49:00.079Z Reads: 187

```
All looks ok.... 
 
I just see that you have 4 ESC's, it might be that the can bus load is to high for the BMS to keep up with it all (will look into can bus filtering at one point). 

You could try to lower the can status rate to 20 Hz on all vesc's and try again.
```

---
## \#711 Posted by: DooMMasteR Posted at: 2019-01-14T15:28:37.595Z Reads: 185

```
This project ist very nice but 12S is too small…
The LTC6813 would be great, I am bound to 16S so the small 12 channel brothers does not work for me, but maybe some parts of this could be reused/expanded…
```

---
## \#712 Posted by: MrEpiquad Posted at: 2019-01-14T15:34:43.165Z Reads: 190

```
@DooMMasteR  You might need some more patience than as the LTC6813 just been released and will not be available for another 6 months. 

![image|690x454](upload://18HQXqogIBM3K7WkGLv4NBoFGqd.png)
```

---
## \#713 Posted by: JTAG Posted at: 2019-01-14T15:40:35.034Z Reads: 184

```
But there are plans to support it!
```

---
## \#714 Posted by: evoheyax Posted at: 2019-01-14T16:50:52.713Z Reads: 181

```
Tried 20hz, and still nothing. I did solve my issue with one of my focbox's. It had a different canbus baud rate than the other 3.

Can you confirm the baud rate for can on the diebiems is 500k?
There's no settings for baud rate on the diebiems tool.
```

---
## \#715 Posted by: JTAG Posted at: 2019-01-14T17:05:20.431Z Reads: 182

```
Well it should be the same as the default of the vesc, can't Remember that I changed that. I'll check.
```

---
## \#716 Posted by: evoheyax Posted at: 2019-01-14T17:19:43.292Z Reads: 189

```
I also inspected the canbus port area to see if anything looks burnt or broken or improperly assembled. But everything looks perfect. 

![image|374x500](upload://6ddR9A2ojxqnjCRYvl51KoqD3Ev.jpeg)
```

---
## \#717 Posted by: deucesdown Posted at: 2019-01-14T17:33:44.972Z Reads: 183

```
have you tried with just 1 vesc? eliminate variables...
```

---
## \#718 Posted by: evoheyax Posted at: 2019-01-14T17:34:51.313Z Reads: 188

```
No, but I did disconnect 2 and bring it down to just 2 vesc's and it still didn't work.

What I'm wondering is if there's some terminal commands I could send to the bms to try and trouble shoot what's going on.

The default baud rate is 500k for the vesc. This would make the most sense and connection and hardware wise, everything looks correct.

Also couldn't find anything about baud rate in the mod can file. Best I could find is this:

> if(modCANGeneralConfigHandle->emitStatusOverCAN) {
		// Send status messages with interval
		if(modDelayTick1ms(&modCANSendStatusSimpleFastLastTisk,200))                        // 5 Hz
			modCANSendSimpleStatusFast();
		
		// Send status messages with interval
		if(modDelayTick1ms(&modCANSendStatusSimpleSlowLastTisk,500))                        // 10 Hz
			modCANSendSimpleStatusSlow();
}

But that seems more like the status rate than the baud rate.
```

---
## \#719 Posted by: evoheyax Posted at: 2019-01-16T19:18:37.411Z Reads: 183

```
So is there no hope then of getting the canbus to work on this bms?

I tried 1 vesc only, but that didn't work either. Has anyone else had this issue also?

@JTAG @bevilacqua
```

---
## \#720 Posted by: bevilacqua Posted at: 2019-01-16T19:52:50.237Z Reads: 185

```
actually I have... but I connected the can bus pins 5-1 instead of 1-5 reversing the polarity. So I thought it was because of my error

Even whough I changed the components in this pic, but I still get no signal :/ 

![image|690x467](upload://3T2Y9ODqKUn5wcVmABfCeNvPpOF.png)
```

---
## \#721 Posted by: evoheyax Posted at: 2019-01-16T19:57:57.877Z Reads: 188

```
I carefully looked at everything about the can port I could find. From the one diagram that JTAG confirmed was correct, it showed if you look at the can port from the side it is on, the pins increase from 1 to 5, left to right.

I know this is not an issue with @rpasichnyk's metr pro app, and with the bms as I can't connect to the vesc's or vice versa through can. Everything else about the bms seems to be working.

I'm just wondering if there's some commands I could run that could help trouble shoot this.
```

---
## \#722 Posted by: deucesdown Posted at: 2019-01-16T23:13:26.868Z Reads: 189

```
Have you tried in vesc tool in terminal "can_devs"?
```

---
## \#723 Posted by: evoheyax Posted at: 2019-01-17T02:50:14.315Z Reads: 191

```
No I can try that. Thanks.
```

---
## \#724 Posted by: deucesdown Posted at: 2019-01-17T03:30:12.480Z Reads: 192

```
I suppose if it was me I'd be looking at something to snoop on the canbus maybe something like this with a pi

https://www.amazon.com/HiLetgo-MCP2515-TJA1050-Receiver-Arduino/dp/B01D0WSEWU/
```

---
## \#725 Posted by: rpasichnyk Posted at: 2019-01-17T19:11:33.001Z Reads: 188

```
Swap CANH and CANL? Just a wild guess. I hope this doesn't burn anything😅
```

---
## \#726 Posted by: evoheyax Posted at: 2019-01-17T19:25:30.589Z Reads: 197

```
lol, ive done this before without doing any damage on some old chaka vescs. But i've checked this like 6 times now to make sure there's no chance they are mixed.
```

---
## \#727 Posted by: mishrasubhransu Posted at: 2019-01-19T12:13:40.571Z Reads: 198

```
Just showing how I have placed my DieBieMS with N.E.S.E modules. 
![IMG_20190119_064319|666x500](upload://zidwqtiz4f3WUI9klEnUmmrVz5r.jpeg)
https://www.electric-skateboard.builders/t/no-words-just-pictures-delete-words-use-pm/2992/9120?u=mishrasubhransu
```

---
## \#728 Posted by: willumpie82 Posted at: 2019-01-20T18:32:36.473Z Reads: 191

```
what is your cell config? and a bit of topic but where can we find the stl for these n.e.s.e modules ?
```

---
## \#729 Posted by: deucesdown Posted at: 2019-01-20T18:48:29.901Z Reads: 190

```
[quote="willumpie82, post:728, topic:2639"]
stl
[/quote]

http://18650.lt/index.php/resources/
```

---
## \#730 Posted by: mishrasubhransu Posted at: 2019-01-20T21:53:00.994Z Reads: 182

```
It's 10s4p. I'll post the link to my DieBieMS box soon and as an edit to this post.
```

---
## \#731 Posted by: Arek Posted at: 2019-01-20T23:54:12.647Z Reads: 186

```
NESE modules are cool but it would be even better if these would be designed to go outside, with no need for extra covers.
```

---
## \#732 Posted by: bevilacqua Posted at: 2019-01-21T12:51:08.059Z Reads: 185

```
You got the Stl files. Design something custom
```

---
## \#733 Posted by: Arek Posted at: 2019-01-21T14:00:53.915Z Reads: 184

```
I want but don't have enough inspiration :stuck_out_tongue:
```

---
## \#734 Posted by: willumpie82 Posted at: 2019-01-23T13:49:58.869Z Reads: 180

```
The idea is good but I see some limitations, 3D printed stuff is not waterproof, but design wise a small dimple around the perimeters of the lid an O-ring around the screws and a grommet filled with silicon glue should keep water and dirt out mostly (I expect you're not building a submarine board)
```

---
## \#735 Posted by: Arek Posted at: 2019-01-23T13:54:33.197Z Reads: 178

```
If print is of a decent quality and has at least 3 layer shell then there should be no leaks especially that I will print them at 100% infill.
Also as you said it's not a submarine, there will be only water splashes.
```

---
## \#736 Posted by: Wraith Posted at: 2019-01-23T14:45:42.206Z Reads: 175

```
I finally got the balance wires up and tried charging it for the first time. All I got was the version being displayed followed by the charging symbol and then it would shut off after. Not sure why its doing that if its not a misconfiguration on the tool on my part, could there be any other reason why it won’t charge?
```

---
## \#737 Posted by: mishrasubhransu Posted at: 2019-01-23T15:05:21.141Z Reads: 175

```
Hook it up to a computer and connect to DieBieMS too and see what it says.
```

---
## \#738 Posted by: Wraith Posted at: 2019-01-23T15:06:31.313Z Reads: 172

```
Did you mean on the display or from the terminal when connected?
```

---
## \#739 Posted by: mishrasubhransu Posted at: 2019-01-23T15:09:02.727Z Reads: 176

```
Real time data. Basically you have to configure the BMS and then save the settings. Then charge it. If your real time data is not showing see my post above. I had similar problem. On mobile so can't point you to the right section.
```

---
## \#740 Posted by: Hummie Posted at: 2019-01-24T06:42:18.988Z Reads: 176

```
It’s s long thread.  Is anyone getting these made now or in near future? Have one now?
```

---
## \#741 Posted by: Wraith Posted at: 2019-01-24T07:06:06.615Z Reads: 185

```
https://www.electric-skateboard.builders/t/diebiems-v0-8-batch-3/65313?u=wraith
This one is going on now
```

---
## \#742 Posted by: Wraith Posted at: 2019-01-24T09:32:57.892Z Reads: 183

```
Here's the live Data I'm getting
![image|690x423](upload://6x1SEifFi1MvGNnWqZNAmk91DbQ.png) 
Those are my settings. I just configured the Cell count and capacity for my pack. 10s6p 30Q.

still getting the battery charge sign then shut off when charging it while the BMS is switched off

![image|690x420](upload://1N6mL0xzEbHnCMqWQDSDaytYk75.png)
```

---
## \#743 Posted by: deucesdown Posted at: 2019-01-24T23:15:21.446Z Reads: 178

```
[quote="Wraith, post:742, topic:2639"]
when charging it while the BMS is switched off
[/quote]

does it charge when BMS is turned on?

I remember if you want to charge when BMS is off, you have to give it 3v more than pack voltage:

[quote="JTAG, post:664, topic:2639"]
The voltage of the charger should at least be 1V higher than the battery voltage when it is fully charged to charge the battery to full.

If you also want to have the bms to turn on automatically you have to have a charge that provides a voltage that is at least 3V higher than the battery voltage when it is full.
[/quote]
```

---
## \#744 Posted by: Wraith Posted at: 2019-01-24T23:36:27.327Z Reads: 178

```
When trying to charge while plugged in it just shows the empty battery sign which it also just shows when is on and not charging. I’ll need to double check the voltage
```

---
## \#745 Posted by: Wraith Posted at: 2019-01-26T11:43:00.578Z Reads: 177

```


![image|666x500](upload://1mdwWe7QlZYPr3Z7Aedupz4fzGs.jpeg) So I set the output voltage to the charge+ and common - to 45.3v as I understand you need at least .3v for diode and 3v for the auto charge feature

Is the blinking of the switch normal?

Is it also possible to view the current it is charging at?
```

---
## \#746 Posted by: mishrasubhransu Posted at: 2019-01-27T18:57:48.257Z Reads: 175

```
Blinking is normal when charging . So what did you do differently from before when it was getting turned off?
```

---
## \#747 Posted by: mishrasubhransu Posted at: 2019-01-27T19:01:33.946Z Reads: 173

```
What does the BMS do when it hits the soft low voltage? It seems like it is making the board stop immediately. Is that an intended behavior?

I would assume that when the board is in use it would continue supplying power but switch the board off once  the board is not moving. @JTAG, where can I find more information about this?
```

---
## \#749 Posted by: Mich21050 Posted at: 2019-01-27T20:17:54.604Z Reads: 175

```
http://prntscr.com/mcy27k
.....
@Arek
```

---
## \#751 Posted by: Mich21050 Posted at: 2019-01-27T20:24:52.742Z Reads: 173

```
As far as I know you only need to fill in the form.. :slight_smile:
```

---
## \#752 Posted by: Arek Posted at: 2019-01-27T20:25:59.717Z Reads: 174

```
What form, for what?
I asked this asian guy like 20 times if I can buy one, mostly doesn't reply or just say that there are production issues.
```

---
## \#753 Posted by: Mich21050 Posted at: 2019-01-27T20:28:13.140Z Reads: 175

```
https://www.electric-skateboard.builders/t/diebiems-v0-8-batch-3/65313?u=mich21050
It's literally on the first post...
```

---
## \#754 Posted by: Arek Posted at: 2019-01-27T20:29:14.143Z Reads: 170

```
I think I already filled it and nothing.
What's the deal with the question about handle??
```

---
## \#755 Posted by: Mich21050 Posted at: 2019-01-27T20:30:29.161Z Reads: 167

```
I think he refers to your user name.
```

---
## \#757 Posted by: mishrasubhransu Posted at: 2019-01-27T21:09:05.576Z Reads: 174

```
[quote="Arek, post:748, topic:2639"]
Asian selling these is gone
[/quote]

Dude, I don't know what your deal is but learn to be more respectful.

Also don't pollute the technical threads with useless memes(because otherwise people have to dig through a lot of irrelevant information) and please keep your questions to relevant threads. This thread is about the DieBieMS and not the group buy.
```

---
## \#758 Posted by: deucesdown Posted at: 2019-01-27T21:15:08.200Z Reads: 168

```
Seriously wtf? He has a name, and has helped dozens of us on the forum. I see nothing but perfect english. Go buy something else dude if you don't want to deal with some asian dude.
```

---
## \#759 Posted by: Wraith Posted at: 2019-01-27T22:26:12.582Z Reads: 176

```
Okay thanks for the help! I asked @Samau18 and he suggested I up the voltage to 45v and thats what did it! 

Its currently been balancing for a few hours now. I had to double check the balance leads in the 16p male connector again to make sure the cables had a solid connection. 

So far when charging or balancing the bms is within the 54-60C range in case that info helps anyone

I’m going to observe the balancing more later. Hopefully it balances out completely then
```

---
## \#760 Posted by: Wraith Posted at: 2019-01-29T12:54:41.276Z Reads: 179

```
Is it normal for balancing to take considerably longer than during the charging operation?
Mine has been balancing for a good 3hrs now at least and its crawling up the SoC but just wanted to ask if you guys have had similar experience with the Balancing portion of the charge.

This was 3hrs ago
![image|690x436](upload://z4x8XHF2m2yIbBGweoxDHfi6YXP.png) 

and this is the current Cell Bar Graph
![32%20PM|690x432](upload://tt1MoV8TfQS2EBPmf4bGG3WXaDy.png)

its a 10s6p 30Q pack. During charging it read I Pack at 2A which as I understand is the charge current if I'm not mistaken
```

---
## \#761 Posted by: mishrasubhransu Posted at: 2019-01-29T13:02:33.240Z Reads: 176

```
If you have a multimeter and are comfortable probing the voltage across the balance resistors, please see if there is a voltage drop for the cell that should be discharging. Also with everything disconnect measure the resistance of those resistors. 

I have had both the balance resistors and the mosfets fail on me leading to balancing not working. I fixed it by replacing them both. 

There is this thing with DieBieMS where if the balance connectors are connected and not the main battery supply and then you connect to the VESC, a large amount of current passes through the balance circuit frying it. @JTAG knows about it.
```

---
## \#762 Posted by: Wraith Posted at: 2019-01-29T13:10:15.527Z Reads: 173

```
Thanks for the advice though I'm unsure which balance resistors I need to check. I didn't know about that issue as well although so far I've never connected any load with only the balance connectors plugged in. Is there any way for me to visually check the balance resistors and mosfets?

I should also mention that I shorted my pack last night while fixing the balance cable arrangement. it happened for a split second on the series connection but I have yet to open up the P group next to where it shorted and have only done a voltage check which showed about the same voltage before the short happened
```

---
## \#763 Posted by: Wraith Posted at: 2019-01-29T13:49:53.879Z Reads: 170

```
I'm also interested to know what I Pack and P pack negative values mean? I understand it as it draining the blue highlighted cells but I could be wrong lol I switch it on and off and now its showing vastly different voltage values

![02%20PM|690x485](upload://eu6qLKTCLgZfXJaBLWwKNy1mAHt.png)
```

---
## \#764 Posted by: mishrasubhransu Posted at: 2019-01-29T14:00:40.685Z Reads: 174

```
[quote="Wraith, post:762, topic:2639"]
I should also mention that I shorted my pack last night while fixing the balance cable arrangement
[/quote]

Uh oh. Did you short it though the balance cable? Then for sure the mosfet/balance resistor/both are toast. 

The balance resistors are the big 15 ohms resistors on the same side of BMS as  the battery - . Can you take a good photo of the diebiems? Close up. 

If it's toast then you can send it to me(assuming you are in the USA) and I can fix them for you.
```

---
## \#765 Posted by: Wraith Posted at: 2019-01-29T14:13:09.059Z Reads: 187

```
![image|375x500](upload://y5tJl5LT31ytGIZOQzvYNc1qRPd.jpeg) Yeah one balance cable terminal came in contact with one series braid. 

![image|375x500](upload://zi5PMuWyrnYpRIsyZEbapBiMNby.jpeg) 

![image|375x500](upload://et0fXQ7p6jSBh5aLUWRp7vDC9PK.jpeg)

Removed rhe kapton tape I wrapped it with and from what I can tell, nothing seems burnt or anything but I’m not experienced in this area to be able to really tell
@mishrasubhransu
```

---
## \#766 Posted by: JTAG Posted at: 2019-01-29T21:57:00.754Z Reads: 186

```
During balancing the cell voltages look lower on the enabled cell discharging cells, this is normal because of the voltage drop.

During short intervals all resistors are turned off and the highest cell voltages are determined, they are drained in the next cycle, this continues until all cells voltages are matched within the defines threshold. 

Positive pack currents are charging currents, negative are discharging currents. All looks good as far as I can see. What are the cell voltages when you are not charging? What is the mismatch?

I am crazy busy for an efoil costumer to improve the firmware (for the BMS) to support many fun stuf like water detection that triggers a beeper (finnally supported!!!), adressable LEDS for state indication and other fun stuff. I will make an update / release soon! This is for a different pack but seamlessly works also for this BMS.
```

---
## \#767 Posted by: Wraith Posted at: 2019-01-29T22:01:21.293Z Reads: 179

```
Thanks for clarifying that! I’ll check the voltages again and let you know!

Also can’t wait to try the addressable LEDs and even the water detection!
```

---
## \#768 Posted by: mishrasubhransu Posted at: 2019-01-29T22:35:04.147Z Reads: 179

```
He has been charging for over 3 hours but his voltage mismatch is stuck above 0.045. Is that normal?

I was thinking that his balance discharge circuit is broken for a couple of cells.

How do you detect water? Moisture sensor?
```

---
## \#769 Posted by: JTAG Posted at: 2019-01-29T22:56:49.974Z Reads: 177

```
Balancing current is 250mA with 15 ohm and when this is the first time balancing at high resolution (as the LTC does) balancing kan take up many hours like 20 to 40 hours, since it only does 1Ah per 4 hours (when the pack is for example 9 to 12 Ah).
```

---
## \#770 Posted by: Wraith Posted at: 2019-01-30T00:00:40.192Z Reads: 176

```
my pack is 18Ah. yeah first time charging and balancing. so far i've been doing intervals of about 3-4 hours for the past 2 days or so and the total pack voltage and SoC has been steadily increasing. Based on what i've been able to read, C5 and C9 have been discharging for awhile but have yet to actually balance out with the rest. I'll double check when I'm able tonight or tom.
```

---
## \#771 Posted by: JTAG Posted at: 2019-01-30T06:47:23.233Z Reads: 181

```
Yep with 18Ah that takes a while the first time, it will however increase your range! 

Also no need to monitor it that close, it will eventually be matched, I rarely monitor the balancing since it so far always worked :nerd_face:.
```

---
## \#772 Posted by: Wraith Posted at: 2019-01-30T06:52:42.370Z Reads: 183

```
Alright I can try and let it charge completely first and get back to you!  If that doesnt help I can go about draining it and then charging it up again. I'm kind of tempted to leave it balancing as its expected to take that long but I don't know how big of a risk it will be as compared to leaving it charging lol

I can't wait to try it out on "full" charge! (I have it set to OVC 4.2v to be very conservative first)
```

---
## \#773 Posted by: JTAG Posted at: 2019-01-30T07:24:59.274Z Reads: 180

```
Haha well the idea of the BMS is that you don't have to worry 😅. But I understand that it a little scary at first ( I have that as well sometimes when I try new code :p .
```

---
## \#774 Posted by: Wraith Posted at: 2019-01-30T07:50:35.267Z Reads: 182

```
Yeah horror stories just linger at the back of my mind when I think about leaving it unattended while its plugged in lol but you're right about the idea of not having to worry about it :laughing:

Has there been any progress on diagnosing the problems with the Batch 3 PCBs for the Group Buy as well?
```

---
## \#775 Posted by: Esk8enginneer Posted at: 2019-01-31T19:09:01.488Z Reads: 171

```
Was this answered?  Wouldn't manually pushing the board charge the battery as go?
```

---
## \#776 Posted by: sayekim Posted at: 2019-01-31T19:58:47.154Z Reads: 179

```
Shouldn’t you know as you are the esk8engineer?
🤔

I don’t think it was answered. 

Rolling the board does not charge the battery. This only happens when regenerative braking is active. 

So yes I still don’t know if it will continue to drain the battery since you are now forcing the esc to stay on and therefore I’d say you are draining the battery. I suppose it isn’t enough to have an impact. 

I know from the meepo board it does drain the battery enough in this case but with that board it also powers an annoying beep when empty which might be why it does drain the battery enough to further deplete it. 
I personally ran into this problem which is why I raised this question. 
It continues to drain the battery and the beep was no longer heard after a while of kick pushing.
```

---
## \#777 Posted by: Esk8enginneer Posted at: 2019-01-31T20:09:52.333Z Reads: 175

```
Haha I guess my tag is a bit miss leading.  I am a Mechanical Engineer that works in the areospace industry.  I am way out of my league here and new to esk8.  I have however been involved with RC most of my life and that is were all my battery and soilding etc... Experience comes from.
```

---
## \#778 Posted by: Esk8enginneer Posted at: 2019-01-31T21:46:03.444Z Reads: 183

```
@JTAG
There was a question about removing the switch back on post 346 by @sayekim that I do not think was ever answered about how would you turn the board off if you need to manually kick homedue to you battery being to low if the switch was no longer supported and the kick to start was enabled.  Could you please address it.  Thanks for everything you have done on this project.
```

---
## \#779 Posted by: mishrasubhransu Posted at: 2019-02-05T23:07:53.049Z Reads: 184

```
@JTAG, So when I am hitting the soft undervoltage, the VESC is  restarted and the board stops suddenly. It usually happens at low speed so I just hop off. I am a bit scared to ride when low on battery now. I'll program a low undervoltage(like 3.1volts) so that vesc will hit the low voltage and slow down first. 

**Q1:** Is that an expected behavior? 

Digging through the firmware I found the relevant variables. 
float **cellLCSoftUnderVoltage**; // If the lowest cell is under this voltage -> disable low current load
float **cellHCSoftUnderVoltage**; // If the lowest cell is under this voltage -> disable high current load

**Q2:** So what does the **low current load**  and **high current load** mean?
```

---
## \#780 Posted by: evoheyax Posted at: 2019-02-06T01:05:48.047Z Reads: 196

```
[quote="willumpie82, post:564, topic:2639"]
**the CAN connection:**
VESC1 | VESC2 | BMS
canH | canH | canH
canL | canL | canL
– | 5v | 5v CAN
– | 5v | Enable Can (&lt;-- connect to 5v for push2Start)
GND | GND | GND

5v_CAN is mandatory to power the primary can circuit on the dbMS
Enable_Can is optional connected to 5v_VESC for push2Start

pinout of the dbms

[![image|690x260](https://www.electric-skateboard.builders/uploads/db1493/optimized/3X/e/4/e4e74e91c382c4b2f37cc53bb2f4f1985ff0a85d_1_690x260.jpeg)
image.jpg1242x469 86 KB
](https://www.electric-skateboard.builders/uploads/db1493/original/3X/e/4/e4e74e91c382c4b2f37cc53bb2f4f1985ff0a85d.jpeg)
[/quote]

So I picked up another one from hummie who picked it up from someone on here. This time, I wired up just 1 vesc so I can test the functionality with a little complication as possible.

As before, push to start works but I can not see any other vescs when I run "can_devs" on the focbox, and the same from the bms. I tried both CAN ports. Neither worked.

Other then the wiring, what needs to be done on the bms and on the vesc to make this work?
Just seems odd to me that this is my 3rd diebiems and I can't get this essential feature to work.

Here is what I believe is correct, can I have someone confirm this diagram? @JTAG @Samau18

![bmsvesc|690x293](upload://bsHlecWd9b7YeqGvUEcqhBu1HtO.png)
```

---
## \#781 Posted by: mishrasubhransu Posted at: 2019-02-06T02:53:18.822Z Reads: 179

```
This is correct. I have wired it like that.
```

---
## \#782 Posted by: mishrasubhransu Posted at: 2019-02-06T02:53:59.279Z Reads: 182

```
[quote="evoheyax, post:780, topic:2639"]
I run “can_devs” on the focbox, and the same from the bms
[/quote]


Where do you run this? Terminal?
```

---
## \#783 Posted by: Samau18 Posted at: 2019-02-06T03:01:48.151Z Reads: 182

```
May be some thing basic, did you set the CAN ID right? 10 for dbms, I think 0,1 for VESC.
```

---
## \#784 Posted by: Samau18 Posted at: 2019-02-06T03:12:19.025Z Reads: 180

```
Still chasing Danny for feedback.  But still have time as CNY holidays still happening.

Sam
```

---
## \#785 Posted by: Samau18 Posted at: 2019-02-06T03:17:52.755Z Reads: 178

```
Also if you have two vesc, are you able to talk between the two vesc.?
```

---
## \#786 Posted by: mishrasubhransu Posted at: 2019-02-06T03:42:07.252Z Reads: 179

```
how does one talk to the devices on can bus? through vesc terminal?
```

---
## \#787 Posted by: evoheyax Posted at: 2019-02-06T04:32:05.183Z Reads: 178

```
[quote="Samau18, post:783, topic:2639"]
did you set the CAN ID right? 10 for dbms, I think 0,1 for VESC.
[/quote]

yes, and yes. I can communicate between 2 vescs but not to the bms.
```

---
## \#788 Posted by: Samau18 Posted at: 2019-02-06T06:15:35.220Z Reads: 181

```
Yes type ID of the destination device and connect
```

---
## \#789 Posted by: Samau18 Posted at: 2019-02-06T06:16:30.811Z Reads: 186

```
What’s the operation mode of the bms?  Is it passing load voltage to the vesc?
```

---
## \#790 Posted by: JTAG Posted at: 2019-02-06T14:34:15.306Z Reads: 197

```
Q1 -> The BMS wil disable the output if the lowest cell voltage drops below **cellLCSoftUnderVoltage** this is intended to protect the battery, at some point you should stop discharging the battery to protect it. This is indeed an instant cutoff, when in your case when the load is removed the cell voltages will recover to a higher voltage restoring the output enabled state to enable. If you do not want a sudden shut off you should limit the consumption of energy when the battery is almost empty, there is already al solution for that:
![image|690x377](upload://82q0nLoVhxs87ubry9E5DPo84sE.png) 

You should configure the VESC to cut off sooner than the BMS. In the future I will discuss with benjamin an option to communicate with the BMS to do this all automatically.

Q2 -> This is for a different BMS, the BMS used here only has a low current path and only uses the low current config. The high amp shield will use the high current load config to determine the relay or solid state relay enabled state.
```

---
## \#791 Posted by: evoheyax Posted at: 2019-02-12T03:08:53.852Z Reads: 186

```
[quote="Samau18, post:789, topic:2639, full:true"]
What’s the operation mode of the bms? Is it passing load voltage to the vesc?
[/quote]

No, I do not power the vesc with the bms. The bms is in paralell with the vesc. Does the bms need to power the vesc in order for canbus to work properly?
```

---
## \#792 Posted by: Samau18 Posted at: 2019-02-12T03:26:19.335Z Reads: 179

```
No, I just want to make sure the VESC is powered up.
```

---
## \#793 Posted by: Samau18 Posted at: 2019-02-12T03:31:38.878Z Reads: 177

```
I have a unity focbox, I will try to wire one up and takes some pictures.
```

---
## \#794 Posted by: evoheyax Posted at: 2019-02-12T03:43:11.175Z Reads: 176

```
ok, I rewired everything and still can't it to fire up. I feel like theirs some setting I'm missing or something simple.
```

---
## \#795 Posted by: Samau18 Posted at: 2019-02-12T03:44:15.529Z Reads: 173

```
Can you independently usb into both of them?  If so, it is likely the CAN bus wiring.
```

---
## \#796 Posted by: evoheyax Posted at: 2019-02-12T05:27:21.530Z Reads: 186

```
Yes. USB to each one works, I can change their settings using the correct tools. I wired the canbus as I posted above, like 10 posts up.

@JTAG one thing that would be nice right now is a status light for the canbus. Since it seems the vesc powers the canbus on the bms, it would be nice to see the canbus is getting power and it’s actually communicating (blinking light when writing/reading data). I dont know what else to do to fix it. I sent the 2 broken ones to you. But it’s odd with another fresh bms, I still can’t get it to work.

Edit: just double checked and it is 100% correct.
```

---
## \#797 Posted by: Samau18 Posted at: 2019-02-12T06:05:19.034Z Reads: 183

```
Just tested, working on unity with diebiems.  

A note, since the two tools are not directly compatibile with one another.  You will need to use vesc-tool on diebiems when you can forward from the bms usb terminal and diebiems tool on vesc-tool when you are on the vesc side.  I will post a video to illustrate this.
```

---
## \#798 Posted by: Samau18 Posted at: 2019-02-12T06:08:05.706Z Reads: 186

```
https://youtu.be/8iI7OIZlpFo
```

---
## \#799 Posted by: evoheyax Posted at: 2019-02-12T06:19:56.819Z Reads: 181

```
Why not just go to can forward tab and forward that way?

It’s hard to tell in the video, what command did you run?
```

---
## \#800 Posted by: Samau18 Posted at: 2019-02-12T06:29:17.174Z Reads: 179

```
Nothing special,  Just sent the proper ID for the target CAN device, (make sure the tool is matching the end device). 

I was trying to do a clear screen first. .but keep getting chinese text.. But just typed help at the end to show that it is listening.
```

---
## \#801 Posted by: evoheyax Posted at: 2019-02-12T22:49:09.480Z Reads: 180

```
Here's what I get with bms ---usb---> computer ---> vesc tool:

![on%20bms%20to%20vesc%20tool|690x332](upload://yMn73FNCia4oS52kWl0oR3svVKG.png)
```

---
## \#802 Posted by: Samau18 Posted at: 2019-02-13T00:44:34.837Z Reads: 180

```
Yes that’s likely a firmware and tool compatibility problem.   Try to run diebiems-tool, use vesc usb, set can id to 10, and reconnect.  Typing help in terminal should give you dbms functions.

Or 

run vesc-tool, use dbms usb, set can id to 0, and reconnect.   Typing help in terminal should give you vesc functions
```

---
## \#803 Posted by: evoheyax Posted at: 2019-02-13T01:04:11.415Z Reads: 179

```
The issue will be that the firmware on my vescs are 3.40 and the diebiems tool only accepts the 3.38 firmware. If there a newer diebiems tool?
```

---
## \#804 Posted by: evoheyax Posted at: 2019-02-13T01:05:08.981Z Reads: 181

```
I don’t see how the vesc tool would take the diebiems and connect, since it’s firmware is 0.21, not 3.39 or 3.40.
```

---
## \#805 Posted by: Samau18 Posted at: 2019-02-13T05:36:12.875Z Reads: 183

```
You should use the matching tool for the matching device.  

If you are connecting to diebiems, use usb on dbms to connect it with diebiems-tools or canbus on vesc with diebiems-tool.

If you are connecting to vesc, use usb with vesc to connect to vesc-tool and canbus on dbms with vesc-tool.
```

---
## \#806 Posted by: tricky-fpv Posted at: 2019-02-16T02:48:49.229Z Reads: 181

```
Hello all, 

I'm currently done with my battery and want to hook it up to the DieBieMS (hardware 0.8). I am finding it hard to understand the exact process of setting it all up so I'm going to summarise what I think needs to be done and hope someone can either confirm or correct my understanding.

Step 0. Install fuse (I think mine came with it pre-installed).
Step 1. Connect the balance wires. (c0 to c9 for a 10S pack?)
Step 2. Connect the battery pack to the BMS - and + terminals. 
Step 3. Connect the display and then the power button.
Step 4. Connect usb cable to bms and laptop and run DieBieMSTool.
Step 5. Update firmware and configure battery settings. 

Is this somewhat correct, or am I missing a step or am I wrong?
I've been scouring all posts about diebiems and the github for hours now and this is what I understand so far from all the loose bits of information here and there. 

Thanks so much!
```

---
## \#807 Posted by: Samau18 Posted at: 2019-02-16T09:21:24.009Z Reads: 179

```
Sounds about right, just make sure the battery goes to the pack +\- and vesc goes to load +\-.

Sam
```

---
## \#808 Posted by: Ckarg Posted at: 2019-02-19T05:18:10.633Z Reads: 188

```
So finally getting my two packs built, I go about starting to configure them.

One DieBieMS shows
-----Battery Pack Status-----
Pack voltage          : 42.06V
Pack current          : 0.01A
State of charge       : 0.2%
Remaining capacity    : 0.01Ah
Operational state     : Power down
Load voltage          : 0.00V
Cell voltage high     : 0.000V
Cell voltage low      : 0.000V
Cell voltage average  : 0.000V
Cell voltage mismatch : 0.000V
Discharge enabled     : False
Charge enabled        : False
---End Battery Pack Status---

The other plugged into the same pack shows
 
-----Battery Pack Status-----
Pack voltage          : 42.07V
Pack current          : 0.00A
State of charge       : 0.0%
Remaining capacity    : 0.00Ah
Operational state     : Power down
Load voltage          : 0.00V
Cell voltage high     : 3.514V
Cell voltage low      : 3.513V
Cell voltage average  : 3.513V
Cell voltage mismatch : 0.001V
Discharge enabled     : False
Charge enabled        : False
---End Battery Pack Status---

@JTAG @Samau18  Any ideas what have I done wrong that the one isn't reading cell voltages? I followed the above steps when connecting the DieBieMS's and this my first time doing anything with them since I got them. Same behavior regardless of which of the two 12s6p packs I connect to. Leading me to believing it is something with the one DieBieMS but I haven't a clue what it would be.
```

---
## \#809 Posted by: mishrasubhransu Posted at: 2019-02-19T05:23:57.853Z Reads: 182

```
Do you have a photo of the setup?
```

---
## \#810 Posted by: Ckarg Posted at: 2019-02-19T05:40:12.305Z Reads: 194

```
![20190218_223536|690x335](upload://eQ1X7jEroKyGQv2kZWU8Z7Yxd5g.jpeg) ![20190218_223550|690x335](upload://jhG0OaW00RaF249Z9RywGC97i2L.jpeg) ![20190218_223621|690x335](upload://l5rOA9WSeyBAKU2hb0kcbMiCQ89.jpeg) 

The one on the right is the one not reading cell voltage and it haven't matter which pack it is connected to.
```

---
## \#811 Posted by: mishrasubhransu Posted at: 2019-02-19T05:47:37.749Z Reads: 195

```
Disconnect the DieBieMS and could you check for the connectivity(using a multimeter) between the marked points? If connection doesn't exist that would definitely explain it. 

It is safe to do that. You won't short anything even if you tried. But make sure you disconnect the DieBieMS completely.
![93cb53e7a5ce625f4c68ed2b36f9e398bd16ef79|600x500](upload://fpja6rWrpbuJgaLXsEcrG745ciA.jpeg)
```

---
## \#812 Posted by: Ckarg Posted at: 2019-02-19T05:55:25.455Z Reads: 193

```
There is continuity, 0.2 ohms
```

---
## \#813 Posted by: Pimousse Posted at: 2019-02-19T08:00:20.241Z Reads: 198

```
@JTAG, @rpasichnyk, 
I was wondering...
How you'll manage the change in the new VESC FW about CAN ID calculation ? (Based on UUID IIRC) 
I mean, is there an automated way for letting Metr app to know the CAN ID of DieBieMS ?
```

---
## \#815 Posted by: rpasichnyk Posted at: 2019-02-19T17:45:39.116Z Reads: 196

```
I fail to see advantage of CAN id being calculated this way. This will lead to collisions. Questionable design choice. I suggest leaving DieBieMS CAN ID as it was before and do nothing.
```

---
## \#816 Posted by: mishrasubhransu Posted at: 2019-02-22T06:04:45.852Z Reads: 195

```
@Wraith wanted the modified NESE DieBieMS case, so posting here in case someone else finds it useful. Files here: https://www.thingiverse.com/thing:3444525
![DieBieMS_nonstandard2|690x353](upload://ktPQYEbHjpjamZyldzoeAZMEJ1L.jpeg) ![DieBieMS_nonstandard|476x500, 90%](upload://aEQVxv1Zu0DbSS5Nk7Naxp8f2Ce.jpeg)![IMG_20190119_064319|227x500](upload://ozvJwsY5rhzqtss0MjtdftA7rcy.jpeg)
```

---
## \#817 Posted by: Prism Posted at: 2019-02-23T16:48:48.367Z Reads: 193

```
Wish I knew this existed sooner. I just took the original NESE one and modified it by hand for my needs.

![20190205_175300|690x353](upload://cJaViA916Nw9siS9N29ACPc3aAP.jpeg)
```

---
## \#818 Posted by: PatRocks Posted at: 2019-02-26T08:44:45.917Z Reads: 191

```
To anyone that has struggled with the small crimp connectors (WR-MPC3), I just got a package of 50 for $10! Hit me up if you need some, and I'll just mail 'em to you! In the US, that would cost about a stamp ($0,43), but I'll put it on your tab, lol. And look!! I've learned the metric version of commas/decimals !!
```

---
## \#819 Posted by: Giga Posted at: 2019-02-28T20:45:03.157Z Reads: 196

```
Hi,
I got a strange issue on one of my DieBieMS 0.7 from the first GB. 

The battery is a 12S9P pack custom build and was connected properly. 

The first connection to the PC was made with just the battery (pack +/- and balancers including tempsensors) connected to the BMS and the USB cable (no switch, no display, no load etc...). 

After the USB plug in, the power led got solid green an the other one blinking. The connection with the DieBieTool 0.24 was successful, but I got a message that the software on the BMS was newer than the Tool. Which is strange since I never connected the BMS before and with the other BMS I got, it was the other way round and I had to do the bootloader_jump thing. 
Anyway the connection was established and it could read the firmware version. After that I disconnected the USB-cable and let the BMS connected to the battery sit there for a day.

Nothing touched it, it was not moved, nothing. 

The other day I connected the USB cable again and there is the sound of windows: "something was plugged in" and I can find the COM port, also the Tool states: "COM 3 DieBieMS". But when trying to connect it takes some seconds and tells me then "Can not read firmware version. blabla be sure the port belongs to DieBieMS". Also non of the LEDs is on/flashes, no matter how long the USB cable is plugged in. 

So thats the issue. 

Now what I already tried to troubleshoot: 
- check fuse
- check pack voltage (at BMS terminals)
- different USB cables
- different PCs
- disconnect everything (battery) and try again after a while (hoped for all caps to be empty by waiting some mins)
- trying Tool V0.25
- connect power switch and display and try power on by button (might not work because battery is 12S and BMS was never changed from standard config which I guess is 10S)
- measure the voltage on the 3.3V rail which is ~0V when only battery is connected and ~1.5V when connected to the USB and battery, button (dis)connected and/or pressed makes no difference
- and last but not least: connect via CAN forward with the DieBieTool over a VESC6 to Can ID 10 which leaded to the same "can not read firmware version..." message. 

After that I didn't got a clue what to try else. :worried: 

Any help is deeply appreciated!
```

---
## \#820 Posted by: JTAG Posted at: 2019-03-01T20:23:25.957Z Reads: 183

```
Wow well you started off good, but no response at all is a bit strange. 

When pack+ and pack- are connected to a supply of at least 12V at least the power supply LED should turn on when you connect the usb to a computer, independent of software or firmware. The USB to serial interface will always works since its usb powered and does not depend on the rest of the board. Could you check whether there is battery voltage between these pins? 

Image will be placed here soon
```

---
## \#821 Posted by: Giga Posted at: 2019-03-02T14:01:26.788Z Reads: 188

```
First of all, thank you very much for your quick reply! 

Now:
[quote="JTAG, post:820, topic:2639"]
Could you check whether there is battery voltage between these pins?
[/quote]
Sure, that was one of the things I checked first: 
[quote="Giga, post:819, topic:2639"]
check pack voltage (at BMS terminals)
[/quote]
43.9V, like I would expect from a 12S battery pack at storage voltage, same after fuse, so that should be fine as well.

[quote="JTAG, post:820, topic:2639"]
at least the power supply LED should turn on when you connect the usb to a computer, independent of software or firmware
[/quote]

Thats what I thought too. But the LED (and the 3.3V rail) only sees 1.5V when connected via USB, when disconnected 0V (no matter if the button is connected or pressed). 

What is the supply of the 3.3V rail? I had a quick look at the schematics and couldn't find a regulator. Is it done by the LTC chip? 

From my limited viewpoint my guess is that either the 3.3V rail/power supply is broken or the firmware got somehow corruped (so that the STM never awakes). 

Reflashing firmware from the debug port with a STlink-V2 should work in any case (given that the MCU itself is not dead), right?
```

---
## \#822 Posted by: JTAG Posted at: 2019-03-02T14:19:52.431Z Reads: 188

```
I was hoping that the uploading of pictures would be restored in a timely manner but unfortunately it isn't fixed yet. The picture I was planning to show showed different points then the main terminals, most importantly, there is an extra fuse on the BMS that isn't replaceable, if you follow the main PACK+ input there is another small trace that powers everything accept for the main output (main output is powered by the big fuse), the fuse is in that line. 

But you shared some useful information already, namely that the 3V3 is trying to power up but is for some reason not able, this means that the power management input circuit is still working and that it is trying to enable the power supply. The first thing you could try is doing a resistance measurement between the 3V3 rail and the GND (please use the outside of the USB connector as ground point). I did the same and I measure >50KOhms (when you measure in the order of mega ohms or kilo ohms the 3V3 rail and the connected devices are most likely OK if it is in the order of ohms something failed on it). If that is ok likely the power supply input is not ok and you should be able to follow the trace that goes above the main fuse from PACK+ to the power supply, you will find a 1206 fuse and a 150Ohm current limit resistor right next to it, please test that as well.
```

---
## \#823 Posted by: mishrasubhransu Posted at: 2019-03-05T11:45:34.779Z Reads: 188

```
Just showing how the Metr pro displays the DieBieMS data. 
 
![Screenshot_20190304-210600|281x500](upload://sq7aAmu3jsFjWJ5UGDI3oyzNA9J.png)
```

---
## \#824 Posted by: Sn4pz Posted at: 2019-03-05T13:11:17.680Z Reads: 180

```
What do the green droplets mean on packs 3 7 and 9?
```

---
## \#825 Posted by: mishrasubhransu Posted at: 2019-03-05T13:41:46.160Z Reads: 182

```
Discharging for balancing.
```

---
## \#826 Posted by: Giga Posted at: 2019-03-05T14:05:45.521Z Reads: 189

```
Again, thank you very much for your quick and helpful reply! 

I did the said measurements:
[quote="JTAG, post:822, topic:2639"]
The first thing you could try is doing a resistance measurement between the 3V3 rail and the GND (please use the outside of the USB connector as ground point). I did the same and I measure &gt;50KOhms
[/quote]

This is about 150kOhm. 

[quote="JTAG, post:822, topic:2639"]
you should be able to follow the trace that goes above the main fuse from PACK+ to the power supply, you will find a 1206 fuse and a 150Ohm current limit resistor right next to it, please test that as well.
[/quote]

Oddly the resistor R55 is 15 Ohm and the fuse F1 tripped. 

How may I proceed? Is just replacing the fuse safe? What could be the reason for the fuse to trip?
```

---
## \#827 Posted by: Sn4pz Posted at: 2019-03-05T14:11:20.491Z Reads: 183

```
I had thought that but I figured 0 2 and 6 would have the droplet too :P 

You changed your balancing point for the cells, is that hard to do? Ill be using a 12s7p 30q so I feel like its going to easy for one pack to drift... I want to be ontop of that batteries health... lol
```

---
## \#828 Posted by: mishrasubhransu Posted at: 2019-03-05T14:14:32.369Z Reads: 183

```
I have limited the max number of discharge resistors to 3  so you don't see all of them

Yeah, configuring the voltage when it starts balancing is very easy from the DieBieMS tool.
```

---
## \#829 Posted by: Sn4pz Posted at: 2019-03-05T14:16:06.377Z Reads: 180

```
[quote="mishrasubhransu, post:828, topic:2639"]
I have limited the max number of discharge resistors to 3 so you don’t see all of them
[/quote]

Is there any reason for this? Last question :)
```

---
## \#830 Posted by: mishrasubhransu Posted at: 2019-03-05T14:28:18.920Z Reads: 178

```
Rate of heat produced is less when you are discharging through fewer resistors.
```

---
## \#831 Posted by: Giga Posted at: 2019-03-11T16:51:03.857Z Reads: 175

```
[quote="Giga, post:826, topic:2639"]
Oddly the resistor R55 is 15 Ohm and the fuse F1 tripped.

How may I proceed? Is just replacing the fuse safe? What could be the reason for the fuse to trip?
[/quote]

@JTAG any suggestions?
```

---
## \#832 Posted by: Jarno Posted at: 2019-03-11T18:29:57.117Z Reads: 186

```
R55 is 15 Ohm according to the schematic![image|690x446](upload://gnPmYFaSy9Cfh6FqqocoWeADDFU.png) 

Go check if there's no short between J2 and J1, J3, J5, J4.

The next step is booting up the BMS with a labsupply with a limited current, if you don't have this you can use a resistor to limit the current (watch out for magic smoke from the resistor if there is a short).
```

---
## \#833 Posted by: mishrasubhransu Posted at: 2019-03-18T04:35:16.161Z Reads: 176

```
@JTAG, what would happen if a balance wire were to disconnect somehow. Would it disconnect the power or is there some kind of smart logic to detect this and not cut power until restarted?

Maybe it can be made into an option that can be enabled in the DieBieMS_tool to improve safety.
```

---
## \#834 Posted by: JTAG Posted at: 2019-03-18T07:01:00.911Z Reads: 177

```
Currently it stops the discharge because the BMS will see an extreme high and extreme low voltage. 

The LTC has a limited voltage range of about 5V, so it is unable to guess that the sum of the voltages is ok.

If you move the safety threshold as you suggest by this method the "safe" border gets blurred quickly :stuck_out_tongue:.
```

---
## \#835 Posted by: Pimousse Posted at: 2019-03-18T08:50:08.210Z Reads: 178

```
IIRC LTC application note mentions a way of detecting an open wire.
Don't remember the exact way though.
Could be interesting to have a dedicated fault code for open wire.
```

---
## \#836 Posted by: JTAG Posted at: 2019-03-18T09:13:59.605Z Reads: 178

```
Yes, I did a tribute to implement that for factory testing. Boils down to that it takes quite some time and cycles to detect and the result will be close to the same. 

To ease the pain, there is a "Yolo" / bypass mode you can allow to be enabled. When you are traveling and discover that the BMS is not allowing turn on because there is something wrong you can trigger Yolo mode by turning the BMS on by a long press, then the BMS will ignore the limits and safeties and just bypass and allow discharge ( and you to get home ). Be aware that this does also not protect against over discharge.
```

---
## \#837 Posted by: JTAG Posted at: 2019-03-26T17:51:47.214Z Reads: 174

```
@everyone, I am currently in San Fransisco and have some difficulties welding a battery. Does anybody know or have a spotwelder? Preferably one that can weld a big battery?


Edit: Not needed anymore! Thanks!
```

---
## \#838 Posted by: steve_f Posted at: 2019-03-28T08:22:11.231Z Reads: 177

```
Hi, got a problem I'm trying to work through.

I can't charge my battery, I think it's because it is failing to read my pack voltage, then erroring out - would that be true?

I have probed pin 1 (V+) on the LTC chip and it is correctly reading 29ish volts -- I assumed that this is where the pack voltage direct is read from?

    -----Battery Pack Status-----
    Pack voltage Direct   : 0.00V
    Pack voltage CVAverage: 28.48V
    Pack current          : 0.00A
    Low  current          : 0.00A
    High current          : 0.00A
    State of charge       : 0.0%
    Remaining capacity    : 0.00Ah
    Operational state     : Power down
    Load voltage          : 0.00V
    Cell voltage high     : 3.822V
    Cell voltage low      : 3.073V
    Cell voltage average  : 3.560V
    Cell voltage mismatch : 0.749V
    Discharge enabled     : False
    Charge enabled        : False
    Power button pressed  : False
    CAN safety state      : False
    ---End Battery Pack Status---

    ---   BMS Configuration   ---
    NoOfCells                  : 8
    batteryCapacity            : 3.50Ah
    cellHardUnderVoltage       : 2.300V
    cellHardOverVoltage        : 4.350V
    cellLCSoftUnderVoltage     : 2.700V
    cellSoftOverVoltage        : 4.200V
    cellBalanceStart           : 3.000V
    cellBalanceDiffThreshold   : 0.010V
    CAN ID                     : 10
    --- End BMS Configuration ---
```

---
## \#839 Posted by: Devilmycry Posted at: 2019-03-28T13:33:18.513Z Reads: 171

```
Hi how are you I send you a pm when you have a chance can you look at it thank you
```

---
## \#840 Posted by: ldemps Posted at: 2019-03-29T07:17:41.142Z Reads: 172

```
I think this is due to the ISL issue found in the group buy batch 3 thread (https://www.electric-skateboard.builders/t/diebiems-v0-8-batch-3/65313/338). Can someone confirm this? @JTAG?

If so, how can I roll back my firmware to a version that works - I can't really find any versioning anywhere. I found this one https://github.com/DieBieEngineering/DieBieMS-Tool/blob/master/res/firmwares/DieBieMS/DieBieMS_defaultOld.bin but it's fairly non-descriptive of what version it is and I'm scared to flash it. My Hardware is V0.9
```

---
## \#841 Posted by: JTAG Posted at: 2019-03-29T07:52:04.460Z Reads: 177

```
Hi all!

Yes this might be because of the smaller allowed voltage measurement difference (ISL issue vs my voltage margin) I allowed in my previous firmware version, I corrected this back, just today I released a new firmware version on github that should resolve this issue and bring it back to the original operation! If you have issues and you get the chance to install the new firmware please run in the terminal the command:

testbms 2 1 

and post the result here. Please mind that your main fuse should be installed and be OK.
```

---
## \#842 Posted by: mishrasubhransu Posted at: 2019-03-29T08:07:33.085Z Reads: 180

```
@JTAG, while you are here, I wanted to bring up another issue. 

When my battery is full(4.1Volts) and going on a flat road and I brake. The BMS switches off and then restarts. I understand that the cell voltage go beyond the max voltage and that triggers the shutdown, but a logic to detect something like this would be nice.

I guess I can increase the hard over voltage limit while keeping the soft over voltage at 4.1. Would that be your suggestion too?
```

---
## \#843 Posted by: JTAG Posted at: 2019-03-29T08:21:36.447Z Reads: 176

```
I would suggest to set the hard over Voltage to 4.35V. and if that still gives issues you pack might be to small of have a to high resistance for the amount of regen current. 

Good luck!
```

---
## \#844 Posted by: ldemps Posted at: 2019-03-31T11:32:45.422Z Reads: 187

```
Thanks for that @JTAG - you're a legend, charging and balancing is working now.

Here is my output: 

    ---------     Test inputs:     ---------
    Error threshold:   2.0V
    Balance threshold: 1mV
    ---  Starting voltage measure test  ---
    Pack voltage Direct   : 30.82V
    Pack voltage CVAverage: 30.81V
    Measure error         : 0.01V
    Result                : Pass
    ------  Starting connectionTest  ------
    [ 0] 2.946V - 3.619V = -0.673V -> Pass
    [ 1] 3.799V - 3.826V = -0.027V -> Pass
    [ 2] 3.831V - 3.829V =  0.002V -> Pass
    [ 3] 3.729V - 3.729V =  0.000V -> Pass
    [ 4] 4.110V - 4.107V =  0.003V -> Pass
    [ 5] 4.036V - 4.043V = -0.006V -> Pass
    [ 6] 3.842V - 3.839V =  0.003V -> Pass
    [ 7] 3.852V - 3.826V =  0.026V -> Pass
    ------    End connectionTest     ------
    ------    Start balance test     ------
    [ 0] 3.619V - 3.611V =  0.009V -> Pass
    [ 1] 3.825V - 3.836V =  0.010V -> Pass
    [ 2] 3.839V - 3.828V =  0.010V -> Pass
    [ 3] 3.716V - 3.729V =  0.013V -> Pass
    [ 4] 4.119V - 4.107V =  0.012V -> Pass
    [ 5] 4.040V - 4.051V =  0.012V -> Pass
    [ 6] 3.839V - 3.828V =  0.010V -> Pass
    [ 7] 3.826V - 3.837V =  0.010V -> Pass
    ------    End balance test     ------
    ------     Overall: Pass       ------
```

---
## \#845 Posted by: Arek Posted at: 2019-03-31T14:05:58.416Z Reads: 183

```
Guys how do you put together diebiems and unity as both have a switch, do you short it on the unity or bms?
```

---
## \#846 Posted by: christucker Posted at: 2019-04-01T14:36:43.580Z Reads: 184

```
Hello everyone, I am beginner in code, would there be someone who could compile the BMS program in an exe ??
Thank you.
```

---
## \#847 Posted by: Prism Posted at: 2019-04-01T15:17:24.714Z Reads: 187

```
Download the zip-archive from here: https://github.com/DieBieEngineering/DieBieMS-Tool/releases

extract the zip-archive content into a folder. In that folder you'll find an exe.
```

---
## \#848 Posted by: supmike Posted at: 2019-04-03T08:49:07.541Z Reads: 189

```
I have a problem with the Fuse F1- it's blown from unknown cause :disappointed_relieved:

In the material list it's specified as slow blow

![image|690x25](upload://uW7HaNCWKpSIPcctHDo9RkFPbwE.png) 

But when I look at Farnell it's Very Fast Acting - what's right?

Because I have ordered and already paid two new one I would ask if you can put two or three of the fuses in the order.
```

---
## \#849 Posted by: JTAG Posted at: 2019-04-03T09:03:02.281Z Reads: 186

```
this one is not critical, take 500mA if you want! It is just to protect the traces from burning when something is connected wrong or partially. Pleae also check the resistor next to it!
```

---
## \#850 Posted by: supmike Posted at: 2019-04-03T09:05:14.860Z Reads: 191

```
[quote="supmike, post:848, topic:2639"]
Because I have ordered and already paid two new one I would ask if you can put two or three of the fuses in the order.
[/quote]

The resitor is quite ok.
```

---
## \#851 Posted by: christucker Posted at: 2019-04-03T15:57:38.349Z Reads: 190

```
hi, is there a file with pcb type (copper layers, hole size, thickness ......)
It's to start manufacturing.
Thank you
```

---
## \#852 Posted by: christucker Posted at: 2019-04-04T16:53:56.163Z Reads: 186

```
172/5000

Thanks to JTAG for putting his creation in open source and spend a little time to answer on this forum. Is there a charge cycle count in the firmware?
```

---
## \#853 Posted by: JTAG Posted at: 2019-04-04T20:00:03.575Z Reads: 185

```
The PCB will fit almost all standard pools, no real need for thick copper.

Currently not, but I am more and more thinking about implementing one. Maybe a bit more a Ah counter that later on can be used to calculate cycles. Thanks for the question.
```

---
## \#854 Posted by: christucker Posted at: 2019-04-04T22:45:31.269Z Reads: 183

```
the ideal would be a data logger on the SD card, but it would add a real-time clock and also a lot of code ....
```

---
## \#855 Posted by: gecko242 Posted at: 2019-04-05T08:32:08.955Z Reads: 184

```
Hey JTAG, is there a document out there outlining the CAN commands you have implemented?
```

---
## \#856 Posted by: Prism Posted at: 2019-04-08T18:50:58.384Z Reads: 183

```
I don't think it was discussed here before, but regenerative breaking from the VESC should still work with this BMS, right?
The generated voltage will just pass through the body diodes of the power switch mosfets back into the battery. 
Can you confirm this @JTAG?
```

---
## \#857 Posted by: mishrasubhransu Posted at: 2019-04-08T19:23:19.794Z Reads: 185

```
not JTAG, but yes, can confirm.
```

---
## \#858 Posted by: ugashack Posted at: 2019-04-14T19:28:34.417Z Reads: 182

```
Is there anyone who have tried to use DieBieMS in setup with Freefly ARC200 motor drive, any compatibility issues?
```

---
## \#859 Posted by: amazingdave Posted at: 2019-04-17T13:09:41.886Z Reads: 185

```
Just waiting for my bms to be delivered.... 

Does anyone know whether this meanwell supply will be ok for 12s? Seems to do 54v at nearly 4amps.

https://www.digikey.co.uk/product-detail/en/mean-well-usa-inc/ELG-200-54/1866-1518-ND/7702988?utm_adgroup=&mkwid=sGaj31WLh&pcrid=337211407576&pkw=&pmt=&pdv=m&productid=7702988&slid=&gclid=CjwKCAjwndvlBRANEiwABrR32M5onDPVYwreg9UM1lFxbpJKLjnZuXRINr1i7qX0YcmmJ01cJMwnoRoC8O4QAvD_BwE
```

---
## \#860 Posted by: deucesdown Posted at: 2019-04-17T16:09:27.128Z Reads: 182

```
That one looks like voltage and current are fixed.

This one is similar but adjustable

https://www.digikey.co.uk/product-detail/en/mean-well-usa-inc/HLG-240H-54A/1866-2450-ND/7704006

The "A" at the end of the model indicates adjustable. In this model 50-57v.
```

---
## \#861 Posted by: Elektrospy Posted at: 2019-04-26T07:01:36.682Z Reads: 171

```
hey @PatRocks did this wiring worked for you in the end?
```

---
## \#862 Posted by: MiniChopper4Me Posted at: 2019-04-26T19:11:58.229Z Reads: 175

```
@jtag Is it safe to charge a 12S4P Samsung 30Q pack with DieBieMS at 8A? Is it necessary/desireable to add a 10A fast acting fuse for the charge port as close to the battery as possible as is usually recommended for said charge port?
```

---
## \#863 Posted by: JTAG Posted at: 2019-04-26T19:30:13.522Z Reads: 175

```
Yes 8A is perfect, my charger charges with that current as well. No need to put a fuse in series.
```

---
## \#864 Posted by: willumpie82 Posted at: 2019-04-26T20:09:02.437Z Reads: 173

```
I just ordered a meanwell HLG-120H-42, but did not pay attention to the ip67 rating, this means that took mee some digging in the potting to get to the trim potmeters ;-) If anyone is ordering this HLG-120H-xx series make sure it is a _A version (ip65 rated, trim pots accessable when top cover removed.
```

---
## \#866 Posted by: oyta Posted at: 2019-05-01T09:03:35.182Z Reads: 170

```
Any chance you'll build the latest DieBieMS version for Mac and publish it? :slight_smile:
```

---
## \#867 Posted by: rpasichnyk Posted at: 2019-05-01T18:31:17.962Z Reads: 173

```
Will do it🤓

Look what I received today
![image|666x500](upload://sjZP4qTYtyyVNFnP95dYfDjIfsr.jpeg)
```

---
## \#868 Posted by: banjaxxed Posted at: 2019-05-01T18:47:33.450Z Reads: 175

```
The matching socks and DieBieMS’s are strangely hypnotic in this formation
```

---
## \#869 Posted by: willumpie82 Posted at: 2019-05-02T06:47:25.590Z Reads: 175

```
I love the symmetry, spot the differences...
```

---
## \#870 Posted by: AlexBE Posted at: 2019-05-02T06:47:59.987Z Reads: 176

```
Random note for anyone that reads this, the Unity has L and H reversed.
```

---
## \#871 Posted by: rpasichnyk Posted at: 2019-05-02T07:23:35.718Z Reads: 177

```
[quote="oyta, post:866, topic:2639"]
Any chance you’ll build the latest DieBieMS version for Mac and publish it? :slight_smile:
[/quote]
I just checked and nothing really changed from the last time I uploaded 0.21 macOS build. Am I wrong?

Upstream https://github.com/DieBieEngineering/DieBieMS-Tool

macOS builds https://github.com/rpasichnyk/DieBieMS-Tool/releases
```

---
## \#872 Posted by: oyta Posted at: 2019-05-02T07:28:56.910Z Reads: 178

```
I think you are right - there are no big changes from v0.21 to v0.27, and I guess (haven’t tried) I can use the v0.21 for my needs. I just thought I should use the latest version. Thanks for checking it out :slight_smile:
```

---
## \#873 Posted by: rpasichnyk Posted at: 2019-05-02T07:44:54.307Z Reads: 176

```
Now I see, I was checking the wrong (master) branch on GitHub. @JTAG what branch should I use to build v0.27? :nerd_face:
```

---
## \#874 Posted by: JTAG Posted at: 2019-05-02T18:47:11.391Z Reads: 175

```
https://github.com/DieBieEngineering/DieBieMS-Tool/tree/efoildevelop this is the latest.

Will merge it once I added some other features.
```

---
## \#875 Posted by: oyta Posted at: 2019-05-03T07:00:48.477Z Reads: 184

```
I am new to the CAN stuff and think I made some mistake as it does not work. I have connected the VESC 6.0 and DieBieMS with a CAN cable like this:
![DieBieMS%20and%20VESC%20CAN%20connection|448x500](upload://4K6O4QJid8swCsjNOBNA6tUqNuL.png) 

(The colors are according to my wires).

So I booted the board, and hoped that Metr would show me the DieBieMS data. But nothing happened. Then I connected the PC to the VESC 6.0 and ran the command

`can_scan`

in the terminal. It returned

`No CAN devices found`

That seems odd. The App Settings on the VESC are:
![image|578x500](upload://2rmcRm27Hk1l9Wnk3du667FsDj0.png) 

Edit: I changed the VESC CAN ID from 108 to 0. But it did not help.

I then ran the command `config` in the DieBieMS Tool:

    ---   BMS Configuration   ---
    NoOfCells                  : 10
    batteryCapacity            : 9.00Ah
    cellHardUnderVoltage       : 2.300V
    cellHardOverVoltage        : 4.350V
    cellLCSoftUnderVoltage     : 2.700V
    cellSoftOverVoltage        : 4.100V
    cellBalanceStart           : 3.800V
    cellBalanceDiffThreshold   : 0.010V
    CAN ID                     : 10
    --- End BMS Configuration ---

![image|509x99](upload://enIJWrkZqGjO9NSsaXLAwypCjmT.png) 

I have tested the cable, and it should be ok.

Should I enable CAN Fwd or something? Do anyone see an obvious mistake? :grimacing:

@bevilacqua Did you succeed in connecting the DieBieMS and VESC? Any tips?

Edit: VESC 6.0 is on FW version 3.55.
```

---
## \#876 Posted by: bevilacqua Posted at: 2019-05-03T07:25:04.412Z Reads: 177

```
Check that you haven’t connected the 5p cable backwards, that was my problem. I got push to start to work, but sadly fried some component related to the CAN system when I wired it wrong. 

I’ll take a look to my current connector when im back home.
```

---
## \#877 Posted by: Elektrospy Posted at: 2019-05-03T11:05:09.496Z Reads: 175

```
Hey @oyta, for the CAN bus connection you don't need to cross the datalines, 
its not like serial communication. :wink:
Just connected them in parallel and make sure every slave on the bus has another slave id.
```

---
## \#878 Posted by: oyta Posted at: 2019-05-03T11:20:40.490Z Reads: 173

```
Thanks for your reply. I am connecting CAN H with CAN H and CAN L with CAN L. Is that incorrect? The illustration is crossing the cables, but that is purely because of the order on the plugs.
```

---
## \#879 Posted by: Elektrospy Posted at: 2019-05-03T11:28:12.608Z Reads: 170

```
oh yea sry, i missed the letters :sweat_smile:, but it should be fine like that :thinking:
```

---
## \#880 Posted by: oyta Posted at: 2019-05-03T18:06:23.561Z Reads: 176

```
**Push to start actually works! So that is great. But the Metr and the VESC does not find any CAN devices**.

What do I need to set the different config parameters to? The VESC has CAN Id = 0 and DieBieMS has CAN Id of 10. That is correct according to what I've read.

What about other parameters such as CAN forward? Are there any parameters I should check on the VESC or the DieBieMS? I have tried to read about CAN without luck.
```

---
## \#881 Posted by: bevilacqua Posted at: 2019-05-03T18:34:44.469Z Reads: 175

```
my connector has the CAN_L and CAN_H reversed. Check if that is the problem. 
Best of luck ;)
```

---
## \#882 Posted by: oyta Posted at: 2019-05-03T19:02:10.173Z Reads: 171

```
Thanks for checking it.

I have checked my wiring and according to my own post which JTAG confirmed, it should be correct: https://www.electric-skateboard.builders/t/diy-6s-to-12s-bms-with-can-diebiems/2639/445?u=oyta

On the VESC 6.0 each wire is marked next to the port socket, so that is quite easy to see. I will try to check once again. Still not getting it.

I have DieBieMS hardware version 0.5. Could there be any problems with that specific hardware?
```

---
## \#883 Posted by: bevilacqua Posted at: 2019-05-03T19:06:55.902Z Reads: 167

```
You are prob. right, I run a dual FB and I only checked the cable color... Maybe the coloring is reversed and that's it. *edit (the coloring of my connector) 

You could try extracting and flipping the crimp connector just to see if it works, swiching data wires should be ok...
```

---
## \#884 Posted by: oyta Posted at: 2019-05-04T07:03:36.977Z Reads: 164

```
@JTAG I tried to find some commands to run in the DieBie terminal giving some info on CANBUS. But no success. Do you know if there are any? Any way to troubleshoot the CANBUS further? I suspect it is my lack of knowledge putting me off here.
```

---
## \#885 Posted by: gecko242 Posted at: 2019-05-08T07:47:18.801Z Reads: 161

```
What ESC Are you using? My focbox was incorrectly marked, CANH and CANL were swapped...
```

---
## \#886 Posted by: oyta Posted at: 2019-05-08T13:32:12.121Z Reads: 170

```
I’m using the first VESC 6 from Vedder&Trampa. And DieBie MS Hw version 0.5. I tried to find forum posts about whether the VESC or the DieBie could have been swapped from what I have drawn in the illustration above, but haven’t. 

Is it risky swapping them to test it?
```

---
## \#887 Posted by: oyta Posted at: 2019-05-08T19:20:29.047Z Reads: 173

```
So, I did try swapping CH and CL without luck. I also made a new cable, but same result. If there are no config settings other then the CAN ID I need to make sure of, I do not know what to try next. BTW, push to start still works. Anyone with the VESC 6 and DieBieMS version 0.5 tried to use CAN?
```

---
## \#888 Posted by: andi91 Posted at: 2019-05-10T18:39:12.931Z Reads: 193

```
Hey guys!

I need some help and I hope you can help me.

I have orderd my DieBieMS in the last batch.
https://www.electric-skateboard.builders/t/diebiems-v0-8-batch-3/
On monday I have received it.

For me and my friends it is hard to understand, how to control it or what are the requirements to start the DieBieMS.
On tuesday we started to test it.
We have two VESCs and connected it with the DieBieMS. (Only with the power cables, no CAN)
We wired the switch like this wiring diagramm:
https://www.electric-skateboard.builders/t/diy-6s-to-12s-bms-with-can-diebiems/2639/570
We are a bittle bit confused which is the coorect wiring, because the text say that we have to wire up "black and NC" and the text says "black and NO" and NC is not connected.

In the Tool we can see that the switch act normally, but maybe inverted. But we don't know which state we need at bootup.
In the Tool it shows all voltages of the Cells and the Total voltage.

Here the staus from terminal:

-----Battery Pack Status-----
Pack voltage Direct   : 24.65V
Pack voltage CVAverage: 24.66V
Pack current          : 0.04A
Low  current          : 0.04A
High current          : 0.00A
State of charge       : 100.0%
Remaining capacity    : 12.00Ah
Operational state     : Power down
Load voltage          : 0.00V
Cell voltage high     : 4.149V
Cell voltage low      : 4.078V
Cell voltage average  : 4.109V
Cell voltage mismatch : 0.071V
Discharge enabled     : False
Charge enabled        : False
Power button pressed  : True
CAN safety state      : False
---End Battery Pack Status---
 
After 1 hour of testing we give up for on tuesday.

Today we started again.
We connected the battery with the Batteries and after we pressed the button one (or two) times the VESCs Leds light up.
We don't know what was the problems two days before but it seems to work.

Then we wanted to start "the real tests" with current draw. 
At first we have to mount the batteries, better than in "light test"
After this, the DieBieMS begins to turn on and shut down again.

We notice with the Toolbox, that one of the balancing wires are a little bit wobbly and the cell measurement was wrong, if we bond the cable.
We disconnted all and correct this issue.

But since this time the DieBieMS won't boot up again.
If we press the switch, one of the leds flashs up (0,1 secs)
Also I don't get a USB connection. (One time no serial port and one time it says can't detect firmware.

I was afraid to blow up one the LTC chip (and maybe more).
But the connection worked before, also with the wobbly balance lead.
I have looked at the Datasheet of the LTC, maybe there was to much voltage on one balance input if there was one cell not connetect. It should be also no problem, because the terminals can catch up to 25V.

But then I don't know why the DieBieMS won't boot up.
Is there a chance to hard reset, without software?! Or another way like USB?!
Now we test with few hours without power, because from tuesday to today it worked also, and we don't know why ;)

Sorry for my bad english.
We are looking forward to your answers.

regards
Andreas
```

---
## \#889 Posted by: Prism Posted at: 2019-05-11T15:09:54.099Z Reads: 178

```
Sorry for the confusion about the switch wiring. 
I made a mistake in the picture. The text description is the correct one.
Black needs to be connected to the NO contact of the switch.
```

---
## \#890 Posted by: rpasichnyk Posted at: 2019-05-12T16:44:13.353Z Reads: 177

```
DieBieMS-Tool (macOS build) with v0.27 firmware https://github.com/rpasichnyk/DieBieMS-Tool/releases/tag/v0.27
```

---
## \#891 Posted by: Margoo Posted at: 2019-05-15T20:11:06.591Z Reads: 188

```
Got my DieBieMs from last third batch.
Now I want to quicktest with the Diebiems tool with to retrieve any information from the device.

According to https://github.com/DieBieEngineering/DieBieMS this powering is supported?!


_When a USB cable is connected or 5V is applied on the CAN connector the BMS will boot into external power mode. Firmware updating trough the hardware bootloader or communication over CAN bus is now possible. The power on enable by CAN functionality allows an externally battery powered telemetry device to enable the BMS and request battery pack data (giving for example daily / weekly / monthly status updates)._

I connect USB, windows recognizes, shows addtional com port 6 and the tool also shows "COM6 DieBieMS". When connecting after some seconds it says "Could not read firmware version" and state not connected. No leds on board are active?!

1. Is the firmware not preprogrammed?
2. Do I have to connect at least something else? Soft Power Switch? I already short those to pins!
Do I need a battery to connect via Config Tool?

Thank you for your ideas..
Margoo
```

---
## \#892 Posted by: andi91 Posted at: 2019-05-17T20:50:02.655Z Reads: 184

```
Hey @all!

We have solved the problem!
We don't know, what we have done, but we have damaged the R55 resistor.
The only reason, we think is to much current, but not enough for fuse.
Maybe we plug in the wrong socket or bridge any pad.
Now we know the "can't detect firmware" error was because the STM32 can't boot and also one led should light up.
At first we thought that we killed the voltage regulator-

Measure different voltages with the help of the shematics brings us to the solution.
Now we have soldered a new resistor in place and all works fine.

Now it is working perfectly. Thank for this great BMS!!!

regards
Andi
```

---
## \#893 Posted by: Acido Posted at: 2019-05-23T06:01:41.962Z Reads: 182

```
Can someone confirm that this is the balance wire connector WR-MPC3 ?
```

---
## \#894 Posted by: Jumpman Posted at: 2019-05-23T10:59:33.431Z Reads: 181

```
WR-MPC3 16 way, 3mm, 2 row.

For the part attached to your balance leads, have a look at 662016113322.
```

---
## \#895 Posted by: willumpie82 Posted at: 2019-05-25T07:32:18.211Z Reads: 178

```
Hey, i noticed graphical glitches with the .27 mac tool that are not present in .21e (running om latest mojave on mbpt’18)
```

---
## \#896 Posted by: rpasichnyk Posted at: 2019-06-01T05:32:50.037Z Reads: 174

```
Hi, thanks for letting me know. I rebuilt .27 with older framework and uploaded the binary again. The glitches seem to be gone https://github.com/rpasichnyk/DieBieMS-Tool/releases/tag/v0.27
```

---
## \#898 Posted by: Pimousse Posted at: 2019-06-03T08:58:02.360Z Reads: 171

```
I'm considering jumping into DieBieMS journey and I'm looking closer at the OLED display.
Is the BMS only compatible with the 0.96 128x64 display ? Or is it possible to configure a smaller one (such as [a 128x32](https://www.ebay.nl/itm/OLED-LCD-0-91-Inch-Display-blue-128x32-Module-SSD1306-Driver-For-Arduino-5038Z/163712410640?hash=item261e052410:g:RtcAAOSwGJpc74pQ) for thin enclosure) ?
Can't wait to join the DieBieMS adventure !
```

---
## \#900 Posted by: saybot Posted at: 2019-06-04T09:55:15.082Z Reads: 162

```
can you public step file for modeling battery with this BMS?
There is no step file anymore in Github
```

---
## \#901 Posted by: bevilacqua Posted at: 2019-06-04T10:55:19.645Z Reads: 173

```
https://github.com/DieBieEngineering/DieBieMS/blob/master/3DFiles/DB10005_BMS.step
```

---
## \#902 Posted by: Acido Posted at: 2019-06-05T18:26:08.800Z Reads: 165

```
does anyone know the specific type of tool do I need to crimp the balance wires?
```

---
## \#903 Posted by: MiniChopper4Me Posted at: 2019-06-08T22:49:33.903Z Reads: 162

```
post 611 was what @Prism recommended and worked for him.  I used PA-09 from Amazon and that worked fine for me.
```

---
## \#904 Posted by: MiniChopper4Me Posted at: 2019-06-08T22:53:34.522Z Reads: 164

```
Can anyone confirm the proper connect-disconnect sequence to ensure not burning anything out?

What I think it is:

Connect order

1) Battery negative
2) Battery positive
3) Balance connector

Disconnect order

1) Balance connector
2) Battery positive
3) Battery negative

I assume all the other connectors don't matter when you connect/disconnect them.
```

---
## \#905 Posted by: JTAG Posted at: 2019-06-10T10:26:14.535Z Reads: 164

```
When the load/USB is not connected it doesn't matter. But when there / it is, it is preferred to prevent currents flowing trough the balance wires. So if possible when connecting to the battery connect the balance lead last and when disconnecting from a battery disconnect the balance lead first.
```

---
## \#906 Posted by: Martin Posted at: 2019-06-15T13:04:35.541Z Reads: 165

```
I attendied DieBieMS 3rd batch.
I wonder power switch wiring.
Is the wiring diagram shown in the picture below correct?

![power|457x142](upload://dJcVSXLtpCWZsMPtZeVoppQvEzM.jpeg)
```

---
## \#907 Posted by: Prism Posted at: 2019-06-15T14:23:05.948Z Reads: 164

```
No, the PushButton Pin is labeled incorrectly. It needs to be connected to the NO contact of the switch. Here is an updated diagram: 

![bms%20switch|690x339](upload://ikyQrhghXZhzZjFF6qS3fv6rrj9.jpeg)
```

---
## \#908 Posted by: Martin Posted at: 2019-06-15T17:07:20.100Z Reads: 162

```
Thank you so much.!!:smiley::smiley:
```

---
## \#909 Posted by: Martin Posted at: 2019-06-16T02:37:35.198Z Reads: 161

```
I use a 12s1p 15ah battery.
I use a power supply of 50.4V, 10a.

BMS temperature during charging increases to 70 degrees celsius.
Is it normal?

Do I need a cooling fan?
```

---
## \#910 Posted by: Devilmycry Posted at: 2019-06-16T03:11:52.995Z Reads: 160

```
![image|626x500](upload://w2acP0Gl9HglA4c90XfexM9hTBB.jpeg) 

😎😎😎😎
```

---
## \#911 Posted by: Prism Posted at: 2019-06-16T12:03:15.979Z Reads: 163

```
That connection is not needed. If you look at the OLED I2C display you'll see it only has four pins. ![2019-06-16|690x149](upload://mlrEuvBk4q8worNdLzUhBbiWmdi.png)
```

---
## \#912 Posted by: Prism Posted at: 2019-06-16T12:42:26.370Z Reads: 166

```
If the red area gets hot during charging, that's normal. Those are the balance resistors. If you are uncomfortable with how hot they get you can decrease the number of active resistors in the configuration. Doing this will decrease the temperature but also increase the time for balancing your pack. 
![DieBieMSV0_4TOP|690x302](upload://kjMzPnDv7ebXEEOE8DVOpBaFChn.png) 
![2019-06-16%20(1)|690x159](upload://cYGU3IDQ2uAYOE3AEqSiMuRGetS.png) 

also, what kind of cells do you use in your pack? 12S1P with 15Ah means 12 cells with 15Ah each.
```

---
## \#913 Posted by: Martin Posted at: 2019-06-16T12:52:18.049Z Reads: 164

```
That's corrent. I'm using 15Ah cell.

Thank you for your help. :smiley:
```

---
## \#914 Posted by: hahne Posted at: 2019-06-21T16:07:28.798Z Reads: 164

```
Somewhat random question: 

I am currently using a different 12s BMS (yes, I will upgrade to the DieBieMS eventually) with a charger that outputs exactly 50.4v. I notice that every time I charge my board, it stops charging when the batttery is at 48.5v or thereabouts. Is this because there is voltage drop across the bms? I am hoping that it is not faulty or something.

I know it was mentioned earlier that the DieBieMS requires 1-3V higher than the full pack voltage, but I was not sure if that was specific to the DieBieMS for running some extra electronics or something.  

Is it just a standard procedure to charge all BMSs at a slightly higher voltage than the full battery pack voltage?
```

---
## \#915 Posted by: Devilmycry Posted at: 2019-06-27T01:08:54.351Z Reads: 154

```
Hi need help for this
I downloaded the zip but after 😭😭😭😭
```

---
## \#916 Posted by: evoheyax Posted at: 2019-06-27T01:23:56.484Z Reads: 157

```
Idk where JTAG is, but I can't seem to get a hold of him anymore. I have since moved on to another smart bms and couldn't be happier.
```

---
## \#917 Posted by: bsancken Posted at: 2019-06-27T02:51:47.086Z Reads: 156

```
What smart BMS are you on now?


Btw
@JTAG  ig people are looking for you...
```

---
## \#918 Posted by: evoheyax Posted at: 2019-06-27T03:04:12.174Z Reads: 158

```
xiaoxiang smart bms from bmsbattery.

https://bmsbattery.com/bmspcm/833-16889-smart-bms-10s13s-60a-with-blue-tooth-android-or-ios-app.html

It's less expensive, and you don't need to discharge though it. Just use it as a charge only, you can view cell voltages on your phone, current charging rate, and more. It's not all in the same app, but If you need something that just works, no fuss, this is it.
```

---
## \#919 Posted by: Freemann Posted at: 2019-07-02T07:56:21.679Z Reads: 153

```
Watch some video's about the BMS and noticed a "startup"/precharge delay while switching from charging to discharging or the other way around.

I want to use this BMS for my diy-PowerWall and for this purpose I need a constant output, because devices like my 12v Router/Switch/Accesspoint/etc are connected and don't want to reboot them X time a day.

Is this BMS able to constantly output XA 24h a day while charging X time a day random times with random durations?
```

---
## \#920 Posted by: Pimousse Posted at: 2019-07-05T09:17:18.621Z Reads: 149

```
Dear DieBieMS users, I started to write a light manual condensing all info I collected to start my experience with the DieBieMS.
Feel free to join the adventure by adding your stuffs (drawings and schematics are more than welcome, too much time consuming for me).

https://drive.google.com/file/d/1cAlaAxA7yCMaTV4SlLBUlxvXA49OH1vI/view?usp=sharing

(Read only. Please duplicate and activate "Track changes" in Revision tab before adding stuffs. Then, submit me the file back. Thanks !!)
```

---
## \#921 Posted by: Prism Posted at: 2019-07-06T18:50:44.307Z Reads: 145

```
Nice, I was thinking of writing some sort of manual too. I'll write down what I know and leared about the BMS and submit it to you when I have some time.
```

---
## \#922 Posted by: janpom Posted at: 2019-07-09T10:49:13.844Z Reads: 146

```
[quote="evoheyax, post:609, topic:2639"]
All Vesc’s GND -> BMS CAN GND
[/quote]

Is it really necessary to connect all VESC's GND to the BMS CAN GND? Wouldn't it be sufficient to connect only the master VESC GND?

When interconnecting two VESCs via CAN, only CAN L and CAN H need to be connected (not GND).
```

---
## \#923 Posted by: bevilacqua Posted at: 2019-07-09T14:40:41.239Z Reads: 147

```
I only use the master GND, the rest is not needed.
```

---
## \#924 Posted by: directC Posted at: 2019-07-13T13:28:53.632Z Reads: 146

```
should pack- and pack+ be connected without a fuse? and why?
![25|375x500](upload://cJtxgjYrb2GSdLw4BHS015v10dq.jpeg)
```

---
## \#925 Posted by: JTAG Posted at: 2019-07-13T13:59:23.979Z Reads: 146

```
Leakage current for the board power supply.
```

---
## \#926 Posted by: directC Posted at: 2019-07-13T14:24:09.395Z Reads: 147

```
connected everything, but it's not connecting in the bms tools

![35|375x500](upload://hn7Kgb8rjNEDs0qz9XeJgoLnWi2.jpeg)   
![36|375x500](upload://eWEKzNdPd9ccOezryTS77SRrc6C.jpeg) 
![33|375x500](upload://fiieWbRopdvjIxS203RGg3sl5lB.jpeg)
```

---
## \#927 Posted by: directC Posted at: 2019-07-13T15:09:33.535Z Reads: 144

```
got it, needed to install the driver
can be found here: https://drivers.softpedia.com/get/Other-DRIVERS-TOOLS/Others/Silicon-Labs-CP2104-USB-to-UART-Bridge-VCP-Driver-661.shtml#download
```

---
## \#928 Posted by: directC Posted at: 2019-07-17T09:53:43.510Z Reads: 140

```
what settings do you guys recommend for a 12S14P Li-ion battery?
```

---
## \#929 Posted by: Kug3lis Posted at: 2019-07-17T10:10:40.376Z Reads: 140

```
@JTAG is it me or LTC6803-2 got even more expensive? 19$ right now :(
```

---
## \#930 Posted by: GeorgS Posted at: 2019-07-18T09:29:17.014Z Reads: 140

```
How to calibrate the internal temp reading? It should be around 22-25 at most currently.

![image|690x313](upload://5elNBSfQZo9EJrr6oV8OmHh3Vj8.png) 

These settings are for the external temp sensors? because changing them did nothing....
![image|690x171](upload://uKGnaWIn3TurC99cCGQI6qj5HuG.png)
```

---
## \#931 Posted by: directC Posted at: 2019-07-18T10:11:17.923Z Reads: 133

```
is a 50.4V charger only capable of charging a 12S battery to 48V?
or did i miss something in the configuration?
```

---
## \#932 Posted by: Kug3lis Posted at: 2019-07-18T10:19:59.173Z Reads: 133

```
![image|690x57](upload://3hTpu2NmB5okY9ZCbmh6XxseFi.png)

To charge to 50.4V u will need 53.4V charger or etc
```

---
## \#933 Posted by: directC Posted at: 2019-07-18T11:26:04.558Z Reads: 134

```
is this only for diebiems or every bms?
```

---
## \#934 Posted by: Klaerke91 Posted at: 2019-07-18T11:57:30.646Z Reads: 135

```
only for this bms
```

---
## \#935 Posted by: GeorgS Posted at: 2019-07-18T15:28:19.331Z Reads: 136

```
Anybody got any ideas how to fix this? 
Not sure really what happend. I was configuring the bms. Got it setup. Then I added charging cable and connected vesc and the canbus cable. Tried to power it up but the power led started flickering and the bms made a buzzing sound. Usb seems to be working still, shows up as com4, but I cant flash or connect to it.

https://drive.google.com/file/d/1--CxY4fAFC_Ysu8C46EpwRzpnXyzZzJu/view?usp=drivesdk

EDIT: Seems like R55 resistor has gone bad. Just like @andi91. Will solder a new one tomorrow.
```

---
## \#936 Posted by: Klaerke91 Posted at: 2019-07-18T15:43:26.068Z Reads: 135

```
i dont have access.
```

---
## \#937 Posted by: GeorgS Posted at: 2019-07-18T20:46:15.108Z Reads: 135

```
@Klaerke91 Fixed the drive video link, and also fixed my bms. I replaced the R55 resistor and got it working again. Luckily it was an easy fix.
```

---
## \#938 Posted by: Olli Posted at: 2019-07-18T21:31:40.293Z Reads: 136

```
I just connected my DieBieMS, battery pack is around 40v, same for load but charge port is 1.3V...is it normal?
```

---
## \#939 Posted by: Giga Posted at: 2019-07-18T22:38:33.105Z Reads: 128

```
Thats wrong. 
A 50.4V charger will charge your battery till 49.7V on charge port and to 50.4V on discharge port (as long as you enable charging through discharge).
The 3V difference are just for charge detect (which can be triggered by switching on by button, so you can also charge below 3V difference).
 
So e.g my batter is 12S and I always charge with 50.4V charger through charge port. 
Auto detect also works because I drive the battery below 47V...so there is 3v< difference between charger and battery. But it only charges to 49.7V because of the 0.7V diode drop at the charge port.

Which is also the reason for this:
[quote="Olli, post:938, topic:2639"]
but charge port is 1.3V…is it normal?
[/quote]

The charge is secured by a diode (so you cant short your battery by a broken charger). Thats the reason why there is no voltage on the port, it's a one way.
```

---
## \#940 Posted by: glyphiks Posted at: 2019-07-19T00:36:51.625Z Reads: 126

```
I'm confused. Heaps of posts saying that you need a charger that will charge 3v higher.
```

---
## \#941 Posted by: annihil8ted Posted at: 2019-07-19T02:15:05.683Z Reads: 129

```
You need a charger with a higher than 3V to automatically turn on the bms and charge. You just need a .7V higher charger that'll charge the battery.
```

---
## \#942 Posted by: Pimousse Posted at: 2019-07-21T20:12:53.023Z Reads: 134

```
Hi @JTAG,
My DieBieMS is nearly connected (I'm waiting for pre-crimped wires for connecting balance leads).

But I have 2 "issues" :

1.   The "allowForceOn"parameter doesn't stay to True in DieBieMS Tool. Each time I try it, I need to reconnect and re-assign to True.
2. I constantly get "Precharge Error" when I try to force it on. I tried to increase the timeout to 400 then 500ms (instead of 300ms by default), but still can't have it switched on. Any idea ? Is it related to the absence of cells voltages ?

EDIT : It's connected to a dual FSESC 6.6 with 6x 470 uF caps, powered by a 12S battery. The LEDs of the FSESC light up during precharge.
```

---
## \#943 Posted by: JTAG Posted at: 2019-07-21T20:29:27.392Z Reads: 137

```
Next to writing the config to the BMS ( this transfers it and makes it active ) you can / should also store the config with the diskette logo below it ( this makes it persistent ).

Normally you only get a pre charge error when the cell count doet not match the real pack or when the output load is not valid.
```

---
## \#944 Posted by: Pimousse Posted at: 2019-07-21T20:39:13.349Z Reads: 137

```
[quote="JTAG, post:943, topic:2639"]
you can / should also store the config with the diskette logo below it ( this makes it persistent ).
[/quote]

I do ! 

The first try is ok, the BMS tries to force ON (but still this "Precharge Error" maybe due to the lack of cells voltages). But if I try again, the DieBieMS doesn't want to force it on.
Back on DieBieMS Tool, the setting is back to "False".

I'm running DieBieMS FW 0.27 and DieBieMS Tool 0.27
```

---
## \#945 Posted by: mishrasubhransu Posted at: 2019-07-22T09:29:13.573Z Reads: 133

```
@JTAG, Is it still possible to set the config through terminal? I don't see the set commands when I type help. My BMS is now in a sealed enclosure which is a lot of work to get into. I would like to use the Metr Pro connected to one of the VESC configure DieBieMS.
```

---
## \#946 Posted by: Giga Posted at: 2019-07-22T12:19:35.330Z Reads: 137

```
Why not use Can forward?
```

---
## \#947 Posted by: Pimousse Posted at: 2019-07-22T21:46:00.132Z Reads: 139

```
@JTAG,
I performed some other tests and it appears that ALL the config is reset to default value when I try to force ON.
The config remains the same as long as I don't try to force ON.

Looking at the code I find out that maybe this line causes this behaviour (in `Modules/Src/modOperationalState.c`) :

![bug_forceOn_diebiems|671x153](upload://9dRjSP4L51fWLFoc1g1c7ZFGn1f.png)   

What is the purpose of erasing the flash memory when forcing ON ?

This should also explain the Precharge error, because the FORCE_ON state is triggered but the allowForceOn is false. So when it comes to check the conditions for jumping from `OP_STATE_PRE_CHARGE` to `OP_STATE_LOAD_ENABLED`, it times out.

BTW, do you want me to open an issue in Github instead of using this thread ?
Thanks in advance for your support.
```

---
## \#948 Posted by: JTAG Posted at: 2019-07-22T21:56:13.791Z Reads: 132

```
Hmmmmm this goes far dar back in the history of development of the BMS. Yes please open an issue and I will resolve this. Thanks for reporting!

(I never use force on anymore, I was used my some of me and my friends back in the days when you knew the pack was ok but some of the balance leeds got disconnected )
```

---
## \#949 Posted by: Pimousse Posted at: 2019-07-22T22:25:36.032Z Reads: 137

```
[quote="JTAG, post:948, topic:2639"]
(I never use force on anymore, I was used my some of me and my friends back in the days when you knew the pack was ok but some of the balance leeds got disconnected )
[/quote]

And that makes sense completely ! That could save you if a wire break far from home.
Is there a routine for detecting such a case like this ?

I read in the LTC application notes that there is a routine to implement for detecting a wire break.
But maybe, just summing up all the cell voltages and comparing them to the whole pack voltage could lead to this kind of detection. :+1: 

I created an issue :
https://github.com/DieBieEngineering/DieBieMS-Firmware/issues/4
```

---
## \#950 Posted by: Pimousse Posted at: 2019-07-24T14:08:27.790Z Reads: 130

```
Did someone managed to compile the firmware and software ?
@rpasichnyk ?
```

---
## \#951 Posted by: rpasichnyk Posted at: 2019-07-25T06:24:06.804Z Reads: 133

```
I did not manage to do it long time ago when I wanted. It's not GCC, you need some proprietary software to compile
```

---
## \#952 Posted by: Pimousse Posted at: 2019-07-25T06:27:59.296Z Reads: 133

```
Sure, there's no makefile.
But what software ? STM32CubeMX ?
I'd like to fix this "Force On" bug before going further as this feature sounds critical to me.
```

---
## \#953 Posted by: walleywalker Posted at: 2019-07-31T17:28:52.339Z Reads: 121

```
Does a system with the DieBieMS in it require a loopkey?
```

---
## \#954 Posted by: janpom Posted at: 2019-08-03T09:08:49.016Z Reads: 124

```
I'm having trouble powering on my DieBieMS. I connected the balance leads as well as PACK- and PACK+. I get 5V reading between COMMON- and CHARGE+. When I press the power on button I get a quick LED blink. An on-board LED blink that is. The button LED as well as the display remain off. I also get a quick LED blink when I connect the USB, so it looks like it's registering the power-on signal but then nothing happens. Any ideas?
```

---
## \#955 Posted by: Pimousse Posted at: 2019-08-03T10:59:58.417Z Reads: 129

```
[quote="walleywalker, post:953, topic:2639, full:true"]
Does a system with the DieBieMS in it require a loopkey?
[/quote]

No.

[quote="janpom, post:954, topic:2639, full:true"]
I’m having trouble powering on my DieBieMS. I connected the balance leads as well as PACK- and PACK+. I get 5V reading between COMMON- and CHARGE+. When I press the power on button I get a quick LED blink. An on-board LED blink that is. The button LED as well as the display remain off. I also get a quick LED blink when I connect the USB, so it looks like it’s registering the power-on signal but then nothing happens. Any ideas?
[/quote]

Is the battery voltage ok ?
Nothing displayed on the screen ?
Could you connect DieBieMS Tool to check some realtime values ?
```

---
## \#956 Posted by: GeorgS Posted at: 2019-08-03T13:04:33.198Z Reads: 128

```
https://www.electric-skateboard.builders/t/diy-6s-to-12s-bms-with-can-diebiems/2639/935?u=georgs

@janpom Watch the clip from my drive... I am guessing you have the same issue I had?
I had to replace the R55, its an 15 Ohm resistor. 

![Marginaal%202019-08-03%20160030|690x343,50%](upload://fgUTpmhhD7F0m2736GNVUzoupuV.jpeg)
```

---
## \#957 Posted by: janpom Posted at: 2019-08-03T15:28:38.840Z Reads: 127

```
[quote="Pimousse, post:955, topic:2639"]
Is the battery voltage ok ?
[/quote]

Yes.

[quote="Pimousse, post:955, topic:2639"]
Nothing displayed on the screen ?
[/quote]

No. I think the screen doesn't even power on.

[quote="Pimousse, post:955, topic:2639"]
Could you connect DieBieMS Tool to check some realtime values ?
[/quote]

Nope. :(

[quote="GeorgS, post:956, topic:2639"]
I had to replace the R55, its an 15 Ohm resistor.
[/quote]

This may indeed be it. I'm not getting any resistance reading on that resistor. I'll try to desolder it and temporarily replace it with a THT 15 Ohm resistor (I don't have a SMD replacement). Will report back. Thanks.
```

---
## \#958 Posted by: janpom Posted at: 2019-08-03T15:54:59.115Z Reads: 129

```
That was it! It's working now. Yay! Thanks @GeorgS! 

![IMG_2232|374x499](upload://nieCoTzMrLVZgfq58baBHmryHro.jpeg)

![IMG_2233|666x500](upload://7kb0cQxGlY27AMOsf6aoMNnR3Jr.jpeg) 

@Samau18, how does this happen? Do the boards go through QC?
```

---
## \#959 Posted by: Samau18 Posted at: 2019-08-04T19:26:39.929Z Reads: 123

```
We tested every board. Will check with the team on why that resister problem is not picked up.
```

---
## \#960 Posted by: walleywalker Posted at: 2019-08-04T22:18:49.859Z Reads: 120

```
Can I hook this up to my desktop power supply with 50.4v @ 5 amps just to do the setup, or does it need to have all the balance plugs working? 

I ask cause there seems to be a very specific order of plugging steps in the instructions.
```

---
## \#961 Posted by: Prism Posted at: 2019-08-05T05:06:25.024Z Reads: 115

```
For configuration you can power it with just a power supply. 12V is enough.
```

---
## \#962 Posted by: shark78921 Posted at: 2019-08-05T17:56:28.122Z Reads: 115

```
if my vesc has a power button too which do i go off, the bms power button or the vesc one?
vesc is the flipsky 6.6 https://flipsky.net/collections/electronic-products/products/fs-esc-6-6
```

---
## \#963 Posted by: Prism Posted at: 2019-08-05T19:46:34.685Z Reads: 119

```
I would make the VESC "permanent" on and use the BMS switch. 
Otherwise you would need to have the BMS always on and that's not ideal as it would slowly drain your battery.
```

---
## \#964 Posted by: Prism Posted at: 2019-08-05T22:19:05.509Z Reads: 120

```
Hey @JTAG or anyone else,
ever had a problem with R52 going open circuit?
That's what happend on my BMS. 
R52 connects the negative of the first cell to GND. So I guess there was higher than intended current flow over that resistor causing it to burn up. But I have no idea why or what caused it?
```

---
## \#965 Posted by: walleywalker Posted at: 2019-08-06T02:52:52.331Z Reads: 128

```
Am I just a dumby or is something gone wrong here? I'm able to get connected but when I plug in I get a crossed out battery then it says "bye" on the OLED. 

The DieBie Tool says that the DieBie's firmware is too new to use this tool then it sets me on limited function. 

I'm on v0.27 diebietool with V0.8 hardware. When I boot up the OLED says V0.16

Is this happening cause I don't have balance wires plugged in?

![20190805_213821|666x500](upload://w5Ju7Btgm8Mn4StO2JkANJdFW2i.jpeg) 
![20190805_214901|666x500](upload://fOY4UV7042KFzJNjoTsrSx2fzdl.jpeg)
```

---
## \#966 Posted by: Pimousse Posted at: 2019-08-06T08:25:44.921Z Reads: 121

```
Yes, you get the battery with cross then "bye" message without balance leads.
Try to update the FW using the latest DieBieMS Tool version.
```

---
## \#967 Posted by: glyphiks Posted at: 2019-08-06T08:38:07.082Z Reads: 120

```
Where on earth did you find instructions!?
```

---
## \#968 Posted by: Pimousse Posted at: 2019-08-06T08:48:14.955Z Reads: 122

```
Perhaps he's refering to my draft :

https://www.electric-skateboard.builders/t/diy-6s-to-12s-bms-with-can-diebiems/2639/920?u=pimousse
```

---
## \#969 Posted by: janpom Posted at: 2019-08-06T14:20:29.386Z Reads: 121

```
Fixed properly! First time soldering such a tiny thing. Pistachio nut for scale. Apologies for not using a banana. :laughing:

![image|410x500](upload://l34Ojge5yDkpQ6T0SrJExdryfU8.jpeg)
```

---
## \#970 Posted by: walleywalker Posted at: 2019-08-06T15:00:26.645Z Reads: 120

```
Is there an official procedure for that? I can only find the DieBieMsDefault.bin file on github to load manually but it's pretty nondescript as to whether it's the latest or not.

I believe I'm on the latest DieBieMS tool. I'm using v0.27, is there something greater than that one?
```

---
## \#971 Posted by: Pimousse Posted at: 2019-08-06T15:11:03.021Z Reads: 120

```
FW v0.27 is the latest one I guess.
I'm using DBMS Tool v0.20.
Just go under Firmware tab/Loaded Files and load DieBieMS_default.bin.
```

---
## \#972 Posted by: rene Posted at: 2019-08-06T16:36:50.943Z Reads: 118

```
wow - my first recognition was "Thats a wallnut!" ...
```

---
## \#973 Posted by: walleywalker Posted at: 2019-08-06T18:17:15.263Z Reads: 115

```
Still not getting anywhere with this. I've uploaded the firmware more times than I can count and still can't get out of the "Limited Mode"
```

---
## \#974 Posted by: Pimousse Posted at: 2019-08-06T20:49:50.447Z Reads: 116

```
Maybe your's is a bit older than mine. I recall having seen that for previous version, you need to do a "special" update then it will be possible to flash it with the Tool.

However, I don't know precisely the procedure.

Anyone ?
```

---
## \#975 Posted by: Prism Posted at: 2019-08-06T23:04:13.723Z Reads: 124

```
There was something about manually triggering the bootloader if you updated to the first firmware that supports the DBMS-Tool. 
I think this is what you are thinking of:
https://www.electric-skateboard.builders/t/diy-6s-to-12s-bms-with-can-diebiems/2639/415?u=prism
```

---
## \#976 Posted by: on1y Posted at: 2019-08-07T06:11:50.450Z Reads: 121

```
How do I get a diebiems? Is there a shop or site, or is it thru a person here only? Lemme know. Thx
```

---
## \#977 Posted by: Brianr058 Posted at: 2019-08-07T06:25:39.010Z Reads: 120

```
Can anyone help with the balance lead wiring?
And with downloading the diebiems tool and getting it running as I haven't been able to? Thanks
```

---
## \#978 Posted by: Prism Posted at: 2019-08-07T17:02:14.916Z Reads: 123

```
@Samau18 made group buys. He has a company and manufactured them. He sold them together with all the accessorys you need to get stated like display, on/off switch, cable terminals etc. 
If you are lucky he might still have some left. 
Just message him and ask. 120$ for his kit
```

---
## \#979 Posted by: Prism Posted at: 2019-08-07T21:22:34.319Z Reads: 122

```
You can download the DBMS config tool here:
https://github.com/DieBieEngineering/DieBieMS-Tool/releases/tag/v0.27
assuming you're on windows you just download the zip, extract it into a folder and run the exe that is in that folder. 

What help do you need with the balance leads?
```

---
## \#980 Posted by: Brianr058 Posted at: 2019-08-08T04:41:24.931Z Reads: 116

```
Thank you sir 😊 I'm looking for a diagram. It's my first time building a battery and first time with this bms. Battery is built and ready to go
```

---
## \#981 Posted by: JTAG Posted at: 2019-08-08T10:08:12.912Z Reads: 116

```
You now have firmware V0.30 on the BMS right? Is it giving the limited warning still?

( Edit: oops, you indeed got it working but this is a different topic... my apologies :slight_smile:)
```

---
## \#982 Posted by: Prism Posted at: 2019-08-08T16:15:41.996Z Reads: 117

```
![DieBieMS%20Ballance%20wireing|507x500](upload://9NE0tbTS0rR69suJAwi6oQZTuKl.png) 

Hope this helps you. Pack- and Pack+ connect directly to the screw terminals on the BMS.
Feel free to message me if you have any questions.
```

---
## \#983 Posted by: linsus Posted at: 2019-08-08T16:50:56.596Z Reads: 115

```
The notation on the newer ones read something like C0- and C0+. scratched my head a few times before i realised its gnd and 3.7V
```

---
## \#984 Posted by: Tello1969 Posted at: 2019-08-08T19:11:23.535Z Reads: 115

```
Anyone have a idea on how to run diebiems with unity. Using only unity on/off switch?
```

---
## \#985 Posted by: linsus Posted at: 2019-08-10T18:13:04.804Z Reads: 112

```
Can confirm theres something fishy with R55 on the batch 3. 

Batch 2 R55 (unused BMS) 15 Ohm

Batch 3 R55 (unused BMS) 170 Ohm

Batch 3 R55 (connected for a few minutes) 50k Ohm
```

---
## \#986 Posted by: linsus Posted at: 2019-08-10T18:14:45.037Z Reads: 113

```
@mackann and @rpasichnyk can probably tell you how they did it.
```

---
## \#987 Posted by: walleywalker Posted at: 2019-08-10T20:27:22.066Z Reads: 116

```
I'm interested to know this too. I can't seem to get the DBMS and the Unity talking over CAN.

Edit: I got it working. I had to power both the Unity and the DBMS directly from my power supply. I think it didn't work when the Unity was connected to the Common & Load junctions because I don't have balance wires (or a real battery) attached so no power is being supplied to there. 

I also shorted out my R6 and R7 15ohm resistors somehow by crossing some wires. Need to order some of those.
![Screenshot_2019-08-10-16-45-52|250x500](upload://dBd1l5IDhP0R1Ousn2AjQhBmbhJ.jpeg)

8/12/19 Edit: Correction, R6 and R7 burnt, R55 is fine it seems.
```

---
## \#988 Posted by: SkaterBoy58 Posted at: 2019-08-12T04:59:39.396Z Reads: 108

```
yeah - both of my batch 3 had R55 go open circuit within a few weeks. 
Either a bad batch or a design issue  power rating a bit low)    Cheers
```

---
## \#989 Posted by: JTAG Posted at: 2019-08-12T17:20:03.571Z Reads: 112

```
This 15R resistor or "fuse" burns when wiring is done incorrectly or when you try to enable the BMS trough either the USB connected or pressing the button when the "main"  pack+ and pack- are not connected.
```

---
## \#990 Posted by: walleywalker Posted at: 2019-08-12T18:32:50.388Z Reads: 113

```
1. Get CAN working between the two. 
2. Wire your Unity in "always on" state by shorting the connecting pins on the power button terminal. 
![](https://enertionboards.zendesk.com/hc/article_attachments/360001470995/2018-12-23_1034.png)
See here: https://enertionboards.zendesk.com/hc/en-us/articles/360000672636-How-to-put-Unity-on-always-on-mode-

This way when the DBMS starts up, the Unity will automatically power up when it receives power.

Edit: I'm not sure if this method will allow for the "push to start" option to work in either the Unity or DBMS
```

---
## \#991 Posted by: Prism Posted at: 2019-08-13T00:58:03.895Z Reads: 112

```
Push to start on the DBMS should still work as long as you connect the 5V rail of the unity to the "can enable" pin of the DBMS.
```

---
## \#993 Posted by: janpom Posted at: 2019-08-13T21:03:48.768Z Reads: 111

```
So I managed to short my balance leads as [described here](https://forum./t/the-battery-builders-club/720/758?u=janpom) and that seems to have broken my DieBieMS. :sob:  It still partially works. I can start it with the button and it shows stuff on the display but it won't enable discharge. I noticed that the  LTC6803 chip gets really hot. So hot that I can't keep my finger on it. I immediately disconnected the battery pack including the balance leads from the BMS after discovering this.

@JTAG, could it be that the short has destroyed the chip? Is there a chance that if I get it replaced the BMS will still work or is there likely more damage? There are no visual signs of damage (at least as far as I can tell). Thanks.
```

---
## \#994 Posted by: JTAG Posted at: 2019-08-13T21:23:35.652Z Reads: 115

```
Send it to me and I'll repair it for free (DM) 😁
```

---
## \#995 Posted by: janpom Posted at: 2019-08-13T21:51:43.362Z Reads: 116

```
You're the best! I'll PM you.
```

---
## \#996 Posted by: bsancken Posted at: 2019-08-15T22:14:22.530Z Reads: 116

```
@JTAG First of all, Thank you for your contributions to this project! Just a quick question for you.

Is the "Full battery" sign the only thing implemented for when everything is ok?
I was hoping to be able to have a % or a voltage/both or a cell v readout. I see that was an intended feature initially, just wasnt sure how far you got with that. 

- Searching this thread, I only really saw mentions of the display talking about problems with setup...

I just got my first DBMS up and running, hopefully connecting it to metr soon! 
Thanks!
```

---
## \#997 Posted by: JTAG Posted at: 2019-08-15T22:56:14.398Z Reads: 116

```
On initial firmware writing it shows 100% SoC, when you start using it ( or actually after you fully charge the battery ) the SoC will correspond with the real SoC of the battery. And indeed when the batt is not full it will show a partially filled battery icon.
```

---
## \#998 Posted by: directC Posted at: 2019-08-18T00:03:04.677Z Reads: 113

```
@JTAG is this bms balancing while discharging?  
did a maiden-ride and one of my p-groups is .2V off  
I'm charging it now, to check if it goes back to normal, but just hoping for some more intel

here's full details  
https://forum./t/is-my-battery-ok/6349/
```

---
## \#999 Posted by: glyphiks Posted at: 2019-08-18T00:10:04.463Z Reads: 115

```
![20190818_100751|375x500](upload://bMU9ACVYLhd56nB5EowqoN5ytXA.jpeg) 
 ![20190818_100534|374x500](upload://r7MODV4ZIiDY211OOSja1RqYVjB.jpeg) 

I got the balance wires C1 - C10 figured out, but where do all the other ones go for 10s config?
```

---
## \#1000 Posted by: directC Posted at: 2019-08-18T00:15:38.687Z Reads: 112

```
10S needs from -0 to 9

-0 is - lead  
+0 is + end of first pack  
1 is + end of 2nd pack  
etc  
9 is + end of 10th pack/+ lead
```

---
## \#1001 Posted by: glyphiks Posted at: 2019-08-18T00:21:38.006Z Reads: 111

```
Right... so the C1 is the positive end of the second pack not the first?🤦‍♂️🤦‍♂️🤦‍♂️

All my wires are now the wrong length. Thought it would be pretty safe to assume that c1 would be positive of pack 1
```

---
## \#1002 Posted by: directC Posted at: 2019-08-18T00:29:15.529Z Reads: 111

```
[quote="glyphiks, post:1001, topic:2639"]
so the C1 is the positive end of the second pack not the first?
[/quote]

exactly  
it's a bit confusing whenyour building your first battery  
for me 1 is enough, next one I'll buy ready to use
```

---
## \#1003 Posted by: glyphiks Posted at: 2019-08-18T00:35:04.974Z Reads: 109

```
What a sick sad world we live in. Cheers bro gotta go modify some wires 🤦‍♂️
```

---
## \#1004 Posted by: bsancken Posted at: 2019-08-18T00:58:08.879Z Reads: 114

```
https://drive.google.com/file/d/1cAlaAxA7yCMaTV4SlLBUlxvXA49OH1vI/view

Check this (WIP) manual out that someone else wrote, its also liked up in this thread
```

---
## \#1005 Posted by: glyphiks Posted at: 2019-08-18T02:35:23.997Z Reads: 118

```
So what about the gnd, t0 and t1?
```

---
## \#1006 Posted by: JTAG Posted at: 2019-08-18T05:35:41.839Z Reads: 119

```
Those are for optional external temperature sensors, you can omit them. 

The BMS only balances when charging and almost full.

One thing to try, when connecting a battery and with BMS off, does any of the balance resistors get warm?
```

---
## \#1007 Posted by: banjaxxed Posted at: 2019-08-18T23:39:24.843Z Reads: 119

```
Pull the pins from the JST & reorder that way
```

---
## \#1008 Posted by: glyphiks Posted at: 2019-08-18T23:42:45.706Z Reads: 120

```
Exactly what I ended up doing 👍 was a bit worried it would ruin the crimps but it was all good.
```

---
## \#1009 Posted by: Peakon28 Posted at: 2019-08-20T18:44:24.844Z Reads: 120

```
Hi All , Danny what is the latest release of the firmware. I managed to update to the firmware version 0.27 but I could see a reference to 0.30 firmware. Should I upgrade to this version?
I managed to build DieBieMS myself by ordering boards from JLC PCB and parts from Digikey. It was not easy but second attempt kind off working but I have not tested balancing yet, anyway just wanted to share.![IMG_20190820_193929|690x437](upload://8pdMPEGcPLZiVGsO2mrqKWrFwr7.jpeg) !
![diebie|671x499](upload://3lSxBK8CgG7eugS9vYuvQ8dYDgo.png)
```

---
## \#1010 Posted by: Peakon28 Posted at: 2019-08-20T18:50:40.650Z Reads: 114

```
I think  I have found an answer to my question 0.30 is tagged as pre-release (Temporary release to assist with switching from V3.38 to V0.30) while 0.27 tagged as a latest release.
```

---
## \#1011 Posted by: JTAG Posted at: 2019-08-20T19:42:55.125Z Reads: 113

```
Nice solder job!
```

---
## \#1012 Posted by: trainingforutopia Posted at: 2019-08-20T19:57:17.451Z Reads: 113

```
I love what you are doing here. Great job!
I have one wish and one question:

Wish: please include 16S for people who want to run LiFePO4 batteries. They are becoming more popular as their price keeps dropping. 

Question: I might have missed it, but why did you not include balancing?
```

---
## \#1013 Posted by: linsus Posted at: 2019-08-20T21:04:16.790Z Reads: 112

```
[quote="trainingforutopia, post:1012, topic:2639"]
They are becoming more popular
[/quote]

source on this please :rofl:
```

---
## \#1014 Posted by: trainingforutopia Posted at: 2019-08-20T21:20:51.216Z Reads: 109

```
They are popular with me. That's enough for me. Haha
Jk aside, the camper community is switching over, and there's some early adopters among esk8ers, like @b264. They have their limits (volume), but for a commute board they are ideal.
```

---
## \#1015 Posted by: Peakon28 Posted at: 2019-08-20T23:44:55.464Z Reads: 108

```
Thanks JLC PCB do nice steel stencil it makes your life easier. Placing all those 0402 components was hard work though. How did you do yours?
```

---
## \#1016 Posted by: MiniChopper4Me Posted at: 2019-08-21T18:47:58.617Z Reads: 110

```
For whatever reason, my pack only wants to charge to 4.15V per group.  Is there a setting I need to change in order for it to either allow it to charge to 4.2V per group or at the minimum consider 4.15V full (100%)? Currently it reads as 90% with this capacity.

I double checked the charger already, and it is definitely outputting 50.4V output (12S), so I'm assuming something else needs to be done on the DieBieMS setup?
![image|281x500](upload://ywWrt3dG8UfLtrUnJndtlQOucNy.png)
I realize the picture shows 71%, but it was disconnected at the time.  After reconnecting it read 90% at basically the same state.
```

---
## \#1017 Posted by: walleywalker Posted at: 2019-08-21T19:42:59.471Z Reads: 102

```
Your charger should be at least 3v higher than your max pack voltage. It could be that it's cutting off early because you need at least a 53.4v for a 12s pack.
```

---
## \#1018 Posted by: sayekim Posted at: 2019-08-21T19:55:43.659Z Reads: 100

```
Diebiems takes 0.7 volts so you for full charge you need a charger that charges to 51.1. 

It’s better to charge to less volts anyway for battery wear.
```

---
## \#1019 Posted by: MiniChopper4Me Posted at: 2019-08-21T21:06:09.182Z Reads: 102

```
No, the 3V thing is for it to automatically turn on and start charging, but in any case the problem happens regardless of the point at which I charge the pack.  In other words, even if I plug in my charger at 46V, it still only charges to 4.15V per cell.
```

---
## \#1020 Posted by: MiniChopper4Me Posted at: 2019-08-21T21:09:02.385Z Reads: 106

```
The thing is sayekim, I opened the charger and adjusted the voltage pot to test, and bumped it up to 50.9V output, same result.  I don’t think this is it either :confused:

@JTAG, any advise?
```

---
## \#1021 Posted by: Giga Posted at: 2019-08-21T21:41:05.848Z Reads: 107

```
Did you check the charge current?
Default is charge finished with less than 0.5A 
So if you got a small battery and a slow charger, the CV phase gets quite shallow the closer you get to the 50.4V. 
I guess you need to change the voltage and CV phase of your charger. Or change the min charging current closer to 0.
```

---
## \#1022 Posted by: Prism Posted at: 2019-08-21T21:46:05.701Z Reads: 105

```
What's your configuration? 
Cell soft overvoltage defines the charge cutoff. 
Sounds like it's set to 4,15V in your configuration.
```

---
## \#1023 Posted by: MiniChopper4Me Posted at: 2019-08-21T22:58:04.659Z Reads: 108

```
The charger is 8A, and it throttles down as it gets over 4V/cell.  Its a 12S4P 30Q pack, so not a small pack by any stretch.

Thanks for the tip @Prism, just figured out how to get the config via terminal:![image|281x500](upload://8NadAD9mp8z5y4jKlH0yadcjozt.png)
```

---
## \#1024 Posted by: MiniChopper4Me Posted at: 2019-08-22T02:12:40.613Z Reads: 105

```
Looks like it was in fact the charger.  It has two pots and I tried adjusting both various times to see what their function is, but adjusting either doesn't appear to impact the output voltage.  I'm not sure what the original position of the first pot was before I messed with it ( I made sure to mark the second before I moved it), so when I went to close it back up, I set it in the middle of its range.  This time when I plugged it back in and set the board to charge again, it took the cells all the way up to 4.2V each.  Wish I knew what the pots are for, but unable to find any documentation for the charger (YZPower-450)
```

---
## \#1025 Posted by: walleywalker Posted at: 2019-08-25T22:29:16.361Z Reads: 100

```
Would it be exceedingly difficult to get the DieBieMS working with a 128 x 32 pixel OLED vs the 128 x 64 for space saving?
```

---
## \#1026 Posted by: Tadagami Posted at: 2019-08-26T19:51:07.060Z Reads: 102

```
hey guys, im new to esk8 . Ordered DieBieMS a while ago and just connected it to my battery pack. Right now the pack has 33.3 V and is build out of 10s4p samsung 30Q cells. unfortunately when I connect DieBieMS to my computer the screen turns on and shows DieBieMS logo and 0,27 verion , then crossed battery and then constantly shows BYE. The same thing happens when I use a power button - But BYE disappears. I cant connect it to the tool to configure it . What should I do ??
```

---
## \#1027 Posted by: M77 Posted at: 2019-08-26T22:24:41.426Z Reads: 102

```
Would really like this too. I was thinking about having a look at the code but haven't found a display of that size with the same interface as the one used, all the ones I found was i2c (didn't Google that much).
```

---
## \#1028 Posted by: walleywalker Posted at: 2019-08-26T23:29:13.193Z Reads: 104

```
These are SSD1306 just like the bigger display.  Would they work? 

https://www.amazon.com/MakerFocus-Display-SSD1306-3-3V-5V-Arduino/dp/B0761LV1SD/ref=sr_1_1?keywords=128x32+oled&qid=1566861953&s=gateway&sr=8-1
```

---
## \#1029 Posted by: Pimousse Posted at: 2019-08-27T10:55:20.793Z Reads: 101

```
This is a normal behaviour if you don't connect balance leads.
Did you installed drivers ?
What do you really mean by "can't connect" ?
```

---
## \#1030 Posted by: Tadagami Posted at: 2019-08-27T13:21:05.924Z Reads: 100

```
installed drivers and now I can connect , everything works fine , thanks!
```

---
## \#1031 Posted by: walleywalker Posted at: 2019-08-27T17:58:35.293Z Reads: 102

```
For what it's worth I'd be willing to pitch in on someone's hourly rate to make a fork DBMS firmware for a 128x32 pixel display! 

Calling all coders n'all.
```

---
## \#1032 Posted by: M77 Posted at: 2019-08-27T20:55:15.528Z Reads: 103

```
I also need this very much for my board, will probably have a look at it but don't have so much time at the moment.

Haven't developed with QT before but can't be that different 🤷‍♂️😁 Already got QT setup for visual studio so just need some time to have a look at the code. 

Would be nice with a setting for type of display so both types could be used and set in the config tool.
```

---
## \#1033 Posted by: walleywalker Posted at: 2019-08-28T23:35:23.095Z Reads: 104

```
I just got a 128*32 oled in and wired it up. For the most part I don't think there will be any issue using the small display for normal charge state indication.

The only thing that can't be seen is really small text like the "Bye" and possibly error text. That and the legibility of the small text from a bootloader updating. But the battery logos and boot up splash screen look fine. 

![20190828_182958|375x499](upload://sxGeiTPDL7sc462CI0qaQNOaCtI.jpeg) 
![20190828_182948|375x499](upload://jvfrRykcOi6dVrDCZRDhq0Bz1jU.jpeg)
```

---
## \#1034 Posted by: M77 Posted at: 2019-08-29T06:02:56.507Z Reads: 102

```
That's great 🙂 The text will probably be ok then, also had a look at the code yesterday and not much text is written.
```

---
## \#1035 Posted by: Pimousse Posted at: 2019-08-29T07:07:23.981Z Reads: 101

```
Did you modify the FW code for this ?
I'm desesperatly looking for someone who may explain how to compile the source code.
I've plenty of features ideas (and bug fix) I'd like to develop for this wonderful BMS.
```

---
## \#1036 Posted by: M77 Posted at: 2019-08-29T12:28:10.493Z Reads: 99

```
No modification done for using the smaller display, it works but images gets a little squashed and text might be missing or cut of due to offsets used is for the larger display.

I forked the project yesterday and will probably add a display option letter on but not a priority since it still works ok with the smaller one. Haven't tried to compile it yet so don't know if there is any blockers there.

Have you tried to compile it and had any problems? Anything missing?
```

---
## \#1037 Posted by: Tadagami Posted at: 2019-08-29T13:19:51.807Z Reads: 102

```
Hey guys , I just fucked up my DieBieMS. Was finishing my build and 1 metal screw shorted a lead, i saw some sparkles and now DieBieMS shows wrong C0 voltage. I checked the battery pack and voltages and everythings fine but BMS keeps showing bad voltage. How can I repair it? ![image|634x360](upload://zBHiyd4C85DtKmkBWd0zlejgTmQ.png)
```

---
## \#1038 Posted by: walleywalker Posted at: 2019-08-29T15:04:52.259Z Reads: 101

```
hey man, no I didn't mess with the code, I just plugged in the smaller display.
```

---
## \#1039 Posted by: walleywalker Posted at: 2019-08-29T15:05:24.575Z Reads: 100

```
Did you look for burnt components on the board?
```

---
## \#1040 Posted by: Tadagami Posted at: 2019-08-29T15:06:15.457Z Reads: 97

```
The board looks normal
```

---
## \#1041 Posted by: Pimousse Posted at: 2019-08-29T19:44:16.209Z Reads: 98

```
[quote="M77, post:1036, topic:2639"]
Have you tried to compile it and had any problems? Anything missing?
[/quote]

I don't know how to proceed. I'm used to code VESC FW using Notepad++ (actually Atom) and GCC with terminal.
Here there's no makefile, so it should use another FW.
I got in touch with a canadian guy but he told me that I need a $10k software to compile it... :frowning:
```

---
## \#1042 Posted by: M77 Posted at: 2019-08-29T20:45:06.392Z Reads: 100

```
He has used uVision http://www2.keil.com/mdk5/uvision/ there is a project file in one of the folders in the repository, don't remember where now (on the go atm)
```

---
## \#1043 Posted by: Pimousse Posted at: 2019-08-29T21:00:51.675Z Reads: 102

```
Is there any workaround ? I'd like to avoid spending 10k in a soft just for the DieBieMS FW
```

---
## \#1044 Posted by: M77 Posted at: 2019-08-30T18:15:26.609Z Reads: 98

```
Haven't check but usually there is a free version or for educational purposes?

Any other IDE for ARM should work but you will need to setup for the right processor etc so the build will be correct
```

---
## \#1045 Posted by: JTAG Posted at: 2019-09-04T12:00:02.963Z Reads: 97

```
I had some friends using the latest free environment of STM ( ST took over Atollic ) and they were able to compile and use the code.
```

---
## \#1046 Posted by: JTAG Posted at: 2019-09-04T12:00:45.518Z Reads: 94

```
In what section did the screw land? The balancing section?
```

---
## \#1047 Posted by: Tadagami Posted at: 2019-09-04T12:13:20.965Z Reads: 100

```
actually not, i think it was the opposite side, but not sure cause and removed it super quickly.
```

---
## \#1048 Posted by: JTAG Posted at: 2019-09-04T12:31:33.617Z Reads: 104

```
Good think is that your LTC is still working. Do you have a multi meter around? Can you measure the resistance between the lowest balance pin connection (C0-) that would normally go to the minus of the battery (so not the main minus cable but the one on the balance connector) and the pack- press fit on the BMS ?
```

---
## \#1049 Posted by: glyphiks Posted at: 2019-09-09T04:41:06.715Z Reads: 95

```
Hey guys, 

Finally got my diebiems all hooked up and i'm not having much luck with it.

When i push the button i get the Diebiems screen, then a battery with a cross through it, then it just says bye and turns off.

It also wont connect to the computer, if I try and connect it just displays the same as above but it doesnt turn off, just says bye forever

Was so excited that I got it all hooked up and now i dont know what to do!
```

---
## \#1050 Posted by: glyphiks Posted at: 2019-09-09T05:06:51.691Z Reads: 89

```
Hmm i think that half of my problem is not being able to run the config tool on Mac... any tips?
```

---
## \#1051 Posted by: glyphiks Posted at: 2019-09-09T08:28:42.847Z Reads: 91

```
Got my hands on a PC and I still cant figure out how to open the config tool... beginning to feel waaaayyy over my head
```

---
## \#1052 Posted by: Pimousse Posted at: 2019-09-09T08:33:06.890Z Reads: 94

```
You got it here, right ?
https://github.com/rpasichnyk/DieBieMS-Tool/releases
```

---
## \#1053 Posted by: glyphiks Posted at: 2019-09-09T08:48:41.705Z Reads: 94

```
Thanks! Got the tool now but the BMS wont connect to it...
```

---
## \#1054 Posted by: Pimousse Posted at: 2019-09-09T08:50:01.845Z Reads: 97

```
What voltage do you have between PACK+ and PACK- ?
```

---
## \#1055 Posted by: glyphiks Posted at: 2019-09-09T08:50:36.350Z Reads: 95

```
34 10chars
```

---
## \#1056 Posted by: Pimousse Posted at: 2019-09-09T08:51:25.913Z Reads: 99

```
@JTAG @Samau18
```

---
## \#1057 Posted by: glyphiks Posted at: 2019-09-09T08:55:16.200Z Reads: 97

```
Its not connected via CAN to the ESC... does it need to be?
```

---
## \#1058 Posted by: Pimousse Posted at: 2019-09-09T08:55:44.733Z Reads: 93

```
No `10char`
```

---
## \#1059 Posted by: JTAG Posted at: 2019-09-09T09:03:55.118Z Reads: 101

```
This is good -> the config is not matching the battery and therefore the BMS wants to turn off, the USB is forcing it on (all as intended).

When you open the BMS tool you should be able to connect, if not there is a good chance you need to install the USB - Serial drivers -> google CP2104 driver and youll find them.
```

---
## \#1060 Posted by: glyphiks Posted at: 2019-09-09T09:15:32.005Z Reads: 102

```
Legend! Thanks!

Im connected!

![20190909_191345|666x500](upload://2t2UDU8AkFSysT3ClOUlGj6ForA.jpeg)
```

---
## \#1061 Posted by: JTAG Posted at: 2019-09-09T09:21:24.683Z Reads: 99

```
Perfect! Now change the cell count to 10 and store the config (M with the arrow down) and then safe it (diskette icon) -> followed by a reboot and i think you are good!
```

---
## \#1062 Posted by: glyphiks Posted at: 2019-09-09T09:37:46.061Z Reads: 95

```
Excellent. It worked. now just gotta get motors connected and put it all together and my first build is complete!

Cheers @JTAG and @Pimousse !
```

---
## \#1063 Posted by: MiniChopper4Me Posted at: 2019-09-09T19:45:41.885Z Reads: 98

```
Its happened like 20 times in this thread, and 100 other threads like it:
"Its not working, what do I do?"
"Read through the thread, its answered above"
"TL;DR, please what do I do?"

I'm surprised we don't encounter more folks who don't even want to read the answer to their own question :stuck_out_tongue:

And to be clear, I'm not poking fun at anyone in particular, or even glyphiks, as I myself am guilty of asking a question before I've even properly dedicated the time to reading through for an answer which already exists.
```

---
## \#1064 Posted by: glyphiks Posted at: 2019-09-09T21:16:43.374Z Reads: 96

```
To be fair mate there is like 4 different threads on the diebiems and I did search through them before asking the questions.

With such a massive forum it is sometimes hard to find the exact information you are looking for.
```

---
## \#1065 Posted by: MiniChopper4Me Posted at: 2019-09-09T21:28:10.211Z Reads: 97

```
/agreed, and keep in mind I specifically said I wasn't trying to call you out.  Also, this thread has literally over 1000 posts, so yeah.

Nonetheless I think we are all slowly wanting to read less and less, myself included, and the comment was about that.

Also, Danny is still long overdue with an instruction manual :smile:
```

---
## \#1066 Posted by: walleywalker Posted at: 2019-09-09T21:51:01.403Z Reads: 98

```
It's more than fair for the community to build document and amass all the trouble shooting info into it. We just need to have Danny add a link to it in his first post above so people know where to find it. Someone posted a Google doc a month ago or so, it's a great starting point.
```

---
## \#1067 Posted by: Pimousse Posted at: 2019-09-10T07:09:10.561Z Reads: 102

```
I added a note in the manual about your issue (drivers missing). So your case wasn't a waste of time for everybody :grin:

Each questions of issue someone is encoutering, I put it in the manual.
In a few, we'll have kind of complete manual. :slight_smile:

https://drive.google.com/open?id=1cAlaAxA7yCMaTV4SlLBUlxvXA49OH1vI 

Feel free to contribute. I do this only for sharing purpose, on my spare time.

Remember the time you received your DieBieMS and what kind of document you'd have loved to read for helping you. ;)
```

---
## \#1068 Posted by: walleywalker Posted at: 2019-09-10T14:13:51.859Z Reads: 99

```
@JTAG Can we add a link to @pimousse's DBMS manual in the first post?
```

---
## \#1069 Posted by: JTAG Posted at: 2019-09-10T14:28:17.830Z Reads: 103

```
I wish I could edit that.... Forum rules don't allow me to.... We need a mod to do that.
```

---
## \#1070 Posted by: walleywalker Posted at: 2019-09-10T22:39:40.014Z Reads: 106

```
@anorak234 
@Namasaki 

Could you guys help us put the DieBieMS community User Manual into JTAG's OG post up top? 

It'll really go a long ways folks find setup, FAQ, and trouble shooting documentation. 

https://drive.google.com/file/d/1cAlaAxA7yCMaTV4SlLBUlxvXA49OH1vI/view
```

---
## \#1071 Posted by: drbauer03 Posted at: 2019-09-15T08:15:16.781Z Reads: 109

```
Hi, my BMS just arrived and it looks nice and everything but it won't connect to the BMS tool saying it can't get the firmware version. On the screen it shows a crossed-out battery and then "bye" no matter if the balance connector is plugged in or not. I've read about the R55 being faulty and I checked mine and to my surprise, there's not an 15R0 (15 ohm) resistor but an 10R0 (10 ohm). I have the 0.9 version of the BMS and I checked some photos online and it seems every other board has a 15 ohm one. Can changing that resistor be the solution for my struggles?
![Screenshot_20190915-095621_Gallery|281x500](upload://hIdWGkjQsVL1zEp2KKSNjSuhJ6I.jpeg)
```

---
## \#1072 Posted by: drbauer03 Posted at: 2019-09-15T08:25:05.314Z Reads: 106

```
Okay so I dont get it now :smile: 
Tried to connect (just for fun) and it connected and voltage readings seem okay
```

---
## \#1073 Posted by: bsancken Posted at: 2019-09-16T03:55:03.877Z Reads: 108

```
Make sure it has atleast 12v on the Batt posts for it to "power up"
```

---
## \#1074 Posted by: Xenon Posted at: 2019-09-16T11:28:53.072Z Reads: 104

```
i got also the v.0.9 and it work for weeks yesterday no boot up no usb connection display black..... 
now i solder a 15Ohm resistor and it runs again
```

---
## \#1075 Posted by: Prism Posted at: 2019-09-17T14:52:57.776Z Reads: 100

```
hey @JTAG what would happen if the SOC and the actual charge of the battery don't match and the SOC reaches 0%? Does that affect the output in any way. Or is it purely for the display?
```

---
## \#1076 Posted by: rene Posted at: 2019-09-17T18:11:59.267Z Reads: 105

```
@JTAG - I made a stupid mistake:
I disconnected a cable from the common ground port and it hit somewhere around the balacing resistors.

Now I see this:

![image|562x500](upload://kMUwrA2Tlq5naetiAXhPP2PAmJX.png) 

Is there a way to repair?
```

---
## \#1077 Posted by: JTAG Posted at: 2019-09-17T19:44:03.567Z Reads: 99

```
One of your 100 ohm resistors is blown, try to replace it and check whether anything else gets warm. The LTC seem to have survived 🤐.
```

---
## \#1078 Posted by: JTAG Posted at: 2019-09-17T19:44:55.449Z Reads: 96

```
No the SoC is just a calculation which is used to inform the user, nothing gets done with the information for the control of other things
```

---
## \#1079 Posted by: rene Posted at: 2019-09-18T09:49:14.323Z Reads: 101

```
Sorry to ask, but whats the exact name of this resistor and where best to buy it in europe (I am from Hamburg / Germany)?
```

---
## \#1080 Posted by: Prism Posted at: 2019-09-18T15:17:41.501Z Reads: 102

```
I've seen a fault like that before. Had one of my balance leads make intermittent contact and when I wiggled it around I had one cell go over 5V and the one below it at like 3V. 

I assume you mean this resistor @JTAG?
![resistor|690x74](upload://5flB4MPc6QjAM0YmL7oLWbRVEKD.png) 
![ksdgfjhs|690x371,75%](upload://i3KNW0dEsW9YaDFgmoyCjmv0Qye.png)  

Look at places like reichelt or conrad @rene search for 100 ohm 0603 resistors.
```

---
## \#1081 Posted by: drdrs Posted at: 2019-09-21T20:02:45.324Z Reads: 101

```
I'm trying to communicate with my DBMS using the DBMS tool through the DBMS CAN port with a CANable USB to CAN adaptor device (https://canable.io) .  The CANable device is visible on my Mac as a TTY device but it does not show up in the "Port" dropdown menu of the "(USB-)CAN" tab of the "Connection" menu of the DBMS tool.  I'm able to connect to the DBMS with the DBMS tool using USB.

Is there some setting or driver I should use so that the DBMS tool recognizes the adaptor or is this not a use case that the DBMS tool is designed for?
```

---
## \#1082 Posted by: bsancken Posted at: 2019-09-22T01:20:47.050Z Reads: 102

```
Why not just use the usb port on the DBMS??
```

---
## \#1083 Posted by: JTAG Posted at: 2019-10-02T08:07:47.549Z Reads: 90

```
This does not work because of a protocol mismatch. At some point I wish to add support for a USB to CAN converter but did not yet came around to build that ....
```

---
## \#1084 Posted by: banjaxxed Posted at: 2019-10-07T08:46:43.339Z Reads: 86

```
[quote="Samau18, post:351, topic:2639, full:true"]
I preflashed it already. If you want to you can use jlink or stlink to flash it again.
[/quote]

Hi Samau, any chance you or @JTAG or @fedestanco could share the ST-Link method to flash?

I have one which is not registering  as a USB device, I have a second which registers fine, same cable, same computer, same physical usb port. It was working until a massive ESC short took out one of my controllers (small explosion inside an aluminium case), I'm guessing it caused some f/w corruption when it blew..I think.

Anyway I think trying to flash via this port makes a good first check..but open to to other suggestions.

Thanks for ideas!
```

---
## \#1085 Posted by: Samau18 Posted at: 2019-10-07T09:50:59.980Z Reads: 88

```
A bit confused.  So you have one that can’t load up the usb drives after the esc short?  That one please sent it back. We can fix it if traces are not damaged . 

The one with usb driver you can just get st flashing utility and get it flashed.  Need testing tho.  Don’t have specific instructions.
```

---
## \#1086 Posted by: banjaxxed Posted at: 2019-10-07T09:54:31.517Z Reads: 86

```
thanks, it's from fedestanco's batch, I was just picking the community's collective mind. I'll try the STLink  approach. Just flash the f/w and see if it helps..maybe it's more busted then that, I also saw a post above for testing usb voltage, may try that
```

---
## \#1087 Posted by: drdrs Posted at: 2019-10-08T03:18:33.202Z Reads: 87

```
Good to know.  I'm able to send my own bytes to the BMS over UART to COMM_GET_VALUES and COMM_GET_BMS_CELLS and and I'll start working on direct CAN access next after I grok CAN_PACKET_PROCESS_RX_BUFFER, etc...
```

---
## \#1088 Posted by: drdrs Posted at: 2019-10-08T03:22:55.391Z Reads: 89

```
I have a similar problem.  I have one BMS that I can communicate with over USB but second brand new and unused (GB3) one where the USB does not show up as a port in the DBMS-tool with the same computer and cable.

I've checked R55 is 15 ohms and the 3V3 rail (tested between USB connector and pin 1 of the CAN chip) reads 3.24V.

I think I may have two problems.  The USB transceiver might be down and since this DBMS is on the bench with only a power supply and no individual cell voltage harness, I might be getting a low cell voltage shutdown.
```

---
## \#1089 Posted by: banjaxxed Posted at: 2019-10-08T16:10:02.731Z Reads: 88

```
Damned if I know! sorry
```

---
## \#1090 Posted by: drdrs Posted at: 2019-10-10T05:06:16.626Z Reads: 88

```
I don't know how to make CAN requests yet, but I've been able to connect the VESC and DBMS on a CAN bus, set both to emit status over CAN and read and filter the frames using the python canard library and the canable USB-CAN device.  Next step will be to use an arduino CAN controller to filter the frames for a display.
```

---
## \#1091 Posted by: drdrs Posted at: 2019-10-10T05:12:53.960Z Reads: 88

```
For the USB-CAN stuff, there may be some work you can leverage from the Axiom folks.

https://hackaday.io/project/164932-axiom-100kw-motor-controller/log/165890-new-feature-gui-canbus-support
```

---
## \#1092 Posted by: PatRocks Posted at: 2019-10-24T22:10:28.115Z Reads: 81

```
@janpom do you have a link for that specific resistor? does anything besides the 15Ohm metric matter? thin/thick film resistor? there's so many 15ohm resistors on mouser... Thanks alot!!
```

---
## \#1093 Posted by: janpom Posted at: 2019-10-25T07:18:54.123Z Reads: 81

```
IIRC, I purchased this one: https://www.gme.cz/r0805-15r-1-yageo

I'm by far not an expert but I'd assume that pretty much any 15 Ohm resistor will do.

[Here's](https://www.electric-skateboard.builders/t/diy-6s-to-12s-bms-with-can-diebiems/2639/958?u=janpom) what I have done initially. I soldered on 10 Ohm THT resistor since that was the closest thing I had on hand. It worked just fine.
```

---
## \#1094 Posted by: PatRocks Posted at: 2019-10-25T16:48:10.051Z Reads: 81

```
Genuinely appreciated my friend!!
```

---
## \#1095 Posted by: drbauer03 Posted at: 2019-10-28T16:02:15.314Z Reads: 84

```
Hi @JTAG,
I´ve read about people dropping things onto the balancing part of the BMS.
The same thing happened to me but I thought the balance leads weren´t connected. (they probably were)
My cell readings are looking like this now:
![aaasas|690x393](upload://jFYnw1HUc0kR7R8PQkx9gotzdDX.png)  

:((((
What components do I have to check or is there any chance that the LTC has survived? If I change out the LTC would it work right away or something more is needed?
```

---
## \#1096 Posted by: JTAG Posted at: 2019-10-28T16:39:15.678Z Reads: 84

```
Happens to the best! 

Without any power to the board evaluate whether all tracks are still intact ( also look at the bottom ), look whether the smal pcb fuses are still in tact (RED):
![image|690x362](upload://pKMHmWhG8fxH4ppf6ZnAKVpDeZS.png) 

Also measure all 12 resistors in the blue circle ( they should measure 100Ohm ).

Also measure all 12 resistors in the Yellow circle ( they should measure 3300Ohm ).

When a pack is connected (to the balance port and main PACK+ and - ) evaluate whether anything gets warm when the BMS is off. ( this should not be the the case ).
```

---
## \#1097 Posted by: drbauer03 Posted at: 2019-10-29T18:34:29.382Z Reads: 84

```
Okay, so I did everything you told me and all the PCB tracks are okay and those fuses as well
...measured all the resistors and everything seems fine

When I connect the pack to the BMS, the area on the picture from you gets warm (around those circeled resistors) 

..so what to do next?
```

---
## \#1098 Posted by: drbauer03 Posted at: 2019-10-30T10:31:03.196Z Reads: 82

```
@JTAG Is it possible to somehow measure if those SMD transistors are okay?
```

---
## \#1099 Posted by: drdrs Posted at: 2019-10-31T03:49:34.190Z Reads: 85

```
Folks,

I've put together a troubleshooting document that tries to spell out symptoms and also references posts that demonstrate the problem and fixes.

https://github.com/dsoto/DieBieMS-Manual/blob/master/troubleshooting.md

I'll continue to add to it and I welcome pull requests.
```

---
## \#1100 Posted by: JTAG Posted at: 2019-10-31T10:56:32.740Z Reads: 80

```
Well, if the big resistor heats up either the FET is faulty or the LTC tells it to enable. The part is a TSM2323.

Remove all power to the BMS and measure resistance between the drain and source of the transistor, the resistance should be high.

When it is and you want to confirm that the transistor is being asked to turn on. Connect the battery to the BMS but leave the BMS off. Now measure the transistor next to the resistor that is heating up and measure between gate and source. the voltage should be close to zero.
```

---
## \#1101 Posted by: Darkie02 Posted at: 2019-11-06T23:36:11.627Z Reads: 75

```
so finished wiring up a DieBiems today.

what should happen the pushing the NO momentary switch?

so fare id I connect a USB a green led flashes momentarily in the middle of the board

if no usb is connected a green LED in the middle of the board flashes brightly at the start of a power button bee pressed (this stops happening as soon as a USB is attached)

tried installing 2104 drivers on my Mac but this had no effect

can't connect the DieBieMS tool and stuck for any thing els to try 5 hours later. any one got any suggestions to any thing to try?
```

---
## \#1102 Posted by: JTAG Posted at: 2019-11-07T10:40:25.010Z Reads: 76

```
When the USB is inserted the power LED should come on and stay on, the status LED might die if the pack config is not correct yet. 

When a USB is inserted you should see a COM / serial power in your device list ( not sure how that works on mac but probably similar to windows ). If not please install the CP2104 drivers ( that is the USB serial chip on the BMS ). 

When you are at this you should be able to connect, if not report back and we will try to resolve!
```

---
## \#1103 Posted by: Darkie02 Posted at: 2019-11-08T07:50:06.259Z Reads: 73

```
So I swoped our the DieBieMS and I had the constant led seems the 1st one is faulty som how 

I did need to install the CP210X USB-UART drivers befor it would conect

What I’m a little confused about is if I write the config it works untill you power off the unit then it reverts back to default on power up.

If I click the save icon it seems to remember the settings after power down is this correct?
```

---
## \#1104 Posted by: JTAG Posted at: 2019-11-08T08:33:53.807Z Reads: 71

```
[quote="Darkie02, post:1103, topic:2639"]
If I click the save icon it seems to remember the settings after power down is this correct?
[/quote]

Yes the storing of a config is a two stage approach.

1. Put the configuration from the tool in the BMS - Volatile memory
2. Store the configuration from the volatile in the flash non volatile memory

This is because of for example the following scenario:
You have your BMS already operational ( configured correctly and the BMS is happy ) and build into an enclosure where the usb port is unavailable ( the USB port is key here because that is the only interface to program trough that forces the BMS on ). You are connected with the BMS tool trough passtrough trough an ESC or bluetooth module, you change a setting which make the BMS think something is wrong and instantly the power to the esc stops and the BMS turns off. If the settings written to the BMS were non-volatile you will have had to open the enclosure to dig to the USB connector of the BMS to restore the operation, Now in with the 2 step storage approach you just re-enable the battery/BMS ( you first apply and verify, then make it final by storing the config ), the known working config is retrieved and used and you are good for another try of configuring the BMS.
```

---
## \#1105 Posted by: PatRocks Posted at: 2019-11-14T02:31:11.539Z Reads: 69

```
@JTAG / @Giga am I dumb, or is it impossible to find a slow-blow 1206 fuse? even checked the farnell site and the me-being-dumb evidence seems to be mounting... Dearest Danny, will a fast-blow fuse work? thanks for the help every/any one
```

---
## \#1107 Posted by: Giga Posted at: 2019-11-14T17:43:42.293Z Reads: 70

```
[quote="JTAG, post:849, topic:2639, full:true"]
this one is not critical, take 500mA if you want! It is just to protect the traces from burning when something is connected wrong or partially. Pleae also check the resistor next to it!
[/quote]
FYI


It got replaced by the same again and it holds up since.
But [this](https://octopart.com/0468.500nr-littelfuse-672821?r=sp&s=eXXNvv2USK-ALBIvVJT5EA) would be a 0.5A Slow blow.
```

---
## \#1108 Posted by: Chricious Posted at: 2019-11-14T22:58:49.459Z Reads: 67

```
Hi Danny,

@Darkie02 drew attention to the 70A fuse trigger on the BMS and he said that it could limit our 12S12P configuration and create a bottle neck. We didn't experienced such a thing so far, but I want to check with you to get sure.
```

---
## \#1109 Posted by: PatRocks Posted at: 2019-11-15T05:41:11.972Z Reads: 71

```
Well, i f*cked it up:
![20191114_191138|666x500](upload://40JorqxWO5nbxGpOuBm19J9kHag.jpeg)  
Anyone think this is salvageable? Pads are gone, i don't know if there's any way to fix it?
![20191114_191123|666x500](upload://a5rTUPp3ubtdJ5Y8BeOR85rjiFb.jpeg)
```

---
## \#1110 Posted by: Prism Posted at: 2019-11-15T23:10:26.917Z Reads: 74

```
Depends on how good you are with soldering small stuff. 

This is how I would fix it:
![fix|690x476](upload://bpvxAriEUuG23GbJENELiEXDgNz.jpeg) 
solder the resistor directly to the fuse and jump the other side with a small piece of wire to the trace that was connecting the pad to the via.
```

---
## \#1111 Posted by: SZapatero Posted at: 2019-11-21T15:58:06.926Z Reads: 71

```
Hi Danny,

I recently bought some DieBieMS in order to use them for an electric bike project.
I've been able to interface all of them and connect them to the 12S batteries that I built for them.
Unfortunately, there is one of them which I'm not able to make work.

I could connect to it via USB and I was able to make it work with the battery, but one day it suddently
stopped detecting the battery cells, and no matter what I configure, the screen just shows the symbol
with the battery crossed out. The software also lets me configure the parameters but won't show any 
level for any battery.

It looks as if some hardware component has stopped working, but the microcontroller is still working.
I know that the battery is working because it is recognised by other DieBieMS. I've also tried to reflash
the board but nothing changes.

Have you ever experienced this? Is there an obvious thing I could try?

Thank you in advance for the support. It's a great project.
```

---
## \#1112 Posted by: Trdolan03 Posted at: 2019-11-28T06:06:33.705Z Reads: 67

```
Is there a production run going on right now or any for sale?
```

---
## \#1113 Posted by: drdrs Posted at: 2019-11-28T17:26:11.769Z Reads: 72

```
According to the DieBieMS v0.8 Batch 3 thread, they sold out in mid-October and don't have a date set for Batch 4.  You might be able to find some second-hand.
```

---
## \#1114 Posted by: rpasichnyk Posted at: 2019-11-29T09:41:13.684Z Reads: 70

```
I finally added support for DieBieMS configuration to Metr app, so you can change all parameters on the go. At the moment only FW0.27 is supported

https://media.giphy.com/media/fuVCNbEX5QrSEahxJV/giphy.gif

@JTAG while I was doing it I noticed there is a mismatch between DieBieMS-Tool and DieBieMS-Firmware. I used branch `efoildevelop` in both repos, but it turned out that these parameters are not present in FW0.27

```
packVoltageDataSource
emitStatusProtocol
HCLoadVoltageDataSource
HCLoadCurrentDataSource
DCDCTargetVoltage
```
However they are present in the `efoildevelop` branch in `DieBieMS-Firmware.git`. I decided to go with the binary included in DieBieMS-Tool instead and not include these parameters. So it all seemed to work out but I was a little confused :blush:

I noticed you have another branch `solardevelop`, which is great, new features :smiley: I wonder if you maybe have time at some point to merge everything in master and make a new release? :grimacing:
```

---
## \#1115 Posted by: JTAG Posted at: 2019-11-29T10:42:39.609Z Reads: 70

```
Wwwoooowwww this is awesome!

Yes yes I know I need to iron out many things..... I am very sorry for the confusion :frowning: . There is so much happening; A solar car drove with a battery of which the firmware was based on the DieBieMS and multiple eFoils are working with it and many features are build for those applications where we all might benefit from. 

I also do some engineering for other companies who made me work with USB PD a lot and one for which we developed fast electrical fusing ( so fast that it is self recovering from a short ). The biggest challenge is to merge all developments in one firmware that supports all the different hardware.
```

---
## \#1116 Posted by: Eretron Posted at: 2019-12-05T09:43:32.978Z Reads: 67

```
Just got diebiems working 💪💪💪. One question though, is there a way to limit charging current? 

Thanks in advance.
```

---
## \#1117 Posted by: Nisse977 Posted at: 2019-12-05T12:21:09.674Z Reads: 67

```
Nice work!!!

I got my DieBieMS a few weeks ago, but I am not gona install it until next year in a new batterybuild. Looking forward to that :)
```

---
## \#1118 Posted by: webst Posted at: 2019-12-08T06:04:45.408Z Reads: 65

```
Smaller charger / smaller regen limit
```

---
## \#1119 Posted by: JanMrlth Posted at: 2019-12-11T22:23:55.178Z Reads: 58

```
Hi Danny, 

thank you for your design! I have ordered 3 v0.9 PCBs at asiler and want to build them between the years. 
Is there any chance you could help me to find some replacement parts. Seems that some parts of the provided BOM are out of stock at farnell. 

Thanks a lot! 

Jan
```

---
## \#1120 Posted by: trainingforutopia Posted at: 2020-01-03T07:51:26.800Z Reads: 39

```
Hi Danny, 

I am looking for a DieBieMS, as I have a DaveGA X incoming and I am really excited to see how it now even integrates with mere. Thank you for your hard work!
Is there a new batch coming where I could join?

Thank you!

PS, are you on the other side? This forum has been down too often lately.
```

---
