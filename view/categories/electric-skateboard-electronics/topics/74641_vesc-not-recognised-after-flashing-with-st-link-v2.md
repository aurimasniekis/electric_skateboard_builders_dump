# VESC not recognised after flashing with ST-Link V2

### Replies: 9 Views: 505

## \#1 Posted by: HappyFridge Posted at: 2018-11-13T23:11:14.924Z Reads: 93

```
Hi,
I have just finished soldering on the MCU on the VESC 6.0 board. The next steps I followed for flashing were described well by @JdogAwesome here: https://www.electric-skateboard.builders/t/vesc-boot-loader-installation-tutorial/32103
It started to be a bit different when I was going through step 5: uploading hex file through ST-LINK. I couldn't find any hex file for the VESC 6.0. I did however find "60_o_75_300.bin" on GitHub somewhere. Flashed that one to the chip instead, and ST-link utility reported that all went fine and Full flash memory checksum was good.

But then, I unplugged the ST-LINK -V2 (SWD) from computer and VESC. Supplied 15V to VESC and hooked up USB cable. My computer (windows 10) didn't show any sign of some USB device being connected. No bleep, nothing to see in the devicemanager, it just says COM1, but searching online there should be a text like "STMicroelectronics ST-LINK...(COM x). 

I thought the cable was bad (although I have used it for uploading E-books to my ereader recently, but still grabbed another one. That one I used on my old Nokia phone which I used for data transfer. Unfortunately still no sign of life. 
Re-flashed it again; no sign of life.
Installed ST-LINK009 drivers on my desktop; no sign of life.
Rebooted my desktop 2 times; no sign of life
:pensive:

Is my MCU dead? Why is the checksum oke then when flashing? Can't I use the bin-file? What then? All other threads are about HW 4.xx. Searching for an easy answer at the STM website and discussion groups is like finding a needle in a haystack. Different boards and boatloaders.

Any thoughts are appreciated! I am just not that well into flashing and bootloading software part.
![flash_problem1|690x387](upload://pAQ0zgnrXgh20eLC8DLxZyRe7om.jpeg)


EDIT: Solved; it was the ADP2108 choice. Somehow that one doesn't work, but the LM3671 did. It is weird though, they seem the same. Also with LTSpice I came at the same design as for the LM3671 (minor differences). Perhaps the batch of the ADP2108 chips is corrupted.
```

---
## \#2 Posted by: Sn4pz Posted at: 2018-11-13T23:24:46.536Z Reads: 77

```
if you bought that from frank you can PM him or just @ frank (no space) and you can get in touch with him

otherwise youre probably looking for the guidance of a vesc wizard... @JohnnyMeduse maybe you know whats happening? :)
```

---
## \#3 Posted by: JdogAwesome Posted at: 2018-11-14T04:23:56.095Z Reads: 66

```
Could you post some pics of the 6.0 board your trying to flash, maybe also some closeups of the MCU itself. The fact that its flashing but not reading makes me think it could be bad solder joints on the MCU. Also how did you go about soldering the MCU? Stencil and reflow oven, hand pasted and placed and then hot air gun, etc? Also I would try finding the exact right bootloader instead of just some .bin that has 6.0 in the name lol.
```

---
## \#4 Posted by: Santino Posted at: 2018-11-14T05:50:45.996Z Reads: 64

```
I did it, Frank sent me a guide a few months ago, it was really simple. Hope it's helps the way he helped me...

his is a how to for flashing a VESC:

A short Guide summary for all Windows User with the same problem:

You Need: STlink V2. 

Remove the plastic connectors from 3 cable ends and put shrink tube/tape over the exposed metal connector. Now you can plug the cables directly to the SWD port (IO, GND and CLK)

Cables should not be longer than roughly 8cm

1. Download STlink Utility (http://www.st.com/en/embedded-software/stsw-link004.html)
2. Download the last FW from Benjamin for HW6.0 &gt;&gt; https://github.com/vedderb/vesc_tool/blob/master/res/firmwares/60/VESC_default.bin
3. Install STlink Utility (it is inlc. drivers for the STlink)
4. Connenct the STlink to the Vesc with only 3 Pins SWDIO --&gt; IO, GND --&gt; GND, SWCLK --&gt; CLK  **(NEVER connect the 3.3v pin, RTS no need)**
5. Power on the Vesc
6. Open STlink Utility
7. Open the tap TARGET and klick Connect --&gt; the program show you the infos of your VESC
8. Open the Tap FILE and klick open --&gt; search for the file "982347289347209837_VESC_default.bin" and select
9. Use the write button (The second on the right)
10. Press Start at the open window --&gt; the programm will flash your Vesc
11.After finisch close the Programm, power off your Vesc and disconnect the STlink
12. Connect the Vesc via USB and open the Vesc Tool to upgrade the FW
```

---
## \#5 Posted by: HappyFridge Posted at: 2018-11-14T20:04:00.364Z Reads: 52

```
@JdogAwesome  Here are some pics
![S20181114_0002|640x480](upload://vEJ0lll10V6DfIIN2SBUNQYfkcv.jpeg) ![S20181114_0003|531x500](upload://zrEuSY3twga9PdgphIw3mVZZddj.jpeg) 
It is not a professional soldering job, sorry. I used a stencil and hot air. The solder mask in the stencil however is too large and therefore left too much solderpaste on the small pads,  I had several solderjoints all around. Removed that with wick and iron.

I also measured the resistance between USB connector pins and D-/D+ on the chip; 22.6Ohm as per design. So USB traces appear to be good.

@Santino : I was triggered by your follow-through list point 4 where you mentioned that 3.3V pin should not be connected. I had done that though when flashing with ST-Link. :frowning:
I remember a post by Frank [somewhere](https://vesc-project.com/node/45) where he said that, but I don't really understand why. Instead of the LM3671 in the standard design, I use ADP2108-3.3V step down converter. That document says (as does the LM3671 doc by the way) that the FB, SW pins could handle more than Vin + 0.2V?
![CaptureADP2108|369x361](upload://6q6WTdfcLSzngwshEpNiNuBwb7k.jpeg) 

Not sure how to define Vin though in this situation...

So I measured the Vcc voltage when VESC on power: whooping 5.1V! :astonished:. It wasn't converting voltage at all.
I think my step down converter is fried? There is no short between my 5V rail and 3.3V rail. Will order a new one to solder on.

I found a small difference in the size of L1 between ADP2108 and LM3671:
![L1diff|690x180](upload://uyH48cRtRtJi6Wr6YK3888VShOp.jpeg) 
I have a 2.2uH inductor instead of the 1uH. Does that matter that much? I don't have an oscilloscope unfortunately.
```

---
## \#6 Posted by: Santino Posted at: 2018-11-14T20:54:52.402Z Reads: 46

```
I am not an expert, I purchased a MTB from Trampa, needed to flash again both vesc 6. I just followed Frank instructions and everything went easy... If I where on your situation, I will probably do al the job meticulously, since Vesc is made to save you (controlling the board for your safe), so yes try to flash again with the 3.3V pin out, use the 1uH, play it safe, check what you have done and when you make it run, take it slowly until you have confidence. Use a lot of silicone to protect de connections from the vibration. I hot glued my receiver. And ask to the right people within the forum, I am sure they will help you!   Just PM them!!
```

---
## \#7 Posted by: RedEagle Posted at: 2018-11-14T22:36:44.552Z Reads: 45

```
I flashed tons of vescs, though they were 4.12. Haven't flashed a 6.0 but you can ask me anything. I'll be glad to help.
```

---
## \#8 Posted by: HappyFridge Posted at: 2018-11-29T21:54:34.075Z Reads: 36

```
Hi, an update:
I soldered a new DC converter (ADP2108-3.3) and 1uH inductor. Didn't do anything except now I have 0V on my Vcc rail instead of 5V. Safer, but no good.
Looking for a short due to me having put on 3.3V from the ST-Link, I even desoldered the MCU and other main chips (CAN, NRF, power managements). Still no sign of life.

The DRV8301 is giving off 5V, so that looks to be working fine. But why can't the Vcc be at 3.3V? I checked an unpopulated board; seems to be fine, no shorts, no crazy resistances. So board design seems oke.
While getting more frustrated, I made another board by populating the one I still had. Made sure not to make any mistakes. Soldering looks even better now. But still: 0V on Vcc rail. 

I checked the DRV8301 file and it says that it has internal power pin 23 (DVDD)(3.3V) and 27 (AVDD)(6V). They are bypassed to GND by caps 17 and 20 respectively. If I measure the voltage across these caps, I get 0V. Is there someone with a working  VESC that can check if this is normal?

Any help is appreciated.
Thanks
```

---
## \#9 Posted by: HappyFridge Posted at: 2018-12-10T12:52:44.994Z Reads: 28

```
Solved; it was the ADP2108 choice. Somehow that one didn't work, but the LM3671 did. It is weird though, they seem the same. Also with LTSpice I came at the same design as for the LM3671 (minor differences). I tried 3 times with 3 different ADP2108 chips. Perhaps the batch of the ADP2108 chips is corrupted, or I am misreading the documentation.

Further improvements were the bootloader, the one given by Santino works, the one I had before didn't really.
And I accidently reversed USB D- and D+ in the schematics! :persevere:. Had to make a small jumper.

Finally! Back on track
```

---
