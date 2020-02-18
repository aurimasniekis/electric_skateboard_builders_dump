# VESC. How can I download VESC older firmware 2.16 and where can I download it from?

### Replies: 5 Views: 2082

## \#1 Posted by: Tampaesk8er Posted at: 2017-02-04T14:10:50.035Z Reads: 143

```
My vesc is 4.12 hardware version, tried to install 4.12 firmware but it says " firmware on conected vesc is 2.16". Is there a way I can download older vesc firmware 2.16?

What is FOC? 

Thank you in advance for the help. This is my first build and first time messing around with eboard stuff.
```

---
## \#2 Posted by: rpn314 Posted at: 2017-02-05T00:33:22.142Z Reads: 125

```
Welcome!
It sounds like you already have firmware v2.16, so no need to download and install it again. I suspect you're a little lost on all of the version numbers (and it can be a little confusing), so I'l give you a quick run down (I apologize in advance if this is old news for you). To start with, the firmware version numbers do not match the hardware version numbers. There's some correlation, as in some firmwares only work on some hardwares and vice-versa. The other wrench that's thrown into this is BLDC Tool (the computer application that you use to connect to your VESC to change its parameters). It has some limitations on the firmware versions it supports. The current release of BLDC tool only supports firmware v2.17 and v2.18 to my knowledge.

Now with all that, by "4.12 firmware" do you mean firmware v2.18 (the current release)?

FOC is Field Oriented Control. It's a different way for the VESC to control the motor. It's usually a bit quieter than BLDC mode. See here: http://www.electric-skateboard.builders/t/vesc-faq-what-is-foc-field-oriented-control/419

If you haven't already, I'd recommend reading this: http://www.electric-skateboard.builders/t/new-vesc-user-read-this-complete-walktrough-of-the-vesc/2980
```

---
## \#3 Posted by: Tampaesk8er Posted at: 2017-02-05T01:11:13.761Z Reads: 109

```
The circuit board says vedder 4.12. But when I click on connect in bldc tool, it says my firmware is too old on vesc. when I try to update firmware from bldc folders (4.10, 4.11, 4.12) it keeps giving me a buffer reader timedout error and doesnt let me connect to the vesc. check out pics. Im going crazy, i even went on google and found old version of firmware including 2.16. I tried uploading the 2.16 firmware so that i can then uldate to the current 2.18 but i still get buffer read timeout error code. yes i did read the link you sent me already. SMH. Thank you.<img src="/uploads/db1493/original/3X/4/9/49dd9a4acfff42eb74fa817af42d2a97da91c775.jpeg" width="499" height="499"><img src="/uploads/db1493/original/3X/3/c/3c34c2f778b4b772522e2788b320782ddc784237.jpeg" width="669" height="499"><img src="/uploads/db1493/original/3X/b/8/b85d2a070aa906613fd83172a9f663eb572ea077.jpeg" width="499" height="499"><img src="/uploads/db1493/original/3X/8/2/82c1cab9d406c3f038ecee774e5294d4bc1356e1.jpeg" width="669" height="499"><img src="/uploads/db1493/original/3X/7/1/71fbeebf2ba544e83b68a39de8a2cc832bb3d401.jpeg" width="669" height="500">
```

---
## \#4 Posted by: Tampaesk8er Posted at: 2017-02-05T01:18:32.589Z Reads: 90

```
<img src="/uploads/db1493/original/3X/8/4/84d20b09fb159fe7b160b4e49875f65d7438618c.jpeg" width="373" height="500">
```

---
## \#5 Posted by: rpn314 Posted at: 2017-02-05T01:30:54.462Z Reads: 86

```
Thanks for having read that. Many don't :slight_smile:
You already have v2.16 and if I'm understanding that correctly, I think the download you have (where it's pointing to on your desktop) is still v2.16. The process you're doing should update it without any problems to v2.18, as long as the file you're pointing to is v2.18.
```

---
