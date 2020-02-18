# VESC not connecting via usb, only blue led on

### Replies: 32 Views: 5108

## \#1 Posted by: Stefan Posted at: 2016-09-26T21:24:26.215Z Reads: 308

```
Hey everyone,

I got a Magneto Board a few days ago and it already stopped working the same day. I ordered a VESC from enertion and wired it up. But when i try to connect it via usb, it does not pop up on my pc and bldc also does not recognize the VESC. When i power it up only the blue led is glowing but no green led (this needs to be if the VESC is working fine?).

I'm new to the whole electric skateboarding thing and i have no clue why the VESC does not connect to my pc..
```

---
## \#2 Posted by: Jobbel Posted at: 2016-09-26T23:29:11.880Z Reads: 301

```
Most likely you are missing the Bootloader/Firmware. It happened with my last VESC from enertion too. 
Depending on your experience with Linux it can be rather hard getting it to work again.
You need to get a Linux PC (I'd reccomend Ubuntu) and a stm32 Programmer in order to upload the firmware.
A suitable Programmer : 

http://www.ebay.de/itm/Neu-ST-Link-V2-Mini-Metal-Shell-STM8-STM32-Programmer-Emulator-Downloader-/121507212413?hash=item1c4a64ec7d:g:JpIAAOSwGvhT6iIl

How to connect the Programmer to the VESC:

http://vedder.se/2014/12/connecting-a-programmerdebugger-my-custom-stm32-pcbs/

The instruction Video by vedder:

https://www.youtube.com/watch?v=17CSl1iXYE8

but be careful you cannot use the terry private Repository for building the Toolchain
use this ubuntu one instead:

http://packages.ubuntu.com/de/trusty/gcc-arm-none-eabi

And yes normally the LED next to your blue one should flash 3 times on startup, indicating no errors
```

---
## \#3 Posted by: Blasto Posted at: 2016-09-27T01:21:04.020Z Reads: 269

```
Bootloader is for reprogramming the firmware via usb. This is not the problem here.

Make sure you have the correct com port on the bldc tool
```

---
## \#4 Posted by: Jobbel Posted at: 2016-09-27T01:25:26.180Z Reads: 258

```
If the VESC gets power, the red LED HAS to flash 3 times, otherwise there is no software programmed onto the stm32 microcontroller. In this case you cannot reprogram the firmware via usb because bldc tool wont be able to connect to the stm at all.
Your only possible way of saving the VESC is to program it with a hardware programmer
```

---
## \#5 Posted by: Blasto Posted at: 2016-09-27T01:37:03.138Z Reads: 248

```
Well let's @Stefan give us more info, jumping to missing firmware is worse case
```

---
## \#6 Posted by: Jobbel Posted at: 2016-09-27T02:13:54.307Z Reads: 240

```
[quote="Stefan, post:1, topic:10184"]
When i power it up only the blue led is glowing
[/quote]

Sadly there is almost no other explanation to this.
The other possibilities are broken LEDs, broken LED traces or voltage issues.
I am quite certain the firmware is missing
```

---
## \#7 Posted by: zmoney Posted at: 2016-09-27T02:17:40.215Z Reads: 228

```
Firmware is def. missing.  Flashing a Vesc is not extremely difficult, I bet you can do it yourself. All the code you need is on Vedder's [site](http://vedder.se)
```

---
## \#8 Posted by: JohnnyMeduse Posted at: 2016-09-27T02:50:30.926Z Reads: 228

```
Please contact your vendor... It is really the best thing to do in these kind of situation...
```

---
## \#9 Posted by: Stefan Posted at: 2016-09-27T14:57:27.050Z Reads: 228

```
Hey everyone,

first of all, thanks for your quick responses.
@Jobbel I orderd this one [https://www.amazon.de/gp/product/B012VR3PVA/ref=oh_aui_detailpage_o03_s00?ie=UTF8&psc=1](https://www.amazon.de/gp/product/B012VR3PVA/ref=oh_aui_detailpage_o03_s00?ie=UTF8&psc=1) from amazon. Delivery needs only a few days. I am still a little confused on how to connect everything together for the flashing process but i made a foto of the vesc

<img src="/uploads/db1493/original/3X/5/6/56d334f722111411cb1d3934b6eb0812768276c4.jpg" width="487" height="500">

Moreover i am not sure how to connect the bluetooth receiver to the vesc. Is it the 3 pins i gave the number 1 or do i have to connect it to the area i gave the number 2? Or neither of them :D
```

---
## \#10 Posted by: Jobbel Posted at: 2016-09-27T15:21:02.134Z Reads: 205

```
Hey Stefan

if your bluetooth receiver is a nunchuck you'll have to connect it at pin header 2
if it is a RC receiver with a PPM Signal you have to connect it to pin header 1
to program your VESC you have to hook up your stlink programmer to the only 
pinheader you didn't mark, it's the one between 1 and 2, it should have 6 pins. On the other side of the board you can see what to connect where
```

---
## \#11 Posted by: Stefan Posted at: 2016-09-27T15:26:12.010Z Reads: 197

```
I think it is a RC receiver. I am not familiar with nunchuck but these have more than 3 cables, right?
Will it be enough to install an Ubuntu on something like a virtual machine on my laptop?
```

---
## \#12 Posted by: Jobbel Posted at: 2016-09-27T15:40:13.926Z Reads: 192

```
you could even make a bootable USB drive or CD (i'd recommend this tool: http://www.linuxliveusb.com/download), a virtual machine should work as well
And if it is an RC one with 3 Pins you have to connect it to Pin Header 1
```

---
## \#13 Posted by: Stefan Posted at: 2016-09-27T17:29:33.182Z Reads: 187

```
I installed Ubuntu on a virtual machine now. Hopefully the adapter will come thursday or friday.
```

---
## \#14 Posted by: Stefan Posted at: 2016-09-27T18:14:56.369Z Reads: 181

```
Update:
I followed all the steps mentioned in vedders video until 4:40 when it comes to connecting the vesc. Since i did not know what i was doing with those commands i did not recognize any errors/problems. @Jobbel you said i could not use the terry private Repository for building the Toolchain. I think i did that with following the steps mentioned in the video, right? I had no problems with that, is it still wrong this way?
```

---
## \#15 Posted by: Jobbel Posted at: 2016-09-27T22:29:22.683Z Reads: 178

```
what happens if you type make inside the BLDC-firmware folder ?
If it compiles OK you are fine, if not you need the Toolchain
```

---
## \#16 Posted by: Stefan Posted at: 2016-09-27T23:16:16.300Z Reads: 175

```
You mean like this?

<img src="/uploads/db1493/original/3X/2/6/26a4dacd38609c6ab6d37d785337c0ad94217b14.png" width="690" height="412">

I installed Ubuntu in german so the terminal also is in german..
But i assume you meant this. What do i have to do differently?
```

---
## \#17 Posted by: Jobbel Posted at: 2016-09-28T13:47:27.448Z Reads: 168

```
I'll answer in german :

Ja dir fehlt die Toolchain deshalb steht da in der letzten Zeile auch dass das compilieren scheiterte. Du muss dir auf dem Ubuntu Rechner http://packages.ubuntu.com/de/trusty/gcc-arm-none-eabi das hier für deine Architektur runterladen.(AMD oder Intel)
dann einfach ausführen, Ubuntu installiert das von alleine. Dann nochmal make in dem bldc-firmware Verzeichnis ausführen, sollte dann anders aussehen :smiley:
kannst dann auch mit make upload direkt auf die VESC schreiben solltest du den Programmer schon haben


Edit: You are missing the Toolchain. you can download it here:
http://packages.ubuntu.com/de/trusty/gcc-arm-none-eabi
just download the .deb file and execute it, ubuntu will install it automatically
make upload should now work
```

---
## \#18 Posted by: Stefan Posted at: 2016-09-28T17:12:02.489Z Reads: 162

```
Praktisch. Das habe ich jetzt gemacht und sieht auch soweit gut aus. Der Programmer kommt morgen oder übermorgen voraussichtlich. Kann ich dann als nächstes nach dem Anschließen des Programmers direkt make upload machen und dann ist die firmware drauf, sodass ich den Rest über die "normale" Windowsoberfläche mit dem BLDC Tool machen kann? Oder muss ich danach noch etwas in Ubuntu machen? Im Video macht er ja danach noch weitere Anweisungen im Terminal.
```

---
## \#19 Posted by: DeathCookies Posted at: 2016-09-28T17:56:22.992Z Reads: 159

```
Please keep the language to english only that everyone can understand what you are talking about and that others can learn! If you really want to speak german please make a private message ;)
```

---
## \#20 Posted by: Jobbel Posted at: 2016-09-29T11:49:11.781Z Reads: 158

```
No once the firmware is properly flashed on the VESC you can use the BLDC tool again :smiley:
And yes if the programmer is connected you can directly execute make upload
Because you use a VM you will have to do some usb routing for the  programmer
ok I ' ll try to keep it in english
```

---
## \#21 Posted by: Stefan Posted at: 2016-09-29T17:07:04.241Z Reads: 152

```
I made a picture with the connections of the programmer and the connections on the vesc:

<img src="/uploads/db1493/original/3X/a/5/a50cb4c64b7ff3c776136206cc876cd6512f1ffa.jpg" width="690" height="399">

Am i right with these connections? And which one do i have to connect for pins 4 (dio) and 5 (rst)?
```

---
## \#22 Posted by: Jobbel Posted at: 2016-10-02T17:03:04.224Z Reads: 151

```
I think you have to connect DIO to pin 6 of your Programmer
And I also connected the NC one to Ground.

Use this Picture as a reference 

http://vedder.se/wp-content/uploads/2014/12/EbayStlink_small.jpg

The green cable on the Programmer is 3.3 V or Pin 1 on your VESC
I'd use the SWIM RST btw
```

---
## \#23 Posted by: Stefan Posted at: 2016-10-02T18:19:45.047Z Reads: 142

```
I successfully flashed the vesc. Thanks everyone.
```

---
## \#25 Posted by: kien Posted at: 2017-04-16T00:01:34.303Z Reads: 117

```
Hi everyone,

I've got a VESC 4.12 recently and I succeeded in connecting to BLDC Tool in Windows and making the motor move using BLDC sensorless mode by following the tutorials on Youtube. 

Today, however, it doesn't work anymore, no led on, even the blue one and the L1-220 (near the CAN Bus) is very hot when VESC is connected to battery. I might have made an error by connecting the battery to the VESC before connecting it to the PC... 

Do you know what wrong with my VESC? Should I flash the VESC again as @Stefan did or anything else?

Thanks you guys for help!
```

---
## \#26 Posted by: PDXroses Posted at: 2017-12-06T01:17:38.550Z Reads: 80

```
I'm so glad I stumbled onto this post.  Is it possible to install the bootloader/firmware with my Mac?  I bought an STM32F4 discovery board.  Thanks for any tips you can provide.
```

---
## \#27 Posted by: GrecoMan Posted at: 2017-12-06T01:20:37.421Z Reads: 79

```
you don’t even need a boot loader anymore 😮

just download VESC-Tool and do it from there
```

---
## \#28 Posted by: PDXroses Posted at: 2017-12-06T01:25:43.641Z Reads: 78

```
Wow.  My MCU is blank.  The VESC Tool will get it to work?  Thanks!
```

---
## \#29 Posted by: GrecoMan Posted at: 2017-12-06T01:30:00.694Z Reads: 81

```
You can upload a boot loader through the vesc tool and flash the firmware from there
```

---
## \#30 Posted by: PDXroses Posted at: 2017-12-06T01:31:06.733Z Reads: 83

```
Thank you so much.  Where do I get a bootloader?  Is there a specific version I should get?
```

---
## \#31 Posted by: PDXroses Posted at: 2017-12-06T01:32:34.632Z Reads: 83

```
It looks like the VESC Tool doesn't have a Mac version.  True?
```

---
## \#32 Posted by: JohnnyMeduse Posted at: 2017-12-06T02:16:20.469Z Reads: 83

```
@PDXroses http://www.electric-skateboard.builders/t/vesc-6-released-and-the-forum-is-open/32265/28?u=johnnymeduse :wink:
```

---
## \#33 Posted by: Brando Posted at: 2018-02-12T02:59:02.715Z Reads: 73

```
I am getting this same error when I try "make upload". When I try to install the .deb file, it says a newer version is already installed. Does anyone know the issue?
```

---
