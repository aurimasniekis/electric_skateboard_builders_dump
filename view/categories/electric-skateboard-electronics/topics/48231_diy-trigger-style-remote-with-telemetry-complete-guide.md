# DIY Trigger Style Remote with Telemetry - Complete Guide

### Replies: 430 Views: 22281

## \#1 Posted by: ervinelin Posted at: 2018-03-05T17:07:16.955Z Reads: 1410

```
![Transmitter_DM_Switch|281x500](upload://ihiSlzmTNtTiTQVQ405JwGelgWd.jpg)![Transmitter_1|281x500](upload://bG1JZTIVIvKssq4hulE0RFCZ5A0.jpg)

First off, hats off to SolidGeek's DIY remote thread (https://www.electric-skateboard.builders/t/simple-3d-printed-nrf-remote-arduino-controlled/28543 & https://github.com/SolidGeek/nRF24-Esk8-Remote) from which this is based off. I decided to start another thread so as not to dilute his original version of the remote.

------------------------------------------

If you build your own electric skateboards, you'll know that the current off the shelf remotes are not exactly ideal. Most do not have telemetry data, others are rather expensive for what they are and of course for some reason a lot of them are thumbwheel driven which I personally don't like.

In my search for my own personal remote, I've bought, hacked and built several variations including the very popular GT2B mod, the mini remote and I finally stumbled upon SolidGeek's Simple 3D-printed NRF remote. I built that as well but really didn't like the thumbwheel.

I ended up hacking a mini remote to hold the electronics in SolidGeek's design but it required extreme creativity in dremeling out the necessary cavity for the new electronics.

![Hacked_MiniRemote_1|281x500](upload://8LY1NgIvVS5E8CND0ZAOcCkNWnn.jpg)![Hacked_MiniRemote_2|281x500](upload://AspJ6qIzrTSzq8hAsdIYaE7wEM0.jpg)

I also really hated the fact that there are a million and one wires to individually solder between all the various components. Thus I began my journey to build my own based on SolidGeek's initial schematic with a goal of sharing it with the esk8 community. 

The idea was simple, design an a easy to build, decent sized trigger style ambidextrous remote with telemetry and a deadman's switch as a safety feature. The last point was made painfully clear to me after my finger got caught in the gears when I accidentally bumped the trigger in my old remote.

The remote I designed has the following features:

* A dead man's switch which deactivates the throttle when the remote is not held (safety feature because the trigger can accidentally go off otherwise, ask me how I know)
* A mode switch which swaps between displayed data (Speed, distance, battery voltage, Ah drawn, current draw)
* Ergonomic OLED display position so you don't need to twist your wrist to read it.
* Menu to adjust settings
* Programmable deck selection via menu
* Calibration of throttle via menu
* Ambidextrous design, swap to left hand use by adjusting the script-
* Skate bearing used in trigger mechanism for smoother operation as well just a fun detail considering it's meant for an esk8
* Hall sensor instead of potentiometer to prevent potential wear of a pot

To do this, I started designing my own custom PCB to hold the electronics (https://easyeda.com/ervinelin/New_Project-35f7bf3537744cda8e1064904f6a78a5), which is a completely new adventure for me. I made some minor mistakes along the way but I am glad it worked out. The latest versions have corrected these mistakes.

![Schematic|690x347](upload://lUztI8os5yzU0Aj5bKY3KkA82lu.jpg)
![PCB_Soldered|690x388](upload://hoR0UgOrMz6Hjd2Vs0CL6jGXrpn.jpg)

I also took weeks to refine the remote design starting from paper sketches, to iteration after iteration of the 3D model, test fitting, re-modelling, re-printing and more testing to get to the final design (which still could do with more refinements).

![InitialSketch|281x500](upload://qhIzw60xfCZ1Y5jsEPmC00XcH4B.jpg)![PaperPrint|281x500](upload://xQlTyukIacxgBuIbBroLCFec0IV.jpg)
![DIY_Remote_Massing|649x499](upload://oObGsKWdQgZrkYtDT4pY08cILkv.JPG)

The trigger mechanism uses hall sensor instead of a potentiometer as well as a skate bearing to ensure a smooth operation (as well as to pay homage to the fact that it's a skateboard). Again refinements were made to the position of the magnets as well as the size of the magnets. 

![IMG20180202222940|690x388](upload://wpYfRdUJGk17B9gQZnHz5gSqc6T.jpg)

The receiver itself is also relatively easy to build and is very small.
![Rx_2|281x500](upload://pE2f4S1w5bLncQlzVbh9qoW1Xzv.jpg)

The eventual remote works as I had intended, telemetry, deadman's switch, deck selection, mode button and work.

![Deck_Select|281x500](upload://cRCTNHRmz178EC8pjQVKix8oAHQ.jpg)![Transmitter_2|281x500](upload://pwXCsQzi9X6t1cO2CvLinGvCxkH.jpg)

It's also slim enough to easily fit into pockets or bags.

![Rx_inBag|281x500](upload://1Us0oW5VbjFL3zrYtq4x3QOygh5.jpg)

Overall I'm very happy with the end results, it's a fair bit of work with many parts to order but I hope this repository helps you build your own!

![DIY_Kit_1|690x388](upload://hEalwT16nYs22WbkYQQBr3neXsZ.jpg)


------------------------------------------


STLs available at https://www.thingiverse.com/thing:2800544

Youtube video available at https://www.youtube.com/watch?v=gQl7mLMAiAs&feature=youtu.be

Part List available at https://docs.google.com/spreadsheets/d/1vXR9ce0m25Ap6XxzlymFo_pfpIeT2RAqWCypW-a-Jes/edit?usp=sharing

PCB Files available at https://easyeda.com/ervinelin/New_Project-35f7bf3537744cda8e1064904f6a78a5

Firmware available at https://github.com/ModMiniMan/nRF24-Esk8-Remote

Build guide available at https://github.com/ModMiniMan/nRF24-Esk8-Remote/wiki


------------------------------------------


You will need to have intermediate soldering skills to complete the build as well as knowledge on how to program an Arduino and adjust simple code. Of course if you print this yourself you will need to know how to 3D print.


**Caveats:**
**Remote is experimental and not an off the shelf product that has undergone proper testing. Build and use at your own risk. Please bench test extensively before actual use. Lastly, I highly recommend protective gear when using the remote just in case something doesn't work (many many things can go wrong)**
```

---
## \#2 Posted by: Der6FingerJo Posted at: 2018-03-05T17:33:56.400Z Reads: 1022

```
I love it!
Would have definitely done this if it was around when i built my GT2B Sparkle Mod Arduino Oled thingy!
Looks really clean and i especially like the addition of the dead man switch where it is. 
Hope to see a lot of them on here since people now can't complain that there isn't a trigger remote with all the functions :smile:
```

---
## \#3 Posted by: Zyb Posted at: 2018-03-05T18:33:30.815Z Reads: 990

```
love the trigger style design, its on my to do list after i finish my board! good work
```

---
## \#4 Posted by: chocol4te Posted at: 2018-03-05T18:48:24.600Z Reads: 972

```
I'm starting work on a STM32F103-based version, using the 433MHz nRF modules. Obviously, it won't have any real-world difference, but I thought encryption and integrity for telemetry and control would be cool :)
```

---
## \#5 Posted by: ervinelin Posted at: 2018-03-06T06:47:32.467Z Reads: 908

```
@Der6FingerJo - The G2TB Sparkle case mod was such a pain to do honestly, I still have mine but the lack of a safety mechanism makes me not want to use it.

@Zyb - Great! Let me now if you run into problems

@chocol4te -  What difference is the STM32F103? It LOOKS very much similar to my Ardunio Nano V3.
```

---
## \#6 Posted by: chocol4te Posted at: 2018-03-06T07:11:57.478Z Reads: 823

```
@ervinelin  The STM32F103 is a 32 bit ARM micro controller. Essentially it boils down to having much more processing power than the Arduino Nano's ATmega 328P, running at nearly 5x the clock speed, and being much better at floating point math.
```

---
## \#7 Posted by: ervinelin Posted at: 2018-03-06T10:03:39.834Z Reads: 788

```
Hm.... I wonder what difference will it make. I don't think the code is doing any crazy maths.
```

---
## \#8 Posted by: Okami Posted at: 2018-03-06T10:25:14.905Z Reads: 792

```
Cool remote. Too bad telemetry is available only for vescs, as of now. 

I like the design. I hope u manage to assemble and offer for sale at least a few units. 

Not saying i would be the buyer but i think it would instill confidence and remove the hassle of ordering parts and assembling everything.

 At least this looks like next logical step to me but depends how much time u have got for that.

Nice work non the less. Maybe more accent could be put on what battery it uses but im sure it is in the part list.
```

---
## \#9 Posted by: ervinelin Posted at: 2018-03-06T10:35:37.573Z Reads: 761

```
It takes too much time for me to assemble one for it to make monetary sense (also I don't think I can ship the lipo inside the remote either). I have sold some kits to a couple of friends of mine who expressed interest.

As for the battery, yes it's in the parts list. I use a 18350 battery, there is also an STL without the 18350 holder that you can use any generic 1S battery that will fit.
```

---
## \#10 Posted by: ElskerShadow Posted at: 2018-03-06T11:15:38.472Z Reads: 720

```
[quote="ervinelin, post:1, topic:48231"]
ask me how I know)
[/quote]
Well.... how do you know ?
```

---
## \#11 Posted by: banjaxxed Posted at: 2018-03-06T11:18:16.945Z Reads: 701

```
Thank you so much for this guide

I prefer a thumb throttle/brake but the guide is wonderfully put together so very useable for someone following the original conception from a schematic-instructional perspective...where it was lacking tbh again thank you
```

---
## \#12 Posted by: chocol4te Posted at: 2018-03-06T11:52:20.710Z Reads: 669

```
Oh it won’t make the slightest difference for the current codebase, I was planning on developing a fork with encryption, and error checking/correction which would require a more powerful MCU.
```

---
## \#13 Posted by: Scoo_B_SK8 Posted at: 2018-03-06T12:15:00.336Z Reads: 652

```
@ervinelin Been watching your introduction, glad to see its got its own spot now.  I agree with @banjaxxed, very well thought out and complete instructions.

Cheers!
```

---
## \#14 Posted by: ervinelin Posted at: 2018-03-06T13:30:47.446Z Reads: 646

```
@ElskerShadow I was checking the belt tension when I accidentally hit the throttle, finger got caught in the gears. Months later it still hurts.

@chocol4te that'll be cool if you can somehow get the connection more secure. Do share what you come up with!

@banjaxxed some friends of mine also prefer thumbwheels and asked if I can design one. Quite frankly this trigger remote took up so much of my time that I rather be skating.. if it's a thumbwheel you want solidgeeks version works as well.

Glad you guys like the build guide... Hopefully someone can improve on this version.
```

---
## \#15 Posted by: Deckoz Posted at: 2018-03-06T19:14:11.540Z Reads: 612

```
This is pretty nice.

In a bit out of touch with solidgeeks  repo... But does it work with ack 3.100 firmware?
```

---
## \#16 Posted by: ervinelin Posted at: 2018-03-06T22:57:55.281Z Reads: 597

```
Hm.. I am not sure what ack firmware is. You can just use mine as it is modified specific for my remote.
```

---
## \#17 Posted by: Deckoz Posted at: 2018-03-06T23:04:13.964Z Reads: 591

```
Ackmaniac Extended ESC Tool... I figured your "firmware" was for the remote's Arduino. I'm speaking of the VESC firmwares
```

---
## \#18 Posted by: ervinelin Posted at: 2018-03-06T23:49:48.844Z Reads: 607

```
Ah! I never tried that actually.

You'll need to make sure it will work with RollingGeckos VESC UartControl first. If that is possible then shouldn't be an issue.
```

---
## \#19 Posted by: pennyboard Posted at: 2018-03-07T17:24:56.411Z Reads: 593

```
If you have to estimate an approximate cost for components for this remote, assuming minimal mistakes so you don't have to keep re-buying parts, what would you guess it to be?
```

---
## \#20 Posted by: ervinelin Posted at: 2018-03-08T00:49:54.393Z Reads: 602

```
@pennyboard the cost is tabled in the parts list. 

The problem is many items require you to buy them in sets. Eg. You need 2 switches. It comes as 20.

Mostly this is okay but I just found out my PCB cost doubled after EasyEda made some changes... So that's pretty irritating. I am asking them why this is so.
```

---
## \#21 Posted by: Eboosted Posted at: 2018-03-08T03:39:40.032Z Reads: 537

```
Your solution is brilliant, thats what I've been waiting for all my life, I really love you.

Now, for a Newby on arduino and pcb building, would you please point me to the right direction on how to build the PCB? Should I just send the PCB design a company? How should I but the board and make all the traces?

Sorry if this is a stupid question
```

---
## \#22 Posted by: ervinelin Posted at: 2018-03-08T03:40:47.313Z Reads: 528

```
Just click on the link I shared and order the PCB...

I am checking with EasyEDA why the PCB prices went up in the last 2 days though.
```

---
## \#23 Posted by: Eboosted Posted at: 2018-03-08T06:12:24.256Z Reads: 533

```
I did try that and there is no button to order it, I even registered

 [quote="ervinelin, post:1, topic:48231"]
PCB Files available at https://easyeda.com/ervinelin/New_Project-35f7bf3537744cda8e1064904f6a78a5
[/quote]
```

---
## \#24 Posted by: ervinelin Posted at: 2018-03-08T06:33:18.930Z Reads: 544

```
Ah it's a little complicated.

You gotta go into the editor, then hit export gerber button at the top to order.

But it seems like there's something wrong with the system (they just did a major upgrade yesterday it seems).

I'm also getting some new DRC errors which never showed  up previously, need to go sort those out.
```

---
## \#25 Posted by: Eboosted Posted at: 2018-03-08T06:38:16.224Z Reads: 536

```
Yeah, the email address verification link isn't working either

![image|690x322](upload://wPlaJIUpGuCzA9m09Jdu69z0S3E.png)
```

---
## \#26 Posted by: Slak Posted at: 2018-03-09T20:52:39.150Z Reads: 511

```
I like your style, dude ! ;)
```

---
## \#27 Posted by: junwoo091400 Posted at: 2018-03-10T05:49:24.880Z Reads: 508

```
Thank you very much for sharing PCB design!

I will try to make all-in-one PCB for transmitter, not a Stacked-design.

+ Use nRF24l01 modules with 2x4 pin-Header.
```

---
## \#28 Posted by: junwoo091400 Posted at: 2018-03-10T07:26:23.541Z Reads: 492

```
Hmmmm

While designing the PCB I discovered that '5V Boost' converter's PCB Layout doesn't match the Product you linked in google datasheet.

Your PCB and module(presumably, since it didn't let out magic smoke) has both Input Terminal on 'Long-Side' of the rectangle. But the product in link(alibaba) has both Input Terminal on 'Short-Side' of the rectangle.

If anyone buys your pcb + linked boost board, they can short the Battery, because your PCB gives GND and VBAT to 'long-side', but linked-product has IN- and OUT- on 'long-side', ouch!

Even worse since your TP4056 doesn't have dedicated Output-Port. So short-circuit detection isn't possible. That can be extremely Dangerous.

So can you provide link to the same boost-converter you used? Thanks.
```

---
## \#29 Posted by: ervinelin Posted at: 2018-03-10T09:37:58.626Z Reads: 455

```
You are right, in this case it's a matter of the photo on the link not being the same as the product sent to me. You see one thing online, it comes as something else in the mail.

Let me try to find a better link with the correct photo.
```

---
## \#30 Posted by: junwoo091400 Posted at: 2018-03-10T10:29:34.218Z Reads: 472

```
This one (https://ko.aliexpress.com/item/DC-DC-Boost-Power-Supply-Module-Converter-Booster-Step-Up-Circuit-Board-3V-to-5V-1A/32788045286.html?spm=a2g12.10010108.1000014.9.69182faeKDqNio&traffic_analysisId=recommend_3035_null_null_null&scm=1007.13338.98466.000000000000000&pvid=4425630d-8821-4e7f-a11a-b51420c58086&tpp=1) seems like the boost module you used. As you said, can't be sure if product and Photo will match, but at least photo is much more similar, including pinout.

Btw, did you measure the distances between pad & added new pcb-lib for Boost module Footprint?
```

---
## \#31 Posted by: junwoo091400 Posted at: 2018-03-10T11:03:07.562Z Reads: 493

```
![image|309x500](upload://gATzoay0O52EIjuClSfQEmUGLXk.png)

I have a feeling that this Won't fit inside original solidgeek's remote. Due to it's width, and also length is pretty tight too(I've forked your Schematic & PCB, and modified quite a bit).

Solidgeek's freeSpace : 26(L) x 63(H) / ArduinoNano: 18 x 44 / TP4056 : 17 x 22/ Boost : 15 x 19
```

---
## \#32 Posted by: cnd Posted at: 2018-03-10T14:02:09.377Z Reads: 437

```
You are SO awesome!!  I've been trying to work out how to build a 100% waterproof (underwater - not for a skateboard:-) throttle and had no idea how to use hall sensors for that... before now!!!
```

---
## \#33 Posted by: Ghettobird117 Posted at: 2018-03-13T01:11:44.293Z Reads: 440

```
@ervinelin got any complete kits together?
Im pretty keen to get started on a side ardino project, but dont have the time to wait 49 days for Aliexpress to ship out
```

---
## \#34 Posted by: ervinelin Posted at: 2018-03-13T04:36:16.376Z Reads: 437

```
Incomplete kits... Simply because of what you said.. some items take more than a month to reach me... 

Sorry a bit caught up with the flu and work, need some time to get things sorted.
```

---
## \#35 Posted by: Ghettobird117 Posted at: 2018-03-13T09:52:08.147Z Reads: 430

```
If I may ask, what bits are you missing?
Or am I better off waiting for a full kit if you are going to sell them?
```

---
## \#36 Posted by: ervinelin Posted at: 2018-03-13T10:33:13.487Z Reads: 442

```
Magnets and springs take an eternity to reach me. More than a month still nothing.

Some other parts here and there I need to check, also my PCB i have in stock is the older design. EasyEDA doubled their prices so I am very hesitant to order more of which I don't need any.
```

---
## \#37 Posted by: ervinelin Posted at: 2018-03-15T03:42:26.996Z Reads: 487

```
Okay, I've run into some problems. I won't sell any kits until I find good solid solutions for them.

1. I had instances of my board losing power going very slowly uphill, at first I thought maybe it was a amp draw issue but I noticed last night that for some weird reason, the remote disconnects when I go very slowly uphill (going fast is not an issue). So as it stalls along the way up, the remote disconnects and I lose all control until a few seconds later when it comes back.

Honestly I have absolutely no idea what is going on with this. Anyone?

2. After that episode, thinking that I need more shielding, I opened up the transmitter only to have my stupidity fry the lipo charger. So I desoldered and replaced the entire lower PCB and its components and now my transmitter won't fire up without a hard reset or flipping the switch quickly between on and off and back on. 

https://youtu.be/FtXSKLNl2PM

Again, totally confused why this is happening. USB power works fine. Current possible solution is to add a cap between the reset and GND pins.

Anyone Arduino masters can clue me in on what's happening?
```

---
## \#38 Posted by: Zyb Posted at: 2018-03-15T07:37:54.407Z Reads: 471

```
I have exactly the same thing on my receiver side, it’s a weird problem. Luckily I’m powering my remote from usb socket so no problem there. Did you try the possible capacitor solution yet?
```

---
## \#39 Posted by: Cncninja Posted at: 2018-03-15T17:29:06.727Z Reads: 477

```
The hill climb drop out is just due to voltage sag issues on the rx side under load. In the rc world, we call them brownouts. the fix is a capacitor to help stabilize voltage on the 5v rx input. ![image|673x264](upload://wfdaoQZ5dgzez1oxPNWMOLLAVSi.jpg)
```

---
## \#40 Posted by: Cncninja Posted at: 2018-03-15T17:34:42.757Z Reads: 463

```
For the second issue, i think its a step up voltage reg issue. i.e you flip the switch and the step up reg ramps to the full 5v and the Arduino is under voltage on boot. but a quick reset the reg is already up to 5v (caps charged) so the audio boots correct. if you have a O-scope you can check this.
```

---
## \#41 Posted by: ervinelin Posted at: 2018-03-16T01:25:26.242Z Reads: 440

```
HMMMmmmm... yes I know of brownouts in RC.

Okay I will try adding a huge cap on the 5V and see what happens. There is already an LC filter but I think that just smooths the noise rather than store voltage for brownouts.

As for the second issue, I was considering swapping to a pololu setup (previous DIY remote used it without any issues), but that means I need to re-do the PCB and desolder the two halves. Another friend of mine suggested that the arduino might be going into bootloader mode for some reason on startup.

I haven't tried the cap on reset pin trick yet, will report back when I have done so.
```

---
## \#42 Posted by: Deckoz Posted at: 2018-03-16T03:23:34.680Z Reads: 431

```
If your having issues on the receiver side with 5v line coming from the vesc... Then your drv is probably about to die as the DRV is the output of the 5v buck.
```

---
## \#43 Posted by: ervinelin Posted at: 2018-03-16T13:58:13.545Z Reads: 444

```
![IMG20180316215112|690x388](upload://jnrBtO7H5EwXvXuj3X71Rjy2de0.jpg)

So a 10v 100uF cap between reset and ground pins did the trick of needing a hard reset to boot.

Now to fix the brownout issue....
```

---
## \#44 Posted by: ervinelin Posted at: 2018-03-16T16:19:57.400Z Reads: 428

```
IT WORKED!!!

I added a 1000uF cap to the output of the LC filter and it was smooth sailing from there for a test 15km ride I just did. Even managed to start on a slope without any issues.

YAY! All issues resolved!! (For now)

One more thing to note, I realised it's not enough to just wrap the NRF module in copper tape, I needed to tape the entire bottom PCB covering the NRF module. Again no idea why this is required but it made the difference between no connection and a solid connection...
```

---
## \#45 Posted by: Zyb Posted at: 2018-03-16T16:53:48.947Z Reads: 408

```
im glad the issue was resolved. did you put the cap after LC filter? 
to be clear 5v-- LC-- cap--arduino?
```

---
## \#46 Posted by: ervinelin Posted at: 2018-03-16T16:57:48.135Z Reads: 401

```
Yes cap after LC filter
```

---
## \#47 Posted by: Zyb Posted at: 2018-03-16T18:01:24.665Z Reads: 399

```
going to try it on receiver side but need a cap first :slight_smile:
```

---
## \#48 Posted by: Cncninja Posted at: 2018-03-16T18:05:51.980Z Reads: 406

```
Awsome, now i need to build one i have everthing but the dang hall sensor... not finding them on a fast shiping option only slow boat option 60 days etc does anyone know if a difrent p/n will work?
```

---
## \#49 Posted by: Zyb Posted at: 2018-03-16T20:15:56.283Z Reads: 398

```
Ordered PCBs from easyEDA, used DHL express all was 13 euros in total shipping to EU
```

---
## \#50 Posted by: ervinelin Posted at: 2018-03-16T22:44:15.712Z Reads: 392

```
Oh? How is it so cheap?
```

---
## \#51 Posted by: ervinelin Posted at: 2018-03-16T22:45:02.643Z Reads: 377

```
I think any 5v hall sensor will work. You can try other options other than aliexpress
```

---
## \#52 Posted by: Zyb Posted at: 2018-03-16T22:54:44.742Z Reads: 380

```
i have no idea is it supposed to be more expensive? they are using jlcpcb.com for the orders and thats the price for 5 each total of 15 pcbs.
```

---
## \#53 Posted by: ervinelin Posted at: 2018-03-17T01:16:29.252Z Reads: 375

```
Last time I checked the price ballooned after they upgraded their website. Maybe they corrected it.
```

---
## \#54 Posted by: Zyb Posted at: 2018-03-17T13:14:19.596Z Reads: 406

```
[quote="ervinelin, post:44, topic:48231"]
I added a 1000uF cap
[/quote]

is it possible to place that 1000uF cap on the pcb where marked with 220uF ? 
![661cd9e2-9b95-4502-b298-bbd4297c4484_1_0_1|172x500](upload://pziDYhLE4M6J84OQkGL7ZHt1GwV.png)
```

---
## \#55 Posted by: ervinelin Posted at: 2018-03-18T00:17:39.866Z Reads: 378

```
Yes just that the 1000uF will stick out like a sore thumb
```

---
## \#56 Posted by: ervinelin Posted at: 2018-03-18T12:28:11.122Z Reads: 419

```
![IMG20180318174848|281x500](upload://dR3nJWxcMaRDRpXJWxalPS2q5dI.jpg)

I found a way to use removable pins to stack the two PCBs! Now it will be easier to repair the board should the need arise!

![IMG20180318174202|690x388](upload://w3k18IeD9ifJe6O8mvBLQ9bDh38.jpg)
To make this fit I had to do without the plastic on the header pins of the Arduino and solder it directly onto the pcb.

![IMG20180318175010|690x388](upload://dmDBuwSLVR19rrBU14lGL3bRM9p.jpg)
![IMG20180318175508|690x388](upload://94SZw6yq6RYws9vMbxMWuVqBtxO.jpg)
On the bottom PCB i found that I had to shield the entire bottom for some weird reason. This includes sheilding the nrf module with copper tape first. I then use blenderm tape and copper tape to cover the entire bottom leaving the antenna exposed of course. 

![IMG20180318170124|281x500](upload://ftEyiUNEm2zVKOpLBygt3gUl3hm.jpg)
![IMG20180318170130|281x500](upload://vsrn1dugdjRrBGvrkCTdAqKOo34.jpg)
Another modification I made was to replace the resistor on the lipo charger with a 2.2k resistor to lower the charge amp. The lipo can take the charge at 1A but it gets a bit too warm for comfort.
```

---
## \#57 Posted by: ervinelin Posted at: 2018-03-19T17:43:15.202Z Reads: 405

```
Built another remote just to see how long it takes me to do up one now that I know what I am doing. Still took me 2 long nights including all the electronics as well as sanding, spray painting.

The buttons are a real bother to install, need to bend the limit switch flap just right to get it to activate correctly.

Also didn't realise the AliExpress shop sent a different coloured oled... I prefer the white actually.

![IMG20180320012827|666x500](upload://oadECO5tgyyq4LRfWnXuNgDPk4T.jpg)
```

---
## \#58 Posted by: Cncninja Posted at: 2018-03-19T23:36:06.276Z Reads: 400

```
Lets cnc some cases, i have a Haas 4 axis cnc mill we can make some out of HDPE? for a production
```

---
## \#59 Posted by: Nandox7 Posted at: 2018-03-19T23:46:43.042Z Reads: 394

```
Did anyone looked into mod the parts so that there is only one USB port to power/charge the battery and to program the arduino?
```

---
## \#60 Posted by: ervinelin Posted at: 2018-03-19T23:49:08.910Z Reads: 392

```
Yes you can jumper some wires to the USB charge port. Someone did it in solidgeeks remote.

Although I wouldn't bother as adjusting and uploading the code is a rare occurrence unless you are busy dabbling with it like I have been.
```

---
## \#61 Posted by: ervinelin Posted at: 2018-03-20T01:53:04.551Z Reads: 386

```
So I am trying to figure out how to get better range and reliability off the connection. Right now it works, but it's effective range is like 2-3m (good enough when you stand on the board but I would much prefer it to be like 100m to be safe).

After some quick googling (https://hackaday.com/2016/05/31/fixing-the-terrible-range-of-your-cheap-nrf24l01-palna-module/ & https://blog.blackoise.de/2016/02/fixing-your-cheap-nrf24l01-palna-module/), it seems like the main culprits for poor range are:

1. Switching DC-DC 5V step up converter spewing noise (I suspect that's why I need to shield the bottom of the PCB, but I'm not 100% sure)
2. Noisy 3.3V step down converter onboard the arduino that powers the NRF.

Of note some of the comments include:

"Similarly for the PA/LNA ones, we use 47uF tantulum that can be lowered to 22uF as well if it is on its own dedicated 3.3v linear supply rail."

"One thing we do NOT do as this has never worked in production: use a switcher supply nearby or to feed power to these clones."

So essentially a linear supply or at least a cleaned up 3.3V is essential.

I'll try adding a cap to the 3.3V arduino output feeding the NRF to see how that works out.
```

---
## \#62 Posted by: Nandox7 Posted at: 2018-03-20T20:00:46.875Z Reads: 357

```
Interesting, hope to get the new OLED's tomorrow so I'll be able to give this another try.
Mya pick he spektrum analyzer and see if any of the parts is making noise on the 2.4Ghz band.
```

---
## \#63 Posted by: ervinelin Posted at: 2018-03-20T23:09:47.759Z Reads: 371

```
Some updates:

Adding a 100uF cap to the 3.3v output on the Arduino seems to make things worse not better.

Trying to force it to channel 108 didn't work at all, wouldn't connect.

Dropping the transmission speed down to 250kbs seemed to make the most improvement. Range increased from maybe 2m to 5m or so when in direct line of sight.

Lastly, adding a cap to the reset and ground pins solved the booting up problem but prevents a new sketch from being uploaded. Had to desolder the cap to upload a new sketch.
```

---
## \#64 Posted by: Twinsen Posted at: 2018-03-21T23:28:47.488Z Reads: 358

```
I always thought the PA+LNA modules look sketchy but they seem to just be crazy sensitive in your case.
I use a module without the PA and while I don't have power problems it's range is pretty small for my comfort.

I'm actually considering on switching to the ESP32 or ESP8266. With ESP32 you get a Dual Core 32 bit processor+wifi+adc+dac+plenty of io for 4$
I made a project with ESP8266 and they have been rock solid for more than a year now.
```

---
## \#65 Posted by: ervinelin Posted at: 2018-03-22T11:09:38.823Z Reads: 343

```
Used a suggested 47uF tantalum cap on the 3.3V supply to the NRF module.

Made no noticable difference...
```

---
## \#66 Posted by: ervinelin Posted at: 2018-03-22T11:09:56.394Z Reads: 348

```
Would love to see someone try with more reliable electronics
```

---
## \#67 Posted by: Zyb Posted at: 2018-03-22T11:23:19.815Z Reads: 365

```
Shipping was so quick, from ordering to my door it took around 5 days. 
![image|375x500](upload://qoKQICrci3UIo5bWyWdSluGcH9H.jpg)
```

---
## \#68 Posted by: ervinelin Posted at: 2018-03-22T13:16:35.317Z Reads: 350

```
That's super fast considering they had to manufacture the boards!

Did you manage to buy all the parts yet?
```

---
## \#69 Posted by: Zyb Posted at: 2018-03-22T14:18:57.498Z Reads: 351

```
i have some extra springs, micro switches, arduinos, dc dc booster, magnets, tp4056 board from earlier build and ordered what im missing from aliexpress im afraid they gonna take a while :smiley: i dont want to salvage my current remote as it is working just fine also need different battery and switches in order to complete your version so theres no point. 
just one question tho, is it not possible to use 5x5 magnets? what was the reason for switching to 5x8mm ones?
```

---
## \#70 Posted by: ervinelin Posted at: 2018-03-22T15:15:01.784Z Reads: 346

```
You can try with the 5mm ones first, mine were not strong enough so there was a lot of deadzone around the center. Swapping to 5mm stacked with 3mm worked for me.

Some retailers on AliExpress are terrible.. 1.5 months after I ordered the magnets then they shipped. The springs just never came....
```

---
## \#71 Posted by: Zyb Posted at: 2018-03-22T15:45:02.148Z Reads: 332

```
yea some orders take really long time, so annoying but cant complain price is really cheap. i just dont understand how this pcb shipping cost is so cheap. DHL is expensive but they charged me only 3 dollars for express shipping service :D
```

---
## \#72 Posted by: ervinelin Posted at: 2018-03-22T18:27:03.422Z Reads: 334

```
First order gets $10 off shipping I think
```

---
## \#73 Posted by: ervinelin Posted at: 2018-03-23T10:48:04.282Z Reads: 356

```
I ordered some NRF modules that have a uFL connector so that I can add a 2.4GHz antenna to it to try to increase the range... Will report back when I have the results..

https://www.aliexpress.com/item/Sale-price-holyiot-smd-nRF24l01-PA-LNA-wireless-module-nRF24L01-ipx-antenna-long-distance-transmission/32791996740.html?spm=a2g0s.9042311.0.0.WhZhyb

https://www.aliexpress.com/item/1PC-New-Arrival-100mW-AS01-SPIPX-nRF24L01-wireless-pa-lna-2-4g-wifi-module-Wireless-Transmission/32819372747.html?spm=a2g0s.9042311.0.0.WhZhyb

One other update...

So I built 2 remotes, and even though they are identical in theory, the sensitivity around the center is different. I suspect this is down to the slight differences in the strength of the magnets used... Not sure how best to get around this problem.
```

---
## \#74 Posted by: Twinsen Posted at: 2018-03-24T23:40:29.176Z Reads: 378

```
I returned from a trip with my version of the remote.
I went 22km+27km with no problems at all, no disconnections and no drops through both trips. The receiver was placed in the middle of two ESCs, but my ESC uses a linear regulator that delivers super clean 5V. The antennas were also pointing towards each-other.

I use just a simple NRF24L01+ without the PA. It seems to be enough range for this purpose and without all the power problems. I can only make it disconnect if I cover the remote with both my hands and my body, and hold it at weird angles.

About my remote:
I remixed ervinelin's remote with custom changes in the model, schematic and code. I'm still actively working on the code, but if anyone is interested here's the info:

Preliminary parts list:
[https://docs.google.com/spreadsheets/d/1Ayte5Xm0up_AQHfdTZghDGnGC5o7WZZo4H4hzZ2LCAw/edit?usp=sharing](https://docs.google.com/spreadsheets/d/1Ayte5Xm0up_AQHfdTZghDGnGC5o7WZZo4H4hzZ2LCAw/edit?usp=sharing)
Work in progress code(see page for feature details):
[https://github.com/asafteirobert/nRF24-Esk8-Remote](https://github.com/asafteirobert/nRF24-Esk8-Remote)

For now I removed the VESC UART since I use normal car ESCs. But I implemented plenty of features and improvements.
EDIT: I posted about it here: https://www.electric-skateboard.builders/t/twinsens-3d-printed-nrf-remote/50482

![IMG_0642|666x500](upload://gyj5CHqKh8v4WqSPM1Sk3tqGt5o.JPG)![IMG_0645|666x500](upload://5sEqa7KmBXsaIOofwTowAA0uMRr.JPG)![IMG_0650|666x500](upload://iepzeunpADze2cm9dgHjdSr4KT3.JPG)![IMG_0649|666x500](upload://zCdjcPg1f1BJmQQeWH3JIq0e6WO.JPG)

EDIT: I posted about it here: https://www.electric-skateboard.builders/t/twinsens-3d-printed-nrf-remote/50482
```

---
## \#75 Posted by: SimosMCmuffin Posted at: 2018-03-26T06:00:16.699Z Reads: 358

```
Where did you order the PCBs from?
```

---
## \#76 Posted by: Zyb Posted at: 2018-03-26T07:27:47.142Z Reads: 349

```
From jlcpcb.com
```

---
## \#77 Posted by: SimosMCmuffin Posted at: 2018-03-26T07:40:06.352Z Reads: 357

```
Gotta do a order from them in the future and they have such short production time as well.  I've been using Seeedstudio before, but sometimes the boards do take quite some time.
```

---
## \#78 Posted by: Kug3lis Posted at: 2018-03-26T07:46:38.659Z Reads: 348

```
There is also allpcb.com they deliver in 10 days to the uk.
```

---
## \#79 Posted by: Zyb Posted at: 2018-03-26T08:41:12.301Z Reads: 344

```
Well yea they are quite fast. Production for 15 boards took 2 days and 3 days on top for shipping from China to Europe. Very impressive imo.
```

---
## \#80 Posted by: Nandox7 Posted at: 2018-03-27T09:13:28.509Z Reads: 340

```
I'm new to EasyEDA and couldn't find a clear answer to this.

For the PCB's layouts above, is it possible in EasyEDA to change track width and track spacing without doing all routing back?
I'd like to give it a try and made in my CNC, but track width is a bit too small for it.
Thanks
```

---
## \#81 Posted by: ervinelin Posted at: 2018-03-27T09:14:17.977Z Reads: 319

```
If you are editing the board yes, you can change track width.
```

---
## \#82 Posted by: Nandox7 Posted at: 2018-03-27T10:14:51.259Z Reads: 325

```
But will it update automatically in the layout?
Tried to change to 0.4mm track clearance and track to track width and nothing happened.
```

---
## \#83 Posted by: ervinelin Posted at: 2018-03-27T11:33:22.657Z Reads: 330

```
I believe u need to reroute with the thicker traces
```

---
## \#84 Posted by: ervinelin Posted at: 2018-04-01T17:20:00.056Z Reads: 345

```
![IMG20180324183800|281x500](upload://h6rPemi8zL6NIL6qZeXqt9Lfg0C.jpg)

I desoldered the ceramic antenna on the Rx and replaced it with a 2.4ghz whip antenna (Frsky RC antenna). Instant range boost!

Problem is I tried doing the same on the transmitter and it just was not happy at all... Had to go back to the ceramic antenna.

Other changes I made, replaced the current DC boost with a DC boost LC filter combo. So far not sure if this helps but cleaner power is always better in my opinion.

I have also ordered sheilded NRF modules with a ufl port for a whip antenna (no more soldering like above). Hopefully this will end all problems associated with range.
```

---
## \#85 Posted by: Zyb Posted at: 2018-04-01T17:32:32.934Z Reads: 316

```
it is only range related i hope? you dont have any connection problems while riding without any modifications?
```

---
## \#86 Posted by: ervinelin Posted at: 2018-04-01T17:35:15.465Z Reads: 317

```
Quite honestly I have only had one known instance of lost connection but that's due to brownout when climbing. Since resolved with 1000uF cap on the 5v input.

And that's in my 100s of km of riding with these style of remotes.

I am just trying to make the connection even more stable and reliable without weird mods like strategic copper tape here and there.
```

---
## \#87 Posted by: Zyb Posted at: 2018-04-01T18:03:05.273Z Reads: 335

```
yes i read that post, im also going to add some low ESR 1000 cap. well practically it replaces 220uf one which is in the original design. yea whip antenna is a good idea are you going to use that module which you linked earlier? https://www.aliexpress.com/item/Sale-price-holyiot-smd-nRF24l01-PA-LNA-wireless-module-nRF24L01-ipx-antenna-long-distance-transmission/32791996740.html?spm=a2g0s.9042311.0.0.WhZhyb
im waiting for battery and new 8x5 magnets then i ll order the 3d printed parts from my friend. i hope it works out well because im used to trigger style remotes so thanks again for this design.
i tried to build this with what i had and instead of soldering the pins i modified some IC sockets to make them seperable like you recommended and it gave me around 19mm with arduino installed but i still miss nrf chip at the bottom so it going to raise it to around 22-23mm i guess. is that too tall for the internal dimensions of the case?
![image_123923953 (17)|690x337](upload://pzPtvmGmiXKEyiBYchLVntdZyXg.jpg)
```

---
## \#88 Posted by: ervinelin Posted at: 2018-04-02T03:17:51.388Z Reads: 320

```
Gotta feeling that's too tall. I had to remove the plastic holders on the pins under the Arduino board to fit.

I am putting my bet on this NRF module.. 2.4GHz nRF24L01 PA LNA Wireless rf Module Power Amplifier E01-ML01SP4 SPI SMD 2.4 ghz Radio rf Transmitter Receiver for Arduino 
 http://s.aliexpress.com/eUB7RJZv?fromSns=Copy to Clipboard

Only worry is if it will fit.
```

---
## \#89 Posted by: Zyb Posted at: 2018-04-02T18:16:36.127Z Reads: 309

```
i built the receiver and it has like 1 meter range :( my original receiver has like 15 meters of range theres wasa  wall in the middle when i tried that. same parts but one has a pcb in the middle i wonder why theres such a difference
```

---
## \#90 Posted by: webst Posted at: 2018-04-02T18:44:26.249Z Reads: 320

```
https://forum.mysensors.org/topic/1153/we-are-mostly-using-fake-nrf24l01-s-but-worse-fakes-are-emerging
```

---
## \#91 Posted by: ervinelin Posted at: 2018-04-02T22:53:04.635Z Reads: 310

```
What's the difference between the two receivers that you built?
```

---
## \#92 Posted by: Zyb Posted at: 2018-04-02T23:30:05.151Z Reads: 312

```
as you know its the same thing on the receiver side, 1 arduino and 1 nrf module. they were exactly the same except one was built using cables other one was using the pcb. the one with the cables had solid connection with a very good range. like i said there was a thick wall in between and i got at least 15 meters of range before i lost the connection but with the one i built earlier today i barely had 1 meter range and connection was constantly dropping. like webst linked i think those nrf modules are shitty. probably the one you linked with the antenna will be much better. its fairly small and it should fit to the pcb.
i almost forgot, i didnt use copper tape.
```

---
## \#93 Posted by: ervinelin Posted at: 2018-04-02T23:45:27.416Z Reads: 309

```
The cable version did you use copper tape? 

Also, both were from the same supplier?

I had a slightly similar experience although no where as dramatic. Maybe 8m vs 6m...

I also have no idea why the PCB would make such a big difference. In any case now all my NRF modules have a small cap on the 3.3v line, copper tape on the module and a modified antenna (transmitter has no antenna).
```

---
## \#94 Posted by: Zyb Posted at: 2018-04-03T00:02:43.473Z Reads: 292

```
yea same supplier, both receivers lack copper tape but i will get some and use it. i dont think its the pcb probably something went wrong or it was a really bad chip or something. sadly i dont have any other nrf modules to further test but i ll have some to feed my curiosity :slight_smile: how small is the cap on 3.3v?
```

---
## \#95 Posted by: ervinelin Posted at: 2018-04-03T00:44:35.495Z Reads: 303

```
I use a 47uF tantalum cap on the 3.3V supply to the NRF module. I originally reported that it didn't make much difference but my own unscientific observations have shown that it might.

Most noticable differences have been dropping the transmission rate to 250kbps via the code and adding the antenna.

What I find most curious is that my very first hacked up remote with a rats nest of wires never had any of these problems!
```

---
## \#96 Posted by: Zyb Posted at: 2018-04-03T17:06:44.859Z Reads: 315

```
i did try couple of things today like adding a cap to 3.3v line, shielding the nrf module, modifying the antenna, touch up on solder joints etc etc. non of it seemed to work. the longest stable connection lasted for 30 seconds from 1 meter range its just terribly unreliable. i read alot of things about these shitty nRF24L01+ PA LNA modules. most of them have strange problems as well, its kinda up to your luck if you get a proper working one. so im getting another nRF24L01+ PA LNA model with antenna and see if it works. these are the threads regarding the problems and possible fixes.
https://forum.mysensors.org/topic/3719/nrf24l01-vs-nrf24l01-pa-lna
https://blog.blackoise.de/2016/02/fixing-your-cheap-nrf24l01-palna-module/
https://forum.allaboutcircuits.com/threads/nrf24l01-pa-lna-seems-that-the-pa-power-amplification-portion-of-the-module-is-failing.127403/
```

---
## \#97 Posted by: ervinelin Posted at: 2018-04-03T17:22:17.112Z Reads: 291

```
But this wasn't a problem with the wired non-PCB receiver?

I did a ground test and got maybe 20m away in direct line of sight. Honestly that's more than I ever need for esk8 but more range wouldn't hurt!
```

---
## \#98 Posted by: webst Posted at: 2018-04-03T18:05:29.644Z Reads: 296

```
This module/company has good history according to [that](https://forum.mysensors.org/topic/3602/alternatives-for-nrf24l01/11) thread: https://www.aliexpress.com/item/E01-ML01DP5-Ebyte-2-4GHz-20dBm-2100m-nRF24L01-SPI-Wireless-transceiver-module/32638720689.html
```

---
## \#99 Posted by: Zyb Posted at: 2018-04-03T18:06:20.709Z Reads: 298

```
nope this wasnt a problem with non pcb receiver and i got those nrf modules about 1-2 months ago. after that ordered another 2 nrfs to try out your version and these 2 modules have exactly the same problem and behaviour. i desoldered everything from pcb and tried with cables, result was the same so pbc is not the problem here. people on forums say step down voltage regulator like LM2596 must be used for stable 3.3v and use it to power nrf module along with LC filter but some tried and did not change a thing. some say it works etc..
```

---
## \#100 Posted by: Zyb Posted at: 2018-04-03T18:08:58.455Z Reads: 289

```
yes i just bought 2 modules from this seller. im already curious about the result but unfortunately at least 3 weeks until they arrive
```

---
## \#101 Posted by: ervinelin Posted at: 2018-04-03T18:13:45.825Z Reads: 275

```
I will update once mine come in. I bought 3 different ones just to test...
```

---
## \#102 Posted by: Zyb Posted at: 2018-04-03T19:16:50.744Z Reads: 282

```
ok looking forward to your tests. i think im going to use a small voltage regulator like this http://uk.farnell.com/taiwan-semiconductor/ts2940cz-3-3-c0/ic-v-reg-3-3v-2940-to-220-3/dp/7261373
basicly going to feed it with 5v and ground resulting in stable 3.3v
```

---
## \#103 Posted by: webst Posted at: 2018-04-04T08:18:03.038Z Reads: 293

```
Omitting high power consumption (still acceptable though), how hard would be porting the code to following ESP32 platform?
https://www.banggood.com/Wemos-TTGO-WiFi-Bluetooth-Battery-ESP32-0_96-Inch-OLED-Development-Tool-p-1213497.html

That would solve most problems and will allow much easier replicability.
```

---
## \#104 Posted by: Zyb Posted at: 2018-04-04T14:14:29.240Z Reads: 285

```
ive seen that board yesterday and it looks like has alot inside for its price. if i had enough knowledge in programming i would have definitely tried. 

meanwhile that company is specialized in wireless communication, they claim they get their parts from japan and germany also they are using genuine nordic nrf24 chip.
i got 2 from these https://www.aliexpress.com/item/2-4GHz-rf-Wireless-uhf-Module-Power-Amplifier-E01-ML01SP4-Original-SENET-1-8km-2-4g/32806320077.html?shortkey=eUB7RJZv&addresstype=600

these are from the same company but with integrated antenna 
https://www.aliexpress.com/store/product/CDEBYTE-2PCS-Lot-SPI-SMD-Module-E01-ML01S-2-4GHz-0dBm-110m-nRF24L01-Wireless-RF-transceiver/2077046_32803028476.html?spm=2114.12010612.0.0.62fe19e9gUMIhc 
depending on space constraints the one with integrated antenna might be the one for the transmitter but either way im gonna try the first one with short whip antenna and see how it goes.
```

---
## \#105 Posted by: ervinelin Posted at: 2018-04-04T14:43:21.742Z Reads: 254

```
That's the shielded one I ordered, should reach me next week I hope...
```

---
## \#106 Posted by: Zyb Posted at: 2018-04-04T16:15:00.589Z Reads: 260

```
hope it works, looks like a good chip but we will see :slight_smile:
```

---
## \#107 Posted by: webst Posted at: 2018-04-04T20:19:43.032Z Reads: 264

```
This is the same module and company I pasted yesterday. But going back to this almost ready ESP32 dev tool there's ChibiOS nunchuck code written by Benjamin that somebody with more programming knowledge could port to FreeRTOS that runs on ESP32. Adding joystick or hall sensor and we're set with almost no soldering.
```

---
## \#108 Posted by: ervinelin Posted at: 2018-04-05T10:10:09.634Z Reads: 277

```
The ESP32 looks super cool but coding for it is waaaay over my head. Hopefully someone can take up he challenge!
```

---
## \#109 Posted by: ervinelin Posted at: 2018-04-07T16:35:29.438Z Reads: 297

```
So I got some of the new NRF modules in (not the shielded ones yet).

![IMG20180407235044|690x388](upload://1PjyRzaYY4pzhxNiAhgZbQ5xtkm.jpg)

I compared two identical receivers, one with the old ceramic antenna, and one with the uFL antenna. All other things equal, same arduino, same copper tape shielding, same 47uF tantulum cap on the 3.3V line. In this case I tried the smaller module which LOOKS like it's a better build... The black module in the middle looks exactly the same as the ceramic cap module just with a uFL connector instead.

![IMG20180408003016|690x388](upload://90rWE4SQi8Rsu1nM7A3nBDIoCpR.jpg)

The one with the antenna is a clear winner, much longer range on the bench and I suspect will be the same outdoors as well. I highly recommend to use this style of modules moving forward.

I am waiting for the shielded module to put it into my transmitter.
```

---
## \#110 Posted by: ervinelin Posted at: 2018-04-07T16:37:13.750Z Reads: 270

```
I was researching a little more... looks like a port MIGHT be possible.. I'll see if I have enough time to try this..
```

---
## \#111 Posted by: webst Posted at: 2018-04-07T16:46:22.161Z Reads: 272

```
This thing is programmable using Arduino IDE
```

---
## \#112 Posted by: ervinelin Posted at: 2018-04-07T17:14:07.297Z Reads: 264

```
Yes I know, but doesn't mean you can port over everything so readily...
```

---
## \#113 Posted by: FalconNL Posted at: 2018-04-08T21:49:24.957Z Reads: 271

```
[quote="ervinelin, post:110, topic:48231"]
looks like a port MIGHT be possible
[/quote]

Dude I love the project so far. You are miles ahead of anything i could do at this point but you're such a inspiration to me! Thank you so much for the write up! Would love to build
```

---
## \#114 Posted by: JamesNothing Posted at: 2018-04-08T23:00:58.464Z Reads: 267

```
this is really awesome and I'd love to make one, but I'm shit with electronics, arduinos and stuff like that. 
But I really like this project and want to help, so aside from being really sad for my lack of skills, I could print the remote for anyone who needs it and does not have access to a 3d printer (at least in Europe, as I'm located in Italy) for the price of material+shipping.
```

---
## \#115 Posted by: ervinelin Posted at: 2018-04-08T23:16:57.993Z Reads: 262

```
@FalconNL

Glad you liked it, hopefully you can attempt building one.

@JamesNothing

We all gotta learn sometime!
```

---
## \#116 Posted by: JamesNothing Posted at: 2018-04-08T23:25:37.381Z Reads: 268

```
[quote="ervinelin, post:115, topic:48231, full:true"]
We all gotta learn sometime!
[/quote]

you're totally right and I think I'll give this a try once I'll have a little more free time.
in the meanwhile if I can help someone else with it I more than glad to do it.
I work with 3d printers for a living (sls machines) and we have an ultimaker2 for fast prototypes use, so putting some remotes on it is not a big deal for me :)
```

---
## \#117 Posted by: moon Posted at: 2018-04-08T23:27:58.324Z Reads: 257

```
Working with 3d printers seems like a fun job!

You should prepare pricing for the 3D prints
```

---
## \#118 Posted by: JamesNothing Posted at: 2018-04-08T23:39:17.652Z Reads: 256

```
I can get nice materials like petg or things like colorful XT (co-polyester) relatively cheap, so the material price should be in the vicinity of 2-3€ for a complete set.
I'll search some low cost shipping companies (any advice here?) to keep the final cost as low as possible.
```

---
## \#119 Posted by: moon Posted at: 2018-04-09T00:13:07.183Z Reads: 264

```
[quote="JamesNothing, post:118, topic:48231"]
I can get nice materials like petg or things like colorful XT (co-polyester) relatively cheap, so the material price should be in the vicinity of 2-3€ for a complete set.
[/quote]

Wow! Really cheap

It really depends were your from with shipping prices but in most cases if it is a small package it is usually the government owned shipping company that will be the cheapest
```

---
## \#120 Posted by: Zyb Posted at: 2018-04-09T00:22:15.313Z Reads: 259

```
results are expected, thanks for taking time and budget for testing all these modules. i think the shielded one will be better and you wont have to use copper tape. im also currently waiting for mine.
```

---
## \#121 Posted by: ervinelin Posted at: 2018-04-09T00:50:57.178Z Reads: 246

```
Great... Just remind me to upload the latest STLs to thingiverse first! Made some minor almost not noticable changes but still better to use the most update one.
```

---
## \#122 Posted by: TarzanHBK Posted at: 2018-04-09T06:35:58.910Z Reads: 242

```
With Italian Post, should be something like a padded maxi-letter for something about 7€ shipping worldwide.
```

---
## \#123 Posted by: JamesNothing Posted at: 2018-04-09T09:45:03.142Z Reads: 261

```
Tarzan  i'd prefer not to use Italian Post services if possible at all: They're renowned to be as bad as it can humanly get :smile:
BUT if they're the cheapest of them all I think we can compromise.

[quote="ervinelin, post:121, topic:48231"]
Just remind me to upload the latest STLs
[/quote]
Sure thing! let me know when it's safe to download them. I'll try a couple of materials as soon as possible to choose what's best to print it with in terms of price/performance/"beauty"
```

---
## \#124 Posted by: moon Posted at: 2018-04-12T15:30:05.643Z Reads: 244

```
Can you do carbon fibre reinforced ABS?
```

---
## \#125 Posted by: JamesNothing Posted at: 2018-04-12T15:45:34.518Z Reads: 265

```
it's not that I can't but I don't. Cf infused materials (and also fluorescent materials/metal infused...) are a pain in the ass to print because they chew trough nozzles like crazy. I can do pla, abs (if needed, but I prefer not to have nasty fumes around the office), colorfabb XT (Amphora HT5300 3D copolyester), petg, some nylon filaments (not as strong as you may think but very flexible)
```

---
## \#126 Posted by: moon Posted at: 2018-04-12T15:46:11.784Z Reads: 265

```
Nylon will do the job, thanks :)
```

---
## \#127 Posted by: ervinelin Posted at: 2018-04-16T09:20:07.609Z Reads: 286

```
Shielded NRF reached me.

Really tiny! But it's just a hair wider blocking one of my bolts that hold down the PCB.

![IMG20180415114442|281x500](upload://mNnpS2fQ1CTgnQUiAYCHbVoPy0n.jpg)

Still busy wiring it up but I got connected without the need for any copper tape...
```

---
## \#128 Posted by: ervinelin Posted at: 2018-04-16T18:45:51.192Z Reads: 266

```
So I finished the new remote with the new shielded module, oddly the range is not as good as the original plain ceramic version...

Not sure what gives, will have to investigate a bit more...
```

---
## \#129 Posted by: ervinelin Posted at: 2018-04-17T17:44:00.344Z Reads: 262

```
SUCCESS!!! (On the bench at least).

I used a Frsky PCB antenna (https://www.banggood.com/FrSky-PCB-Antenna-For-X8R-X6R-Receiver-p-991728.html?cur_warehouse=CN) and bench testing has shown to have much further range than before.

However, antenna placement is very finicky and the lack of space in the remote doesn't help. Any pressure on the NRF module and there goes the signal.

Took me a while before I managed to get it to work reliably. Will test in the field tomorrow.
```

---
## \#130 Posted by: osbor Posted at: 2018-04-17T18:22:27.364Z Reads: 254

```
good thing i stumbled on this; this is an excellent, high feature diy design, good shit.
although it seems like there's been a lot of progress since the first post, any chance of updating that assuming you haven't already?
```

---
## \#131 Posted by: Zyb Posted at: 2018-04-17T18:56:19.105Z Reads: 284

```
im surprised that antenna even fits inside the remote looks bulky. i got 2 types of antenna from this one https://www.aliexpress.com/item/3DBI-Brass-2-4G-Receiver-Antenna-Omnidirectional-IPEX-Port-Compatible-Futaba-JR-WFLY/32791504529.html?spm=a2g0s.9042311.0.0.snbcUf and from this one https://www.aliexpress.com/item/5PCS-150mm-2-4G-Receiver-Antenna-IPEX-Port-For-FRSKY-JR-FRSKY-IPEX-interfaces/32754319893.html?spm=a2g0s.9042311.0.0.snbcUf see how it goes with them when they arrive. also still waiting on the modules :confused:
anyway while waiting for them i did a minor modification to receiver side for a good 3.3v source. i used voltage regulator TS2940CZ-3.3  http://uk.farnell.com/taiwan-semiconductor/ts2940cz-3-3-c0/ic-v-reg-3-3v-2940-to-220-3/dp/7261373 basicly feeding with ground and 5v and gives you a stable 3.29 v according to my measurement. in order to make it easy for the soldering job i eliminated the 3v3 connection from arduino to pcb instead i soldered 3v3 output from regulator to the corresponding hole in pcb (the one with the red cable) also added nichicon 1000uF lowESR cap next to it. i hope all these improvements gonna have a positive effect because i have had enough of these crappy wifi connection issues :( 

![image_123923953 (10)|500x500](upload://aAtO3QGXkc6K5SDAyABxMj9GB0S.JPG)
![image_123923953 (9)|500x500](upload://whwfqGobUDYJMKlGltOTdvHIdJ2.JPG)
```

---
## \#132 Posted by: ervinelin Posted at: 2018-04-18T01:02:40.517Z Reads: 269

```
I plan to but so busy with work and family and building and rebuilding. I had a lot of problems with this particular build, stripped a pad, smoked a trace, had to jumper wires manually. Not sure why it would happen too!

Essentially some things I need to update once I am confident everything should work seamlessly.
1. Some minor changes to the STLs
2. Updates to the BOM to include the better modules and antennas
3. Updates to the code to include the 250kbps transfer speed
4. Updates to the PCB files to correct for the changes in the modules
5. Updates to the build guide to reflect these updates.

As you can see, a fair amount of work with hardly any time to do them all...
```

---
## \#133 Posted by: ervinelin Posted at: 2018-04-18T01:04:19.556Z Reads: 262

```
In my testing only 2 things made a significant difference.

1. Changing connection speed down to 250kbps
2. Using whip 2.4gHz antennas (either modding the ceramic one or using another module with uFL)

I suspect the better NRF modules are also better at modulating noise in the voltage lines but let me know if all that work to regulate the 3.3v helps.

The PCB antenna is long but it's very flat, so it fits quite nicely actually.
```

---
## \#134 Posted by: ervinelin Posted at: 2018-04-18T10:25:44.454Z Reads: 267

```
Here's a video of the range I am getting...

https://youtu.be/b6dGFBtb3PI
```

---
## \#135 Posted by: osbor Posted at: 2018-04-18T13:15:32.759Z Reads: 272

```
hah, now you're just showing off.
Also i wouldn't worry about packaging issues, once the BOM is more nailed down it's easy to modify the casing STL to be a little wider to accommodate components.

also if your printer can do it, highly recommend printing with carbon fiber nylon. Just make sure you have a hardened nozzle and print from the filament inside a tub with moisture absorbing beads.
also, nice tesseract deck
```

---
## \#136 Posted by: Zyb Posted at: 2018-04-18T15:37:42.660Z Reads: 259

```
that is an impressive range. did you get any dropouts? also did you use the same antenna*nrf combo on both receiver and transmitter?
```

---
## \#137 Posted by: ervinelin Posted at: 2018-04-18T15:50:12.604Z Reads: 265

```
I rode for about 2km, no issues so far. I did have to re-do the bottom PCB as the stupid lipo charger died on me (2nd one that I had to replace).

At the maximum range in the video the signal icon started to drop in and out but any closer and it was solid throughout.

Transmitter is using the shielded module, receiver is using the normal ceramic version but modified with a whip antenna.

But word of caution, the antenna placement in the transmitter is VERY finicky... I don't know what exactly is it that's the problem but in some orientations it just refuses to work.
```

---
## \#138 Posted by: Zyb Posted at: 2018-04-18T16:53:26.316Z Reads: 273

```
do you mean that tp4056 module as a lipo charger? 
oh i see ok i ll will try with the antennas i ordered if they dont work well going to try your antenna or get one of these for transmitter. https://www.aliexpress.com/item/CDEBYTE-2PCS-Lot-SPI-SMD-Module-E01-ML01S-2-4GHz-0dBm-110m-nRF24L01-Wireless-RF-transceiver/32803028476.html?spm=a2g0s.8937460.0.0.EnZr0i
considering they are from the same company they should work better than those with ceramic ones but ofc tests are needed in order to confirm but for receiver definitely going to use that shielded nrf with the antenna as the space is not a big issue there.
and maybe with this module https://www.aliexpress.com/item/DC-5V-2-1A-USP-Mobile-Power-Diy-Board-4-2V-Charge-Discharger-boost-battery-protection/32824032545.html?spm=a2g0s.8937460.0.0.EnZr0i it is possible to use the same layout as your receiver pcb design. this replacing the 5v boost and tp4056 and nrf module being smaller than the ceramic one could squeeze side by side under the arduino.
```

---
## \#139 Posted by: ervinelin Posted at: 2018-04-19T04:03:26.930Z Reads: 266

```
Hm... that all in one charger/booster might save some space but there's still a need for the USB port.

Let me order a few pieces and see if everything can be squeezed more readily into one neat package. That'll mean a need to redesign the PCB as well.

To be honest I think the non-antenna version should be good enough, we only need maybe 10-20m range (in the case of a run away board). I'll order some as well to test.

Erv.
```

---
## \#140 Posted by: Zyb Posted at: 2018-04-19T15:52:48.012Z Reads: 273

```
yea sadly usb port must be wired like the original build or can be replaced with a small barrel plug but i think its not really convenient so usb port is still a way to go imo.
also that module has a charge,discharge and battery protection features according to the description which is nice to have.
also theres a place for an on/off key on the module, similar to how evolve remote works. press once it turns on, double press and hold it turns off. that could be used with the momentary switches which is already in the build but probably the ones you use are a more solid approach and less prone to failure.
module is 27mm long and the new nrf with antenna is 18mm long which gives you just enough room to fit them together under your receiver pcb giving you only nrf and 5v-gnd connections. all the rest must be soldered on the arduino or like you said a new pcb design.
```

---
## \#141 Posted by: Zyb Posted at: 2018-04-19T18:54:23.404Z Reads: 282

```
ok this is my first take on this, total noob but i tried to make a schematic with the new module. one thing i noticed is we cant put the on off switch between the battery and the boost+charger. if we put a switch in between it wont be able to charge it when the circuit is open. so battery must be hard wired to the module. i wired + side of the battery with 10k resistor to pin A2 but the actual on off switch is on the output side of the module so im not sure how this is going to work or going to work at all.. or may be its designed to work only with its on off key which i mention in my previous post.
![Capture|592x500](upload://9uILdAUrkhEnHUB7CSMVSLxcK2S.JPG)
```

---
## \#142 Posted by: ervinelin Posted at: 2018-04-19T23:11:11.595Z Reads: 262

```
I am wondering if there is a means to NOT use the onboard switch. I much prefer a rocker.

I ordered a few pieces to try... Let's see.. schemetically wise looks fine.

I also ordered some esp32s as well to see how hard it is to port over the software. From what I have seen the only problem is actually the VESC data which if we don't have a library it won't be able to port.
```

---
## \#143 Posted by: Zyb Posted at: 2018-04-19T23:48:09.479Z Reads: 262

```
yea i think rocker is a better solid choice too. this specific board may force you to use its on off key but theres another one which is without that key. just battery, usb and 5v terminals in total 6. probably you have seen it, it was in the related products. rocker switch definitely would work with this one https://www.aliexpress.com/item/6W-5V-UPS-mobile-power-Diy-Board-Charger-Step-up-DC-DC-Converter-Module-for-3/32790658678.html?spm=2114.10010108.1000023.9.14e97b70TYSyNv
yes esp32s is very nice package it has everything. if you can make it work it would be awesome :slight_smile:
```

---
## \#144 Posted by: Zyb Posted at: 2018-04-20T22:51:00.743Z Reads: 279

```
i tried to design a new pcb with the modified components it is one piece 2 layers i have no idea if it is allright to use i think someone experienced needs to check it but at least there are no DRC errors. also added cap along with a voltage regulator to the nrf24 module. theres no cap on 5v line tho. on the side are the measurements of the modules. theres a small gap in between them so they should mount ok.
here is the link https://easyeda.com/orhanyoruk/kumandam
![Capture1|401x500](upload://fTTZYOH14IfuWwoRVjFEQ7WFcJQ.JPG)
EDIT: edited and updated the pcb with MCP130T-300I/TT supervisory chip which holds the reset until nano has a 3v on 3.3v line and then resets the board. it can be ignored if the issue is not present but it has a place just in case.
EDIT2: i just inspected the nano v3 board and under it theres already an ams1117 3.3v regulator. looking at these types of regulators data sheets they all require tantalum capacitor at both ends (vin, vout) usually 10-22uf tantalum is recommended on the vout side. in this case i thought it would be better to remove lm1117 and replace it with 22uf capacitor for 3.3v line. also added another one for 5v line.
```

---
## \#145 Posted by: Zyb Posted at: 2018-04-26T09:56:57.474Z Reads: 256

```
i just remembered this post and tried to search for 250 value in your code but i couldnt find it. googled for this particular subject and i saw post saying you have to put ''radio.setDataRate(RF24_250KBPS);'' right after ''radio.begin();'' is it correct?
```

---
## \#146 Posted by: ervinelin Posted at: 2018-04-26T18:54:08.116Z Reads: 254

```
Yes you are right, after radio.begin().

  radio.begin();
  radio.setDataRate(RF24_250KBPS);
```

---
## \#147 Posted by: ervinelin Posted at: 2018-05-11T23:45:57.297Z Reads: 247

```
So I got all the newer components as well as the ESP32s but I have no time to go fix things up as I'm busy building my boards... 

Anyone else progressed?
```

---
## \#148 Posted by: Zyb Posted at: 2018-05-12T09:20:47.573Z Reads: 252

```
My wifi modules just arrived but I’ve changed the pcb layout and added some smd tantalum caps. Waiting for them right now. Transmitter pcb is one piece like we discussed earlier. It utilizes that 2in1 booster/charger module. Transmitter pcb has 220uf tantal d case on 5v. 100uf d case, 10uf b case and 1206 ceramic 100nf for 3,3v. Receiver has the same cap layout but instead of 220uf it has enough room for 1000uf on 5v. I ll see how it’s gonna turn out after they arrive. I think it strongly depends on booster/charger to work as intended. The rest is ok. 
Also prints went ok, they might need some sanding here and there :slight_smile:
```

---
## \#149 Posted by: ervinelin Posted at: 2018-05-12T09:37:57.094Z Reads: 243

```
So u fit everything on one PCB??? Got a pic?
```

---
## \#150 Posted by: Zyb Posted at: 2018-05-12T11:54:58.068Z Reads: 251

```
Yes pcb design is shared. I ll find the link and share it when I arrive at home. I kept the same dimensions of your original pcb design and pcb holes are in the same place. I hope I didn’t do any mistake with the design. I will test it when they arrive of course I need that booster/charger module it is on its way too.
Edit: Forgot to mention I also added a place for mcp130 to watch for 5v line. That’s of course totally optional just in case for power/reset issues we had earlier but some people did not have this problem.
```

---
## \#151 Posted by: Zyb Posted at: 2018-05-12T12:58:33.249Z Reads: 293

```
these are the final designs which i ordered. 
![Capture1|283x401](upload://sySNhYAhvhwhd0efwishMyMgZBV.JPG)![Capture2|283x488](upload://Aqye0DJeDmX10iNNj10tptMtAZL.JPG)
![Capture3|157x420](upload://o1dAxzoxxGguYH53KjIZHOLH75F.JPG)![Capture4|161x430](upload://z8pfpOhangLs55xIE7gf0xGAJO9.JPG)
you can find them in this link https://easyeda.com/orhanyoruk/kumandam  ''rx'' and ''finalSMD'' are the ones i ordered.
```

---
## \#152 Posted by: Zyb Posted at: 2018-05-18T21:53:15.733Z Reads: 298

```
I just received the pcbs and wireless modules today. Tried out couple of prototypes. So far these crappy antenna is no good. Unless I touch it with my hand it doesn’t connect to the receiver. I have 5 of these some of them doesn’t work even if I touch them. So like you suggested that antenna seems like superior (forgot it’s name). Build another receiver with internal antenna from the same company and made the connection with original firefly remote (with ceramic antenna) and I got the best signal so far. 7 meters with 2 solid walls in between. Waiting on another antenna purchase a while ago, once I got it i ll use it on transmitter side and report back. Btw receiver pcb has 100uf tantal, 10uf tantal, 100nf ceramic all parallel to 3.3v -gnd and 1000uf low esr on 5v![image|400x500](upload://kQtMM60fTMtPrVUBi4gtp6vhJXQ.jpeg)
```

---
## \#153 Posted by: ervinelin Posted at: 2018-06-02T09:22:43.014Z Reads: 288

```
**IMPORTANT UPDATE**

So @Zyb has been asking why his remote loses connection when he rapidly changes throttle positions (e.g. accelerate and brake rapidly). This was an issue on the bench but not in not really in the real world but was worth investigating.

So I spent several hours debugging component by component and it wasn't the hall sensors, the connection between receiver and transmitter or anything like that. It was the code using analogWrite instead of the servo.write function to send the throttle position to the VESC.

I have adjusted the code to use the servo library instead and have bench tested this, see the GitHub below.

https://github.com/ModMiniMan/nRF24-Esk8-Remote/tree/master/receiver_VESC6

**DO NOTE THAT YOU DO NEED TO RECALIBRATE YOUR REMOTE IN VESCTOOL AFTER FLASHING THIS NEW FIRMWARE!!**

**ALSO, PLEASE USE THIS WITH CAUTION AT YOUR OWN RISK. PAD UP!!**

Many thanks to @zyb for raising this concern!
```

---
## \#154 Posted by: Acido Posted at: 2018-06-02T10:07:38.822Z Reads: 267

```
Im really interested in this, nice work @ervinelin !
I will try and wait for a month or two so I can trust this a little bit more, kinda sceptic on it since i will be building it and a lot of my stuff breaks down especially electronics since I just want them to work and hurry up and not take time to make it nicely :smiley:
```

---
## \#155 Posted by: ervinelin Posted at: 2018-06-02T10:34:43.735Z Reads: 265

```
I know what you mean... I've spent MONTHS working on this remote..

I've built like 5 of them, each time improving on the last... Really rather be riding
```

---
## \#156 Posted by: Acido Posted at: 2018-06-02T10:44:41.817Z Reads: 263

```
My board is out of commission for at least a month or so and i haven't ridden it at least 2-3 months because im rebuilding it, kinda feels sad
only the drive train left to do :D
```

---
## \#157 Posted by: ervinelin Posted at: 2018-06-02T12:01:16.124Z Reads: 266

```
That's why you always have more than one board!
```

---
## \#158 Posted by: Acido Posted at: 2018-06-02T12:05:27.382Z Reads: 261

```
I got myself a gasoline goped, changed the engine, tuned it out and it has 6hp :D
```

---
## \#159 Posted by: webst Posted at: 2018-06-02T13:41:35.811Z Reads: 258

```
So slightly less than dual 2,5kW motors? :slight_smile:
```

---
## \#160 Posted by: Jc06505n Posted at: 2018-06-02T13:49:59.258Z Reads: 252

```
Did you do a push request of this correction also to @solidgeek’s repo ?
```

---
## \#161 Posted by: Acido Posted at: 2018-06-02T14:40:26.243Z Reads: 247

```
If i press full throttle it throws be backwards, much more torque, doing burnouts with no problem
the difference is huge when going uphill i have a single 6374 and a 1.5hp hand held land mower engine kills it uphill with the same driver and thats 43cc
now imagine driving a 200hp motorcycle :smiley: it must be super fun but i would kill myself within a week
```

---
## \#162 Posted by: ervinelin Posted at: 2018-06-02T14:44:26.433Z Reads: 238

```
No I did not... actually this is the first time I've used Github... not sure exactly how push (or pull) work...
```

---
## \#163 Posted by: Zyb Posted at: 2018-06-02T16:40:49.615Z Reads: 248

```
just wow man.  you are brilliant @ervinelin i tested it the way i tested yesterday and its working everytime now. i think you fixed another problem too. along with that problem i was having %50 brakes ocassionally when in reality i was givin %100 input. that happened alot during the bench testing and this was not related with quick flicking the throttle. i had this problem during my ride too but i just kinda overlooked it but its of course dangerous as when i realize brakes are not working properly i was letting go off throttle and applying the breaks for the second time and hoping they will work.(they usually work) that problem is gone. all i can see is butter smooth acceleration and brakes in vesc tool. 
btw this problem is present in original firefly remote too.
```

---
## \#164 Posted by: Zyb Posted at: 2018-06-02T16:43:24.115Z Reads: 239

```
oh i forgot to add to whom who wanna use the new code make sure ''const uint64_t pipe ='' value is matching on both transmitter and receiver code. i downloaded the receiver ino and they just wouldnt connect then i realized values are different so make sure to correct that.
```

---
## \#165 Posted by: ervinelin Posted at: 2018-06-03T00:33:31.527Z Reads: 247

```
Oh yes sorry I forgot about that on the GitHub...

In any case you are supposed to use your own pipe address just in case you meet someone who is using the same remote
```

---
## \#166 Posted by: Zyb Posted at: 2018-06-03T13:54:36.490Z Reads: 266

```
![image|375x500](upload://skErFIJauxJMdGGP3bgPCxLPCFr.jpeg)![image|644x500](upload://53c9K4F78Z92i6nuBZLvxFbeiM7.jpeg)

Quick testing with one piece pcb looks like working for now. As soon as I complete it will report back
```

---
## \#167 Posted by: ervinelin Posted at: 2018-06-03T14:03:52.250Z Reads: 254

```
Woah u fit everything!! Awesome
```

---
## \#168 Posted by: dg798 Posted at: 2018-06-03T14:54:04.753Z Reads: 251

```
Would anyone want to trade one of these for a brand new nano x in box with everything including cable and a brick for the cable
```

---
## \#169 Posted by: Zyb Posted at: 2018-06-03T16:35:45.482Z Reads: 270

```
![image|375x500](upload://uyoFINmTZK5qQEhtiDkisrako38.jpeg)![image|375x500](upload://idZGLikGPtlh3w7nLgzCZxJxe3x.jpeg)![image|375x500](upload://5csrH62kQZ8lsqIz2ePo4toincQ.jpeg)
Feels very good in hand everything works no gimmicks. I might change the antenna looks unreliable but still holds its signal as you can see I didn’t even notice when I was taking picture but there are 2 walls in between at the moment of the shot and it still shows the voltage of my battery. I added mcp130 to the board just in case of a power issue but I didn’t have the chip so instead I had to use 470ohm resistor in series with 10uf capacitor to make it work because even fast flick of on off button doesn’t work. You need to press reset button or the solution I did. Credits to arduino forums.
Edit: and the receiver
![image|375x500](upload://lRApqPq78fuUgXg9aAsW147SWj6.jpeg)
```

---
## \#170 Posted by: mikenyc Posted at: 2018-06-03T17:36:37.358Z Reads: 264

```
https://www.youtube.com/watch?v=Yd0fBXwDBmo
```

---
## \#171 Posted by: dg798 Posted at: 2018-06-03T18:35:20.474Z Reads: 257

```
That’s great!
Anyone wanna trade?
```

---
## \#172 Posted by: Zyb Posted at: 2018-06-03T18:43:46.495Z Reads: 254

```
You might have better luck on firefly remote thread as there are more remotes made of that version. Dunno how many of us are there with this version but I feel like there are very few of us :slight_smile:
```

---
## \#173 Posted by: b264 Posted at: 2018-06-03T18:53:02.019Z Reads: 261

```
[quote="ervinelin, post:162, topic:48231, full:true"]
No I did not… actually this is the first time I’ve used Github… not sure exactly how push (or pull) work…
[/quote]

I made one

https://github.com/SolidGeek/nRF24-Esk8-Remote/pull/8

SolidGeek has to approve it and inspect your changes...
```

---
## \#174 Posted by: dg798 Posted at: 2018-06-03T18:56:18.530Z Reads: 247

```
Well just putting out here in case anyone wants to
```

---
## \#175 Posted by: dg798 Posted at: 2018-06-03T18:59:06.917Z Reads: 251

```
Or if someone wants to send a kit to trade I would do that to. It doesn’t have to be assembled.
```

---
## \#176 Posted by: mikenyc Posted at: 2018-06-03T19:03:00.029Z Reads: 246

```
Could you explain the rationale behind your thinking? Why would someone want to trade for a nano-x?
```

---
## \#177 Posted by: dg798 Posted at: 2018-06-03T19:57:11.963Z Reads: 251

```
I don’t know if someone would want to. I just want to trade because looking at the parts list the price comes out to about the price of a nano x
```

---
## \#178 Posted by: mikenyc Posted at: 2018-06-03T19:59:18.866Z Reads: 244

```
Maybe you can ask if someone is willing to make one for you?
```

---
## \#179 Posted by: dg798 Posted at: 2018-06-03T20:06:12.222Z Reads: 242

```
That works to. As long as I get the remote. Whether it’s a kit the remote or someone building one for me.
```

---
## \#180 Posted by: ervinelin Posted at: 2018-06-04T01:06:31.611Z Reads: 253

```
Can I know what the resistor and cap are meant to do?

Also can you share your new PCB file for reference?
```

---
## \#181 Posted by: Zyb Posted at: 2018-06-04T08:34:30.354Z Reads: 243

```
sure its already shared but let me drop it again https://easyeda.com/orhanyoruk/kumandam in this project i ordered files named ''rx'' and ''FINALsmd" im not sure if the others are ok or even finished.
it is for infamous reset problem. you did that aswel by adding a cap between reset and gnd pins.
here https://forum.arduino.cc/index.php?topic=256771.30 post number 37 explains if you connect a cap(10uf) in series with a resistor(470Ohm) you avoid damaging reset switch or anything else. well that worked like a charm for me but on the pcb theres a place for mcp 130-450. it is supposed eliminate reset issue but havent tested myself so im not sure.
going to order these if i ever make another remote https://www.aliexpress.com/item/Free-shipping-10pcs-lot-MCP130T-450I-TT-MCP130-SOT23-3-new-original/32823005999.html?spm=a2g0s.8937460.0.0.130d2e0ejSGG0x
```

---
## \#182 Posted by: ervinelin Posted at: 2018-06-04T12:34:32.625Z Reads: 238

```
Oh one more thing.. how are you juicing the lipo charger board? Thru the Arduino USB?
```

---
## \#183 Posted by: Zyb Posted at: 2018-06-04T12:42:38.147Z Reads: 248

```
Oh no, just like firefly remote I use a seperate usb mini port tho I only connect 5v and gnd pins. There’s a place for it on the pcb too on the bottom left corner there’s a polarity marking on it too. So connecting it is just like any other dm or trigger switch. This charger/booster board really saves a lot of space and hassle. If it is proven to be reliable then I think it’s the best choice.
edit: actually if there was a bit more space infront of the usb port of arduino board i could have connected 2 data wires from external port to nano port and 5v/gnd pins to chargerboard. this is how i wired my firefly and it gives you the luxury to program your arduino without opening the case. you can probably solder data wires behind the usb port of arduino nano but they really fine and i dont think i can solder wires to those microscopic pads. relocation of usb port opening would work too. i dunno its not much of a big deal you dont program it everyday so its fine like that.
```

---
## \#184 Posted by: dg798 Posted at: 2018-06-04T17:36:38.658Z Reads: 233

```
Anyone selling these?
```

---
## \#185 Posted by: mlp Posted at: 2018-06-04T21:07:28.944Z Reads: 243

```
I was going to order the MCP 130 myself, but I’m am not sure if the 130 version would work with the Arduino Nano. Doesn’t the reset pin need to be grounded to be activated?

I think the difference between 120 and 130 is that the 120 version has a low level reset output while the 130 has a high output level reset. (Edit: Not correct)

This guy use the 120 version on the Arduino due (3.3V)( post #32)
https://forum.arduino.cc/index.php?topic=256771.30

PDF: http://ww1.microchip.com/downloads/en/DeviceDoc/11184d.pdf
```

---
## \#186 Posted by: Zyb Posted at: 2018-06-04T21:39:15.430Z Reads: 234

```
yes i added mcp 130 to my pcb design according to that post and its completely optional. the guy on the post uses 300 version so it can watch over 3.3v line. i designed mine with 450 version in mind so it can watch over 5v line. mcp 130 has internal pull up resistor which you need to add to mcp 120 from external sources because it doesnt have it. also like you said it needs to be grounded and it is grounded. it has 3 legs 1-reset, 2-gnd, 3-source voltage to watch over. but then again i didnt test it yet so im not sure if it is going to work.. for now cap and resistor combo is incredibly simple and efficient. completely eliminates the problem. i have lc filter and low esr cap on receiver but the problem was still there. i even have 220uf tantalum cap on transmitters 5v line but still problem persists so its not up to those components. nothing seems to work except for the cap/resistor or possibly mcp120-130 solution.
```

---
## \#187 Posted by: mlp Posted at: 2018-06-04T22:07:23.903Z Reads: 223

```
Thanks for the reply. Ordered some to try out. I've previously tried the capacitor/resistor fix. It fixed the start up problem, but I had to remove the capacitor to be able to upload software to the microcontroller. Are u experiencing any problems when uploading software to the uC when the cap and resistor are present?
```

---
## \#188 Posted by: Zyb Posted at: 2018-06-04T22:34:00.762Z Reads: 224

```
to be honest i added the cap/resistor combo as a last minute update on the build so everything was already updated and installed but if thats gonna be a problem im definitely going to buy mcp130's to try them out. in our local shop they only have mcp130-300 which is no good to me. i need something close to 5v so it can actually work with my pcb. seems like aliexpress is my only option again :)
```

---
## \#189 Posted by: Zyb Posted at: 2018-06-04T23:10:08.007Z Reads: 212

```
booster/charger module gets too warm almost hot and battery get warm with my 5V 2A phone wall charger. then i switched to my computers usb power and everything became cool to touch so another note on that.
```

---
## \#190 Posted by: ervinelin Posted at: 2018-06-04T23:11:03.578Z Reads: 206

```
When uploading it will stall, hit the reset button when it stalls and off you go! Worked for me the last 20 times I had to upload the firmware with the cap soldered over the reset pins
```

---
## \#191 Posted by: ervinelin Posted at: 2018-06-04T23:13:12.782Z Reads: 209

```
Can you replace a capacitor on the charging board to bring down the charging amps? Or is it something else that is getting hot
```

---
## \#192 Posted by: Zyb Posted at: 2018-06-04T23:18:07.633Z Reads: 215

```
i didnt actually touch the board i was holding it from the outside so it must be even hotter in the inside but i stopped the charging let it cool off and powered it from computer everything is cool. dunno what caused it. looking at the product page https://www.aliexpress.com/item/6W-5V-UPS-mobile-power-Diy-Board-Charger-Step-up-DC-DC-Converter-Module-for-3/32790658678.html?spm=a2g0s.9042311.0.0.19834c4d6RLP6F it says charging current 0-1A is it supposed to be current going in to the module or actual charging current feeding into battery its not really clear to me. thats allright tho i have plenty of 1A chargers laying around, shouldnt be a problem.
```

---
## \#193 Posted by: ervinelin Posted at: 2018-06-04T23:55:02.146Z Reads: 214

```
Ah okay so you juiced it with too many amps. On the charging side did anything get hot?
```

---
## \#194 Posted by: Zyb Posted at: 2018-06-05T00:20:45.204Z Reads: 228

```
yea when i fed it with 2A everything got hot but after switching to computers usb power (which is i believe 900mA for usb3.0) everything is cool and charging is just finished now. im glad i didnt blow anything up as i dont have a spare board :confused:
```

---
## \#195 Posted by: Zyb Posted at: 2018-06-05T14:05:20.936Z Reads: 243

```
@ervinelin I was wondering if you got the same flysky antenna. In the product pictures it looks like it has some sort of sleeve on it but mine doesnt. Also got this one on the left see how they both perform![image|368x500](upload://yU5wX58HrM1Wz16QJmXKPXF0zM2.jpeg)
```

---
## \#196 Posted by: ervinelin Posted at: 2018-06-05T14:10:39.666Z Reads: 234

```
I use the one on the right... It fits just nicely at the back of the remote where my palm hits the remote.

The little tab at the end can be broken off
```

---
## \#197 Posted by: Zyb Posted at: 2018-06-05T14:13:36.452Z Reads: 228

```
Yes it’s really slim, it looks quite big and fat in the pictures but it’s gonna fit well
```

---
## \#198 Posted by: Zyb Posted at: 2018-06-05T21:05:36.278Z Reads: 249

```
i have 3 types of antennas at the moment. worst of them is whip antenna. it sometimes work sometimes doesnt. in above picture antenna on the left works good when theres nothing in between but as soon as i put it in the remote and hold it signal is intermittent. 
flysky one has a very strange behaviour, in open space its ok but when i put it in the remote signal is gone, disconnects for good. interesting this is when you pick up the remote and hold it, it connects and never disconnects maintaining a strong connection. as soon as i put the remote down bam there goes the signal. just dunno what to say :D but considering you are supposed to hold the remote all the time it is acceptable. antenna placement has a big role
on the other hand firefly remote has those crappy modules with ceramic antenna but it seems to be most reliable one. forgot to mention i have this module in the receiver side with internal antenna. https://www.aliexpress.com/item/CDEBYTE-2PCS-Lot-SPI-SMD-Module-E01-ML01S-2-4GHz-0dBm-110m-nRF24L01-Wireless-RF-transceiver/32803028476.html?spm=a2g0s.9042311.0.0.37a94c4dTgts39
it works good and you dont wonder if your antenna is lacking or not. if i ever build another remote i think im gonna use from those on both ends (tx and rx) + it is only $1.11 for a piece which is probably the cheapest one at the moment.
for good measure i will build another receiver with external antenna and test it the same way. see if it makes a difference. may be having external antennas on both ends will make a difference.

Update:

![Inkedimage_123923953%20(3)_LI|393x500](upload://to5mMTbqlNKWUCQswdP3B5CPJBW.jpg)
seems like i had a half build receiver which i didnt know of :D i quickly attached it to my pc to power it and started testing all possible combinations. first i would like to say antenna placement is like a night and day. the way i positioned the antenna in the transmitter works just perfect! no signal loss no disconnections and it is rock solid. end part of the antenna must face the bottom of the transmitter, other way around is just terrible. frsky antenna was still playing up when i installed it on transmitter side so i gave it a go on receiver side. transmitter was as it is in the picture with frsky antenna on receiver side. this combination gave me the best result. i went outside of my apartment walked towards the elevator and it is like 25 meters away and 3 apartments in between. cant even imagine how many walls are in between but there was a solid signal. then i swapped frsky with the other one which makes the same antenna on both sides and signal was like a tad weaker. i would say it has 1-2 meters less range than the previous combination. i was really satisfied with the result then i just tried the same connection test with my board which has the module i linked in post above with internal antenna. as soon as i step outside my apartment and walk like 2-3 meters signal disappears. modules with external antennas are just superior as long as they have optimal antenna placement. but then again we dont fly rc planes or remote control cars we need to be on the board when using the remote but knowing that you have a long range on your wireless system may help with the trust issues :)
```

---
## \#199 Posted by: ervinelin Posted at: 2018-06-05T23:05:27.609Z Reads: 230

```
Yes this mimics my experiments as well. Antenna placement within the transmitter is critical... For me the frsky PCB antenna worked the best with it being placed on the back side edge of the casing facing my palm. 

Honestly I don't know why it's soooooooo sensetive.

Erv.
```

---
## \#200 Posted by: Zyb Posted at: 2018-06-06T15:00:20.034Z Reads: 232

```
I just found mcp130t-475 chip in some online store. When they arrive hopefully in a week gonna report back if it can replace cap resistor solution
```

---
## \#201 Posted by: Zyb Posted at: 2018-06-09T11:50:02.997Z Reads: 238

```
Update: problem is solved with mcp130 i can confirm it works. 
![image|358x500](upload://nzLQTJdUZmqJFhmQ2mUf6kLwRMZ.jpeg)
The one on the right has no problem whatsoever, I tried to make it fail to boot like 10 times but it works just fine. So I had to open up my old receiver and the moment I removed the cap/resistor from reset gnd pins it failed to boot 5 times in a row. Chip is so small but some pre paste on solder pads and touching with pre tinned soldering iron for a second does the job. This specific mcp130 is mcp130T-475I/TT it releases the reset around 4.625V 
![image|297x499](upload://wFyCdfdKOZXKuNkb4fjEwTIqJUO.jpeg)
```

---
## \#202 Posted by: mlp Posted at: 2018-06-09T17:24:43.264Z Reads: 215

```
Have you figured out why the charging/boost module is getting hot? Looks like you could change a resistor going to the ME4056 IC to lower the charging current (like the original charging module).

http://www.cnzls.com/PDF/Li-ion%20Battery%20Charger/ME4056_E2.0.pdf
http://budgetlightforum.com/node/57414
```

---
## \#203 Posted by: Zyb Posted at: 2018-06-09T17:46:30.503Z Reads: 218

```
To be honest I can’t deplete the battery in a day so I’m just charging it overnight when I’m home from my computer or from 1A usb charger I have at hand. So I forgot about the problem 😂 but yea when I connect it to a 2A charger it gets really hot so I’m avoiding them but if I get a second module i might change the resistor like you suggested.
```

---
## \#204 Posted by: mlp Posted at: 2018-06-09T18:13:53.671Z Reads: 216

```
I really like how you compressed the TX stack down to one PCB! I’m going to order the TX and RX PCB's soon. Before I do so I have to ask if you have planned any PCB design changes in the near future? Is there anything you would like to change?
```

---
## \#205 Posted by: Zyb Posted at: 2018-06-09T18:40:17.698Z Reads: 216

```
It’s all thanks to that booster charger module otherwise it’s impossible at least beyond my skills. Well I didn’t have any problems or difficulties when I soldered everything. All of the caps are ok everything works just fine so yea I’m not thinking to change anything at all. Get the mcp130 just in case because you never know you may have a problem. Interesting thing was when I connected my vesc via laptop brick to program it, receiver module didn’t have any issues. The moment I switched to actual battery startup issue started to happen but on the other hand my new receiver doesn’t have any problems I’m not sure what’s causing this problem. It’s not random for sure because if you have a problem it is persistent on every boot. It doesn’t go away for couple of boots and then re appear. At least it is fixable. Signal is strong with the modules, make sure to get one of those suggested in previous posts.
```

---
## \#206 Posted by: mlp Posted at: 2018-06-09T19:28:21.516Z Reads: 198

```
Thank you for your reply. I have a few spear nrf24 with the ceramic antenna from my Firefly build. They worked ok. I have also order the 1.11$ ones with pcb antenna as you recommend in a post above. I’m thinking about ordering the shielded version with external antenna as well. Is it worth the extra $$ performance wise? 


(https://www.aliexpress.com/item/2-4GHz-rf-Wireless-uhf-Module-Power-Amplifier-E01-ML01SP4-Original-SENET-1-8km-2-4g/32806320077.html?shortkey=eUB7RJZv&addresstype=600).
```

---
## \#207 Posted by: Zyb Posted at: 2018-06-09T20:07:23.271Z Reads: 207

```
my experience with ceramic antennas are if they work then fine but i may have been unlucky and got hit by a bad batch on my second order and it was incredibly painful to see the signal dropping every second or so. i got 3 modules on that order and they were all the same. after quick googling i found various other forums related to arduino reporting the same thing and in conclusion they are unreliable to me i wont spend another dime on them. 
i cant tell for sure what would happen and the performance would be like if you have from those with internal antennas on both ends. i built my firefly with ceramic antenna and works ok with that internal antenna one on rx side but sometimes the connection is disconnecting for a second but quickly reconnects. you cant notice that while riding its for a brief moment but i dont like this and it never happens on trigger style one because i have ml01sp4 with antenna in it. definitely makes the signal stronger by a mile. if you ask me at least one of the ends should be with external antenna. but then again  E01-ML01S on both ends may work better than ceramic / E01-ML01S combination i just dont have a way to test this bcuz i bought only one E01-ML01S to test it and it became my daily drive :)
```

---
## \#208 Posted by: birdus Posted at: 2018-06-09T20:18:33.226Z Reads: 206

```
"NRF24L01+PA+LNA" is no longer available on AliExpress. What should I get instead?

Thanks,
Jay
```

---
## \#209 Posted by: birdus Posted at: 2018-06-09T20:22:50.181Z Reads: 203

```
"TP4056 1A Lipo Battery Charger Board" is no longer available on AliExpress. What should I get?

Thanks,
Jay
```

---
## \#210 Posted by: birdus Posted at: 2018-06-09T20:23:57.550Z Reads: 206

```
"0.91 inch OLED module" is no longer available on AliExpress. What should I get?

Thanks,
Jay
```

---
## \#211 Posted by: moon Posted at: 2018-06-09T20:25:51.116Z Reads: 191

```
Just search the parts into google bro
```

---
## \#212 Posted by: birdus Posted at: 2018-06-09T20:25:57.149Z Reads: 195

```
"DC-DC Boost Power Supply" is no longer available on AliExpress. What should I get?

You might want to update your spreadsheet, as several items are no longer available at the links you provided. By the way, I sure appreciate the effort you've put into this.

Thanks,
Jay
```

---
## \#213 Posted by: Zyb Posted at: 2018-06-09T20:30:08.482Z Reads: 191

```
there must be other sellers in aliexpress selling those parts. they cant be out of stock. just search them in aliexpress and you will find everything.
```

---
## \#214 Posted by: rey8801 Posted at: 2018-06-09T20:32:53.163Z Reads: 195

```
As example SMD NRF24L01 1100 meter long-distance NRF24L01 PA LNA SMD wireless modules 1100meters in stock fast delivery
 http://s.aliexpress.com/EVV3ey2I?fromSns=Copy to Clipboard
Youliterally have to copy paste the name. The are dozen of sellers. Then just order them based on number orders (top left options). Pick the you like.
```

---
## \#215 Posted by: birdus Posted at: 2018-06-09T20:35:28.798Z Reads: 199

```
Thanks, guys. Doing some Googling.

Jay
```

---
## \#216 Posted by: birdus Posted at: 2018-06-09T20:50:52.740Z Reads: 204

```
That was my first time on AliExpress. Didn't know there were different sellers. Now I get it. I just did a search on their site and looks like I found all the missing items.

Thanks,
Jay
```

---
## \#217 Posted by: moon Posted at: 2018-06-09T20:59:09.094Z Reads: 199

```
You should know that delivery can take a very long time so make sure what you order is right
```

---
## \#218 Posted by: birdus Posted at: 2018-06-09T21:03:44.351Z Reads: 206

```
Yeah, I noticed the shipping times. 40-50 days in some cases. Yikes!

Thanks,
Jay
```

---
## \#219 Posted by: birdus Posted at: 2018-06-09T21:04:01.059Z Reads: 201

```
Where can I get Ervine's Custom PCB? Google is failing me.
```

---
## \#220 Posted by: moon Posted at: 2018-06-09T21:11:58.223Z Reads: 195

```
You will either have to buy some off ervine

Or get them made by a website like pcbway
```

---
## \#221 Posted by: birdus Posted at: 2018-06-09T21:14:02.379Z Reads: 190

```
There's no ervine.com. Do you know their URL?
```

---
## \#222 Posted by: moon Posted at: 2018-06-09T21:18:10.701Z Reads: 197

```
😂😂

I meant @ervinelin .. I couldn't remember his name. He made the remote and he might have pcbs laying around.
```

---
## \#223 Posted by: birdus Posted at: 2018-06-09T21:21:34.395Z Reads: 197

```
Ah, cool. Thanks!
```

---
## \#224 Posted by: Zyb Posted at: 2018-06-09T22:22:35.898Z Reads: 201

```
:D and gotta be patient sometimes it just takes ages to get the parts. pcbs are easy you will have them in 15days max. i suggest get what you can from domestic electronics shop if the price difference is not big because you never know the part you needed the most can be available in your country and at the same time it may take 2 months to get it from aliexpress.
```

---
## \#225 Posted by: ervinelin Posted at: 2018-06-10T00:54:19.396Z Reads: 210

```
Hi guys,

Some development has taken place since I initially posted my schematics.

These include @Zyb coming up with a single layer PCB and changing some parts on the PCB, changing to better NRF modules, updating the firmware slightly etc.

Unfortunately you will need to read through the whole thread again to track everything.

I am also seeing if I can find time to redesign @Zyb current PCB to include an on board usb port, if I do so I will update all the links above. 

But first I need to finish building my current board!
```

---
## \#226 Posted by: markyoe Posted at: 2018-06-10T01:08:13.062Z Reads: 202

```
Thanks for all your work on this remote! @Zyb too! I've been following this thread for a while and seen the issues with the connection. I ordered parts that were on the BoM almost exactly a month ago. What components have you changed, and would you be able to update the parts list? Do you think it's too early in the development progress to do that?
```

---
## \#227 Posted by: ervinelin Posted at: 2018-06-10T01:44:54.807Z Reads: 201

```
The main improvement is the code actually... That has already been updated. 

The old ceramic NRF modules will work but to get more range you need to swap with the better shielded module with external antenna (might be more work than it seems).

Other than that, the reset issue is resolved either by using the hack of adding a cap between reset and ground pins or with what @Zyb has done.

Essentially the current BOM will work and had worked, we just trying to make everything even better.
```

---
## \#228 Posted by: markyoe Posted at: 2018-06-10T02:05:08.104Z Reads: 193

```
Ok, cool. What's the approx range with the ceramic modules?
```

---
## \#229 Posted by: ervinelin Posted at: 2018-06-10T02:18:16.411Z Reads: 194

```
5m or so? Good enough for esk8...
```

---
## \#230 Posted by: rey8801 Posted at: 2018-06-10T06:59:12.584Z Reads: 199

```
Is it correct model for a shielded antenna?
2.4GHz nRF24L01 PA LNA Wireless rf Module Power Amplifier E01-ML01SP4 SPI SMD 2.4 ghz Radio rf Transmitter Receiver for Arduino 
 http://s.aliexpress.com/eUB7RJZv?fromSns=Copy to Clipboard
Do we basically installed on one side, let's say the receiver since there is more space, follow the same schematic than the NRF module. Is it correct?
```

---
## \#231 Posted by: ervinelin Posted at: 2018-06-10T07:01:24.520Z Reads: 198

```
I use this only on the transmitter side. Technically you can use it on both sides. Just connect using the same pins to the PCB.

Remember to get antennas for this and never ever power them without an antenna on.
```

---
## \#232 Posted by: rey8801 Posted at: 2018-06-10T07:17:55.936Z Reads: 206

```
So the module doesn't come with an antenna. Did you used this one https://m.banggood.com/FrSky-PCB-Antenna-For-X8R-X6R-Receiver-p-991728.html?cur_warehouse=CN?
Concerning the module. Would you suggest a shielded module or the standard one it's fine as well? Thx for help. Your remote is sick :grin:
```

---
## \#233 Posted by: ervinelin Posted at: 2018-06-10T08:05:36.198Z Reads: 200

```
Yes it doesn't come with an antenna. I am indeed using the PCB frsky antenna in the link you posted.

I believe the external antenna helps but it can be an absolute nightmare to get it in the right position within the transmitter for it to work properly. 

There's also always the chance the antenna might get unplugged by accident...
```

---
## \#234 Posted by: rey8801 Posted at: 2018-06-10T08:15:49.220Z Reads: 206

```
That something I do not understand. How is suppose an antenna with enanched signal is still affected by the position inside a remote where the positions can differ for few cm. Is it perhaps a directional antenna? Meaning it needs to pointing towards the receiver. Than what the normal remotes use normally? Since I don't have problem of signal lost with them. Is it not possible to use the same solution?

So to recap also for others interested, you used the shielded module https://www.aliexpress.com/item/2-4GHz-rf-Wireless-uhf-Module-Power-Amplifier-E01-ML01SP4-Original-SENET-1-8km-2-4g/32806320077.html?spm=2114.search0104.3.15.323b3306vrSfhP&ws_ab_test=searchweb0_0,searchweb201602_5_10152_5722813_10151_10065_10344_10068_10342_5722613_5722913_10343_10340_10341_10696_10084_10083_5722713_10618_10304_10307_10820_10821_10302_10059_100031_10103_10624_10623_10622_10621_10620_5722513,searchweb201603_11,ppcSwitch_5&algo_expid=d061597b-8859-4057-b081-c8c71c34efda-2&algo_pvid=d061597b-8859-4057-b081-c8c71c34efda&priceBeautifyAB=0
plus the https://www.aliexpress.com/item/-/32855336002.html?spm=a2g0s.13010208.99999999.261.70c73c0065jeSQ
Here AliExp link.

Thx man!
```

---
## \#235 Posted by: ervinelin Posted at: 2018-06-10T08:26:03.039Z Reads: 186

```
Honestly I have no idea why the antenna placement is so critical. @Zyb had the same experience as me.

When I first tried using an external antenna I spent hours trying to figure out why it wasn't working... Turns out it's placement...
```

---
## \#236 Posted by: ElskerShadow Posted at: 2018-06-10T08:40:39.194Z Reads: 186

```
I have the 3D printer but not the skills to build the remote I think... If someone don't have a 3D printer but the skills we can make an exchange ;)
```

---
## \#237 Posted by: ervinelin Posted at: 2018-06-10T08:55:51.626Z Reads: 200

```
If you don't want to muck around with an external antenna, can consider this from the same store:

https://www.aliexpress.com/item/CDEBYTE-2PCS-Lot-SPI-SMD-Module-E01-ML01S-2-4GHz-0dBm-110m-nRF24L01-Wireless-RF-transceiver/32803028476.html?spm=a2g0s.9042311.0.0.731b4c4dT34h7Y

I have one of these in one of my receivers. Didn't have to do weird copper foil shielding for it to work...
```

---
## \#238 Posted by: rey8801 Posted at: 2018-06-10T10:25:55.381Z Reads: 200

```
This has an integrated antenna I guess. Do you think it's still better than the ceramic NRF? Then maybe using two of these two new modules will do the work. Or probably one it's already enough either in the receiver or in the Transmitter.
```

---
## \#239 Posted by: rey8801 Posted at: 2018-06-10T10:28:14.839Z Reads: 200

```
I am going to build one in the next months. Waiting for parts. If I will be able to do it, everyone can do it. Let's see it :grin: I am curious. I ordered parts for 3 remotes at least just in case something goes wrong :sweat_smile:
```

---
## \#240 Posted by: Zyb Posted at: 2018-06-10T10:32:25.357Z Reads: 195

```
get the E01-ML01S module i think its better than ceramic one. at least the company itself is specialized on wireless data transmission products.
```

---
## \#241 Posted by: ervinelin Posted at: 2018-06-10T10:36:28.654Z Reads: 194

```
Definitely better than the ceramic ones... Ceramic ones only worked with my ghetto style copper tape shielding for some stupid reason...
```

---
## \#242 Posted by: rey8801 Posted at: 2018-06-10T10:54:40.535Z Reads: 189

```
@ervinelin @Zyb deal guys. Thank you very much. Your contributions are great.

Maybe I missed something but only the STL files are available or also the original sketchs are shared? The reason why is because if someone want to change the remote frame at least can use the internal measures fixed and remodel only the outside of the remote. With STL file converted in BRep (fusion 360) you still don't have the full capability of an original file. I just wanted to ask. Of course it's not mandatory to share it :wink:
```

---
## \#243 Posted by: ervinelin Posted at: 2018-06-10T11:01:45.986Z Reads: 184

```
For now only the STL, I have shared other formats directly with those who have expressed interest in modifying it.
```

---
## \#244 Posted by: rey8801 Posted at: 2018-06-10T11:02:59.988Z Reads: 191

```
Fair enough. Thanks :grin:
```

---
## \#245 Posted by: ElskerShadow Posted at: 2018-06-10T12:03:43.383Z Reads: 190

```
Yeah I have to find the motivation :stuck_out_tongue:
```

---
## \#246 Posted by: birdus Posted at: 2018-06-10T20:21:46.267Z Reads: 203

```
Is there a higher resolution version of the schematic? Like a PDF? It's difficult to read the graphic at the top of this thread.

Thanks,
Jay
```

---
## \#247 Posted by: birdus Posted at: 2018-06-10T20:23:49.328Z Reads: 210

```
I'm planning on building a deck with 3 layers of Baltic Birch and two layers of carbon fiber cloth in between them. Will this transmitter/receiver (or any, for that matter) work with a carbon fiber deck, since carbon fiber blocks radio waves? Will the radio waves transmit around the board?

Thanks,
Jay
```

---
## \#248 Posted by: ervinelin Posted at: 2018-06-10T22:49:57.149Z Reads: 204

```
See PCB link in first post.
```

---
## \#249 Posted by: ervinelin Posted at: 2018-06-10T22:50:35.069Z Reads: 204

```
Carbon fiber will affect it for sure, but if your enclosure is not CF it might be okay.
```

---
## \#250 Posted by: b264 Posted at: 2018-06-13T19:58:58.486Z Reads: 203

```
[quote="ervinelin, post:153, topic:48231"]
I have adjusted the code to use the servo library instead and have bench tested this
[/quote]

SolidGeek [said](https://github.com/SolidGeek/nRF24-Esk8-Remote/pull/8) this fix is in the mainline code already
```

---
## \#251 Posted by: ervinelin Posted at: 2018-06-13T22:47:55.410Z Reads: 195

```
Yup I know
```

---
## \#252 Posted by: ervinelin Posted at: 2018-06-16T00:54:38.694Z Reads: 190

```
Btw anyone tried this on ackmantics vesc firmware instead of the default one? Wondering if I should swap but worried telemetry won't work anymore..
```

---
## \#253 Posted by: skslingo21 Posted at: 2018-06-18T16:41:37.233Z Reads: 190

```
You arduino controller guys are truley pioneers.
```

---
## \#254 Posted by: clistpdx Posted at: 2018-06-18T17:06:13.786Z Reads: 205

```
[quote="ervinelin, post:225, topic:48231"]
These include @Zyb coming up with a single layer PCB and changing some parts on the PCB, changing to better NRF modules, updating the firmware slightly etc.
[/quote]

@Zyb have you posted your single-layer PCB files somewhere, or can I purchase them from you? I'd like to try to build this remote using your simplified PCB's.
EDIT: Nevermind, I think I found it in post #181: http://www.electric-skateboard.builders/t/diy-trigger-style-remote-with-telemetry-complete-guide/48231/181?u=clistpdx
```

---
## \#255 Posted by: Zyb Posted at: 2018-06-18T18:00:42.839Z Reads: 201

```
@clistpdx yea that’s the one. Just make sure to order correct booster/charger module as the other ones won’t work with the pcb
```

---
## \#258 Posted by: Zyb Posted at: 2018-06-20T08:44:03.456Z Reads: 193

```
Also cases are 220 uf and 100uf D case, 10uf is B case and 100nf is 1206.
```

---
## \#259 Posted by: cryo Posted at: 2018-06-20T11:40:12.610Z Reads: 194

```
how are people running dual vescs with this remote? can it pair with 2 receivers?
```

---
## \#260 Posted by: ervinelin Posted at: 2018-06-20T11:46:57.853Z Reads: 197

```
Can bus or split ppm.
```

---
## \#261 Posted by: Zyb Posted at: 2018-06-20T11:47:43.793Z Reads: 193

```
your question doesnt apply only for this remote this is one of the fundamental information you have to acquire before running dual vescs. if you use canbus cable between vescs you connect your receiver to master vesc and its done. (of course you need to set up your slave one in vesc tool) or you can use split ppm
```

---
## \#262 Posted by: cryo Posted at: 2018-06-20T12:05:36.323Z Reads: 192

```
yup i know that but some people dont do canbus or split ppm at all and just use 1 remote with 2 receivers, 1 receiver for each vesc. was wondering if u could do that with this one.

It might screw up speed calculation but im okay with that, could probably modify code to use a new formula.
```

---
## \#263 Posted by: webst Posted at: 2018-06-20T12:07:30.737Z Reads: 187

```
Show me one of those people
```

---
## \#264 Posted by: cryo Posted at: 2018-06-20T12:11:37.607Z Reads: 194

```
https://www.electric-skateboard.builders/t/going-over-options-to-connect-two-vescs-to-remote/30484/6?u=cryo

that's 2 so far(including me)... seeing as how theres 13 likes on his post im betting theres some more people whove done it.
```

---
## \#265 Posted by: webst Posted at: 2018-06-20T12:20:52.430Z Reads: 194

```
Ok, now I understand what you're asking for. You'd like some one side redundancy. It's theoretically possible when you set same pipe address on two receivers but it should be tested first.
```

---
## \#266 Posted by: Zyb Posted at: 2018-06-20T12:21:18.432Z Reads: 194

```
there are couple of threads about this situation but im no expert i can only try but i dont have a dual setup to clarify it.
https://forum.arduino.cc/index.php?topic=448593.0
https://www.reddit.com/r/arduino/comments/2xuw7n/nrf24l01_one_transmitter_multiple_receivers/
```

---
## \#267 Posted by: ervinelin Posted at: 2018-06-20T12:25:30.721Z Reads: 187

```
Still not sure what he wants to achieve. 

Reason for 2 receivers is?
```

---
## \#268 Posted by: webst Posted at: 2018-06-20T12:27:48.454Z Reads: 188

```
4WD or one side redundancy
```

---
## \#269 Posted by: Zyb Posted at: 2018-06-20T12:35:27.504Z Reads: 186

```
well some dont like canbus because if master fails you lose slave aswell also be careful canbus easily can fry vesc if not powered at the same time. i think subject is drifting away there are plenty of discussions about this, veery long ones :D
```

---
## \#270 Posted by: ervinelin Posted at: 2018-06-20T12:39:23.972Z Reads: 191

```
Power receiver through seperate 5V BEC, dual PWM outs from single receiver?
```

---
## \#271 Posted by: Zyb Posted at: 2018-06-20T12:42:47.148Z Reads: 188

```
he means 2 seperate individual receivers per focbox so they power their own receiver from their own servo cable. eliminating the need for split ppm or canbus
```

---
## \#272 Posted by: ervinelin Posted at: 2018-06-20T12:49:26.994Z Reads: 196

```
If I am not mistaken you can do that but you need to adjust the code to take two different pipes and make sure they take turns to send the data...

Not ideal...

The idea is redundency?
```

---
## \#273 Posted by: Zyb Posted at: 2018-06-20T13:00:02.615Z Reads: 194

```
i will just drop that here thats benjamins opinion on the matter https://www.electric-skateboard.builders/t/y-piece-or-canbus/26461/85?u=zyb
```

---
## \#274 Posted by: webst Posted at: 2018-06-20T13:05:02.666Z Reads: 193

```
Still the only proper solution for 4WD would be dual receivers to masters and CAN to slaves. Or is there any other way?
```

---
## \#275 Posted by: Zyb Posted at: 2018-06-20T13:07:20.029Z Reads: 189

```
if daisy chain canbus is not possible i think yes dual receiver with can sounds ok to me
```

---
## \#276 Posted by: cryo Posted at: 2018-06-20T14:04:14.082Z Reads: 196

```
sorry didn't mean to derail the thread. After googling a bit more seems it is possible just need both receivers to have same address. Will try and report back once i have everything built
```

---
## \#277 Posted by: ervinelin Posted at: 2018-06-20T21:10:44.846Z Reads: 198

```
If this was one way communication yes, but it's 2 way. You might have problems on the transmitter end when both receivers send back telemetry information at the same time.
```

---
## \#279 Posted by: clistpdx Posted at: 2018-07-01T04:38:17.069Z Reads: 188

```
[quote="ervinelin, post:109, topic:48231"]
same copper tape shielding
[/quote]

How do you shield the NRF with copper tape without shorting any components on it? Do you heatshrink it and THEN apply the copper tape over the top?
```

---
## \#280 Posted by: ervinelin Posted at: 2018-07-01T05:00:11.203Z Reads: 199

```
Only the lousier ceramic modules seem to need shielding. I am going without sheilding for the better modules.

I cover it with tape first then copper tape. Copper tape is non conductive on the adhesive side too but the additional tape layer is for additional security
```

---
## \#281 Posted by: mlp Posted at: 2018-07-06T17:57:52.595Z Reads: 210

```
I just got the charger/boost converter. 

I have tested it with the original 1K Rprog and a 3.3K Rprog.

With the 1K resistor I measured the charge current to be approximately 850mA. The Charging module got HOT right away. 

With the 3.3K resistor I measured the charge current to be approximately 380mA. The charging module barley got warm, even after 15 min of charging. 

![ch_bo_resistor_values|440x499](upload://pwKhFEhqNFPL9uHEpd5i99S7Tcx.jpg)


(For calculations and examples) here is the ME4056 charge IC datasheet:
http://www.cnzls.com/PDF/Li-ion%20Battery%20Charger/ME4056_E2.0.pdf
```

---
## \#282 Posted by: Zyb Posted at: 2018-07-06T21:57:05.634Z Reads: 189

```
i messaged aliexpress supplier and they advised me the same thing tho they didnt tell me what size resistor should i use. is it 1206 size in the picture? i think i will go with 5k for the value
```

---
## \#283 Posted by: mlp Posted at: 2018-07-06T22:34:40.339Z Reads: 191

```
I used a 0805 resistor. I believe the 1K I took off also were 0805 sized. (The 250 Ohm resistor in the top left corner is 1206) 

I measured the capacity of the battery I am going to use in the remote to be 800mAh. I figured out that I would be satisfied with ½ a C charge rate/ ≈ 2-hour charge time. I’ll probably do a full charge cycle on the bench, just to make sure it works properly.
```

---
## \#284 Posted by: mlp Posted at: 2018-07-08T19:20:31.350Z Reads: 200

```
I just wired up one receiver and one transmitter using the E01-ML01S. I tested the connection between them using the GettingStarted_CallResponse example in the Arduino IDE. 

I got a stable connection within a few meters.![GETTING%20STARTED%20NRF|690x283](upload://pJOpbKUC3zIq4oYfnXGlQRenrTT.PNG)!


When I then tried to use the esk8 remote codes I could not establish connection. I have only downloaded the code (from here: https://github.com/ModMiniMan/nRF24-Esk8-Remote)  and changed the PIPE, so they matched in both the receiver and transmitter code. Does anyone know what I am doing wrong?

i have tried the following pipe adresses: 0xCABDABABEDLL  0xA8A8FEFEE1LL 0xA8A8F0F0E1LL

I think they are on the same channel' :slight_smile: 

I reinstalled all the libraries, but it did not make any difference.
```

---
## \#285 Posted by: mlp Posted at: 2018-07-12T12:53:52.936Z Reads: 192

```
The problem for me was that the receiver data rate was set to 250KBPS and the transmitter data rate was not. (See line 117 in RX code “radio.setDataRate(RF24_250KBPS);”)

Either removing this line or adding it to the transmitter code works for me. Looks like others are getting better range by setting it to the lower 250KBPS data rate. I’ll have to test that out.
```

---
## \#286 Posted by: rey8801 Posted at: 2018-07-12T21:14:44.496Z Reads: 199

```
Hi! I would like to ask you something. I am at the point to build the receiver part. I followed your advices and I have a mcp120 and a power filter for the servo connection. I would have few questions:
- May I connect the mcp130 chip to the additional  5v GND and Reset at ICSP on Arduino nano? Or I need to use the same 5V GND where the servo cable is connected? I think that I can do it but I want to be sure.
![IMG_20180712_231415|690x388](upload://cevffc45l2jXp4BRFxahKK4pG74.jpg)
- after using the power filter, do you still add the 220uF cap between 5v and GND of the servo connection on Arduino?

Thank you very much. If you have any additional info please share it.
```

---
## \#287 Posted by: Zyb Posted at: 2018-07-13T13:50:44.973Z Reads: 198

```
The whole deal of Mcp is to check if the voltage is above the desired value. So in theory you should be able to connect it to any 5v source. For the 220uf cap I don’t use it, instead I went for the 1000uf to prevent brownouts. @ervinelin had the issue and solved it with 1000uf cap. This is actually a thing in RC world. There are even products like in the picture to solve the issue   ![image|690x471](upload://zI2uZMPFuHzxuRu9wsIOEEve7qh.jpeg)
```

---
## \#288 Posted by: rey8801 Posted at: 2018-07-13T13:58:28.653Z Reads: 200

```
Thanks! I ended like that. I put a power filter along the servo and 5v and ground. 220 cap (if I need higher I can put more in parallel)and a mcp130 micro chip where I shied you before (next time I will buy it the TO-92 version :sweat_smile:)
![IMG_20180713_155509|690x388](upload://jKsfm25dxxYYxxjLBCmYPxGhqIG.jpg)![IMG_20180713_155324|690x388](upload://iduJd62nvIln3LQRigHN399LeAK.jpg)![IMG_20180713_155337|690x388](upload://37QEshHwiQE8ulZseTM62PNPLGg.jpg)

Do yuu know if there is a way to test them without connect them to the VESC? I would like to avoid unmount the enclosure for nothing.
```

---
## \#289 Posted by: Zyb Posted at: 2018-07-13T14:08:58.142Z Reads: 191

```
Looks good, I would just add some hot glue around some of the solder joints. If you can heat shrink the whole thing that would be the best. For testing just connect your receiver from its USB port and power up your remote see if you get a connection. That’s the easiest way. Tho you can’t test if mcp is working unless you power your receiver from vesc. Because you don’t need the mcp if you can power your arduino from its USB port. Bear in mind tho some arduinos work without a problem. In this case adding a mcp functions like a backup plan if anything goes wrong.
```

---
## \#290 Posted by: rey8801 Posted at: 2018-07-13T14:10:48.331Z Reads: 179

```
I am planning to add the hot glue when I see that everything works. FOr the moment if I turn them on I do not see any connection. Do I have to write the pipe line address in the reciver code?
```

---
## \#291 Posted by: Zyb Posted at: 2018-07-13T14:13:39.749Z Reads: 188

```
Yea make sure pipe addresses match on both receiver and transmitter code otherwise they won’t connect
```

---
## \#292 Posted by: rey8801 Posted at: 2018-07-13T14:15:56.783Z Reads: 203

```
Address on the Transmitter and the address in the receiver code. Are they the same? The 0x....LL matter or not? 
![IMG_20180713_161405|690x388](upload://ix7w0lYJFtOpPt9bKniZkkSzGMl.jpg)![IMG_20180713_161410|690x388](upload://hniX7PLCDJxzERLRAuFqZoaTC59.jpg)
```

---
## \#293 Posted by: Zyb Posted at: 2018-07-13T14:21:37.050Z Reads: 196

```
They should be identical, I would check the transmitter code aswell and make sure they are absolutely identical. Use copy paste command to be sure :slight_smile:
```

---
## \#294 Posted by: rey8801 Posted at: 2018-07-13T14:22:49.252Z Reads: 197

```
I checked now and they are the default ones and are identical. To see that they connected I guess you have to see that the symbol on the screen stops blinking, right?

This one the libraries and sketches I used:
I used https://github.com/RollingGecko/VescUartControl/tree/VESC6 the VESC6 branch plus U8g2lib.h, rf24.h on both transmitter and receiver.
```

---
## \#295 Posted by: Zyb Posted at: 2018-07-13T14:29:51.662Z Reads: 198

```
Yes it should be still. Before coming to conclusion try different codes like original firefly code and then @ervinelin s code. Make sure you installed libraries correctly. If you still can’t make it work then check you solder connections make sure every connection is correct with a multimeter. In the past I had a bad nrf module or I fcked it up I dunno but when I swapped it with a new one I got a connection.

Yea they seem right I think they were written somewhere in solidgeeks build guide.
```

---
## \#296 Posted by: ervinelin Posted at: 2018-07-13T14:34:36.687Z Reads: 190

```
If it connects the little wifi icon should not be blinking. You can also set the transmitter or receiver to be in debug mode then use the Arduino serial monitor to see if it's working.
```

---
## \#297 Posted by: rey8801 Posted at: 2018-07-13T14:41:17.849Z Reads: 193

```
@zyb @ervinelin Good news that with your Esk8 program it works and connects. Now I need to get it work with the solidgeek one.
```

---
## \#298 Posted by: rey8801 Posted at: 2018-07-13T14:49:48.231Z Reads: 224

```
At leat I know that the connection are fine but now to be sure I dowloaed the file again from https://github.com/SolidGeek/nRF24-Esk8-Remote/tree/development DEVELOPMENT branch. SHould I use MASTER?

Add these libraries:
I used https://github.com/RollingGecko/VescUartControl/tree/VESC6 the VESC6 branch plus U8g2lib.h, rf24.h on both transmitter and receiver.

Trasmiter went fine. With the receiver I get this error message:
I know that it's not your software but since you worked on it maybe you know it. Thanks a lot.

Arduino: 1.8.5 (Windows 7), TD: 1.41, Board: "Arduino Nano, ATmega328P"

C:\Users\Administrator\Downloads\nRF24-Esk8-Remote-development\receiver\receiver.ino: In function 'void setup()':

receiver:144: error: 'SetSerialPort' was not declared in this scope

       SetSerialPort(&Serial);

                            ^

Multiple libraries were found for "buffer.h"
 Used: C:\Users\Administrator\Documents\Arduino\libraries\VescUartControl-master
 Not used: C:\Users\Administrator\Documents\Arduino\libraries\VescUartControl-VESC6
 Not used: C:\Users\Administrator\Documents\Arduino\libraries\VescUartControl-VESC6
 Not used: C:\Users\Administrator\Documents\Arduino\libraries\VescUartControl-VESC6
 Not used: C:\Users\Administrator\Documents\Arduino\libraries\VescUartControl-VESC6
exit status 1
'SetSerialPort' was not declared in this scope

This report would have more information with
"Show verbose output during compilation"
option enabled in File -> Preferences.

![IMG_20180713_165317|690x388](upload://5fU2BC8fAtqwL9JQo5T3HNsbeFI.jpg)
```

---
## \#299 Posted by: mlp Posted at: 2018-07-13T15:08:33.336Z Reads: 196

```
@ervinelin Did you manage to get telemetry to work with Ackmaniack 3.1 firmware? Which VESC firmware are you currently using?
```

---
## \#300 Posted by: ervinelin Posted at: 2018-07-13T17:15:29.712Z Reads: 201

```
I never managed to try. I am just using the latest regular vesc firmware.
```

---
## \#301 Posted by: ervinelin Posted at: 2018-07-13T17:17:22.197Z Reads: 214

```
Oh this problem... I managed to resolve it by adjusting some of the code, you can see the way I declare the serial port in my code is different from solid geeks if I am not mistaken.

I got the tip from someone within solidgeeks remote thread.
```

---
## \#302 Posted by: rey8801 Posted at: 2018-07-13T17:20:55.519Z Reads: 229

```
Solved. I didn't delete the VESC master library adn IDE was loading that one instead of the VESC6 one. Thanks for the help!
```

---
## \#303 Posted by: rey8801 Posted at: 2018-07-15T13:52:39.429Z Reads: 237

```
I just want to report it back since I do not know if someone tried before but I used this antenna (https://www.aliexpress.com/item/CDEBYTE-2PCS-Lot-SPI-SMD-Module-E01-ML01S-2-4GHz-0dBm-110m-nRF24L01-Wireless-RF-transceiver/32803028476.html?spm=a2g0s.9042311.0.0.731b4c4dT34h7Y) on both receiver and transmitter. I can share that I rode for the past 2 days without any signal drop. I get a stable connection within 5 meters with obstacle and walls, probably outside is more but didn't try it the max range. More than 5m it starts to becoming unstable. Not to bad for esK8. I am just wondering what for instance a nano-X is using since I can go in other rooms on the other side of the apartment and still have signal. Hope it helps!
```

---
## \#304 Posted by: Linny Posted at: 2018-08-14T15:08:42.605Z Reads: 236

```
Does anyone use Torqueboard's VESC with this remote? Any idea which pins to plug the Rx and Tx to? Currently unable to get telemetry.

![39161496_1898588123782191_7371115442825330688_n|275x500](upload://xINVmD3f7nUXwuVQL30wFgVOCpC.jpg)
```

---
## \#305 Posted by: clistpdx Posted at: 2018-08-14T22:48:25.087Z Reads: 226

```
@Zyb I finally got your PCB's in the mail from JLC (I chose the cheap shipping...big mistake) and I'm looking at your 'FinalSMD' pcb and making sense of all the ins and outs before I begin soldering. I think I have everything identified except the 'I/O' ports in the corner. It's been so long that I can't recall where/what these connect to. **Can you remind me what the I/O pads connect to?**
```

---
## \#306 Posted by: Zyb Posted at: 2018-08-15T09:25:41.231Z Reads: 231

```
@clistpdx its ok ask anything which is not clear because i kinda made it without making the circuit first :) i/o is simply where you connect your on/off switch. it is the universal on off sign you may see it around on some electrical devices. USB is for charging usb port mind the polarity. also be careful when soldering the battery cable because i shorted it for a second and board got ruined somehow. i should have made bat holes abit far away from each other just to be safe.
```

---
## \#307 Posted by: Jansen Posted at: 2018-08-16T21:12:30.488Z Reads: 225

```
I didn't have time to read the rest of this form from where I left off the other day but does anyone here want to make a little extra cash by making me one of these remotes....? Happy to compensate what your time and skills are worth. I am just not super handy with this stuff and am really buys with work so don't have enough free time to try and learn. Would really appreciate more than you know. PM me or hit me back here.

Thanks so much in advance, really do appreciate anyone who can help me out! Ready with paypal payment ASAP! I live in SoCal if that makes any difference at all.
```

---
## \#308 Posted by: riverside.rider Posted at: 2018-08-17T07:00:39.669Z Reads: 210

```
Same for me: would also like to buy this ready-to-roll remote control with the aforementioned component fixes. Kindly pm me with an offer ($$$)
```

---
## \#309 Posted by: mishrasubhransu Posted at: 2018-08-31T10:41:26.150Z Reads: 213

```
So @ervinelin and @Zyb , what final nrf do you suggest now?

Also Zyb is your rx different from ervinelin's receiver?
```

---
## \#310 Posted by: ervinelin Posted at: 2018-09-03T05:47:44.168Z Reads: 213

```
E01-ML01S small size SPI nRF24L01P 2.4Ghz 1mW PCB antenna IOT uhf wireless transceiver(transmitter/receiver) module
 http://s.aliexpress.com/ZnAZj2em?fromSns=Copy to Clipboard

I currently use this, or the version which requires an external antenna. So far this has proven to be effective without having to resort to the weird copper tape shielding of the other modules.
```

---
## \#311 Posted by: ivanflo Posted at: 2018-09-15T00:43:22.758Z Reads: 188

```
Out of pure laziness. Is anyone selling something like this off the shelf?
```

---
## \#312 Posted by: Zyb Posted at: 2018-09-15T08:09:34.973Z Reads: 194

```
just a tad different. theres a place for 1000uf cap for 5v also 100uf, 10uf and 100nf for 3.3v and place for mcp130 chip other than that its the same and yes like @ervinelin suggested that chip works ok for me too tho im using it with combination of this one https://www.aliexpress.com/item/2-4GHz-rf-Wireless-uhf-Module-Power-Amplifier-E01-ML01SP4-Original-SENET-1-8km-2-4g/32806320077.html?spm=a2g0s.9042311.0.0.27424c4dAN0H5T and they work great with one another
```

---
## \#313 Posted by: ervinelin Posted at: 2018-09-18T04:07:51.235Z Reads: 178

```
One point to note about the chip with the external antenna... MAKE SURE THE ANTENNA DOESN'T FALL OFF! Also make sure you get the right kind of antenna (2.4GHz), there are other frequencies that might fit but will be the wrong antenna.

Doing so might fry the chip.

I would recommend sticking to the inbuilt antenna version for better piece of mind.

Erv.
```

---
## \#314 Posted by: dastsong Posted at: 2018-10-05T17:36:03.314Z Reads: 176

```
I am also using this VESC. Have you been able to get telemetry working? You are probably connecting to the correct pins. I used oscilloscope to read the same Tx and Rx pins while the receiver is connected, and was able to see the uart packets. However the receiver is probably not sending them out back to the remote. It seems that telemetry only work on VESC6, not 4.12
```

---
## \#315 Posted by: Linny Posted at: 2018-10-05T17:38:00.636Z Reads: 180

```
Unfortunately no. I'm still using the remote but everything's in 0s. I'm going to try it on focboxes with the latest firmware and try it again.
```

---
## \#316 Posted by: dastsong Posted at: 2018-10-05T17:53:43.821Z Reads: 180

```
same here. going to build a new one with better nRF module and get a FOCBOX. Have you got your FOCBOX from enertion too?? I ordered mine in August and was told it will be shipped in November......

Oh I just realized, you probably mean the single FOCBOX... Mine was FOCBOX unity.... It is still in production
```

---
## \#317 Posted by: Linny Posted at: 2018-10-06T00:45:39.856Z Reads: 180

```
Yep I got two normal focboxes. Ordered it in late June and just got it recently 🤣

Also got a unity and am waiting for it too. Perhaps it's a firmware or torqueboards ESC issue.
```

---
## \#318 Posted by: ervinelin Posted at: 2018-11-22T00:42:07.362Z Reads: 192

```
![IMG20181121205621|281x500](upload://lXDPydNzxH9CHZXjZBEczKzoulO.jpeg) 
Just an update after months of not changing anything...

I am redesigning the remote and PCB to use the Adafruit Feather board instead. This makes it 10x easier than before to build simply because it has both inbuilt lipo charger and regulators.

![IMG20181122001248|281x500](upload://hTtYpnMZ5lZT3DU2DqlgWrKsfnF.jpeg)

 Instead of direct soldering I am using jst plugs because they just make life easier, it also comes with wires so all I need is to trim then down to length.

![IMG20181122001252|281x500](upload://ywAYZ6u1W9MnnRG8pUtq1i6p9Kw.jpeg) 

Instead of the feather that has an inbuilt 900+mhz radio module, I opted to stick with my tried and tested 2.4gHz NRF module. 2.4 being more commonly allowed. Also the bare bone feathers are cheaper.

![IMG20181122025836|281x500](upload://yRY70KlFpcu5bTb9V4oZOZ27HAd.jpeg) 

I made some critical mistakes. The first, for some reason I cut the PCB to fit a Feather m0 but what I actually bought were feather 328Ps! Thankfully all I needed was two short jumpers to correct the pin order.

Another issue was that the 328P feathers did not boot properly for me, same with some other people online. So I had to use a USBasp to reflash the bootloader with the Arduino equivalent.

![IMG20181122025038|281x500](upload://cOo3KzOiZGp7PaWNf43DaIYhKpw.jpeg) 

Once that was done, the rest was smooth sailing. JST connectors made it super easy to hook things up to test. The OLED also works on 3.3V so I didn't need a stepup.

Still some assembly required but much much cleaner and easier than before.

That's all for now.

I will share the files once I have fully built and tested the remote.
```

---
## \#319 Posted by: butt_stallion Posted at: 2018-11-22T02:00:10.502Z Reads: 170

```
Planning on building this remote in the future, can't wait to see how this upgrade tests out.
```

---
## \#320 Posted by: ervinelin Posted at: 2018-11-22T17:13:49.418Z Reads: 181

```
More updates...

![IMG20181122234016|281x500](upload://v0XJhmZ9qphnwEmhCsyvkACiesC.jpeg) 
Removed pins from OLED and soldered it directly... Luckily this runs off 3.3V so I didn't need a step up reg.

![IMG20181122234756|281x500](upload://yYrcYOuWMe3n83pJcuyF4NuXgE1.jpeg) 
Had to use this 3 way power switch because to turn off the feather you need to ground the En pin instead.

![IMG20181122235029|281x500](upload://y68nsCW19VKCOQDqG3xg2CXjpKo.jpeg) 
Everything fits just nicely... 

![IMG20181123000420|690x388](upload://1kHqP0ofHNZZqv14pz4XSFqivpC.jpeg) 
Swapped to a 3.3V hall sensor instead of the original 5V one so that everything just runs off 3.3v including the NRF module and the OLED.

![IMG20181123004627|281x500](upload://iLsQa9sAZfUXPO095hEWz8Ur6sj.jpeg) 
Neat AF compared to my previous version!! Might extend the wires for the on off and mode switches to run under the PCB instead of across it. That weird yellow blob on the right part of the PCB antenna.

![IMG20181123010426|281x500](upload://rQnfShPUq8pd1QhKguyIrv2lKeQ.jpeg) 
Switches work. Telemetry works. Throttle needed some calibration but also works.

![IMG20181123012305|281x500](upload://xX06RFY72r5mYgkSr6fBigXXnN.jpeg) 
Old versus new version... The difference really is in the ease of building.. the new one is much much easier. Not to mention less components.

Had problems with my 3D printer so the casing is really poorly printed... Getting it reprinted by professionals...

Now will need to test ride to know if there are problems but I am quite confident it will be fine.
```

---
## \#321 Posted by: rene Posted at: 2018-11-22T17:48:01.790Z Reads: 165

```
@ervinelin Great! I got all parts lying around for months to build your version, but was not proceeding because it would take some evenings.

But with the new version - wow. 
Happy to get the full parts list to order!

THX!
```

---
## \#322 Posted by: ervinelin Posted at: 2018-11-22T17:55:55.461Z Reads: 166

```
Yup you can quite easily do this in an evening... I took two because I had problems flashing the board and i had to work around my mistakes with the PCB.

Also, soldering the NRF and JST plugs is a real pain... But the JST plugs and cables just make it super easy to install...

Oh and the switches now are literally drop in. My previous version with the limit switch was a real pain to adjust till you got it just right...
```

---
## \#323 Posted by: Zyb Posted at: 2018-11-23T01:34:44.432Z Reads: 157

```
awesome update, ive been thinking to do the same thing and only thing that bothered me was the hall sensor. can you tell me which one did you  use specifically?
i found this one Unisonic Tech SK1816G-G03-K claims to be working in range 2.5-20V but never tried it.
```

---
## \#324 Posted by: Zyb Posted at: 2018-11-23T01:37:54.319Z Reads: 160

```
also wanted to add that this battery fits very well into your case design. https://hobbyking.com/en_us/turnigy-nano-tech-750mah-1s-35-70c-lipo-pack-fits-nine-eagles-solo-pro-180.html
```

---
## \#325 Posted by: ervinelin Posted at: 2018-11-23T01:41:41.608Z Reads: 161

```
I'm using this sensor... I got the link from somewhere in the forum that was also looking for a 3.3V hall sensor.

https://www.aliexpress.com/item/10-pcs-Hall-Element-49E-OH49E-SS49E-Linear-Hall-Switch/1903819684.html?spm=a2g0s.9042311.0.0.27424c4dsXsvRf
```

---
## \#326 Posted by: ervinelin Posted at: 2018-11-23T01:42:40.252Z Reads: 165

```
good to know!

I just happened to stock up on a few 18350s but I can understand that it's not a common cell to find.
```

---
## \#327 Posted by: Zyb Posted at: 2018-11-23T02:35:45.488Z Reads: 168

```
Thanks for the info appreciate it.
It’s a good battery and I tested it it’s exactly 750mah as advertised. Way better than those no name batteries also you don’t have to modify the resistor with this one. As it can take 2c charge rate which is around 1.4A. Size wise that’s as much as it can go before touches any moving parts.![image|375x500](upload://15dI5ZJs4YKDBJIZIJ9Pg3W9lG1.jpeg)
```

---
## \#328 Posted by: ervinelin Posted at: 2018-11-23T02:46:03.427Z Reads: 165

```
that's pretty sweet... wire routing? Just go over the lipo?

I also like how you added what looks like a CF rod for additional support!

I did beef up some of the smaller parts in my latest design, also added another 0.5mm to the shell to make it a little sturdier. The plan was also to print it in a better material...
```

---
## \#329 Posted by: Zyb Posted at: 2018-11-23T03:14:39.513Z Reads: 161

```
oh its not thick theres enough space to double stack that battery and its not a bad idea lol, i would route everything under the battery. before i started printing my own cases i ordered it from someone else and first and only thing that snapped was that pillar holding the spring. so i just made a beffy cylinder and tap m4x20mm steel grub screw in there :)) strong as hell.
yea thickness would definitely help but layer adhesion is probably the most important thing. if it is good enough your design is good as it is. another thing i changed was the interlocking system. i printed around 3-4 sets and they all failed on that point where the case has thinner walls in order to interlock to each other. so i just made it thicker and created tabs on the top half to the inner walls without sacrificing from the wall thickness. pretty much like how firefly interlocks top and the bottom.
```

---
## \#330 Posted by: ervinelin Posted at: 2018-11-23T03:33:58.570Z Reads: 163

```
Ah, I thickened the lip (interlock) just because someone complained that their printer had trouble printing it... (was it you?)

In any case it now fits very well and is easier to print too... 

Let me know how your 3.3V hall sensor works out for you, one issue I had was it seemed that the sensitivity is different from the 5V one, which required me to adjust the end points via the remote. Seems to work okay now.

I also adjusted the magnet positions on the trigger. Previously before you pull the trigger completely it would already be at max throttle, i.e. the full throw of the trigger was not utilised. I have since changed this such that the full throw is now registered.
```

---
## \#331 Posted by: ervinelin Posted at: 2018-11-23T09:12:32.291Z Reads: 162

```
The parts list is here:

[Parts List for V2 Remote Transmitter](https://docs.google.com/spreadsheets/d/16yFgw0h830DYDCNLdNoN9N3cgaNEd7jQIoZ__qk-8wo/edit?usp=sharing)

I haven't changed the receiver for now.
```

---
## \#332 Posted by: Zyb Posted at: 2018-11-23T09:26:22.181Z Reads: 160

```
it wasnt me :) printing is no issue it actually prints beautifully but the strenght of it was the problem. i think i will have a bigger issue with installing a bootloader on it. it uses atmega32u4 chip right? if yes then probably need to go with arduino leonardo bootloader?
```

---
## \#333 Posted by: ervinelin Posted at: 2018-11-23T09:27:25.443Z Reads: 153

```
328p... arduino pro/pro mini 3.3v bootloader..

Was a real pain to do so without the right rig...
```

---
## \#334 Posted by: Zyb Posted at: 2018-11-23T09:32:14.903Z Reads: 149

```
Oh ok for some reason I thought you had basic proto model. I blame the coffee.
```

---
## \#335 Posted by: Zyb Posted at: 2018-11-23T09:38:45.220Z Reads: 156

```
Forgot to mention, that hobby king battery connector probably won’t fit into a normal jst housing. It took me a while to figure out what it is. Turns out it’s a molex connector. Here is the male end.. could be used to make small molex to jst cable or can be soldered where needed. In my case I shortened the cable and soldered it to the board. 
https://s.click.aliexpress.com/e/bkqQlxvO
```

---
## \#336 Posted by: rene Posted at: 2018-11-23T10:42:58.498Z Reads: 152

```
Thanks!

Do you also got an update on the PCB Link to order?
And Thingyverse for the Case
```

---
## \#337 Posted by: ervinelin Posted at: 2018-11-23T10:58:29.763Z Reads: 152

```
Still testing... So not releasing it just yet...

Had some strange issue today when I was testing... I rode around perfectly fine... But then when I wasn't holding the remote I would lose connection. Need to figure out what's wrong.
```

---
## \#338 Posted by: totalgeek9224 Posted at: 2018-11-23T11:01:33.642Z Reads: 155

```
Sounds like a lose connection (maybe) When you hold it it puts pressure against a wire or connector and when you let go theres not enough contact 

all speculation :)
```

---
## \#339 Posted by: Zyb Posted at: 2018-11-23T11:15:15.666Z Reads: 154

```
i had the same issue, for some reason same setup and everything is not behaving identical on the second remote. when the cable of the antenna makes a good contact with the top metal shield of the nrf module signal is kinda getting boosted. so try that and tape or glue it, you should get good result. to eliminate that issue i started to avoid putting nrfs with antenna in the remote side. sometimes it just doesnt work.
```

---
## \#340 Posted by: ervinelin Posted at: 2018-11-23T17:24:33.152Z Reads: 155

```
So I thought I had to do something a bit crazy like remove and replace the NRF module...

In the end all I did was flip the antenna. 

But I agree, might not be worth the trouble, will build the next one without antenna.
```

---
## \#341 Posted by: Zyb Posted at: 2018-11-23T17:49:19.537Z Reads: 162

```
interestingly receivers with antenna has no issues for me and having at least one side with antenna is a big boost for signal. so, remote without antenna and receiver with antenna is good enough.
i never tried this module so far http://www.ebyte.com/en/product-view-news.aspx?id=113 it seems to be giving the freedom to choose between with or without antenna. its just abit longer(25mm) than their products. i might give it a go in the future see how it does in practice.
```

---
## \#342 Posted by: ervinelin Posted at: 2018-11-23T18:32:37.381Z Reads: 175

```
![IMG20181124020223|281x500](upload://lyKfarNTnVPeFiZ0u8h7s3lICqu.jpeg) 
I rigged up a little bootloader flashing jig, takes a bit of wriggling to get the pins to contact properly on the pads but I did manage to reflash another two feathers.

Really no idea why these feather boards are so problematic to work with...
```

---
## \#343 Posted by: Zyb Posted at: 2018-11-23T20:02:19.397Z Reads: 165

```
ive seen people use other arduinos as their programmer is that not possible?
```

---
## \#344 Posted by: ervinelin Posted at: 2018-11-23T23:46:41.150Z Reads: 163

```
Yes that's called ArduinoISP I think. Possible, but I had the USBasp stick so it's just easier...
```

---
## \#345 Posted by: Hoxtible Posted at: 2018-11-24T02:09:08.781Z Reads: 175

```
Could anyone build one of these for me? I would be willing to pay.
```

---
## \#346 Posted by: StefanMe Posted at: 2018-11-24T11:37:14.490Z Reads: 184

```
I showed up this Sensor... I use it in my [FeatherRemote](https://www.electric-skateboard.builders/t/featherremote-and-smartremote/74084) and it works great. Range goes from 790 to 275. Good range on 3.3v
```

---
## \#347 Posted by: ervinelin Posted at: 2018-11-24T13:25:27.907Z Reads: 186

```
That's about range I am getting too for the 3.3V hall sensor.

![IMG20181124180301|690x388](upload://tBbRwmjO8Q11ClTtcJqFYS8CrHI.jpeg)

Rode 25km with the new remote without any issue.... now to wait for the better 3D print from my friend...
```

---
## \#348 Posted by: StefanMe Posted at: 2018-11-24T14:13:43.439Z Reads: 181

```
Looks cool! I would love to put my code into this thing :wink:
```

---
## \#349 Posted by: ervinelin Posted at: 2018-11-24T15:12:21.631Z Reads: 182

```
Sure why not... My code is super outdated now... Still works so I haven't bothered to change it..
```

---
## \#350 Posted by: ervinelin Posted at: 2018-11-24T15:17:51.064Z Reads: 197

```
![IMG20181124144213|281x500](upload://yIlUJl0xPyxEeUK8K5qCfbQ4B1c.jpeg) 

![IMG20181124144218|281x500](upload://oM9SJwZTQCBlPzWuOq3NkuW6YEC.jpeg) 

I am hoping to get rid of the LC filter and cap that I currently use to clean up the 5v from the ESC. So I incorporated some of it to the new Rx PCB.

One big caveat... I don't really know if I am doing this right... But so far it seems to connect so that's a good step.
```

---
## \#352 Posted by: Boeufsk8 Posted at: 2018-11-29T14:09:02.617Z Reads: 172

```
Any luck getting @Ackmaniac's software to work with telemetry ?
```

---
## \#353 Posted by: ervinelin Posted at: 2018-11-30T01:25:00.095Z Reads: 178

```
Was planning to give it a go soon... No idea if it works for now
```

---
## \#354 Posted by: ervinelin Posted at: 2018-11-30T18:40:21.702Z Reads: 181

```
![IMG20181201022404|281x500](upload://87hzwYPgKHxrBjYXkyu2Fqz9Jl.jpeg) 

Building my second remote for a friend... Damn this is so much easier than the old version! I was done with the main PCB soldering in about an hour...

![IMG20181201020213|281x500](upload://x3IS2Y9qa5cTyKCsihxoaFvsVn.jpeg) 
This time I laid the NRF module flat against the PCB... Previously it was lifted by the pin holder plastic things. What I didn't realise was the antenna plug would make it too thick to fit properly into the remote... Laying it flat should do the trick.
```

---
## \#355 Posted by: Mich21050 Posted at: 2018-11-30T18:51:06.775Z Reads: 171

```
Any idea when you will release the new version? :smile:
```

---
## \#356 Posted by: ervinelin Posted at: 2018-12-01T01:00:20.510Z Reads: 172

```
Few more changes to the design and I should be all good
```

---
## \#357 Posted by: ervinelin Posted at: 2018-12-04T13:17:00.404Z Reads: 178

```
![IMG20181204205109|281x500](upload://aK390L5XW0nqKsChdQccaLBsNvH.jpeg) 

Latest version uses M3 screws to reinforce the weak parts
```

---
## \#358 Posted by: ervinelin Posted at: 2018-12-05T17:03:53.368Z Reads: 171

```
Capacitor array seems to work, I can do without the external LC filter it seems...

Telemetry also works with the latest VESC firmware (Ackmanics not tested)...
```

---
## \#359 Posted by: ervinelin Posted at: 2018-12-07T02:23:59.854Z Reads: 172

```
![IMG20181206130218|281x500](upload://sVctet3YsXgnHT5JaBajdaf9XyS.jpeg) 

Sent these for print only to change the design after.... Now have to reprint the new design... Groan...

BTW the new version with the M3 screws has been tested... So far so good...
```

---
## \#360 Posted by: ervinelin Posted at: 2018-12-07T10:08:13.087Z Reads: 171

```
![IMG20181207180453|690x388](upload://dmjorogyBqEQe8J2aez9l3kA8L1.jpeg) 

Close up look at the use of the m3 screws to beef things up...
```

---
## \#361 Posted by: rayn Posted at: 2018-12-09T11:42:36.388Z Reads: 176

```
@ervinelin Thanks for the guide and the parts! Mine's finally, finally done. Made some mods:

* 128x64 screen instead of 128x32
* Pot from junk rc remote control instead of hall sensor
* Arduino Fio I had lying around
* Screen orientation is different for both left and right hand usage
* Shape is different, the flatter shape lets you hold it with wrist guards comfortably

Also changed the code around a bit, each packet transmission is done with timer ISR at ~50ms intervals now. 

![DSC_0738|690x276](upload://wDhbJu2ugD7Ek2ZxeadueW114zH.jpeg) 
![DSC_0739|690x336](upload://4Yz3S4yPyBvMV58RsHxjqXkUOx2.jpeg) 
![DSC_0741|367x500](upload://arrKUosC8MkG1yqXVNO5l0zDPpJ.jpeg)
```

---
## \#362 Posted by: ervinelin Posted at: 2018-12-10T17:35:56.483Z Reads: 178

```
![IMG20181211003151|281x500](upload://2X8yOEOaBbqSFp2Qkw1xlr850Lg.jpeg) 

Transplanted my electronics into the new casing only to realize I made a small mistake with the wrist strap attachment area... Had to file in a small depression for it..

![IMG20181211012259|375x500](upload://16Jey2ZR6xQdvdp2P3PBRcaHJVr.jpeg) 

![IMG20181211012328|375x500](upload://6yWxrp0oSSHEeHKTQRcDwGHPk3A.jpeg) 

![IMG20181211012340|375x500](upload://ptMr6Hp2Bhh3iZeS1cNmVdJw59b.jpeg) 

Sprayed some 2 part epoxy truck bed liner in hope of creating a more robust casing... Not sure if I like the speckled texture just yet..

It doesn't scratch my hands, adds somewhat of a nice grip but looks a bit too rough...
```

---
## \#363 Posted by: ervinelin Posted at: 2018-12-21T04:23:58.813Z Reads: 169

```
![IMG20181221121634|690x388](upload://bcjOpcnMydHK2Ic0PdOlyxg1jgU.jpeg) 

Redesigned the receiver to be enclosed in a printed casing instead of just heat shrink.
```

---
## \#364 Posted by: ervinelin Posted at: 2018-12-21T08:33:09.295Z Reads: 173

```
![IMG20181221162832|281x500](upload://jiGLctZ9OuTGOOvpsQGjjrgW0yR.jpeg)t

Tried to print some text to show the pinouts... Not super clear but I suppose good enough..

![IMG20181221162848|281x500](upload://rWu7U9IxP5PbfmNwSQn0vkeNYav.jpeg)
Case is held together by 4 screws which in turn also holds the PCB down.
```

---
## \#365 Posted by: totalgeek9224 Posted at: 2018-12-21T09:39:22.194Z Reads: 163

```
Why dont you do a write up for this on a seperate thread so those who would like to do the same could do so? Also, how are you finding the power switch location? Does it ever get accidentally switched?
```

---
## \#366 Posted by: rayn Posted at: 2018-12-21T17:15:27.856Z Reads: 167

```
I do actually intend to do that but I'm still trying to get things organised. I've started a build thread for the entire project [here](https://www.electric-skateboard.builders/t/first-build-a-pushable-drop-through-gear-drive-the-dilettante-bustin-maestro-6-83mm-abec-11-caliber-ii-50s-diy-geared-drive-turnigy-esk8-esc-10s2p-sony-vtc6-diy-3d-printed-enclosure-diy-remote/78633), it'll get filled in slowly as I find the time to write what I did down. 

The switch location is great and does not accidentally get pressed... but possibly only for me. I printed a whole bagful of shapes to get things fitting my hand nicely.
```

---
## \#367 Posted by: Arzamenable Posted at: 2018-12-22T08:24:26.769Z Reads: 170

```
Great coating. I put pistol grips on mine at one point. ![image|500x500](upload://yEUhjA634lCYEDYfpUGyHUNxdXX.jpeg)
```

---
## \#368 Posted by: ervinelin Posted at: 2018-12-24T09:00:14.859Z Reads: 177

```
![IMG20181224144908|281x500](upload://5SR8YyK9CreCAdYqCz7v845Q0HW.jpeg) 

![IMG20181224155305|281x500](upload://iO1HDtlF5TQdUmKLNEu6LHNg8Ha.jpeg) 

![IMG-20181224-WA0023|666x500](upload://qjKJkxxTxd9BaiS5m2D08oKUPup.jpeg) 
Building a very small batch of remotes for friends...

Hope I have enough parts for everything
```

---
## \#369 Posted by: ervinelin Posted at: 2018-12-30T16:28:13.888Z Reads: 167

```
![IMG20181230174807|281x500](upload://o0awE3sW1peH578e7gU1YNpPcLd.jpeg) 

![IMG20181230234845|690x388](upload://18WdkJs9NNee4KWLW2OiLIOcsiB.jpeg) 

![IMG_20181231_002943|690x387](upload://73fFevsCdQarY8BUO85Uof4JgaS.jpeg) 

Urgh.. so much work!!
```

---
## \#370 Posted by: Blix Posted at: 2018-12-30T16:32:35.908Z Reads: 157

```
The red one looks awesome!
```

---
## \#371 Posted by: ervinelin Posted at: 2018-12-30T16:33:01.693Z Reads: 157

```
That's mine... Haha...
```

---
## \#372 Posted by: StefanMe Posted at: 2018-12-30T16:36:38.065Z Reads: 160

```
the masters one :slight_smile:

nice work!
```

---
## \#373 Posted by: ervinelin Posted at: 2018-12-30T16:37:28.587Z Reads: 161

```
Still not done yet... one last layer of 2k clear coat!
```

---
## \#374 Posted by: Adstars Posted at: 2019-01-05T19:21:21.310Z Reads: 161

```
Looking good!
```

---
## \#375 Posted by: FalconNL Posted at: 2019-01-09T21:59:33.161Z Reads: 159

```
Any idea when you will release the new version?
```

---
## \#376 Posted by: ervinelin Posted at: 2019-01-09T22:55:33.367Z Reads: 162

```
In a week or two... Planning some last few micro changes after I realised some issues in the latest prints ..
```

---
## \#377 Posted by: ervinelin Posted at: 2019-01-13T17:19:17.033Z Reads: 172

```
![IMG20190113152559|690x388](upload://mSYVD0dAw4KoQhXIDhiiySiMf0R.jpeg) 
Started building the small batch of remotes finally..

![IMG20190113160642|281x500](upload://iYXly4SFXXmrkc4lsbS2TVehbYW.jpeg)
SLA casing with HP fusion parts

![IMG20190113160651|281x500](upload://6Vb6O5m5mRX9nFy064Wnw5Ydkgv.jpeg) 
Made a mistake with the polarity, fried one board's charging circuitry... Sigh

![IMG20190113161632_1|281x500](upload://fyNkatRmJ8zDYbkTv6eN6pV900m.jpeg) 
Got longer wires to route under the PCB for an even cleaner look..

![IMG20190113163600|690x388](upload://8SpC9KucC7PfkwDYztpk6ELVH2Q.jpeg)  
Sprayed with metallic grey paint and 2K clear coat.

![IMG20190114001735|281x500](upload://5n5KDwVbAXe7OCqXAVzbnh1FTeY.jpeg) 
Built my red one as well...

![IMG20190114001815|281x500](upload://6lvHvbgqI1BWTpNeDXOXHmnbUXi.jpeg)
Different generations of the same thing..
```

---
## \#378 Posted by: Indiangummy Posted at: 2019-01-13T17:44:26.025Z Reads: 162

```
Are selling these or are these just for you?
```

---
## \#379 Posted by: totalgeek9224 Posted at: 2019-01-13T21:08:32.965Z Reads: 163

```
Looks good!
```

---
## \#380 Posted by: ervinelin Posted at: 2019-01-14T01:00:36.499Z Reads: 158

```
Only made a few extras for friends... Too much time needed to build one even after I simplified the PCB.
```

---
## \#381 Posted by: Mich21050 Posted at: 2019-02-04T12:09:48.603Z Reads: 158

```
Any updates on the new feather version? :slight_smile:
```

---
## \#382 Posted by: ervinelin Posted at: 2019-02-04T12:20:14.193Z Reads: 157

```
Sorry I been so tied up with work and family... Files are all ready to be shared I believe.. give me some time to upload everything
```

---
## \#383 Posted by: sanderfu Posted at: 2019-02-05T12:45:21.573Z Reads: 153

```
Have scrolled through the thread today, amazing work! Was wondering if you could update the link for the 1000uF Capacitor as it is currently linking to JST Connectors in the V2 of the parts list :-)
```

---
## \#384 Posted by: ervinelin Posted at: 2019-02-06T02:54:11.215Z Reads: 156

```
Ok let me look into it shortly... Chinese New Year now so even more busy with family stuff than before...
```

---
## \#385 Posted by: lazerusrm Posted at: 2019-02-11T03:26:26.611Z Reads: 154

```
Do you have any PCB's around? id like 3 or 4 if you do.
```

---
## \#386 Posted by: Ruubie200 Posted at: 2019-02-11T09:28:45.824Z Reads: 156

```
is it posible to make a remote without the pcbs?
```

---
## \#387 Posted by: ervinelin Posted at: 2019-02-11T09:46:01.462Z Reads: 158

```
Better off just ordering them from EasyEDA.
```

---
## \#388 Posted by: ervinelin Posted at: 2019-02-11T09:47:00.468Z Reads: 162

```
Yes, but you will go crazy soldering 1001 wires to each other. Also there's always a higher risk of one of the wires dislodging.

My first remote was like this (see first post).
```

---
## \#389 Posted by: Chrisjarram Posted at: 2019-02-22T11:32:43.777Z Reads: 147

```
@ervinelin great remote! Don't suppose you have the original cad files posted somewhere so I can remix for a colour oled?  Will happily make the update available. 

Cheers
```

---
## \#390 Posted by: ervinelin Posted at: 2019-02-22T11:37:23.773Z Reads: 148

```
PM me direct
```

---
## \#391 Posted by: Chrisjarram Posted at: 2019-02-22T12:34:52.738Z Reads: 150

```
Pm'd. Cheers
```

---
## \#392 Posted by: Leander Posted at: 2019-02-28T19:55:26.812Z Reads: 152

```
Hello, was just wondering if you could use the Adafruit Feather HUZZAH with ESP8266 as the main board.  Is the pin out the same as the arduino nano.  Also would i need to change the code for the wifi module?
https://www.adafruit.com/product/2821
```

---
## \#393 Posted by: ervinelin Posted at: 2019-02-28T22:54:31.509Z Reads: 151

```
Totally different. You would need to change the code completely, this won't even run an Arduino sketch.
```

---
## \#394 Posted by: Leander Posted at: 2019-03-01T20:31:48.766Z Reads: 148

```
Oh ok, thank you. So is the feather m0 basic the same pin out? Also is there an other cheaper place to buy them from then right from adafruit.
```

---
## \#395 Posted by: ervinelin Posted at: 2019-03-02T02:29:43.573Z Reads: 145

```
All of them have different pin outs I think...

Mine is specifically for the 328P feathers. I bought them from Mouser, it was the cheapest for me because buying a few meant free shipping.
```

---
## \#396 Posted by: markyoe Posted at: 2019-03-06T03:22:39.244Z Reads: 136

```
Have you had a chance to put together a wiring diagram?
```

---
## \#397 Posted by: ervinelin Posted at: 2019-03-07T03:10:32.500Z Reads: 141

```
Not yet, been so busy I haven't even skated much in the past few months...
```

---
## \#398 Posted by: MatteoCarnelos Posted at: 2019-03-22T17:11:15.002Z Reads: 133

```
Hi Leander, I'm currently working on a version with the HUZZAH32. It is completely different from Arduino but my goal is to program it using MicroPython (with multithreading!). I think ESP32 is better because with BLE you can connect the remote to your phone and tune some settings or download telemetry data. Anyway, I'm almost done with my work, when I finish it I will publish it here.
```

---
## \#399 Posted by: Nandox7 Posted at: 2019-03-22T18:03:07.932Z Reads: 130

```
Out of curiosity, I suspect you using ESP-Now for the radio/board link?
```

---
## \#400 Posted by: MatteoCarnelos Posted at: 2019-03-23T17:57:53.674Z Reads: 124

```
I use BLE also for the remote-board connection. The reciever will be an HUZZAH32 or just a BLE module (like the HM-10) connected to an Arduino (this solution is cheaper)
```

---
## \#401 Posted by: Silverline Posted at: 2019-03-23T18:23:06.806Z Reads: 125

```
Nice.... Looking forward
We need trigger remotes...
```

---
## \#402 Posted by: StefanMe Posted at: 2019-03-23T18:34:01.747Z Reads: 130

```
Crazy how many diy remotes coming at the moment! Awesome!!

Firefly Remote
Firefly nano remote
Feather remote
Trigger style remote
... a lot more are in development and of course I forgot a lot project...
```

---
## \#403 Posted by: Uri Posted at: 2019-03-31T17:43:41.345Z Reads: 125

```
Hello,
I have this error in the transmitter, someone can help me.
Thank you very much

Arduino:1.8.8 (Windows 7), Tarjeta:"Arduino Nano, ATmega328P (Old Bootloader)"

C:\Users\Laura\Documents\Arduino\Mando Sk8\receiver_VESC6\receiver_VESC6.ino: In function 'void setup()':

receiver_VESC6:70:25: error: 'SetSerialPort' was not declared in this scope

   SetSerialPort(SERIALIO);

                         ^

C:\Users\Laura\Documents\Arduino\Mando Sk8\receiver_VESC6\receiver_VESC6.ino: In function 'void loop()':

C:\Users\Laura\Documents\Arduino\Mando Sk8\receiver_VESC6\receiver_VESC6.ino:89:52: warning: large integer implicitly truncated to unsigned type [-Woverflow]

     radio.writeAckPayload(pipe, &data, sizeof(data));

                                                    ^

exit status 1
'SetSerialPort' was not declared in this scope
```

---
## \#404 Posted by: Uri Posted at: 2019-03-31T17:49:58.546Z Reads: 128

```
![Captura|690x407](upload://kpqhJMvFJjbW8nCGzLEmMNR4iFq.png)
```

---
## \#405 Posted by: ervinelin Posted at: 2019-03-31T22:58:21.326Z Reads: 126

```
Sounds like you are using the wrong library.

[https://www.electric-skateboard.builders/t/diy-trigger-style-remote-with-telemetry-complete-guide/48231/302?u=ervinelin](https://www.electric-skateboard.builders/t/diy-trigger-style-remote-with-telemetry-complete-guide/48231/302?u=ervinelin)

Make sure u clear out the old library first. This refers to the older Rollinggecko vesc library, replace it with solidgeeks.
```

---
## \#406 Posted by: Uri Posted at: 2019-04-01T12:25:17.440Z Reads: 120

```
You're right, it was a problem with the library.
But the problem has been solved with this library ... (https://github.com/RollingGecko/VescUartControl/tree/VESC6)

Thank you very much for your help
```

---
## \#407 Posted by: ervinelin Posted at: 2019-04-01T12:38:46.304Z Reads: 122

```
Glad to be of some help...

But from what I remember u might need solidgeeks version for the latest vesc firmware... I think telemetry won't work using the Rollinggecko version.
```

---
## \#408 Posted by: Ruubie200 Posted at: 2019-04-01T12:45:09.937Z Reads: 119

```
what does the lc filter do and do u need it to work corect?
```

---
## \#409 Posted by: Ruubie200 Posted at: 2019-04-01T12:47:42.553Z Reads: 113

```
can i use this hall effect? SS49E https://www.tinytronics.nl/shop/nl/componenten/overige/oh49e-hall-effect-switch-ss49e-compatible
```

---
## \#410 Posted by: ervinelin Posted at: 2019-04-01T13:13:37.978Z Reads: 112

```
In some cases it was critical... Especially with the older NRF module. My more recent versions have done away with it and just use a series of capacitors instead.
```

---
## \#411 Posted by: ervinelin Posted at: 2019-04-01T13:14:30.152Z Reads: 114

```
Can't read the German. But should work. My current hall sensor uses 3V not 5V.
```

---
## \#412 Posted by: Ruubie200 Posted at: 2019-04-02T07:46:44.670Z Reads: 111

```
can i use the new receiver with the old remote?
```

---
## \#413 Posted by: ervinelin Posted at: 2019-04-02T07:53:29.499Z Reads: 109

```
Should be able to. My new remotes connect to old receivers.
```

---
## \#414 Posted by: Ruubie200 Posted at: 2019-04-02T08:03:58.020Z Reads: 117

```
is there a schematic for the new remote? or an updated guide
```

---
## \#415 Posted by: ervinelin Posted at: 2019-04-02T08:38:07.611Z Reads: 115

```
No time to do one changing job and moving so will be too busy to do so.

Will try to post an update in May.
```

---
## \#416 Posted by: Uri Posted at: 2019-04-03T11:56:53.360Z Reads: 113

```
Hello,
Can you send me the link to download the correct library? it only allows me to compile with the RollingGecko library ...

Thank you
```

---
## \#417 Posted by: ervinelin Posted at: 2019-04-03T12:12:49.809Z Reads: 114

```
You have to hunt it down in the forum. Again look for solidgeeks version not rolling gecko.
```

---
## \#418 Posted by: Uri Posted at: 2019-04-03T20:43:50.085Z Reads: 124

```
Hello,
I continue to have problems in the compilation of the receiver. I have installed this library:
https://github.com/SolidGeek/VescUart
And I have this error message:
receiver_VESC6:45:20: error: aggregate 'bldcMeasure uartData' has incomplete type and cannot be defined

 struct bldcMeasure uartData;

                    ^

receiver_VESC6:56:20: error: aggregate 'bldcMeasure measuredValues' has incomplete type and cannot be defined

 struct bldcMeasure measuredValues;

                    ^

C:\Users\Laura\Documents\Arduino\Mando Sk8\nRF24-Esk8-Remote-master\receiver_VESC6\receiver_VESC6.ino: In function 'void setup()':

receiver_VESC6:63:26: error: 'SetSerialPort' was not declared in this scope

   SetSerialPort(&SERIALIO);

                          ^

C:\Users\Laura\Documents\Arduino\Mando Sk8\nRF24-Esk8-Remote-master\receiver_VESC6\receiver_VESC6.ino: In function 'void loop()':

C:\Users\Laura\Documents\Arduino\Mando Sk8\nRF24-Esk8-Remote-master\receiver_VESC6\receiver_VESC6.ino:82:52: warning: large integer implicitly truncated to unsigned type [-Woverflow]

     radio.writeAckPayload(pipe, &data, sizeof(data));

                                                    ^

C:\Users\Laura\Documents\Arduino\Mando Sk8\nRF24-Esk8-Remote-master\receiver_VESC6\receiver_VESC6.ino: In function 'void getVescData()':

receiver_VESC6:133:35: error: 'VescUartGetValue' was not declared in this scope

     if ( VescUartGetValue(uartData) )

                                   ^

exit status 1
aggregate 'bldcMeasure uartData' has incomplete type and cannot be defined
```

---
## \#419 Posted by: Uri Posted at: 2019-04-03T20:43:59.828Z Reads: 105

```
thank you very much for your help and patience!
```

---
## \#420 Posted by: gmurad Posted at: 2019-04-03T21:54:56.245Z Reads: 107

```
I've read the full Feather Remote and Firefly nano threads but I'm gonna ask a question here without reading through the full thread. Sorry in advance.

If I understand correctly there the parts list on the first page uses outdated hardware? There is already a new remote?

What are the main differences between old and new and is there a parts list for the new remote?
```

---
## \#421 Posted by: ervinelin Posted at: 2019-04-04T00:14:24.054Z Reads: 113

```
2 possible things.

1. Did you manually remove the old rolling gecko UART library yet?
2. Are you trying to compile my version of the receiver? If so I think the one online is outdated.
```

---
## \#422 Posted by: ervinelin Posted at: 2019-04-04T00:20:15.287Z Reads: 114

```
The new remote is easier to build by miles. I would also argue it's more reliable.

It uses different Arduino and NRF boards. A custom PCB and a redesigned casing.

If you read a few posts up, you will know I plan to update these in May. Too busy this month.
```

---
## \#423 Posted by: Uri Posted at: 2019-04-04T11:25:13.074Z Reads: 114

```
I have manually deleted the Rolling Gecko library and installed the SolidGeek library correctly and the error persists.
I am trying to compile your receiver version. I downloaded it from the GitHub Master.
Please, can you update the online version?

Thank a lot
```

---
## \#424 Posted by: ervinelin Posted at: 2019-04-04T12:31:17.467Z Reads: 117

```
Wouldn't make sense to just upload the receiver alone. Like I mentioned I am swamped this month. Will put up a proper update in May.
```

---
## \#425 Posted by: cfairn Posted at: 2019-04-09T19:45:50.642Z Reads: 118

```
i am trying to gear up a hobby![IMG_0026|375x500](upload://jFBkPPnZXMEyIzCLvpzRNHWQbzY.jpeg) sky 2.4 remote to my swagboard any advice on how to wire it? does the receiver need to be external? any help would be greatly appreciated, thanks!
```

---
## \#426 Posted by: ervinelin Posted at: 2019-04-10T00:55:05.648Z Reads: 116

```
I don't understand. You are asking me about another remote? I won't know, this thread is about my specific remote.
```

---
## \#427 Posted by: Mich21050 Posted at: 2019-04-11T13:29:31.776Z Reads: 112

```
Anyone on here got the old Gerber files? Because I have the parts laying around for the old one. :slight_smile: Bc on easyeda are only the new PCB files.
```

---
## \#428 Posted by: Wisp Posted at: 2019-05-14T21:05:55.004Z Reads: 97

```
Hi @ervinelin 2 small questions after reading the full thread:
1. Im using an app to quickly switch ride settings trough bluetooth. Is this still possible with your receiver (when the remote is not connected I guess)
2. Is the distance, lifetime distance or trip?

Thank you
```

---
## \#429 Posted by: ervinelin Posted at: 2019-05-14T23:00:59.998Z Reads: 99

```
1. Only possible if u running dual escs. Then one is connected to a Bluetooth module, the other to the remote. Via the Bluetooth module and app you can adjust settings to both escs through the can bus.

2. Trip only. Never figured out how to do a proper odo.
```

---
## \#430 Posted by: Wisp Posted at: 2019-05-15T16:59:05.089Z Reads: 99

```
Thanks!

10c
```

---
## \#431 Posted by: mechase2000 Posted at: 2019-05-22T06:46:55.299Z Reads: 94

```
Did you have to adjust the code from eeprom to something else with the feathers? Mine boots right on a uno and a micro, but I get an eeprom error on my feather proto m0. Am I using the correct transmitter code?
```

---
## \#432 Posted by: FalconNL Posted at: 2019-06-19T23:01:40.661Z Reads: 80

```
Any updates?
```

---
## \#434 Posted by: Qrob Posted at: 2019-08-13T23:02:25.037Z Reads: 50

```
@ervinelin can I buy one??
I will pay how much you say
```

---
## \#435 Posted by: Hypnos Posted at: 2019-09-11T09:10:11.886Z Reads: 37

```
@ervinelin are you planning any updates?
```

---
