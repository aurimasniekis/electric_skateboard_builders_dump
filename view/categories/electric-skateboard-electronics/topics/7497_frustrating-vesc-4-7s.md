# Frustrating VESC 4.7&rsquo;s

### Replies: 7 Views: 936

## \#1 Posted by: Jojosensor Posted at: 2016-08-11T15:33:00.732Z Reads: 169

```
So I finally decided to set up my extra board. I have two early VESC's. They're 4.7's that I obtained from enertion boards quite some time ago. As others have said and seen the 4.7's were particularly frustrating for several reasons. First, both of the VESC's I bought from Jason were of the "deconstructed" type. This basically meant they came with their caps and nothing else. The soldering was up to the user to figure out and accomplish. Considering the VESC's cost $100 each I thought this was a bit "unfair". However, I've read all of Jason's threads on the subject and do understand completely where he is coming from. He's a great person and innovator. Instead of simply sitting around and complaining which is what the majority of us do (including myself) he's forged ahead making in roads into this new and exciting field. The dual raptor is a quality item with incredibly solid components. I feel it has some growing to do but the actual "feel" of the product is one of quality. I have the Evolve Carbon GT unit also. Theres no question that the board is a sick board which all others have to be compared to. Jeff has made such an amazing board you just have to admire its beauty. That being said, when I compare the raptor to the GT (whether its true or not) the "feel" of the components feels a bit more substantial on the raptor. The mounts and the R-SPEC motors in particular are amazing. I digress........Back to the VESC's. Anyway, the 4.7's also needed a boot loader. They did not come with one so I needed and STLink. I didn't know anything about this at first so I needed to contact Jacob Bloy who's knowledge and help was great. His website is incredibly detailed and he was able to link with me (9000 miles away!!!) and program my VESC's. I finally had everything set up and got my motors running. I said to myself it's been a while since I updated the firmware for the 4.7's so I had better do this. When I uploaded the latest firmware to my 4.7's they stopped working.........(no I didn't make the mistake of uploading the wrong version and frying the VESC) It turns out that in order for me to use my 4.7's I can only use the older (limited) version of the firmware. I think its version 2.16. The latest version is 2.18, I think. It took me almost an entire night thinking I had fried my VESC's somehow but now they're working with a CAN bus controlling two VESC's. It's definitely a learning curve but I'm beginning to get better......
```

---
## \#2 Posted by: Nordle Posted at: 2016-08-11T18:51:31.507Z Reads: 130

```
Just run them on the old firmware under BLDC thats what they are made for and they do great
```

---
## \#3 Posted by: elkick Posted at: 2016-08-11T21:54:54.049Z Reads: 107

```
I have 6 VESCs v4.7 running FW 2.18 without any issues, 4 of them even with FOC. It's not true that those would require an older Firmware version.
```

---
## \#4 Posted by: sl33py Posted at: 2016-08-11T22:06:48.640Z Reads: 103

```
I have 4 older hw4.7 VESC's with no issues at all.  I haven't updated firmware (it works so why "fix" it!), and think they are running original fw1.13 iirc.

The only issues i had were some voltage errors - both overvoltage and abs - fixed by adjusting values in BLDC tool.  WHen testing afterwards i did manage to fry two DRV's - no fault of the VESC as i was hammering hard start/stops repeatedly (don't do that).  Lesson learned and no issues since.

Not frustrating at all.  They work great.  The cabling is preference - i frequently have removed the cables that they came w/ to put the bullets directly on the phase wire out connector pads, and power in leads when i added my own cap.  

If you follow the steps (step-by-step) from vedder's site w/ Ubuntu - i think you don't need the stlink?  Not sure as mine work fine this way (when i updated to 1.13 fw).

Good luck!
```

---
## \#5 Posted by: sl33py Posted at: 2016-08-11T22:12:26.844Z Reads: 86

```
I also have a bunch of extra CAP PCB's if you want the slimmer 3 cap setup vs the one big cap on the 4.7hw VESC.  Shoot me a PM if you'd like a set.
```

---
## \#6 Posted by: chap Posted at: 2016-10-17T20:56:22.682Z Reads: 52

```
Which old firmware works with VESC 4.7?  I'd love to just get these working without having to install a Bootloader...  a huge thanks if you can be of any help - feel like I'm painting myself into a corner over here and just want to ride
```

---
## \#7 Posted by: rpasichnyk Posted at: 2016-10-18T12:22:47.017Z Reads: 34

```
You can compile any version of the firmware as described here http://vedder.se/2015/01/vesc-open-source-esc/ 
It works best on Ubuntu, if you are running another OS, I would suggest to install Ubuntu in VirtualBox.
```

---
