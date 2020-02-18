# Going back to FW 2.18 after using VESC tool

### Replies: 3 Views: 374

## \#1 Posted by: nordlicht Posted at: 2018-06-15T11:51:27.860Z Reads: 91

```
Hi,

I'm reading live data with an arduino for a project at the uni and am displaying this on a LCD screen and an app. I tryed the VESC tool, updated the FW and had to find out that the library from rolling gecko on github apparently doesnt support newer FW (PLEASE CORRECT ME IF IM WRONG HERE!).

So I'm trying to get back to FW 2.18 where it works. I flashed in the VESC tool FW 2.15 to use the BLDC tool again. (I couldnt find the 2.18 in VESC).
Than I went to the BLDC tool to flash the proper FW, but after flashing VESC_default.bin and reconnecting the device in BLDC tool I **still** get the message that the VESC has a too old FW. Tells me the version on connected VESC is 2.15 (the FW I flashed from VESC tool).

Any clues how to proceed? If I had the correct file I could just flash it from the VESC tool, but I have no clue which one it is.

I'm using HW 4.12.

Cheers,
Nordlicht
```

---
## \#2 Posted by: nordlicht Posted at: 2018-06-15T12:56:40.469Z Reads: 67

```
Ok. I had old firmwares installed somehow. I made it to flash to 2.18 with this link:
http://www.hellray.de/tutorials-bedinungsanleitung-d-e-f/download-files/
```

---
## \#3 Posted by: armend Posted at: 2019-03-12T15:48:02.458Z Reads: 25

```
Hi nordlicht,

can you show me how you achieved to flash your VESC to the Firmware 2.18?

I want to build a selfdriving vehicle. For that i need a VESC 4.12 with the Firmware 2.18.
But i can only find a VESC 4.12 with a newer Firmware.
So, maybe i can buy the VESC 4.12 with the newest Firmware and then flash it back to the Firmware 2.18.

According to your post you managed to flash the Firmware 2.18.
How did you do that? -> please consider that i am a beginner :slight_smile: 

Best Regards
Armend
```

---
