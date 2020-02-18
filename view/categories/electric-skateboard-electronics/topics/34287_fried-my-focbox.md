# Fried my FOCBOX

### Replies: 21 Views: 1273

## \#1 Posted by: Octavio Posted at: 2017-09-29T15:42:41.986Z Reads: 243

```
Hello,
Fried my FOCBOX and I am wondering if it is fixable, and how to prevent this from happening. I was going over very bumpy terrain when it happened. I'm wondering of somehow there was a short created then. I've provided some pics in hope someone can see what I did wrong.  I did go about 20 miles on pavement without any problems. My FOCBOX were contained in a tight space. I wonder if the slight gap in phase wires was the culprit, but idk. I was also going down hill. No acceleration. 

torcboards Motor 6355 190KV
focbox
10s30c8A lipo from zippy
70/15 gear ratio
TorqueBoards 2.4ghz Nano Remote Controller

<img src="/uploads/db1493/original/3X/e/8/e832be63d05e5a2f270bface24a5c54b6a5808dd.JPG" width="375" height="500"> 

<img src="/uploads/db1493/original/3X/9/c/9cac93b5616fd6fa7fbb7346fe510dc57ce4966c.JPG" width="375" height="500">

<img src="/uploads/db1493/original/3X/0/f/0fd3d9fbf726a1579e129cf75aa44f454a74a21b.JPG" width="375" height="500">
```

---
## \#2 Posted by: Acido Posted at: 2017-09-29T16:27:53.372Z Reads: 214

```
You probably went over 60k erpm and fried the drvEDIT: didnt see the pics
```

---
## \#3 Posted by: scepterr Posted at: 2017-09-29T16:28:35.785Z Reads: 215

```
depends if the pcb itself is still good, that looks like the fet exploded(wow)

@acido I dont think its possible with his setup, besides the drv looks physically fine....unlike that missing fet lol

Is the motor that focbox was plugged into still working?
```

---
## \#4 Posted by: SilentException Posted at: 2017-09-29T16:32:25.731Z Reads: 215

```
Damn man, that FET is oblierated!

Could it be the sparking between the phase wires due to exposed metal part? I use bit of heat shrink on the bullet connectors to 1. keep them in place and 2. prevent any contact or sparks...
```

---
## \#5 Posted by: Martinsp Posted at: 2017-09-29T16:42:33.413Z Reads: 210

```
What happened in my opinion there was a short on the phase wires somewhere, maybe your motor wires shorten in the motor or the connectors. Or maybe through the holes where the cables exit the FOCBOX that some metal entered the case and shorted something out. The reason for thinking this is that FETs explode when they are overloaded and yours had so much current going through it that it ripped the case (i think nickel plated copper or whatever) when failing... 

Unfortunately it is unrepairable unless you dont mind it not being elegant anymore.
<img src="/uploads/db1493/original/3X/f/c/fc90d7efa4c9fb89f477f1abab48c83d7c199ae3.JPG" width="375" height="500">
Here on the picture you can see copper that has been just ripped off of the PCB itself. It is fixable but it would require a lot of effort and creativity to join the copper that is remaining and the input of the mosfet, output of the mosfet and also the gate trace that has been destroyed. Usually there are pads underneath the FET that are completely missing on yours. Another thing that would happen is you would no longer be able to use the blue aluminum part of the case because it would not fit anymore due to mention wires. Solution for this would be individual heatsinks for the FETS. If you can get a new one, the repair would be cheaper but still pretty expensive since it is not and ordinary job.
```

---
## \#6 Posted by: Octavio Posted at: 2017-09-29T16:43:03.077Z Reads: 190

```
Yes. The other controller successfully completed a motor detection on it. (The motor)
```

---
## \#7 Posted by: scepterr Posted at: 2017-09-29T16:49:47.261Z Reads: 193

```
It might still be usable, would need it cleaned it off to really see extent of damage
<img src="/uploads/db1493/original/3X/4/6/46726e8312a6bcd97e6dcfcde57411c74df00f0b.jpg" width="281" height="500">
```

---
## \#8 Posted by: Octavio Posted at: 2017-09-29T16:50:37.819Z Reads: 184

```
So. When I buy a new focbox. To prevent this: secure everything and heat shrink those phase wires.
```

---
## \#9 Posted by: Martinsp Posted at: 2017-09-29T16:51:58.417Z Reads: 182

```
yes heatshrink or tape around the connectors and what I suggest is to just cover the 3 holes where the phase wires are. You can use just tape hot glue.. anything is better than nothing.
```

---
## \#10 Posted by: scepterr Posted at: 2017-09-29T17:06:11.214Z Reads: 176

```
If you're not planning to get it fixed wanna donate it for science?
```

---
## \#11 Posted by: Skitzor Posted at: 2017-09-29T17:42:23.843Z Reads: 172

```
If your terrain was vibrating, it's also likely that your phase wires internal in your motor rubbed against each other and lost the enamel, resulting in a phase wire short going back to your vesc. So I advise you to be carefull with that same motor.
```

---
## \#12 Posted by: Octavio Posted at: 2017-09-29T19:21:03.702Z Reads: 167

```
Would I be able to see this if I opened up the motor?
```

---
## \#14 Posted by: Octavio Posted at: 2017-09-29T19:25:18.246Z Reads: 162

```
Does it make sense, or is it possible to place a fuse between the motor and the esc? To protect it?
```

---
## \#15 Posted by: Skitzor Posted at: 2017-09-29T20:58:20.348Z Reads: 149

```
What I did (I had it on 2 different 6355 motors) i hotglued the entrance and the leads of the motor so the coating is preventing it from rubbing against the windings and wires on it's own. So far these are holding up for about 6 months. No issues with heat or melting of the glue.
```

---
## \#16 Posted by: onepunchboard Posted at: 2017-09-29T22:58:11.873Z Reads: 137

```
do u even know what drv is?😂
```

---
## \#17 Posted by: JohnnyMeduse Posted at: 2017-09-30T03:04:34.437Z Reads: 127

```
Direct Revolution per Voltage aka Torque per Speed.... 

Nha.... 😂  It's all bullshit except for the torque per speed...
```

---
## \#18 Posted by: Acido Posted at: 2017-09-30T09:33:42.338Z Reads: 109

```
ye but i didnt see the images some way i was on my phone so that might be the reason
```

---
## \#19 Posted by: ShawnyP Posted at: 2017-09-30T12:32:51.621Z Reads: 103

```
Hi i was wandering if any of the LED's were still working after your focbox got fried, reason i ask i have one was working now wont do anything just has rapid flashing blue LED?
```

---
## \#20 Posted by: Octavio Posted at: 2017-09-30T13:04:48.501Z Reads: 96

```
Yes. All are working. Blinking red.
```

---
## \#21 Posted by: ShawnyP Posted at: 2017-09-30T13:09:18.434Z Reads: 96

```
 Ah ok iv just got 1 blue rapid flashing different i must have a different fault, cant connect to the focbox either
```

---
## \#22 Posted by: ShawnyP Posted at: 2017-09-30T13:22:25.430Z Reads: 93

```
Thanks for reply man, just tried another battery fired up straight away at least i know where my fault is now
```

---
