# Vesc shows no Leds or usb funtion, but powers reciever after being connected by can bus

### Replies: 11 Views: 1637

## \#1 Posted by: uncosk8r Posted at: 2016-12-18T00:16:28.978Z Reads: 118

```
I was in the final stages of building an electric long/mountain board using a couple of hub motors salvaged from a dead hoverboard and re terminated as delta for more rpm.

I had sourced two vescs from "diyelectric skateboard", (one of which was dead on arrival due to a poor solder joint on the positive battery wire\capacitor board.(easily fixed..apparently they've never heard of quality control and don't test before shipping as they advertise)

Both then were fired up on 12V and found to be containing the latest firmware already were programmed for cut off voltages, but wouldn't detect the motors successfully on 12v.
At this point (having not fried on a power supply) they were connected to a higher voltage (10s2p lion) and detected the motors just fine.

Both were tested (on the bench) and seemed to work reasonably well.
they were then programmed for ppm, which after pulse width calibration performed as expected. (torqueboards nano remote and reciever)
           
I then reconnected them individually and altered the programming to enable dual motors and following the method outlined from vesc.net, setting the slave esc to "send can over bus" the motors were then connected the vescs in parallel to a 10s2p lithium ion battery (made of 2.2ah 1865 li-ion cells) as well as individually to the appropriate motors with the receiver plugged into only the master vesc. 

Only the motor connected to the master spun, and upon further inspection another cold solder joint which was apparently only being held on by flux residue had come loose and formed an intermittent connection on the slave vesc preventing booting (capacitor board negative lead out).
When held in position both vescs  booted and both motors performed as expected.
Everything was powered down, disconnected, at which point the offending solder joint was reflowed; the slave esc was then tested individually and performed as expected.

Everything was reconnected *exactly* as before,(even the motor leads were on the same vesc in the same order as before) but this time after a momentary function as expected,(with both motors spinning after a quick blip on the throttle) further input gave no response and upon closer inspection i found that the master vesc crashed and its blue led went out.

Upon disconnecting and reconnection of the power, I got no response to the ppm input and could see that although the slave vesc booted normally and reciever was still being powered by the master vesc, there were no other leds lit on the master.
The connections were double checked and found to be correct, the power was then disconnected.
The power was reconnected, and the same state was repeated (slave booted, master no response except to power the receiver)

Upon individual testing, the vesc that was set as the master continued to be unresponsive in every way including including no longer being detected by usb. (except for powering the receiver)

The Vesc that was set to slave still boots and performs normally.

Despite knowing how to solder well, I don't have any experience or the required equipment for surface mount components, and don't know quite enough about exactly how the vesc works to troubleshoot. 

In case it is relevant, I am using xt90 connectors for the batteries, and 5.5mm bullet connectors on the output leads.
The solder joints on these connections were mechanically and electrically tested and found to be of good quality (mechanically sound, no added resistance)
Its also worth noting that the shrink wrap was only removed after the testing, in order to take the pictures, and didn't have any obvious signs of smoke or heat damage.

Despite knowing how to solder well, I don't have any experience or the required equipment for surface mount components, and don't know quite enough about exactly how the vesc works to troubleshoot it.
 "diy electric skateboard" will not repair them without a significant and undisclosed cost (and taking into account that they charge $40 just to ship, as well as the extremely long international shipping times....also, if they cant even get a good joint on a power lead......) 

I'd obviously like to have this vesc repaired as it was a considerable investment, but avoiding the supplier due to the above reasons, would rather have it repaired somewhere else if possible, but unfortunately upon further research, it appears that there is nobody who will, (particularly in Australia) repair this for me at any cost. 

Having a very expensive paperweight that can't be repaired is obviously not an attractive option, and as such if necessary will try to effect a repair myself; I would have done so already, but the vesc is *much* more complex than anything that I've ever worked with before, and as such i need a little help in diagnosing this thing.

I didn't see any obvious signs of damage (burnt chips etc), but admittedly this was only done with the naked eye as I don't currently have access to any magnifying devices.
Because of this, I've attached some pictures of the vesc taken with the highest resolution camera that I could source.

Although the positive input lead *looks* like it could short on the pins beneath it, it can not be made to touch. (because the wire is apparently filled with solder and is too rigid to move)

I'd attach screenshots of the bldc settings, but cant get the vesc to show up on usb as it did previously, but outside of voltage cutoff limits, ppm, and motor detection, the settings are default.
(also set to  "current, no reverse")

Any help you can offer would be greatly appreciated.

(edit, Sorry for the long winded post, I wanted to be sure to include all relevant information.
<img src="/uploads/db1493/original/3X/d/8/d8424ac0497fbe3e688a858e6fcdebc4bbe0918b.JPG" width="375" height="500"><img src="/uploads/db1493/original/3X/1/1/1112319b71eb27ef79c964f7a6ae0274805268a6.JPG" width="666" height="500"><img src="/uploads/db1493/original/3X/0/f/0f7ed654cd8d338215f110858f89ac73339e8cdf.JPG" width="375" height="500"><img src="/uploads/db1493/original/3X/e/6/e613b66d273543a2756f524b2c39f4cd3dd1111a.JPG" width="666" height="500"><img src="/uploads/db1493/original/3X/b/8/b8cf9c8a2de0329c8eae30270c4f428a8f8ea442.PNG" width="281" height="500"><img src="/uploads/db1493/original/3X/7/e/7ead1c35978cad682d38739d1407e036ef42f0be.JPG" width="666" height="500"><img src="/uploads/db1493/original/3X/9/c/9ce3042434345b7b6bfe15c67f263307a98c626e.JPG" width="375" height="500">
```

---
## \#2 Posted by: saul Posted at: 2016-12-18T01:32:52.423Z Reads: 88

```
only made it though part of that wall of text. keep it short if you want more responses, we are kinda lazy thats why we put motors on our skateboards lol

post your vesc settings,
test them individually.

i'll try to read more later lol :nerd:
```

---
## \#3 Posted by: uncosk8r Posted at: 2016-12-18T02:22:39.022Z Reads: 88

```
I did that....


The wall of text was in response to the  "If you don't have enough details or a minimum of four pictures, we'll just delete your post" note posted by the admins.

In short, both vescs were working with default settings except those outlined in the dual vesc via can bus walkthrough and the cutoff voltages for the 10s pack (26v).
After connecting them via can-bus and successfully running the motors for a moment it stopped working and no motors spun.

when tested individually, the one that was the master is now seemingly dead.

The wall of text was unfortunately required to fit enough detail to prevent replies suggesting things I've already tried.
```

---
## \#4 Posted by: JohnnyMeduse Posted at: 2016-12-18T02:26:40.664Z Reads: 86

```
Check the can tranceiver

http://www.electric-skateboard.builders/t/no-power-to-enertion-vesc/7600/8?u=johnnymeduse
```

---
## \#5 Posted by: uncosk8r Posted at: 2016-12-18T04:59:22.850Z Reads: 77

```
Thanks, I've tested as per the link, and I think your probably correct.

When testing across c25, I get the same result as shorting the meter probes against each other. (a short)
Considering that the problem started when connected via the can-bus, and the vesc worked previously, it makes sense that it would be the can transceiver that has an issue and not a solder bridge somewhere.

Is there any way to test this component to be certain? (u401)

What other components might it be?

Assuming that it is indeed the can transceiver that is damaged, what could have caused it to malfunction? (to prevent it happening again)

Ive ordered one from mouser, any tips on removing/replacing without damaging anything else or lifting the traces?
```

---
## \#6 Posted by: JohnnyMeduse Posted at: 2016-12-18T05:22:58.953Z Reads: 70

```
pretty sure it is u401(experience tel me this), but the best way to test is by removing u401 (by unsoldering it) from the circuit, and then do the test again.

 Or if try the same procedure but over cap c33 (that will tell you if u2 is problematic)

but still if you have a short over c25, it is 90% chance of u401 busted (it is the only chip that doesn't have any protection)
```

---
## \#7 Posted by: JohnnyMeduse Posted at: 2016-12-18T05:25:07.599Z Reads: 73

```
[quote="uncosk8r, post:5, topic:14841"]
any tips on removing/replacing without damaging anything else or lifting the traces?
[/quote]


best way is to use hot air station.
```

---
## \#8 Posted by: uncosk8r Posted at: 2016-12-18T06:20:04.984Z Reads: 67

```
I've just tested over c33 on your reccomendation, and got the same result.

Since I don't have the appropriate tools with me at the moment to remove u401, and the part is <$2, Ive ordered a few so that when I get access to a hot air station in a few days I can just mount the new part right away if the test result changes when that part is removed.

I'll add a further update once I've tried that test and solution in a few days.
```

---
## \#9 Posted by: Eboosted Posted at: 2016-12-18T06:49:23.241Z Reads: 67

```
I've been using chipquik instead of hot air for a while, amazing stuff, really cheap, can remove any SMD in seconds, afterwards just use wick and flux to absorb the lead and clean the board with isopropyl alcohol and a soft brush

https://www.amazon.com/ChipQuik-SMD1-Leaded-Temperature-Removal/dp/B0019UZP7I/ref=sr_1_1?ie=UTF8&qid=1482043553&sr=8-1&keywords=chipquik
```

---
## \#10 Posted by: uncosk8r Posted at: 2016-12-30T13:59:53.914Z Reads: 58

```
Finally got access to my hot air station again and successfully removed u401 (and C401 by accident....), but am still getting continuity over c25.
I am however *not* detecting continuity over C33 as I did before the removal of u401.

Does this mean that U401 was not the problem?
If so, what else could it be?
```

---
## \#11 Posted by: Jebe Posted at: 2017-02-17T09:48:40.976Z Reads: 44

```
Bumpo - anyone else got any ideas?
```

---
