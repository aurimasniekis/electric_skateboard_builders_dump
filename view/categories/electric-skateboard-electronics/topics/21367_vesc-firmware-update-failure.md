# Vesc Firmware update failure

### Replies: 9 Views: 2543

## \#1 Posted by: Mox Posted at: 2017-04-19T14:03:20.527Z Reads: 190

```
I have a Vesc with the hardware number 4.12.
I'm using this version of BLDC tools
https://www.electric-skateboard.builders/t/extended-bldc-tool-with-watt-control-mode-ppm-cruise-control-individual-throttle-curve-and-android-app/12286
I try to upload the Firmware File "VESC_Ackmaniac_Mod_2_54.bin" just like the guide suggests But when I do my Vescs disconnects and wont reconnet unless I unplug and then reconnect the powersource. I cant seem to get it to work.
Usually I stick to lurking but this left me clueless and searching the forum doesnt bring anything useful up either.

[IMG]http://i.imgur.com/M5Zr9Ch.png[/IMG]
```

---
## \#2 Posted by: JohnnyMeduse Posted at: 2017-04-19T14:08:43.161Z Reads: 178

```
Where did you buy your vesc.... it look like you don'y have the bootloader inside.
```

---
## \#3 Posted by: Mox Posted at: 2017-04-19T14:35:21.976Z Reads: 165

```
e-greenmotion, 
Holy crap thats compicated.
Time to learn linux I guess...
```

---
## \#4 Posted by: rwxr Posted at: 2017-04-19T14:40:49.918Z Reads: 162

```
E-greenmotion is rebranded Maytech VESCs and Maytech VESCs doesn't have a bootloader for some stupid reason.
```

---
## \#5 Posted by: Maxid Posted at: 2017-04-19T14:44:09.465Z Reads: 161

```
[quote="rwxr, post:4, topic:21367, full:true"]
Maytech VESCs doesn't have a bootloader for some stupid reason.
[/quote]

Actually I like that they don't - makes choosing a reputable seller easier and shows who skimped on the VESC ;)
```

---
## \#6 Posted by: flatsp0t Posted at: 2017-04-19T15:52:58.311Z Reads: 153

```
Well, but you only learn it after someone fell into the Trap.
```

---
## \#7 Posted by: Tampaesk8er Posted at: 2017-04-21T09:28:40.155Z Reads: 137

```
This happened to me, i tried different usb cables, the vesc likes different usb cables for some reason. Next, if you look at your pic, on the top right corner you'll see a tab that says (COM3). try changing it to (COM5). Thats what i did with both my vesc on 2 eboards and is working good now. Try this first before downloading bootloader.
```

---
## \#8 Posted by: TarzanHBK Posted at: 2017-04-21T10:08:56.316Z Reads: 133

```
like @rwxr said, they sell them without bootloader.
So get an Stlink V2 and follow the upload procedure.
Some impressions here:

https://www.electric-skateboard.builders/t/vesc-installing-a-bootloader/752
```

---
## \#9 Posted by: treenutter Posted at: 2017-04-21T15:39:12.185Z Reads: 121

```
Thanks for linking this @TarzanHBK - @Mox it's a lot easier to install a bootloader w a "normal" programmer. I ended up with a weird one and needed help deciphering the abbreviations on the pins, which @chaka was kind enough to help me with.
```

---
