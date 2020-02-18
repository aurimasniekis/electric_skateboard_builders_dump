# \[SOLVED\] Vesc Enertion &#124; Blue LED on constant, no other lights

### Replies: 9 Views: 2344

## \#1 Posted by: nzeboarder Posted at: 2016-10-14T07:57:01.057Z Reads: 190

```
I received my two vesc's and one of them will not connect via usb to my laptop. Connection process:

* connect 12v 1.5amp power supply
* connect usb to laptop
* motor is connected

<img src="/uploads/db1493/original/3X/a/f/af1c35aff72792294ebbed05c60ea72724b8a311.JPG" width="690" height="388">

<video width="320" height="240" controls>
<source src="https://drive.google.com/file/d/0B2G8asF3BQNFUjJjOFN1RUZYNG8/view?usp=drivesdk" type="video/mp4">
</video>

I've checked all cables and connections and given my other vesc is working fine I suspect it's a vesc issue. Searching on the forum points the cause to missing firmware although given they test all units before shipping I don't know how this would occur. 

How likely is missing bootloader/firmware? 

I have raised with @EnertionSupport who pointed me to this forum.
```

---
## \#2 Posted by: rpn314 Posted at: 2016-10-14T13:49:47.052Z Reads: 174

```
Blue light means it's got power. If it won't connect to your laptop, then it's very possible it's missing the bootloader or even firmware.

Just to double check, you got 2 VESCs from enertion, they both get blue lights when you plug them into your 12v power supply, and when they are plugged into your laptop one connects to BLDC tool just fine and the other doesn't....does it show up in the list of devices? It should say something more to the effect of "blah blah VESC blah blah", instead of "cu.Bluetooth-Incoming-Port" like mine says right now, since I don't have my vesc plugged in at the moment.
<img src="/uploads/db1493/original/3X/6/9/690fe4928383462431b87f72375693cb81d37cbf.png" width="524" height="218">

If all of that is the case, I don't know why @EnertionSupport directed you here. I don't think many of us can assist unless you're interested in seeing if re-flashing the bootloader fixes it (that would require an ST-Linkv2 dongle of some sort)
```

---
## \#3 Posted by: rodriguejoe1 Posted at: 2016-10-14T23:41:35.553Z Reads: 158

```
http://www.electric-skateboard.builders/t/upgrading-the-vesc-firmware/2780
```

---
## \#4 Posted by: rodriguejoe1 Posted at: 2016-10-14T23:44:06.928Z Reads: 158

```
http://www.electric-skateboard.builders/t/vesc-faq-in-depth-video-how-to-program-your-vesc/2088

see if these help any.
```

---
## \#5 Posted by: nzeboarder Posted at: 2016-10-19T07:39:39.907Z Reads: 138

```
Just wanted to check in and confirm that I managed to revive my VESC. It turned out to be missing firmware, so if your VESC only shows the blue LED when powered up and is not detected via USB connection that's probably the cause.

Resolution:
* I downloaded the lastest firmware from [vesc.net.au](http://vesc.net.au/flash/)
* Using a Raspberry Pi and instructions (modified) from [here](https://learn.adafruit.com/programming-microcontrollers-using-openocd-on-raspberry-pi/wiring-and-test?view=all) managed to flash the firmware into the VESC ST chip without a usb programmer
* Plugged VESC back into laptop and configured as per normal using BLDC Tool

Enertion did offer to replace it but this was quick and free :sunglasses:
```

---
## \#6 Posted by: WeeChumlee Posted at: 2016-10-19T08:45:52.060Z Reads: 125

```
My opinion:
Pretty slack of Enertion "support" to send you to a public forum to get help. What sort of "support" is that?
Hmm, Enertion says all VESCs are programmed and tested with motors before shipment. Pretty difficult to do that with no firmware loaded.
Glad you got it sorted though.
```

---
## \#7 Posted by: Devo Posted at: 2016-10-22T07:57:07.479Z Reads: 109

```
I'm in the same situation with the one I received earlier this week. Constant solid blue light and it won't detect via usb. I've sent an email to @EnertionSupport today to inquire as to what I'm supposed to do. I've built my whole esk8 from scratch and this is my final part which is a little disappointing. There's no way I'd manage to hardware install the bootloader/firmware. I don't have the tools, resorces or knowledge.
```

---
## \#8 Posted by: rpn314 Posted at: 2016-10-22T15:11:26.318Z Reads: 99

```
@nzeboarder Well done! I didn't even know the raspberry pi had that capability. Thanks for the link, I'm very curious now.

@Devo If you were close, I'd offer to do it for you (heck if you're traveling through Utah, feel free to PM me. I could definitely meet you at the airport or something). That's probably your best bet: find someone on here who's somewhat local and knows how. Seems @EnertionSupport has been slacking. Sorry.
```

---
## \#9 Posted by: Devo Posted at: 2016-10-22T21:06:01.823Z Reads: 89

```
@rpn314. Sorry mate but I live in land of oz other wise I'd defiantly take you up on your offer. I only sent the enquiry off to @EnertionSupport yesterday and it being the weekend I didn't expect a response right away. I'll see what happens in a few days other wise I might have to resort to something else to get it working.
```

---
