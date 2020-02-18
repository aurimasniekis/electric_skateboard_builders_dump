# Motor Detection Failed, not sure why

### Replies: 26 Views: 1464

## \#1 Posted by: Enzon Posted at: 2017-10-11T20:19:34.906Z Reads: 115

```
Hello all,
I recently made a post about purchasing a new motor after my old one stopped detecting.  I had been using the old motor for around a month when it suddenly stopped working during a ride.  When I brought the board back to my apartment to see what was wrong, every time I tried detecting the motor, it failed.  Right before it would tell me it failed, the vesc would emit a green light but no red one.  When I checked both the terminal and realtime data tabs for faults, both say that no faults have been detected since startup.  I purchased a new motor and the same thing seems to be happening.  I've seen people with similar problems where the motor slowly jerks, but my motor doesn't move at all.  I'm not sure what to think since the vesc shows no faults but neither motor will work with it.  I suppose it could have something to do with the motor phase wires not being soldered properly, but this also doesn't seem too likely since the first motor worked for 20+ rides before suddenly failing.  If anyone has any insight, I'd love to hear it.  Thanks guys!

Edit:  Additionally, when I look at the PPM tab, the bar moves when the remote is pressed, and when I turn the motor with my hand, current fluctuates to about 4 amps when I look in realtime data.
```

---
## \#2 Posted by: MysticalDork Posted at: 2017-10-11T20:34:38.557Z Reads: 110

```
How much resistance does the motor give when you turn it? Does it spin freely, or does it feel like it's fighting you?
```

---
## \#3 Posted by: GrecoMan Posted at: 2017-10-11T20:39:33.724Z Reads: 108

```
Didn’t even read the essay you wrote but I’m gonna give you my advice:  

LOOSEN MOTOR MOUNT SCREWS
```

---
## \#4 Posted by: Enzon Posted at: 2017-10-11T20:41:11.677Z Reads: 99

```
@MysticalDork The motor doesn't appear to be any more difficult to turn than the motor that I do not have connected to anything. 

@GrecoMan I currently don't even have the motor attached to the mount yet since it won't spin up anyways.
```

---
## \#5 Posted by: GrecoMan Posted at: 2017-10-11T20:42:28.788Z Reads: 92

```
Can you give us a video of what happens when you try to do motor detection?
```

---
## \#6 Posted by: JohnnyMeduse Posted at: 2017-10-11T21:26:05.959Z Reads: 90

```
Can you post your setting and some picture of your setup... It might be something as simple as a wrong setting, or as complicated as a Burn DRV
```

---
## \#7 Posted by: JohnnyMeduse Posted at: 2017-10-11T21:27:24.636Z Reads: 90

```
Also can you give is more detail abouth your setup... VESC vendor, motor type, sensor/unsensor, ..,
```

---
## \#8 Posted by: Enzon Posted at: 2017-10-11T22:25:42.595Z Reads: 89

```
@GrecoMan here is a video that shows my set up and what's happening. Sorry that it's not the best quality and try ignoring that my current workspace is my bed lol. 
https://vimeo.com/237823161
```

---
## \#9 Posted by: Enzon Posted at: 2017-10-11T22:30:00.935Z Reads: 86

```
@JohnnyMeduse I purchased my vesc from diyelectric skateboard, I'm using 2 5s 8,000 mAh LiPos in series, and my original motor is a 6374 192kv sk3 but the one I currently have hooked up is a 245kv tacon bigfoot, both sensorless.  I have bat max at 57v, min at 8v, and the cutoffs at 11v and 6v just to ensure they shouldn't be an issue.  For current, motor max is 40A, min -40A, batt max 25A, bat min -12A, and absolute max at 130A.  I'm using PPM and like I said that seems to be working fine since the bar moves when I use the controller.  I've also tried motor detection ranging from 6-10 amps and none have worked.  If you need any more info, let me know.
```

---
## \#10 Posted by: JohnnyMeduse Posted at: 2017-10-11T22:40:51.505Z Reads: 83

```
Send some screen shoot specially of the advance and bldc tabs it's much more easier to find out any flaws... I can't really tell from a enumeration
```

---
## \#11 Posted by: Enzon Posted at: 2017-10-11T22:51:39.345Z Reads: 78

```
@JohnnyMeduse<img src="/uploads/db1493/original/3X/a/a/aac764eed7bf6b2c3420152762fb85bdbe573d20.png" width="690" height="359"><img src="/uploads/db1493/original/3X/4/c/4c6e31df282e36cdcac71ef7e39f613a9d9d6e2c.png" width="690" height="359"><img src="/uploads/db1493/original/3X/0/8/08fd57a79e1838976547d4f374e62e1be30d5dc5.png" width="690" height="359"><img src="/uploads/db1493/original/3X/c/4/c4b6ff1a2a14cdbeb8efa5f8566360916dd601b0.png" width="690" height="388"><img src="/uploads/db1493/original/3X/d/a/dab47fbd4913af863fdd6b82fe1f688cabd409b9.png" width="690" height="359">
```

---
## \#12 Posted by: JohnnyMeduse Posted at: 2017-10-11T23:40:04.916Z Reads: 67

```
Try to disable the ppm signal, before running a new motor detection
```

---
## \#13 Posted by: Gynpe Posted at: 2017-10-12T00:41:39.539Z Reads: 66

```
Are you using the same cable as before? I ask because this happened to me, until I realizad it was a USB charge cable and not a USB data cable.
```

---
## \#14 Posted by: Enzon Posted at: 2017-10-12T01:01:48.497Z Reads: 67

```
I'm 95% sure it's the same cable, but I don't think I have any other cables to test it with.  Also, the PPM signal was originally disabled when I first read the conifguration on the new motor and it was still failing motor detection.
```

---
## \#15 Posted by: Enzon Posted at: 2017-10-13T16:31:08.105Z Reads: 61

```
Anybody else have any ideas? If not, I'll probably just have to bite the bullet and pick up a new vesc.
```

---
## \#16 Posted by: JohnnyMeduse Posted at: 2017-10-13T16:40:14.707Z Reads: 62

```
[quote="Enzon, post:1, topic:35333"]
the vesc would emit a green light but no red one.
[/quote]

With this kind of behaviour (and I why I wanted to see your parameter)the first thing you have to look for Is if the sensor option is check, which in your case wasn't and that right thing to have. But one thing I do see in your parameter, Is you have all the default motor setting, which make me believe that the motor detection wasn't properly write inside the vesc setting at first and that could lead to a broken DRV.

Next question is does the red light flash when you power up the VESC ?

Regards
JF
```

---
## \#17 Posted by: chaka Posted at: 2017-10-13T16:44:40.536Z Reads: 59

```
Might have some poor solder joints on the gate resistors.
```

---
## \#18 Posted by: JohnnyMeduse Posted at: 2017-10-13T16:48:48.305Z Reads: 58

```
Yeah might be... but if the Red led doesn't show up at the start the DRV is most likely to be fry and it isn't able to properly communicate with the MCU. That a unlikely scenario, but it's the easiest to check at first :wink:
```

---
## \#19 Posted by: Enzon Posted at: 2017-10-13T16:52:20.528Z Reads: 59

```
@JohnnyMeduse I had read the settings in the past and they were always the ones I set, but now I can't remember what I had them set to. Could they be the defaults now because it is no longer detecting a motor or would they not change?  A red light does not flash when I turn the vesc on, only when I power it off, which I assume is normal behavior.

@chaka would that have allowed my motor to detect fine when I first put the board together? It just seems odd that a problem would only arise now, but obviously you guys are much more familiar with the hardware than me lol
```

---
## \#20 Posted by: chaka Posted at: 2017-10-13T16:53:21.846Z Reads: 56

```
He is getting feedback when moving the motor by hand so the drv is probably fine. I bet the problem lies somewhere between the drv and the gate pins. Still, hard to say without having it in hand.
```

---
## \#21 Posted by: chaka Posted at: 2017-10-13T16:56:16.039Z Reads: 54

```
> @chaka would that have allowed my motor to detect fine when I first put the board together? It just seems odd that a problem would only arise now, but obviously you guys are much more familiar with the hardware than me lol

I didn't catch that part...

No blinking light on startup... could be a number of things. Might try re-flashing the firmware with the bootloader.
```

---
## \#22 Posted by: JohnnyMeduse Posted at: 2017-10-13T16:59:01.222Z Reads: 56

```
[quote="chaka, post:21, topic:35333"]
No blinking light on startup... could be a number of things
[/quote]

Well it's most likely to be a burn down DRV, since those setting are the one by default

<img src="/uploads/db1493/original/3X/f/6/f60eadbaf736231de204d0bc85e4bf006158bdef.png" width="690" height="359">

And yes the Vesc could have work for a bit with those in place, but overtime they will most likely burn your DRV.
```

---
## \#23 Posted by: cloudy Posted at: 2017-10-16T05:54:44.300Z Reads: 49

```
The drv recently burned on my Ollin ESC, which I sent in to @chaka, he has not replied to any of my emails. Are they usually hard to repair?
```

---
## \#24 Posted by: chaka Posted at: 2017-10-16T13:26:24.489Z Reads: 48

```
We don't see any recent emails regarding a repair. Try sending your email to jclark@ollinboardcompany.com

If you can give me your order number here I can look it up for you.
```

---
## \#25 Posted by: cloudy Posted at: 2017-10-16T14:04:25.035Z Reads: 46

```
The package arrived with attention to warranty last Thursday to the repair po box. My name is on the from field.

I guess I was emailing an old email address, even when I sent emails through the support box on the website I never received confirmation (week ago).

I would pm you order # but I don't think I can yet as my account is new. Don't think posting it here is best idea.I did forward you the email chain as well as ny order # though.


Thanks,
```

---
## \#26 Posted by: chaka Posted at: 2017-10-16T14:22:02.543Z Reads: 42

```
Thank you, Melissa is on it now. In the future, feel free to send a follow up email. Melissa is pretty good at keeping up with emails but she is spending more time helping out in the shop these days.

Welcome to the community!
```

---
