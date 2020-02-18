# (RESOLVED) VESC Help On NYE - Failed Motor Detection

### Replies: 34 Views: 3533

## \#1 Posted by: nmagz3 Posted at: 2016-12-30T22:57:33.459Z Reads: 233

```
Hey everyone!  To start off, if you're reading this thank you!  **I've outlined below my Failed Motor Detection scenerio and as much info as possible.  If you could help that would be such a blessing!**  I've really taken my time putting everything together, little by little.  I finally worked up the courage to plug in my 10s2p 5000 mah Lipo to a series connector to a 9mm bullet/XT90 adapter to my vesc () to my 6372 motor (enertion).  
<img src="/uploads/db1493/original/3X/b/0/b004e27c34210e09f1704882a09a9343bc6bdacd.jpg" width="690" height="404">

I was able to connect and flash my VESC and make sure I had the 2.18 firmware as recommended.  When I went to hit the detect motor button, I was like a little kid waiting for Santa, until nothing.  The motor moved like a centimeter and I was given a message that I had a Failed Motor Detection.  
<img src="/uploads/db1493/original/3X/2/9/2991e2db83a9ab64002b346a262831b6c8a05664.jpg" width="689" height="409">

Here is a pic of my read configuration:
<img src="/uploads/db1493/original/3X/e/4/e42fbf9e71472329b25e25df0fafde1781d2a68e.jpg" width="690" height="407">

**Steps taken after motor detection failed:**
•	Flashed VESC and installed firmware path C:/Program Files (x86)/BLDC Tool/Drivers/firmwares/hw_410_411_412/VESC_default.bin
•	Adjusted current and min erpm 
•	Decreased low duty down 0.1 
•	Lipo capacity was only 25% first try of motor detection.  Charge Lipos to 100% or 42 volts
•	Tired detecting on both PC and Mac
•	Tried several length mini usb wires

I tried these steps individually and in combination and still the same results.  I've also added a picture below of my VESC in case you all can see something in the VESC I cannot.  If you need me to take off the shrink warp let me know and I'll take new pics.  Anyhow, I know it's NYE and most likely I wont' get many responses but, I'd like you all to know their are some bright minds in here and honestly, building is our fun.  But, trust me I'd probably be out if my kid wasn't sick, LOL.  In any case, happy new year everyone!
<img src="/uploads/db1493/original/3X/6/f/6f35869dec12e5fdd88cf10c6345d1bf7ef17eb2.jpg" width="690" height="468"><img src="/uploads/db1493/original/3X/3/5/3534b8252dd70c5d78b3f95a938df132cc74fa70.jpg" width="666" height="500">
```

---
## \#2 Posted by: JohnnyMeduse Posted at: 2016-12-30T23:13:55.657Z Reads: 204

```
could you in the terminal and write down "fault"  after you retry a motor detection to see witch was the problem exactly ?

EDIT: faults I forget the s
```

---
## \#3 Posted by: nmagz3 Posted at: 2016-12-30T23:38:31.652Z Reads: 198

```
Awesome!  You're the first and only to reply :smile:  Could you elaborate on what you're saying?  I'm not sure what you mean: [quote="JohnnyMeduse, post:2, topic:15414"]
could you in the terminal and write down "fault"  after you retry a motor detection to see witch was the problem exactly ?
[/quote]

of if it's easier than explaining a screen shot of what you're trying to say would be so helpful. Thanks man!  You've definitly made it feel like I'm not stranded alone haha :sweat_smile:
```

---
## \#4 Posted by: Alextech Posted at: 2016-12-30T23:42:37.942Z Reads: 191

```
Oh your not alone! It just takes some of us a while to see the threads  :wink: 
Connect your VESC to your PC and connect to it. From there go to the terminal tab in the BLDC tool. Enter in fault on the bottom, tell us if anything comes in.
```

---
## \#5 Posted by: mmaner Posted at: 2016-12-30T23:43:19.796Z Reads: 187

```
In the BLDC tool, go to the terminal tab and type fault in command line field.  You should get a result, post that here and I'm sure someone will help.
```

---
## \#6 Posted by: cmatson Posted at: 2016-12-30T23:45:58.509Z Reads: 190

```
You can also go to the "real time data" tab, and click "active sampling" which is located at the bottom. It will show the faults in the bottom left.
```

---
## \#7 Posted by: nmagz3 Posted at: 2016-12-30T23:51:43.348Z Reads: 185

```
Awesome!  Thanks @Alextech @mmaner @cmatson & @JohnnyMeduse let me give your suggestions a try.  But, it will have to be in a bit as the wife is calling, LOL!  However, I appreciate your quick response.
```

---
## \#8 Posted by: nmagz3 Posted at: 2016-12-31T05:14:20.887Z Reads: 179

```
@JohnnyMeduse @Alextech @mmaner Thanks again guys!  After typing in fault in the terminal tab, like you all had mentioned, I come up with the response FAULT_CODE_NONE (image below).  Also, @cmatson after following your method of clicking the realtime data tab and activate sampling box the fault code shows NONE (image below).  I hope this makes sense to you all as this is now going over my head at this point.  Let me know if I can help narrow down the issue any more for you.<img src="/uploads/db1493/original/3X/a/2/a24ef0aa50977b1e02a3409832f16674abe5808c.jpg" width="690" height="406">
<img src="/uploads/db1493/original/3X/a/8/a8ae9e8fba4668f8e9050613aff890abf4c689f4.jpg" width="690" height="377">
```

---
## \#9 Posted by: nmagz3 Posted at: 2017-01-01T19:05:40.723Z Reads: 151

```
@JohnnyMeduse @Alextech @cmatson @mmaner hey guys happy new year!  Anyhow, uploaded my fault results as you all suggested.  Any ideas you can share?
```

---
## \#10 Posted by: Alextech Posted at: 2017-01-01T19:19:35.427Z Reads: 147

```
Well no fault codes!  That's a good start.  Those wavelength on the graph show that it is trying to send current to the motor.  Are the all the phase wires connected?
```

---
## \#11 Posted by: Ackmaniac Posted at: 2017-01-01T19:20:55.761Z Reads: 150

```
Is the remote application disabled. It looks like you have no remote connected at the moment but please set it to disabled and then try the motor detection again. Just to be sure.
```

---
## \#12 Posted by: JohnnyMeduse Posted at: 2017-01-01T19:34:51.304Z Reads: 146

```
Did you change the bullet connector for the motor lead ? If so can you remove the tape and take a picture, of your soldering. 

Also be sure to do a read before trying the motor detection.
```

---
## \#13 Posted by: nmagz3 Posted at: 2017-01-01T19:55:17.476Z Reads: 144

```
Thanks!  Glad to hear that's a good sign.  Yes, the phase wires are connected.
```

---
## \#14 Posted by: nmagz3 Posted at: 2017-01-01T19:58:08.604Z Reads: 140

```
Thanks for helping!  You're right I do not have a remote attached as of yet.  When you refer to the remote application are you talking about the App Configuration tab and the PPM tab?  It does say disabled and under the General tab it say No App.
```

---
## \#15 Posted by: nmagz3 Posted at: 2017-01-01T19:59:49.589Z Reads: 139

```
Hey Johnny thanks for the reply!  I did change the power leads from the Lipo.  The leads on the motor have not been changes since receiving it.  Are you suggesting I take of the shrink wrap from the motor leads to show you?
```

---
## \#16 Posted by: Alextech Posted at: 2017-01-01T20:11:20.642Z Reads: 138

```
Try to reflash your Vesc. Then afterwards, Put your Battery details, Then try the motor detection agian.
```

---
## \#17 Posted by: nmagz3 Posted at: 2017-01-01T20:18:09.342Z Reads: 139

```
Reflashed VESC with 2.18 firmware.  Next read configuration.  Start detection....same results.
```

---
## \#18 Posted by: nmagz3 Posted at: 2017-01-01T20:20:08.747Z Reads: 138

```
Because the VESC is connecting and when I click activate sampling there shows a graph.  Does that lead you all to believe that the VESC is in working condition?
```

---
## \#19 Posted by: JohnnyMeduse Posted at: 2017-01-01T20:42:38.356Z Reads: 138

```
does the red led flash when you try to run a motor detection ?
```

---
## \#20 Posted by: nmagz3 Posted at: 2017-01-01T20:43:38.787Z Reads: 136

```
It does!  When the power supply is attached the blue and green lights are lit.  When connected to the VESC and any action is made on the keyboard or trying motor detect the red light will blink.  Hope that helps.
```

---
## \#21 Posted by: JohnnyMeduse Posted at: 2017-01-01T20:52:23.192Z Reads: 132

```
ok, then try a motor detection and right after go on the terminal and write faults
```

---
## \#22 Posted by: nmagz3 Posted at: 2017-01-01T20:57:54.110Z Reads: 133

```
Ahh, there we go. Thanks Johnny!  What perspective can you give me based on the faults?

**Clicked Motor Config > Red Light Blinks > Bad Detection > Clicked Terminal Tab > then the following faults appear:**

The following faults were registered since start:

Fault            : FAULT_CODE_DRV8302
Current          : 0.1
Current filtered : 0.3
Voltage          : 38.09
Duty             : 0.02
RPM              : 5.5
Tacho            : 15
Cycles running   : 4
TIM duty         : 1019
TIM val samp     : 529
TIM current samp : 22245
TIM top          : 43433
Comm step        : 2
Temperature      : 29.23

Fault            : FAULT_CODE_DRV8302
Current          : 0.0
Current filtered : 0.3
Voltage          : 38.08
Duty             : 0.02
RPM              : 2.0
Tacho            : 16
Cycles running   : 3
TIM duty         : 991
TIM val samp     : 523
TIM current samp : 22415
TIM top          : 43784
Comm step        : 3
Temperature      : 29.28

Fault            : FAULT_CODE_DRV8302
Current          : 0.4
Current filtered : -1.0
Voltage          : 38.09
Duty             : 0.02
RPM              : 1.9
Tacho            : 17
Cycles running   : 4
TIM duty         : 991
TIM val samp     : 523
TIM current samp : 22415
TIM top          : 43784
Comm step        : 4
Temperature      : 29.36
```

---
## \#23 Posted by: Alextech Posted at: 2017-01-01T20:59:37.675Z Reads: 123

```
Oh no!  Definitely don't want to start the new year with a DRV failure.  You will need to get it replaced
```

---
## \#24 Posted by: nmagz3 Posted at: 2017-01-01T21:03:02.475Z Reads: 126

```
Damn, The DRV is located on the VESC correct?  I'd rather have the issue with the VESC then the motor.  Reason being is logistically Enertion is further then Tourqboards.  Also, I have a new VESC on the way from Miami Electric Boards.  ugh.  

How do DRV's normally fail?  And, can they come like that from the manufacturer?  **Thanks so much for your help @Alextech and @JohnnyMeduse !**  Do you think that's the only issue at this time or are their any other tests you can suggest?
```

---
## \#25 Posted by: JohnnyMeduse Posted at: 2017-01-01T21:11:47.013Z Reads: 124

```
Sorry to bring you the bad new... but there is no other test that we can do... the problem is a fry drv from the vesc. I can only suggest you to contact @torqueboards to see what option he can offer you.

Or you can use some repair services offer on this forum.
```

---
## \#26 Posted by: Alextech Posted at: 2017-01-01T21:11:54.920Z Reads: 123

```
Yes the DRV will the suspect.  Now DRV fail for many reason.  If the phase wires touch,  DRV failure,  incorrect firmware,  DRV failure, Bad Foc settings.  You guessed it DRV failure.  

The Vesc X is supposed to be much less susceptible to DRV failures just make sure your phase wires are 100% insulated and your settings are right and you should be okay.  Most DRV honestly are from user errors.
```

---
## \#27 Posted by: nmagz3 Posted at: 2017-01-01T21:13:37.034Z Reads: 120

```
Gotcha!  Honestly this is better news from where I was yesterday!  It kills me to keep an issue unsolved.  At least I know what it is and I can move forward.  What are some reasons a DRV would be fried?  Thanks again for your help brotha!
```

---
## \#28 Posted by: nmagz3 Posted at: 2017-01-01T21:16:13.458Z Reads: 114

```
Wow!  That's nuts :confounded: thanks for the insight and help!  I was honesty hoping for smooth sailing as soon as I got all my parts.  But then again, if that's what I really wanted I would have bought a complete set up right?!  I'll reach out to tourqeboards and see what my options are.
```

---
## \#29 Posted by: JohnnyMeduse Posted at: 2017-01-01T21:20:18.298Z Reads: 113

```
Also, from I can see in your picture you probably have one mosfet that is burn and act as a short (probably the root cause of your problem)

<img src="/uploads/db1493/original/3X/c/e/ce5663f3f2d32794a3c29a3171599b3c05171215.jpg" width="666" height="500">
```

---
## \#30 Posted by: lox897 Posted at: 2017-01-01T22:34:39.964Z Reads: 105

```
[quote="JohnnyMeduse, post:25, topic:15414"]
Or you can use some repair services offer on this forum.
[/quote]

*cough* *cough* @JohnnyMeduse
```

---
## \#31 Posted by: nmagz3 Posted at: 2017-01-02T02:24:50.200Z Reads: 100

```
@lox897 @JohnnyMeduse  Hahaha!  Yes, I'd much rather get it fixed the brick it.  I'll have to find out first if there's any warranty on it cause it's seriously been less than a week.  Appreciate the suggestion.  Johnny would my repair for the mosfet and DRV be in your wheelhouse?
```

---
## \#32 Posted by: JohnnyMeduse Posted at: 2017-01-02T05:00:52.256Z Reads: 95

```
No problem... after all I'm a "Vescpert" :wink:
```

---
## \#33 Posted by: Theshiatispimpin Posted at: 2017-02-13T19:49:12.899Z Reads: 81

```
Doing first build here had a question in general, not pertaining to this problem you had. Couldnt you use an anti spark from the vesc and not need a anti spark key? just use an anti spark xt90 female connected to male xt90/connector?
```

---
## \#34 Posted by: sl33py Posted at: 2017-02-13T21:28:29.711Z Reads: 81

```
depending on your wiring - yes.  If you have a Series adapter, or Parallel adapter - this is a good spot to use an XT90 anti-spark.  When you have multiple batteries - that's where it can get expensive if you swap each.  Plus a loop key that's accessible from the outside acts as a power switch when not riding vs unplugging your batteries fully.

It's definitely doable and preference.  I have some of both.
```

---
