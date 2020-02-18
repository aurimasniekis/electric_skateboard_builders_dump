# Frequent DRV8302 Faults? Help me troubleshoot! (With telemetry)

### Replies: 22 Views: 1435

## \#1 Posted by: jmasta Posted at: 2017-07-23T01:17:08.960Z Reads: 141

```
Frequently I am getting a **DRV8302 Error** while riding, but otherwise the board functions fine.  When this occurs, the VESC abruptly cuts out. In one example, you can see I went from 24mph to 12mph in less than a second (_Example 1_).  Needless to say, the transition from 30A to 0A is very jarring.  It has nearly sent me to the pavement a few times.  Once or twice has even briefly applied a braking current of up to -20 motor amps!  Talk about wobbles...

In total I have received the DRV error **at least 6 times**, but it has been more frequent as of late.  Typically I get the fault code while climbing a steep hill, so I thought it may be related to high current draws. But today I received the same error on flats in the first 3 minutes of my ride, while pulling only 11A (_Example 2_)

**Setup:**

* VESC v4.12 (2.18 firmware) - from DIY
* SK3-6374 149kV @ 12S
* 18:34, 15mm belt drive on 83mm wheels 
* FS-GT2B Remote (stock)

**Troubleshooting** _(Tried all of these, and still received error after)_:

* Removed belt and re-performed motor detection
* Reduced motor amps
* Reduced battery amps
* Check for loose connections. Taped phase wires
* Checked for potential shorted pins on the VESC


**Telemetry:**

**_Example 1:_**

* DRV8302 Error 

<img src="/uploads/db1493/original/3X/4/2/42d730dcbcb6b3d104fedf54e54cd2d4c4c9c5ed.jpg" width="347" height="500">
<img src="/uploads/db1493/original/3X/4/c/4c37103fb6a7896377945a719d24c897a7a16a13.jpg" width="348" height="500">

https://metr.at/r/AdYXH

==================================================

**_Example 2:_**

* DRV8302 Error 
<img src="/uploads/db1493/original/3X/8/5/85cee80cfe8f220e24da4b78493e2c2dadd8d36a.jpg" width="349" height="500">

<img src="/uploads/db1493/original/3X/c/d/cd07439eab0f721e6def86abef323ff36b9ee1db.jpg" width="348" height="500">

=====================================================================

**VESC Settings:**

<img src="/uploads/db1493/original/3X/f/1/f15b62191a6ccb9bef992f427cfaf8d409f012a4.png" width="690" height="420">

<img src="/uploads/db1493/original/3X/4/d/4d0aba3f0c74c5ce44a871df1fde769a1433bfe3.png" width="690" height="421">


<img src="/uploads/db1493/original/3X/6/2/62a5b0d286d83b0d31afebbbd493de3619f371a6.png" width="690" height="421">


<img src="/uploads/db1493/original/3X/f/8/f8684cb09e8e509f74be6649349c9af06543a19c.png" width="690" height="420">
```

---
## \#2 Posted by: rpn314 Posted at: 2017-07-23T03:46:47.531Z Reads: 116

```
It sounds like your DRV chip is failing. They don't always die in one massive boom, sometimes it's more of a slow death. Unfortunately, since your description seems to indicate it getting worse I'd say slow death. Mine did something very similar.

Still post your settings, especially the advanced tab. Maybe we can see what if it was caused by a settings issue.
```

---
## \#3 Posted by: Namasaki Posted at: 2017-07-23T06:56:18.800Z Reads: 113

```
[quote="jmasta, post:1, topic:28332"]
Removed belt and re-performed motor detection
[/quote]


Did you also remove the motor pulley to do the motor detection?

I did a comparison just the other day.
motor detection with motor pulley on and again with pulley off.
It made a difference in the bemf coupling by 100 points
```

---
## \#4 Posted by: jmasta Posted at: 2017-07-24T00:15:26.487Z Reads: 100

```
Thanks @Namasaki!  I did not realize the motor pulley would make that much difference. I will brave the red loctite removal and rerun the motor detection.  I posted a screenshot from the current motor detection settings (belt removed, but motor pulley still affixed)

[quote="rpn314, post:2, topic:28332, full:true"]
It sounds like your DRV chip is failing. They don't always die in one massive boom, sometimes it's more of a slow death. Unfortunately, since your description seems to indicate it getting worse I'd say slow death. Mine did something very similar.
[/quote]

I was afraid of that...  It's been working great for most of the year, and only starting giving the DRV in the last month or so.  Unfortunately I did not buy a VESC with a warranty (this time...)

 I updated the original post with my VESC settings.  Please take and let me know what you think.  The soft battery cutoff is set fairly low, because I have found that is anything but "soft"
```

---
## \#5 Posted by: rpn314 Posted at: 2017-07-24T00:50:24.922Z Reads: 90

```
Sorry to be the bearer of bad news: guaranteed you have a dead DRV chip. On the advanced tab, the max current ramp step has maxed at 50 (should be about 0.04). You have the buggy version of firmware 2.18.
```

---
## \#6 Posted by: jmasta Posted at: 2017-07-24T02:37:28.607Z Reads: 88

```
Nice catch, thank you!  I even checked to make sure I did not have the current ramp bug when I first got the VESC, but clearly I missed it

I reprogrammed it using a value of 0.004 for the current ramp step, so it ends up at 0.04 after one configuration write.  I'll install new firmware when I have time (either the native firmware for Metr, or the one for watt control)

After a quick test, it feels much better and no errors yet. But I didn't push it very hard.  Only pulled around 15A max on somewhat flat ground

https://metr.at/r/e9qDL
```

---
## \#7 Posted by: Hummie Posted at: 2017-07-24T02:55:28.362Z Reads: 85

```
What's the back emf coupling?
```

---
## \#8 Posted by: jmasta Posted at: 2017-07-26T00:02:35.581Z Reads: 80

```
Yep it's official. This VESC is going to kill me.  The DRV chip is definitely failing.  Received the same error charging up a steep hill today. Continued on riding without stopping, but that transition from +30A motor current to -23A braking current....  _wow_.   It gave me such serious "whiplash" that my front hand nearly slapped the pavement.  Good thing I was in a race stance with a lowered CG or it definitely would have tossed me...

Pretty disappointed in DIY/TorqueBoards for selling a VESC with bugged firmware, months after the bug had been reported.  It ended up frying my VESC and could have seriously injured me on multiple occasions.  Going to hit up @chaka for a legit VESC with a warranty.  Ollin's product support has been stellar so far


<img src="/uploads/db1493/original/3X/d/2/d2dbe56600ca323dee732173d1f297a9d41fbe59.PNG" width="281" height="499">

<img src="/uploads/db1493/original/3X/9/a/9ac3a14997f517095a3c35f9444d5a02475eea8b.PNG" width="281" height="499">
```

---
## \#9 Posted by: rpn314 Posted at: 2017-07-26T00:40:46.514Z Reads: 75

```
Yeah, it was a very unfortunate bug. I fried 2 DRV chips (though I soldered my own VESCs, so it wasn't as big a deal for me since I could just replace them myself). I wish vedder had made the fixed version 2.19 instead of keeping the same version 2.18, cause it's pretty impossible to tell if it's the buggy one before loading it.
```

---
## \#10 Posted by: Jinra Posted at: 2017-07-26T00:42:00.558Z Reads: 76

```
My rule of thumb is to just reflash f/w no matter who I get it from. Or just flash Ackmaniac's f/w.

chaka once said that he doesn't think this bug has any effect on the drv issue, but from all the examples, I've seen, I don't think that's right.
```

---
## \#11 Posted by: rpn314 Posted at: 2017-07-26T01:03:14.420Z Reads: 72

```
The problem is I was fairly new here and didn't know who was a reputable download source (before I learned how to compile it myself)

I'm fairly confident the bug definitely caused (or at the very least accentuated) DRV error
```

---
## \#12 Posted by: Jinra Posted at: 2017-07-26T01:04:34.454Z Reads: 69

```
Just to clarify I mean that I don't believe chakas claim was right and i definitely do think it has led to some burned VESCs
```

---
## \#13 Posted by: jmasta Posted at: 2017-07-26T01:12:41.254Z Reads: 72

```
It seems to make sense to me that a high current ramp step could be the cause of the DRV error.  I interpret this parameter to be the maximum allowable change in current per time step  (or the maximum rate of change of current). Every time I received the DRV8302 fault was after a high current flux (e.g., while climbing a short steep hill, or after accelerating hard from a rolling stop)
```

---
## \#14 Posted by: jmasta Posted at: 2017-11-26T17:20:18.753Z Reads: 67

```
Well now I'm stumped...  I replaced the suspected faulty TB VESC with a brand new Ollin VESC 4.12.  After configuring all the settings and running motor detection, I got another DRV8302 error while bench-testing at max throttle.  The error occurred after less than one minute of use.  The VESC reset and there was no permanent damage as it still works fine.  But I can't figure out what could have caused the DRV error again.  Any ideas?

My two theories were a faulty DRV chip or a battery problem.  I'll spare you the details, but after lots of troubleshooting the battery is fine.  The VESC is brand new.   I took everything apart and checked for cold solder joints.  There are no shorts and the phase wires are taped

What could be the source of the non-latching DRV8302 error on the brand new Ollin VESC?   
@Jinra @rpn314 @chaka    

Here is the Metr log which shows the DRV error while bench-testing. Notice that the error occurred while only pulling 1.4A


https://metr.at/r/2KXMJ
```

---
## \#15 Posted by: chaka Posted at: 2017-11-26T17:23:53.001Z Reads: 64

```
What motor are you running?. Is it a cheap hub motor? I have a few other customers frying hardware on a those cheap little bastard motors.
```

---
## \#16 Posted by: jmasta Posted at: 2017-11-26T17:25:22.661Z Reads: 61

```
It's an SK3-6374 149kV from HobbyKing. Single drive
```

---
## \#17 Posted by: chaka Posted at: 2017-11-26T17:26:16.445Z Reads: 61

```
Was just editing my post after I read your initial post. What mode are you running?

Also, what battery are you running? Are you using a BMS?
```

---
## \#18 Posted by: jmasta Posted at: 2017-11-26T17:33:05.078Z Reads: 65

```
BLDC mode.  Never touched FOC. Running the stock firmware included with your VESC right now

Battery is 4x 3S Zippy 40C 6.2Ah wired in series.  I am in the process of building a 12s4p 30Q battery

SuPower 60A 12S BMS
```

---
## \#19 Posted by: chaka Posted at: 2017-11-26T17:38:44.695Z Reads: 67

```
If the VESC is toast we can throw another one at your build but you might have something else going on with your board. I would check that motor as best as you can for broken windings or a possible short where the phase wires enter the motor housing. Keep us posted with what is going on with it and we will help you out the best we can.
```

---
## \#20 Posted by: jmasta Posted at: 2017-11-26T18:19:43.452Z Reads: 70

```
The VESC is still good.  Nothing is blown.  I ran it on the bench after the error and wasn't able to replicate it.  Even after getting dozens of DRV errors on the old TB VESC, there was never any permanent damage to the speed controller after  it reset

But.... Thanks to your suggestion,  I think I found the problem

**Broken motor winding**.  You can see an impact mark on the windings and one strand is clearly broken

<img src="/uploads/db1493/original/3X/0/c/0ce85be4fe86b6c4b9383d8893ae2704b41b88c8.png" width="374" height="500">

So the good news is it's not the VESC. Bad news is I spent  $500 replacing the VESC and building a new battery, only to figure out I need a new motor :sweat_smile:

 Or at the very least, I need to redo all the windings
```

---
## \#21 Posted by: chaka Posted at: 2017-11-26T18:25:26.217Z Reads: 68

```
I have run motors with a few broken windings early on in my eboarding addiction without getting faults. Check where the phase wires go into the motor to be sure they are not shorting out on each other from excessive rubbing or strain. Might have to disassemble the motor to get a good look at them
```

---
## \#22 Posted by: Jinra Posted at: 2017-11-27T06:29:03.963Z Reads: 53

```
I covered this kind of thing in a post as well

http://www.electric-skateboard.builders/t/ever-get-an-over-current-fault-check-your-motor-for-shorts/35286
```

---
