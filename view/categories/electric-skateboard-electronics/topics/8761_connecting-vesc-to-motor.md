# Connecting VESC to motor

### Replies: 7 Views: 4179

## \#1 Posted by: robskie Posted at: 2016-09-01T11:15:10.631Z Reads: 346

```
Hi there, I just received my last part (a tiny little servo cable), so I'm setting up my VESC atm.
now, i was about to start connecting my motor to the VESC when I realised I don't know which cables go where, i've done quite a bit of reading on everything I needed to know in order to complete the build but never saw anything about connecting the motor to the VESC
http://alienpowersystem.com/shop/brushless-motors/alien-5065-outrunner-brushless-motor-270kv-2200wa/
This is the motor I have, some help would be appreciated, I'm really excited to get it running for the first time!
```

---
## \#2 Posted by: crameur Posted at: 2016-09-01T11:27:03.595Z Reads: 341

```
Well just plug them in until it works, you won't burn anything trying out
```

---
## \#3 Posted by: makevoid Posted at: 2016-09-01T15:48:09.113Z Reads: 315

```
If it's sensorless then yes, connect the three motor cables, be sure you are powering the vesc correctly and then try or check this guide or watch other yt videos first of other motor detection / battery settings and limits configurations / motor limits parameters configuration.

On the forum you can start here with these two topics:

http://www.electric-skateboard.builders/t/vesc-faq-motor-detection-step-by-step-guide/500

http://www.electric-skateboard.builders/t/new-vesc-user-read-this-complete-walktrough-of-the-vesc/2980

If the motor is spinning in the other direction invert two motor cables.
```

---
## \#4 Posted by: CHANCE5 Posted at: 2016-09-02T07:24:10.234Z Reads: 264

```
<img src="/uploads/db1493/original/2X/3/39d9fa58422a29438b9719d054dfeedf6481a424.JPG" width="666" height="500">



Hey guys just recently made my e-board. it was working yesterday, but the next day after I charged it (I did not over charge it), it wont connect to the controller or the motor won't work. any suggestions? here's my setup. Please help.
```

---
## \#5 Posted by: racidon Posted at: 2016-09-02T07:43:01.635Z Reads: 263

```
does the VESC light up? and does the Receiver light up?

-YES - what lights on the VESC light up?

--BLUE - When you use the remote does it flash red?

---YES - Likely DRV is fried (small chip that controls power to motor)

---NO - Plug into a computer and use the BLDC tool and do a motor detection

-NO - You must not have power running to the VESC, what does your battery readout say? Is your fuse in tact? What voltage is being output at your XT60 plug?
```

---
## \#6 Posted by: JohnnyMeduse Posted at: 2016-09-02T13:29:20.656Z Reads: 249

```
Did you follow the step by step for the configuration of VESC (because they are not plug and play), it might just be some configuration issue.

http://www.electric-skateboard.builders/t/vesc-faq-easy-to-follow-vesc-getting-started-playlist/5560

http://www.electric-skateboard.builders/t/vesc-faq-easy-vesc-configuration-in-windows-mac-for-noob/2963/1

Or try to search Using VESC FAQ

And if you don't find what you need from known people on this forum  Email @EnertionSupport, using the tool on there web site

Also you might want to check this 

http://www.electric-skateboard.builders/t/vesc-faq-negative-squared-cross-mark-warning-negative-squared-cross-mark-risk-of-short/6805
```

---
## \#7 Posted by: AutoNoe Posted at: 2018-12-08T15:32:59.864Z Reads: 33

```
A little late to the party but perhaps it will help any other unfortunate souls who follow the same thing I did... You're receiver is connected the wrong way around. I googled 'esc connections' to quickly check which way I should plug it and following your image did not work. The negative (black) terminal is to the outside of the VSC. Can be checked quickly for continuity with the negative terminal of the battery connection. (My multimeter's batter my flat when I googled your image :P)
```

---
