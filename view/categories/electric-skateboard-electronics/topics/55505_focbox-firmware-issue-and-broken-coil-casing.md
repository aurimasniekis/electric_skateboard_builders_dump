# FOCBOX Firmware issue and broken coil casing

### Replies: 11 Views: 582

## \#1 Posted by: ggalisky Posted at: 2018-05-15T02:54:42.021Z Reads: 103

```
Hello all,

I just got my replacement FOCBOX and it has some issues. First off when I connect my FOCBOX to the BLDC tool, it reads: "The firmware on the vesc is too old, please update using a programmer.
Also a component is damaged on the focbox. (see pictures) 
![IMG_6842|375x500](upload://fOS1YgLZUqL9N61VwQXTSunA67n.JPG)
Can anyone help me with this
```

---
## \#2 Posted by: b264 Posted at: 2018-05-15T02:58:03.801Z Reads: 95

```
This looks like you should contact enertion if the inductor is physically missing material.  I wouldn't even power it on
```

---
## \#3 Posted by: ggalisky Posted at: 2018-05-15T03:02:05.118Z Reads: 94

```
This is exhausting as I was told I would be receiving a new FOCBOX
```

---
## \#4 Posted by: ggalisky Posted at: 2018-05-16T00:45:35.340Z Reads: 66

```
I have been told "You need to flash the 2.18 firmware using the vesctool as a custom firmware." by enertion customer support. They provided no links on how to do this or any other direction. They also did not address the broken part of the coil. Can anyone help me here with finding links?
```

---
## \#5 Posted by: Deckoz Posted at: 2018-05-16T00:51:09.289Z Reads: 63

```
While the casing for the inductor is broke it should function fine.

For the firmware just use the tool to update the firmware in the firmware tab...
```

---
## \#6 Posted by: ggalisky Posted at: 2018-05-16T00:56:03.131Z Reads: 61

```
I don't think you understand, the BLDC tool won't even let my FOCBOX connect, it says it is too old(attached picture). I have already attempted to update firmware, and I cant even connect to the BLDC tool.
![22 PM|690x372](upload://lKoodXRq9JaI00lkNxJV3R522Ku.png)
```

---
## \#7 Posted by: Deckoz Posted at: 2018-05-16T01:06:26.224Z Reads: 58

```
Oh man. I don't understand the bldc tool at all. 😂😂. It's the worst, can you tell me how to go to the firmware tab without connecting and flash the update? I can't figure it out.

Basically, you need to use vesc tool because your vesc has no bootloader possibly.. but it's a focbox so not likely. Just plug it in and wing it?
```

---
## \#8 Posted by: SeanHacker Posted at: 2018-05-16T01:09:29.079Z Reads: 58

```
@ggalisky Go here https://www.vesc-project.com/node/17. Download the VESC_Tool and flash the firmware in the firmware tab (choose bootloader tab). Then after you flash the correct bootloader you can use the BLDC_Tool or whichever you like better. Looks like they shipped with a really old bootloader and/or firmware?
```

---
## \#9 Posted by: ggalisky Posted at: 2018-05-16T01:15:18.778Z Reads: 58

```
Thank you, I will try this tonight
```

---
## \#10 Posted by: ggalisky Posted at: 2018-05-16T02:46:00.230Z Reads: 54

```
THANK YOU! This worked for me! Check your PM
```

---
## \#11 Posted by: SeanHacker Posted at: 2018-05-16T03:29:02.676Z Reads: 50

```
Anytime dude. It's why this forum exists. ;)
```

---
