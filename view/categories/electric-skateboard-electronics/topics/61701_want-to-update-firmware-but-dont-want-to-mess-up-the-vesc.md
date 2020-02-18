# Want to update firmware but don&rsquo;t want to mess up the VESC

### Replies: 8 Views: 425

## \#1 Posted by: Lunasi Posted at: 2018-07-12T22:28:14.618Z Reads: 71

```
![vesc|690x440](upload://cuyXZF56VUV38gMZbWUIxA4hsCd.jpg)

Trying to update my firmware so I can use VESC tool instead of BLDC tool for this older vesc. The older VESC supports firmware for 2.18 but my VESC tool requires 3.37 or 3.38. I see the options to update firmware but its given me a couple warnings when doing so. Can someone tell me what I need to do here before I mess something up?
```

---
## \#2 Posted by: Winfly Posted at: 2018-07-12T22:30:02.940Z Reads: 66

```
Trust it and don't interrupt it. Do not unplug the power.
```

---
## \#3 Posted by: PredatorBoards Posted at: 2018-07-12T22:30:17.114Z Reads: 67

```
I’d suggest getting an STlink
```

---
## \#4 Posted by: Winfly Posted at: 2018-07-12T22:31:00.836Z Reads: 66

```
If you messed up then you need a STlink to reflash firmware.
```

---
## \#5 Posted by: RedEagle Posted at: 2018-07-12T22:45:01.736Z Reads: 60

```
Any luck updating the firmware?
```

---
## \#6 Posted by: briman05 Posted at: 2018-07-12T23:31:13.871Z Reads: 56

```
You most likely have a 4.12 hw so you will want to flash the 410,411,412 vesc-default. Where did you get your vesc
```

---
## \#7 Posted by: abenny Posted at: 2018-07-12T23:46:38.726Z Reads: 59

```
https://youtu.be/v1glLDO-EjA
```

---
## \#8 Posted by: skatardude10 Posted at: 2018-07-13T00:19:14.326Z Reads: 56

```
You are in the bootloader tab. Have you tried just the included files tab and selecting 410 411 412, and does that give you the same message? 

If you haven't flashed a bootloader, your vesc from TB should have came with one preinstalled and you should just be able to select the firmware in the other tab instead of your bootloader in the bootloader tab and update FW that way.
```

---
