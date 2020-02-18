# VESC BLDC problem

### Replies: 12 Views: 769

## \#1 Posted by: kingbing Posted at: 2016-08-11T19:54:01.422Z Reads: 96

```
Hi guys, 
Just received my VESC from enertion and followed the instruction from http://vesc.net.au/ to configure the vesc. But once i updated the firmware to 4.12 (vresion of the esc) I get this problem:<img src="/uploads/db1493/original/2X/f/f8c1c143b41e936409b9cf5d63593386ba2b9f34.png" width="690" height="410">

I would really appreciated if someone could guide me through this. 
Also i have to mention that as soon as I received the Vesc and plugged it to my sk3 6374 149kv, the motor would turn but as soon as I put some slight resistance to the motor (holding it ) it would stop turning. Really hope the Vesc isnt damaged. 
Thank you in advance for helping me.
```

---
## \#2 Posted by: Skitzor Posted at: 2016-08-11T20:13:54.729Z Reads: 86

```
You should download the according windows tool to the firmware.
And did you do the motordetection before testing, what battery and remote you use is also good info

Edit: Firmwares: https://github.com/vedderb/bldc (although I would flash it to 2.18)
```

---
## \#3 Posted by: kingbing Posted at: 2016-08-11T20:21:34.017Z Reads: 85

```
The bldc tool i have says it supports firmware 2.17 and 2.18. I did not do the motor detection before testing. And i am using a HK-GT2B from hobbyking as well as a 4 cell lipo. And can i flash the vesc with BLDC (using the usb connection) ?
```

---
## \#4 Posted by: Skitzor Posted at: 2016-08-11T20:24:01.641Z Reads: 80

```
Yeah, you should just downgrade the windows tool to the firmware ur using which is 4.12 at this moment. Also 4s is maybe a little low for such a powerful motor
```

---
## \#5 Posted by: kingbing Posted at: 2016-08-11T20:28:17.596Z Reads: 76

```
How do i downgrade to v4.12? Any download links? Thanks
```

---
## \#6 Posted by: sl33py Posted at: 2016-08-11T20:29:07.477Z Reads: 78

```
4s is plenty to configure your VESC to start.  I frequently use 3s (old/tired traxxas lipo - like 1300mAh) to do first connection and configure.  Or lab power supply at 12v.  Something Vedder used to suggest (and may still - haven't checked).

Once motor detection is done and it's configured - i use my 8s or 10s just fine.
```

---
## \#7 Posted by: kingbing Posted at: 2016-08-11T20:31:58.365Z Reads: 73

```
Yes thats what i thought as well.
```

---
## \#8 Posted by: Skitzor Posted at: 2016-08-11T20:34:32.010Z Reads: 69

```
but you said you were running the motor
> the motor would turn but as soon as I put some slight resistance to the motor (holding it ) it would stop turning.
```

---
## \#9 Posted by: kingbing Posted at: 2016-08-11T20:37:21.215Z Reads: 64

```
I use to have an older VESC and i could ride it with a 4cell battery with all my weight on the board. The motor  should not stop so easily with just a slight pressure on it.
```

---
## \#10 Posted by: Skitzor Posted at: 2016-08-11T20:46:45.039Z Reads: 61

```
http://vesc.net.au/BLDC-TOOL/Windows/OLD%20Versions/
```

---
## \#11 Posted by: kingbing Posted at: 2016-08-11T20:48:21.420Z Reads: 59

```
Ok just downloaded the older version of bldc tool (firmware 2.15) And i can get a detection. Everything works fine but when i press the trigger the motor spins from 0 to full power. How do I  change that so its gradual?
```

---
## \#12 Posted by: makevoid Posted at: 2016-08-11T20:53:08.414Z Reads: 57

```
usually that's correct if you already did the controller configuration, you just need to apply some load to it (mount everything and ride your board for example) - make sure that  you don't have wrong values before testing (current limits too hugh, max current ramp step still low), accelerate and apply load gradually
```

---
