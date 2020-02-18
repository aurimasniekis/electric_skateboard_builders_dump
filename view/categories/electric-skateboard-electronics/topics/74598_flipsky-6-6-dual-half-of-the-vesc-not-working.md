# Flipsky 6.6 dual - half of the VESC not working

### Replies: 28 Views: 1521

## \#1 Posted by: Steven1 Posted at: 2018-11-13T17:29:37.007Z Reads: 291

```
After finishing my electronics upgrade of my Evolve GT, I powered on the VESC and connected it to the VESC tool to set up the motors. Unfortunately, the left side of the VESC soon started flashing a red light and now won't turn on at all. The left green led does flash when powering up but stays off afterward. The VESC-tool also cant connect when I attach the USB-cable to this side of the VESC. 

When it was still flashing red, I tried to diagnose the problem in the VESC tool, but I didn't see any faults show up. Maybe I checked the wrong place?

I can't see any burn marks on the pcb or mosfets nor did I smell anything burn. 
Any help is much appreciated, I was sooo close! :(

Board Specs
10s4p Samsung 30q
Besttech HCX-223v1
Flipsky Dual 6.6
Metr pro module
Nano remote


![IMG_20181113_181707|666x500](upload://ijVMTcZ12Yft758i7Z1Z1nh1Qfc.jpeg) 

![IMG_20181113_181712|666x500](upload://eNIMLlqk30vJtPcOgRnlRt7ujJz.jpeg)
```

---
## \#2 Posted by: evoheyax Posted at: 2018-11-13T17:32:46.741Z Reads: 270

```
Yep, I have had the same issue with all 3 of my 6.6's. I would recommend staying away from them. You likely did nothing wrong. Unfortunately, only vesc 6 I trust is the official one, which frank charges an arm and a leg for. I burnt out 3, which is the cost of a vesc 6. So I really just lost in the end. Not worth it, just buy the real deal.
```

---
## \#3 Posted by: mackann Posted at: 2018-11-13T17:34:49.584Z Reads: 268

```
Do you get any error msg in the metr app? Like drv error?
```

---
## \#4 Posted by: Steven1 Posted at: 2018-11-13T17:35:30.954Z Reads: 263

```
Oh shit! Did you contact Flipsky about it? Did they offer you any compensation or offer to RMA it?
```

---
## \#5 Posted by: evoheyax Posted at: 2018-11-13T17:37:06.210Z Reads: 257

```
They offered to fix them. I will send them back to them. But I have to pay shipping to china, which is not cheap.

I have my sources that tell me its a design flaw. So I would stay away.
```

---
## \#6 Posted by: evoheyax Posted at: 2018-11-13T17:38:28.005Z Reads: 253

```
It fails to load the bootloader it seems... You can't connect, you just get a blue light, no red or green. It's either failing to load the bootloader it getting stuck.
```

---
## \#7 Posted by: Steven1 Posted at: 2018-11-13T17:40:10.970Z Reads: 247

```
Ahh can't remember, I'm trying to connect again right now
```

---
## \#8 Posted by: mtuan293 Posted at: 2018-11-13T18:01:21.554Z Reads: 237

```
You removed the heat shrink. Could it be possible that you sorted some of the components?
```

---
## \#9 Posted by: Steven1 Posted at: 2018-11-13T18:11:15.831Z Reads: 228

```
Dont think so, at least I cant see anything that's shorted on the board. When you say heatshrink do you mean the plastic cover of the vesc or the battery heatshrink?
```

---
## \#10 Posted by: Steven1 Posted at: 2018-11-13T18:12:03.645Z Reads: 227

```
Is there anything I can do to fix a bootloader? The green light does flash on at start up but stays off afterwards.
```

---
## \#11 Posted by: mtuan293 Posted at: 2018-11-13T18:12:31.283Z Reads: 224

```
[quote="Steven1, post:9, topic:74598"]
plastic cover of the vesc
[/quote]

Yeah I meant this
```

---
## \#12 Posted by: Steven1 Posted at: 2018-11-13T18:12:48.257Z Reads: 217

```
I guess the only option is to send it to China unfortunately...
```

---
## \#13 Posted by: Steven1 Posted at: 2018-11-13T18:18:57.286Z Reads: 215

```
Aha, well no visible sign of shorts at least. Here's two more close up pics:

![IMG_20181113_191637|666x500](upload://ws8vXk740kEZP1VA7KiWju21glR.jpeg) ![IMG_20181113_191633|666x500](upload://xN1cX5ybhHGvrSBgJNdtbFdjncl.jpeg)
```

---
## \#14 Posted by: evoheyax Posted at: 2018-11-13T23:13:00.039Z Reads: 199

```
I'm not quite sure what the problem is. I just know there is a design flaw. I can't tell you how I know, but it's true. Don't waste your money on it. Return it if you can and buy a better one.
```

---
## \#15 Posted by: Steven1 Posted at: 2018-11-14T07:42:37.201Z Reads: 180

```
I contacted them and they responded already so at least that's positive. It seems like I might have to reflash the firmware. Will keep this topic updated, might help others if it works.
```

---
## \#16 Posted by: riverside.rider Posted at: 2018-11-14T09:20:14.895Z Reads: 176

```
Hi @evoheyax: if you know what the design flaw is then perhaps you could let us all know so that This could be improved on in subsequent versions ?
```

---
## \#17 Posted by: linsus Posted at: 2018-11-14T09:25:21.939Z Reads: 177

```
flipsky is already in contact with BV, and donated a few hundred euros to him so far. 
BV gave them some design input, not sure what happened after that. Been pretty radiosilent.
```

---
## \#18 Posted by: Steven1 Posted at: 2018-11-26T15:36:59.852Z Reads: 171

```
Update, I sent my unit back to Flipsky and they sent me a replacement (has yet to arrive).
```

---
## \#19 Posted by: SkyTheEpic Posted at: 2018-12-03T23:03:27.734Z Reads: 161

```
How is the replacement holding up? I'm interested to know :slight_smile:
```

---
## \#20 Posted by: Steven1 Posted at: 2018-12-04T14:09:11.811Z Reads: 154

```
It just arrived. Might hook it up this weekend, will let you know.
```

---
## \#21 Posted by: brschaefer74 Posted at: 2019-02-28T13:29:18.218Z Reads: 121

```
I had the same issue happen to me after 3 days of riding. I just sent the unit back to them. Sounds like a design flaw.
```

---
## \#22 Posted by: bobyhack Posted at: 2019-09-18T07:00:06.179Z Reads: 59

```
Hi All , 
I had the same issue .The probem is flash memory coruption of the ARM .
It is a HW issue and can be cured with replaceemnt of the ARM.
Once replaced the chip should be flashed with the ST-Utility wil the default.bin (for vesc 6) .
Then the vesc should be rebooted and the USB port wil become operational .
After that you can just connect it to the vesc tool and upload the latest bootloader and FW .
The ARM chip is available at ebay for 5 pounds from China .
I already fixed mine and it is working as before .
```

---
## \#23 Posted by: JoelMatousek Posted at: 2019-10-15T23:45:14.662Z Reads: 51

```
How hard is that chip to replace? Could you send a link? My esc 6.6 just stopped working, won't connect or anything. Blue light stuck on, nothing else
```

---
## \#24 Posted by: bobyhack Posted at: 2019-10-16T07:29:15.155Z Reads: 47

```
https://www.ebay.co.uk/itm/Original-STM32F405RGT6-chip-microcontrollers-32-bit-1MB-flash-memory-LQFP-64/253121350700
```

---
## \#25 Posted by: bobyhack Posted at: 2019-10-16T07:29:41.539Z Reads: 46

```
https://www.ebay.co.uk/itm/ST-Link-V2-Stlink-Emulator-Downloader-Programming-Mini-Unit-STM8-STM32-doETP/401912048397?_trkparms=ispr%3D1&hash=item5d93d32b0d:g:kYoAAOSwUxhbN53u&enc=AQAEAAACMBPxNw%2BVj6nta7CKEs3N0qX0%2B6pC1Phu65NRHRti%2BOuREQgpuieHuJDiwLsnFsGIrFDvmqphkYUFBIniNusp5XYo2vu2OtP2JzeUqhPrntkm4om47vUC%2BvH2UB5UFeX7fV1g0AkxuRlp8iyAVz5nZw8%2B0nBL6AyBvHd22EZrqh8XGtPsToilx%2BjD%2FtZdwqm9w3pdJgf5s3XMs%2FIwzQyT5zs5oHpHnb4OVDrhyww4wQNS%2FMLdTR4yDdKMaruz6%2Fmp3ulVz4jgz5V3OnSDuvt0JZHkJ50wnrkVKpV6y6AOlmNXqopDT5StM%2FHCZLKXDZ%2BydHlgF8E1q20RPQxKTbL%2FY4lrtUMmba7bjkkE5pZ%2BrhcLp66aOLX%2F7hVIUZ6lXSX%2BdhoWpFGFzAbqCdC0OVWwxWMvlqpq7M%2BFm8oYG37QQO2zIT6JDOiJkI3pOro3fp872meGaVdtwUbfgEO0o8uKngQku5wAkCWgIo6EEgO1E3lcE0BHqw7ruuQjhHxRbA0q6B3nmzqK0c%2BZSgFIDHmjtXavVQFfEZMDEtQKRUYXvk8Q0LpAwcOPl%2FU4wo4AA0YOIDWJBOx4JzqOx%2BgmCm2MRYdAWy8hzJr9y6TroiSiySsuMpjOzQDjYpIhRwl3PGRyG7lGuIC4TbhjXprRKuR6FwzXdHW6lfVv2rFPoMZJHfPeQtJtl%2FZP1EdGEG3X49AREZ5mn%2B0kYedzQ3cYhZy756gs1LyA5qzqfJp9XTX5CQjq&checksum=40191204839767db3fac52514891a6c3edfb99aead28&enc=AQAEAAACMBPxNw%2BVj6nta7CKEs3N0qX0%2B6pC1Phu65NRHRti%2BOuREQgpuieHuJDiwLsnFsGIrFDvmqphkYUFBIniNusp5XYo2vu2OtP2JzeUqhPrntkm4om47vUC%2BvH2UB5UFeX7fV1g0AkxuRlp8iyAVz5nZw8%2B0nBL6AyBvHd22EZrqh8XGtPsToilx%2BjD%2FtZdwqm9w3pdJgf5s3XMs%2FIwzQyT5zs5oHpHnb4OVDrhyww4wQNS%2FMLdTR4yDdKMaruz6%2Fmp3ulVz4jgz5V3OnSDuvt0JZHkJ50wnrkVKpV6y6AOlmNXqopDT5StM%2FHCZLKXDZ%2BydHlgF8E1q20RPQxKTbL%2FY4lrtUMmba7bjkkE5pZ%2BrhcLp66aOLX%2F7hVIUZ6lXSX%2BdhoWpFGFzAbqCdC0OVWwxWMvlqpq7M%2BFm8oYG37QQO2zIT6JDOiJkI3pOro3fp872meGaVdtwUbfgEO0o8uKngQku5wAkCWgIo6EEgO1E3lcE0BHqw7ruuQjhHxRbA0q6B3nmzqK0c%2BZSgFIDHmjtXavVQFfEZMDEtQKRUYXvk8Q0LpAwcOPl%2FU4wo4AA0YOIDWJBOx4JzqOx%2BgmCm2MRYdAWy8hzJr9y6TroiSiySsuMpjOzQDjYpIhRwl3PGRyG7lGuIC4TbhjXprRKuR6FwzXdHW6lfVv2rFPoMZJHfPeQtJtl%2FZP1EdGEG3X49AREZ5mn%2B0kYedzQ3cYhZy756gs1LyA5qzqfJp9XTX5CQjq&checksum=40191204839767db3fac52514891a6c3edfb99aead28
```

---
## \#26 Posted by: bobyhack Posted at: 2019-10-16T07:31:32.867Z Reads: 47

```
Any GSM repair shop can replace the chip .You will need the ST-Link to dump the flash from the working chip or you can download the bin from vedder github .
With the ST-link you can flash the empty chip .The USB port is not active until you flash it .
```

---
## \#27 Posted by: Voxu Posted at: 2019-10-16T08:50:03.605Z Reads: 47

```
No worries dude XD I fried the whole VESC too? or Did I? I found that sensors from the motors were the factor of fucking up one side then another. Now I only got blue lights on both sides which indicate that the 5V is present but 3,3V is not. After some brainstorming on a discord server we came to a conclusion that the MCU needs to be replaced. And maybe you will need to flush the memory with an ST-Link. Check if the 3,3V is present on the non working side. If not, it's the MCU. Also unplug the sensor wires.
```

---
## \#28 Posted by: SheldonTrever Posted at: 2019-10-16T14:15:10.129Z Reads: 36

```
Is it an DRV error or anything else???
```

---
