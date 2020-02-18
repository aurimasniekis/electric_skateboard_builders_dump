# Confusion about VESC version vs. Firmware Version vs. BLDC Version

### Replies: 15 Views: 4105

## \#1 Posted by: bill_f Posted at: 2016-07-09T03:19:40.039Z Reads: 355

```
Hi. Just got two new VESCs and want to get things right from the get go and at least fry the during a ride, not while sitting at my computer.
The VESC bag says VESC v4.12, so it seems pretty clear that the version of the VESC **hardware is 4.12**  On it, it also says the version of the **firmware is 4.18**. Check.

Just downloaded BLDC tool from [Jacob Bloy's site](http://vesc.net.au/download-now/) which shows **BLDC Tool as V2.17-2.18** 
____________________________
<img src="/uploads/db1493/original/2X/9/9626b263e5047e92adc8f1a0121f8075e75cac09.PNG" width="257" height="195">
_________________________________________

Opened up BLDC tool and on the firmware tab it shows it's compatible with firmware 2.17 2.18.
<img src="/uploads/db1493/original/2X/c/c5d9d6cc658b6d03877feb909fe55d414a7d838a.jpg" width="666" height="500">

Is there an error on the bag? or the BLDC info in the photo above?

Also saw this recent post [here](https://endless-sphere.com/forums/viewtopic.php?f=35&t=80877#p1191297) which adds to my confusion and makes me pause.<img src="/uploads/db1493/original/2X/1/1d04e16e9a0fe7071e606a7a34851dc6eb559111.PNG" width="690" height="131"> 

Anyhow, thanks for your thoughts and suggestions.
```

---
## \#2 Posted by: chipoi84 Posted at: 2016-07-09T03:25:40.449Z Reads: 330

```
That is a typo. Both np127 and the label on your diyElectricskateboard vesc meant 2.17/2.18 instead of 4.17/4.18. Also, there was a reported bug with Window version of bldc tool 2.18 a while back. I assumed everything has been fixed now.
```

---
## \#3 Posted by: torqueboards Posted at: 2016-07-09T03:37:14.004Z Reads: 321

```
@bill_f - Please check some recent videos we made for VESC as well as visit the other sites for more info if needed.

https://www.youtube.com/watch?v=dxDXUrk-7ek

I do recommend to configure and set your motor first as well as your battery cut off values.
```

---
## \#4 Posted by: bill_f Posted at: 2016-07-09T11:39:40.084Z Reads: 291

```
Okay, thanks for your input, @chipoi84 

@jacobbloy  Has the bug been fixed in the 2.18 WIN version that you currently have for download?  Seems like I remember reading about this too.  Thanks for your work with the VESC, btw.
```

---
## \#5 Posted by: bill_f Posted at: 2016-07-09T12:05:46.874Z Reads: 274

```
@torqueboards Yeah, I've been reading and watching everything I can find about the VESC over the last few months. Not easy as stuff is really fragmented even with the VESC FAQ stuff here. Seen Jacob's new vids also but it seems like there's always something vague or there's conflicting info that stops me in my tracks. That's part of DIY for sure. In your vid above, you mention firmware 4.18 as you do on your VESC packaging, which is confusing for someone like myself who's new to the VESC. Anyhow, I appreciate the recent VESC vid and hope you (and the community) make more explaining basic settings for beginners.   Question: do most people use an on/off switch like you show in the [video](https://www.youtube.com/watch?v=dxDXUrk-7ek)? On multirotors I just plug things in via XT connectors. Was just thinking of using an anti-spark XT90 as switch for my board, at least to start with.
```

---
## \#6 Posted by: torqueboards Posted at: 2016-07-09T18:33:12.495Z Reads: 252

```
@bill_f It's real simple... no brainer to configure VESC once you understand the concept. 

Hardware - meaning the PCB board and setup/parts is version v4.12
Firmware - meaning Software version, Firmware for the "code" - is v4.18.

Hardware doesn't change as often as Firmware does. But it's just the latest version of the code.

**In reality, just change the following.**
- battery cut off settings to your "battery setup" *REQUIRED*
- motor detection for your motor *REQUIRED*
- set your motor/regen amp requirements *Not required, but if you wanted to change it*
- Set on BLDC *Already set, double checking doesn't hurt.*
- Set PPM *Already set, double checking doesn't hurt.*

**For FOC,**
- Select the 3x Auto detect options
- Apply, Apply
- Set Motor to FOC
- Write configuration

Done deal...

As for on/off switch, you don't need an on/off switch. I just use it.

That image that you posted is now old news.. Jacob has fixed the Windows version long time ago. I use the Windows version as well.
```

---
## \#7 Posted by: Bender Posted at: 2016-07-10T01:08:01.545Z Reads: 217

```
[quote="torqueboards, post:6, topic:5797"]
Hardware - meaning the PCB board and setup/parts is version v4.12Firmware - meaning Software version, Firmware for the "code" - is v4.18.
[/quote]

Just to alleviate some confusion the latest firmware is 2.18 for hardware version 4.12

I think Dexter you just misread this, even in the video it says firmware version 2.18 (bottom right when you connect)

Otherwise great video!

I'd love to hear why you chose the values for the max/min motor and battery. I'm trying to set mine and would love a little more info
```

---
## \#8 Posted by: torqueboards Posted at: 2016-07-10T01:14:03.779Z Reads: 197

```
@Bender - Yeah, that's what I meant. :)

Hardware v4.12
Firmware v4.18

As for max/min motor and battery, depends on your setup. I was using 10S Lipo for the setup. Depends if your using single motor or dual motor. For a 18650 pack with 40A, you'd set each motor to 20A continuous. You'd set battery to 20Amp so it doesn't try and pull more than 20amps per motor which is your limit if you had a 40a fuse.
```

---
## \#9 Posted by: Blasto Posted at: 2016-07-10T01:21:17.914Z Reads: 185

```
[quote="torqueboards, post:8, topic:5797"]
Hardware v4.12Firmware v4.18
[/quote]

Haha again fw 2.18
```

---
## \#10 Posted by: torqueboards Posted at: 2016-07-10T01:22:56.620Z Reads: 180

```
oh doh! i see what your saying now LMFAO... :joy: FW v2.18! 2! 2!
```

---
## \#11 Posted by: Bender Posted at: 2016-07-10T01:26:13.659Z Reads: 178

```
I'm using 12s 40a battery on a single drive with your 6355 motor
I'd love to hear your setting suggestions :grin:
```

---
## \#12 Posted by: torqueboards Posted at: 2016-07-10T01:38:01.715Z Reads: 167

```
I think at 40amp for your motor settings you should be fine. I haven't tested it yet with VESC though so don't know just yet.
```

---
## \#13 Posted by: NNGG Posted at: 2016-07-10T23:12:56.649Z Reads: 154

```
can you link the newest firmware to use? i heard the newest one had some issues?
```

---
## \#14 Posted by: bill_f Posted at: 2016-07-12T13:51:27.102Z Reads: 149

```
As I understand it, this issue has been cleared up. Haven't tried it yet though. I believe you can choose the desired firmware from within the BLDC tool available from http://vesc.net.au/
```

---
## \#15 Posted by: PB1 Posted at: 2016-07-12T14:57:32.151Z Reads: 137

```
Oh great! 

Where can I get Firmware v4.18? Really advanced, years ahead of everything else. 

Suppose there are a lot of really cool features implemented now

:yum: :innocent:
```

---
