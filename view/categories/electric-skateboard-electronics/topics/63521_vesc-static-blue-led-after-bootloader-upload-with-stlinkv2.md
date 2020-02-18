# VESC - static blue LED after bootloader upload with STLINKV2

### Replies: 4 Views: 203

## \#1 Posted by: Strassa Posted at: 2018-08-01T19:16:12.775Z Reads: 56

```
Hey community,

I actually am really frustrated now, short overview of what happened:

-  got VESC (4.12 from HK) after an Car-ESC
-  set it up on a friends PC using BLDC-Tool
-  wanted to edit settings - downloaded VESC-Tool
-  did a firmware upgrade cause it said so (for 4.12 HW) 
-  NO USB connection between PC and VESC possible anymore  (static blue LED)
-  flashed bootloader with STLINKV2 
-  VESC still cannot connect to PC (even installed STM32 drivers for windows again, allthough they worked 
    previously)

I am really down right now, don't have the money to get another VESC. Can someone help?

Best regards, Thomas

EDIT: USB-Cable is tested
```

---
## \#2 Posted by: killaton Posted at: 2018-09-26T02:42:12.782Z Reads: 33

```
I have the same issue.
VESC stopped connecting. Blue led only. Flashed new bootloader with stlinkv2, no change in behavior.
Any updates?
```

---
## \#3 Posted by: danielz Posted at: 2018-09-26T04:06:00.443Z Reads: 30

```
Try flashing the whole firmware with stlink, not just the bootloader. Boot loader only wouldnt work for me either.
```

---
## \#4 Posted by: killaton Posted at: 2018-10-02T16:12:14.891Z Reads: 27

```
Thanks. I figured that out eventually. Had to try several versions before it worked.
```

---
