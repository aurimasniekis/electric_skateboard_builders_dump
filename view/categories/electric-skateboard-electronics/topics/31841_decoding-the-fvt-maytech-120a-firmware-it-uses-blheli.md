# Decoding the FVT/Maytech 120A firmware (it uses BLHeli)

### Replies: 16 Views: 1704

## \#1 Posted by: kaspars Posted at: 2017-08-30T08:52:30.137Z Reads: 176

```
During the weekend I managed to capture the UART traffic used by the FVT USB Link software to upload the [latest firmware revision 170818](http://szfvt.com/en/download-6.html) to the Favourite 120A 12S ESC (also known as Maytech MTES 120A SBEC) and noticed a `#Skywalker20A#` string in the [byte sequence](https://gist.github.com/kasparsd/cd132a5a0d313a249f8dcc3078f357af#file-firmware-update-csv-L15040-L15053) right at the end of the firmware upload:

<img src="/uploads/db1493/original/3X/f/a/faa88b65c13f1e682ed33fa167a8ffb210fce3b3.png" width="690" height="335">

With a bit more work I managed to figure out that their `HGM` firmware files have all bytes XORed with `0x68`. And with that I could decode the full firmware and notice multiple references to the [BLHeli firmware](https://github.com/bitdump/BLHeli).

Here is the full write-up on how I did that:

https://kaspars.net/blog/electronics/fvt-firmware
```

---
## \#2 Posted by: Okami Posted at: 2017-08-30T20:48:37.105Z Reads: 152

```
Nice job, i still got to read your article but would it be possible to access more config options since u have decoded it?
```

---
## \#3 Posted by: Deckoz Posted at: 2017-08-31T13:54:11.765Z Reads: 138

```
Have you tried connecting to the c2 pin? You should be able to connect it to blheli suite.
```

---
## \#4 Posted by: kaspars Posted at: 2017-09-01T08:56:01.234Z Reads: 136

```
Here is the byte sequence when reading the settings:

```
Time [s], Analyzer Name, Decoded Protocol Result
0.895004240000000,Async Serial,'225' (0xE1)
0.895564400000000,Async Serial,'225' (0xE1)
0.909020840000000,Async Serial,'227' (0xE3)
0.909556370000000,Async Serial,'3' (0x03)
0.910088380000000,Async Serial,'3' (0x03)
0.910620390000000,Async Serial,'1' (0x01)
0.911152390000000,Async Serial,\t (0x09)
0.911684400000000,Async Serial,'0' (0x00)
0.912216410000000,Async Serial,'2' (0x02)
0.912748420000000,Async Serial,'4' (0x04)
0.913280420000000,Async Serial,'0' (0x00)
0.913812410000000,Async Serial,'1' (0x01)
0.914344420000000,Async Serial,'3' (0x03)
0.914876430000000,Async Serial,'1' (0x01)
0.915408430000000,Async Serial,@ (0x40)
0.915940440000000,Async Serial,'0' (0x00)
1.071019510000000,Async Serial,'225' (0xE1)
1.071550400000000,Async Serial,'225' (0xE1)
```

I haven't figured out the protocol, yet. There seem to be [13 settings in the UI](http://www.electric-skateboard.builders/t/maytech-12s-esc-new-firmware-to-fix-the-brakes/13545/78) which is exactly the number of bytes after the `0xE3` request, I think.
```

---
## \#5 Posted by: kaspars Posted at: 2017-09-01T08:58:58.714Z Reads: 128

```
> Have you tried connecting to the c2 pin?

Not yet. I'm still waiting for some parts to build a proper connector for those tiny pads:

https://www.flickr.com/photos/kasparsdambis/28427575405/
```

---
## \#6 Posted by: Deckoz Posted at: 2017-09-01T10:45:35.990Z Reads: 123

```
Ah, I use a pogo pin/needle board setup as its modular and can work across many projects

<img src="/uploads/db1493/original/3X/7/7/7781ac8a68315ae575022814cee49253817bf0b2.jpg" width="690" height="457">
```

---
## \#7 Posted by: kaspars Posted at: 2017-09-01T14:49:39.727Z Reads: 117

```
Wow, that looks awesome! Is that an AVRISP "connector" :slight_smile: (based on the number of pins)?
```

---
## \#8 Posted by: Deckoz Posted at: 2017-09-01T14:59:07.249Z Reads: 114

```
yea thats correct. this was before 1 wire bootloaders were prevalent in most drone ESC's. but it can be adopted for many things. like make shift SWD connectors, or if you only had pads for stlink, testing traces on a pcb...ect
```

---
## \#9 Posted by: kaspars Posted at: 2017-09-01T15:02:35.291Z Reads: 120

```
Tried reading the `0x0000-0x3DFF` memory region (via C2) and got back only zeros -- it must be locked. The BLHeliSuite confirmed that.

<img src="/uploads/db1493/original/3X/a/5/a53abb2294c4976971f936172130f3796651d8ae.png" width="620" height="500">

And BLHeliSuite doesn't seem to recognise the UART response when reading the setup parameters so it might be a completely modified version of BLHeli.
```

---
## \#10 Posted by: Deckoz Posted at: 2017-09-01T15:05:14.319Z Reads: 120

```
Try with an older 14xx version of blheli suite, i doubt the ESC is running 16.xx BLHELI_S. :)

That is interesting that the memory is locked though... You should still be able to pull version information off of the ESC however.

Also normally with BLHELI the memory is stored/flashed as the 13th page on silabs chips... I wonder if FVT switched it around and it is flashed as the first page.
```

---
## \#11 Posted by: manuel.covas Posted at: 2018-01-23T17:53:35.257Z Reads: 102

```
Hi,
This is slightly out of topic but I believe you might be able to give me an answer since you have already been fiddling around with this and probably know more about it then I do.
So my question is since fvt's USB link uses UART to communicate with the esc as stated online, could a standard USB to UART converter from eBay (such as https://rover.ebay.com/rover/0/0/0?mpre=https%3A%2F%2Fwww.ebay.com%2Fulk%2Fitm%2F232634397949) be used to program it instead of the 10$ link? And if so, since the port atleast on the fvt wolf series only has 3 wires, would TX or RX be hooked up to the white wire? How can a two way link ever occour?
```

---
## \#12 Posted by: kaspars Posted at: 2018-03-14T20:10:36.858Z Reads: 82

```
I tried using a similar "generic" adapter and it didn't work. I think it's because the USB Link software uses software libraries specific to the SiLabs chip:

https://www.flickr.com/photos/kasparsdambis/36788711932/
```

---
## \#13 Posted by: manuel.covas Posted at: 2018-03-20T10:37:24.380Z Reads: 76

```
I see, thank you for the info!
```

---
## \#14 Posted by: PredatorBoards Posted at: 2018-05-04T03:14:49.859Z Reads: 65

```
So what's the progress on this project?

Is it possible to overhaul the firmware and do things like replacing the duty-cycle control mode in favor of @Ackmaniac's watt/current mode? I'm pondering whether or not we can make the FVT or other car ESCs as programmable as say a VESC.
```

---
## \#15 Posted by: kaspars Posted at: 2018-05-04T05:20:54.653Z Reads: 62

```
I haven't done any additional work on this after the initial research. It should be possible to just write a custom firmware or configure BLHeli to match the specific layout and pins of the FVT ESC.
```

---
## \#16 Posted by: PredatorBoards Posted at: 2018-05-05T04:31:38.582Z Reads: 49

```
Well the specific ESC I would like to reflash is the Mamba XLX. It's programmability, as is, is already pretty sophisticated versus the other cars ESCs on the market. Would you be interested in pushing that boundary? If not, would you know who is?
```

---
