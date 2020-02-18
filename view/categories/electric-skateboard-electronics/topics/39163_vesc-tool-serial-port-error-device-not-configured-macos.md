# VESC Tool &ldquo;Serial port error: Device not configured&rdquo; - MacOS

### Replies: 4 Views: 698

## \#1 Posted by: GunnarK Posted at: 2017-11-24T14:00:24.429Z Reads: 83

```
I am trying to update the firmware from 2.18 to 3.31 with VESC Tool.
I connect my VESC and get the message my firmware is too old, so a limited connection is available which is understandable.

But on flashing the firmware 3.31 from the VESC Tool itself or flashing firmware 3.28 from @rpasichnyk
I get this error

`Serial port error: device not configured`

Here is the debug log
<img src="/uploads/db1493/original/3X/c/a/ca3de1454b4ee581228c1ce5b411b786b1d12ce6.png" width="690" height="160">

After trying to flash the firmware my vesc disconnects and I can't reach it anymore other than by manually restarting the board..

I am using @rpasichnyk's Mac compiled VESC Tool

PS: this is the second time posting this topic, since it seems the first one didn't go 'public' or something

edit: 
PPS: oh wait it did, thought that since this bar was missing
<img src="/uploads/db1493/original/3X/b/3/b300e77da9e0f6dc4d887a0e9af31d582ee80eb5.png" width="690" height="67">
The topic might have gone in dm-mode or something since I tagged rpasichnyk..
```

---
## \#2 Posted by: GunnarK Posted at: 2018-02-05T23:55:13.050Z Reads: 66

```
Apparently there was no bootloader present.
```

---
## \#3 Posted by: TranxFu Posted at: 2018-04-28T00:18:49.656Z Reads: 54

```
hey mate, how'd you solve this ? Did you just upload the boot loader via the vesc tool ?
```

---
## \#4 Posted by: GunnarK Posted at: 2018-04-28T13:29:58.704Z Reads: 47

```
Correct. I used the Vesc tool, not bldc
```

---
