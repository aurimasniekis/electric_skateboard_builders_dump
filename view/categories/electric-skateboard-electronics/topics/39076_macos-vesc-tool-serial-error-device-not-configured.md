# MacOS VESC Tool &ldquo;Serial error: device not configured&rdquo;

### Replies: 2 Views: 442

## \#1 Posted by: GunnarK Posted at: 2017-11-23T15:18:43.498Z Reads: 64

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
```

---
## \#2 Posted by: GunnarK Posted at: 2018-02-05T23:54:39.645Z Reads: 38

```
Apparently there was no bootloader present
```

---
