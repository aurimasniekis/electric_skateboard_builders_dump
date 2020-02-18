# VESC Boot Loader Installation Tutorial

### Replies: 43 Views: 11191

## \#1 Posted by: JdogAwesome Posted at: 2017-09-02T17:32:54.896Z Reads: 638

```
This thread is simply a straight forward tutorial on how to install the boot loader onto a VESC. I'm using a Maytech VESC for this, but it should work for any VESC that does not have a boot loader installed. All sources and credits are at the end of this thread.

**Step 1:**

Purchase a ST-Link V2 Like [THIS](http://www.ebay.com/itm/ST-Link-V2-Programming-Unit-mini-STM8-STM32-Emulator-Downloader/222595881285?ssPageName=STRK%3AMEBIDX%3AIT&_trksid=p2057872.m2749.l2649) one. They only cost about $5. Your also going to want to buy a 6-pin JST-PH 2mm male header for connecting to the VESC like [THIS](http://a.co/6FRES8c) one. You may also need some female to female jumper cables like [THESE](http://www.ebay.com/itm/40pc-Dupont-Wire-Jumper-Cable-1P-1P-2-54mm-female-to-Female-length-20cm-/311756641186?hash=item489624d3a2:g:SEMAAOSwQTVV8ECu).

**Step 2:**

Once all the parts from step 1 have arrived connect the JST and ST-Link together like in the image below. Green JST wire to 3.3v, Orange to SWCLK, Yellow to GND, White to SWDIO, and Red to RST the black wire can just be trimmed off or left alone.<img src="/uploads/db1493/original/3X/9/1/919b898797c9c7cbd969bf470a8af7b6a2ff6a61.jpg" width="690" height="389">


**Step 3:**

Now that you've connected the ST Link and JST plug it into your VESC port like in the pic below. Then plug the ST Link into a USB port in your computer running Windows. I used Windows 7 though it works with 8 and probably Win 10 as well. Also during this entire process of installing the boot loader the VESC does **NOT** need to be externally powered.
<img src="/uploads/db1493/original/3X/0/5/0521f0871095cde4cb7baa373edb5bc5a0b1b19b.jpg" width="690" height="389">

**Step 4:**

Next download the STM32 ST-LINK utility from [HERE](http://www.st.com/en/development-tools/stsw-link004.html). After you download that run and install the .exe to install the drivers and ST Link Utility itself. Next open the ST-Link Utility, there should be a desktop icon, and click Target Connect. at this point a  a large list of address should show up and that means you've connected properly. 

<img src="/uploads/db1493/original/3X/c/a/cacfa6bec63ec4f753f5a5c040e03ba48cfc2f40.jpg" width="652" height="500">

**Step 5:**

Download the VESC bootloader from **[THIS](http://vedder.se/forums/download/file.php?id=6&sid=a6b085428455d0f9a617d880da259517) link. Unzip it and there should be a file inside called "BLDC_4_Bootloader" thats the file we need. Next go back to ST Link and click Open File from the top left button. Navigate to the BLDC_4_Bootloader.hex file and click open. Next click Program Verify, the button just below Target then click Start, this may take a few seconds or a few minutes so just give it some time. Once its done verifying you can close the ST Link Utility and you've successfully installed the boot loader! Now just unplug the ST Link power the VESC and upload your firmware as usual!

<img src="/uploads/db1493/original/3X/d/1/d1b821a8f6df48adbb615b62b0b741ba3a14c24f.jpg" width="630" height="403">



Thanks to  the people on [THIS](https://www.electric-skateboard.builders/t/vesc-installing-a-bootloader/752) thread as its how I figured out how to do this. Big thanks to Esk8 Support, or Jacob and his video [HERE](https://youtu.be/H4sbDhRcaOQ) because this thread is pretty much just a transcription of that lol. 

**Thanks @TarzanHBK for the link to the .hex file as I could not have found it otherwise!
```

---
## \#2 Posted by: Mobutusan Posted at: 2017-09-04T20:21:37.145Z Reads: 492

```
Thanks for the write up. Will this boatloader work on FVT/@Torqueboards 12s car esc's too?
```

---
## \#3 Posted by: torqueboards Posted at: 2017-09-04T20:32:52.042Z Reads: 471

```
@Mobutusan No, this is only for VESC.
```

---
## \#4 Posted by: Riako Posted at: 2018-02-19T14:20:44.923Z Reads: 439

```
Hi, thanks you for this JdogAwesome :blush:
There are some posts like this aournd here, but nothing specialy dedicated to the FocBox Boot Loader.
I just find this [here](http://www.electric-skateboard.builders/t/vesc-installing-a-bootloader/752/78) :

> http://www.electric-skateboard.builders/uploads/db1493/optimized/3X/8/a/8a2ef07201f43a21888614f462db954da875dc62_1_375x500.JPG

So I can try on my fox with all your files safetly ?

Thanks a lot for your help :v:
```

---
## \#5 Posted by: JdogAwesome Posted at: 2018-02-19T16:42:35.793Z Reads: 392

```
Yeah @Riako the FOCBOX is based off of the VESC 4.12 hardware, that's why it uses the same software so yeah using those pin headers should work fine.
```

---
## \#6 Posted by: Riako Posted at: 2018-02-19T20:25:12.424Z Reads: 385

```
Perfect @JdogAwesome ;) :+1:
I asked because like I see a different wiring diagram propose for Fox in the other topic.

Now it wont pass the motor detection haha but I will end up getting there I hope.
I just feel like I'm totaly new in all this stuff with fox with vesctool... :sweat_smile: I haven't got any problem with ever when programming my vescs 4.xx with BLDCTool or VESC 6 with vescTool by the past. But here it looks like I got trouble with fox + vesc6 on same VESCTOOL ... don't really know.
```

---
## \#7 Posted by: Riako Posted at: 2018-02-20T01:35:58.099Z Reads: 376

```
Hey guys,
https://m.popkey.co/2c28b1/mM7y5_f-thumbnail-100-0.jpg
So I really need your help,.. I got some issue using a same vesc tool with vesc 6 or Fox I guess (I have to try with vesc 4.10 but I'm affraid its the same).
Here is the thing : 
All was all good using bldc tool with ack version 2.54 under bldc mode etc standard.
Then I try with fox, same all good too.
Now I need a lastest version of the official vesctool so I use one that I get with my V6, fw3.31 but there was any HW choice just the 60 once. 1st I try to force it by the custom files ... but I think I crap
asking a bootloader missing thing...
I bootload it by stlink, so now got vesctool 0.87 > fw3.34 > and here, no choice at all ?.. ok ... well its well connected, good version FW, HW and supported FW ...
Start the wizard and there motor detection failed itch time !! Haaaa, that never happen to me before !!! ever !

I try immediatly with an other fox of a single cruiser, all good, no pb I could reprogram it all.

What is the thing with this other fox ?
I try to increse D abit 0.01 by 0.01 but arrived to 0.07 and no result (I dont know much about that ... how high I could go, the help say to not go to high.) cause my motor make an unreal noize at the end :hushed: never see/hear that before !! Totaly freaky ... I try a new motor sensored lower kv ... same

Here are some screenshot : 
![Capturefoxfwsection|690x431](upload://9ikP7q1VtiWfHn4CPIwD836Ef17.JPG)

Config : 
(APS HEV 6374 170kv - old setup, but same issu) and 6374 130kv sensored
(vesc 4.10 - old setup), then Fox (cause BlackFriday...)
Lipo graphene 12s 8Ah
ADC control ...

**Thanks to all of you for any help guys** :blush: I may miss some info, don't hesitate please ..
```

---
## \#8 Posted by: Jamy Posted at: 2018-02-20T21:53:24.701Z Reads: 314

```
Reflash the original 2.XX firmware (using STLink), then open vesc tool and and install the bootloader when it asks and then upgrade without the custom files option.
```

---
## \#9 Posted by: Riako Posted at: 2018-02-21T01:29:04.106Z Reads: 314

```
thanks for your help Jamy !
So I re-reflash again, cause I already just made with the last files from benjamin.
It upgrade the fox to 3.34. And don't ask anymore about bootloard or other message for newer version etc. it's already working. But now with this one I don't pass the motor detection ... who is working before. And I also try with an other fox and it work fine. 
So like you say, how to reflash to the original fw2.18 from enertion/focbox ? 
I can dl the .hex file for this ?
```

---
## \#10 Posted by: driver Posted at: 2018-04-24T05:34:55.136Z Reads: 279

```
Hey @Jamy, where can i get the original Firmware?

I have the 4.8 FW on my focbox now and flashing the 4 from the tutorial didnt work out. 

Thanks!
```

---
## \#11 Posted by: Jamy Posted at: 2018-04-24T14:19:10.902Z Reads: 267

```
http://www.electric-skateboard.builders/t/where-can-i-find-the-vesc-2-18-firmware/23852/9?u=jamy

Install vesc_default.bin @driver
```

---
## \#12 Posted by: driver Posted at: 2018-04-24T20:15:22.135Z Reads: 256

```
Thanks alot @Jamy :grin:
I will try it tomorrow!
```

---
## \#13 Posted by: celica39 Posted at: 2018-06-11T03:28:22.436Z Reads: 239

```
hi, there , can i recovery a bricked vesc with this method because i have flash wrong hardware firmware  on my 4.10 vesc
```

---
## \#15 Posted by: Nanorider Posted at: 2019-01-04T06:32:01.548Z Reads: 176

```
anyone has link for HW60?
```

---
## \#16 Posted by: Nanorider Posted at: 2019-01-05T05:01:45.854Z Reads: 176

```
Ok i Have fixed the 2 Escapes by clearing the chip using the St Link tools.. then loading generic bootloader and then using Vesc Tool to upload their bootloader and their firmware then able to go across platform to Ackmaniac and back to Vesc which before I was not.
My issues was that the Escape had 3.38 version on and it would not upload new firmware.. Once I used St-Link utility it would upload latest firmware but I couldn't update firmware using Vesc Tool nor Ackmaniac Esc Tool.. only through ST-Link which was later fixed by clearing the data on the chip using the ST-LINK... use at your own discretion
```

---
## \#17 Posted by: Nanorider Posted at: 2019-01-05T05:02:30.674Z Reads: 173

```
some of the files I compiled into folder 

https://drive.google.com/drive/folders/1Yc7IKCECU4cz1LAiPgP-TPwnNLJXqwRI?fbclid=IwAR1shmuhBdCf6WmePWYsjzLJU4Po7ozFLCN3q2AZQq8LM-kmWzDq9_jjl28
```

---
## \#18 Posted by: trampa Posted at: 2019-01-05T17:18:20.965Z Reads: 171

```
If your VESC based ESC has no boot loader installed, you don't need a ST-Link to ad the bootloader. There is a bootloader tab in VESC-Tool (under firmware). Simply upload the missing bootloader via USB. 
A ST-Link is only needed when things got messed up.
```

---
## \#19 Posted by: Matt_54 Posted at: 2019-03-14T20:35:51.722Z Reads: 160

```
The link provided for the BLDC_4_Bootloader.hex file was not working and it took me a bit to find one that worked. I found the hex file on [this website](https://fishpepper.de/2017/10/31/tutorial-initial-flashing-a-new-born-vesc/) you can visit the website to get the zip or I will link it [here](https://www.dropbox.com/s/4mp6phkypx8hmuw/VESC_FW_AND_BL_092017.zip?dl=0).  I used the file "BLDC_4_BL_AND_MAIN_MERGED.hex" and it work on my vesc 4.12.
```

---
## \#20 Posted by: JdogAwesome Posted at: 2019-03-14T21:37:58.338Z Reads: 157

```
Thanks @Matt_54 I would update the link in the original post, but it's been to long so I can't change it anymore.
```

---
## \#21 Posted by: Fungineers Posted at: 2019-04-22T12:14:33.406Z Reads: 154

```
Guys, need help here. I tried this and ended up frying 2 stm32s.
I am using an stlink V2 programmer from ebay.
I connected as shown, 3.3, CLK, DIO, RST, GND, and all worked fine. The programmer connected to the stm32, and I could see all the memory allocations. So far so good. 

After a few seconds, the connection was terminated. So i reconnected, and thats when I saw it...the magic smoke, it escaped the stm32. I have heard that connecting the 3.3V could be problematic for VESC6 but I have a 4.12 so it should be fine?

Im really lost at what could be wrong here. Why would the programmer connect then disconnect. Sounds like a short circuit, but I checked all my connections and they look fine (no bridges). 

Any leads? (pun intended).
```

---
## \#22 Posted by: taz Posted at: 2019-04-22T12:24:56.106Z Reads: 142

```
You only need to connect DIO - GND - CLK and power the vesc normally through the battery.
```

---
## \#23 Posted by: Andy87 Posted at: 2019-04-22T12:49:42.096Z Reads: 143

```
If you have one working vesc you could flash the others via can bus as long as you use the newest firmware. I didn’t do that by my own yet, but @trampa for sure can let you know what to take care of if to do so.
```

---
## \#24 Posted by: Andy87 Posted at: 2019-04-22T12:51:39.305Z Reads: 139

```
And for the st link you can find a „how to“ also here:  
https://vesc-project.com/comment/225#comment-225
```

---
## \#25 Posted by: trampa Posted at: 2019-04-23T08:34:15.981Z Reads: 129

```
Never connect 3.3V on a China ST-Link clone! They fire 3.3V towards the chip, although the pin should be a voltage sniffer only, detecting if the chip is powered or not. GND, IO and CLK only.
```

---
## \#26 Posted by: Fungineers Posted at: 2019-04-23T09:08:01.109Z Reads: 134

```
Hey @Andy87 @taz @trampa thank you!

I had learnt that the 3.3V pin if connected to Chinesium stlinks only fries VESC6, but is OK with older versions, but apparently not.

So what I gather from your advices is connect the VESC through a bench power supply and connect GND CLK RST DIO? Will give it a go.
```

---
## \#27 Posted by: taz Posted at: 2019-04-23T09:17:46.562Z Reads: 132

```
No, only GND, IO and CLK.

Not RST.
```

---
## \#28 Posted by: Flasher Posted at: 2019-06-01T04:36:02.596Z Reads: 125

```
Anyone have insight on how to plug and use the nucleo64? Images on where to pin on the nucleo and where to pin on a flipsky dual vesc6.6 would be awesome. The master side of mine received the wrong hw/fw and I need to flash it back to life![IMG_20190531_200020523|375x500](upload://o0cy8k9D9yAWVbQ4L7IbnwFvzaR.jpeg) ![IMG_20190529_000352970|375x500](upload://cBzcaLYZPYe4meuarvcVWbOMEtM.jpeg)
```

---
## \#29 Posted by: trampa Posted at: 2019-06-01T06:38:58.204Z Reads: 117

```
You can flash the master via the slave. VESC-Tool had a SWD Prog feature. Interconnect gnd, Io, clk, on both SWDs. Open Vesc- tool, connect to working VESC, select SWD Prog menu on the left, hit connect, select vesc six, hit upload. 

Benjamin Vedder has a YouTube video up. Just search for him on YouTube.
```

---
## \#30 Posted by: Pimousse Posted at: 2019-06-01T06:47:48.694Z Reads: 115

```
Didn't work for @Manu39 and I (VESC couldn't find target, using FW3.57 on ESCAPE)
He had to buy a STLink though.
```

---
## \#31 Posted by: trampa Posted at: 2019-06-01T09:14:40.338Z Reads: 109

```
Should work. Both units powered, interconnect  IO, GND,CLK, ca. 8cm Long cable.
```

---
## \#32 Posted by: Pimousse Posted at: 2019-06-01T09:52:50.286Z Reads: 110

```
Should, but didn't.
Everything was set as it. 
I did it remotely with @Manu39, he has maybe more details to provide.
```

---
## \#33 Posted by: trampa Posted at: 2019-06-01T19:24:05.272Z Reads: 106

```
I hope this helps.

https://youtu.be/PFFiVxFHDM4
```

---
## \#34 Posted by: Flasher Posted at: 2019-06-01T19:34:01.228Z Reads: 104

```
I tried that but wasn't finding target :( it's why I went for the nucleo
```

---
## \#35 Posted by: Flasher Posted at: 2019-06-01T19:44:14.886Z Reads: 104

```
Btw can I use these one next to another or is the connector too big? I can't solder a full connector without removing the heatsink

https://www.amazon.ca/dp/B072L1XMJR/ref=cm_sw_r_cp_apa_i_4tT8Cb7A4S5VJ
```

---
## \#36 Posted by: Gamer43 Posted at: 2019-06-01T20:26:09.694Z Reads: 105

```
you will need a 5pin JST PH connector, believe me, I tried using standard jumper wires X_X.

Also, uploading video now, will tag and send to you on original thread once it's done uploading.

Wait, the SWD header is not populated on the dual...... hmmmmmm. You might be able to get away with soldering male jumpers. What I really like that Flipsky did is that the SWD pinout on their ESC follows the same pinout on the nucleo board's ST-link. Some smart people at Flipsky xDD.
```

---
## \#37 Posted by: Skyart15 Posted at: 2019-06-18T03:37:33.710Z Reads: 102

```
I am trying to connect to my Fsesc 6.6 but i get this error in the SWD prog screen. Do you have any idea what could be cousing this?![15608289824601578189988105241858|375x500](upload://oYYjrkIEEQI2P3j5R81mJoWRx5I.jpeg) ![1560828999634792459551862789929|375x500](upload://5pqbUfq920wZLEvhd0A3zTRBYcM.jpeg) 
I am trying to fix what looks like a bad bootloader on one side of my dual fsesc 6.6 greatly appreciate any help!
```

---
## \#38 Posted by: trampa Posted at: 2019-06-18T05:48:53.800Z Reads: 96

```
You need a working ESC and that needs the latest FW on. This ESC is then used to program the non working ESC. Interconnect both SWD ports: GND to GND, IO to IO, CLK to CLK. Then use SWD PROG feature to recover the non working ESC. 

You can also try and upload the bootloader via the bootloader tab in the Firmware menu. 
If that doesn't work, SWD PROG is the next step to take. 

This is third party hardware and customer support should be done via the vendor.
```

---
## \#39 Posted by: conquerco Posted at: 2019-07-03T05:17:21.277Z Reads: 84

```
I’m getting a blinking red light that flashes 3 times after being connected by ST Link. Nothing else is connected to the VESC, any ideas? it's a VESCX, my other VESCX connects just fine but not this one.
```

---
## \#40 Posted by: Micro Posted at: 2019-08-14T12:00:59.653Z Reads: 70

```
Did you find a solution. I have the same dual esc and changed one STM32. Getting the same error message ...couldnt connect to target.
The STM is from my miniquad with Betaflight Bootloader.:thinking:
```

---
## \#41 Posted by: Skyart15 Posted at: 2019-08-14T12:55:11.467Z Reads: 64

```
No I never figured it out, just gave up on it and ordered a metr pro
```

---
## \#42 Posted by: atlasdev Posted at: 2019-08-30T11:26:13.627Z Reads: 56

```
Does anyone know how the pinout works for the unity? I'm trying to follow this guide, but I can't find the required pins
```

---
## \#43 Posted by: auveele Posted at: 2019-10-07T07:19:52.377Z Reads: 36

```
I'm trying to do the same. I wanna flash the Focbox Unity because it doen't start.
Have you solved anything?
```

---
## \#44 Posted by: atlasdev Posted at: 2019-10-08T14:35:20.959Z Reads: 33

```
Hi there!

I don't know If this is the bootloader, but if it is I made a writeup of it. You can find it here: [How to fix a broken Unity bootloader](https://forum./t/how-to-fix-a-broken-unity-bootloader/9582).

Enertion is removing links to this site, so if the link suddenly breaks go to `forum (d0t) esk8 (d0t) news` and search for `How to fix a broken Unity bootloader`.
```

---
