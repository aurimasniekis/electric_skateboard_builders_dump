# No power to Enertion Vesc

### Replies: 32 Views: 4408

## \#1 Posted by: Strawbs Posted at: 2016-08-13T18:15:50.489Z Reads: 181

```
So I finally got my board put together, and tested it out on my first ride.  About 5 minuets in I lost power to the motors.  Came home to check it out and I find that the master VESC is not turning on.  I've emailed Enertion Support and am waiting for a response.  Attached are some images of the VESC.  Any suggestions?

Thanks,

<img src="/uploads/db1493/original/2X/1/1088d5b21c25af46b80b49152ecd1fe445f3031e.JPG" width="375" height="500">
<img src="/uploads/db1493/original/2X/2/2e1580b9773e3632e55e5597b81732b122a6f2fb.JPG" width="375" height="500">
```

---
## \#2 Posted by: Skitzor Posted at: 2016-08-13T18:34:56.191Z Reads: 170

```
Dont want to state the obvious, but did you check the vesc warning about piercing the red power lead on the bottom?
```

---
## \#3 Posted by: Strawbs Posted at: 2016-08-13T18:40:14.632Z Reads: 174

```
I did,  there appears to be a small indentation on the red wire.  I noticed it when it arrived in the mail, so I re-did the heat shrink to prevent any further damage.  The plastic wire is not punctured, but like i said there is a mark.  Could this cause failure?
```

---
## \#4 Posted by: Skitzor Posted at: 2016-08-13T19:08:34.751Z Reads: 167

```

What exactly were you doing at the time of shut-down of the vesc? 
Have you tried mesuring he voltage, is that still coming trough?
Have you checked all components? Smd-connections? Does something smell burned?
Have you tried it again after an hour or so to make sure it wasn't just over-heating?
What battery are you using?

Sorry for all the questions, just trying to pinpoint you in the right directions and getting some info gathered for other members that would chime in.

The red wire should be good then if you checked and upgraded the protection.
```

---
## \#5 Posted by: Strawbs Posted at: 2016-08-13T19:13:36.245Z Reads: 168

```
I was riding on flat ground for about 5 minuets before it cut out for a second, then came back for a second, then went out completely.  

I have checked all connections and tested my XT-60 wires,  they all work fine.  The master VESC is not powering on.  

I have not tried to measure the voltage.  I don't have the equipment to do so.

I don't believe it was an over-heating issue,  I came home about 30 min later, unplugged everything removed the vesc and tested it at my PC.  No response.
```

---
## \#6 Posted by: JohnnyMeduse Posted at: 2016-08-13T19:31:05.851Z Reads: 169

```
Do you have a multimeter with you? If so can you check if you have continuity between the 5v and the gnd (or C25 capacitor)

Edit: If the power led doesn't light up, It may be a failure of the can tranceiver (U401)
```

---
## \#7 Posted by: Strawbs Posted at: 2016-08-13T19:45:31.044Z Reads: 197

```
I don't have a multimeter,  but I can pick one up today.  Do you have any resource to show me how to test these things?
```

---
## \#8 Posted by: JohnnyMeduse Posted at: 2016-08-13T20:51:07.982Z Reads: 194

```
1- You need to put the Multi-meter in diode Check mode. (should be a symbole similar to this one)
<img src="/uploads/db1493/original/2X/2/2988d03d7616a80cc5936ddd8ee9a46cb76c5927.jpg" width="666" height="500">

2- Check if you get a beeping song when touching de lead together.  (or if you don't hear any sound check if the multi-meter show 0000 or something similar)
<img src="/uploads/db1493/original/2X/e/ee88b16605551db247f2809e5d686d8ca8db4636.jpg" width="666" height="500">

3- Use the c25 capacitor to see if the 5v is short to the ground (it is the easiest part to access for checking the 5v to the gnd)
<img src="/uploads/db1493/original/2X/a/aad1723f09da6b393a64bd1c4b649897cb89e710.jpg" width="666" height="500">

4- If you the doesn't get the same result as touching the lead together, GOOD New the 5v is ok, but the problem is somewhere else. But if you get a beeping sound or the result is the same as touching the lead together, then you have a short over the 5v, and from my experience, it is 90% chance of a internal short over the can tranceiver (u401).

<img src="/uploads/db1493/original/2X/3/3edcca9df7def3fae966f7457cebb3a8297f6861.jpg" width="666" height="500">
```

---
## \#9 Posted by: Strawbs Posted at: 2016-08-13T21:07:05.674Z Reads: 181

```
Wow thanks.  I'll go grab a multi-meter and check this.  

Do I have any options to fix this?  Or will I need to replace the VESC regardless?

I'm not very good a soldering and I don't want to void my warranty.
```

---
## \#10 Posted by: JohnnyMeduse Posted at: 2016-08-13T21:12:21.676Z Reads: 184

```
Well, do you have the enertion warranty, if so I think you might need to wait for their respond, and you might need to send it, to their USA manufacturer
```

---
## \#11 Posted by: Strawbs Posted at: 2016-08-13T22:03:38.645Z Reads: 177

```
Ok UPDATE!

The vesc turned on again.  I'm able to access the settings in the BLDC tool.  Can someone please take a look at my motor settings and make sure I'm not pushing the VESC too hard or something?  

Dual Enertion R-Spec motors
Space cell pro-4
Enertion receiver and remote

<img src="/uploads/db1493/original/2X/2/22563175a79f1b5fd1ed7a465344ae7c81fc94f4.PNG" width="690" height="407">
```

---
## \#12 Posted by: Evan Posted at: 2016-08-13T22:13:19.005Z Reads: 162

```
Maybe try to set max input higher than 42v.....  I got a similar problem [here](http://www.electric-skateboard.builders/t/battery-voltage-and-max-input-setting/7589).
```

---
## \#13 Posted by: JohnnyMeduse Posted at: 2016-08-13T22:18:28.531Z Reads: 162

```
Put the max voltage at around 57V if you are using a space cell pro, also I may suggest to drop the MAX ERPM to 70 000 to prevent damage on the drv.
```

---
## \#14 Posted by: Jinra Posted at: 2016-08-13T22:30:59.601Z Reads: 164

```
If you're running dual motors, your current limits are too high. Keep in mind that values should be halved since you're running dual setup. I'd make motor max 40-50 per vesc and adjust as needed. motor regen should be at 40ish or you will be braking pretty hard. Battery max is a bit low and should be higher at about 30amps per VESC. Your SCP4 supports 80A continuous, but you want to try to be below that. Battery regen is too high and it should be -8A per VESC for safe charging.
```

---
## \#15 Posted by: Strawbs Posted at: 2016-08-13T22:39:15.398Z Reads: 156

```
Wow thanks guys.  Glad I asked.

See below for new config.  Any last things before I stress test it?

Thanks.

<img src="/uploads/db1493/original/2X/9/9c3b82eba863312ea09187ed8fcec53160f1111b.PNG" width="690" height="295">
```

---
## \#16 Posted by: Jinra Posted at: 2016-08-13T22:40:58.677Z Reads: 148

```
Looks good, though your low voltage cut off end is a bit low. You can keep it at that for more range, but make sure you get to a charger asap when you feel it kicking in.

This gives you an idea of how a voltage meter reads % to voltage.

http://www.electric-skateboard.builders/uploads/db1493/original/2X/f/fb95302d91aa992329d1d0ccb21f626ae71fc139.png
```

---
## \#17 Posted by: JohnnyMeduse Posted at: 2016-08-13T22:42:17.987Z Reads: 142

```
Maybe you should follow @onloop advise, for is setup.

http://www.electric-skateboard.builders/t/vesc-faq-regen-braking-configuration-bldc-tool-brake-force/353
```

---
## \#18 Posted by: Jinra Posted at: 2016-08-13T22:45:36.585Z Reads: 138

```
My advice is similar to his, though he was speaking about the SCP3 not 4
```

---
## \#19 Posted by: Strawbs Posted at: 2016-08-13T22:46:01.422Z Reads: 134

```
Got it Jinra,  

Looks like 36 at 10s would be safer.  I'll update that.
```

---
## \#20 Posted by: Jinra Posted at: 2016-08-13T22:47:37.467Z Reads: 135

```
I do 33v cut off start and 32v cut off end personally. You're voltage will sag while riding so if you start the cut off too high you might trip it when riding with high current draw like up hills.
```

---
## \#21 Posted by: JohnnyMeduse Posted at: 2016-08-13T23:05:03.254Z Reads: 129

```
I did not say that your advice where not good, but,  there is not so much difference between the SCP3 and SPC4, because by using the same 10S bms, they are in fact limited to the same continuous current. The major difference between the two are in term of the capacity and range they provide.

Also, you may want to use a lower Batt Min, at around -15A so it will provide a better braking solution.
```

---
## \#22 Posted by: Jinra Posted at: 2016-08-13T23:07:28.867Z Reads: 121

```
Actually the SCP4 outputs 80A continuous vs 60A on the SCP3 due to the extra parallel cell. This also affects charging current so -8A battery min (dual vesc) is the safe spot for these cells. There is more capacity on the SCP4, but charging/discharging is also affected.

I have -8A on my dual VESCs with 45A motor regen and have no problem braking hard.
```

---
## \#23 Posted by: JohnnyMeduse Posted at: 2016-08-13T23:16:14.923Z Reads: 118

```
Yes you are right, my mistake there is a difference between the SPC3 and SPC4, but the continuous current is still not rated for 80Amp, it is  the peak current at 80amp.

> Pack rated to peak output of 80AMP, However incorporates a 40A Fuse for protection, this is ample for use on electric skateboards. This pack is for motors of 2400W or less (Including the 6372)

http://www.enertionboards.com/electric-skateboard-parts/space-cell-pro4-electric-skateboard-battery/
```

---
## \#24 Posted by: Jinra Posted at: 2016-08-13T23:18:11.208Z Reads: 116

```
peak is actually higher than 80A, but you're right it wont support continuous 80A, but should work for bursts. I've been trying to find a small fuse that's rated higher than 40A to replace the stock one, but have had no luck finding one in this size. I may just swap out the fuse holder for a larger one that supports 80A.
```

---
## \#25 Posted by: JohnnyMeduse Posted at: 2016-08-13T23:30:00.775Z Reads: 111

```
But, be aware I think there BMS is only rated for 60AMP. So if you're going over the bms limits you will probably burn the bms internal fuses (if there one, but with these Chinese (for now...)  product you never know), or the BMS.
```

---
## \#26 Posted by: Jinra Posted at: 2016-08-13T23:31:32.975Z Reads: 105

```
True, I'm not too concerned though as I'll replace the BMS as well. Though with my current limits and constant uphill riding, I've never tripped the 40A fuse yet. Esk8 probably doesn't pull that many continuous amps at 10s.
```

---
## \#27 Posted by: Strawbs Posted at: 2016-08-13T23:34:47.133Z Reads: 105

```
Ok, I put everything together and all seems to be in working order.  However the motors only spin together intermittently.  I think my JST connector is faulty.  When I jiggle the wire the motors spin together, otherwise I only get one. I bought a JST connector from Ollin board co, but it broke immediately.  I'm currently using one from a local hobby shop.  Anybody have a good recommendation for a quality JST that will last?
```

---
## \#28 Posted by: Jinra Posted at: 2016-08-13T23:37:15.367Z Reads: 106

```
I wouldn't recommend connecting it like this for this reason. Mine would move ever so slightly and cut out my motor. I gave up on various solutions and settled on soldering the connection in place.
```

---
## \#29 Posted by: Strawbs Posted at: 2016-08-13T23:38:25.730Z Reads: 107

```
Interesting,  I didn't know that was an option.  Do you have any pictures?
```

---
## \#30 Posted by: Jinra Posted at: 2016-08-13T23:39:09.570Z Reads: 111

```
http://www.electric-skateboard.builders/t/honey-driver-honey-velocity-v3-deck-caliber-iis-83mm-evolve-gt-wheels-dual-om5065-200kv-space-cell-pro4-diy-pulleys-enertion-pulley-bones-super-reds-enertion-mounts-winning-remote-chaka-vescs-build-complete/5760/73?u=jinra

You can take the wires out of the plastic JST housing and solder directly to the pins. Make sure to push all the way down.
```

---
## \#31 Posted by: Strawbs Posted at: 2016-08-13T23:46:44.294Z Reads: 110

```
Got it.  What is the purpose of the ferrite ring?
```

---
## \#32 Posted by: Jinra Posted at: 2016-08-13T23:47:40.105Z Reads: 113

```
to clean up electrical noise and interference, though probably not necessary on the CAN cable.
```

---
