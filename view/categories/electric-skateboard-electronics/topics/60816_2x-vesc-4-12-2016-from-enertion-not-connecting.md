# 2x VESC 4.12 (2016) from Enertion not connecting

### Replies: 14 Views: 499

## \#1 Posted by: Kororor Posted at: 2018-07-03T17:16:09.607Z Reads: 103

```
Hi everyone.

I purchased two 4.12 VESC's from Enertion way back 2016. Sadly that summer was pretty much over by the time I got all my parts for my first build. Next summer was very cold and I had other shenanigans, but now it's warm again and I figured I could try to build my board.

I started by checking if I could update my VESC's that had never been powered on before and immediately halted by not getting these things appearing in windows 10 device manager, first I tried with half charged 3S LiPo, and nothing but blue light shines on the ESC's.

Then I did the TeamViewer dance with Enertion support and they claimed it has to be at least 6S battery in order to work, so I did what I could and put two very beefy 4S pack's in series, measured 30V output and connected with anti-spark XT90 connector, but it was exactly the same, just blue light no new devices.

Guy had no clue what to do and suggested I should ask here if anyone has any idea what might be going on.

I suppose it doesn't matter if they are connected to a motor or not in order to poke at them under windows.
Like I said, I have never installed or powered these before this day.

Any bright minds out there?

![IMG_20180703_192858|666x500](upload://8U2IJycwCUBSAtDTdn23q6YFt5z.jpg)
```

---
## \#2 Posted by: Martinsp Posted at: 2018-07-03T18:47:34.977Z Reads: 82

```
Do you by any chance havce an st link?
I assume you/enertion support already checked if you have drivers installed so next step would be to check if the firmware is the problem. Id try to erase the memory and upload a new one.
```

---
## \#3 Posted by: Battosaii Posted at: 2018-07-03T18:53:34.082Z Reads: 76

```
Make sure you use a USB cable that can transfer data there are a lot of charge only cables only out there.
```

---
## \#4 Posted by: Kororor Posted at: 2018-07-03T19:07:39.238Z Reads: 70

```
I continuity checked the usb cable pins all the way from the end to the vesc pcb to be absolutely sure there was no issue with the connector, and I think it should appear in device manager even if there are no drivers.

So I guess the next logical step would be to stlink the shit out of it, too bad I don't own one yet, so I have to order one and wait for ages. Is there any differences what stick I should get?
Funny thing is that they insist they never ship any vesc's w/o bootloader or firmware.

Hopefully I won't fk this up.
```

---
## \#5 Posted by: Martinsp Posted at: 2018-07-03T19:50:28.488Z Reads: 66

```
You may be able to find a stlink-v2 locally. People use them quite often so you may be able to find it locally in some electronics store or maybe second hand...

Just to make sure, when you power it on, nothing happens with the LEDs on the PCB? Except the blue one, that one indicates that the power is on (not that the VESC/MCU is powered on, just that the powerline is present). What is important is if the RED one blinks or if the green one turns on after a few seconds. If not, my educated guess would be firmware is not present at all or not OK in some way, preventing the MCU go through the power on sequence.
```

---
## \#6 Posted by: Kororor Posted at: 2018-07-03T20:19:54.976Z Reads: 58

```
Close look at the led's while powering on, only blue one gets lit. Nothing from the others.
But yeah, thanks, I'll look for some cheap STLinkV2. Sadly we can't have anything fun locally in Finland.
```

---
## \#7 Posted by: Martinsp Posted at: 2018-07-03T23:08:27.538Z Reads: 52

```
BTW you should also get the headers for the programming port while you are at it so that you can connect the stlink to the VESCs. 6 pin 1.2mm pitch
```

---
## \#8 Posted by: Kororor Posted at: 2018-07-04T14:23:34.780Z Reads: 39

```
Good point, luckily I already had them, seem to be the same connector most small stepper motors have.
```

---
## \#9 Posted by: Martinsp Posted at: 2018-07-04T14:33:20.862Z Reads: 38

```
Yeah, alternatively you could just solder the wires of the STlink directly to the VESC. Programming it is just a one time thing so it is not too big of a deal.
You will need firmware and a bootloader I just uploaded it here.
https://drive.google.com/open?id=1E3aSOi57B0740b3ssqJu9Vl-aoNE8pyy
The zip contains fw2.54, fw2.18 and a bootloader.
```

---
## \#10 Posted by: Kororor Posted at: 2018-07-05T00:19:05.158Z Reads: 35

```
Appreciate the effort, Google Chrome just didn't allow me to download them. Didn't personally even think this far yet. But I'll probably try to find files needed from some more reputable sources.

Got me curious though, does there exist more than one bootloader, and what config tool + firmware combo I should go for?
```

---
## \#11 Posted by: Martinsp Posted at: 2018-07-05T05:57:51.526Z Reads: 31

```
I am not sure if the bootloader for a V6 is different but I don't think so. The one in the link is what I flash on customer devices when the bootloader is not present. Same for th firmware it is not a virus I would not do that... Unfortunately I am not able to upload the files directly here on the forum.

The bloc tool is for 2.xx firmwares and vesc tool is for 3.xx 
Other than that you only need to choose the correct hardware once you are flashing from the bloc tool, in your case it is 4.12
```

---
## \#12 Posted by: Kororor Posted at: 2018-07-05T13:32:28.231Z Reads: 27

```
Tried again and it downloaded w/o issues, and the files seem to have same hashes as what I got elsewhere.
First time around Chrome literally didn't allow me to get the file, which was bit worrying.

I assume with Acramaniac mod it's better to use his tool also?
```

---
## \#13 Posted by: Martinsp Posted at: 2018-07-05T13:57:21.654Z Reads: 24

```
That's good to hear, the files there are good t get you started and then update to whatever firmware you like the most via the tool. It was hard to find the bootloader so I wanted to share it so you don't have to search for too long. 

They each have their own tool since the firmwares have different features 
For both ackmaniacs firmwares there are threads
On the forum with download links for the tool. And for the regular firmware you can use enertions tool for the 2.18 and on vesc project there is tool for 3.Xx original (not ackmaniacs firmware).
```

---
## \#14 Posted by: Kororor Posted at: 2018-08-05T14:00:09.830Z Reads: 17

```
Update.

Got my programmer finally. Memory was indeed empty, so I flashed bootloader.
Then had some trouble flashing firmware. Found precompiled .hex by pepperfish with combined bootloader+firmware, used that, then connected with "ACKMANIAC_ESC_TOOL_3_102" and flashed firmware once again with the one that comes in the tool to make proper match.

Have not yet wired these on skateboard, but everything seems fine now. Thank you all.
```

---
