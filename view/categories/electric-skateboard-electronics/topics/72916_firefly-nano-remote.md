# Firefly Nano remote

### Replies: 579 Views: 18369

## \#1 Posted by: DroidSector Posted at: 2018-10-31T14:29:45.580Z Reads: 1136

```
First I'd like to thank SolidGeek for his great [Firefly remote](https://www.electric-skateboard.builders/t/simple-3d-printed-nrf-remote-arduino-controlled/28543) and all the people in that thread for providing tons of useful information. When I printed the remote, it felt kind of big for my hand since I got used to Ownboard/WowGo remote. So I decided to design a smaller version around Feather M0 RFM69 board. _Update: Heltec v2 with the same built-in screen is also suitable, I'm currently re-designing remote to accommodate this board._

Changes:

* Bigger battery, up to 1000mAh.
* Bigger screen (128x64). Allows seeing speed, distance, battery, and distance at once.
* Second page shows throttle, motor amps, and battery amps.
* [Smaller size](https://www.electric-skateboard.builders/t/firefly-nano-remote/72916/27), same as Ownboard/WowGo remotes.
* Instant on, deep sleep mode with the idle timer.
* One remote can be used with multiple boards.
* Board ID is generated from chip ID / MAC address.
* Vibration motor for disconnection alert.
* Fewer components (easier to solder but more expensive)
* Settings menu: 
  * Remote calibration
  * Remote settings (coming soon)
  * Board configuration (coming soon)

Source code: [github.com/DroidSector/RF69-Esk8-Remote](https://github.com/DroidSector/RF69-Esk8-Remote)
Parts list: [docs.google.com/spreadsheets/d/13rUPX8BsSac...](https://docs.google.com/spreadsheets/d/13rUPX8BsSac1AdnFAXx4dwR3XoQiU4FAKbunFaeW-oY/edit?usp=sharing)

https://www.thingiverse.com/thing:3185093

![remote|676x500](upload://lcrsgjp2iAo5dpDLNJJRb78Z3f9.jpeg) 

In the bottom half of the remote, there is room for a 51x34x6mm battery. Simply connect a 4.2/3.7V Lipo or LiIon battery to the JST jack. When the USB power is powered, Feather will automatically switch over to USB for power, as well as start charging the battery at 100mA.

![electronics_schematic_remote|690x487](upload://t6zpPX8tl83VOYTTOJrxtbWujXz.jpeg) 

I've tested the receiver with Flipsky Dual ESC 4.20 and it's working without a logic level converter.
![electronics_schematic_receiver|690x487](upload://u8dqqWvmxUXOMuJVs42RMjCeipF.png)
```

---
## \#2 Posted by: Tomer Posted at: 2018-10-31T14:31:25.471Z Reads: 935

```
What a slik looking remote!
```

---
## \#3 Posted by: brenternet Posted at: 2018-10-31T14:38:08.954Z Reads: 923

```
Amazing work!
```

---
## \#4 Posted by: nuttyjeff Posted at: 2018-10-31T14:44:20.070Z Reads: 914

```
love it!       .
```

---
## \#5 Posted by: tsr Posted at: 2018-10-31T14:54:24.625Z Reads: 901

```
Nice one! Could you also provide the step files for the printed parts?
```

---
## \#6 Posted by: StefanMe Posted at: 2018-10-31T16:09:58.880Z Reads: 869

```
I am confused. U are talking about sending every 50ms data to the reciever, but don’t include there refreshing display and getting UART Data...
What is your total cycle time between one and another transmission in worst case? If u have Refresh the display AND getting UART data?

Some more thoughts:

- u use only one encryption key?! No automatic generated encryption key for each user? No ID for the board handling? U just use one default keys in one remote with all the same boards?SUPER DANGEROUS! U cannot trust people changing this manually.

- u have absolute no menu? Nothing to reset or set any values? Nothing to store or restore?

Sorry but this code is definitely not ready to release ;) there are many things inside u need to rework urgently!

I CANNOT SEE ANY WARNING THAT THIS CODE IS DEFINTY IN A SUPER UNSAFE AND ERALY STATE AND NOT FOR DAYLY USE. My code is much further and I ll still not comfortable to release it...

But of course. Still great work. But the way how I released it is not ok. Please overthink this. The remote is a fucking important safety feature...
```

---
## \#7 Posted by: DroidSector Posted at: 2018-10-31T19:05:18.800Z Reads: 787

```
[quote="StefanMe, post:6, topic:72916"]
I am confused. U are talking about sending every 50ms data to the reciever, but don’t include there refreshing display and getting UART Data…
What is your total cycle time between one and another transmission in worst case? If u have Refresh the display AND getting UART data?
[/quote]
I didn't measure it yet, but response feels on par with other "dumb" remotes. I didn't include duration into frequency. That 50 ms comes from this line of SolidGeek's code:

> if ( millis() - lastTransmission >= 50 )

Getting UART data happens only 4 times per second and potentially while waiting for the next packet of data. I've separated drawing and sending buffer to the screen since there is no point of redrawing the same data every 50ms. So, I think the probability of these operations happening at the same time is rather low, but of course, there should be a more optimal way (timers?).

[quote="StefanMe, post:6, topic:72916"]
* u use only one encryption key?! No automatic generated encryption key for each user? No ID for the board handling? U just use one default keys in one remote with all the same boards?SUPER DANGEROUS! U cannot trust people changing this manually.
[/quote]
I've just removed the default key, now a new random key had to be included to compile the code. Will implement menus and pairing soon, probably before anyone builds this remote :slight_smile:  

I don't agree that it's "super unsafe", there were no delays or disconnections during my testing (~50 km, up to 40 km/h). But early state for sure :slight_smile:
```

---
## \#8 Posted by: ElectricCoast Posted at: 2018-10-31T21:09:56.350Z Reads: 687

```
Excellent work
```

---
## \#9 Posted by: Livid Posted at: 2018-10-31T22:09:56.102Z Reads: 680

```
I like this very much, might build another firefly remote if i cant iron out the problems with my current one
```

---
## \#10 Posted by: solidgeek Posted at: 2018-10-31T22:35:31.035Z Reads: 664

```
Love the graphical interface, looks sleek ;)
```

---
## \#11 Posted by: Jinra Posted at: 2018-10-31T23:28:03.256Z Reads: 674

```
Anyone know where to get the switch nowadays? It seems to be a discontinued product.
```

---
## \#12 Posted by: neiru37 Posted at: 2018-11-01T00:07:05.248Z Reads: 670

```
I have a few with me, want me to bring them this saturday?
```

---
## \#13 Posted by: lrdesigns Posted at: 2018-11-01T00:46:09.872Z Reads: 684

```
The physical design of the remote is REALLY nice! Nailed it. :hammer:

The radio and software aspects I am a little skeptical.
915 MHz - 7.8 cm antenna is an interesting choice, its good for going through stuff and long distances but how good is at rejecting noise? I assume that's all in software, is there any provisions for noise rejection, packet loss, error correction type stuff?

The receiver is pretty cute though :smirk:
![image|595x389](upload://wLWm3RJB2BFdrM8dXGUSou0N5kZ.jpeg)
```

---
## \#14 Posted by: dspx Posted at: 2018-11-01T01:00:16.960Z Reads: 654

```
Hmm, are they the long lever type (30mm)? I have a few of the standard switches from a previous Firefly build - I guess I could MacGyver an extension to the lever? Unless you're up to shipping some out? 🤓
```

---
## \#15 Posted by: neiru37 Posted at: 2018-11-01T01:48:27.018Z Reads: 639

```
Oh I didn't know you needed long levers. Yeah I have the same short ones, about 13mm.
```

---
## \#16 Posted by: DroidSector Posted at: 2018-11-01T02:48:41.897Z Reads: 640

```
Thanks! I'll update the code in the future to match your RemoteDisplay.cpp file, so it would be easy to change the display and use this mod, for example:

https://www.thingiverse.com/thing:3184630
```

---
## \#17 Posted by: DroidSector Posted at: 2018-11-01T03:01:50.338Z Reads: 635

```
I found that switch in Jaycar store and assumed that it would be easy to get a similar model on Aliexpress, but it's not the case. The lever size is ~17mm. 

https://www.jaycar.com.au/spdt-125v-3a-sub-miniature-micro-switch-with-lever/p/SM1036 

https://www.jaycar.com.au/medias/sys_master/images/9142685663262/SM1036-dataSheetMain.pdf
```

---
## \#18 Posted by: dspx Posted at: 2018-11-01T04:01:17.149Z Reads: 605

```
Ah, ok! The linked switch points to the 30mm variant, but that's great news lol 😌
```

---
## \#19 Posted by: DroidSector Posted at: 2018-11-01T04:32:52.659Z Reads: 634

```
The transceiver chip performs CRC check and noise filtering:

>  SX1231 packet handler performs several packet oriented tasks such as Preamble and Sync word generation, CRC calculation/check, whitening/dewhitening of data, Manchester encoding/decoding, address filtering, AES encryption/decryption, etc. This simplifies software and reduces uC overhead by performing these repetitive tasks within the RF chip itself.

> The role of the channel filter is to filter out the noise and interferers outside of the channel. Channel filtering on the SX1231 is implemented with a 16-tap Finite Impulse Response (FIR) filter, providing an outstanding Adjacent Channel Rejection performance, even for narrowband applications.

There are also different modulation types and data rates available:

> FSK_Rb2Fd5 = 0,	   ///< FSK, Whitening, Rb = 2kbs,    Fd = 5kHz
> ...
> 	FSK_Rb250Fd250,    ///< FSK, Whitening, Rb = 250kbs,  Fd = 250kHz
> 
> 	GFSK_Rb2Fd5,	    ///< GFSK, Whitening, Rb = 2kbs,    Fd = 5kHz
...
> 	GFSK_Rb250Fd250,    ///< GFSK, Whitening, Rb = 250kbs,  Fd = 250kHz
> 
> 	OOK_Rb1Bw1,         ///< OOK, Whitening, Rb = 1kbs,    Rx Bandwidth = 1kHz. 
... 
> 	OOK_Rb32Bw64,       ///< OOK, Whitening, Rb = 32kbs,   Rx Bandwidth = 64kHz.
```

---
## \#20 Posted by: Jinra Posted at: 2018-11-01T04:33:25.344Z Reads: 591

```
Oh yea that's a bit confusing. Perhaps you should change the link to the jaycar one @DroidSector
```

---
## \#21 Posted by: DroidSector Posted at: 2018-11-01T04:56:34.817Z Reads: 579

```
Updated the link for now, I'll modify the trigger design to accomodate the switch with 13mm lever, looks like there is no other differences. 

Boosted remote has an interesting solution:
![boosted|291x250](upload://524N5AVbJ1qprki0pA7CZMiZLaA.jpeg)
```

---
## \#22 Posted by: sami Posted at: 2018-11-01T09:12:57.932Z Reads: 573

```
Looks nice.. I have the parts for the firefly ready to assemble but I think I'm gonna build this one instead and sell the kit or maybe gift it in the secret santa
```

---
## \#23 Posted by: Jinra Posted at: 2018-11-01T14:04:46.618Z Reads: 585

```
Some thoughts after printing out a quick model to test hand feel

* Are the bolts supposed to self thread into the bottom case?
* The design seems to suffer from some of the ergo problems I found on the Nano X (see review [here](https://www.electric-skateboard.builders/t/nano-v2-full-review/25159)). As you can see from the pic below, my thumb resting position is well above where the wheel is. Similarly with the nano x, I have to scrunch my thumb back to get it into a position where I can use the wheel, and after riding for a while, it starts cramping my hand. However this design is still more comfortable than the nano x, so I'll probably do a trial run of a remote.
* Could you design a throttle with a little nub similarly to how the Firefly has two options for throttle.

![15410811328596672354375961572731|375x500](upload://uzKlqcfuwJZcq6SeRRC9S5T6csc.jpeg)
```

---
## \#24 Posted by: deucesdown Posted at: 2018-11-01T14:35:31.175Z Reads: 558

```
Thanks for doing this. I really like the ergos of the Ownboard remote. I'll put this on my long eskate todo list.
```

---
## \#25 Posted by: rayn Posted at: 2018-11-01T15:18:17.698Z Reads: 552

```
Very nice @DroidSector! Have you considered using any of the hardware timers via interrupt for the radio communication? I've been thinking of doing that myself but I don't know if the timers are all used up by the various libraries already. 

I also don't know if you can let minVoltage go all the way down to 3.1v, will the feather's regulator still be able to power everything?
```

---
## \#26 Posted by: Jinra Posted at: 2018-11-01T18:21:48.125Z Reads: 551

```
For anyone looking for these super hard to find switches. It looks like Honeywell has a new model (ZX) series that's available on digikey and mouser (ZX10C30J01). It looks like for straight actuator arms they only have 13mm and 30mm now. Do you think 13mm would be too short @DroidSector? Also the ZX10C's only support 100ma of current, though I think that's a non-issue.
```

---
## \#27 Posted by: Jinra Posted at: 2018-11-02T05:12:12.239Z Reads: 558

```
Side by side 
![15411354868296311689441652260473|374x500](upload://mwTgOM2Z7T92y7dMJdRqbSS9c83.jpeg)
```

---
## \#28 Posted by: DroidSector Posted at: 2018-11-02T07:49:57.538Z Reads: 552

```
[quote="Jinra, post:23, topic:72916"]
Are the bolts supposed to self thread into the bottom case?
[/quote]
Yes, makes the assembling little easier I think.

I'm holding it a bit lower, the trigger is almost at fingertip.

I'll make a variation with a nib.
```

---
## \#29 Posted by: DroidSector Posted at: 2018-11-02T08:24:50.364Z Reads: 542

```
@rayn  yes, that would be more logical. Just did some measurements today, drawing the main screen UI takes only 15ms, but sending the buffer to the screen takes 35 ms. No tested at this voltage yet.

@Jinra I'm moving the switch to another location so it will work with 13mm arm.
```

---
## \#30 Posted by: StefanMe Posted at: 2018-11-02T10:38:21.341Z Reads: 544

```
Compare it to mine... 

https://www.thingiverse.com/thing:3191091/files
```

---
## \#31 Posted by: Bob6677 Posted at: 2018-11-02T13:48:36.775Z Reads: 531

```
Awesome. looks very good. look forward......Can this work with VESC?
```

---
## \#32 Posted by: StefanMe Posted at: 2018-11-02T14:01:02.530Z Reads: 524

```
Yes, they will all work with VESC and FOCBOX
```

---
## \#33 Posted by: Bob6677 Posted at: 2018-11-02T14:06:05.774Z Reads: 510

```
Great!!!!!!!! 
Why not to open mold?
```

---
## \#34 Posted by: PickSix24 Posted at: 2018-11-02T14:09:14.992Z Reads: 503

```
Am I correct that I need two of the feather boards ? One as a Rx and one as Tx
```

---
## \#35 Posted by: dspx Posted at: 2018-11-02T14:12:06.877Z Reads: 516

```
For now, yes, but it looks like he's testing a cheaper alternative with a nano + transceiver module.
```

---
## \#36 Posted by: DroidSector Posted at: 2018-11-02T15:30:51.510Z Reads: 521

```
Yes, also just got these TTGO LoRa32 modules, $15 including the same OLED screen:
![IMG_20181102_152441|690x398](upload://kMZCIkLGdgQpeavCU0xLURfSTUB.jpeg)
```

---
## \#37 Posted by: StefanMe Posted at: 2018-11-02T15:38:50.058Z Reads: 525

```
I think they ll be an perfect alternativ part for the expensive Feathers... but probably not the LoRa version. Is there a normal HCW Version available?
```

---
## \#38 Posted by: DroidSector Posted at: 2018-11-04T05:06:17.036Z Reads: 521

```
Just tested the transmission speed, it was around 100 ms in default mode but dropped to 11ms after setting this modem configuration:

> Bw500Cr45Sf128: Bw = 500 kHz, Cr = 4/5, Sf = 128chips/symbol, CRC on. Fast+short range.

Not as good as RF69 (2 ms), but still ok. The SX1276 chip itself supports faster FSK modulation, but it's not supported yet by RadioHead library. I'll build a new remote with this board and test it in real life conditions next week.

Big thanks to @Fabialbo for recommending this board.
```

---
## \#39 Posted by: StefanMe Posted at: 2018-11-04T13:54:32.779Z Reads: 501

```
Build in an counter for failed transmission ect. Would be interesting how stable the connection is... 

I have an debug screen where I show RSSI, longest cycle time since remote switched on and how many lost transmissions. That’s the best way how to check stability in real world.
```

---
## \#40 Posted by: StefanMe Posted at: 2018-11-04T17:10:53.696Z Reads: 529

```
Here I count a few data on extra sites... 

This one is just real-time data. 
-RSSI
-transmission and receive time for ALL data
-TOTAL cycle Time 
![image|375x500](upload://crWrao4ABWst5ELrSTBWDf9ea49.jpeg) 
-Maximum Cycle Time including failed transmissions
-failed transmissions
-Cycle time
![image|375x500](upload://rXRaUjqabGaKsPHcE17CahwlYp.jpeg)
```

---
## \#41 Posted by: DroidSector Posted at: 2018-11-05T09:00:12.836Z Reads: 510

```
I've updated stl files and the parts list with the same switch as in Firefly remote. Also added a small nib as an option. No need to re-print the bottom part, just fix the switch in the new location with some hot glue.
![switch|690x437](upload://wUjvoKeftxPg2lUNd80xk4LCdz2.jpeg)
```

---
## \#42 Posted by: Jinra Posted at: 2018-11-05T16:33:17.715Z Reads: 497

```
I already bought the extended lever switches but I'll just snip it off, thanks for the nib! 😅
```

---
## \#43 Posted by: Jinra Posted at: 2018-11-05T18:53:47.717Z Reads: 497

```
https://www.mouser.com/ProductDetail/Honeywell/ZX10C30C01?qs=sGAEpiMZZMumBvQ1hY%2ffBe344fzIDDqEwKvXjvX1TKY%3d

Standard lever switch from mouser for anyone who needs it
```

---
## \#44 Posted by: StefanMe Posted at: 2018-11-05T20:08:47.558Z Reads: 483

```
I don’t know what u mean when u say they are hard to find... just search for „Mirco Switch“ u ll find tons of these on eBay...
```

---
## \#45 Posted by: Jinra Posted at: 2018-11-05T20:09:22.597Z Reads: 482

```
i meant the long lever arm version was hard to find. Standard arm is a dime a dozen.
```

---
## \#46 Posted by: StefanMe Posted at: 2018-11-05T20:10:34.409Z Reads: 477

```
Ahhhh ok, now I understand ;)
```

---
## \#47 Posted by: PickSix24 Posted at: 2018-11-05T22:17:01.881Z Reads: 473

```
Where can I find th anntena that’s noted in the parts list
```

---
## \#48 Posted by: Jinra Posted at: 2018-11-05T22:52:21.600Z Reads: 471

```
You can just solder a piece of wire to the antenna pinout. If you want a bigger antenna, you can solder this to it instead https://www.adafruit.com/product/1661 and get a larger antenna for it
```

---
## \#49 Posted by: PickSix24 Posted at: 2018-11-05T23:59:28.338Z Reads: 479

```
Wonder if this would work , I’ve got these from FPV flying lying around 
https://www.googleadservices.com/pagead/aclk?sa=L&ai=DChcSEwjnqe6_ur7eAhUJiH4KHfUoB3YYABAbGgJwYw&ohost=www.google.com&cid=CAESQOD2K_l19ooxss5pv6QpXV70XFCedS_izves56it0xRDQeUkwK0KWxkiDhzwH5jhTvBi2oeHAWvhe8bZm3UB9WQ&sig=AOD64_3muXtnCkCjtO1L4_syJ6Y3En-bMQ&ctype=5&q=&ved=0ahUKEwjVmue_ur7eAhWDHTQIHbc5D9wQwg8IKw&adurl=
```

---
## \#50 Posted by: DroidSector Posted at: 2018-11-06T01:44:30.519Z Reads: 469

```
Sure, both Feather and TTGO boards operate on 915 Mhz.
```

---
## \#51 Posted by: Devilmycry Posted at: 2018-11-06T04:02:42.445Z Reads: 464

```
Hi everyone I have a question  love the remote I use 
I just want to know if is possible for me to just add a screen for see the battery % and my speed and maybe the distance 
Some one can help me thank you
```

---
## \#52 Posted by: PickSix24 Posted at: 2018-11-06T05:37:00.655Z Reads: 459

```
What material is recommended for the 3d prints
```

---
## \#53 Posted by: StefanMe Posted at: 2018-11-06T06:17:21.525Z Reads: 460

```
Be careful! It depends on what version u have! I am in Europe, where u have to use 433Mhz instead of 915! 915Mhz is not allowed in eu without license.

For 915 MHz the length of the antenna should be exact 78mm. For 433 MHz it should be 164mm. A not drilled cooper wore is perfect. (It’s not recommend to use an normal drilled wire... works but ll decrease the transmission power)
```

---
## \#54 Posted by: StefanMe Posted at: 2018-11-06T06:18:47.455Z Reads: 447

```
Depends in what u want... PETG oder ABS should be the choice for durability
```

---
## \#55 Posted by: PickSix24 Posted at: 2018-11-06T07:00:52.137Z Reads: 446

```
Cool , I went with ABS
```

---
## \#56 Posted by: PickSix24 Posted at: 2018-11-06T07:02:07.832Z Reads: 442

```
Does anyone have a link for the 1k resistor. I did a bunch of searching but wasn’t sure I found the right one
```

---
## \#57 Posted by: StefanMe Posted at: 2018-11-06T07:23:50.491Z Reads: 466

```
https://www.ebay.de/itm/Kohleschicht-Widerstande-0-25W-5-Werte-und-Menge-WAHLBAR-5-10-50-100-Widerstand/221833069520?hash=item33a64803d0:m:mgqJj_CZGYMp6nXvl25tQ9w

Use the cheapest one u can find. 1/4 watt is enough.
```

---
## \#58 Posted by: DroidSector Posted at: 2018-11-06T07:40:15.930Z Reads: 446

```
All moving parts are attached to bolts, so PLA can be used, but it will probably crack if you drop it.
```

---
## \#59 Posted by: StefanMe Posted at: 2018-11-06T08:23:28.129Z Reads: 494

```
I work a lot at the code in secret... here is an update what i did allready :)  Give me a shout when i forgot some a feature u want ;)

Features:

- 0.96inch OLED with 128x64 with high frequently display update rate to have smooth and accurate informations (every 60ms)
- join settings menu with 5 seconds press on extra button or hold trigger on start up
- trigger can be used as DEADMAN-Switch or CUISE-Control
- vibration feature (Alarm on low battery from Board, Remote battery...)
- extra button to switch between 4 different main Screens 
  - Speed, Distance, Voltage
  - Voltage, Motor amps, Battery amps
  - DEBUG RSSI, cycle time, failed transmissions
  - alternative main screen design from  @DroidSector  
- headlight integration by pushing the extra button for 2 seconds
- over 16 updates per seconds from throttle position to PWM output (every 60ms)
- pair up to 200 boards with unique ID
  - one remote will handle all boards by selection the board ID from settings menu

Safety Features:

- RFM69 over RHReliableDatagram manager to send organized messages to addressed nodes
- automatic generated 16 bytes encryption key (15 bytes for unique key and 16th byte for board selection)
  - after first tun on from remote, it will generate a random 15 byte key
  - every new receiver can be paired from settings menu with the new key and board ID
- ESTOP automatic slow down until stop - more than 300ms no new values from remote will force the receiver into ESTOPMODE and slow down the trigger value every 50ms by 5 until it reaches 25% break trigger to stop the board safe (THIS WORKES SO GOOD :heart_eyes:)
  - ESTOP will armed automatically after first valid transmission between remote and receiver
- priority transmission handling! Deactivating display refresh and UART pull if no valid transmission is received until
  - ESTOPMODE is triggered, then display is refreshing again for analysing error
- break light integration with adaptive flash warning
  - if trigger is under middle position the break light will be bright 
  - if trigger is close to full break position the break light will flash

Upcoming features:

- different riding modes for beginners | intermediate | pros
  - trigger value will be attached to 50% | 75% | 100%
- police mode
  - Trigger value will be cut of at 25%, can be unlocked with button press combination
...

PCBs are comming on wednesday ;) 

![11|341x500](upload://5LksvoXMAW2mCQGV8khPhZLoPN0.png) 
![29|690x383](upload://v9u6xZNHr0KlI0ukGfR6uB1poZr.png)
```

---
## \#60 Posted by: rayn Posted at: 2018-11-06T12:44:03.503Z Reads: 464

```
[quote="StefanMe, post:59, topic:72916"]
ESTOP automatic slow down until stop - more than 300ms no new values from remote will force the receiver into ESTOPMODE and slow down the trigger value every 50ms by 5 until it reaches 25% break trigger to stop the board safe (THIS WORKES SO GOOD :heart_eyes:)

* ESTOP will armed automatically after first valid transmission between remote and receiver
[/quote]

This sounds really interesting, how does it recover back from ESTOPMODE?

Also maybe you should start a thread if you have something to show already.
```

---
## \#61 Posted by: StefanMe Posted at: 2018-11-06T13:18:24.979Z Reads: 456

```
Thanks,

I want to work with @DroidSector together... we ll decide this in the next days. He is more the good designer than me. Awesome remote design. I am more focused on stability and functions.

The ESTOP workes perfect for me. Never had any fault. Scary to switch off the remote while driving full speed ;) At the moment u have to switch off and on the board again. But i ll implement an option where u can recover from ESTOP (UART must send good values || RMP == 0 for 3 seconds || 10 good tranmissions with trigger at full break... ) something like this.
```

---
## \#62 Posted by: Silverline Posted at: 2018-11-06T19:49:09.637Z Reads: 456

```
Love your projekt. But holding it, this way, feels more natural to me.
![IMG_20181106_204520|690x388](upload://4IkzOoZUsLsECltEiJMWqWKik9D.jpeg)
```

---
## \#63 Posted by: rey8801 Posted at: 2018-11-06T19:57:54.114Z Reads: 457

```
You should also try it with the thumb wheel because in my case is what makes the standard firefly a bit on the over size for me. On this remote the range of motion of the wheel is a thing, which is great for the smooth throttle, but you need to extend you thumb quite a lot. If you hold it as you do, you could feel not comfortable on full accellaretion. Just my two cents :slight_smile:
```

---
## \#64 Posted by: PickSix24 Posted at: 2018-11-07T01:03:59.060Z Reads: 436

```
Got all my parts ordered yesterday. Now just have to be patient.... Most of the US based stuff has already shipped :)
```

---
## \#65 Posted by: fedestanco Posted at: 2018-11-08T17:35:54.563Z Reads: 426

```
Have you thought about implementing FHSS (frequency hopping)? Probably not 100% necessary but it'd be a nice addition to the new safety features that you added.
```

---
## \#67 Posted by: StefanMe Posted at: 2018-11-08T18:12:12.304Z Reads: 419

```
Fmdjjcvhmcfjmvffrjkvsskcsfjb


Hmm... for what safety reason exactly? I always open for new ideas like this! Can u explain it in more detail?

I allready got the addresses messages ID with 16 byte encryption key... I think this is more safe then every other remote at the moment.
```

---
## \#68 Posted by: fedestanco Posted at: 2018-11-08T20:15:17.831Z Reads: 426

```
Basically frequency hopping is a software trickery that allows the receiver and the emitter to synchronously "hop" between  subfrequencies (for example the 2.4ghz spectrum allows about 100 subfrequencies) tens of times per second.  

The main benefits are 1) the probability of 2 devices transmitting on the same set of frequencies is super low; thus even if one freq. is very crowded and packets fail to transmit, there is no problem since the next few milliseconds a new packet will be sent on the next freq.
2) it offers a somewhat second layer of data security: the potential hacker has to know when to hop and to which freq. to read the message you are transferring. 

The main programming challenges are: 1)receiver and transmitter have to be synchronized with an error margin of few milliseconds. This could be achieved for example by including in the packets a clock info (adjusted for transmission delay);
2)if you want to have a new set of subfreq. on each reset (for further security) receiver and transmitter have to agree on that too.
```

---
## \#69 Posted by: lrdesigns Posted at: 2018-11-09T00:42:59.504Z Reads: 404

```
This feature would be a huge win for any esk8 remote! I really don't know how easy it is to run that on arduino type hardwares? I hope someone can figure it out.

I use the GT2B because of this feature. Coming from the RC model world frequency hopping gives you a rock solid connection even in very noisy environments.
```

---
## \#70 Posted by: DroidSector Posted at: 2018-11-09T01:15:38.232Z Reads: 426

```
LoRa 32 uses similar technology:

> Chirp Spread Spectrum was developed for radar applications in the 1940’s. Traditionally used in a number of military and secure communications applications; over the past twenty years this modulation technique has seen increased adoption in a number of data communications applications due to its relatively low transmission power requirements and inherent robustness from channel degradation mechanisms such as multipath, fading, Doppler and in-band jamming interferers.

> In LoRa modulation the spreading of the spectrum is achieved by generating a chirp signal that continuously varies in frequency. An advantage of this method is that timing and frequency offsets between transmitter and receiver are equivalent, greatly reducing the complexity of the receiver design.

> LoRa modulation is both bandwidth and frequency scalable. It can be used for both narrowband frequency hopping and wideband direct sequence applications. Unlike existing narrowband or wideband modulation schemes, LoRa can be easily adapted for either mode of operation with only a few simple configuration register changes. 

https://www.semtech.com/uploads/documents/an1200.22.pdf
```

---
## \#71 Posted by: lrdesigns Posted at: 2018-11-09T01:47:26.102Z Reads: 406

```
COOL! :sunglasses: That pdf has a lot of interesting info. 

Is that LORA32 module a usable alternative to the Feather?
```

---
## \#72 Posted by: DroidSector Posted at: 2018-11-09T01:56:37.995Z Reads: 402

```
I'll try to solder and take it for a test ride today. Radio transmission takes more time but should be more resistant to interference.
```

---
## \#73 Posted by: DroidSector Posted at: 2018-11-09T16:05:53.133Z Reads: 405

```
The new remote mostly works, but likes to reboot by itself so much :angry: Some kind of conflict between radio and display libraries. Migrated to AdaFruit display library and now it's more stable, more FPS as well. This ESP32 board also has more sensitive inputs, due to 12-bit ADC I think. Overall, it's harder to develop for, but has greater potential.
```

---
## \#74 Posted by: dspx Posted at: 2018-11-09T17:00:56.575Z Reads: 395

```
Are these results while using the TTGO LORA32? 
I decided to go with adafruit for the receiver, will you continue to support that (in as far as you are able to, I mean :smile:)
```

---
## \#75 Posted by: DroidSector Posted at: 2018-11-10T03:10:01.988Z Reads: 379

```
Yes. I'll continue to test and support all suitable boards. They all use the same libraries for display and radio transmission, so the board-specific code will be minimal.
```

---
## \#76 Posted by: DroidSector Posted at: 2018-11-11T07:31:15.707Z Reads: 375

```
Spent the whole day looking for the reason of those reboots, turns out ESP32 processor doesn't like the massive code that RadioHead library has inside an interrupt routine. Had to replace it with LoRa library. Good thing is, now there is like 10 times less code in the radio and display libraries.
```

---
## \#77 Posted by: DroidSector Posted at: 2018-11-11T09:33:02.779Z Reads: 376

```
Just tested LoRa frequency hopping by putting Feather remote right next to the LoRa one (using the same 915 Mhz frequency). Only 1 packet of 20 was lost every 1 second or so. No packets were lost when I moved the remote 1 meter away.
```

---
## \#78 Posted by: fedestanco Posted at: 2018-11-11T13:01:49.728Z Reads: 377

```
Basically the only downside of Lora is that it runs on frequencies that are either legal in Europe (800khz) or the US (400khz), but not both. So you'd have to make 2 different designs for the 2 continents.
They also came up with a new chip (sx1280) which runs lora on 2.4ghz (that is fine for US and Europe) but it is more expensive and there arent much modules available.

As an alternative to the feather have a look at this: http://m.mmrix.top/h.3PHHd2b?sm=650f29
The documentation is very good but in chinese.
```

---
## \#79 Posted by: Zentaria Posted at: 2018-11-12T09:57:53.430Z Reads: 373

```
I wish someone could teach me to code something like that :slight_smile: Nice Project tho. Im planning to build a remote but waiting a lil bit more.
```

---
## \#80 Posted by: PickSix24 Posted at: 2018-11-12T16:45:09.859Z Reads: 395

```
Glad you will support the feather board cause I bought everything already 😂 just waiting on the magnets and I’ll be ready to test.
```

---
## \#81 Posted by: PickSix24 Posted at: 2018-11-13T04:23:31.927Z Reads: 412

```
![image|374x500](upload://meOuPZ05jNAK8mS5FTwF3tfPqtO.jpeg)
```

---
## \#82 Posted by: Fabialbo Posted at: 2018-11-13T11:00:02.724Z Reads: 398

```
Great to see some development on the ESP32 boards :slight_smile:
thank you very much @DroidSector  for your development work

[quote="fedestanco, post:78, topic:72916"]
As an alternative to the feather have a look at this: [http://m.mmrix.top/h.3PHHd2b?sm=650f29 ](http://m.mmrix.top/h.3PHHd2b?sm=650f29)
The documentation is very good but in chinese.
[/quote]

also looks interesting, but i still think the ESP with integrated Oled is superior in availability and Price.
If some of you are curious here is a English documentation of the board:
http://dl.intoyun.com/terminal/modules/datasheets/en/IntoRobot-Ant_Datasheet_en.pdf
```

---
## \#83 Posted by: DroidSector Posted at: 2018-11-13T16:29:14.675Z Reads: 401

```
[quote="fedestanco, post:78, topic:72916"]
Basically the only downside of Lora is that it runs on frequencies that are either legal in Europe (800khz) or the US (400khz), but not both. So you’d have to make 2 different designs for the 2 continents.
[/quote]
TTGO boards have the same design for all frequencies, I think. It's just an appropriate frequency in the code needs to be set. That 2.4ghz sx1280 chip looks great, but I'll wait for a cheap board with OLED screen.

Just implemented the parallel processing in both cores of the ESP board, so screen updates won't delay the radio transmission, which is 11ms for tx + rx.

> **Remote:** 
> * Core 1:
>   * Handle buttons
>   * Update display
> * Core 0:
>   * Calculate throttle position
>   * Transmit/receive data

> **Receiver:** 
> * Core 1:
>   * Get telemetry
>   * Update display
> * Core 0:
>   * Receive/transmit data
>   * Control speed
```

---
## \#84 Posted by: StefanMe Posted at: 2018-11-13T17:27:49.114Z Reads: 362

```
Sorry but maybe I understood something wrong...  but u has two cores in the TTGO boards?? Two different cores, one for display handling and the other core for telemetry and the work parallel??

GREAT WORK!
```

---
## \#85 Posted by: DroidSector Posted at: 2018-11-13T17:37:51.395Z Reads: 359

```
Yes, and it's rather easy to use:
https://randomnerdtutorials.com/esp32-dual-core-arduino-ide/
```

---
## \#86 Posted by: StefanMe Posted at: 2018-11-13T18:11:21.801Z Reads: 363

```
Very nice! Makes the timing part very easy! Cool feature of the ESP Chip. Unfortunately not available for the SAMD chip! And maybe not necessary but as I said before... makes a lot things easier! U removed the 10ms transmitting time completely! Nice work!
```

---
## \#87 Posted by: fedestanco Posted at: 2018-11-13T18:44:55.998Z Reads: 369

```
[quote="DroidSector, post:83, topic:72916"]
TTGO boards have the same design for all frequencies, I think.
[/quote]

The description of the feather made me think there are 2 chips for the 2 frequencies: 

_This is the 900 MHz radio version, which can be used for either 868MHz or 915MHz transmission/reception - the exact radio frequency is determined when you load the software since it can be tuned around dynamically. We also sell a 433MHz version of the same radio chipset!_ (from adafruit website)
```

---
## \#88 Posted by: DroidSector Posted at: 2018-11-14T00:42:58.412Z Reads: 380

```
Yeah, the same with TTGO boards. But their physical size is the same.

It's possible to get [SX1280 transceiver](https://www.aliexpress.com/item/SX1280-LoRa-Bluetooth-Wireless-rf-Transceiver-2-4-GHz-Module-E28-2G4M12S-SPI-Long-Range-2/32835072788.html) and use it with a WiFi LoRa board to make a universal remote, but I can't find Arduino library to interact with it yet.
```

---
## \#89 Posted by: DroidSector Posted at: 2018-11-14T08:14:50.527Z Reads: 388

```
Turns out this board is almost exactly the same size as a battery meter in Ownboard ESC case, so I printed a new case for the receiver and added the software battery meter:

https://youtu.be/Dv1gESdI6rU
```

---
## \#90 Posted by: myreala Posted at: 2018-11-18T09:04:57.452Z Reads: 380

```
Good stuff man. Also doing a build with feathers It'll probably take a month to get all the small stuff from china though.
```

---
## \#91 Posted by: myreala Posted at: 2018-11-18T21:44:18.052Z Reads: 376

```
So the parts list does not list a separate antenna. Is the default antenna just a regular wire of 7.8 cm?  
And if I were to get this https://www.getfpv.com/tbs-xf-race-antenna-915mhz.html  race antenna mentioned in the thread would it fit inside the remote housing easily?
```

---
## \#92 Posted by: PickSix24 Posted at: 2018-11-18T22:34:51.428Z Reads: 365

```
I’m still waiting on a few parts. I have the antennas already and my case printed. The antenna is pretty small and flat, looks like it should fit no prob. I’ll mock some parts up later to double check.
```

---
## \#93 Posted by: DroidSector Posted at: 2018-11-19T02:44:18.533Z Reads: 373

```
https://www.electric-skateboard.builders/t/firefly-nano-remote/72916/48?u=droidsector

Probably the same antenna: https://www.aliexpress.com/item/RCmall-868MHz-915MHz-FPC-Antenna-868MHz-Spring-IPX-IPEX-1-13-Antenna-IPEX-Antenna-850-1850MHz/32862215507.html. It will fit, just make sure to use 28-30 AWG wire because there is not much space between Feather board and OLED screen.

Finally tested TTGO boards in ~30 km group ride with more than 20 people, worked perfectly. 

The only problem is that I got an older version without a battery probe. Now I'm waiting for this one, most probably will use in the final product: 
https://www.aliexpress.com/item/TTGO-LoRa32-V2-1-1-6-version-433-868-915Mhz-ESP32-LoRa-OLED-0-96-Inch/32872078587.html

Will test this one as well for the receiver side, will save you $10 if you don't need/want a battery meter display on the skateboard:
https://www.aliexpress.com/item/TTGO-ESP32-SX1276-LoRa-868-915MHz-Bluetooth-WI-FI-Lora-Internet-Antenna-Development-Board-for-Arduino/32845370112.html
```

---
## \#94 Posted by: lrdesigns Posted at: 2018-11-19T03:19:50.086Z Reads: 377

```
[quote="DroidSector, post:93, topic:72916"]
Finally tested TTGO boards in ~30 km group ride with more than 20 people, worked perfectly.
[/quote]

Nice! 

[quote="DroidSector, post:93, topic:72916"]
Now I’m waiting for this one, most probably will use in the final product:
[/quote]

isn't the SMA antenna mount on this one kind large and get in the way?

Edit, never mind I see it also has the small style antenna mount. :grinning: 
![image|625x500](upload://p7JF3D7Sr88tUwHlR6A5XAyBPl1.jpeg)
```

---
## \#95 Posted by: DroidSector Posted at: 2018-11-19T03:23:12.120Z Reads: 354

```
Yeah, the big one will need to be removed I guess.
```

---
## \#96 Posted by: oyta Posted at: 2018-11-19T06:35:51.321Z Reads: 360

```
I haven’t really been able to follow all the talk in this thread lately. Please understand this post as a desire to understand the remote design you’ve done.

If yes to the following question you can skip the last part 😊 Are you using the Bluetooth or or Wifi options on the TTGO for the remote control?

If no, are you using the LoraWAN protocol for the remote controls? LoraWAN is designed for an IoT wide area network and is from what I understand not really ment for this kind of application. LoraWAN is a competitor to among others SigFox, NB-iot and Lte-m. I believe some of the design goals of this protocol are long range (in terms of sensitivity), low power (devices on battery holding several years), low bandwidth (long interval and or few bytes which is also relevant for the low power) and many devices on the same bandwidth. I could be wrong, but there should be other technologies better suited?
```

---
## \#97 Posted by: DroidSector Posted at: 2018-11-19T07:28:11.843Z Reads: 342

```
I'm not using LoraWAN protocol, only LoRa radio in a [fast mode](https://www.electric-skateboard.builders/t/firefly-nano-remote/72916/38?u=droidsector). Basically, we need a board with a radio transceiver, a battery charger, and screen to make the assembly easier, so if anyone can recommend a more suitable board in $15-25 range I'll test it as well.
```

---
## \#98 Posted by: DroidSector Posted at: 2018-11-19T07:42:01.416Z Reads: 335

```
Just ordered [LM3UU linear bearings](https://www.aliexpress.com/item/10pcs-LM3UU-LM4UU-LM5UU-LM6UU-LM8UU-LM10UU-LM12UU-Linear-Bushing-8mm-CNC-Linear-Bearings-for-Rods/32894477568.html) for testing, at 3x7x10mm one should fit right inside the throttle wheel.
```

---
## \#99 Posted by: oyta Posted at: 2018-11-19T08:11:26.294Z Reads: 341

```
Interesting. What tx-power and frequency band are you using?
```

---
## \#100 Posted by: DroidSector Posted at: 2018-11-19T08:55:50.623Z Reads: 353

```
I've set the frequency to 920 MHz and used these settings:

>     LoRa.setSignalBandwidth(500E3);
>     LoRa.setTxPower(10);  
>     LoRa.setSpreadingFactor(6);
>     LoRa.enableCrc();
```

---
## \#101 Posted by: wapkoen Posted at: 2018-11-19T09:04:04.245Z Reads: 355

```
maybe i misunderstand. but those bearings are linear. the are supposed to go along an axle. Not rotate around it. 
so if i understand your intention correctly. those lm3uu bearing will not work .

I use ptfe tube as a bushing in my remote wheel. it works great. it sits on a small 2mm carbon rod.
```

---
## \#102 Posted by: StefanMe Posted at: 2018-11-19T09:11:32.502Z Reads: 333

```
These bearings are worst on turning! They are made for LINEAR movement...
```

---
## \#103 Posted by: StefanMe Posted at: 2018-11-19T09:21:38.127Z Reads: 340

```
Use 693ZZ bearings :) they are great for this.

https://www.ebay.de/itm/10-Stk-Kugellager-693ZZ-Miniatur-Rillenkugellager-3x8x4mm/362210414011?ssPageName=STRK%3AMEBIDX%3AIT&_trksid=p2060353.m2749.l2649
```

---
## \#104 Posted by: DroidSector Posted at: 2018-11-19T09:22:09.387Z Reads: 336

```
That's a good idea, I have an extra ptfe tube laying around. I really missed the linear bit in the bearings description :)
```

---
## \#105 Posted by: botiejedi Posted at: 2018-11-23T18:22:57.643Z Reads: 331

```
Does anyone know if someone is building and selling these yet? or am i just forced to have fun and build it on my own?
```

---
## \#106 Posted by: PickSix24 Posted at: 2018-11-23T19:08:20.859Z Reads: 329

```
I’m just waiting on a few more parts that should arrive soon. Probably going to sell mine as a kit or assembled, as I’ve got too many projects.
```

---
## \#107 Posted by: swimmydude Posted at: 2018-11-23T23:31:31.853Z Reads: 339

```
Same, I have a few more parts I'm waiting on. I bought enough where I can make a good number of remotes (original Firefly, not this modification) minus the nano and nRF24 module. I only got enough for 2 remotes for the more expensive parts because I'm not entirely sure yet if I will make any to sell or whatever. So @botiejedi, it's a possibility but not a guarantee and it wouldn't be right now. It would probably be at the earliest, beginning of next year because I won't have access to a 3D printer until then.
```

---
## \#108 Posted by: botiejedi Posted at: 2018-11-24T00:28:27.051Z Reads: 330

```
Alright good to know I might just go the diy route
```

---
## \#109 Posted by: katsuma Posted at: 2018-11-24T00:29:16.282Z Reads: 356

```
Hey @DroidSector , thanks for this project your making. Its quite interesting using these feathers as trans/recv for the esk8 !

I am trying to compile the code you exposed on github but i'm having difficulties. It is giving me an error when using the Arduino IDE : 

'class USBDevice_' has no member named 'standby'

Board that i had chosen was Adafruit feather 32u4

Also, if i try to use your method described in the wiki -> https://github.com/DroidSector/FireFly-Nano-Remote/wiki/3.-Software

I am not able to launch it through the PlatformIO of Atom, when i check i see that in the repository i dont see any file relating to  "platformio.ini"

Would be cool to shed some light in this, i really am confused on how to try to compile this

Thanks!
```

---
## \#110 Posted by: StefanMe Posted at: 2018-11-24T00:54:49.355Z Reads: 322

```
U chooses the wrong board. It’s feather M0...
```

---
## \#111 Posted by: katsuma Posted at: 2018-11-24T10:06:07.613Z Reads: 324

```
oh .. my ... god, youre right!!! 
My problem is that i bought the 32u4 version :(.... ugh , that sucks..
```

---
## \#112 Posted by: DroidSector Posted at: 2018-11-24T12:57:40.117Z Reads: 329

```
Yes, try exchanging it for Feather M0, 32u4 doesn't have enough flash storage to fit the code. I did the same mistake btw.

Still refactoring the code for PlatformIO to support both Feather and several TTGO boards. All basic stuff is already working, just need a couple more days.
```

---
## \#113 Posted by: PickSix24 Posted at: 2018-11-25T19:52:05.427Z Reads: 316

```
Are the magnet dimensions 5mm x 5mm ?
```

---
## \#114 Posted by: swimmydude Posted at: 2018-11-25T21:28:31.693Z Reads: 306

```
If it is unchanged from solidgeek's design, then yes.
```

---
## \#115 Posted by: PickSix24 Posted at: 2018-11-25T21:29:04.363Z Reads: 313

```
Thanks , trying to find some alternatives
```

---
## \#116 Posted by: PickSix24 Posted at: 2018-11-26T01:21:00.039Z Reads: 320

```
Ok I was able to find some 5mm x 1mm on Amazon. Figure I can stack 5 to make a 5x5mm magnet. That should work right ?
```

---
## \#117 Posted by: ervinelin Posted at: 2018-11-26T01:28:58.211Z Reads: 339

```
I did that before for the same exact reason... Works but the magnet strength might not be the same so might need some calibration...

But definitely will work.
```

---
## \#118 Posted by: Jinra Posted at: 2018-11-26T04:18:43.658Z Reads: 345

```
@DroidSector I bought the screen on your shopping list but the holes dont seem to line up 🤔

![IMG_20181125_201838|666x500](upload://dbDeTYWlQOArxVFOGP7PuufWztC.jpeg)
```

---
## \#119 Posted by: DroidSector Posted at: 2018-11-26T06:02:48.793Z Reads: 335

```
That's strange, I got mine from Australian eBay but the one from AliExpress has the same size in the description. Does it fits if you cut the pins?
```

---
## \#120 Posted by: ervinelin Posted at: 2018-11-26T06:10:07.658Z Reads: 328

```
I've had some that don't fit as well... looks same in the picture, arrives with some slight variability...
```

---
## \#121 Posted by: Jinra Posted at: 2018-11-26T06:53:31.651Z Reads: 334

```
you mean the pins on the enclosure?I did that but the recess for the PCB pins is too high up for the screen and it sits tilted a bit
```

---
## \#122 Posted by: DroidSector Posted at: 2018-11-26T07:31:34.307Z Reads: 337

```
Can you cut it like this?
![cut|334x250](upload://fLxLETiu5CHuw2N9c5BwILudPZF.jpeg) 

I've also cut the metallic pins on the screen side. I actually ordered the screen with the unsoldered header, but of course, it arrived with the soldered one. :angry:
```

---
## \#123 Posted by: Jinra Posted at: 2018-11-26T08:15:53.202Z Reads: 322

```
Yeah I'll Dremel it off like you showed. just hope it sits alright with hot glue
```

---
## \#124 Posted by: PickSix24 Posted at: 2018-11-27T00:49:08.742Z Reads: 341

```
![image|375x500](upload://m3oubd7qXanj6UWAPgBeLtG2O2q.jpeg) 

Same issue here

![image|375x500](upload://vu99bCPUYgRIGAxRzt6cYvanQDE.jpeg) 

Tried trimming the corner of the board. Screen sits center now, I’ll glue it in place
```

---
## \#125 Posted by: PickSix24 Posted at: 2018-11-27T02:38:56.040Z Reads: 327

```
I’ve got my remote fully built. I’m not super versed in Arduino... I’ve got the program open and the transmitter file open but I’m getting some errors when trying to upload. Can anyone give me a little guidance please ? Thanks in advance
```

---
## \#126 Posted by: DroidSector Posted at: 2018-11-27T06:43:23.247Z Reads: 334

```
Please see this wiki page:
https://github.com/DroidSector/FireFly-Nano-Remote/wiki/3.-Software

Arduino IDE requires a lot of time to manually install all boards and libraries. I've just uploaded new code rewritten for PlatformIO, it will install all required libraries automatically. Please let me know if something go wrong or the guide is unclear.

I tested this code on TTGO board connected to ESC, with Feather I did only radio transmission test. Will do a test ride with Feather tomorrow.
```

---
## \#127 Posted by: PickSix24 Posted at: 2018-11-27T10:35:55.888Z Reads: 320

```
Thank You ! Looks straightforward, I’ll give this a shot when I get home today.
```

---
## \#128 Posted by: PickSix24 Posted at: 2018-11-28T02:10:15.857Z Reads: 331

```
Am I doing something wrong here... ? Not seeing where to build the file. Would it be possible to post a few more photos of the steps on the wiki ? 

![image|666x500](upload://tQAsbK8J8cdjUibNRMEVE7ThQWw.jpeg)
```

---
## \#129 Posted by: DroidSector Posted at: 2018-11-28T03:57:34.633Z Reads: 327

```
Please re-download the code and make sure that "platformio-ide" package is installed. Restart Atom if you don't see buttons on the left:
![25|690x431](upload://ofEm9am5SvGIOyt7BCa8h7grHzZ.jpeg)
```

---
## \#130 Posted by: PickSix24 Posted at: 2018-11-28T06:24:30.064Z Reads: 326

```
Ok so I was able to enable platformio. When I load the file and hit build I get an error. Sorry if I’m missing something 
![image|666x500](upload://2XWlqWFZG9x5LfelPZl5ENC1Q7q.jpeg)
```

---
## \#131 Posted by: DroidSector Posted at: 2018-11-28T06:39:02.368Z Reads: 318

```
Looks like it needs this structure:
FireFly-Nano...master
  L include 
  L src

Try to remove the FireFly-Nano...master folder in the left panel (right click > Remove Project Folder) and add the immediate parent of src folder.
```

---
## \#132 Posted by: PickSix24 Posted at: 2018-11-28T06:39:06.386Z Reads: 336

```
![image|666x500](upload://cgUw3TY3tKvB17v1LF8xFnkHaIc.jpeg) 
I think I got the build to upload to the feather but I can’t get the remote to turn on or the OLED to come on. Looks like all my connections are good.
```

---
## \#133 Posted by: DroidSector Posted at: 2018-11-28T06:47:46.654Z Reads: 304

```
Could you please scroll up the window that says [error]? There should be a more specific error listed.
```

---
## \#134 Posted by: PickSix24 Posted at: 2018-11-28T06:51:33.669Z Reads: 308

```
That window doesn’t scroll
```

---
## \#135 Posted by: DroidSector Posted at: 2018-11-28T06:57:16.067Z Reads: 301

```
Try to press Ctrl+Alt+V to reopen the build panel and scroll with the mouse wheel or resize it.
```

---
## \#136 Posted by: DroidSector Posted at: 2018-11-28T08:50:35.972Z Reads: 303

```
My bad, VescUart library didn't get uploaded to GitHub. Please [download](https://github.com/DroidSector/FireFly-Nano-Remote/archive/master.zip) the code again.
```

---
## \#137 Posted by: PickSix24 Posted at: 2018-11-28T14:15:01.378Z Reads: 305

```
So it looks like I was able to successfully upload the program onto the feather. OLED and power button don’t show any life though so I’m not sure what’s wrong.
```

---
## \#138 Posted by: dspx Posted at: 2018-11-28T15:35:46.436Z Reads: 316

```
That happened to me, but that's because I mistakenly bought a 12v OLED instead of the recommended 3~5.5v on the parts list. They all look the same, devil's in the details  :sweat_smile:

Oh, and I also ran into the problem of having the opposite pinouts for the battery (bought mine from Amazon instead of Adafruit)so I had to switch those around.
```

---
## \#139 Posted by: DroidSector Posted at: 2018-11-28T15:46:00.942Z Reads: 314

```
Make sure that this line is uncommented:
env_default = Remote.Feather

You should see these lines after uploading:

Environment Remote.Feather              [SUCCESS]
Environment Receiver.Feather            [SKIP]
```

---
## \#140 Posted by: PickSix24 Posted at: 2018-11-28T16:08:17.088Z Reads: 300

```
I had the same thing with the battery
```

---
## \#141 Posted by: PickSix24 Posted at: 2018-11-28T16:35:06.171Z Reads: 314

```
In the event I can’t figure this thing out...:rofl:
Is anyone in the US interested in taking this project off my hands ? I’ve got everything plus some spares of the items I had to buy in bulk. Someone in the US wouldn’t have to wait on shipping from China. Just starting to think it’s a little above me :roll_eyes:
```

---
## \#142 Posted by: PickSix24 Posted at: 2018-11-29T01:08:47.877Z Reads: 316

```
Made sure I changed to Remote.Feather. Saved and built then uploaded. Seems to be something going on with the upload process though, it’s been running for like 10 minutes....![image|666x500](upload://cWhV9lD7P6iw5pHXk5TtVkC9sLN.jpeg)
```

---
## \#143 Posted by: PickSix24 Posted at: 2018-11-29T01:19:25.044Z Reads: 297

```
In the meantime I tried to program the receiver and that worked ! , took like 20sec. Just need to figure out what’s going on with the transmitter
```

---
## \#144 Posted by: DroidSector Posted at: 2018-11-29T01:45:52.848Z Reads: 295

```
[quote="PickSix24, post:142, topic:72916"]
Seems to be something going on with the upload process though, it’s been running for like 10 minutes…
[/quote]
I have this issue from time to time, try pressing the reset button on Feather before upload starts.
```

---
## \#145 Posted by: PickSix24 Posted at: 2018-11-29T01:57:54.052Z Reads: 287

```
Ok I’ll give that a go. Is it possible I screwed up the board on the previous attempts like does it need to be erased, or will it just overwrite.
The reciever went easily !
```

---
## \#146 Posted by: PickSix24 Posted at: 2018-11-29T03:55:06.734Z Reads: 295

```
I’ve tried this a dozen times now. The build is correct for the remote but I can’t get it to upload. 
Scratch that!!! It finally worked !!!! Wooooo
```

---
## \#147 Posted by: PickSix24 Posted at: 2018-11-29T13:51:51.558Z Reads: 289

```
Does the direction of the magets matter for the thumbwheel ?
```

---
## \#148 Posted by: butt_stallion Posted at: 2018-11-29T14:54:55.615Z Reads: 288

```
Has anyone tested this remote with @Ackmaniac's VESC firmware?
```

---
## \#149 Posted by: DroidSector Posted at: 2018-11-29T15:47:31.521Z Reads: 286

```
@PickSix24 their polarity should be opposite to each other. If you turn on remote only, you'll see hal values on connecting screen.

@butt_stallion yes, both with original and @Ackmaniac's firmware.
```

---
## \#150 Posted by: DroidSector Posted at: 2018-11-29T16:19:48.527Z Reads: 284

```
Tested today BLE packet forwarding on TTGO board, essentially it works the same as HM-10 Bluetooth module. Got original VESC-Tool mobile to connect and show real-time data. Not quite sure that it will work good enough in parallel with the remote, but at least the ability to configure motor settings on mobile devices would be useful.
```

---
## \#151 Posted by: katsuma Posted at: 2018-12-03T10:36:26.310Z Reads: 309

```
Hey @DroidSector, so i got finally my Feather M0's and it looks like im finally able to compile & upload the code to them . They indeed are connecting and after soldering all the other components i was making some tests.

I saw that in the OLED screen if i press the power button i can then have further debug on checking the hall sensor values. It appears he goes from 127 to 20 from one way but if i move the thumbwheel on the oposite from neutrall the value goes reaallly small , from 127.500 to 127.800. is it intended? to have a completly different sensitivity on one of the ways ?

Also when i power on the transmitter and it is connected to the receiver, the LED of the power switch is constantly blinking. Is this normal ? 
And i have this issue when i turn the thumbwheel any of the directions , the connection gets lost for some miliseconds and back on. Looks like the magnets are affecting the communication? If so, is there something i can do to fix this?

And related to the receiver, i have it connected to my Maytech VESC based controller. I honestly don't know what are the steps to correctly set it up. I just connected the pinouts to the UART port from the receiver but i am not getting any telemetry data. Do i need to update the firmware first of the VESC? If so, by using the vesc tool what do i need to configure there to properly get UART port work with the feather m0 receiver?

Hope someone can shed some light on this for me. Thanks.
```

---
## \#152 Posted by: katsuma Posted at: 2018-12-04T01:33:01.311Z Reads: 290

```
Alright, i got an update on my issues.

Regarding the HALL sensors values. This was just a misjudgment from my side. It is indeed working as it should be and the values are relative if im pressing the deadman trigger or not. After also adjusting the min/max/center of hall the values appear to be alright.

Now after some more tries i realized that my vesc was not updated to the latest FW. After updating and changing baud rate to 9600 it looks like the receiver was collecting UART data.

Now i got ran into a weird problem.... I see the transmitter connected with the receiver, however it looks like there is an issue with comunication. The OLED transmitter keeps blinking from 0% deck battery to 100% and speed from 0 to max, in 2 in 2 seconds. Sometimes if i write something on the config of the vesc , out of nowhere the transmitter and receiver are working perfectly. Then if i switch everything off and the on, the problem appears again. I can sometimes get the  transm/receiver working by constantly changing baudrate of the vesc and for some unkown reason in one of the tries , it starts to work until i switch off.....

Im lost now on where is the issue of this. i see on the log the UART data is being collected and transmitted, but the transmitter /receiver connection is really weird and only sometimes it work perfectly until i shut it off.
```

---
## \#153 Posted by: DroidSector Posted at: 2018-12-04T01:37:49.524Z Reads: 264

```
Are you testing it while your computer is connected to the vesc? Please try to disconnect all the cables.

You can also try to increase the baudrate both in vesc and in receiver.cpp:

> 59: Serial1.begin(9600);

Also comment out DEBUG directive and rebuild code for receiver and remote, it should also speed things up.
```

---
## \#154 Posted by: katsuma Posted at: 2018-12-04T09:23:45.235Z Reads: 283

```
@DroidSector, i tried that but unfortunately no progress...

I tried something to make sure what is wrong and i went to the receiver code and uncommented the debug fields of UART message:

// telemetry.setVoltage(41.35);
...
 // telemetryUpdated = true;
// return; 

After that the communication between the transmitter and receiver is working perfectly and it never went down , even if i shutdown any of them and put them back on.

So this indicates there is an issue on constantly fetching UART data from the VESC. I am having a strong gut feeling that this is related to the way my feather m0 is connected to the VESC.

Here is a small indication on how i have it currently connected:

Feather m0              VEsc UART
3v3 -------------------------3v3
GND------------------------GND
TX---------------------------RX
RX---------------------------TX

Now, i dont have any more connections because i saw the feather being powered up through the 3v3pinout...?!
However it does not make sense because from the spec of the feather m0, that pinout actually provides power and not receiving it.

If had my feather connected though through usb to my PC for debugging purporses. 

Do you think i have to use the 5V pinout from UART Vesc port to power as well the feather m0? could that be the issue? If that is it, which pinout connection should be ? USB/BAT to 5v UART ?
```

---
## \#155 Posted by: DroidSector Posted at: 2018-12-04T09:44:39.571Z Reads: 266

```
Try to set `uartPullInterval = 1000;` (1 sec) in receiver.h and maybe uncomment `UART.setDebugPort(&Serial);` in receiver.cpp. 

You can connect UART 5v or 3.3v to BAT pin, it will use the regulator but I guess it won't feed power into vesc from the USB cable.
```

---
## \#156 Posted by: katsuma Posted at: 2018-12-04T10:26:05.643Z Reads: 274

```
So just to make sure, the connection pins your are saying is 

Feather m0             Vesc UART
BAT ----------------------3v3/5v
GND ---------------------GND
TX   ----------------------RX
RX  -----------------------TX

Is just that on your diagram https://raw.githubusercontent.com/DroidSector/RF69-Esk8-Remote/development/images/electronics_schematic_receiver.png

I see the 3v3 connected from/to UART and feather m0.
And then i see a power filter of 5v to GND, but which gnd and which 5v ? from feather ? i think its a power filter from the vesc to the feather, but then which pinouts should they be connected to ? 


Thanks for the help , i will try though on doing the bat/3v3 and changing that code line.
```

---
## \#157 Posted by: DroidSector Posted at: 2018-12-04T10:36:02.808Z Reads: 251

```
Sorry, I was lazy and copy-pasted it, it should be 3.3v instead of 5v. Because the capacitors were rather big, I've placed this filter around the middle of power wires between Feather and UART.
```

---
## \#158 Posted by: katsuma Posted at: 2018-12-05T00:07:07.129Z Reads: 282

```
Alright so after performing aditional trial and errors and following @DroidSector advice, here are the observations:

the wiring of the receiver it should be indeed

Feather M0 ---------- UART Vesc
      BAT          ---------         3v

                       OR
      USB      -----------        5v


All the others are the same as in the receiver image that Droid provided.

After this i got stable connection for throttling the engine and breaking...
 However, weirdly enough i am having issues with the telemetry information exchange.

With ddebug i did not find any weird error message or missing information when building the packet to send to the transmitter. But, on the transmitter i saw that i get sometimes, and for some periods i get only "No reply" debug message. This however does not interfere at all with the throttle/break command.

On the debug of the transmitter i see that before it gives "No reply" he actually receives a packet but with different information.

Response: 0 , chain: 23, CRC: 46

After these packets are shown on debug, then the "No reply" debug message shows after.

If i get a Response:1, chain:23, CRC: 77   It is then working fine.

I dont know where the response:0 messages are coming from but it is why my transmitter is giving incorrect  telemetry on the OLED.
Just to clarify, sometimes it does get proper info for some seconds and i see corrrect information, but most of the time is just giving default/different values than it should be.

Also on the receiver i am never getting UART data issues.

I changed the baudrate and the timeout to 1 sec of capturing UART data and it did not make a difference in this.
```

---
## \#159 Posted by: DroidSector Posted at: 2018-12-05T05:44:38.837Z Reads: 253

```
Please try to increase the timeout to 100 in responseAvailable() function (remote.cpp):

> if (millis() - ms > 10) return false;

I'll connect Feather to vesc to test it more thoroughly today.
```

---
## \#160 Posted by: katsuma Posted at: 2018-12-05T08:35:37.666Z Reads: 269

```
@DroidSector, it really worked! the refresh time of telemetry is not quick but honestly its more than fine for me. throttle/break response is quite good so its not conflicting with the driving. 

Thanks a lot !!! 

Just as an improvement for me, do you know where can i change the sensitivity of the acceleration?
I feel that the moment i get close to the thumbwheel on a specific point it starts engaging almost full speed. Perhaps i could change the acceleration relative to the hall values? If you could help me checking which place it would be great!

Again, thanks a lot DroidSector, finally it is working ! and awesome transmitter btw :)
```

---
## \#161 Posted by: DroidSector Posted at: 2018-12-05T09:05:35.729Z Reads: 270

```
Thanks! You can change _HALL values in globals.h. Move the throttle wheel to the full stop or a position convenient for you and note the hall value on the debug screen (should be around 600). Use it for MAX_HALL value. Repeat the same for brake and MIN_HALL. CENTER_HALL should match the idle hall value.

Another value to tweak is this one (in bold) on [line 691](https://github.com/DroidSector/FireFly-Nano-Remote/blob/05ac647a4cef60b30f5df2489861892b045b727d/src/remote/remote.cpp#L691):
> position = constrain(map(hallValue, settings.centerHallValue + hallNoiseMargin, settings.maxHallValue, **127**, 255), 127, 255);

Stand on the board and give a little throttle, just enough to start moving. Note the hall value and use it instead of 127. This will expand the useful range of the throttle wheel. I'm currently working on a calibration screen to automate this process.
```

---
## \#162 Posted by: mptrs Posted at: 2018-12-05T21:41:11.387Z Reads: 250

```
@DroidSector looking at the specs I see you are using a different hall-effect sensor than the original Firefly. Just to be sure, I can use the Honeywell that was specified with the original Firefly as well right? (I have an extra laying around hehe)
```

---
## \#163 Posted by: DroidSector Posted at: 2018-12-06T02:26:32.814Z Reads: 256

```
I guess it should work:
https://www.electric-skateboard.builders/t/simple-3d-printed-nrf-remote-arduino-controlled/28543/233?u=droidsector
```

---
## \#164 Posted by: mptrs Posted at: 2018-12-06T07:36:50.688Z Reads: 249

```
Thanks! Missed the voltage difference. A step-up isn't that big, so I'll keep that as an option.
```

---
## \#165 Posted by: StefanMe Posted at: 2018-12-06T07:44:12.023Z Reads: 257

```
NO STEP UP! U have to use the 3.3V input on the feather/TTGO both are not 5V tolerant!
```

---
## \#166 Posted by: mptrs Posted at: 2018-12-06T07:47:27.318Z Reads: 257

```
If I added a step-up I should add a step-down as well I guess than. That sounds like too much work, I'll get a 3.3V one if this one doesn't work.

Thanks for the heads up!
```

---
## \#167 Posted by: StefanMe Posted at: 2018-12-06T08:18:46.999Z Reads: 259

```
definitly... 

but i many people told that the 5v honeywell sensor is working good on the 3.3v. the Honeywell SS49E is the 3.3V version of this.
```

---
## \#168 Posted by: katsuma Posted at: 2018-12-06T10:02:05.152Z Reads: 272

```
this line that you mentioned @DroidSector:

position = constrain(map(hallValue, settings.centerHallValue + hallNoiseMargin, settings.maxHallValue,  **127** , 255), 127, 255);

it really gave a much better feedback and control on the throttle of the board. instead of only getting response half way through the throttle , now i have the full range of throttle motion in the thumbwheel. 
I applied the same relation to the braking, that is another code line beneath. And its working really good. 

Just that the screen is not refreshing in 25ms or something, it now updates info more slowly but honestly... i dont have any issue at all with that since im not looking at the remote all the time.

Thanks again @DroidSector, now with it all finished it really is an awesome transmitter!.

I checked on the code that there is cruise control code commented out. You think i could enable it or it needs further development ?
```

---
## \#169 Posted by: DroidSector Posted at: 2018-12-06T10:49:34.867Z Reads: 261

```
This code is not ready yet, I've tried vesc built-in cruise control but it works with one motor only for some reason.

I've also tried to set the UART speed to 115200 and it worked good - much better data refresh rate, but I need to fix some problems. Will upload the code in a few days.
```

---
## \#170 Posted by: katsuma Posted at: 2018-12-06T10:53:48.588Z Reads: 264

```
[quote="DroidSector, post:169, topic:72916"]
I’ve tried vesc built-in cruise control but it works with one motor only for some reason.
[/quote]

Thats perfect because i only have one motor! :D 

Cant wait for that code update! :)
```

---
## \#171 Posted by: Jamie42 Posted at: 2018-12-07T15:35:49.899Z Reads: 267

```
Hii @DroidSector !  I have read this whole topic and I really like your remote! Will probably use it for my next longboard. 

I have a few questions however:
- I want to use the TTGO board, do you already have a 3D design for it? 
- Does your code (on github) work with the TTGO board? 

Thanks!

Edit: Another one:
- What did you do with that antenna on the LoRa32?
```

---
## \#172 Posted by: DroidSector Posted at: 2018-12-07T21:26:58.413Z Reads: 262

```
Not yet, still looking for a suitable board, should get latest Heltec board on Monday. The TTGO v2 does not fit without major enclosure redesign and small antenna connector does not work.

The good news is that the code is already compatible with both Feather and TTGO/Heltec boards. Menu, calibration and pairing should be ready next week.
```

---
## \#173 Posted by: Jamie42 Posted at: 2018-12-07T21:35:17.024Z Reads: 284

```
Nice that the code works! Not so nice the small antenna connector doesn't, could other versions of this board maybe have a working small connector? Like the v2.1 for example? Looking forward to the results of the Helltec board!
```

---
## \#174 Posted by: StefanMe Posted at: 2018-12-08T00:05:41.018Z Reads: 287

```
Unfortunately the heltec board is the worst one...

https://youtu.be/cjVwTf8iDFY
```

---
## \#175 Posted by: Jamie42 Posted at: 2018-12-08T07:30:28.031Z Reads: 280

```
What about [these](https://s.click.aliexpress.com/e/9SMfAyY)? 433 Mhz version.
```

---
## \#176 Posted by: DroidSector Posted at: 2018-12-08T09:08:31.362Z Reads: 288

```
Sorry, I was talking about v2.1, but v2 has USB connector on the side and no battery probe. I also don't really like that they changing the physical design every few months.

[quote="Jamie42, post:175, topic:72916"]
What about [these ](https://s.click.aliexpress.com/e/9SMfAyY)? 433 Mhz version.
[/quote]
This is a good board for receiver.

@StefanMe I don't see Heltec board in this video. Anyway, I hope [version 2](http://www.heltec.cn/wifi-lora-32-new-edition-comparison/?lang=en) will work better.
```

---
## \#177 Posted by: Jamie42 Posted at: 2018-12-08T13:00:52.069Z Reads: 273

```
Guess I will use that 433 Mhz then. That one is also legal hete.
```

---
## \#178 Posted by: dspx Posted at: 2018-12-09T22:23:24.432Z Reads: 284

```
[quote="PickSix24, post:137, topic:72916, full:true"]
So it looks like I was able to successfully upload the program onto the feather. OLED and power button don’t show any life though so I’m not sure what’s wrong.
[/quote]

@DroidSector I'm running into this issue after installing the vibration motor. Uploading the program worked fine, it powered on through the usb initially, LCD lit up with information and connected to the receiver just fine. But once I disconnected from usb and attached the battery, the transmitter continued to fail. It blinks once and dies. Before the motor, the transmitter functioned as expected. After the motor, the transmitter refuses to power on even when connected to usb without the battery. The parts I'm using, save for the battery, are identical to those listed in your google doc. The battery I'm using should also be sufficient http://a.co/d/8wMa0mr

The board is still able to be recognized and programmed, but it simply won't power on by usb or battery. This is the second feather I've tested with the same result. Again, same components, so I wouldn't expect any compatibility issues.

I'm wondering if you or anyone else has experienced this and would be able to help me troubleshoot. For now, I'll revert back to the motor-less configuration and hope I can get it back to working order :crossed_fingers:

Edit: /sigh disconnected the motor and it still won't power on.
```

---
## \#179 Posted by: PickSix24 Posted at: 2018-12-09T22:52:06.791Z Reads: 263

```
Battery polarity correct ? I found I had to reverse mine as the plug came incorrect.
```

---
## \#180 Posted by: dspx Posted at: 2018-12-09T22:54:41.033Z Reads: 267

```
Yeah, I'd mentioned that in an earlier post ^_^ but it's not the case here. I'd fixed that early on and it powers the receiver just fine and charges, etc. I don't think it's the battery since the transmitter won't boot up while connected to USB either.

I'm wondering if I overloaded the 3V / GND (if that's possible? I'm no expert in electronics, definitely painting by numbers here). There would be three components on a split to 3V and five components to GND. But again, just using the parts recommended so I'm at a loss as to why this happens.
```

---
## \#181 Posted by: DroidSector Posted at: 2018-12-10T01:00:14.630Z Reads: 277

```
Feather has 500mA peak regulator, so it should be enough for the screen (20ma) and motor (60-90ma). I'm using exactly the same vibration motor module. 

If the board is still able to be programmed, it should be alive. Try to uncomment DEBUG directive in globals.h and check the serial monitor output. Also, make sure that only one line is uncommented in platformio.ini:

> [platformio]
> env_default = Remote.Feather
> ; env_default = Receiver.Feather

If you accidentally uncomment both PlatformIO will use the last one, i.e. receiver.
```

---
## \#182 Posted by: DroidSector Posted at: 2018-12-15T14:34:19.995Z Reads: 278

```
Just pushed the new code, the receiver should be able to work at full UART speed now (115200 bauds). Also added some menus and hall sensor calibration. 

A basic cruise control (VESC feature) is working, but with one motor only on my FlipSky 4.12. After seeing the @Deodand code I have high hopes that it should work as intended with Unity firmware. I'll add support for Unity-specific features as soon as I get it.

Heltec board seem to have all required functionality, the battery probe shows a more or less correct voltage. It also communicates fine with $10 TTGO board. Will finally work on adapting the design, it should not take long.
```

---
## \#183 Posted by: dspx Posted at: 2018-12-15T16:37:38.915Z Reads: 287

```
It works!!! I'm just having an issue with the display information being shifted to the right. :woman_shrugging:
![DSC_1282|281x499](upload://pCiaRIeQ0zavOzF3ZoJWHpwWhlu.jpeg)
```

---
## \#184 Posted by: DroidSector Posted at: 2018-12-16T02:07:24.256Z Reads: 278

```
Hmm, I though only TTGO has this issue. Please download the updated code.
```

---
## \#185 Posted by: DroidSector Posted at: 2018-12-16T02:41:52.998Z Reads: 281

```
There is a faster way to download the code using Atom git tool: press **Alt+G**, then **=** key. In the 'Clone from' field, enter this URL: https://github.com/DroidSector/FireFly-Nano-Remote.git

To download an updated code afterward, press **Alt+G**, then **Shift+F**. These commands also available in the menu: Packages > Command Palette, type _git_.
```

---
## \#186 Posted by: Jamie42 Posted at: 2018-12-17T18:33:22.836Z Reads: 282

```
Does the HELTEC board also work with the FPC antenna?
```

---
## \#187 Posted by: DroidSector Posted at: 2018-12-18T04:48:43.361Z Reads: 290

```
Yes, it works fine.

Changed the design a little, will print and assemble Heltec-based remote tomorrow.
![design|384x500](upload://sFUFIRfVnQRsepxfPE33AGPAov1.jpeg)
```

---
## \#188 Posted by: Jamie42 Posted at: 2018-12-18T19:52:05.201Z Reads: 276

```
What version of the antenna do I need?
```

---
## \#189 Posted by: mptrs Posted at: 2018-12-19T00:11:37.899Z Reads: 268

```
Can you update the thing files on thingiverse?
Will be printing tomorrow, cause I'll be getting some electronics for x-mas :slight_smile:
```

---
## \#190 Posted by: DroidSector Posted at: 2018-12-19T07:13:47.516Z Reads: 276

```
@Jamie42 I've updated the parts list with links to 433 and 915 Mhz versions of both the board and antenna. You can also solder a wire to the board or use the connector from the included large antenna.  

@mptrs I'm finishing the design and will upload it after checking that everything fits together, most probably tonight.
```

---
## \#191 Posted by: rey8801 Posted at: 2018-12-19T13:54:35.706Z Reads: 279

```
Super nice. Shallow question. I guess with tthe Lora32 module than you have blue text. Or it is possible to get the white OLED version or change the screen with an external one?
```

---
## \#192 Posted by: DroidSector Posted at: 2018-12-19T14:32:21.064Z Reads: 285

```
It's a light blue, bearable I think :)

![IMG_20181220_011325|690x389](upload://ictAPrgOPhHz6N4goipdKZLqDdR.jpeg) 

I don't know how hard it will be to change the screen, it looks like this:
![images|423x500](upload://8bc7aUygOn2PNLfQxPws08FxhWN.jpeg)
```

---
## \#193 Posted by: rey8801 Posted at: 2018-12-19T14:33:40.642Z Reads: 273

```
[quote="DroidSector, post:192, topic:72916"]
bearable
[/quote]

I see thanks! No probably not worth it change the screen. Thank you man!
```

---
## \#194 Posted by: mptrs Posted at: 2018-12-19T14:51:40.864Z Reads: 274

```
Thx! In the meantime I'll do a test print, cause it looks like the transparant PLA needs some more heat :)
```

---
## \#195 Posted by: DroidSector Posted at: 2018-12-21T17:37:08.364Z Reads: 281

```
https://www.thingiverse.com/thing:3303495

Changed the design a bit so the top and bottom parts are now connected only by the battery wires:

![IMG_20181220_194000|573x500](upload://s3ff5EHBgKEltbwv1qvHbjcUGQy.jpeg)
```

---
## \#196 Posted by: Jamie42 Posted at: 2018-12-22T07:35:23.981Z Reads: 281

```
Does this make more space for the battery? A 7 mm high battery for example?
```

---
## \#197 Posted by: DroidSector Posted at: 2018-12-22T11:21:22.465Z Reads: 283

```
Probably, if it's a bit shorter (~47 mm) or if you remove the battery connector (yellow).

![Capture|690x373](upload://opMD1nhRrBOPodETypNvGPY7RjH.jpeg)
```

---
## \#198 Posted by: mptrs Posted at: 2018-12-23T09:52:50.868Z Reads: 278

```
Thanks for the update. Is this only for the Heltec board? Or will my feather fit as well?
What is your recommendation, the lora or the feather?
```

---
## \#199 Posted by: DroidSector Posted at: 2018-12-24T03:19:20.412Z Reads: 281

```
Yes, only Heltec board will fit. All essential functions work fine on both boards. Heltec is cheaper and has BT and WiFi, which allows adding OTA updates and some features in the future.  You can also use it as a [battery meter](https://www.youtube.com/watch?v=Dv1gESdI6rU) inside ESC enclosure. 

Just installed Unity in my build and cruise control is now working with both motors.
```

---
## \#200 Posted by: KrisKraanen Posted at: 2018-12-30T02:02:34.806Z Reads: 279

```
Is anybody selling electronic parts kits for this build, and at what price would be intrested, I prefer to buy a kit than to source the parts myself
```

---
## \#201 Posted by: Chrisjarram Posted at: 2018-12-30T22:34:23.459Z Reads: 278

```
For the battery I found this 1200mah one on Amazon which fits the sizing almost perfectly if it helps anyone...

sourcing map Power Supply DC 3.7V 1200mAh 603450 Li-ion Rechargeable Lithium Polymer Li-Po Battery https://www.amazon.co.uk/dp/B07DM49DQ3/ref=cm_sw_r_cp_apa_i_7DukCb8RSMJA5
```

---
## \#202 Posted by: hanyelkomy Posted at: 2019-01-08T09:16:54.402Z Reads: 275

```
[quote="DroidSector, post:16, topic:72916"]
Thanks! I’ll update the code in the future to match your RemoteDisplay.cpp file, so it would be easy to change the display and use this mod, for example:
[/quote]


Awesome job bro,, cant wait till u finalize it with the cheap *Heltec v2*.
Meanwhile could u please send me the  RemoteDisplay.cpp for the bigger display for the original firefly remote?
```

---
## \#203 Posted by: Jamie42 Posted at: 2019-01-08T17:30:38.114Z Reads: 273

```
Got my Heltec v2's. Tried to let them connect but the output of the receiver is as follows:

> ESP3�␂␋#␡␡␀␀␀␀␀␀␀␀h?␃␂␁␄@�␃␂␁␄@�␃␂␁␄@�␃␂␋#␡␡␀␀␀␀␀␀␀␀h?

Going on and on... Any help?
```

---
## \#204 Posted by: DroidSector Posted at: 2019-01-10T06:48:06.208Z Reads: 286

```
@hanyelkomy The Heltec support is ready, I just need to update docs. The schematics is almost the same, just use these pins:

    #define LED           25  
    #define PIN_BUTTON    12
    #define PIN_TRIGGER   32
    #define ADC_THROTTLE  38 
    #define PIN_VIBRO     17

I think you can easily adapt drawMainPage() function:
https://github.com/DroidSector/FireFly-Nano-Remote/blob/91f9380affbac62cd74b10675874fa79fc0adc8d/src/remote/remote.cpp#L1258

@Jamie42 I had the similar issues, please check that serial monitor baudrate set to 115200 and click the reset button on the board a few times.
```

---
## \#207 Posted by: Jamie42 Posted at: 2019-01-16T19:45:02.130Z Reads: 263

```
@DroidSector Baudrate was already set right. Tried the reset button. Maximum that I can get out of it is this:

    Receiver�␂␋#␡␡␀␀␀␀␀␀␀␀h?␃␂␁␄@�␃␂␋#␡␡␀␀␀␀␀␀␀␀h?␃␂␋#␡␡␀␀␀␀␀␀␀␀h?␃␂␋#␡␡␀␀␀␀␀␀␀␀h?␃␂␋#␡␡␀␀␀␀␀␀␀␀h?␃␂␋#␡␡␀␀␀␀␀␀␀␀h?␃␂␋#␡␡␀␀␀␀␀␀␀␀h?␃␂␋#␡␡␀␀␀␀␀␀␀␀h?␃ets Jun  8 2016 00:22:57

	rst:0x1 (POWERON_RESET),boot:0x13 (SPI_FAST_FLASH_BOOT)
	configsip: 0, SPIWP:0xee
	clk_drv:0x00,q_drv:0x00,d_drv:0x00,cs0_drv:0x00,hd_drv:0x00,wp_drv:0x00
	mode:DIO, clock div:2
	load:0x3fff0018,len:4
	load:0x3fff001c,len:952
	load:0x40078000,len:6084

	load:0x40080000,len:7944
	entry 0x40080310
	Receiver�␂␋#␡␡␀␀␀␀␀␀␀␀h?␃␂␁␄@�␃␂␁␄@�␃␂␁␄@�␃␂␋#␡␡␀␀␀␀␀␀␀␀h?␃␂␁␄@�␃␂␁␄@�␃Receiver�␂␋#␡␡␀␀␀␀␀␀␀␀h?␃␂␁␄@�␃␂␋#␡␡␀␀␀␀␀␀␀␀h?␃␂␋#␡␡␀␀␀␀�ets Jun  8 2016 00:22:57

	rst:0x1 (POWERON_RESET),boot:0x13 (SPI_FAST_FLASH_BOOT)
	configsip: 0, SPIWP:0xee
	clk_drv:0x00,q_drv:0x00,d_drv:0x00,cs0_drv:0x00,hd_drv:0x00,wp_drv:0x00
	mode:DIO, clock div:2
	load:0x3fff0018,len:4
	load:0x3fff001c,len:952
	load:0x40078000,len:6084
	load:0x40080000,len:7944
	entry 0x40080310
	Receiver�␂␋#␡␡␀␀␀␀␀␀␀␀h?␃␂␁␄@�␃␂␁␄@�␃␂␁␄@�␃␂␋#␡␡␀␀␀␀␀␀␀␀h?␃␂␁␄@�␃␂␁␄@�␃
```

---
## \#208 Posted by: sanderfu Posted at: 2019-01-16T21:17:23.254Z Reads: 252

```
@DroidSector Will this TTGO board fit in the Heltec version of the remote? Also, I am unable to see a version number, but it uses the LoRa SX1276 chip like the heltec, do you think it will work?

https://www.aliexpress.com/item/2pcs-of-TTGO-LORA32-868-915Mhz-SX1276-ESP32-Oled-display-Bluetooth-WIFI-Lora-development-board/32841743946.html?spm=a2g0s.13010208.99999999.266.16f33c00r1yfaZ
```

---
## \#209 Posted by: DroidSector Posted at: 2019-01-19T09:36:05.514Z Reads: 251

```
@Jamie42 Is it connected to vesc? 

@sanderfu It doesn't have a battery probe, can you get this one instead?
https://www.amazon.com/MakerFocus-Development-Bluetooth-0-96inch-Display/dp/B076MSLFC9/ref=sr_1_5?keywords=LoRa+ESP32&qid=1547889291&sr=8-5
```

---
## \#210 Posted by: sanderfu Posted at: 2019-01-19T11:32:55.277Z Reads: 247

```
What do you mean by battery probe? I spoke with the seller of the one you have in you spreadsheet, and he says it will be back in a couple of days :slight_smile:
```

---
## \#211 Posted by: DroidSector Posted at: 2019-01-19T11:50:43.146Z Reads: 247

```
That's good! It allows measuring the voltage of the battery connected to the remote.
```

---
## \#212 Posted by: sanderfu Posted at: 2019-01-19T11:54:29.871Z Reads: 251

```
I see, so itslike an ADC input-pin the board I linked is missing then if I understood correctly. A bit wierd, cause on the pinout it looks like it has several pins for measuring analog signal.

Was looking for one without a screen with white colour, could I use tge TTGO board with no screen that you have linked before and just connect a 0.96 inch lcd to it? Would that fit in the remote?
```

---
## \#213 Posted by: HSGeorge Posted at: 2019-01-19T12:08:10.619Z Reads: 236

```
Is there anyway to get this working with the Heltec 433-470mhz version
```

---
## \#214 Posted by: DroidSector Posted at: 2019-01-19T22:12:49.109Z Reads: 231

```
You'll need to connect battery and ADC pins, which will be tricky. The screen as well:

https://www.electric-skateboard.builders/t/firefly-nano-remote/[72916/192](tel:72916192)?u=droidsector

You can build the Firefly version or buy a remote from @StefanMe.
```

---
## \#215 Posted by: DroidSector Posted at: 2019-01-19T22:17:02.558Z Reads: 231

```
Yes, just make sure it's version 2. There is an AliExpress link in the parts list (Europe tab).
```

---
## \#216 Posted by: sanderfu Posted at: 2019-01-20T00:04:34.394Z Reads: 231

```
Thanks for the reply mate, I am going with heltec board in your part list when it becomes available again I think 'cause I really like the design and feel of your remote.
```

---
## \#217 Posted by: fabu Posted at: 2019-01-22T19:49:45.786Z Reads: 240

```
hi @all
I have tried to setup both heltec v2 but I don´t get them connected.
Also the values on the remote are turning like the voltage from low to high (3.9V to 4.3) and for example some values in the line above like 0 ... 1023 ...127 - I think the values for the hall sensor?
What can I do now?
I am a little confused.
But in the end, a really nice a very powerfull code :-) respect.
bye Fabian
```

---
## \#218 Posted by: gmurad Posted at: 2019-02-02T20:33:34.219Z Reads: 234

```
@DroidSector Thanks for making this. 
Been wanting to buy a 3D printer for a while and this project pushed me over the edge (getting a CR10S PRO). Are you able to update the docs for the new micro-controller(Heltec v2)? e.g.: https://github.com/DroidSector/FireFly-Nano-Remote/wiki/2.-Electronics
```

---
## \#219 Posted by: gmurad Posted at: 2019-02-03T22:11:58.240Z Reads: 237

```
I want to build this remote with the Heltec V2 board.

General question for anyone who uses this remote. What is the state of this remote in terms of reliability? Is it good enough to use on a daily basis?
```

---
## \#220 Posted by: DroidSector Posted at: 2019-02-06T03:11:24.448Z Reads: 246

```
It’s reliable enough, but not all safety features are implemented yet. For example, if the battery on the remote dies, the board will continue going.

The schematics is almost the same, just use these pins:

```
#define LED           25  
#define PIN_BUTTON    12
#define PIN_TRIGGER   32
#define ADC_THROTTLE  38 
#define PIN_VIBRO     17
```

I'm currently busy with another project (TeraCopy for Mac) but will continue working on the remote very soon.
```

---
## \#221 Posted by: Boeufsk8 Posted at: 2019-02-10T02:09:15.970Z Reads: 241

```
So I'm in the process of building the feather version of this remote and in the wiring diagram it says that the uart of my VESC needs to connect to the 3.3V, rx, tx and ground. I'll be using the Focbox for my board and was wondering if anyone could tell me how to hook it up to that VESC? I see it has an rx and tx connection but I will be using those for a metre pro so I'm a little confused about where to make the connection.
```

---
## \#222 Posted by: DroidSector Posted at: 2019-02-11T13:19:41.765Z Reads: 240

```
With Unity it would be more complicated since both receiver and Metre are using the same tx/rx connection. I'll try to connect Unity with the receiver using PPM cable tomorrow.
```

---
## \#223 Posted by: DroidSector Posted at: 2019-02-21T08:10:35.743Z Reads: 239

```
A few updates for the remote:
- More efficient sleep mode.
- Better remote battery display, show text values when < 10%.
- No vibration on remote startup, to avoid boot loop on low battery.
- Safer min voltage 3.1 > 3.3v.
```

---
## \#224 Posted by: ccgpandora Posted at: 2019-02-23T06:03:30.429Z Reads: 239

```
Got everything together and connected using Flipsky 6.6 Dual plus. Only getting one motor to spin though (master ESC side with receiver connection). Setup slave and master per the instructions. Not sure if it is on the remote or esc side. Both motors get power when calibrating. Is the software compatible with VESC 6 firmware?
```

---
## \#225 Posted by: DroidSector Posted at: 2019-02-23T07:06:17.119Z Reads: 244

```
I've only tested it with Flipsky 4.2 Dual and Unity, but I think it should also work with 6.6. 

Master:
![Annotation%202019-02-23%20064840|345x222](upload://vSKdN6BC7NZ1DOFLBTStMkDHCFX.jpeg) 

![Annotation%202019-02-23%20064925|344x194](upload://89k8pmZoLljiYZjIzq90vv2y8IR.jpeg) 

Slave:
![Slave|345x209](upload://6p8m4lBYT5O8pZUkNx9IDUk0B31.jpeg) 

Send CAN Status = true on the slave and different VESC IDs are the main requirements. It could be also just a glitch, try to restart the VESC and do Input Setup Wizard again for both salve and master.
```

---
## \#226 Posted by: ccgpandora Posted at: 2019-02-23T08:08:51.063Z Reads: 229

```
Yea those are the exact settings I have. I have gone through the setup multiple times on both the slave and master VESC. Starting to think my board is defective or something. The green light on both sides are on. It gets brighter with forward throttle on the master side and the motor spins. On the slave side it only gets brighter when the brake is applied.
```

---
## \#227 Posted by: McEboards Posted at: 2019-02-24T06:31:59.922Z Reads: 235

```
I plan on making a few batches of the Firefly remote come June, July, August. I am an engineering student looking to make some extra dough this summer alongside my Co-Op. I want one myself and know it would be smart to help meet the high demand for this remote for some other people. I plan on making them to order once I am done with this semester. Let me know if you would be interested in purchasing one in the future. Thanks.

Email: Brendan.McClanahan@yahoo.com
```

---
## \#228 Posted by: ccgpandora Posted at: 2019-02-24T21:33:11.667Z Reads: 229

```
Eureka! So I figured it out and now have both motors functioning with the remote. For whatever reason turning on the nunchuk settings to current no reverse fixed everything for me. I was so certain I got a bad Flipsky board. Now to just finish the build... oh I was reading earlier in the post. My sensitivity is also super high and the 0-100% speed is very quick with little increase in throttle input even after calibrating. Will have to tinker with code more. This has all been such a learning experience for me!
```

---
## \#229 Posted by: chickengun Posted at: 2019-03-03T14:41:58.106Z Reads: 229

```
@DroidSector Is the part list still up to date?
https://docs.google.com/spreadsheets/d/13rUPX8BsSac1AdnFAXx4dwR3XoQiU4FAKbunFaeW-oY/edit#gid=0

I haven't keep track, are the Heltec Lora modules from aliexpress your prefered choice?

For the hall sensor you recommend DRV5053OAQLPG. Is it ok to use SS495A1 instead?
https://aliexpress.com/item/5pcs-SS495A1-TO-92L-95A-TO-92-high-precision-Hall-SS495A-screen-95A-new-original/32882688006.html
```

---
## \#230 Posted by: DroidSector Posted at: 2019-03-04T09:16:31.805Z Reads: 221

```
Heltec is cheaper and has more features. I've just implemented receiver update via WiFi. Auto stop on connection loss is mostly ready. 

According to specs, SS495A1 requires 4.5 V voltage. But it might work, please test it if you already have it.
```

---
## \#231 Posted by: StefanMe Posted at: 2019-03-04T09:18:02.935Z Reads: 223

```
Do i see this correct, u dont use the PPM as signal. U go straight over UART and the nunchuck variables?
```

---
## \#232 Posted by: DroidSector Posted at: 2019-03-04T09:22:23.187Z Reads: 223

```
Yes, I've tested PPM control with Feather, but not with Heltec. I guess it should work as well, I'll test it soon.
```

---
## \#233 Posted by: alanwong Posted at: 2019-03-04T14:23:37.042Z Reads: 235

```
Hi DroidSector,

I have problem to get the board ID from the receiver. The Receiver.Heltec.v2 has been uploaded successful. After that, I use PlatformIO to monitor the serial print but it cannot show the correct ID like 0x.... Would you help me? Thank you.
![unnamed%20(1)|325x500](upload://b5f1XVPrVWjBCD9aIgWBUjgu10v.jpeg)
```

---
## \#234 Posted by: DroidSector Posted at: 2019-03-05T03:03:20.366Z Reads: 234

```
Try pressing the reset button on Heltec. 

You can also temporarily replace this line:

    display.print("Remote not connected");

with this line:

    display.print(String(CPU::getID(), HEX));

at this location:

https://github.com/DroidSector/FireFly-Nano-Remote/blob/62c7e264d4d1e3fc18385538f683eca3b4bb1205/src/receiver/receiver.cpp#L154
```

---
## \#235 Posted by: alanwong Posted at: 2019-03-07T03:21:36.812Z Reads: 221

```
Thanks for your help. But still cannot show the ID after replace the code.:pensive:

Code uploaded successful 
![20190307_110023|666x500](upload://98v4pPdUJtRVhfi2p9ZTzAQieYZ.jpeg)
```

---
## \#236 Posted by: alanwong Posted at: 2019-03-07T03:22:08.797Z Reads: 225

```
Serial monitor setting
![20190307_110104|666x500](upload://dXjf0SjbLOwoYzA58lP8MuXPdim.jpeg)
```

---
## \#237 Posted by: alanwong Posted at: 2019-03-07T03:23:09.358Z Reads: 225

```
Only show Null....
![20190307_110112|666x500](upload://gspLPtgn8N0l3g7fD6BQgc8FC6k.jpeg)
```

---
## \#238 Posted by: KrisKraanen Posted at: 2019-03-10T22:40:23.777Z Reads: 215

```
anybody selling electronics kits? Feather version or Heltec
```

---
## \#239 Posted by: KrisKraanen Posted at: 2019-03-10T22:43:54.540Z Reads: 219

```
and instead of Heltec module https://www.banggood.com/2Pcs-Wemos-TTGO-LORA32-868915Mhz-ESP32-LoRa-OLED-0_96-Inch-Blue-Display-p-1239769.html?rmmds=search&cur_warehouse=CN does this one also work?
```

---
## \#240 Posted by: DroidSector Posted at: 2019-03-11T04:21:35.242Z Reads: 221

```
@alanwong Try to upload the code for the receiver to another board. You should see board id on the OLED screen.

@KrisKraanen With this board, you won't be able to see the remote battery level, which is rather critical information. It might not fit properly in the remote case as well.
```

---
## \#241 Posted by: sami Posted at: 2019-03-11T08:15:17.652Z Reads: 222

```
@DroidSector can I use the same hall-sensor from SolidGeeks build?
 the SS495A TO-92 SS495A1 95A Linear Hall-Effect Sensor
```

---
## \#242 Posted by: willumpie82 Posted at: 2019-03-11T08:41:10.872Z Reads: 210

```
Would it be feasible to make a receiver module that can connect to the CANbus instead of UART/PPM? this way we might also be able to fetch battery data from e.g. DieBieMS from @JTAG 

even wilder dream with a 4wd board it would become possible to make it steer/turn by controlling 4 VESCs independently
```

---
## \#243 Posted by: floyd Posted at: 2019-03-11T17:46:45.421Z Reads: 206

```
I seem to have the same issue as you.. I don't get anything displayed on the receiver oled, but remote works fine. And serial monitor has same output.
```

---
## \#244 Posted by: Jamie42 Posted at: 2019-03-11T18:25:56.871Z Reads: 197

```
Same here.
```

---
## \#247 Posted by: krazor Posted at: 2019-03-12T11:28:08.965Z Reads: 205

```
Ok so i found and ordered the parts from where i could in Aus but i cant seem to find this hall effect sensor, they want to charge me over $25 USD to ship the dam thing to Australia. so far this builds cost is about $165 without the sensor. if anyone has a couple spares in aus or knows whereelse i can get them from with reasonable shipping prices that would be great
```

---
## \#248 Posted by: StefanMe Posted at: 2019-03-12T11:29:53.338Z Reads: 203

```
Search for an SS49E sensor
```

---
## \#249 Posted by: krazor Posted at: 2019-03-12T11:31:55.075Z Reads: 208

```
someone linked this above, https://www.aliexpress.com/item/5pcs-SS495A1-TO-92L-95A-TO-92-high-precision-Hall-SS495A-screen-95A-new-original/32882688006.html

does it have to be exactly or would this give same results or different?

Sorry i just checked that requires a higher voltage to use, and there hasnt been a response for it. thanks for the info i will see if i can find this specific sensor you mentioned
```

---
## \#250 Posted by: StefanMe Posted at: 2019-03-12T11:32:37.912Z Reads: 201

```
I dont know... i can just recommend this one...

https://de.aliexpress.com/wholesale?catId=0&initiative_id=SB_20190312033210&SearchText=SS49E

This type i use on all my FeatherRemote builds.
```

---
## \#251 Posted by: krazor Posted at: 2019-03-12T11:34:20.272Z Reads: 201

```
thanks, im building the feather remote, but the dam things are $48 each in my country, we get so ripped off here =/ that link you provided takes me to ali express but it doesnt take me to the product just a selection of them
```

---
## \#252 Posted by: StefanMe Posted at: 2019-03-12T11:37:42.848Z Reads: 197

```
All of theses products will work... just pick one...
```

---
## \#253 Posted by: krazor Posted at: 2019-03-12T11:56:13.284Z Reads: 198

```
thanks all parts sorted.
```

---
## \#254 Posted by: mptrs Posted at: 2019-03-14T18:49:29.062Z Reads: 196

```
https://www.electric-skateboard.builders/t/firefly-nano-remote/72916/167?u=mptrs

hope this helps
```

---
## \#255 Posted by: KrisKraanen Posted at: 2019-03-15T12:40:42.874Z Reads: 190

```
I am building your heltec version, do you have a wiring digram for this one aswell? Or build video, with how long to cut wires where to rout them etc
```

---
## \#257 Posted by: KrisKraanen Posted at: 2019-03-15T13:06:58.096Z Reads: 192

```
Im not good with coding but is there way to add an relay switch on the reciever thats activated with double tapping the deadmans switch when standing still and is there a way to add my own startup photo/logo
```

---
## \#258 Posted by: KrisKraanen Posted at: 2019-03-17T18:46:51.830Z Reads: 201

```
Abother fearure idea: since the board has wifi (and Bluetooth?) Trip recording via Phone Gps connection?
```

---
## \#259 Posted by: tobias Posted at: 2019-03-19T20:54:21.606Z Reads: 205

```
Hi everyone, 
I run into the same problem with my Heltec receiver. 
I tried the reset button, replace the line: display.print... and to upload the code to another board. But it didn’t work. 

![image|666x500](upload://h6NY7VtlnMJ4y0JkVR5Q1x9xnuO.jpeg) 

@Jamie42  @alanwong  Have you found a solution ?

Thanks for your help.
```

---
## \#260 Posted by: Michaelj1 Posted at: 2019-03-20T00:27:16.686Z Reads: 191

```
im trying to make a regular firefly remote just with a larger screen, what code needs to be changed to make this display work with the original firefly code by solidgeek? also how is the display soldered to the nano? is it the same way as the original OLED display?
```

---
## \#261 Posted by: alanwong Posted at: 2019-03-20T00:40:33.334Z Reads: 183

```
not yet.....
```

---
## \#262 Posted by: DroidSector Posted at: 2019-03-20T02:47:24.231Z Reads: 203

```
I've already implemented an automatic pairing, will upload the code in a few hours. Meanwhile, you can comment out the address check block to make the receiver accept all remotes:

https://github.com/DroidSector/FireFly-Nano-Remote/blob/62c7e264d4d1e3fc18385538f683eca3b4bb1205/src/receiver/receiver.cpp#L261

@KrisKraanen Good idea, is this one ok? This feature will be easy to add. 

https://www.aliexpress.com/item/TOP-MOSFET-Button-IRF520-MOSFET-Driver-Module-for-Arduino-ARM-Raspberry-pi/32640051724.html

I guess you can update logo array in remote.h with this app: https://www.riuson.com/en/lcd-image-converter
```

---
## \#263 Posted by: StefanMe Posted at: 2019-03-20T07:54:36.946Z Reads: 188

```
Really impressive work! Awesome. The code is awesome! 

Looks like u forgot to implement the Smoothed.h

    ******************************************************************
    * Looking for Smoothed.h dependency? Check our library registry!
    *
    * CLI  > platformio lib search "header:Smoothed.h"
    * Web  > https://platformio.org/lib/search?query=header:Smoothed.h
    *
    ******************************************************************

I added it manually
```

---
## \#264 Posted by: KrisKraanen Posted at: 2019-03-20T12:16:51.612Z Reads: 191

```
Should be fine mosfet or relay will both work, i have this board still laying around https://m.banggood.com/nl/5V-Relay-1-Channel-Module-One-Channel-Relay-Expansion-Module-Board-p-91800.html?gmcCountry=NL&currency=EUR&cur_warehouse=CN&createTmp=1&ID=227&utm_source=googleshopping&utm_medium=cpc_bgs&utm_content=frank&utm_campaign=pla-nl-elc2-pc-nl&gclid=CjwKCAjwycfkBRAFEiwAnLX5ITXGKQ0_1lDUorxwmYdicsa5z4l8Gr-GayEd2CMFKbgtx4wkKmIcNBoCWlMQAvD_BwE
```

---
## \#265 Posted by: DroidSector Posted at: 2019-03-20T14:03:16.983Z Reads: 200

```
Just uploaded the new code. Description of new settings and features:

**Auto-pairing**

Just compile and upload as is (keep FAKE_UART). The remote will pair automatically.

    #define FAKE_UART // Comment out after pairing the remote and connecting VESC

**Unity support**

    // const COMM_PACKET_ID VESC_COMMAND = COMM_GET_VALUES; // VESC
    const COMM_PACKET_ID VESC_COMMAND = COMM_GET_UNITY_VALUES; // Enertion Unity

**Endless ride**

For now, it's more for situations when remote is out of power. Just push with a speed over 12 km/h for 3 seconds and stand still. Cruise control will be activated for 30s when speed drops below 12 km/h.

Slide the board backward while standing on it or foot brake to produce a spike in the current and stop the board. Please test it first in an open space and be ready to turn on the remote.

    const bool  AUTO_CRUISE_ON = false;     // disabled by default
    const float PUSHING_SPEED = 12.0;       // km/h
    const float PUSHING_TIME = 3.0;         // seconds
    const float CRUISE_CURRENT_SPIKE = 5.0; // Amps

Board will stop after 30 seconds if the current is low (flat ground).

    const float AUTO_CRUISE_TIME = 30.0;    // seconds
    const float CRUISE_CURRENT_LOW = 5.0;   // Amps

Auto-stop if remote is not connected and speed is over 20 km/h - not tested yet!

    const float MAX_PUSHING_SPEED = 20.0;   // km/h

**Auto-stop**

The receiver will apply gradual breaking if the connection with the remote is lost.

    const float AUTO_BRAKE_TIME = 5.0;    // time to apply the full brakes
    const int AUTO_BRAKE_RELEASE = 5;     // time to release brakes after the full stop

The display will turn on only if the battery charge > 15% to avoid boot loop.

    const int DISPLAY_BATTERY_MIN = 15;

**OTA updates**

Future updates for the receiver can be applied over WiFi. Just set your network name and password in receiver.cpp. 

platformio.ini:

    ; upload_port = 192.168.1.x ; IP from receiver screen
```

---
## \#266 Posted by: tobias Posted at: 2019-03-20T21:23:42.147Z Reads: 202

```
@DroidSector awesome work !  
I forgot to change the frequency to 433 MHz. The pairing is now working.

But the connection to the FOCBOX is not working (LED is constantly blinking).
Do I need to make some configurations in the BLDC tool? Baudrate is set to 115200.

Focbox   —  reciever      
  5V   <====>  5V  
GND <==>  GND  
RX   <====>  TX  
TX <====>  RX

![image|375x500](upload://zyl00jkp0wUpL7P5GpC4TbsJ6sO.jpeg) ![image|690x336](upload://GEezrtzYLL2gqseufbm1FMvcXx.jpeg)
```

---
## \#267 Posted by: StefanMe Posted at: 2019-03-20T22:48:08.316Z Reads: 189

```
Awesome!

Is there no running compiling code for the TTGO REMOTE? I Just see a TTGO RECEIVER...?

Thx
```

---
## \#268 Posted by: Sn4pz Posted at: 2019-03-20T22:56:14.853Z Reads: 189

```
Is there any easy fix to the previous connectivity issues that the Firefly has @DroidSector ?

Amazing work by the way, you're convincing me that maybe I should buy a nano in white.... Instead of the maytech waterproof remote...

How many other code improvements do you think you'll be doing for the Firefly? :)
```

---
## \#269 Posted by: DroidSector Posted at: 2019-03-21T03:59:01.335Z Reads: 187

```
@StefanMe thanks! Just add the target like this:

    env_default = Remote.TTGO.OLED.v1

@tobias the last build is for Unity by default, make sure to uncomment COMM_GET_VALUES.
```

---
## \#270 Posted by: DroidSector Posted at: 2019-03-21T04:31:42.670Z Reads: 191

```
@Sn4pz if you're talking about getting receiver ID, it's not needed anymore, since pairing is automatic now.

I still need to add pairing to a new board, configuration menus, trip statistics... Mobile apps for tracking and updating firmware in some distant future :)
```

---
## \#271 Posted by: Sn4pz Posted at: 2019-03-21T04:41:13.235Z Reads: 188

```
Very interested ;) 

Thanks for the explanation
```

---
## \#272 Posted by: krazor Posted at: 2019-03-21T04:54:36.086Z Reads: 202

```
If anyone is interested in having them printed i have a few printed and painted that i would be willing to sell. I would be willing to supply other hardware pieces as well if you like however the hardware is on order.

These would come with all printed parts, Painted if you like or in plain white/grey. these are printed with 3D Fillies PLA+  there is option for PETG also if you want even stronger and heat resilient.

PLA+<br>
$20 printed & painted with a gloss finish<br>
$10 printed no paint, will come in either white or grey<br>

PETG<br>
$26.50 Printed & painted with gloss finish<br>
$16.50 Printed Will come in either grey or white<br>

if you want to get other parts printed check out my thread [Here](https://www.electric-skateboard.builders/t/wts-3d-printing-services-australia-melbourne-based/87820)

Shipping is extra

If this is the wrong place to put this post i can have it removed, Just let me know.

Note this is the Feather version, other versions or files can be printed if you like.


![IMG_20190321_145532|666x499](upload://rrnqWu2xlziDdOCFigVmaMzn2uw.jpeg) ![IMG_20190321_150833|666x499](upload://q5oGQcRGUfqhTRYss7LUz66hxDB.jpeg) ![IMG_20190321_150934|666x499](upload://jguFqB5s0bGO753kz8IOgf3i9PA.jpeg) ![IMG_20190321_151203|666x499](upload://eyfNL9ZtSo6BtKgYncQ66wc8w2N.jpeg) ![IMG_20190321_151326|666x499](upload://yn0v1XrI3siV4PD47azUYCHPSNl.jpeg)
```

---
## \#273 Posted by: DroidSector Posted at: 2019-03-21T05:09:43.825Z Reads: 186

```
Looks nice! Please keep in mind these parts are for Feather version, would be great if you could offer this one as well: https://www.thingiverse.com/thing:3303495

Since I can't edit the first post anymore, I'll make a new topic for Heltec version soon to separate these two versions.
```

---
## \#274 Posted by: krazor Posted at: 2019-03-21T05:11:38.767Z Reads: 186

```
yes that is correct, this is for the feather version i forgot there were 2. i will update post and thank you for reminding me. I can print out any version if another is required. @DroidSector that would be great, also you dont mind me using your designs to print and paint?
```

---
## \#275 Posted by: DroidSector Posted at: 2019-03-21T06:15:39.035Z Reads: 188

```
Not at all, the price is reasonable and I don't have time to do it myself anyway.
```

---
## \#276 Posted by: krazor Posted at: 2019-03-21T06:20:24.638Z Reads: 182

```
thank you, I thought the prices were around the right price of something i would pay, And i'm currently trying to fill in my time since i'm still job hunting =(
```

---
## \#277 Posted by: hanyelkomy Posted at: 2019-03-21T10:31:32.467Z Reads: 181

```
[quote="DroidSector, post:89, topic:72916"]
software battery meter
[/quote]

Hi, Great remote... thanks for the hard work
I was wondering if you can share the code for the receiver with the battery meter function?

Thanks
```

---
## \#278 Posted by: DroidSector Posted at: 2019-03-21T10:59:29.297Z Reads: 170

```
The current code for the receiver already contains this feature.
```

---
## \#279 Posted by: hanyelkomy Posted at: 2019-03-21T11:22:46.601Z Reads: 170

```
ok so i have not hooked the receiver to the vesc yet, but so far the code is ruining on the receiver and remote (helltec2) and there is no any data on the receiver screen
```

---
## \#280 Posted by: tobias Posted at: 2019-03-21T11:44:33.975Z Reads: 178

```
[quote="DroidSector, post:269, topic:72916"]
@tobias the last build is for Unity by default, make sure to uncomment COMM_GET_VALUES
[/quote]
 
I already changed that to VESC, but thanks for the advice.  
The problem still exists. 
But the LED (from the controller) also blinks constantly after uploading the code and pairing the two boards  
the first time (with FAKE_UART).
Is this the way it should be ?
```

---
## \#281 Posted by: StefanMe Posted at: 2019-03-21T11:46:01.103Z Reads: 173

```
Same for me... I tried the TTGO and my screen stays off. 

TTGO is not connected to VESC or remote.
```

---
## \#282 Posted by: Sn4pz Posted at: 2019-03-21T12:06:35.674Z Reads: 179

```
Very interested in this! PMing you
```

---
## \#283 Posted by: DroidSector Posted at: 2019-03-21T16:13:36.900Z Reads: 190

```
@StefanMe @hanyelkomy try to add this line:  

    display.powerOn();

https://github.com/DroidSector/FireFly-Nano-Remote/blob/e3390a121d13bde45506a914bc7bd54b3da4adc9/src/receiver/receiver.cpp#L107

For some reason display works on my boards even without this line :thinking:
```

---
## \#284 Posted by: DroidSector Posted at: 2019-03-21T16:59:54.024Z Reads: 176

```
I'm getting garbage on Serial monitor too if VESC is not connected. Try to reduce baud rate both in BLDC tool and in global.h in (UART_SPEED). Maybe also connect 3.3v <==> 3.3v just in case.
```

---
## \#285 Posted by: deltazeta Posted at: 2019-03-21T18:16:33.124Z Reads: 176

```
Did you ever get the heltec working with ack's vesc android app? would be cool to use the app with a faster bluetooth module.
```

---
## \#286 Posted by: floyd Posted at: 2019-03-22T01:20:07.245Z Reads: 173

```
I think the issue with no display on the receiver has something to do with this error i'm getting from serial monitor:
[E][esp32-hal-i2c.c:1426] i2cCheckLineState(): Bus Invalid State, TwoWire() Can't init sda=0, scl=0

Not sure how to go about fixing it though. I've tried adding display.powerOn() and messing around with the code a bit but haven't been able to get any display or get rid of that error.
```

---
## \#287 Posted by: DroidSector Posted at: 2019-03-22T05:07:56.504Z Reads: 184

```
Does the display work if you upload transmitter's code instead?

Looks like DISPLAY_SDA and DISPLAY_SCL are not initialized, try to set it manually:

    Wire.begin(4, 15); 

https://github.com/DroidSector/FireFly-Nano-Remote/blob/e3390a121d13bde45506a914bc7bd54b3da4adc9/lib/Adafruit_SSD1306/src/Adafruit_SSD1306.cpp#L169
```

---
## \#288 Posted by: DroidSector Posted at: 2019-03-22T05:18:21.038Z Reads: 164

```
[quote="deltazeta, post:285, topic:72916"]
Did you ever get the heltec working with ack’s vesc android app?
[/quote]
No, only with the original app. It might be tricky to use both radios at once, maybe have the receiver record the data and download it later over WiFi...
```

---
## \#289 Posted by: hanyelkomy Posted at: 2019-03-22T11:15:00.391Z Reads: 175

```
its still not working even after i did this changes

 #ifdef 

RECEIVER_SCREEN

    display.begin(SSD1306_SWITCHCAPVCC, 0x3C);
    display.powerOn();
  #endif

-----------------------------------------------------------------------
    Wire.begin(4, 15);
    Wire.begin(DISPLAY_SDA, DISPLAY_SCL);

    Wire.setClock(700000);

also even if removed 
 Wire.begin(DISPLAY_SDA, DISPLAY_SCL);

yes display work with the remote code
```

---
## \#290 Posted by: DroidSector Posted at: 2019-03-22T11:24:07.129Z Reads: 166

```
That's very strange, I have exactly the same code and it works on Mac and PC machines. Maybe removing #ifdef RECEIVER_SCREEN everywhere will help.
```

---
## \#291 Posted by: hanyelkomy Posted at: 2019-03-22T11:40:12.542Z Reads: 172

```
[quote="DroidSector, post:290, topic:72916"]
#ifdef RECEIVER_SCREEN
[/quote]

all the way to (endif) ?
```

---
## \#292 Posted by: DroidSector Posted at: 2019-03-22T11:55:05.853Z Reads: 174

```
No, we need the display-related code between #ifdef and #endif to work for sure, so delete only  #ifdef and  #endif lines. You can remove code inside ARDUINO_SAMD_ZERO block, it's for Feather only.
```

---
## \#293 Posted by: hanyelkomy Posted at: 2019-03-22T12:22:32.643Z Reads: 178

```
i did that still nothing though
```

---
## \#294 Posted by: krazor Posted at: 2019-03-24T01:09:00.429Z Reads: 172

```
just curious to ask were the PCB files available to download anywhere i cant seem to find the, in the thread?
```

---
## \#295 Posted by: DroidSector Posted at: 2019-03-24T13:15:55.079Z Reads: 176

```
Well, after a lot of debugging with @hanyelkomy the display on the receiver should work now. Looks like in recent versions of Heltec in addition to the battery voltage divider VEXT also powers the display. Which is good, it should save more power in the sleep mode.
```

---
## \#296 Posted by: SanderG Posted at: 2019-03-24T17:35:38.391Z Reads: 174

```
Whats the best board to buy? heltec or feather?
```

---
## \#297 Posted by: StefanMe Posted at: 2019-03-24T19:08:53.848Z Reads: 170

```
Difficult. The feather is better but the Heltec has the build in OLED...
```

---
## \#298 Posted by: SanderG Posted at: 2019-03-24T20:01:21.616Z Reads: 169

```
Why is the feather better? What can it do more?
```

---
## \#299 Posted by: tobias Posted at: 2019-03-24T20:11:17.628Z Reads: 175

```
Nice work ! 
The display on the reciever is now working. 
[quote="DroidSector, post:284, topic:72916"]
I’m getting garbage on Serial monitor too if VESC is not connected. Try to reduce baud rate both in BLDC tool and in global.h in (UART_SPEED). Maybe also connect 3.3v &lt;==&gt; 3.3v just in case
[/quote]

I set the baudrate down to 9600, but still not working (no UART data).
I also checked the FOCBOX firmware version, 2.18.
Maybe that’s the problem, too old ?
```

---
## \#300 Posted by: Jamie42 Posted at: 2019-03-24T20:13:03.891Z Reads: 172

```
Same here! Got both screens working now but no UART data. Tried 9600 bauds but still no data. Also on FOCBOX (not unity) version 2.18.
```

---
## \#301 Posted by: nirurin Posted at: 2019-03-24T20:37:11.453Z Reads: 171

```
I really like this remote, especially the little OLED, it's very smart and exactly what is needed! 

I don't suppose there's anyone who has already got a bunch of parts (or a kit) in the UK that has gone spare that I could purchase as a set? Just thought I'd ask before I try and go through the individual parts list. 

Also as I'm in the EU don't I need a different reciever to the 915mhz?
```

---
## \#302 Posted by: tobias Posted at: 2019-03-24T21:24:55.757Z Reads: 177

```
[quote="nirurin, post:301, topic:72916"]
Also as I’m in the EU don’t I need a different reciever to the 915mhz?
[/quote]

Yes, the Heltec board with 433Mhz.

https://www.aliexpress.com/item/2PCS-New-Version-433MHZ-868MHz-915MHz-SX1276-SX1278-ESP32-LoRa-OLED-Bluetooth-WIFI-Lora-Kit-32/32886711232.html?spm=a2g0s.9042311.0.0.27424c4dmxnVsu
```

---
## \#303 Posted by: Jamie42 Posted at: 2019-03-24T22:10:37.330Z Reads: 172

```
Just updated to FW 3.54, still no connection between FOCBOX and Heltec receiver.
```

---
## \#304 Posted by: Chupacabra Posted at: 2019-03-24T22:23:24.264Z Reads: 172

```
Does anyone have a complete remote for sale?
```

---
## \#305 Posted by: DroidSector Posted at: 2019-03-25T03:41:00.309Z Reads: 176

```
Forgot to mention that UART_TIMEOUT should be increased too:

    const int UART_TIMEOUT = 100; // 10ms for 115200 bauds, 100ms for 9600 bauds

VescUart library has an extended debug output, try enabling it with setDebugPort():

    UART.setTimeout(UART_TIMEOUT);
    UART.setDebugPort(Serial);
```

---
## \#306 Posted by: Jamie42 Posted at: 2019-03-25T10:08:05.609Z Reads: 172

```
I already increased the time out too as you stated in the comments. 

Added an & before Serial and tried the setDebugPort but my Serial monitor is spitting out crap.
```

---
## \#307 Posted by: tobias Posted at: 2019-03-25T12:34:18.812Z Reads: 169

```
After I updated the FOCBOX, the receiver is now communicating with the Vesc, but not perfect. The motor is controllable with the remote, the battery voltage is also right,  but the LED is still constantly blinking. It seems the baudrate is not the problem, because I tested it with 9600 and 115200, nothing different. 

When I calibrate the remote with Menu -> Remote -> Calibrate the reciever disconnects and want to connect to WiFi. I thought the calibrate function is for the Hall sensor ?
```

---
## \#308 Posted by: Jamie42 Posted at: 2019-03-25T12:47:04.091Z Reads: 166

```
What FW version are you on now? 

I will try Ackmaniac's firmware too.
```

---
## \#309 Posted by: tobias Posted at: 2019-03-25T16:02:40.187Z Reads: 172

```
FW 3.53 with Vesc-Tool
```

---
## \#310 Posted by: Jamie42 Posted at: 2019-03-25T16:03:19.372Z Reads: 176

```
Okay, I am receiving UART data now but now the screen on the remote is giving me problems. When I upload the code the screen works and shows all telemetry. When I then power it off and power it on again, the screen doesn't turn on. The serial monitor also gives me this error:

    [E][esp32-hal-i2c.c:1146] i2cCheckLineState(): Bus Invalid State, TwoWire() Can't init

Hope you have a solution.


Also a feature suggestion: Throttle Curves
```

---
## \#311 Posted by: DroidSector Posted at: 2019-03-26T11:56:01.579Z Reads: 166

```
It could be just a low battery, try to set this to 0:

    // turn off display if battery < 15%
    const int DISPLAY_BATTERY_MIN = 15;

@tobias LED shows the data exchange, delete `digitalWrite(LED, HIGH)` if it's too annoying. I've just pushed a fix for the Calibration screen.
```

---
## \#312 Posted by: Jamie42 Posted at: 2019-03-26T11:57:24.085Z Reads: 162

```
It's not powered by a battery :frowning: It's powered by my pc usb port. Also tried other power sources. Just removed the battery check and still nog working.
```

---
## \#313 Posted by: DroidSector Posted at: 2019-03-26T12:20:29.055Z Reads: 183

```
That's strange, the board should reboot on wake up. If it's related to sleep mode, try to comment out lines from 374 to 405, start with ones that include DISPLAY and VEXT. I should receive new Heltec boards soon.

https://github.com/DroidSector/FireFly-Nano-Remote/blob/38f17ba0bc82cf201c678affb8a11183497a3eba/src/remote/remote.cpp#L374
```

---
## \#314 Posted by: Jamie42 Posted at: 2019-03-26T12:26:01.134Z Reads: 177

```
Just tried. Doesn't change anything I think. 

What is happening is when I upload "freshly" compiled code it works, but when I then unplug and plug the Heltec the display stays black. The white LED indicator is also constantly on when the receiver is off and blinking when the receiver is on.

Starting to think there's something wrong with my board.
```

---
## \#315 Posted by: tobias Posted at: 2019-03-26T17:22:28.897Z Reads: 181

```
[quote="DroidSector, post:311, topic:72916"]
@tobias LED shows the data exchange, delete `digitalWrite(LED, HIGH)` if it’s too annoying. I’ve just pushed a fix for the Calibration screen
[/quote]

Ok, thanks. I thought it means that there is some issue with the communication. The calibration is now working :) 

What range do you get with the remote ? Mine is currently around 1.5 meters. A little too short, I am getting cutouts. Are there any ways to increase the range?
```

---
## \#316 Posted by: krazor Posted at: 2019-03-27T09:29:27.331Z Reads: 171

```
hmm cant wait for the rest of the parts to come in to finish building these little beasts. just wish the feathers were so dam expensive haha. ordered a 1000mah battery ended up getting an 1100mah battery instead, luckily it still fits love the design of everything. waiting on springs to really test the throttle control to see how smooth it is without a bearing. though i did notice if you install the throttle correctly it is pretty dam smooth. though im thinking about adding a couple of washers so it doesnt rub on the shell and cause it to feel sticky
```

---
## \#317 Posted by: DroidSector Posted at: 2019-03-28T10:58:18.015Z Reads: 187

```
You can use a spring from a pen, those springs from Aliexpress is a bit too strong. 

@Jamie42 Just got new Heltec boards, no display issues. Try reducing this value to 400k:

https://github.com/DroidSector/FireFly-Nano-Remote/blob/38f17ba0bc82cf201c678affb8a11183497a3eba/lib/Adafruit_SSD1306/src/Adafruit_SSD1306.cpp#L172

@tobias With new boards, I'm getting at least 10 meters when the receiver is outside the enclosure. Changing LoRa.setSpreadingFactor() from 6 to 7 in radio.cpp should increase range but reduce response time. Please PM me with more info about your setup and antennas.
```

---
## \#318 Posted by: TSJ Posted at: 2019-03-28T19:37:53.502Z Reads: 166

```
I have been building the original firefly remote and wanted a bigger screen and smaller remote.  I came across @StefanMe's feather version and ordered some Feather boards.  Then I came across this thread.  I was wondering if the code still works with the Feather, or only the Heltec board?
```

---
## \#319 Posted by: DroidSector Posted at: 2019-03-29T02:15:48.560Z Reads: 168

```
Yes, it works on both Feather and ESP32 boards.
```

---
## \#320 Posted by: KrisKraanen Posted at: 2019-03-29T09:59:33.798Z Reads: 168

```
just recieved my last parts, is the wiring diagram the same for feather and heltec?
```

---
## \#321 Posted by: DroidSector Posted at: 2019-03-29T11:25:15.067Z Reads: 177

```
Pins are different, there are only a few unused ones on this board.
![electronics_schematic_remote_heltec|584x500](upload://8s3paWxm6ki2SdnkdUZfY5mXAy7.jpeg)
```

---
## \#322 Posted by: KrisKraanen Posted at: 2019-03-29T11:36:10.229Z Reads: 180

```
and the reciever is the same?
```

---
## \#323 Posted by: DroidSector Posted at: 2019-03-29T13:16:51.293Z Reads: 180

```
Yes, power and tx/rx wires.
```

---
## \#324 Posted by: KrisKraanen Posted at: 2019-03-30T01:00:51.113Z Reads: 187

```
So i connected the reciever part, 5v ground rx and tx. When powered on it gives me 92-93% but my board is half charged..... 8s setup  ![15539075944502806129448473777905|375x499](upload://quCyFpsvuX5g2mv0iTxZHmRMFSO.jpeg)
```

---
## \#325 Posted by: KrisKraanen Posted at: 2019-03-30T01:07:20.843Z Reads: 184

```
Also when powering the transmitter, not yet soldered only programmed it gives me 92% and this km on the bottom junping around, is this normal or do i need to re-upload some new code or something![15539080558968528298491224153688|375x499](upload://n9fUg6i6YmYe3P6JcMMeh8yH1lL.jpeg)
```

---
## \#326 Posted by: hotdoghelper Posted at: 2019-03-30T02:07:19.437Z Reads: 178

```
Noob here. I'm trying to build one of these. When wiring the heltec version together, what are the differences compared to the feather version? Can I use the same schematics with as the feather version?

Edit: just saw the comments above about the differences
```

---
## \#327 Posted by: huntercasillas Posted at: 2019-03-30T02:18:20.265Z Reads: 176

```
How do I get the one on the left that looks like the ownboard one? I love it! Looks amazing!
```

---
## \#328 Posted by: Jinra Posted at: 2019-03-30T04:50:46.206Z Reads: 176

```
thats the firefly shell https://www.electric-skateboard.builders/t/simple-3d-printed-nrf-remote-arduino-controlled/28543
```

---
## \#329 Posted by: Jamie42 Posted at: 2019-03-30T06:41:40.429Z Reads: 176

```
Did you connect it up like this?

5v <---> 5v
Ground <---> Ground
Tx <---> rx
Rx <---> Tx

Also trying commenting out #define FAKE_UART
```

---
## \#330 Posted by: DroidSector Posted at: 2019-03-30T08:19:55.119Z Reads: 178

```
Yes, that's FAKE_UART values. Please also make sure that BATTERY_CELLS = 8 in globals.h to match your setup.
```

---
## \#331 Posted by: KrisKraanen Posted at: 2019-03-30T09:21:40.105Z Reads: 178

```
That did the trick, also changed the motor/wheel/pulley settings to my setup but now i have this problem; https://youtu.be/PN2boHgySZs
```

---
## \#332 Posted by: KrisKraanen Posted at: 2019-03-30T09:36:33.011Z Reads: 181

```
The motor only makes this sound when the remote and reciever are both on and connected
```

---
## \#333 Posted by: DroidSector Posted at: 2019-03-30T12:30:50.997Z Reads: 177

```
The screen shows -100% throttle / full brake. Try it with the hall sensor connected.
```

---
## \#334 Posted by: KrisKraanen Posted at: 2019-03-30T13:31:00.919Z Reads: 170

```
But still braking should not sound like this right
```

---
## \#335 Posted by: KrisKraanen Posted at: 2019-03-30T19:10:37.314Z Reads: 170

```
'found out what the noise was, i was also getting input from the remote i use now so double inputs made it do weird stuff, with my old remote unplugged it does as it should
```

---
## \#336 Posted by: ron Posted at: 2019-03-31T20:35:25.036Z Reads: 177

```
Hi there!

Does anyone have a link to the [illuminated momentary switch](https://www.adafruit.com/product/3105) for european guys. Adafruit is charging over 30USD for shipping for these Switches...

Searched Aliexpress but didn't found any corresponding switch.

Thank you in advance.
Greetings!
Ron
```

---
## \#337 Posted by: tobias Posted at: 2019-03-31T20:44:20.976Z Reads: 180

```
https://de.aliexpress.com/item/12V-Power-Symbol-Momentary-Latching-Computer-Case-20mA-SPST-Switches-Push-Button-Switch-Favorable-Price/32706563731.html?spm=a2g0s.9042311.0.0.30e04c4ddx66Bf

I bought this one.
```

---
## \#338 Posted by: ron Posted at: 2019-03-31T20:47:27.112Z Reads: 183

```
You F-in genius! ... Should have sked before searching aliexpress for almost an hour... WOW....

Thanks bud!
```

---
## \#339 Posted by: deltazeta Posted at: 2019-03-31T21:07:15.318Z Reads: 180

```
https://www.arrow.com/en/products/3105/adafruit-industries

Arrow has a couple in stock, free one-day shipping
```

---
## \#340 Posted by: tor Posted at: 2019-04-02T18:32:49.474Z Reads: 187

```
I plugged in my Heltec V2 without the antennas. Now they wont connect. I've tried changing the frequency. Serial monitor says "send PAIRING" over and over.

Is someone having any ideas or did the SX127 chips broke?

![IMG_0855|375x500](upload://lxN3mK6TggNrEM1VDNMUOT7792s.jpeg)
```

---
## \#341 Posted by: Jamie42 Posted at: 2019-04-02T19:10:11.054Z Reads: 187

```
You have got them both setup as remotes, you should program one as receiver and one as remote.
```

---
## \#342 Posted by: tor Posted at: 2019-04-02T19:29:58.582Z Reads: 182

```
Now it worked. Thank you!
```

---
## \#343 Posted by: KrisKraanen Posted at: 2019-04-04T15:01:33.868Z Reads: 184

```
is led button supposed to light up when the remote is on? mine doesn't do anything, button works just doesn't light up
```

---
## \#344 Posted by: ron Posted at: 2019-04-04T23:51:05.380Z Reads: 190

```
Yep.. Thats what I have also encountered while holding the remote..

When holding it as intended, I am sure I will get cramps im my thumb using it.

Besides that, I love the low ple of this remote.!
```

---
## \#345 Posted by: deltazeta Posted at: 2019-04-06T02:04:14.073Z Reads: 184

```
everything seems to be working for me, but the remote battery voltage is reading 4.4V when its really 4.0V. Is there a way to adjust the measurement?
```

---
## \#346 Posted by: SanderG Posted at: 2019-04-06T14:29:11.036Z Reads: 185

```
Is this a reliable remote? Is the connection strong? No disconnects? Is it safe?
```

---
## \#347 Posted by: DroidSector Posted at: 2019-04-07T01:33:13.418Z Reads: 182

```
@deltazeta You can tweak [this line](https://github.com/DroidSector/FireFly-Nano-Remote/blob/38f17ba0bc82cf201c678affb8a11183497a3eba/src/remote/remote.cpp#L936), add * 4 / 4.4.

@SanderG Yes, I've been using Feather and Heltec boards for several months, no issues so far. It's a good idea to use silicone or polyurethane potting for the receiver to protect it from water and vibrations.
```

---
## \#349 Posted by: SanderG Posted at: 2019-04-07T09:11:07.682Z Reads: 182

```
[quote="DroidSector, post:347, topic:72916"]
@SanderG Yes, I’ve been using Feather and Heltec boards for several months, no issues so far. It’s a good idea to use silicone or polyurethane potting for the receiver to protect it from water and vibrations.
[/quote]

Cool! And is the proces of building one easy? Like the code and stuff? Is it just plug and upload or do you need to change allot? Also is the part list still up to date? I think the Heltec is the best option for the board? I know a bit of coding but im not a master in it lol.
```

---
## \#351 Posted by: deltazeta Posted at: 2019-04-07T17:07:28.629Z Reads: 180

```
Just ride up the dreaded twin peaks yesterday with this remote. There's a cell tower within way too close, which has caused connection issues with feather remotes. But with the optional antennas my Firefly nano didn't have a single dropout.
```

---
## \#352 Posted by: Surfer Posted at: 2019-04-07T22:18:20.528Z Reads: 178

```
Oh nice remote!!
Just a question, this code will work on a feather remote  created by @stefanme with the m0?
```

---
## \#353 Posted by: PickSix24 Posted at: 2019-04-07T22:37:51.194Z Reads: 174

```
I’m kinda curious now too. I’ll try and flash one to see !
```

---
## \#354 Posted by: PickSix24 Posted at: 2019-04-07T22:39:58.093Z Reads: 176

```
Are you using a feather or heltec board ?
```

---
## \#355 Posted by: deltazeta Posted at: 2019-04-07T23:07:33.290Z Reads: 181

```
heltec <del>
```

---
## \#357 Posted by: krazor Posted at: 2019-04-08T05:04:02.500Z Reads: 182

```
ok for anyone that cant build for Feather , make sure that the env_default lines up with the [

like this 

![image|690x473](upload://s4jnXtQLlaun7Vc8Z2Hg1QmykVD.png)
```

---
## \#358 Posted by: krazor Posted at: 2019-04-08T06:15:35.332Z Reads: 178

```
ok i got the remote to turn on now but i cant seem to navigate the menu. the power  button and the trigger works but i cant calibrate the remote because i can not navigate down? im assuming this is done with the fly wheel. i checked the values for my magnets and they are registering values 105 and 255 is there a hard coded value somewhere that causes the navigation of this where 105 is not low enough value? or am i doing something else wrong?
```

---
## \#359 Posted by: DroidSector Posted at: 2019-04-08T09:50:05.697Z Reads: 171

```
Yes, ideally it should go from 0 to 255. You can update these constants in remote.h: MIN_HALL, CENTER_HALL and MAX_HALL. Use values displayed in the middle of the connecting screen.
```

---
## \#360 Posted by: krazor Posted at: 2019-04-08T09:53:48.546Z Reads: 182

```
funny you message just now i fixed it by doing exactly that changing the MIN_Hall to 105, my trigger was not going low enough to make it go down, surprised this doesnt support looping so you could go up even when its at list [0] it would select the last etc.i have the menu navigating now and i can fix it for the next remote. just a pain to read through others code especially when im not familier with the Atom IDE was a trip and a half. still not fully assembled remote yet but i have the electronics connected temporarily while i print out 2 new remotes to complete the build with. i love the design so far. im finding the fly wheel a little tacky with my test prints in PLA+ have you got a solution for that. i was thinking about using a washer but not sure if that will interfer with the magnets and the hall sensor by giving it fake readings.
```

---
## \#361 Posted by: DroidSector Posted at: 2019-04-08T10:01:37.613Z Reads: 185

```
@wapkoen has an idea to use ptfe tube as a bushing. 693ZZ bearing will also work with this mod:

https://www.thingiverse.com/thing:3510570
```

---
## \#362 Posted by: krazor Posted at: 2019-04-08T10:03:09.200Z Reads: 178

```
nice, i will have to see what changes he made as im using the Feather version, seems kinda rare that not many people are using it due to its price
```

---
## \#363 Posted by: Winkelmann Posted at: 2019-04-08T17:57:11.271Z Reads: 182

```
Hey people!
I appreciate all the feedback i can get! :slight_smile:

https://www.electric-skateboard.builders/t/project-board-better-than-boosted/89825?u=winkelmann
```

---
## \#364 Posted by: AlexH Posted at: 2019-04-09T01:33:25.936Z Reads: 178

```
How up to date is the parts list? Given all the chatter on the implementation and issues, is there an updated step-by-step installation that could be compiled? Would be great!
```

---
## \#365 Posted by: KrisKraanen Posted at: 2019-04-10T13:15:44.184Z Reads: 173

```
@DroidSector how am i supposed to secure all the electronics inside, the deadmans switch for example and the main board: hot glue? Superglue? Epoxy? Whats the best option. And my power switch is not lighting up it does as its supposed to but it doesn't light up
```

---
## \#366 Posted by: DroidSector Posted at: 2019-04-10T15:54:15.465Z Reads: 187

```
Hot glue should be fine for securing elements inside the remote. Easier to remove it as well if the shell gets broken, for example. 

For receiver it's very important to use a proper potting, this article recommends a **neutral cure silicone**, could be easily found on eBay or in local shops.

https://electronics.stackexchange.com/questions/18525/what-kind-of-glue-should-i-use-for-pcb-mounted-components-to-avoid-vibrations

For the switch, connect LED + contact to 3.3v for a few moments to test it. 

@AlexH part list is current, I've updated GitHub Wiki with more recent instructions.
```

---
## \#367 Posted by: StefanMe Posted at: 2019-04-10T16:06:24.572Z Reads: 183

```
Yes should work. U just have to redefine other pins for the buttons... bit except of this, the hardware is the same!
```

---
## \#368 Posted by: KrisKraanen Posted at: 2019-04-14T17:14:41.486Z Reads: 183

```
My led is working now, when the remote is on its on, but when its connected to my board it flickers really fast?
https://youtu.be/uZ5kJfwenfc,

And when there are no magnets pressing the deadmans trigger makes it go full throttle
```

---
## \#369 Posted by: Xtreme Posted at: 2019-04-20T20:10:40.415Z Reads: 180

```
I show the "success" message in uploading code to the feather remote and receiver, but in both cases I get a message that says "Could not find active agents. Please start it before on a remote machine using `pio remote agent start` command." and the feather blinks red.  Any idea what the issue is and how to resolve it?  The only thing I can think of is my firewall is stopping something.
```

---
## \#370 Posted by: DroidSector Posted at: 2019-04-21T04:02:02.564Z Reads: 169

```
Just use Upload, not Remote Upload button. You should see your device, connected via USB, in PlatformIO Home > Devices tab.
```

---
## \#371 Posted by: Xtreme Posted at: 2019-04-21T05:35:36.312Z Reads: 177

```
Thank you, @DroidSector !  That resolved it.  I sincerely appreciate your help as well as your willingness to share this excellent and elegant design with us!
```

---
## \#372 Posted by: hotdoghelper Posted at: 2019-04-22T03:58:50.544Z Reads: 176

```
Has anyone built the receiver without the power filter? What does it do exactly?
```

---
## \#373 Posted by: Xtreme Posted at: 2019-04-22T04:30:55.186Z Reads: 176

```
I haven't yet tested this receiver, but I have had problems with off-the-shelf receivers where the board suddenly loses all power while under full accceleration (and I taste asphalt).  I had just concluded it was a power glitch, even though there is little published on this topic.  Assuming my conclusion is correct, I definitely recommend something between power and ground wires for the receiver.

What I don't understand is why several different values of capacitors in parallel are recommend here instead of one capacitor and an inductor, which would provide filtering AND smooth out a power sag.  Does anyone know?
```

---
## \#374 Posted by: Jamie42 Posted at: 2019-04-22T09:04:21.279Z Reads: 171

```
I just built my remote and tried it with the receiver. It all works! However the telemetry data is only updated on the remote every so often, is this normal? Shouldn't it update about real time? Or atleadt every second?
```

---
## \#375 Posted by: Acido Posted at: 2019-04-22T10:12:57.756Z Reads: 175

```
Is here anyone that used this remote for some time and can talk about its reliability? 

Im tempted to get a kit :smile:
```

---
## \#376 Posted by: chickengun Posted at: 2019-04-23T19:45:00.836Z Reads: 171

```
@DroidSector I have [this](https://www.aliexpress.com/item/Mini-ESP32-Wifi-Lora-Development-Board-with-0-49inch-oled-display-LoraBar/32960464571.html) heltec board with 0.49" display. Could I use it to build your remote?
```

---
## \#377 Posted by: KrisKraanen Posted at: 2019-04-24T13:21:41.173Z Reads: 183

```
ok so i have the remote build, but its always on full speed
https://www.youtube.com/watch?v=GtmW5tUNoEI
and when the board is connected to the remote this happens:
https://www.youtube.com/watch?v=uZ5kJfwenfc
i already reuploaded the firmware
```

---
## \#378 Posted by: KrisKraanen Posted at: 2019-04-24T13:49:25.315Z Reads: 185

```
now its reversed......

https://www.youtube.com/watch?v=x5VSllofOUY
```

---
## \#379 Posted by: MikeDIY Posted at: 2019-04-24T15:17:26.758Z Reads: 182

```
:partying_face:   :partying_face:

Is that a TTGO LoRa v2 ?  :thinking:
```

---
## \#380 Posted by: KrisKraanen Posted at: 2019-04-24T15:31:50.451Z Reads: 178

```
heltec lora v2
```

---
## \#381 Posted by: MikeDIY Posted at: 2019-04-24T16:06:35.521Z Reads: 184

```
Can i get a copi of the stl's :pray:  ?
```

---
## \#382 Posted by: KrisKraanen Posted at: 2019-04-24T16:22:38.046Z Reads: 182

```
its litterly the stl from this page :rofl:
```

---
## \#383 Posted by: Mich21050 Posted at: 2019-04-24T16:27:37.695Z Reads: 185

```
There you go:\
https://www.thingiverse.com/thing:3303495
```

---
## \#384 Posted by: MikeDIY Posted at: 2019-04-24T17:11:42.704Z Reads: 181

```
 Thanks :pray:
```

---
## \#385 Posted by: DroidSector Posted at: 2019-04-25T07:02:41.517Z Reads: 179

```
@KrisKraanen it could be the polarity of magnets, they should be opposite to each other.

@chickengun it should be ok for receiver.

@hotdoghelper @Xtreme I'm currently testing it with Unity without power filter, works ok so far. There is Timeout Brake Current option in VESC settings, if it's zero, no braking should occur on power loss.

@Jamie42 it should update a few times per second, try to tweak the UART speed and timeout.
```

---
## \#386 Posted by: Jamie42 Posted at: 2019-04-26T10:15:02.188Z Reads: 176

```
I'Il try to tweak the settings a bit.
```

---
## \#387 Posted by: adrianlee Posted at: 2019-04-29T11:11:59.624Z Reads: 185

```


I ordered this:

https://www.aliexpress.com/item/868MHz-915MHz-LoRa-ESP32-Oled-Wifi-SX1276-Module-IOT-with-Antenna-For-Arduino-Electronic-diy-kit/32836246848.html

 and got this? :open_mouth: same same but different

![20190429_140639|281x500](upload://bmoMWc3IUgdCd9cc7YDq3Ug8A7R.jpeg)
```

---
## \#388 Posted by: chickengun Posted at: 2019-04-29T12:26:14.959Z Reads: 180

```
@adrianlee 
Funny, same happened to me. Just write the seller showing this photo. They will resend the correct one, you can keep this model
```

---
## \#389 Posted by: adrianlee Posted at: 2019-04-29T14:12:04.510Z Reads: 181

```
@chickengun yeah I hope I get correct ones and can keep these, they seem pretty handy!
```

---
## \#390 Posted by: hotdoghelper Posted at: 2019-04-30T07:16:49.570Z Reads: 182

```
I did that and was refunded at 80% while keeping the new ones. Shame that they couldn't send the correct one since they're one of the cheapest vendors I've seen
```

---
## \#391 Posted by: friendlyhorse Posted at: 2019-05-04T04:03:41.168Z Reads: 187

```
I'll join the "wrong modules" club. Those are nicely built but the screen is way too small for use in a remote. ![IMG_20190430_190722|375x500](upload://iqgytSrw5YAPBgbq5qpEaIupqVp.jpeg)
```

---
## \#392 Posted by: KrisKraanen Posted at: 2019-05-04T17:01:25.395Z Reads: 175

```
magnets are opposite polarity facing the hall sensor i now have that it registers braking but not giving throttle.....
```

---
## \#393 Posted by: KrisKraanen Posted at: 2019-05-04T17:02:34.254Z Reads: 175

```
its not recognizing the trottle polarity...
```

---
## \#394 Posted by: deucesdown Posted at: 2019-05-04T22:50:13.152Z Reads: 176

```
flip the magnets?
```

---
## \#395 Posted by: deucesdown Posted at: 2019-05-04T22:53:24.380Z Reads: 178

```
[quote="friendlyhorse, post:391, topic:72916"]
“wrong modules” club
[/quote]

same here. I tried to message the seller but AE changed the messaging system, looks like a hot mess? I had to start a dispute due to no response, and got refunded 85%. I'd have preferred to have them send the correct ones. The seller did message me that they're the same except for smaller display...

Anyone got a track on the white ones with the big display?
```

---
## \#396 Posted by: KrisKraanen Posted at: 2019-05-06T16:25:15.713Z Reads: 176

```
.....
offcourse i have tried that..... no luck
```

---
## \#397 Posted by: KrisKraanen Posted at: 2019-05-06T16:25:57.019Z Reads: 179

```
this is exactly whats happening. its only recognizing one polarity of the magnet, which is the braking polarity

i have this hall sensor:
https://nl.aliexpress.com/item/Free-Shipping-50PCS-LOT-49E-OH49E-SS49E-linear-Hall-Switch-sensor-Hall-element-New-and-Origianl/1900206163.html?spm=a2g0s.9042311.0.0.34b94c4d9T3kw6
```

---
## \#398 Posted by: your_eye_ah Posted at: 2019-05-13T01:36:14.190Z Reads: 167

```
I am having the same problem as you. Any luck fixing this issue yet?
```

---
## \#399 Posted by: Xtreme Posted at: 2019-05-13T03:00:09.553Z Reads: 174

```
@DroidSector / All:  I bought the Heltec board from the link provided to Amazon in Post #206, but there are a bunch of errors during the coded upload, including the one seen here:![Erros%20for%20Heltec%2C%2012%20May%2019|670x500](upload://dMbBXKLjvTueVmKpqoTuBrWOaRy.png) 
Any idea what might be wrong?  The board is labeled "LoRa" and the "V2" and boots up with a Heltec screen.

I was able to load the code on the Feather board, but had other problems there (mostly not receiving metrics data when the throttle was on, plus I like the Thingverse case for the Heltec better), so i figured I'd try the Heltec boards.

Any help would be sincerely appreciated.
```

---
## \#400 Posted by: your_eye_ah Posted at: 2019-05-13T03:28:47.911Z Reads: 167

```
Can you screenshot the page /src\boards\heltec-2.h please?

Did you follow the step in the wiki and download the newest code?
```

---
## \#401 Posted by: myreala Posted at: 2019-05-13T03:30:54.404Z Reads: 166

```
I have a partially assembled feather kit that I want to sell. 1000mhr battery. Everything come with spares, price is $80 plus shipping. I just don't have time to finish it anymore I hope someone else can.
```

---
## \#402 Posted by: your_eye_ah Posted at: 2019-05-13T05:12:29.298Z Reads: 170

```
@KrisKraanen I was able to fix the throttle issue by fixing this line (in remote.cpp):   
adc1_config_channel_atten(ADC_THROTTLE, ADC_ATTEN_DB_11);

Changing ADC_ATTEN_DB_2_5  to ADC_ATTEN_DB_11 changes the attenuation of the hall sensor to the correct amount for the full 3.3v.  
You can read about it [Here]( https://docs.espressif.com/projects/esp-idf/en/latest/api-reference/peripherals)
```

---
## \#403 Posted by: willumpie82 Posted at: 2019-05-13T05:42:20.584Z Reads: 180

```
Hi all,

I'm working on a fork with the use of an AS5047D angle sensor for the throttle wheel and full body PCB :sunglasses:
![throttlewheelmount|690x388](upload://jbUuqczin0F0pdMsh4CdiDwEmoS.jpeg) ![throttleassy-slice|690x388](upload://1QBRZk0pl5n7UpR0YcQQkYTVG9m.jpeg) 

work in progress...

ofcource credits for the body design are to @DroidSector
```

---
## \#404 Posted by: KrisKraanen Posted at: 2019-05-13T11:56:21.524Z Reads: 170

```
my trigger isn''t a deadmans switch, its a cruisecontrol switch how do i change this?
```

---
## \#405 Posted by: KrisKraanen Posted at: 2019-05-13T11:56:34.536Z Reads: 169

```
this worked thanks!
```

---
## \#406 Posted by: Xtreme Posted at: 2019-05-14T01:38:28.434Z Reads: 181

```
@your_eye_ah:  Thanks for responding.  Yes, I believe I was able to download the newest code, though I am unsure how to verify. 

Here is /src\boards\heltec-2.h:
![h%20Screen%20%231|399x500](upload://2djCSoxssSKLYUSHZTmlcCRNGO4.png) ![h%20Screen%20%232|576x330](upload://1FJd4KBoIsfvbzP8xbOlMah80Ha.png)
```

---
## \#407 Posted by: KrisKraanen Posted at: 2019-05-15T12:13:41.813Z Reads: 161

```
So i am having a couple issues, first one is that i can't seem the get the trigger to go from cruise to deadman, i also have the issue that in the menu when i go to any of the board settings the screen goes black and it does nothing until i press the power button to go out of the menu, this also happens in the remote menu when i click auto off, is there a detailed page where you exolain al the features and menus in this remote?
```

---
## \#408 Posted by: your_eye_ah Posted at: 2019-05-17T20:33:49.592Z Reads: 163

```
It seems that you have an older version of the build. I'm not the best with git and what not, so my personal recommendation as to what I would do is completely delete the project(requires deleting the folder in file manager), then re-download it following the [wiki](https://github.com/DroidSector/FireFly-Nano-Remote/wiki/3.-Software).  
  
Hopefully, this works for you. Also, see my comment above about attenuation. Cheers.
```

---
## \#409 Posted by: DroidSector Posted at: 2019-05-18T03:04:24.114Z Reads: 153

```
Currently, the trigger works as both deadman and cruise, i.e. first press will unlock the throttle wheel. The settings screen is not ready yet, sorry.
```

---
## \#410 Posted by: TinnieSinker Posted at: 2019-05-18T07:41:05.687Z Reads: 151

```
is it possible to have the trigger control an aux channel to be on/off
```

---
## \#411 Posted by: BluPenguin Posted at: 2019-05-18T08:08:06.945Z Reads: 153

```
@DroidSector How easy would it be to adapt the arduino code to 2 hall sensors? As in building a remote that has a separate brake/throttle (like the evolve R2 or the maytech). I can design everything hardware side but I'm clueless on the code. Just want to know how manageable it is before I dive too deep into it. Thanks!
```

---
## \#412 Posted by: DroidSector Posted at: 2019-05-18T08:22:53.770Z Reads: 151

```
Very easy, just read values from the brake hall sensor and prioritize it over the throttle.
```

---
## \#413 Posted by: niktwo17 Posted at: 2019-05-18T10:34:29.326Z Reads: 161

```
First of all, great remote!

I do really enjoy using it, but I am having some issues regarding the range: 

My heltec v2s (433mhz, with stock as well as suggested external antenna) already start to drop out once they are 50cm apart.

Anyone else having such an issue or ideas how to fix it?
```

---
## \#414 Posted by: Xtreme Posted at: 2019-05-18T15:18:14.111Z Reads: 167

```
@niktwo17: Even though I have other issues, as far as the radio connection, my Feathers work through multiple room walls 15+ meters away with just a solid 22 gauge wire as an antenna.  One of the things I would do if I were having trouble with range (besides looking for sources of radio frequency interference, shorts, moving the receiver location on the skateboard, etc.) is to build a proper half-wave dipole antenna.  There are great instructions here:  https://www.rcgroups.com/forums/showthread.php?1159968-Build-your-own-TX-antenna-for-FPV.  Since you don't need a half kilometer+ range, no need to worry about keeping the elements straight, you just need to be concerned about keeping the elements from shorting together as well as wires breaking from stress/strain (might need to use epoxy or hot glue at the junction, then pot the whole thing with neutral cure silicone).  You could also try changing the frequency within your band in case you are getting interference from another near-by emitter (see the software section of DroidSector's instructions).  Lastly, you could check its signal output as well as that of nearby competing emitters with a spectrum analyzer such as RF Explorer available on Amazon for $129.
```

---
## \#415 Posted by: Xtreme Posted at: 2019-05-19T20:26:06.630Z Reads: 154

```
@niktwo17:  Another thought--are you sure the antenna connector isn't broken?  with a 50cm range, it almost seems like there is no antenna.
```

---
## \#416 Posted by: Xtreme Posted at: 2019-05-19T20:59:27.476Z Reads: 164

```
@your_eye_ah:  Thank you!  Deleting the project and re-downloading (mostly) worked!  It also fixed the problems I was having with the Feather boards.  The only problem is it gives me an error with the Heltec receiver when I connect to the VESC after commenting out FAKE_UART.  It times out on Serial port COM15, even though that doesn't happen with the Feather boards or prior to connection to the VESC.  It says "A fatal error occurred: Failed to connect to ESP32: Timed out waiting for packet header"  I think baud rates are properly set to 115200, but it seems it can't communicate.

Any thoughts anyone?
```

---
## \#417 Posted by: your_eye_ah Posted at: 2019-05-20T05:47:41.055Z Reads: 157

```
Can you post a screenshot?
```

---
## \#418 Posted by: Xtreme Posted at: 2019-05-21T01:36:59.189Z Reads: 170

```
@your_eye_ah:  Here is the screenshot of the COM15 issue![COM15%20Error|690x369](upload://94ZfQPOh3uUbjYjmyYFfOp97aKQ.png) 
Plugging in the Heltec versus the Feather, whether connected to the VESC or not, changes from COM12 to COM15 as seen in these pictures:
![Heltec%20Port|690x271](upload://3EuXc5IzVvpAXabtKWk7Xr9TPZ.png) 
![Feather%20Port|690x307](upload://xm4MZf3SFgXN1sMn6TFSq2Zp83Z.png) 
COM12 with the Feather creates a successful build, and COM15 with the Heltec does not.
With the exception of a Microsoft Driver on COM12 versus the Silicon Labs driver on COM15, the settings are the same:

![COM15%20Driver|451x500](upload://zbcnxjxNt6ZsLEx9zvHVLZnqN4X.png)
```

---
## \#419 Posted by: Pavlo_H Posted at: 2019-05-23T07:00:14.956Z Reads: 171

```
I just finally received the parts for the Firefly Nano Remote and already have everything built and soldered up. I was able to get the code working on the receiver with it receiving data and showing the battery percentage on the OLED. I'm also able to create a connection between the receiver and remote, and can also send data between them. But the with the Remote, I am able to connect to it, upload code, receive debug data from it, the illuminating power switch and the hall sensor work but the display and the dead man switch doesn't work. The screen has lit up randomly (at least twice)for a split second while pressing buttons but doesn't work in general. I am thinking this is probably code related because when I upload reciever code onto the remote the OLED lights up. But when the remote code is on it. Nothing happens.
Please Help!

TL;DR:

Problem #1(**FIXED**): Display doesn't work on remote side. Figured out that my display wasn’t turning on because my board doesn’t have a batter sensor. Set the min batt voltage to 0 and now it works. 

Problem #2(**FIXED**): Deadman switch doesn't change anything. For me it is always triggered and sending throttle command to the receiver. **EDIT**: There seems to be a typo in the schematics on github where it says to connect the deadman switch to ground and pin 32 but in my case your supposed to go to 3.3v and pin 32.
![image|375x500](upload://kAtSuJovwPmWZdoq5HvlpsDupJq.jpeg) ![image|375x500](upload://5nvFmE1Yl3L7EuMVv4OHxIWoHYS.jpeg) The white wire in the picture goes to pin 33 but I tried changing it to see if that would fix it. Pin 32 and 33 seem to not be recognized by the board

Board: https://bit.ly/2QjKC17
Using Code: https://github.com/DroidSector/FireFly-Nano-Remote.git

Thank you :slight_smile:
```

---
## \#421 Posted by: xatonic Posted at: 2019-05-24T17:09:14.389Z Reads: 157

```
@Pavlo_H @DroidSector I'm having the same problem hope we can figure it out
```

---
## \#422 Posted by: Toymanf Posted at: 2019-05-25T22:47:49.156Z Reads: 170

```
First of all, WOW! Very impressive work on this remote. Thank you!

I am having difficulty calibrating the thumbwheel. My min shows 0 and max shows 1023 and idle shows 475 while remote is on, rec off. I set these same values in the remote.h file. I am using Heltec v2 board.

The "0-255value" is 83 at idle/neutral.
My problem is I do not understand how to get the remote to accept the values from the calibration screen in the menu. When I enter the menu screen I am continuously scrolling unless I hold the thumbwheel forward. I can navigate thru the screens and enter remote>calibrate screen. I move the thumbwheel to push the min max values to 0 and 1023. Here is where I am stuck. I do not know how to get the remote to accept these values. Nothing happens when I toggle the trigger switch. When I tap the (Power)button, it exits the calibration screen with no change in operation. The receiver shows - 35% with the thumbwheel in idle/neutral position.
Is there a step by step somewhere for the menu system?
Any suggestions?
I have been studying both this thread and original Firefly(Solidgeek) thread.
Have not been able to find a good explanation or example of the current menu system.
Thank you for any help on this.
Toymanf
```

---
## \#423 Posted by: DroidSector Posted at: 2019-05-26T14:31:50.322Z Reads: 159

```
It's probably the calibration screen is not working properly. Try to temporarily set these values again after line 80:
  
    loadSettings();

    settings.minHallValue = 0;
    settings.centerHallValue = 475;
    settings.maxHallValue = 1023;
    saveSettings();
```

---
## \#424 Posted by: DroidSector Posted at: 2019-05-26T14:47:54.577Z Reads: 150

```
Code uploading might not work if Heltec is already connected to VESC.
```

---
## \#425 Posted by: Toymanf Posted at: 2019-05-26T14:52:44.422Z Reads: 155

```
Thank you for the help. I read the code in remote.cpp around lines 1140 and got a better understanding of what it was looking for. The problem was I was not returning to the idle position it recorded as I entered the calibrate screen due to the fact I had to hold the thumbwheel off center to get into the menu. As you know, it takes the value of the thumbwheel at the time you enter the calibrate menu and sets center_hall value to that number.
I was able to move the thumbwheel back to center the it stated to hit trigger to save value. After calibrating a few times, I was able to get the thumbwheel centered(due to deadband).

On to my next challenge. Implementing reverse using only the thumbwheel(Not Skateboard specific)Any pointers on where to start in the code??
Thanks again, loving this remote,
Toymanf
```

---
## \#426 Posted by: willumpie82 Posted at: 2019-05-27T07:00:04.692Z Reads: 161

```
Hey guys, I printed all the parts in PETG but i'm strugling to get it together properly, (heltec v2)

- I assenbled the rear-lid (with the display and electronics) 
- put screws in the toplid (screws facing up)
- Assemble the spring fork, thubwheel and trigger
- Fiddle the two halves together without letting the screws fall out.
- I had to file off quite a bit of the trigger and springfork otherwise it got stuck
- When i test the springfork with all opened up, it is fine,when closed and lightly screwed in, the throttle wheel has a big wobble (with no spring action)

any clues what i'm doing wrong?
```

---
## \#427 Posted by: BluPenguin Posted at: 2019-05-29T00:04:43.840Z Reads: 167

```
Here's a spin off of the Firefly nano I've been working on. Yes it looks a lot like some *cough* other remotes. I'm gonna call it Serenity. Will be be finalizing the design and optimizing it for 3D print soon. Using the feather board with the display on the top to be ambidextrous, 50 degrees of throttle trigger for good control on high powered boards, and a PCB antenna mounted to the very tip of the remote so it is not wrapped in your hand. Just gauging to see how much interest this gets. I'll release the design once I see it prints well enough.

p.s. I cannot code C++ for life of me, so someeebody is going to have to add in some lines for 2 hall effects.


![Untitled|690x424](upload://xyPjWCVW10CeWabq6SxL9EV1Wfd.png) 

I'll scootch to a new thread if I'm highjacking this one.
```

---
## \#428 Posted by: willumpie82 Posted at: 2019-05-29T07:52:57.167Z Reads: 160

```
looks more as a maytech remote than a firefly
```

---
## \#429 Posted by: xatonic Posted at: 2019-05-29T07:54:40.025Z Reads: 163

```
LOVE the design I hope it turns out good and gets a good backing! Are you planning to have it be the orientation as the nano where the wheel controls speed or is the trigger going to control speed?
```

---
## \#430 Posted by: BluPenguin Posted at: 2019-05-29T19:33:36.390Z Reads: 156

```
It's suppose to be the maytech configured to use the firefly internals.

Orientation is however you program the feather board. The 2 remotes this was copycatted from is trigger for throttle and thumb for brake.
```

---
## \#431 Posted by: Xtreme Posted at: 2019-05-29T23:31:45.113Z Reads: 146

```
@willumpie82 I've printed the case with both PLA and ABS and the tolerances are much tighter.  Besides filing the trigger, I have to drill out the screw holes.  Have you tried a material other than PTEG?
```

---
## \#432 Posted by: CharlieFlan Posted at: 2019-05-30T01:29:20.300Z Reads: 141

```
this. I've been waiting for it.
```

---
## \#433 Posted by: xatonic Posted at: 2019-05-30T02:44:55.226Z Reads: 141

```
@willumpie82 my remote went together really easily with Petg, actually the screw holes were too big 😝 I'm printing on an original Prusa mk2.5
```

---
## \#434 Posted by: DroidSector Posted at: 2019-05-30T04:19:07.844Z Reads: 144

```
@willumpie82 I've printed small parts with PLA at 0.1 mm last December, still works fine. And my printer doesn't handle PETG that well.
```

---
## \#435 Posted by: willumpie82 Posted at: 2019-05-30T18:38:36.310Z Reads: 144

```
thanks for all the replies, i'll print some parts again with PLA
```

---
## \#436 Posted by: tardyparty7 Posted at: 2019-06-03T01:11:08.417Z Reads: 143

```
like the new evolve remote that came out before maytech i think.
```

---
## \#437 Posted by: hotdoghelper Posted at: 2019-06-09T03:55:00.500Z Reads: 134

```
I noticed that there's some battery drain with my remote without any usage. Has anyone else noticed this?
```

---
## \#438 Posted by: Jamie42 Posted at: 2019-06-09T09:35:10.592Z Reads: 137

```
Yep, me too, remote dies in a few days of no use.
```

---
## \#439 Posted by: tardyparty7 Posted at: 2019-06-13T03:01:54.086Z Reads: 132

```
i mean you can charge it...
```

---
## \#440 Posted by: hotdoghelper Posted at: 2019-06-13T23:56:42.062Z Reads: 132

```
yeah, but if the remote isn't in use and I don't ride my board every day, I may not know if the remote has a charge. I also would rather not have my remote charging 24/7
```

---
## \#441 Posted by: willumpie82 Posted at: 2019-06-15T07:29:58.137Z Reads: 129

```
Add a switch ;-)
```

---
## \#442 Posted by: stefik58 Posted at: 2019-06-17T15:46:44.302Z Reads: 130

```
hi, im situated in europe (Czech Republic) i have lora 868/915 can i use it or i must order 433 version ?thx
```

---
## \#443 Posted by: Kodin Posted at: 2019-06-18T03:46:17.815Z Reads: 130

```
The chips should have a much lower power sleep state option to prevent it from dying in like 2 days while "off" on a 1Ah battery.  What sort of sleep state are we putting the Heltec boards into when "off" and how often is it waking from that sleep state to check for power button input?

Is hibernate, deep sleep, or sleep leveraged in the "off" state?  Haven't had time to dig into the code to confirm quite yet, will likely do so over the next day or two.

@willumpie82 ESP32 devices can sleep down to 2.5 micro-amp-hours in "hibernate", or 10 micro-amp-hours in "deep sleep" mode.  I'm getting ~600 milli-amp-hours (600,000 micro-amp-hours) of drain in a couple days.  Even if I've got a bad lipo cell and it's got half the rated capacity, that's still a huge amount of power consumption for a chip like the ESP32.

Edit: Looked at the code, looks like you're only entering "deep sleep" mode and watching for an input interrupt.  Why not hibernate in cycles to significantly improve "off" battery life?  Something on the order of wake up on timer value every X micro/milli-seconds to check for pin input, then go back to sleep if not found.  Such a change could bring battery life up from a couple days to potentially several weeks.

Edit 2: After fully charging my remote, the battery voltage reads 4.4V.  This will kill my lipo cell very quickly.  Currently leaving the remote on until it gets back down to under 4.2V.  Anyone else see this before?  How does one configure the Heltec board if one wanted to specify charging limits on the remote battery?
```

---
## \#444 Posted by: hotdoghelper Posted at: 2019-06-18T23:51:51.759Z Reads: 115

```
when left unchecked, my battery charges up to 4.7V, definitely something I'd want to change
```

---
## \#445 Posted by: xatonic Posted at: 2019-06-19T02:16:38.094Z Reads: 121

```
Does anyone have a heltec board for sale? Mine just died from an incident... https://www.electric-skateboard.builders/t/everything-blew-up/96897
```

---
## \#447 Posted by: Jamie42 Posted at: 2019-06-19T06:12:29.798Z Reads: 126

```
@Kodin @hotdoghelper Did you check the voltage at the battery with a multimeter? Don't think LiPo's can charge that high without blowing up. And the adafruit ones have a built-in BMS. 

Read this:

[quote="DroidSector, post:347, topic:72916, full:true"]
@deltazeta You can tweak [this line](https://github.com/DroidSector/FireFly-Nano-Remote/blob/38f17ba0bc82cf201c678affb8a11183497a3eba/src/remote/remote.cpp#L936), add * 4 / 4.4.

@SanderG Yes, I've been using Feather and Heltec boards for several months, no issues so far. It's a good idea to use silicone or polyurethane potting for the receiver to protect it from water and vibrations.
[/quote]
```

---
## \#448 Posted by: Kodin Posted at: 2019-06-19T08:11:05.839Z Reads: 129

```
I'll check in the morning to verify voltages, but lipo's (especially low discharge rate cells) are able to tolerate overcharge voltages pretty well for very brief periods of time.  The longer they are stored above storage charge however, the shorter their cycle life.  It's more complicated than that as it also depends largely on cell chemistry, but I've seen cases of guys accidentally charging 16Ah packs to like 4.5, 4.6V per cell without ignition, however in all cases where that occurred, they caught it and immediately discharged slowly and carefully.  I'd honestly prefer if I could set the charge end-voltage to be 4.15V.  the cell I have in my remote has a small board that might have some sort of protection circuit on it, but no idea if it does anything other than short (overcurrent) protection.  If I find the voltage reading is off, is there a correction factor variable I can set in a header file somewhere?  A cursory look into the code didn't show anything too obvious, but I could also have totally missed a variable.
```

---
## \#449 Posted by: hotdoghelper Posted at: 2019-06-19T19:07:12.274Z Reads: 126

```
thanks for pointing this out. I took a measure and while it shows 4.59 on the remote, the multimeter reads 4.04, so feeling a bit better about battery safety.

Update:
After confirming the max voltage of 4.18 from the multimeter, I've added the suggested fix (w/ different value, mine displayed ~4.7V). Seems to fix the readings now. 

Next fix I'd like to see/tackle is the battery drain issue with deep sleep mode

Update 2:
One thing I noticed is fixing these values gives me a "longer" battery life. The readings being more accurate keeps the remote from shutting off prematurely or "random drops" in voltage.
```

---
## \#450 Posted by: Jamie42 Posted at: 2019-06-19T20:26:29.655Z Reads: 124

```
Guess the drain is about 800 microamps, if using the deep sleep specified here:
https://heltec.org/project/wifi-lora-32/

Edit:

However, I have a 500 mAh battery.
800 uA = 0,8 mA
Correction rate: 0,7
500 / 0,8 * 0,7 = 437,5
437,5 / 24 = 18

My remote definitely doesn't reach 18 days.
```

---
## \#452 Posted by: Jamie42 Posted at: 2019-06-19T21:37:35.693Z Reads: 117

```
Think it will, it has the "V2" on it and seems to be the same.

Edit: No assurances tho
```

---
## \#453 Posted by: xatonic Posted at: 2019-06-19T21:39:20.044Z Reads: 120

```
yeah, I'm sorry ab the spam :rofl: I just saw that droidsector recommended it earlier so it should be good. probably should've searched the thread first...
```

---
## \#454 Posted by: hotdoghelper Posted at: 2019-06-20T20:42:36.371Z Reads: 123

```
the v2 version is easiest to differentiate by the coil antenna on the board.
```

---
## \#456 Posted by: krazor Posted at: 2019-07-07T06:45:21.265Z Reads: 125

```
well dam i woulda snached this right up mien cost me over 200 to build
```

---
## \#458 Posted by: krazor Posted at: 2019-07-07T07:29:10.323Z Reads: 126

```
hmm i just did an update and tried to reflash the reciever/Remote and im getting an error 

src\receiver\receiver.cpp:103:11: error: 'Vext' was not declared in this scope
```

---
## \#459 Posted by: farnamweb Posted at: 2019-07-08T00:58:57.615Z Reads: 120

```
Some people had connections issues with the FeatherRemote in US. Isn't 2.4 frequency more reliable?
```

---
## \#460 Posted by: Jamie42 Posted at: 2019-07-08T09:30:36.829Z Reads: 116

```
Revert to an older version, the newest one doesn't work.
```

---
## \#461 Posted by: Jamie42 Posted at: 2019-07-08T10:45:46.383Z Reads: 121

```
@DroidSector or anyone else,

Do you know how to set motor settings of the VESC, I want to change my current settings through my receiver. Maybe you could implement settings into your library?
```

---
## \#462 Posted by: krazor Posted at: 2019-07-09T08:59:49.127Z Reads: 128

```
Here is a Link to the Throttle wthat uses a 693ZZ Miniature Ball Bearing if anyone is interested in using it.
[Thingiverse](https://www.thingiverse.com/thing:3737396)

![IMG_20190706_030616|375x500](upload://AtiuKaRUR7I4YIfuMbOhMmqobf1.jpeg)
![IMG_20190707_160103|375x500](upload://lb5osodqbMZeGYhZfuyzThStZGd.jpeg)
```

---
## \#463 Posted by: Pmuzzio Posted at: 2019-07-12T14:22:32.295Z Reads: 119

```
Hi all! Very nice development! Congrats to the forum community for the colab and feedback to the developers.

I'm building one of theses, bought everything from Ali as I'm in Chile, hope everything arrive well. 

Is it possible, or maybe is already implemented, to add lights controller to the receiver? I would love to add brake lights and headlights to my build. The led drivers could be done with arduino but the signal from the receiver is what I'm looking for.

Kind regards and thank you all!
```

---
## \#464 Posted by: Jamie42 Posted at: 2019-07-12T15:05:03.230Z Reads: 115

```
Hi and welcome to the forum!

It is definitely possible to implement, not even that hard. But it isn't there yet. I plan on doing it as soon as I am back from vacation.
```

---
## \#465 Posted by: krazor Posted at: 2019-07-12T15:22:11.667Z Reads: 114

```
this is something im intersted in myself and plan on making additions to the code base to allow this. since i just finished ordering the main components for my board the lighting will be next on my list. when im finished with it ill do a push with a new settings menu that can incorporate lighting. though this will be a long term goal.
```

---
## \#466 Posted by: Lucifer Posted at: 2019-07-14T19:08:11.611Z Reads: 113

```
I implemented simple light functions [here](https://github.com/simonp0/FireFly-Nano-Remote/) for the Heltec board. It outputs a PWM signal on 2 pins of the receiver for the front and back lights so you can drive the leds via a mosfet on each channel.
```

---
## \#467 Posted by: Maxx Posted at: 2019-07-15T09:00:29.652Z Reads: 111

```
Those features sound awesome! Is your code available somewhere?
```

---
## \#468 Posted by: krazor Posted at: 2019-07-16T13:53:09.117Z Reads: 111

```
would you mind getting this up and running for the feather. Im not well versed in C/C++ and spent the weekend trying to wrap my head around it haha. Havent used this language since uni. even then 99% of my coding is in C# 

If not all good. I plan on adding it myself either way and fixing the issues im having with Feather version and extending the feature set.
```

---
## \#469 Posted by: krazor Posted at: 2019-07-20T06:00:07.546Z Reads: 107

```
would you know which version is currently working i cant seem to get a build on any of them?
```

---
## \#470 Posted by: Jamie42 Posted at: 2019-07-20T10:02:13.407Z Reads: 114

```
@krazor 
I am not completely sure as I downloaded the newest and fixed the errors but I think this version should work:
[https://github.com/DroidSector/FireFly-Nano-Remote/tree/38f17ba0bc82cf201c678affb8a11183497a3eba](https://github.com/DroidSector/FireFly-Nano-Remote/tree/38f17ba0bc82cf201c678affb8a11183497a3eba)

BUT! 

Besides changing the globals.h you have to change two lines in the receiver.cpp:
https://github.com/DroidSector/FireFly-Nano-Remote/blob/38f17ba0bc82cf201c678affb8a11183497a3eba/src/receiver/receiver.cpp#L161

Replace WIFI_NETWORK and WIFI_PASSWORD with your (or any random) Wi-Fi credentials. Like this:

    const char* ssid = "Home-Wi-Fi";
    const char* password = "My123pass";

That should do it.
```

---
## \#471 Posted by: krazor Posted at: 2019-07-20T10:03:39.866Z Reads: 109

```
the errors i got are related to the Feather M0 which i believe the avr library does not support
```

---
## \#472 Posted by: Jamie42 Posted at: 2019-07-20T10:04:38.930Z Reads: 108

```
Ow with that I can't help you. I made the heltec version.
```

---
## \#473 Posted by: krazor Posted at: 2019-07-20T10:05:22.258Z Reads: 110

```
ah i see. i hope the feather version hasnt been dropped and im stuck with $200 worth of boards haha
```

---
## \#474 Posted by: Jamie42 Posted at: 2019-07-21T22:22:58.080Z Reads: 108

```
Hey, could you publish the code you used for this packet forwarding?? I would make a Bluetooth on/off option in the menu...
```

---
## \#475 Posted by: R8IOSHQ1 Posted at: 2019-07-31T03:30:47.925Z Reads: 110

```
Hi all, noob here! I’m building my first board. I have a couple SX1276 LoRa Transceiver Module 915MHz, the V2 versions. I loaded up the transmitter and receiver and have them both talking to each other. I figured out how to get into the settings menu on the TX but can’t navigate it. I’m thinking it’s because I don’t have the hall sensor calibrated. I used Gikfun A3144/OH3144/44E/AH3144E Hall Effect Sensor ( https://www.amazon.com/gp/product/B07QS6PN3B/ref=ppx_yo_dt_b_asin_title_o07_s00?ie=UTF8&psc=1). Can anyone point me to the thread or tell me how to set the min and max? I’m thinking I need to see the values in a terminal in visual studio but I have no idea how to pull that up. I’m assuming after that I adjust a line of code and upload it again. Any help would be awesome!! TIA.![image|375x500](upload://2Z4MGmwVK0kKadPBfLigzTkf7eX.jpeg)
```

---
## \#476 Posted by: R8IOSHQ1 Posted at: 2019-07-31T15:58:25.847Z Reads: 104

```
Okay, so I did a little research on hall sensors and realized I installed a threshold sensor instead of a linear sensor. I have the linear sensors coming now. In regards to the magnet placement in the throttle wheel, do I install the magnets with opposite poles of each other so they have a negative and a positive pole moving in from of the linear sensor as I roll it forward and backwards?
```

---
## \#477 Posted by: Xtreme Posted at: 2019-07-31T16:59:36.457Z Reads: 105

```
@R8IOSHQ1 Yes, the magnet poles should be opposite from each other (e.g. let the magnets connect to each other, pull them apart, flip one 180 degrees, then push them into their holes on the wheel).
```

---
## \#478 Posted by: R8IOSHQ1 Posted at: 2019-07-31T17:14:06.688Z Reads: 110

```
Thank you so much!! Now to go learn a little Visual Studio. I’ll update once I make a little more progress. This is such a cool remote. The programming work is amazing!
```

---
## \#479 Posted by: R8IOSHQ1 Posted at: 2019-08-05T19:39:41.797Z Reads: 112

```
I seem to be having some strange behavior in regards to the hall sensor. If I turn the remote on after it has been sitting for a while, the hall sensor seems to not be working. As soon as I plug in a micro usb to charge it, boom, it begins to work again. Any thoughts? ![image|375x500](upload://ewBXZ30ou6aq3D9pReRsIz06mdt.jpeg)
```

---
## \#480 Posted by: myreala Posted at: 2019-08-05T22:25:15.120Z Reads: 107

```
I have an entire firefly kit for this, available for just $70. If someone want to build one please take it from me.
```

---
## \#481 Posted by: krazor Posted at: 2019-08-06T10:34:09.727Z Reads: 105

```
just got the Lora v2 modules in today and pulled free from git and everything seemed to build without error. should have bought these modules inseatd of the fgeathers since they wont even build.

Well any ways i got a trigger remote in as a backup incase this thing starts playing up, i know its not perfect or refined as its still in development but i may build it this weekend and see how it goes. i have the MetR blutooth module can i use both at the same time?

Also a quick question the lipo battery i picked up fits perfectly fine in the Feather M0 but is too big for the Lora v2, what connector do i need to replace it with on the battery?
```

---
## \#482 Posted by: R8IOSHQ1 Posted at: 2019-08-08T17:34:07.934Z Reads: 103

```
I think it’s just a JST connected.

JST 1.25mm-2P Connector
```

---
## \#483 Posted by: 5oAwes0me Posted at: 2019-08-08T19:02:51.369Z Reads: 108

```
Hey
I had the same problem. first I had a SS495A1 
then I changed to a SS49E 
I'm not sure anymore I first had it connected to 5V but then I got it to work with the 3.3V line
I changed this line in the code and it worked.

ADC_ATTEN_DB_2_5 to ADC_ATTEN_DB_6

here is the post that helped 

https://www.electric-skateboard.builders/t/firefly-nano-remote/72916/402
```

---
## \#484 Posted by: R8IOSHQ1 Posted at: 2019-08-10T03:46:28.162Z Reads: 101

```
Awesome!! That worked.

Is there any way to change the speed and distance to imperial (MPH)?

Thanks
```

---
## \#485 Posted by: krazor Posted at: 2019-08-10T05:37:25.822Z Reads: 104

```
this is the one i have on my battery and its too big ![IMG_20190810_150635|666x499](upload://kpM3WuiGYGAzWRsnLvrUZ8gtcDu.jpeg)
```

---
## \#486 Posted by: Xtreme Posted at: 2019-08-10T06:00:22.200Z Reads: 103

```
I used this connector: Letool®30 Pairs JST 1.25mm 2 Pin Micro Male Female Connector Plug 80mm Wires Cables https://www.amazon.com/dp/B013JRWCBU/ref=cm_sw_r_em_apap_nuFsbCqHsDCqg. 

If you're in the U.S., I'll drop one in the mail to you.
```

---
## \#487 Posted by: krazor Posted at: 2019-08-10T06:16:31.814Z Reads: 103

```
sadly im in the AU so shipping takes weeks from bang good and stores like that was hoping someone in Adelaide had a spare one i could buy off them. i was looking for a couple pieces the come with wires at this point ide be better off buying another battery from coreelectronics online and paying the $20 even though i got 2 of these batteries sitting on my desk. they fit perfectly in the feather M0 but the Lora is a no go

found a seller on ebay that has them for $1 per cable so i got some 1mm and 1.25mm male pieces so 1 of these should fit. ill see how it goes. thanks nay ways though =)

Picked up some 1mm and 1.25mm didnt realise it was actualyl $1 for 10 pieces im assuming 5 male and 5 female picked up 20 of each 1mm and 1.25mm so ill see how it goes =) 


[Ebay Seller](https://www.ebay.com.au/itm/10pcs-JST-2-3-4-5-6-7-8-12-Pin-Male-Female-Battery-Connector-Plug-With-Cable/264338635034?ssPageName=STRK%3AMEBIDX%3AIT&var=563935298515&_trksid=p2057872.m2749.l2649)
```

---
## \#488 Posted by: Xtreme Posted at: 2019-08-10T06:19:18.097Z Reads: 96

```
Or you could just solder the battery to the board.
```

---
## \#489 Posted by: krazor Posted at: 2019-08-10T06:20:45.865Z Reads: 95

```

i was thinking about it honestly but the battery port is on the other end of the USB port i dont want to mess it up i was going to replace the JSt conenctor with a larger one but its not worth messing up so i rahter replace the conenctor on the battery
```

---
## \#490 Posted by: R8IOSHQ1 Posted at: 2019-08-11T13:50:09.561Z Reads: 96

```
I just spliced the connector with the JST the LoRa board came with. Did yours come with a battery lead?
```

---
## \#491 Posted by: R8IOSHQ1 Posted at: 2019-08-11T13:53:26.558Z Reads: 92

```
Well I have searched all over the code. I don’t know enough C++ to figure out how to change km/h to mph and km to m . Can anyone help? I read somewhere that the remote will bounce between both on the display. If that’s the case I guess it’s cool. I’m still building the board so I have not seen the remote live yet.
```

---
## \#492 Posted by: krazor Posted at: 2019-08-11T14:05:37.396Z Reads: 95

```
nope no lead with mine
```

---
## \#493 Posted by: Jamie42 Posted at: 2019-08-11T16:41:33.424Z Reads: 100

```
I know where those calculations are made. I will take a look later today and post here how to do that.
```

---
## \#494 Posted by: R8IOSHQ1 Posted at: 2019-08-14T00:53:20.570Z Reads: 103

```
Any update on where the calculations for the MPH are. 

I have the receiver and remote connected and the Rx and Tx plugged into the ESC. How do I get this ESC to see the receiver in VESC? I have tried the wizard but no dice. Total noob here, this is my first build. I already set up the motor and is spins correctly. 

Thanks![image|666x500](upload://7Eow1sYQ0qWnpJ4NQ7o1zfHtN8p.jpeg) ![image|375x500](upload://AdPQjrH6dlM2oaOXHJu5mrlmo0L.jpeg)
```

---
## \#495 Posted by: R8IOSHQ1 Posted at: 2019-08-14T23:58:59.814Z Reads: 107

```
Well I’m at wits end with getting this thing connected to the VESC. I am not sure how to get it to talk over the Rx and Tx in VESCtool. The receiver and transmitter seem to be talking and showing throttle, but when I go to connect it to VESCtool and try to set up the transmitter, I don’t get any feedback. I also noticed the speed on the remote keeps jumping around. Please help! I’m crying here guys.  ![image|375x500](upload://zOGik4vzPRTawmK9XrARgQXbanx.jpeg) ![image|375x500](upload://l3VQGrtUO3qGwCpJyCXdyiYbYtM.jpeg)
```

---
## \#496 Posted by: R8IOSHQ1 Posted at: 2019-08-15T03:10:24.292Z Reads: 107

```
I figured it out!!

#define FAKE_UART // Comment out after pairing the remote and connecting VESC

Helped if I could read.
```

---
## \#497 Posted by: nativejibroney22 Posted at: 2019-08-16T11:45:16.677Z Reads: 105

```
@DroidSector I am getting this error when I build the code for my remote. Anyway you could help me with this?

    Compiling .pio\build\Remote.Feather\src\remote\remote.cpp.o
    Archiving .pio\build\Remote.Feather\lib559\libWire.a
    src\remote\remote.cpp: In function 'void sleep()':
    src\remote\remote.cpp:343:15: error: 'class Adafruit_USBD_Device' has no member n
    amed 'standby'
         USBDevice.standby();
               ^~~~~~~
    src\remote\remote.cpp:419:15: error: 'class Adafruit_USBD_Device' has no member n
    amed 'attach'
         USBDevice.attach();
               ^~~~~~
    Compiling .pio\build\Remote.Feather\lib1ee\Adafruit_ZeroDMA\Adafruit_ZeroDMA.cpp.
    o
    *** [.pio\build\Remote.Feather\src\remote\remote.cpp.o] Error 1
    Compiling .pio\build\Remote.Feather\lib8c6\SPI\SPI.cpp.o
    ========================== [ERROR] Took 4.13 seconds ==========================

     

    ================================== [SUMMARY] ==================================

    Environment Remote.Heltec.v2            [IGNORED]
    Environment Receiver.Heltec.v2          [IGNORED]

    Environment Remote.TTGO.OLED.v1         [IGNORED]

    Environment Remote.Feather              [FAILED]

    ==================== 1 failed, 0 succeeded in 4.14 seconds ====================

    Environment Receiver.TTGO.OLED.v1       [IGNORED]
    Environment Receiver.Feather            [IGNORED]
```

---
## \#498 Posted by: nativejibroney22 Posted at: 2019-08-16T20:26:18.548Z Reads: 100

```
When you ended up getting the M0 were you able to get rid of this error? I am using the right board but still have it :/
```

---
## \#499 Posted by: annihil8ted Posted at: 2019-08-16T21:18:19.171Z Reads: 100

```
Can someone modify the STL for left handed people :stuck_out_tongue: I realized that mirroring the print isn't enough since the lcd is not fully centered.
```

---
## \#500 Posted by: Jonisonvespa Posted at: 2019-08-16T21:25:20.093Z Reads: 101

```
hello would really like to build one of these but nont have a printer looking for someone to print would obviously pay of course
thanks
```

---
## \#501 Posted by: annihil8ted Posted at: 2019-08-17T19:05:31.135Z Reads: 93

```
Where are you based? I don't mind printing and shipping you some. 

On a separate note, the ones I'm printing have a small gap between the top and bottom shell and it looks like the print is dimensionally accurate. Is this normal? It's almost purely cosmetic and I can always sand the protruding innards so the shell closes seamlessly but I wanted to ask first.
```

---
## \#502 Posted by: walleywalker Posted at: 2019-08-17T23:12:10.793Z Reads: 93

```
Is it safe to say that urban residing people have had more success with this remote and drop-outs than the FeatherRemote? 

ie. If I am going to build one, does the hardware make any difference at all if they're both on 915mhz?
```

---
## \#503 Posted by: annihil8ted Posted at: 2019-08-18T05:31:47.691Z Reads: 91

```
I think it's been deemed the Heltec is the superior build. You can do both but I think the Heltec is more up to the task.

For the magnets, how is the polarity suppose to work? Is it two north sides facing up or one north, one south?
```

---
## \#504 Posted by: Xtreme Posted at: 2019-08-18T05:46:35.472Z Reads: 88

```
Opposite poles on the magnets, one north, one south.
```

---
## \#505 Posted by: annihil8ted Posted at: 2019-08-18T06:17:36.622Z Reads: 95

```
Here's a quote I found from above:
> 
> Yes, only Heltec board will fit. All essential functions work fine on both boards. Heltec is cheaper and has BT and WiFi, which allows adding OTA updates and some features in the future. You can also use it as a [battery meter ](https://www.youtube.com/watch?v=Dv1gESdI6rU) inside ESC enclosure.
```

---
## \#506 Posted by: R8IOSHQ1 Posted at: 2019-08-19T00:50:29.937Z Reads: 98

```
Well I went for my first test drive. I can say the breaks work great. It goes faster then I can handle and it appears to have a solid connection using the Heltec V2. I’m so stoked to be a part of this group.![image|500x500](upload://cYkYLawqlwDfKknjArB4hAPi89u.jpeg)
```

---
## \#507 Posted by: Jamie42 Posted at: 2019-08-19T08:45:03.352Z Reads: 101

```
Hey there,

I am sorry that I didn't hold on to my promise, a lot of things came that I needed to do first.

Here you go: 
https://github.com/DroidSector/FireFly-Nano-Remote/blob/master/src/receiver/receiver.cpp#L959-L972


You can add a factor to these calculations to turn them into mph: 0.621371192.

So:

    float rpm2speed(long rpm) {
      return abs(ratioRpmSpeed * rpm) * 0.621371192;
    }

    long speed2rpm(uint8_t speed) {
      return speed / 0.621371192 / ratioRpmSpeed;
    }

    float tach2dist(long tachometer) {
      return ratioPulseDistance * tachometer * 0.621371192;
    }

Edit 1: Now just search (CTRL+F usually) through the code and edit kmh to mph.
```

---
## \#508 Posted by: R8IOSHQ1 Posted at: 2019-08-19T10:47:41.103Z Reads: 96

```
Awesome!!! Thank you so much!! 🤛🤙🏻😎
```

---
## \#509 Posted by: Jonisonvespa Posted at: 2019-08-19T11:04:56.625Z Reads: 94

```
Please delete
```

---
## \#510 Posted by: R8IOSHQ1 Posted at: 2019-08-20T03:22:49.724Z Reads: 99

```
[quote="Jamie42, post:507, topic:72916"]
ratioRpmSpeed
[/quote]

Am I figuring this correctly for accurate MPH?

(globlas.h)

void calculateRatios() {
  // Gearing ratio
  gearRatio = (float)boardConfig.motorPulley / (float)boardConfig.wheelPulley;
  // ERPM to Km/h
// default board configuration
const int MAX_SPEED = 30;       // KM/H
const int MAX_RANGE = 30;       // KM
const int BATTERY_CELLS = 10;
const int BATTERY_TYPE = 0;     // 0: LI-ION | 1: LIPO
const int MOTOR_POLES = 12;
const int WHEEL_DIAMETER = 83; mm
const int WHEEL_PULLEY = 36; /teeth
const int MOTOR_PULLEY = 16 /teeth

(receiver.pp)

 ratioRpmSpeed = (gearRatio * 60 * (float)boardConfig.wheelDiameter * 3.14156) / (((float)boardConfig.motorPoles / 2) * 1E6);
  // Pulses to km travelled
  ratioPulseDistance = (gearRatio * (float)boardConfig.wheelDiameter * 3.14156) / (((float)boardConfig.motorPoles * 3) * 1E6);
}
```

---
## \#511 Posted by: R8IOSHQ1 Posted at: 2019-08-20T13:26:19.615Z Reads: 90

```
I think I just uploaded to the remote not the receiver. That may be the problem. I’ll check it when I get home. 😳
```

---
## \#512 Posted by: Jamie42 Posted at: 2019-08-22T12:04:47.656Z Reads: 91

```
What do you mean? And could you please use code blocks? It's in your text editor :slight_smile:

Did you get it working?
```

---
## \#513 Posted by: nativejibroney22 Posted at: 2019-08-25T01:27:32.588Z Reads: 95

```
@R8IOSHQ1 Hey sorry to call on you, but you seem to understand how the code works for this. I've been sitting here for a week with everything put together but my remote code, so I'm getting kind of desperate lol. Do you have any idea why i am getting the error i am when i try to build the code? I keep getting "error: 'class Adafruit_USBD_Device' has no member n
amed 'standby'" as well as one fore attach
Any help would be massively appreciated
```

---
## \#514 Posted by: R8IOSHQ1 Posted at: 2019-08-25T01:44:22.655Z Reads: 94

```
I got it working!! Now I just need to fix the Km traveled to Miles. Then I’m good to go.
```

---
## \#515 Posted by: Jamie42 Posted at: 2019-08-25T09:05:04.833Z Reads: 91

```
Could you send the complete error? Indented in code tags please. 

Did you buils Heltec or Feather?
```

---
## \#516 Posted by: Jamie42 Posted at: 2019-08-25T09:06:49.505Z Reads: 90

```
Just replace the code by the code I gave you and then search km and replace it by miles.
```

---
## \#517 Posted by: nativejibroney22 Posted at: 2019-08-25T10:01:15.890Z Reads: 102

```
    Processing Remote.Feather (platform: atmelsam; framework: arduino; board: adafruit_feather_m0)

    -------------------------------------------------------------------------------

    Verbose mode can be enabled via `-v, --verbose` option

    CONFIGURATION: https://docs.platformio.org/page/boards/atmelsam/adafruit_feather_m0.html

    PLATFORM: Atmel SAM 3.8.0 > Adafruit Feather M0

    HARDWARE: SAMD21G18A 48MHz, 32KB RAM, 256KB Flash

    DEBUG: Current (atmel-ice) External (atmel-ice, blackmagic, jlink)

    PACKAGES: toolchain-gccarmnoneeabi 1.70201.0 (7.2.1), framework-arduinosam 4.3.190711

    LDF: Library Dependency Finder -> http://bit.ly/configure-pio-ldf

    LDF Modes: Finder ~ chain, Compatibility ~ soft

    Found 15 compatible libraries

    Scanning dependencies...

    Dependency Graph

    |-- <Wire> 1.0

    |-- <SPI> 1.0

    |   |-- <Adafruit Zero DMA Library> 1.0.4

    |-- <Adafruit GFX Library> 1.5.6

    |   |-- <SPI> 1.0

    |   |   |-- <Adafruit Zero DMA Library> 1.0.4

    |   |-- <Adafruit Zero DMA Library> 1.0.4

    |-- <Smoothed> 1.1

    |-- <RadioHead> 1.89

    |   |-- <SPI> 1.0

    |   |   |-- <Adafruit Zero DMA Library> 1.0.4

    |-- <FlashStorage> 0.7.1

    |-- <VescUart> 1.0.0

    |-- <Adafruit_SSD1306>

    |   |-- <Wire> 1.0

    |   |-- <Adafruit GFX Library> 1.5.6

    |   |   |-- <SPI> 1.0

    |   |   |   |-- <Adafruit Zero DMA Library> 1.0.4

    |   |   |-- <Adafruit Zero DMA Library> 1.0.4

    |-- <CPU>

    Compiling .pio\build\Remote.Feather\src\remote\remote.cpp.o

    Compiling .pio\build\Remote.Feather\src\shared\esp32\radio.cpp.o

    Compiling .pio\build\Remote.Feather\src\shared\samd\radio.cpp.o

    Compiling .pio\build\Remote.Feather\src\shared\utils.cpp.o

    Compiling .pio\build\Remote.Feather\lib559\Wire\Wire.cpp.o

    src\remote\remote.cpp: In function 'void sleep()':
    src\remote\remote.cpp:343:15: error: 'class Adafruit_USBD_Device' has no member named 'standby'
         USBDevice.standby();
                   ^~~~~~~
    src\remote\remote.cpp:419:15: error: 'class Adafruit_USBD_Device' has no member named 'attach'
         USBDevice.attach();
                   ^~~~~~

    *** [.pio\build\Remote.Feather\src\remote\remote.cpp.o] Error 1
    ========================= [FAILED] Took 9.02 seconds =========================
     
    Environment            Status    Duration
    ---------------------  --------  ------------
    Remote.Heltec.v2       IGNORED
    Receiver.Heltec.v2     IGNORED
    Remote.TTGO.OLED.v1    IGNORED
    Receiver.TTGO.OLED.v1  IGNORED
    Remote.Feather         FAILED    00:00:09.018
    Receiver.Feather       IGNORED
    ==================== 1 failed, 0 succeeded in 00:00:09.018 ====================

That's everything I got when I tried to build the code.
And I'm using a feather.
```

---
## \#518 Posted by: Jamie42 Posted at: 2019-08-25T13:01:25.457Z Reads: 89

```
Hey, I have been trying to search for a solution but I can't find it. Only thing that might work is removing the lines:
    USBDevice.standby();
And 
    USBDevice.attach();

I don't really know the code for feather. Also don't have one. I can tell you all about the heltec...
```

---
## \#519 Posted by: nativejibroney22 Posted at: 2019-08-25T20:05:15.462Z Reads: 92

```
Alright thank you for looking at it for me man.
@DroidSector or @solidgeek If one of you could please help me with this that would be amazing, I'm getting desperate haha. I've been sitting here with a finished board for over a week but can't ride it cause I can't flash the firmware and I'm slowly going crazy lol.
```

---
## \#520 Posted by: Jamie42 Posted at: 2019-08-25T20:12:02.240Z Reads: 89

```
Did you try removing those two lines in the remote.cpp?
```

---
## \#521 Posted by: nativejibroney22 Posted at: 2019-08-25T20:17:04.021Z Reads: 87

```
I am about to right now, but I just noticed it says 'class Adafruit_USBD_Device' which I believe should be USB not USBD right? Do you know where that class is defined?
```

---
## \#522 Posted by: Jamie42 Posted at: 2019-08-25T20:18:54.620Z Reads: 86

```
Nope, it is exactly what I have been lookinf for while trying to fix your issue, but I can't find the damn class! Did found some other stuff only, I have the feeling that it's using the wrong class as USBDevice.standby() is part of the Arduino core.

**Edit:** This all seems to relate to the serial debug when you plug it in to your computer. Thing is that I also read stories that code doesn't continue executing if the serial isn't put in standby/waked properly so it will be trial and error for you I guess. Hope removing those lines will work ans just disable your serial output or something. But maybe you processor won't even sleep at all...
```

---
## \#523 Posted by: nativejibroney22 Posted at: 2019-08-26T00:27:19.948Z Reads: 89

```
I'm still continuously getting errors when I try to build it. Is there anyway I could get a link to the code you used so I can clone it to my github?

EDIT: Ok so I cleared everything and started over. I commented out the standby and attach, then it came up in the samd.cpp file, so I commented it out there. It finally built this time and uploaded
```

---
## \#524 Posted by: nativejibroney22 Posted at: 2019-08-26T01:54:10.111Z Reads: 99

```
And now a whole new error when trying to build the receiver code :/ 

    Compiling .pio\build\Receiver.Feather\src\receiver\receiver.cpp.o

    Compiling .pio\build\Receiver.Feather\src\shared\esp32\radio.cpp.o

    Compiling .pio\build\Receiver.Feather\src\shared\samd\radio.cpp.o

    Compiling .pio\build\Receiver.Feather\src\shared\utils.cpp.o

    src\receiver\receiver.cpp: In function 'void setup()':

    src\receiver\receiver.cpp:103:11: error: 'Vext' was not declared in this scope

       pinMode(Vext, OUTPUT);

               ^~~~

    src\receiver\receiver.cpp:103:11: note: suggested alternative: 'exit'

       pinMode(Vext, OUTPUT);

               ^~~~

               exit

    *** [.pio\build\Receiver.Feather\src\receiver\receiver.cpp.o] Error 1

    ========================= [FAILED] Took 9.38 seconds =========================

     

    Environment Status Duration

    ---------------------  --------  ------------

    Remote.Heltec.v2       IGNORED

    Receiver.Heltec.v2     IGNORED

    Remote.TTGO.OLED.v1    IGNORED

    Receiver.TTGO.OLED.v1  IGNORED

    Remote.Feather         IGNORED

    Receiver.Feather FAILED    00:00:09.381

    ==================== 1 failed, 0 succeeded in 00:00:09.381 ====================
```

---
## \#525 Posted by: nativejibroney22 Posted at: 2019-08-26T08:33:58.375Z Reads: 89

```
I'm about to give up and spend the money to get the heltec board lol
```

---
## \#526 Posted by: KranzeKake Posted at: 2019-08-26T11:11:01.231Z Reads: 87

```
Anyone who is willing to make one for me? I really want one with a 2.4 transmitter
```

---
## \#527 Posted by: Jamie42 Posted at: 2019-08-26T11:21:02.729Z Reads: 92

```
I just pushed my modified version for you, compiled it with Remote.Feather succesfully. Hope it works for you. (Branch: patch-1)

There's one thing however: I modified this version to my needs. Here in The Netherlands eboarding is illegal. The police in my area told me that it was okay if you couldn't push the throttle yourself and had to push the board to activate cruise control for some time and then push again. So there's a "police" mode that comes with this code. Mind that it is not sync'd up yet. When you turn off your remote (and leave board on) while in police mode and then turn it back on, the board will be in police mode and the remote in normal mode. This will give some nasty complications when you push the throttle, to fix this, set the remote to police again. (And then back to Sport if you want normal mode on board and remote)

https://github.com/Jamie4224/FireFly-Nano-Remote/tree/patch-1


**Edit**: Ow nevermind, I didn't saw that you got it working. Does it also work after powering it on and off with the button?
```

---
## \#528 Posted by: Jamie42 Posted at: 2019-08-26T11:21:23.838Z Reads: 87

```
I don't think this remote is designed for 2.4Ghz use
```

---
## \#529 Posted by: nativejibroney22 Posted at: 2019-08-26T12:26:17.176Z Reads: 99

```
Ok awesome, thank you so much! I got both working but there are some complications. I had to comment out a piece of the receiver code that used pinMode(Vext, OUTPUT) and digitalWrite(Vext, LOW) because it was saying Vext wasn't declared in this scope, even when I defined vext as pin 21. I am not sure what that does, but my remote is going now.

The main issues I am having are that the remote sometimes freezes and the deadman switch only stops the throttle till i push it once, then the throttle is open regardless of pushing the deadman. Also the Focbox Unity software gets stuck if I try to calibrate my remote throttle.
```

---
## \#530 Posted by: nativejibroney22 Posted at: 2019-08-26T13:53:34.187Z Reads: 99

```
Holy shit, I finally got to test my board haha. So, the remote hasn't frozen yet but makes me nervous. The deadman switch operates as such at first, then becomes a cruise control. I think this is the way it is supposed to be?

So, so far the only issue is for some reason my throttle is backwards. If i pull the wheel back it gives it gas and if I push it forward it brakes. This isn't the that big a problem and I could live with it, but if I had the choice it would be the other way.
```

---
## \#531 Posted by: Jamie42 Posted at: 2019-08-26T17:04:47.015Z Reads: 100

```
I believe the code you commented out is for cutting power to the display, not sure, however. Why don't you try just replacing Vext everywhere with 21?

What do you mean by "freezing", what happens? 

The dead man's switch behavior is totally normal. It is supposed to behave like this:

* When "locked", unlock the throttle by clicking it, the throttle will now be unlocked for a default of 10 seconds, (setting: REMOTE_LOCK_TIMEOUT).
* You can now use the throttle, if you don't the throttle will lock again.
* When the board is moving the throttle will stay unlocked, and the trigger will be a cruise control.
* When you press the trigger, the throttle wheel is in default position and you are moving faster than 3 Km/h you will cruise.
* When you are not moving anymore and don't touch the controls it will time-out again after 10 secs default.

Backwards throttle is caused by wrong magnet polarity, you might be able to reverse your throttle in software.
```

---
## \#532 Posted by: nativejibroney22 Posted at: 2019-08-27T21:55:36.067Z Reads: 94

```
How would i go about that?

It hasn't done it with normal use but it did it when I went into the menu. The whole thing just froze and I had to hit the reset button on it.

Ahh alright, thank you for explaining that to me!

Do you have any idea where that might live in the code?
```

---
## \#533 Posted by: nativejibroney22 Posted at: 2019-08-30T08:44:50.980Z Reads: 89

```
I don't know why, but I'm still struggling to find in the code where to change the polarity of the magnets haha.
```

---
## \#534 Posted by: DroidSector Posted at: 2019-08-31T17:11:29.918Z Reads: 95

```
It's in the readThrottlePosition() function.

[quote="nativejibroney22, post:529, topic:72916"]
I had to comment out a piece of the receiver code that used pinMode(Vext, OUTPUT) and digitalWrite(Vext, LOW) because it was saying Vext wasn’t declared in this scope, even when I defined vext as pin 21.
[/quote]

Vext is declared in 
~\.platformio\packages\framework-arduinoespressif32\variants\heltec_wifi_lora_32_V2\pins_arduino.h, it should present if ` board = heltec_wifi_lora_32_V2 ` is present in platformio.ini. You can also check if there are any updates available in PlatformIO Home tab.
```

---
## \#535 Posted by: xpsking Posted at: 2019-09-02T23:26:37.752Z Reads: 92

```
I know this has been asked before, but is there a way for us to get .STEP or any other kind of modifiable file of the 3d print?
```

---
## \#536 Posted by: matiller Posted at: 2019-09-30T17:51:05.167Z Reads: 81

```
Hey! 
I am total noob in UART things in here (always used just PPM). My question: when wizard setup input, should I chose NRF remote or Nunchuck? (tried both, the receiver and VESC just dont talk to each other) 

Receiver -- VESC,
RX          -- TX,
TX          -- RX,
3.3v        --3.3,
gnd         --gnd,
baud 115200, firmware 3.62


Thanks.
```

---
## \#537 Posted by: Jamie42 Posted at: 2019-09-30T18:03:25.677Z Reads: 78

```
Wiring is correct. You should set your app to 'UART'.
```

---
## \#540 Posted by: Kodin Posted at: 2019-10-08T22:07:37.936Z Reads: 83

```
I'm looking to add SPI addressable LED strips to the underside of my board with a shifting rainbow pattern facing the ground; the goal will be to sync to the position/speed readings off the ESC's and shift the pattern accordingly so it looks like a given color of the rainbow stays static in one spot on the ground as I move forward.  (shift the pattern backward exactly as fast as I'm moving forward)  Do you think that the ESP32 has enough overhead to be able to handle the load of driving the LED's without risking increasing remote response latency?  I'm probably going to use APA102 LED's since they use two-wire SPI with variable clock rates and the FastLED library.  Just curious how sane this sounds, or if anyone recommends I run all of that on a separate MC for safety or practicality reasons.  Already using Samguyer's fork with headlight/brake light control, it works great for that purpose.  Also would be curious to eventually add an extra control for turn signals, though that's more just because I think it'd be funny to see on a skateboard.  Coolest would be if I could add a pushbutton for my ring or pinkey finger and a gyro to read the remote tilt, thus allowing the remote to know which direction to activate the signal on.
```

---
## \#541 Posted by: Kodin Posted at: 2019-10-08T22:15:39.222Z Reads: 85

```
Separate issue: I cannot for the life of me get the receiver to connect to my WiFi.  Does it support WPA2 secured networks or would I need to add a library to provide that support?  As my receiver is almost ready to be potted into my controller enclosure I'd like something that can still be maintained.  Has anyone gotten this to work successfully?

@DroidSector?
```

---
## \#542 Posted by: Movation Posted at: 2019-10-13T10:09:01.030Z Reads: 79

```
I tried this trying to run a speed controlled sk6812 144led RGBW off my reciever esp32 using neopixel library (no official rgbw support in fastled) break light animation worked but others caused remote to be unresponsive. I instead opted for a seperate $3 esp8266 board controlled by esp32 remote and a ws2812 driver board $2, after getting the boards I abbanded my nano esp32 remote infavor of a flipsky vx2 manly due to the issues with hall effect throttle sub par performance.  I have the esp8266 connected to the second uart port on my vesc and though the animations are still work in progress. I can turn my lights on and off change animation via phone app. I am looking at getting the esp8266 to also emulate a bluetooth reciever so I can run the vesc tool.
```

---
## \#543 Posted by: Jamie42 Posted at: 2019-10-22T14:53:46.882Z Reads: 77

```
I've been trying this very thing, too. Haven't got it to work. Still trying.

You could try my version:
It has several improvements like one remote, several receivers. 
https://github.com/Jamie4224/FireFly-Nano-Remote/tree/development

Note that the code is in the development branch.
```

---
## \#544 Posted by: infiniteoffset Posted at: 2019-10-26T06:56:15.581Z Reads: 68

```
I build the heltec remote yesterday, but it has poor range - only few centimeters. I tried to switch antennas, but it didn't help. My heltec board might be defective, is there way how to test if the board is working properly? Some kind of hello world firmware?
```

---
## \#545 Posted by: Jamie42 Posted at: 2019-10-26T07:17:49.139Z Reads: 72

```
Hi, what antennas did you try? You got pictures?
```

---
## \#546 Posted by: infiniteoffset Posted at: 2019-10-26T07:31:02.898Z Reads: 76

```
Ones that were supplies with the boards and the "upgraded" ones from the shopping list <!--td {border: 1px solid #ccc;}br {mso-data-placement:same-cell;}-->https://www.aliexpress.com/item/433Mhz-built-in-PCB-antenna-ipex-connector-18cm-long-2/32513779043.html

EDIT: Antennas that I got with board looks like exposed coil. I see that the board can come with different antennas. I have 433mhz version.

![_SX355_|355x327](upload://7oq8PmcASjvy1zeYXDIqt3G57jp.jpeg)
```

---
## \#547 Posted by: Jamie42 Posted at: 2019-10-26T08:42:25.547Z Reads: 75

```
Oh sorry I can't help you with that one. I have a 868Mhz version and that one works just fine.
```

---
## \#548 Posted by: scott1988 Posted at: 2019-10-31T18:50:12.604Z Reads: 72

```
![remote|690x388](upload://5cZTJR7aWIXHq1KwNiYFcyOi0Gu.jpeg) 

Hi, 
Thanks for all the hard work you have done on this code! 
I'm having a bit of a problem building some of the code hopefully there is a file attached to this post. 
If anyone could help I would be greatful.
```

---
## \#549 Posted by: Jamie42 Posted at: 2019-11-01T09:23:47.991Z Reads: 69

```
Hi,

Please try this version, I improved @DroidSector's code. 

https://github.com/Jamie4224/FireFly-Nano-Remote/tree/development
```

---
## \#550 Posted by: scott1988 Posted at: 2019-11-01T17:43:38.809Z Reads: 71

```
Hi Jamie, 
It still doing the same thing. Not sure if I'm missing something I need to install. They won't even build on my PC which is weird. 
Thanks for getting back to me.
![build|690x388](upload://eY62yXIhuTIIbazmB8uNCH4sbds.jpeg)
```

---
## \#551 Posted by: Jamie42 Posted at: 2019-11-01T18:59:56.399Z Reads: 69

```
Ow I'm so sorry, apparently the version that's on github has an error. I'm currently not home so I will fix this on Monday. You're not doing anything wrong.
```

---
## \#552 Posted by: scott1988 Posted at: 2019-11-01T19:37:16.199Z Reads: 70

```
Thanks Jamie! Cheers for sorting that out for me

Does anyone have code that works for the ttgo v1? I've tried and tried. Managed to upload to the board but the screens not coming up with anything. I'm guessing it's because I've message around with the code.
```

---
## \#553 Posted by: DroidSector Posted at: 2019-11-07T13:47:58.390Z Reads: 66

```
Uploaded .step and .f3d files:

https://www.dropbox.com/sh/52miyzee5i7opfj/AACM2zFjeKi1gpSQLEyf1378a?dl=0
```

---
## \#554 Posted by: DroidSector Posted at: 2019-11-07T13:52:39.659Z Reads: 64

```
It should work with WPA2, however for some reason uploading didn't work on my PC, only on Mac. You can try to create a WiFi hotspot on your mobile device with the same credentials.
```

---
## \#555 Posted by: TechVic Posted at: 2019-11-19T11:05:19.057Z Reads: 51

```
When will the Board settings menu be ready?
Thanx for a nice little project
```

---
## \#556 Posted by: Kodin Posted at: 2019-11-26T21:42:51.812Z Reads: 50

```
Also the latest version of PlatformIO doesn't compile the code any more. Had to downgrade to the second to last version to get it to compile reliably (on Windows).  In addition, is the odometer supposed to keep a continuous count between power cycles? Mine has always reset after powering off the board.  Considering you're writing to flash periodically for that very purpose, I'd like to find a way to fix that if I can.  Possibly later on with a trip/overall odometer counter.
```

---
## \#557 Posted by: nativejibroney22 Posted at: 2019-11-30T22:15:39.548Z Reads: 50

```
Did you ever figure out how to upload the firmware after commenting out fake uart on the heltec? I am getting the same thing and am not sure how to fix it.
```

---
## \#558 Posted by: nativejibroney22 Posted at: 2019-12-01T01:45:21.646Z Reads: 47

```
@DroidSector how should I go about uploading the firmware while the heltec board is connected to the vesc? Whenever I comment out the fake_uart line while its connected and paired with the remote it gives me the "failed to connect to esp32" error.
```

---
## \#559 Posted by: Jamie42 Posted at: 2019-12-01T09:58:43.540Z Reads: 46

```
You can't really. The ESP has one serial interface, this is used for the usb port and the vesc comms, if you wsnt to update, disconnect from the vesc.
```

---
## \#560 Posted by: nativejibroney22 Posted at: 2019-12-01T10:29:59.032Z Reads: 43

```
Huh, alright. Then how do I do the part of the firmware flashing where he says 

" Connect the receiver to the VESC. Uncomment  `#define FAKE_UART`  line and rebuild and upload the code. Now you should be able to see the real telemetry on the remote."
```

---
## \#561 Posted by: Jamie42 Posted at: 2019-12-01T19:55:16.052Z Reads: 43

```
No idea, just try uploading while not connected to your vesc and then connect the receiver to your vesc.
```

---
## \#562 Posted by: nativejibroney22 Posted at: 2019-12-01T21:41:27.471Z Reads: 43

```
And for some reason it won't turn on at all when the battery is plugged in. I can turn it on when its plugged into a power source, but then I plug in the battery and it shuts off. The batter is fully charged, I have a multi meter to test it and the battery works with some of my other arduino boards so its just this one

Edit: @DroidSector So it looks like the screens just arent turning on when the battery is plugged in, I can still turn it on and off based on the white light on the board, but there is nothing on the screen till I unplug the battery
```

---
## \#563 Posted by: nativejibroney22 Posted at: 2019-12-02T09:17:45.757Z Reads: 46

```
Ok so I think I got that sorted.

So now the only issue is that the screen on the remote won't turn on while the battery is connected. I can see from the reciever that they pair and there is signal between them, but the screen will not be on. I have tried loading the code either way between the two heltec boards I have so I know it's not the screen being faulty. The screen will turn on if it is powered by the USB port, but as soon as I plug in the battery it goes off.

@DroidSector Please, some input would be greatly appreciated, when I have used your remote it has been amazing.
```

---
## \#564 Posted by: Lucifer Posted at: 2019-12-02T10:46:01.156Z Reads: 50

```
The battery voltage reading has to be calibrated. There is a function that turns the screen off if the battery voltage is low. If the reading is incorrect, the remote thinks the battery is empty and turns the screen off.

To fix it :

1) in globals.h find the line DISPLAY_BATTERY_MIN = 15;
and change the value to 0 (its the percentage of the battery voltage range under which the screen is off)

2) in remote.cpp, find the function batteryLevelVolts(){}

in this function there is a line where the variable voltage is calculated. You have to add a correction factor. To get it, plug the remote and wait for the battery to be fully charged (which is at 4.1v). Then, switch the remote on, and read the incorrect value on the screen.

Now you can correct the voltage this way:

voltage = voltage * 4.1 / (incorrectValue);
```

---
## \#565 Posted by: Jamie42 Posted at: 2019-12-02T11:18:10.439Z Reads: 50

```
Thanks for explaining, I was about to do that. Just don't forget to set the DISPLAY_BATTERY_MIN, Otherwise you won't see it coming when the board goes in estop when the remote is dead.
```

---
## \#566 Posted by: nativejibroney22 Posted at: 2019-12-02T19:10:10.263Z Reads: 48

```
Yessss, thank you so much! Its working well now!
Also, thank you @Jamie42 for all your help!
```

---
## \#567 Posted by: nativejibroney22 Posted at: 2019-12-02T20:14:35.459Z Reads: 47

```
So it looks like it is calculating the battery to be at a different voltage than it is. My multimeter and power supply are both reading it at 4.1 to 4.2v where the remote thinks that its at 3.4v. Should I just add 0.8v in the remotes code calculation of voltage?
```

---
## \#568 Posted by: Jamie42 Posted at: 2019-12-02T20:57:58.069Z Reads: 49

```
[quote="DroidSector, post:347, topic:72916"]
@deltazeta You can tweak [this line ](https://github.com/DroidSector/FireFly-Nano-Remote/blob/38f17ba0bc82cf201c678affb8a11183497a3eba/src/remote/remote.cpp#L936), add * 4 / 4.4.
[/quote]

@nativejibroney22 You should tweak that, add * (actual voltage) / (screen voltage)
```

---
## \#570 Posted by: nativejibroney22 Posted at: 2019-12-03T01:39:14.498Z Reads: 51

```
Ok perfect that got it straightened out.

I’m still not able to get real telemetry data from the vesc. I feel like it has to do with that connect to uart then flash thing. The remote controls the board and the reciever and remote communicate well, but I can’t get info like speed and battery percent from the vesc to the heltec. I got that info when I used a feather board but I would like to use the heltec as it’s just overall run smoother and with a better connection.
```

---
## \#571 Posted by: Jamie42 Posted at: 2019-12-03T07:47:52.890Z Reads: 47

```
You set everything up in globals.h? Do you get the battery voltage and no percentage or none? Connected rx/tx/gnd correctly?
```

---
## \#573 Posted by: nativejibroney22 Posted at: 2019-12-03T20:47:45.471Z Reads: 48

```
Yeh I set up globals. I made sure the connections were right, the board wouldn’t be able to get throttle input from my reciever if those were wrong right? I’ve tried flipping tx and rx and it didn’t work. I dont get any data. When I break and am at a stop it reads weird data, like the speed and battery percent jump all over the place. But other than that it just says 0 for both all the time.
```

---
## \#574 Posted by: Jamie42 Posted at: 2019-12-03T21:45:31.081Z Reads: 46

```
What VESC are you using?
```

---
## \#576 Posted by: nativejibroney22 Posted at: 2019-12-04T03:21:26.363Z Reads: 48

```
I am using the Focbox Unity. Not sure why it isnt working cause I got it going with the feather and I flashed with it plugging into the Unity. Baud rates and everything are set up with the VESC and it just wont get telemetry.
```

---
## \#577 Posted by: Jamie42 Posted at: 2019-12-06T09:10:47.669Z Reads: 49

```
Did you adjust the VESC_COMMAND? To COMM_GET_UNITY_VALUES?
```

---
## \#578 Posted by: nativejibroney22 Posted at: 2019-12-07T03:34:13.166Z Reads: 45

```
Where is that located in the code?
```

---
## \#579 Posted by: nativejibroney22 Posted at: 2019-12-07T08:24:25.339Z Reads: 48

```
Nevermind, I found it and now it works perfect! Everything is straightened out with the electronics now, thank you so much for the help!
```

---
## \#580 Posted by: hanyelkomy Posted at: 2019-12-18T15:48:41.567Z Reads: 38

```
Hi There, Can anyone tell me where is the #Define FAKE_UART line, i cant seem to find it (assuming its in the receiver.cpp)

Thanks
```

---
## \#581 Posted by: hanyelkomy Posted at: 2019-12-18T16:30:40.538Z Reads: 38

```
never mind, i found it in global.h
```

---
## \#582 Posted by: luckyjacky Posted at: 2019-12-19T04:18:13.674Z Reads: 38

```
Hello, is there any chance to use this with hobbywing ESC?
```

---
## \#583 Posted by: Jamie42 Posted at: 2019-12-19T18:01:00.054Z Reads: 34

```
You need a VESC based controller for this.
```

---
## \#584 Posted by: nativejibroney22 Posted at: 2019-12-20T01:41:59.557Z Reads: 36

```
@DroidSector Is there anyway to put it into a mode "Current with reverse"? I always feel like the brake doesn't hold the board still and not enough force on hills or at an almost stop. I would like if the board had a reverse function as well.
```

---
## \#585 Posted by: Jamie42 Posted at: 2019-12-20T18:48:28.515Z Reads: 32

```
Think the Ackmaniac software could work. But could be for ppm only.
```

---
## \#586 Posted by: nativejibroney22 Posted at: 2019-12-22T14:38:22.274Z Reads: 35

```
Sigh, a new issue came up.

I had the reciever firmware programmed to one of the heltec boards and it was running fine. the 3.3v wire pulled loose and I accidentally wired it to the ground. It obviously did not work and I realized my mistake, rewired it, and now it will not work at all. The board won't run the firmware and I cannot upload new firware as I get the "failed to connect to esp32" error now. The board connects to my computer and is shown on COM5, the orange light will come on but it still won't load the firmware. I tried the capacitor trick, tried to hit the prg button, but still nothing changes.
```

---
## \#587 Posted by: Jamie42 Posted at: 2019-12-22T21:11:07.969Z Reads: 33

```
Sound like its broken. I'm not a specialist in electronics though so not sure.
```

---
## \#588 Posted by: nativejibroney22 Posted at: 2019-12-29T12:15:14.821Z Reads: 30

```
Replaced the heltec board and now on this new one everything works till I comment out the fake uart, then the remote and receiver won't connect. They do if I have fake uart, but as soon as I get rid of it it wont anymore.
```

---
## \#589 Posted by: Jamie42 Posted at: 2019-12-30T23:44:38.902Z Reads: 29

```
Hmm, tried my version? You shouldn't need FAke_UART on that one. Instead the receiver is in pairing mode the first two seconds after startup. So you make sure your remote is in pairing and power the board.
```

---
## \#590 Posted by: nativejibroney22 Posted at: 2020-01-02T19:35:11.914Z Reads: 29

```
Ok, so running your code I am getting the same results. The remote and receiver will not connect when FAKE_UART is commented out. I get Uart data fine from the board to the receiver. If FAKE_UART is in the code then I can't get my board data but the remote connects to it. I'm not sure what it means but when the remote is in pairing you can push the power button and it maybe flips through modes? But whichever one is when it doesn't display the battery percent, when it's on that the white LED on the receiver will flicker and then go solid if I go to the other mode. Still won't pair though.
```

---
## \#591 Posted by: Jamie42 Posted at: 2020-01-02T22:55:41.107Z Reads: 30

```
You downloaded the wrong branch I think. My version should be locked on pairing (remote) when it's not paired to a board.

You need the development branch:
https://github.com/Jamie4224/FireFly-Nano-Remote/tree/development?files=1
```

---
## \#592 Posted by: nativejibroney22 Posted at: 2020-01-03T17:31:59.259Z Reads: 30

```
I dont think it will let me download that specific branch. Atom needs the git link to end in .git and the only one that will pull that up is https://github.com/Jamie4224/FireFly-Nano-Remote.git
Not sure how to clone just the branch.
```

---
## \#593 Posted by: Jamie42 Posted at: 2020-01-03T20:27:37.807Z Reads: 29

```
Just download it directly from github (download zip) and open the folder in atom.
```

---
## \#594 Posted by: nativejibroney22 Posted at: 2020-01-04T02:33:39.328Z Reads: 29

```
The link you sent doesn't have the option to download it. And if I go to the repositories main page and then click on the branch it will just download the master branch and will only give me the git repository link to the master branch. I have no way of just downloading the development branch :![nogitdownload|690x387](upload://wv7ZFj0xWddSzv61umBEdip4hNU.jpeg) /
```

---
## \#595 Posted by: Jamie42 Posted at: 2020-01-04T09:30:37.171Z Reads: 29

```
Here you go:
https://github.com/Jamie4224/FireFly-Nano-Remote/archive/development.zip
```

---
## \#596 Posted by: nativejibroney22 Posted at: 2020-01-04T20:42:33.982Z Reads: 30

```
@Jamie42 you have been the biggest lifesaver! Thank you for being the guardian angel of this thread! Haha
```

---
## \#597 Posted by: Jamie42 Posted at: 2020-01-04T22:56:00.397Z Reads: 31

```
Got it working now?

Note that this version differs a bit from DroidSectors one. You can, for instance, add multiple receivers. It also has a modified menu. New features will be coming soon.
```

---
## \#598 Posted by: matiller Posted at: 2020-01-31T17:09:35.598Z Reads: 19

```
If I am right this was implemented in earlier version and wasn´t working really great. When I started breaking there was a moment it came from breaking to reverse and this kicked me really hard.
```

---
