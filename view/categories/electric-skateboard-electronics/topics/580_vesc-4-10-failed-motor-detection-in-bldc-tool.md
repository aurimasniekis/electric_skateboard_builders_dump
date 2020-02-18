# Vesc 4.10 &ldquo;failed motor detection&rdquo; in BLDC tool

### Replies: 23 Views: 4388

## \#1 Posted by: Alex Posted at: 2015-11-25T18:49:20.762Z Reads: 265

```
hello

I received my vesc about a month ago and everything was great right out of the box. I had roughly 10 hours of issue free ride time when randomly while cruising I lost full control of vesc. Blue and green led lights remained illuminated as usual. I walked home and plugged in the vesc and opened bldc tool on OS X. With Vesc connected as it should I did a quick run through to see if everything was functioning. I was unable to control motor in experiment so I attempted to detect motor and it displays "detection failed.”

Motor, wires and connectors tested good with seperate esc and multimeter.

At this point Im not sure what is wrong. I fear I may have shorted one of my capacitor leads to vesc board but I figure it would fry everything if that happened. 

Do you fellow riders happen to have any suggestions? 

My build 
Sk3 6364 190kv 
1:2 drive ratio
83mm wheel
Vesc 
Quantum pistol transmitter and receiver
2 4s multistar 16ah lipo in series
```

---
## \#2 Posted by: elkick Posted at: 2015-11-25T18:56:37.038Z Reads: 248

```
The blinking red and blue  lights indicate that indeed one of the caps might be damaged. Can you here a "blistering" noise from the backside of the VESC when you power on/off the VESC?

If so, you just need to replace the damaged cap. The VESC might still work.
```

---
## \#3 Posted by: Alex Posted at: 2015-11-25T19:04:47.333Z Reads: 239

```
Thanks for the quick reply.
So far I haven't noticed any blinking lights. Just a steady blue when I first power up vesc and within several seconds the green led also illuminates. Both led illuminate constant
```

---
## \#4 Posted by: lowGuido Posted at: 2015-11-25T20:05:17.138Z Reads: 234

```
Does the motor make any humming noises? 
I found with my 4.10 from enertion i had to re flash the firmware before it would work. I think it was pre programmed for the type r and wouldnt play with my sk3.
```

---
## \#5 Posted by: Alex Posted at: 2015-11-25T20:15:49.875Z Reads: 232

```
Unfortunately no humming noises or movements from the motor. Not even a measure of voltage from the phase wires.

How did you re flash the firmware?
```

---
## \#6 Posted by: lowGuido Posted at: 2015-11-25T20:32:42.472Z Reads: 226

```
http://www.electric-skateboard.builders/t/vesc-firmware-update/237/2
```

---
## \#7 Posted by: Alex Posted at: 2015-11-25T20:52:57.172Z Reads: 215

```
Thanks a lot for your help.
I re uploaded the FW and corrected all my settings and still no luck :(
```

---
## \#8 Posted by: lowGuido Posted at: 2015-11-25T22:23:32.322Z Reads: 218

```
I guess there is something going wrong on the output side of the VESC then if you can read and load firmware ok.
```

---
## \#9 Posted by: onloop Posted at: 2015-11-25T22:41:52.327Z Reads: 212

```
Go over all the soldered wires to ensure everything is well soldered, double check motor wires to make sure all connections are good. no cold solder joints.
```

---
## \#10 Posted by: Iceni Posted at: 2015-11-26T21:12:00.312Z Reads: 208

```
Not sure if it's applicable in your case since you managed to ride it for a while before it happened, but one of my vescs had a shorted pin on one of the big chips by the motor leads, might want to check if that's the case.
Posted a pic of it in my build thread.
Might be worth a shot.
```

---
## \#11 Posted by: Alex Posted at: 2015-12-02T04:03:51.985Z Reads: 198

```
I finally found some time to check out my vesc. I replaced motor wires and resoldered connections. visually inspected the board and everything looks normal. No signs of shorts or anything for that matter
```

---
## \#12 Posted by: Alex Posted at: 2015-12-02T04:14:27.153Z Reads: 198

```
still no luck with motor detection in bldc tool
```

---
## \#13 Posted by: Moja Posted at: 2015-12-18T06:48:46.716Z Reads: 193

```
Im getting the same error message, when I try to detect the motor is jerks once, then again 10 seconds later and it gives me this error. Im using the 4.10 VESC's with the 2.3 BLDC, both have the blue and green lights on. The other motor is fine and its the exact same assembly. 

<img src="/uploads/db1493/original/2X/0/0dd392641b34203b64ac0d6835410d0412ffbf0c.png" width="690" height="361">
```

---
## \#14 Posted by: jonathanngkh Posted at: 2016-01-21T16:05:22.815Z Reads: 176

```
Has this been resolved, if so how?
```

---
## \#15 Posted by: chaka Posted at: 2016-01-21T22:05:58.021Z Reads: 172

```
@jonathanngkh This is a symptom of a variety of things. What do you have going on, any fault codes?
```

---
## \#16 Posted by: jonathanngkh Posted at: 2016-01-21T22:08:39.356Z Reads: 172

```
@chaka I posted this on my own thread earlier at http://www.electric-skateboard.builders/t/diy-electric-penny-board-first-build/992/30

Hi guys, I made some progress today. Soldered the nyko kama nunchuk receiver to the jst connectors and they connect just fine. Soldered the vesc to the motor connectors too, and soldered leads for my zippy batteries.

But I think I fudged up my vesc, really hope not. I was having a lot of trouble with the BLDC, but eventually i got it connected. Motor detection wasn't working, but then I realised that was because i had my receiver plugged in. So I unplugged it, rebooted and reconnected and ran motor detection.

VEEEEEEE the motor starts going, slows down just like in Vedder's video, then VSH it starts up and chokes. Next thing I know, the VESC is no longer connected, and the LEDs on the VESC no longer light up, so I can't connect it.

I had my space cell connected to the VESC, VESC connected to motor. Did it short? Is it fudged? Should I get a new one? If so, how do I prevent the same thing from happening?

So close, yet so far
```

---
## \#17 Posted by: ikjahaa Posted at: 2016-07-26T20:02:50.110Z Reads: 126

```
Did you solve this problem yet ?
```

---
## \#18 Posted by: DevinG Posted at: 2018-04-18T01:36:12.361Z Reads: 42

```
And now I find myself here....
```

---
## \#19 Posted by: Redfire1 Posted at: 2018-06-19T07:00:02.399Z Reads: 38

```
@ckaka or any who know how used VESC TOOL not BLCD TOOL hi do you know anything about Vesc tool I need some help to program my Vesc it only works with Vesc tool not blcd,I copy some set set up on YouTube but my brake don’t work down hills ![image|374x500](upload://ykOYaWfGnAVKymQO4L2bv6w7HU2.jpeg)
```

---
## \#20 Posted by: Ebisane9 Posted at: 2018-06-19T14:17:50.694Z Reads: 39

```
your setup is incomplete... those boxes should be green
```

---
## \#21 Posted by: Redfire1 Posted at: 2018-06-19T20:10:36.302Z Reads: 39

```
@Ebisane9 that’s what I am saying I look on YouTube to program my vesc so that’s why I am asking for help and who used the VESC Tool before.
```

---
## \#22 Posted by: JohnnyMeduse Posted at: 2018-06-19T20:16:33.918Z Reads: 39

```
If you have a 4.10 hardware, I DO NOT RECOMMEND using the new firmware, specially in FOC, it won't damage your esc but it will do some false DRV error. If you want to use the newer firmware you need to add a 4,7uF cap in parallel to C18.
```

---
## \#23 Posted by: Redfire1 Posted at: 2018-06-20T05:12:45.100Z Reads: 30

```
@JohnnyMeduse hi I have spoken to the supplier and they said the Vesc software don’t need updating,I just want to know how to program it so I can drive and when going down hill it brake
```

---
