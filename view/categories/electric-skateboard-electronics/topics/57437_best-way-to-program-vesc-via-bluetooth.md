# Best way to program VESC via bluetooth

### Replies: 28 Views: 4895

## \#1 Posted by: Naysh Posted at: 2018-06-01T03:06:11.702Z Reads: 520

```
What's everyone doing to program their VESC via bluetooth? I got a focbox and an HM 10 module. I have Vesc tools installed on my PC but hate having to lay my board on top each time.
```

---
## \#2 Posted by: Deckoz Posted at: 2018-06-01T03:14:45.004Z Reads: 519

```
I use a metr.at module which supports tcp bridging through your phone.
```

---
## \#3 Posted by: Cobber Posted at: 2018-06-01T03:30:30.564Z Reads: 517

```
I've been thinking of putting the bread and honey down for a metr.at module, I have a couple hm10 modules from scepy... but :thinking: 

I won't need my pc at all then will I?
```

---
## \#4 Posted by: lock Posted at: 2018-06-01T03:38:33.687Z Reads: 510

```
The VESC Tool supports Bluetooth natively now, but only if you're running Linux (Ubuntu) or Android. You'll need a Bluetooth 4 USB dongle if your PC doesn't have it built in.

On the VESC (Focbox) side you'll need a [*programmed* nrf51](https://github.com/vedderb/nrf51_vesc), or you can go for the [easy/expensive option Trampa provides](http://www.trampaboards.com/vesc-connect-wireless-dongle-p-25516.html).  You wont have to program the Trampa module, but note the VESC 6 and Foxbox have different connectors so it may not be plug and play.
```

---
## \#5 Posted by: Mathias Posted at: 2018-06-01T03:46:32.551Z Reads: 491

```
Or, you can flash Benjamin's custom firmware yourself. You'll need this module:
https://www.ebay.com/itm/Low-Power-Consumption-BLE4-0-Bluetooth-2-4-GHz-Wireless-Module-NRF51822/400970594571?epid=1045077976&hash=item5d5bb5b90b:g:7n8AAOSwImRYTg8o
And this to flash the firmware:
https://www.ebay.com/itm/ST-Link-V2-Mini-STM8-STM32-STLINK-Simulator-Download-Programming-Unit-with-Cover/322478832246?ssPageName=STRK%3AMEBIDX%3AIT&_trksid=p2060353.m2749.l2649

All you need to know is written here:
https://vesc-project.com/node/234

I just did it and it was super easy. I can only speak for Linux, though. VESC tool via bluetooth works perfectly on my (Linux) laptop and Android phone.
```

---
## \#6 Posted by: onepunchboard Posted at: 2018-06-01T04:15:08.693Z Reads: 433

```
btw android 8.0 and after does not support metr, just a fair warning.
```

---
## \#7 Posted by: trampa Posted at: 2018-06-01T05:07:17.081Z Reads: 418

```
Easy when you have Linux. The majorities can't flash a module. This is why me made some. Since we didn't start with 1000Units, price is not super low, but acceptable.

Frank
```

---
## \#8 Posted by: RyuX Posted at: 2018-06-01T07:16:30.424Z Reads: 396

```
metr.at App with the Bluetooth Module and TCP Bridge is the best and easiest way. Makes things so easy - never had to open my enclosure
```

---
## \#9 Posted by: Sebike Posted at: 2018-06-01T07:22:20.705Z Reads: 384

```
Since yesterday (?) Ackmaniac's app supports this feature as well. 

Connect your laptop VESC-tool to your app that's connected to your BT-module.

https://www.electric-skateboard.builders/t/vesc-monitor-android-app/20888/646
```

---
## \#10 Posted by: RyuX Posted at: 2018-06-01T08:03:57.268Z Reads: 362

```
Also when I am on outside i use "perimetr" app to directly change VESC Settings and save them to the VESC. Saved me much trouble
```

---
## \#11 Posted by: lock Posted at: 2018-06-01T08:08:22.360Z Reads: 347

```
Can you do firmware uploads and real time data via a HM-10 and TCP bridge?

Firmware upload takes about a minute on a nrf51, that works out to be 12 minutes at HM-10 speeds.
```

---
## \#12 Posted by: Mathias Posted at: 2018-06-01T08:36:13.592Z Reads: 327

```
I'd say when it comes to configuring, VESC tool with NRF is the real deal. You connect on your laptop or the phone to any of your VESCs that's connected via CAN with the actual vesc tool. Super handy for testing things on the road instead of on the bench...
What is really still missing is a good realtime display. I think Benjamin is still working on that. 
For the moment I still have the HM-10 for Ackmaniac's realtime display connected to the Slave-FOCBOX, and NRF for VESC tool on the Master. I won't give up either right now.
```

---
## \#13 Posted by: trampa Posted at: 2018-06-01T09:36:09.367Z Reads: 315

```
That is because Benjamin coded a cutom FW for the NRF51822, knowing what he is doing, getting the root problems nailed first.

Quote Vedder on https://vesc-project.com/node/234:
> This is because it is not simply an USB-UART bridge, it also decodes and encodes the packets to get the maximum possible throughput and reliability.

Frank
```

---
## \#14 Posted by: Slak Posted at: 2018-06-01T10:59:26.678Z Reads: 297

```
Limitations on Ackmaniac new feature :
[quote="Ackmaniac, post:651, topic:20888"]
No firmware updates won’t work. Over Bluetooth it happens that packages get lost. And for a firmware update it needs to deliver like 20000 packets. So that won’t work. But motor detection, and read and write of settings works.
[/quote]
```

---
## \#15 Posted by: Ackmaniac Posted at: 2018-06-01T11:13:44.164Z Reads: 286

```
I don't think that firmware updates work on the others via Bluetooth. 
And if somebody says the opposite then please only do so when you tested it yourself.
And when you have a different Baudrate than the standard that comes with the firmware then you are fucked anyway because the connection won't work.
```

---
## \#16 Posted by: trampa Posted at: 2018-06-01T11:28:55.909Z Reads: 287

```
Doing it all the time! Works a treat with new module. 90 seconds, job done.
```

---
## \#17 Posted by: Kug3lis Posted at: 2018-06-01T12:15:49.982Z Reads: 284

```
STM32 has UART bootloader but you need to set BOOT pins which arent breaked out of package on pcb... 

http://www.st.com/content/ccc/resource/technical/document/application_note/b9/9b/16/3a/12/1e/40/0c/CD00167594.pdf/files/CD00167594.pdf/jcr:content/translations/en.CD00167594.pdf
```

---
## \#18 Posted by: lock Posted at: 2018-06-01T12:23:13.055Z Reads: 276

```
Yep, firmware update worked perfectly the 4 times I've done it. Two times on two different VESCs, with 2 of those updates via CAN fwd. 

I'm guessing it's no accident that the nrf firmware Vedder wrote also adopts the VESC default baud rate.
```

---
## \#19 Posted by: Ackmaniac Posted at: 2018-06-01T12:27:17.457Z Reads: 278

```
NRF isn't bluetooth.

@Kug3lis are you trying to explain to me that it is possible to upload a firmware via UART?

@lock Edit: Now i see that he he did it for NRF51822 modules and he also changed the behavior of the VESC-Tool when bluetooth is connected. In that case it might work. Didn't have a look at this implementation.
Last time i worked with NRF modules were with NRF24L01 which work different.
```

---
## \#20 Posted by: lock Posted at: 2018-06-01T12:32:48.428Z Reads: 275

```
The nRF51822 supports Bluetooth Low Energy and the other non-Bluetooth protocols. My MacBook can talk to my skateboard, and I'm fairly certain it only does Bluetooth :wink:
```

---
## \#21 Posted by: Ackmaniac Posted at: 2018-06-01T13:11:53.153Z Reads: 265

```
LOL, when i look in the mirror i see a stupid fool.

Tested firmware update with my app and the bluetooth module via PC over TCP connection and it worked.
Takes like 5 minutes because of the slow baud rate but it works.

Can't really believe it myself and don't recommend it but...

Good think is that i changed the default baudrate in my firmware to 9600 so it works with standard hm-10 modules.
```

---
## \#22 Posted by: lock Posted at: 2018-06-01T13:42:55.552Z Reads: 260

```
[quote="Ackmaniac, post:21, topic:57437"]
Can’t really believe it myself and don’t recommend it but…
[/quote]

Is it really such a bad idea though? 

Based on my 'possibly flawed' understanding each firmware update packet is written to some other (unused) part of the flash, and it's only if all packets are successfully written that the bootloader will be told to overwrite the actual firmware. If it was to fail halfway through the upload and you got a timeout error then there'd be no harm done as you've just written to an unused part of the flash anyway (that would be overwritten next update attempt). To get a timeout in the first place a single packet must fail 5 times, and this gets reset if a packet gets through. Corrupted data is unlikely to get through due to the crc check performed by the VESC.

The risky part I see is when the bootloader replaces the VESC firmware with what has been uploaded, but that's all done on the VESC so shouldn't matter if it's initiated via USB or BT. If this fails halfway through, then yeah you're going to have to break out the st-link.

It takes a lot longer than 5 minutes to get my enclosure off and on again!
```

---
## \#23 Posted by: Ackmaniac Posted at: 2018-06-01T13:53:57.729Z Reads: 236

```
I see you understood it. But for many others there are a lot of questions and misunderstandings. Like updating the slave over CAN and saving the data in a xml when parameters changed as well. And then when the modules have another baudrate. For example vedders BLE modules wouldn't work with my firmware after the update because i use 9600. It would be easy to have 115200 as well but then people need to be able to change the baudrate on the modules themself. And that is too much for the most. But maybe i can add the baudrate change in the ACKMANIAC-Tool for common modules.
```

---
## \#24 Posted by: Kug3lis Posted at: 2018-06-01T14:52:57.845Z Reads: 233

```
Inside each STM32 there is internal system memory with bootloader which gets triggered using BOOT pins so you can use: USB, UART, CAN, I2C, SPI or some other protocols to program STM32

I found this tool which implements ST protocol for UART and I2C

https://sourceforge.net/projects/stm32flash/
```

---
## \#25 Posted by: Naysh Posted at: 2018-06-01T17:13:46.320Z Reads: 229

```
I wish i knew about metr.at before buying my HM-10 modules.  I definitely go metr.at route next time.
```

---
## \#27 Posted by: hexakopter Posted at: 2018-06-05T20:54:36.280Z Reads: 219

```
[quote="Naysh, post:25, topic:57437"]
I wish i knew about [metr.at ](http://metr.at) before buying my HM-10 modules. I definitely go [metr.at ](http://metr.at) route next time.
[/quote]
I deleted my post of the countdown to Metr Pro release. You can now find all the information about it here: [http://www.electric-skateboard.builders/t/metr-pro-next-gen-bluetooth-module/57780/](http://www.electric-skateboard.builders/t/metr-pro-next-gen-bluetooth-module/57780/)
You will see there that you can update your VESC firmware with Metr Pro directly with the Metr App over the air. Its also possible to use the VESC Tool desktop or mobile app for updating with the mentioned module.
```

---
## \#28 Posted by: Fiddler Posted at: 2019-06-21T03:47:33.132Z Reads: 73

```
I brought 2 Trampa for my 4.1 Vesc.  My Android vesc tool can find the BT but then i get Error " Cant read firmware". Can someone help me ?
```

---
## \#29 Posted by: Fiddler Posted at: 2019-06-21T05:28:03.202Z Reads: 68

```
Got it. I had adc mode only.i have to activate ppt and uart First to pair .then i can change to adc und uart .
```

---
