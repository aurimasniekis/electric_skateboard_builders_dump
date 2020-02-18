# VESC - Installing a bootloader

### Replies: 109 Views: 17233

## \#1 Posted by: treenutter Posted at: 2015-12-19T03:52:18.081Z Reads: 801

```
I was unlucky and received a VESC with no bootloader. I won't mention where it came from, because the excellent dude responsible for making a VESC available to me is on vacation and I'm not gonna bother him! 

I can't upgrade the firmware until I install a bootloader. I've been putting it off, but now that FOC is in full effect, it's time to give it a try! Currently my shit is LOUD and I need to roll in silence during top-secret missions.

I'm using VESC 4.7 and currently have firmware 1.10 installed (that's what the VESC shipped with). It works nicely, but half the fun of having an open-source ESC is being able to install new firmware and use new features.

I'm trying to follow Vedder's instructions. [Here he provides all the command lines needed][1] to prepare a Linux machine to flash the bootloader. (Flash is just a nickname for "programming a chip"). He also gives an example of [how to connect an ST-Link V2 to VESC][2] and that's where I'm getting stuck. 

Vedder provides an image of a similar programmer where you can see the pinout:

<img src="/uploads/db1493/original/2X/8/81bf333df50095db284b4caea942bfa2c7e61867.jpg" width="651" height="500">

But the one I bought looks like this:

<img src="/uploads/db1493/original/2X/9/9041ce7956f40e98daf77f86150b222355b28016.jpg" width="640" height="480">

Here's a closer look at the pinout:

<img src="/uploads/db1493/original/2X/c/c235ce153a4c385ca395919c0560ec776fe094c5.jpg" width="373" height="500">

While it looks like I need to connect GND, SWCLK, SWDIO, 3V3, RST, and GND, I've only got RST, GND, DATA, VDD, RST, SWD, CLK, GND, and VDD. WTF!?

Problem #1 is I don't know which of these pins on my ST-LinkV2 I need to connect.

Problem #2 I know which JST port to use on the VESC, but which pins on the port should connect with the pins on the programmer? Vedder *must* have put a diagram somewhere that shows how to connect the pins on VESC, but I can't find anything.

Problem #3 is I don't have a pin labeled 3V3. I'm assuming that SWCLK=CLK and that SWDIO=SWD

Maybe I should look for a programmer that is exactly like the one in Vedder's example? Any thoughts? Thanks!

  [1]: http://vedder.se/2015/01/vesc-open-source-esc/
  [2]: http://vedder.se/2014/12/connecting-a-programmerdebugger-my-custom-stm32-pcbs/
```

---
## \#2 Posted by: elkick Posted at: 2015-12-19T08:23:30.837Z Reads: 651

```
For the pin layout you can take the same order on the JST connector like shown in Benjamin's picture. But you definitely need a JST-PH 6pin connector.
At least that's what I've done. But you're right, I can't see 3.3 on yours. Is there another row of pins on the other side?
```

---
## \#3 Posted by: treenutter Posted at: 2015-12-29T03:56:09.605Z Reads: 613

```
Thanks @elkick ! No, there are no other pins on the programmer. I may need a different programmer. Without 3V3 I don't think that I can proceed. @jacobbloy @chaka does that sound right?
```

---
## \#4 Posted by: chaka Posted at: 2015-12-29T16:16:01.951Z Reads: 593

```
3.3v is the VDD pin. SWCLK is CLK and SWDIO is most likely SWD on your programmer.

Pin order on the VESC is 3.3v, CLK, GND, DIO, RST, SWO/Data. The labelling on your programmer is inconsistent with what I am used too but this should work.
```

---
## \#5 Posted by: treenutter Posted at: 2015-12-29T16:31:53.390Z Reads: 558

```
Thank you @chaka that's what I needed to know! To flash VESC, do I need to power the VESC with a battery, or does the programmer supply power to the chip during the process?
```

---
## \#6 Posted by: chaka Posted at: 2015-12-29T16:46:37.244Z Reads: 542

```
No need to power the vesc during the flashing process. You only need to power the vesc during configuration.
```

---
## \#7 Posted by: treenutter Posted at: 2016-01-05T15:55:38.728Z Reads: 534

```
Big thanks @chaka and @elkick. Right now I'm waiting for some jumper cables to arrive. Of course, I have a 5-pin set but I need six pins so I ordered this guy

<img src="/uploads/db1493/original/2X/a/a3f5f4984a300e5f7ccacf58b0dfe92c427aa1dc.jpg" width="500" height="500">
```

---
## \#8 Posted by: elkick Posted at: 2016-01-05T19:02:14.946Z Reads: 494

```
These are exactly the ones I'm using too. :smile:
Don't forget to (hot-) glue them to the STlinkv2 to keep everything in place.
```

---
## \#9 Posted by: longhairedboy Posted at: 2016-01-05T20:26:07.199Z Reads: 488

```
i have those same ribbon connectors! any time i need a set i just peel a few off. I'm actually using them to connect my PPM to the receiver. a little hot glue and they stay put nicely, and you can't beat the price.
```

---
## \#10 Posted by: treenutter Posted at: 2016-01-05T20:27:25.307Z Reads: 478

```
@longhairedboy @elkick is there anything that hot glue *can't* fix?
```

---
## \#11 Posted by: longhairedboy Posted at: 2016-01-05T20:33:32.955Z Reads: 478

```
not to my knowledge. lol

And its a hell of a great way to keep your components all tightly secured inside your box. I use it to float battery packs in the box, seal the nuts and washers on charge ports and buttons, cover up potentially problematic solder joints that can't be heat-shrinked, tie down wiring that needs to stay put, fasten my receiver to the inside of the box, pin down the antenna, hold my PPM wires in place, keep my balance leads secured... basically my boards are filled with this silicone based wonder because its tough, non-conductive, sticks to wood and plastic like a boss and is waterproof. 

and it can be peeled off (with some work) without damaging whatever its on. So its sort of temporary while still being sort of permanent.
```

---
## \#12 Posted by: treenutter Posted at: 2016-01-05T20:41:48.512Z Reads: 446

```
@longhairedboy word. I've got this stuff all over too. Do we need a hot-glue thread to showcase this wonder? It would be fun to ask people to post pics of how and where they use it.
```

---
## \#13 Posted by: cmatson Posted at: 2016-01-05T20:52:41.683Z Reads: 464

```
[quote="treenutter, post:12, topic:752"]
Do we need a hot-glue thread to showcase this wonder?
[/quote]

yes!

Must be 20 characters..... :sunglasses:
```

---
## \#14 Posted by: treenutter Posted at: 2016-01-07T20:32:45.756Z Reads: 483

```
OK @chaka @elkick @jacobbloy a quick update. I got my jumper cable ribbon and immediately found that 6 of these don't fit into VESC's JST connector port, so I removed three of the cable encasements and got them all connected:

<img src="/uploads/db1493/original/2X/a/a9198910692ce4ec5a505068a498bbd0b2156c92.JPG" width="375" height="500"> 

<img src="/uploads/db1493/original/2X/e/ef7a97c547a936405f511d67b1572dcc1cd3829b.JPG" width="375" height="500">

I checked and double-checked and I'm pretty certain that I connected the VESC to the programmer in the correct manner. Did you ask for a weird photo angle? Perfect! I got one! Here it is:
<img src="/uploads/db1493/original/2X/e/eb7ce3ff769ba85835e9fbb242a56cfe57c60e17.JPG" width="375" height="500">

Then I got it plugged into my PC and ran my Ubuntu image:<img src="/uploads/db1493/original/2X/c/c4fc216ab049d80d16d64b5b3491cef344fa6ad6.JPG" width="500" height="500">

Everything compiled and prepared just fine. I think this is the way to specify my hardware version, right? I have version 4.7

<img src="/uploads/db1493/original/2X/1/1cc4af9ef39117a3a03d8f66e7829b2f5e6c4de6.JPG" width="500" height="500"> 

But trouble came when it was time to "make upload" it appears that something was wrong and the software couldn't initialize the boot loader upload. There's the error screen:

 <img src="/uploads/db1493/original/2X/b/b0bbf28f6c698de53c1c1a1e091b23b9651a3405.JPG" width="500" height="500">

What does this suggest? Bad programmer? Not connected properly? 

It appears that the programmer didn't interact with my VESC at all... it's still stuck with the 1.10 firmware version and I still can't upload any new firmware versions through BLDC tool. Is there a way to verify that a boatloader is installed?
```

---
## \#15 Posted by: Blasto Posted at: 2016-01-07T20:35:45.155Z Reads: 425

```
did you power the vesc?
```

---
## \#16 Posted by: treenutter Posted at: 2016-01-07T20:36:44.841Z Reads: 432

```
Thanks @Blasto No, you don't need to during the flashing process, the programmer powers it. I did power when I tried to upload the firmware through BLDC tool.
```

---
## \#17 Posted by: elkick Posted at: 2016-01-07T21:19:25.612Z Reads: 432

```
It might be better to upload the bootloader first by following Benjamin's steps for bootloader upload.

Did your STLink show a green light? Make sure not to power on the VESC through the battery as long as you're working with the STlink.
```

---
## \#18 Posted by: treenutter Posted at: 2016-01-07T21:22:07.420Z Reads: 422

```
Thanks @elkick I did my best to follow Vedder's steps... I went step by step using his guide noted above.The STLink green light was one, and blinked during the "upload" of the bootloader. It seemed to fail at that point. I'm trying to figure out why.
```

---
## \#19 Posted by: elkick Posted at: 2016-01-07T21:24:44.051Z Reads: 424

```
All I can see on your screenshot is the firmware, not the bootloader. So when you went through the bootloader part before the firmware it said "verified ok" after bootloader upload?
```

---
## \#20 Posted by: chaka Posted at: 2016-01-07T21:27:16.825Z Reads: 432

```
Have you tried unplugging the USB to cycle the power on the programmer? Sometimes this error will show up during programming. A power cycle has always set things straight in my experience.

Careful setting an uninsulated VESC on a metal tower. Probably wont short anything out through the paint but why tempt fate.
```

---
## \#21 Posted by: treenutter Posted at: 2016-01-07T21:35:20.599Z Reads: 414

```
@elkick now I'm wondering if I made a mistake when I took this photo, I believe that error message shot above came after trying to run this command:

mkdir BLDC
cd BLDC
git clone https://github.com/vedderb/bldc-bootloader.git bldc-bootloader
cd bldc-bootloader
make upload

[There are some reports here][1], specifically this one, that make me wonder whether I have a hardware defect that is preventing the bootloader from being loaded, which might explain why it wasn't successful at the factory that @onloop used:
 
"I’ve tried it with and without the USB cable connected. I suspect the “unable to connect” indicates a hardware error, presumably in my soldering, unless anyone has other ideas."


  [1]: http://vedder.se/2014/12/connecting-a-programmerdebugger-my-custom-stm32-pcbs/
```

---
## \#22 Posted by: elkick Posted at: 2016-01-07T21:39:10.565Z Reads: 387

```
This error message is the same if the bootloader is not present or not correctly installed. 
You might just go through the bootloader part again to check. If that works, the FW part will work as well.
```

---
## \#23 Posted by: treenutter Posted at: 2016-01-07T21:41:12.318Z Reads: 372

```
Thanks @elkick I'll try again tonight. Will report back!
```

---
## \#24 Posted by: treenutter Posted at: 2016-01-07T21:42:55.676Z Reads: 364

```
@chaka very good point! I had the same thought as I placed it there but was too focused on the install! I'll try power cycling the programmer tonight if I don't get a successful install. Does it look like I specified the HW version correctly in conf_general.h ?
```

---
## \#25 Posted by: elkick Posted at: 2016-01-07T21:43:58.905Z Reads: 345

```
And please take some screenshots if there are errors in the bootloader part, we might be able to find the root cause. Also, between bootloader upload and FW upload the STlink needs to be pulled off and inserted again as Chaka mentioned.
```

---
## \#26 Posted by: treenutter Posted at: 2016-01-07T21:45:56.116Z Reads: 333

```
@elkick Ah! I did not do that! I didn't power cycle the programmer between steps. Thanks!
```

---
## \#27 Posted by: chaka Posted at: 2016-01-07T21:47:20.609Z Reads: 344

```
Looks like you are connected incorrectly. I don't have time to go over your photos very closely right now but I'll take another look these evening when I take a break.

@treenutter  Ahh well it will just take second. you deffinitly have the pin order wrong. We will keep your wire order on the VESC and just switch the connectors on you programmer.

Move the black wire to VDD, move the red wire to CLK, move the orange wie to GND, the yellow wire to SWD, the mustard green wire to RST and the green is most likely DATA.

I hope this works for you.
```

---
## \#28 Posted by: treenutter Posted at: 2016-01-07T21:48:57.188Z Reads: 334

```
Thanks @chaka ; I'm also wondering a bit about the integrity of the connections I've made using the jumper cables with the tips lopped off... although that usually works.
```

---
## \#29 Posted by: chaka Posted at: 2016-01-08T02:59:54.362Z Reads: 333

```
Those connections should be fine if you can feel some resistance when plugging them in. 

Did you get a chance to run the programmer again with the connectors moved?
```

---
## \#30 Posted by: treenutter Posted at: 2016-01-08T04:20:35.798Z Reads: 329

```
@chaka I did and it worked! Boot loader and updated firmware installed! I'll post pics and a summary tomorrow. Thanks so much  for taking a close look at my programmer! I tested FOC in my living room tonight. It's so good!
```

---
## \#31 Posted by: trbt555 Posted at: 2016-01-08T09:01:11.754Z Reads: 319

```
@treenutter I would really appreciate a brief recap and maybe a schematic.
Thanks to @Jack I'll be building a couple VESC's myself soon and uploading the bootloader will be part of the process.
```

---
## \#32 Posted by: Blasto Posted at: 2016-01-08T18:04:57.889Z Reads: 344

```
@trbt555 you just need to prepare de proper hardware and follow vedder's steps

You can get the discovery board, include it in your digikey or mouser BOM

 http://www.digikey.ca/product-detail/en/STM32F0308-DISCO/497-13893-ND/4310127

http://ca.mouser.com/Search/m_ProductDetail.aspx?STMicroelectronics%2fSTM32F0308-DISCO%2f&qs=%2fha2pyFadui%2f2iC6LF3Xs1YfU5RtwxMrvqllDc2BnH2%252bYWiSlRTdmw%3d%3d

The connection to the vesc are straight
<img src="/uploads/db1493/original/2X/f/f00818cc4be8f1c55a3ed2defeae3454a2508e4f.jpeg" width="375" height="500">

<img src="/uploads/db1493/original/2X/2/210a465298e8c80969b14a60867b3c38fca4a6a2.jpeg" width="375" height="500">

Jst ph 6 pin mate
http://www.digikey.ca/product-detail/en/06KR-D6S-P/455-2674-ND/2797509
```

---
## \#33 Posted by: treenutter Posted at: 2016-01-08T19:52:31.177Z Reads: 344

```
@trbt555 I think that @Blasto is right; it's all pretty straightforward unless you have a weird STLINK like I did that has an unusual naming convention for the pins... then you need an expert like @chaka to save the day and translate the pin titles for you! Thanks again @chaka and @elkick!

Here are some pics of the successful process, starting with the connection from the STLINK to the VESC (this time using a pad to reduce the risk of shorts):

<img src="/uploads/db1493/original/2X/d/da9344189fa74ae7caf3942cc94999ed09feb1a2.JPG" width="375" height="500">    

Run all of vender's command lines and you'll get these two screens when you finally upload the firmware and the bootloader.

Firmware Success!:<img src="/uploads/db1493/original/2X/0/0ce83e88594dc983bb85d9ac27c932c95c71cc4d.JPG" width="640" height="397">

Bootloader Success!: <img src="/uploads/db1493/original/2X/3/30a4232a689d2194fdcecc4ba6b6498a50b05d40.JPG" width="640" height="415">

Here's the VESC with it's LEDs blinking during\after the programming:
<img src="/uploads/db1493/original/2X/1/17ad19ae307e3d00c0ee1c9f0c01543e75e9e164.JPG" width="375" height="500">

And finally, screens from the Linux version of BLDC Tool:

<img src="/uploads/db1493/original/2X/e/eb3fec19080890dcf59dbd0bfff8133873e1234d.JPG" width="640" height="480">

FTW, the FOC config screen!

<img src="/uploads/db1493/original/2X/0/0ae22a9097cc468559e4c1f548b87f466eef68f0.JPG" width="640" height="408">

A quick review of **FOC**: Holy crap I love it! I could only test it in the living room, but it is dead silent and starts without any stutter using an unsensored motor! It's a vast improvement over the previous motor control process, at least at slow speeds and startup. Configuration of it was easier than I thought it would be... I just clicked the buttons, let the motor do it's thing, and then applied the settings to save them. I can't wait to get it out on the road!
```

---
## \#34 Posted by: Jack Posted at: 2016-01-08T20:50:19.813Z Reads: 315

```
The discovery board was too expensive for me! This ST-Link V2 works perfectly. <img src="/uploads/db1493/original/2X/3/36f6a96bde9cead4ae614290e0a37ac47dbb7ff2.jpeg" width="666" height="500">
```

---
## \#35 Posted by: Randyc1 Posted at: 2016-01-17T03:40:07.162Z Reads: 306

```
HOLY CRAP !!!!
 All this VESC installation is freaking me out !!,... . special wire connecting , ...downloading,... programming !

I have nt recieved it yet,...but i suck with computers and im wondering if i will ever get that VESC to work ???
```

---
## \#36 Posted by: cmatson Posted at: 2016-01-17T04:30:32.903Z Reads: 313

```
[quote="Randyc1, post:35, topic:752"]
HOLY CRAP !!!! All this VESC installation is freaking me out !!,... . special wire connecting , ...downloading,... programming !
[/quote]

haha this is all "extra" stuff; I wouldn't worry about any of it. 

All you need is the BLDC tool: it can be on mac or windows, and is just an application used to set up the VESC. Plug a USB cable into your VESC, open the application, and you are halfway there!

If you want to check out more info, I suggest the VESC faq section. It may seem daunting at first, but realize that if you just want to set up your VESC and then leave it alone, only a couple threads will even be helpful- a lot of them are for more complicated things that you won't need to worry about.

Trust me: I held out on the VESC for so long because I thought it was too complicated.. once I finally bought one, it took me less than an hour to download the application, set up the VESC, and get my board up and running. 

When in doubt, just ask!
```

---
## \#37 Posted by: treenutter Posted at: 2016-01-17T05:21:39.058Z Reads: 304

```
@Randyc1 pls note that this thread was written about a problem that very few people have. Any VESC you buy now will have a bootloader installed already and you don't need to do anything described here.
```

---
## \#38 Posted by: Randyc1 Posted at: 2016-01-17T06:28:09.174Z Reads: 303

```
Allright Guys , ...thanks for reassuring me !
```

---
## \#39 Posted by: GhettoFab.rictation Posted at: 2016-07-31T09:37:39.863Z Reads: 285

```
I've had a problem just getting my bldc tool to read my firmware on windows, having Linux or Ubuntu installed tomorrow when I get free time. Haven't really seen my issues, blue light when plugged in then three red lights flash only once on power up then goes to green light and my bldc tool never picks up firmware
```

---
## \#40 Posted by: marc Posted at: 2016-11-08T14:23:32.474Z Reads: 272

```
Okay, because I bought an alien VESC without releasing that is has no bootloader, so I need to install it. Warning! I'm a bit of a newb but I think I understand, can I use this [St-Link V2](http://www.ebay.com/itm/1PCS-ST-Link-V2-Programming-Unit-mini-STM8-STM32-Emulator-Downloader-New-/182141301471?hash=item2a6877b2df:g:ePAAAOSwbPxXQCcc)?
And so I would connect them in this order right?<img src="/uploads/db1493/original/3X/b/e/beb6119e68ec88d8b845688af530deddd692cf07.png" width="607" height="500">
And then I should download st-link utility from [here](http://www.st.com/en/embedded-software/stsw-link004.html), then I need to get the bootloader Hex file from [here](http://vedder.se/forums/viewtopic.php?t=17).
Could someone please tell me if I have all the necessary things?
```

---
## \#41 Posted by: treenutter Posted at: 2016-11-09T13:29:41.684Z Reads: 259

```
@marc it looks like you're on the right track, assuming you're using Linux and are following the instructions on Vedder's page.
```

---
## \#42 Posted by: marc Posted at: 2016-11-09T13:42:06.352Z Reads: 258

```
Is it possible to do it on Windows?
```

---
## \#43 Posted by: treenutter Posted at: 2016-11-09T13:57:56.673Z Reads: 255

```
@marc if it is, I'm unaware of how to do it. I'd go as far as to say that I don't think so. All of the instructions (and the command lines) for installing a bootloader are for Linux. If you don't have a spare PC you can create a dual-boot system or use a virtual machine within Windows.
```

---
## \#44 Posted by: DanButcher Posted at: 2016-11-09T14:21:16.533Z Reads: 252

```
Setup VirtualMachine with ubuntu and it should work, you can also run ubuntu from pendrive without installing it.
```

---
## \#45 Posted by: marc Posted at: 2016-11-09T21:05:28.543Z Reads: 250

```
Thanks for your guys' help so far. Would this work for me though(this virtual machine stuff looks scary)?
https://youtu.be/H4sbDhRcaOQ
```

---
## \#46 Posted by: treenutter Posted at: 2016-11-09T22:23:34.254Z Reads: 245

```
@marc nice find! I didn't know this was available. I haven't tried it so I can't comment. But hey, this is DIY, so whatever gets the job done is good enough! Personally, I've stopped using Windows ports of VESC tools and only use Linux, I find it easier to understand and more reliable. BLDC Tool is designed for Linux.
```

---
## \#47 Posted by: Lulu1 Posted at: 2016-12-21T21:03:56.232Z Reads: 235

```
Hi, I have a problem, i want to flash my vesc but when I want to connect my StLink to PC there an error message" Cannot connecte the stLink", solutions? Thanks
```

---
## \#48 Posted by: marc Posted at: 2016-12-21T21:09:03.674Z Reads: 238

```
You may not have all the necessary drivers.
```

---
## \#49 Posted by: Lulu1 Posted at: 2016-12-21T21:18:03.887Z Reads: 238

```
What are the necessary drivers ?
```

---
## \#50 Posted by: JTAG Posted at: 2016-12-21T21:27:44.886Z Reads: 235

```
The drivers for the ST-link :). What are you using? Windows/linux
```

---
## \#51 Posted by: Lulu1 Posted at: 2016-12-21T21:29:47.923Z Reads: 235

```
Windows, ;)
```

---
## \#52 Posted by: marc Posted at: 2016-12-21T21:32:40.121Z Reads: 234

```
I'm pretty sure I used these: http://www.st.com/en/development-tools/stsw-stm32102.html
```

---
## \#53 Posted by: JTAG Posted at: 2016-12-21T21:32:43.395Z Reads: 238

```
http://www.st.com/en/development-tools/st-link-v2.html 

Driver is listed at the bottom of the page. What environment are you using to flash?
```

---
## \#54 Posted by: Lulu1 Posted at: 2016-12-21T21:34:36.002Z Reads: 238

```
I use this [http://www.ebay.fr/itm/like/322294570031?lpid=97&chn=ps](http://www.ebay.fr/itm/like/322294570031?lpid=97&chn=ps)
```

---
## \#55 Posted by: marc Posted at: 2016-12-21T21:35:38.875Z Reads: 235

```
That will work fine, I have the same.
```

---
## \#56 Posted by: Lulu1 Posted at: 2016-12-21T21:36:12.161Z Reads: 238

```
Ok but now he dont work ;/
```

---
## \#57 Posted by: marc Posted at: 2016-12-21T21:37:26.719Z Reads: 240

```
Have you tried installing the correct drivers?
```

---
## \#58 Posted by: Lulu1 Posted at: 2016-12-21T21:38:57.383Z Reads: 249

```
I installed tis [http://www.st.com/en/embedded-software/stsw-link004.html](http://www.st.com/en/embedded-software/stsw-link004.html) in the down of the page
```

---
## \#59 Posted by: marc Posted at: 2016-12-21T21:42:51.795Z Reads: 255

```
You also need to install the drivers for the ST Link v2, get them here: http://www.st.com/en/development-tools/stsw-stm32102.html
```

---
## \#60 Posted by: Lulu1 Posted at: 2016-12-21T21:44:31.281Z Reads: 267

```
ok and after if i connect just the stlink v2 alone, normaly its work?
```

---
## \#61 Posted by: Wubbalubbadubdub Posted at: 2017-04-16T11:18:45.357Z Reads: 236

```
This is a great thread, along with the VESC FAQ. I am in the same boat as you guys. Because of my location (Germany) but my mailbox is US (APO), it is best for me if I can order a programmer via Amazon Prime so I'm not waiting months for it to arrive. Can anyone tell me if this model will work? 

https://www.amazon.com/gp/slredirect/picassoRedirect.html/ref=pa_sp_btf_industrial_sr_pg1_2?ie=UTF8&adId=A06950711ZIXXW3LUWGQ5&url=https%3A%2F%2Fwww.amazon.com%2FDAOKI-ST-Link-Programming-Emulator-Downloader%2Fdp%2FB01EE4WAC8%2Fref%3Dsr_1_7%3Fs%3Dindustrial%26rps%3D1%26ie%3DUTF8%26qid%3D1492341267%26sr%3D1-7-spons%26keywords%3DST-Link%2BV2%26refinements%3Dp_85%253A2470955011%26psc%3D1&qualifier=1492341267&id=7701086375568010&widgetName=sp_btf
```

---
## \#63 Posted by: fottaz Posted at: 2017-04-28T01:58:52.195Z Reads: 221

```

It should works good, will you flash with Windows?
```

---
## \#64 Posted by: rpn314 Posted at: 2017-04-28T02:04:26.174Z Reads: 224

```
[quote="Wubbalubbadubdub, post:61, topic:752, full:true"]
This is a great thread, along with the VESC FAQ. I am in the same boat as you guys. Because of my location (Germany) but my mailbox is US (APO), it is best for me if I can order a programmer via Amazon Prime so I'm not waiting months for it to arrive. Can anyone tell me if this model will work? 

https://www.amazon.com/gp/slredirect/picassoRedirect.html/ref=pa_sp_btf_industrial_sr_pg1_2?ie=UTF8&adId=A06950711ZIXXW3LUWGQ5&url=https%3A%2F%2Fwww.amazon.com%2FDAOKI-ST-Link-Programming-Emulator-Downloader%2Fdp%2FB01EE4WAC8%2Fref%3Dsr_1_7%3Fs%3Dindustrial%26rps%3D1%26ie%3DUTF8%26qid%3D1492341267%26sr%3D1-7-spons%26keywords%3DST-Link%2BV2%26refinements%3Dp_85%253A2470955011%26psc%3D1&qualifier=1492341267&id=7701086375568010&widgetName=sp_btf
[/quote]

I have the same one just in a different color. Works in both Windows (10 with some special driver I'd have to dig up if you need it) and Linux (Ubuntu 16.04)
```

---
## \#65 Posted by: Wubbalubbadubdub Posted at: 2017-04-28T08:38:52.479Z Reads: 202

```
Awesome! It just arrived yesterday. If you could tell me what Windows 10 driver you used it would be terrific!
```

---
## \#66 Posted by: Wubbalubbadubdub Posted at: 2017-04-28T08:39:34.954Z Reads: 208

```
Yes I will flash it with windows.
```

---
## \#67 Posted by: fottaz Posted at: 2017-04-28T09:02:16.539Z Reads: 211

```
You Will Just Need theese Pins:

3.3v
Clock 
GND 
Dio 

Follow this guide and everything Will goes fine :) https://youtu.be/H4sbDhRcaOQ
```

---
## \#68 Posted by: rpn314 Posted at: 2017-04-28T13:54:08.802Z Reads: 214

```
He beat me too it :)

[quote="fottaz, post:67, topic:752"]
You Will Just Need theese Pins:

3.3vClock GND Dio 

Follow this guide and everything Will goes fine :slight_smile: https://youtu.be/H4sbDhRcaOQ
[/quote]

I commented on that video as well. When you run the program to flash the hex file, run it in Windows 7 compatibility mode. It'll make life better :D
```

---
## \#69 Posted by: Wubbalubbadubdub Posted at: 2017-04-29T08:21:05.037Z Reads: 207

```
does it matter which pins on the vesc i pin into? i mean, left to right in the same order listed?
```

---
## \#70 Posted by: rpn314 Posted at: 2017-04-29T12:53:22.910Z Reads: 207

```
The pins are labeled on the vesc as well as on any stlink programmer, so just match them up :slight_smile:
I also use the reset pin, but I frankly don't know if you have to.
```

---
## \#71 Posted by: Wubbalubbadubdub Posted at: 2017-04-29T14:29:26.928Z Reads: 208

```
I see now, they're labeled on the back! I'm so observant!
```

---
## \#72 Posted by: TarzanHBK Posted at: 2017-05-11T21:06:16.149Z Reads: 223

```
So one of my Axle Vesc from the first batch from @zmoney was missing a bootloader, while the other one had one :D
I searched a bit and like to help you summerize it here:

1 . Buy a ST-Link V2 (pic from @Jack) :
<img src="/uploads/db1493/original/3X/4/d/4d3b3285ab460126a39e1b1de38fef13214c985e.jpeg" width="666" height="500"> 

2 . Connect your ST-Link to your Vesc and simply match up connectors (written on the back of Vesc):
<img src="/uploads/db1493/original/3X/7/5/756b872cd99ff60711c1bf5fcc0b8c205f6c3c42.jpg" width="375" height="500">

3 . Take a look at Jacobs video how to connect (I used Windows):

https://www.youtube.com/watch?v=H4sbDhRcaOQ&feature=youtu.be&list=PLICpQdAXJazRzoXJByGA_5wd-B4cifmbh

Tip: Connect your St-Link to a USB 2.0 Port and use compability mode on Windows to run it with Windows 8 or earlier - could cause problems connecting otherwise.

Jacobs site is offline at the moment, so to flash the bootloader use this HEX file:
http://vedder.se/forums/download/file.php?id=6&sid=a6b085428455d0f9a617d880da259517

4 . Now download @Ackmaniac or any other BLDC tool you like, connect it and load a desired Firmware with it.

If you still struggle on some point, just comment below :slight_smile:
```

---
## \#73 Posted by: Geddi Posted at: 2017-05-26T18:15:31.652Z Reads: 216

```
https://www.amazon.de/WINGONEER-Cortex-M0-schwimmen-Schnittstelle-programmierer/dp/B012VR3PVA/ref=sr_1_1?ie=UTF8&qid=1495822394&sr=8-1&keywords=st+link+v2

@TarzanHBK @rpn314 I suppose this one should work right? And four pins are enough?

I ordered a VESC from Alien and actually received it already. I was like ohhh wow a VESC for 100 Bucks. 1min later it was ordered. I just unpacked and started doing research on configuring the VESC and stuff and well here I am.
```

---
## \#74 Posted by: TarzanHBK Posted at: 2017-05-29T06:51:29.750Z Reads: 208

```
yep this one should work
```

---
## \#75 Posted by: Mox Posted at: 2017-10-04T19:53:37.150Z Reads: 170

```
thx for this thread guys!
```

---
## \#76 Posted by: landonkun Posted at: 2017-10-04T21:47:08.799Z Reads: 176

```
Just wanted to point out that you no longer need to do all this fancy stuff, because the new Vesc-tool can upload a bootloader to vescs that don't already have one. I did this with my Maytech vesc and it went fine. Let me know if you need any help.
```

---
## \#77 Posted by: okp Posted at: 2017-10-21T15:13:33.494Z Reads: 178

```
Hey folks, maybe i'm too tired but I'm looking for the good wiring on a FOCBOX to flash it with a STLINK 

<img src="/uploads/db1493/original/3X/c/5/c563f01657e92104070115482ecfd7762503cc1c.jpg" width="522" height="500">
```

---
## \#78 Posted by: Blasto Posted at: 2017-10-21T17:03:08.771Z Reads: 185

```
<img src="/uploads/db1493/original/3X/8/a/8a2ef07201f43a21888614f462db954da875dc62.JPG" width="375" height="500">

Focbox.  Stlink
Rst.        Rst
Dio.        Swdio
Clk.        Swclk
Gnd.       Gnd


Dont think you need the 3.3V @okp
```

---
## \#79 Posted by: okp Posted at: 2017-10-21T18:16:52.282Z Reads: 209

```
Thanks for the support. That went perfectly fine. I have put back the FW2.16. 

I just can't upload FW 3.x with VESC TOOL. It seems to upload but nothing is upgraded. Either the FW or Bootloader

Any idea?

https://youtu.be/ulrZ7nEptXA
```

---
## \#80 Posted by: Pimousse Posted at: 2017-10-26T07:24:22.966Z Reads: 204

```
You need to upload the bootloader through command lines, not using VESC Tool.
Bootloader uploading through VESC Tool is only a trick Vedder coded in emergency to deal with VESCs with a FW but no bootloader (I mean, it has NEVER been uploaded).
If you try to upload it although one was already existing, you mess it up.
(See the warning of Vedder at the early stage of Beta for beta-testers : http://vesc-project.com/node/47 )
```

---
## \#81 Posted by: cliofreak Posted at: 2018-01-24T23:40:02.436Z Reads: 202

```
OK, Id really love some things confirmed if anyone can help:

* I have a Vesc with 2.18 FW and its 4.12 HW
* I have a Mac
* I have an STLinkV2 ordered

I want to update the Firmware so I can use full features of the @rpasichnyk Metr App.

1. Do I need to download Ubuntu?
2. Do I need a PC emulator?
3. Or, can I just do the upgrade via VescTool on my Mac?

I've been reading and watching some vague vids for a few hours and there seems to be a few ways to do this and all of them are confusing for different reasons. 
Theres talk of a Hex file. When I download from the link above, I get a folder with a few things in it. Will it all become apparent when I finally figure out how to run the STLink Utility?![59|690x237](upload://4kMEneUQAmsErYBEZWltZb8QgUz.png)![48|419x500](upload://vj8MfJZxrXXEIfWoefG7FmpnLqU.png)![10|690x159](upload://m758xeFMI8ea1T216BZKi2965AF.png)
```

---
## \#82 Posted by: Jamy Posted at: 2018-01-24T23:49:50.415Z Reads: 187

```
If you have a VESC with a firmware already installed you can flash the bootloader from VescTool. If somehow you accidentally removed the firmware from the device you'll need the STLink to recover it.

I had the misfortune to have used a bad USB cable and broke my firmware during a config upgrade on my FOCBOX.
In case that happens, you have to use the STLink tool to flash any firmware (I used 2.18 firmware file) back to the device.
I don't have the instructions for that nearby, but if needed I can go look them up :slight_smile:

TLDR; if there's a firmware on there you can flash bootloader via VescTool.
```

---
## \#83 Posted by: cliofreak Posted at: 2018-01-25T00:12:27.931Z Reads: 187

```
Thanks Jamy! That sounds pretty simple then. SO the VESC TOOL will have the latest firmware automatically on it or do I need to direct it to somewhere?
```

---
## \#84 Posted by: Jamy Posted at: 2018-01-25T00:14:18.382Z Reads: 183

```
Vesc_tool will have the latest 3.XX firmware. I'm not sure if that's compatible with Metr, but if it isn't you can always downgrade :slight_smile:
```

---
## \#85 Posted by: cliofreak Posted at: 2018-01-25T00:15:44.098Z Reads: 177

```
I think it is. SO just to confirm... My Vesc absolutley does not currently have a Bootloader on it. So, with VESC TOOL, this doesnt matter? The tool puts a bootloader on it or acts as the boot loader?
```

---
## \#86 Posted by: Jamy Posted at: 2018-01-25T00:18:17.394Z Reads: 170

```
Vesc tool will ask you if you want to install a bootloader when you connect it :)
```

---
## \#87 Posted by: cliofreak Posted at: 2018-01-25T00:19:20.741Z Reads: 164

```
Cheers man! Ill give it a go and it it goes tits up, the STLink is in the mail.
```

---
## \#88 Posted by: Riako Posted at: 2018-02-19T15:54:40.352Z Reads: 158

```
Hey Jamy, so what was yours wiring diagram to the Fox ? 
Did you use the 3.3v ? Or just Rst Swdio Swclk & Gnd ?
Thanks for your help :v:
```

---
## \#89 Posted by: Jamy Posted at: 2018-02-19T16:13:57.164Z Reads: 157

```
It's all back in my Raptor 2, but I got a picture [here](https://photos.app.goo.gl/AWjfIXA6L2Lmhqz63). I soldered to each of the pins above the cap (which was a pain in the ass because there was solder already in there...

The ground pin was the worst so I just connected elsewhere to ground.

So, tldr; connect to: RST, DTO, GND, CLK, 3.3
```

---
## \#90 Posted by: Riako Posted at: 2018-02-19T22:39:45.085Z Reads: 151

```
:+1: Perfect ! Thank you, treenutter and JdogAwesome a lot guys ;)
```

---
## \#91 Posted by: makeflyeasy Posted at: 2018-03-02T05:35:23.427Z Reads: 155

```
![TIM截图20180302130759|686x500](upload://dIsCpHl0wReBuAtN4q1p9q9e8DG.png)![TIM截图20180302130926|527x499](upload://zCktVSDX7FznzPjxPbmmve4SNLi.png)
```

---
## \#92 Posted by: Ken_Chen Posted at: 2018-03-06T05:56:41.477Z Reads: 147

```
Hi All, does anyone can share the link of the bootlaoder file for VESC 6?  thanks.
```

---
## \#93 Posted by: scepterr Posted at: 2018-03-22T01:45:58.566Z Reads: 144

```
Bump
@JohnnyMeduse have vesc 6 bootloader hex you can post?
```

---
## \#94 Posted by: JohnnyMeduse Posted at: 2018-03-22T01:48:20.595Z Reads: 144

```
Hummmm.... I don't have it... I usually program them with the bootloader from the 4 and upgrade them after :crazy_face:
```

---
## \#95 Posted by: scepterr Posted at: 2018-03-22T01:49:07.463Z Reads: 143

```
Lol ok...if that works, I'm good
```

---
## \#96 Posted by: scepterr Posted at: 2018-03-22T02:48:50.357Z Reads: 136

```
Ok a little heads up for anybody that get stuck in the blue light only situation where you have corrupted or no firmware/bootloader. 

Just flash the corresponding vesc_default.bin for your vesc version using stlink, then you can connect with VESC Tool and flash bootloader, change firmware etc
```

---
## \#97 Posted by: RedEagle Posted at: 2018-03-22T14:54:44.785Z Reads: 132

```
Anybody tried uploading bootloader/firmware with vesc tool? I'm having mixed results..
```

---
## \#98 Posted by: Bjork3n Posted at: 2018-03-22T15:03:49.037Z Reads: 135

```
Yes! 
I did with my maytech vesc.
Was super easy, vesctool did all the work, no need for st-link.
```

---
## \#99 Posted by: moronicity Posted at: 2018-04-25T19:18:06.044Z Reads: 122

```
Im getting the blue light only on my VESC. I am unable to upload anything onto the VESC using the STlink via Ubuntu. Any other ideas?
```

---
## \#100 Posted by: moon Posted at: 2018-06-11T13:46:23.102Z Reads: 115

```
[quote="scepterr, post:93, topic:752"]
@JohnnyMeduse have vesc 6 bootloader hex you can post?
[/quote]

Another bump...

Did you find the bootloader or did you do what johnny did and upgrade it in the VESC tool?

This must be what I am looking for?

https://github.com/vedderb/vesc_tool/blob/master/res/firmwares/60/VESC_default.bin
```

---
## \#101 Posted by: Eboosted Posted at: 2018-09-14T04:57:03.492Z Reads: 97

```
[quote="Blasto, post:78, topic:752"]
Dont think you need the 3.3V @okp
[/quote]

@Blasto I connected everything but the 3.3V and I can't connect the FocBox via ST-Link. Should I power the FocBox to be able to connect? or should I connect 3.3V pin from ST-Link to 3.3V pin from FocBox?
```

---
## \#102 Posted by: Eboosted Posted at: 2018-09-14T05:04:03.485Z Reads: 96

```
[quote="Eboosted, post:101, topic:752"]
@Blasto I connected everything but the 3.3V and I can’t connect the FocBox via ST-Link. Should I power the FocBox to be able to connect? or should I connect 3.3V pin from ST-Link to 3.3V pin from FocBox?
[/quote]

Just wanted to pint out you need to power on the FocBox to be able to connect via ST-Link otherwise you will get a "Can't not connect to target" message.
```

---
## \#103 Posted by: Pimousse Posted at: 2018-09-14T06:20:55.198Z Reads: 88

```
Connect 3.3V only if you don't power the FOCBOX by the main leads.
But if you don't connect 3.3V, that's normal that is does not work.

What you want avoid is connecting simultaneously main leads power AND 3.3V from STLink.
```

---
## \#104 Posted by: trampa Posted at: 2018-09-17T18:09:12.146Z Reads: 84

```
You never ever want to connect the 3.3V PIN! This is  a sniffer PIN, allowing the original ST Link to see that the ST processor is powered up so that it can be programmed. The clone ST Links apply 3.3V instead of sensing 3.3V!
```

---
## \#105 Posted by: Pimousse Posted at: 2018-09-17T18:40:16.317Z Reads: 87

```
https://media.giphy.com/media/l3q2K5jinAlChoCLS/giphy.gif

[quote="trampa, post:104, topic:752"]
You never ever want to connect the 3.3V PIN!
[/quote]

Yes I want Sir !

How would I power the MCU without bringing it 3.3V on Vcc ?
This is the purpose of the SWD 5th pin regarding Ben's HW6.4 schematics :

![SWD_vesc6|690x249](upload://pHvLcTzFbC1Kgq1jVu60ll3akdK.png)

Again, I don't power the VESC through its main leads while programming.

Anyway, did it on FOCBOX and quite a few ESCape without any issue.

But please @Eboosted, stick to @trampa advice.
I don't want any trouble.
```

---
## \#106 Posted by: trampa Posted at: 2018-09-17T18:59:10.751Z Reads: 86

```
https://www.vesc-project.com/node/80

Dead voltage regulator

One of the VESCs that I repaired had a dead 3.3v regulator. One way to kill the regulator is to feed it backwards with a 3.3v source, which has happened to me a few times when connecting a programmer.

Solution: Never feed the 3.3v net with voltage, only current draw is allowed. If you, for example, have a stlink v2 from ebay that outputs 3.3v on a pin then don't connect that pin - power the VESC from the input while the programmer is connected.

Edited by: benjamin on 2017-07-07 11:17
```

---
## \#107 Posted by: Eboosted Posted at: 2018-09-17T21:33:43.673Z Reads: 84

```
That's good to know. Fortunately I powered the vesc through the xt60.
```

---
## \#108 Posted by: conquerco Posted at: 2019-07-03T05:16:16.502Z Reads: 45

```
I'm getting a blinking red light that flashes 3 times after being connected by ST Link. Nothing else is connected, any ideas?
```

---
## \#109 Posted by: TheFlash Posted at: 2020-01-23T02:43:16.024Z Reads: 16

```
can i get those instructions i cant seem to connect to my focbox
```

---
## \#110 Posted by: Jamy Posted at: 2020-02-13T03:57:41.287Z Reads: 9

```
Thiss was a couple of years ago, I don't quite recall. Where are you getting stuck?

If I remember correctly the process was:
- Connect your STLink 2 adaptor as follows:
    - Focbox <-> Stlink
    - Rst <-> Rst 
    - Dio <-> Swdio
    - Clk <-> Swclk
    - Gnd <-> Gnd
    - 3.3v <-> 3.3v
- Load the STLink tool ([See here](https://www.electric-skateboard.builders/t/vesc-installing-a-bootloader/752/58) and [here](https://www.electric-skateboard.builders/t/vesc-installing-a-bootloader/752/59))
- Download whatever VESC firmware you want to upload (I used 2.18 after failing to upload 3 or 4)
- Open the firmware bin file in the STLink tool, click write or upload or whatever feels like a good upload button (might be under STLink or Target or Edit in the top menu)
- Cross your fingers it works..
```

---
