# VESC Not Powering Motors After Heavy Riding

### Replies: 27 Views: 3424

## \#1 Posted by: Jeff Posted at: 2015-12-11T20:09:34.693Z Reads: 131

```
Story:

After riding my board for 4 miles, I came across a large hill which I was able to power up effortlessly on my dual VESC 10S setup. However, after successfully getting up the hill, the board slowed down and would no longer let me transmit power to the motors.

Thinking the VESCs potentially overheated, I let the board cool down for a few hours to try it again. After connecting the power and applying throttle, I heard a slight noise from the motors which quickly died out. Now trying to apply throttle I hear nothing from the motors.

Inspecting VESC's further:


<img src="/uploads/db1493/original/2X/3/35e81f6d11cea5a2d2c4c6eeeb1709dc0b43bcab.jpg" width="690" height="388"><img src="/uploads/db1493/original/2X/a/a88d172303a73d4e0ca11c4fa873100de28057f6.jpg" width="281" height="500"><img src="/uploads/db1493/original/2X/4/4c554a57c7726a613af8ea01ff8b442543cf1632.jpg" width="281" height="500"><img src="/uploads/db1493/original/2X/f/f760658e65cfb70c58f6695d507efce6a7ed8776.jpg" width="281" height="500">

What I have tried:

- One of the motor wires seems to have fatigued so I repaired that.
- Using a multimeter, I confirmed that both the motor leads and motors are working properly.
- Reinstalled firmware and ensured BLDC settings are correct. Using GT2B I am able to confirm signals are being received by the VESC
- No fault codes in either VESC
- VESCs were connected via CAN-BUS, I have de-coupled and tried each one separately (still doesn't work).
 
I am no longer sure what to try.

Thank you all in advance for any help you can provide. Before the VESCs broke, I absolutely loved them! That makes having the board on the bench all the more difficult.
```

---
## \#2 Posted by: treenutter Posted at: 2015-12-11T20:16:32.787Z Reads: 125

```
Quick inspection, it looks like this motor wire broke:
<img src="/uploads/db1493/original/2X/5/5ea0b885eab978275cbadbe4e41134e69374d495.png" width="426" height="500">

and this lead to the battery looks like it cooked: 

<img src="/uploads/db1493/original/2X/d/d89cc21c89580aa71ab0830d369707ccb93b623a.png" width="690" height="402">

Are you using the same gauge wire for positive and negative on the battery wires? it looks like negative is a higher gauge. I would try replacing it either way.
```

---
## \#3 Posted by: NIK Posted at: 2015-12-11T20:35:51.140Z Reads: 122

```
Hi guys. What to do if my VESC did not receive any signal from the transmitter/receiver? and BLDC tool showing bad detection?
```

---
## \#4 Posted by: longhairedboy Posted at: 2015-12-11T20:59:12.354Z Reads: 121

```
youmentioned that you did fix the broken phase lead, but what about that power lead @treenutter mentioned? It does look pretty cooked. You may want to replace all your power leads with 10 gauge wire and then diagnose further.  

This sounds silly but it happens in cars all the time. Cant start your car, but for some reason the accessories are still able to light up the dash. Starter benches ok, solenoid clicks in ok, battery tests ok...Why? because the starter wires are burned up. They only carry enough juice to dim the lights and half ass start the starter, but not enough to turn over well enough to fire up the engine.
```

---
## \#5 Posted by: Jeff Posted at: 2015-12-11T21:18:50.134Z Reads: 120

```
Thanks for your replies.

Yes, I did already repair the broken motor wire. 

I may attempt to replace the power leads when I get some free time. I find it silly that the wire leads were such high gauge though that they could potentially burn up (came from the first Enertion 4.10 batch).

I think the motor wires could also be improved by using something with a greater number of strands to prevent fatigue failures after hundreds of miles of vibrations.
```

---
## \#6 Posted by: sl33py Posted at: 2015-12-11T21:45:10.928Z Reads: 116

```
good quality flexible wire will help, but i think you are trying to angle the motor wires too much.  That torque with the vibrations would be why the wire broke from fatigue.  You could also angle the soldered wire towards the wire path and not have so much solder wick up into the wire so it can remain flexible.

When you swap the broken wire and the burnt wire - does it work?  If not, what errors are you seeing in the BLDC tool?

Fingers crossed it's a simple fix like this!  GL!
```

---
## \#7 Posted by: Jeff Posted at: 2015-12-11T23:12:04.073Z Reads: 118

```
Just swapped out the wire in question. I don't think it was burnt out. The discoloration was probably just excess flux.

Powered on the VESC and still nothing. Here is the realtime plot when I blip the throttle:

<img src="/uploads/db1493/original/2X/6/6df1e5ca42d95efff0ea51612a3f1134eb115e85.png" width="690" height="334">


Could something inside the VESCs be burnt out?
```

---
## \#8 Posted by: sl33py Posted at: 2015-12-11T23:30:19.426Z Reads: 116

```
are you able to see any error codes display in the realtime data tab?
[img]/uploads/db1493/original/2X/2/292676db903bd8fa8e340444f3e0be878e40c825.jpg[/img]
See above, in the lower left there is a "Fault Code" DRV8302 error.

Also -  In the realtime graph area i was seeing a DRV error, then in the terminal
 tab i typed in "fault" and it would return a fault code.  I needed it 
to have failed/errored recently to see it return a code in the terminal, but that's how i confirmed the DRV chip was dead.
```

---
## \#9 Posted by: Jeff Posted at: 2015-12-11T23:42:18.523Z Reads: 108

```
Shoot I just packed up for the day. I will try and check tomorrow. Thanks for the tips!
```

---
## \#10 Posted by: Alex Posted at: 2015-12-12T02:22:55.972Z Reads: 107

```
I also have the same issue with my vesc. No faults listed in bldc for mine. I have replaced all wiring twice and still no luck. Luckily I have another vesc coming in the mail and I will be sending my current vesc back for further diagnosing
```

---
## \#11 Posted by: Jeff Posted at: 2015-12-12T21:03:32.485Z Reads: 105

```
I finally got it to show a fault codes using sl33py's method after a few seconds of throttle.

Here is the first VESC:
<img src="/uploads/db1493/original/2X/1/1fffca9de8b37484394ddd02fffdb141a771142f.png" width="690" height="402"> 

Here is the second (formerly slave) VESC:
<img src="/uploads/db1493/original/2X/d/dee59f52fea3e0364ab420a790367df3de4eeb7d.png" width="690" height="401">

Looks like they are both dead :frowning:
```

---
## \#12 Posted by: NIK Posted at: 2015-12-13T10:51:30.858Z Reads: 99

```
Hi guys, I have tried mine, both realtime data and the terminal doesn't show any error. Does this mean that my motor dead? but why when I push the throttle, the esc green light doesn't blink, it just stay. What to do next guys?<img src="/uploads/db1493/original/2X/2/2e6345b8cbd7809b4ab632b0d8044d00062fcb73.JPG" width="690" height="498"><img src="/uploads/db1493/original/2X/a/a3f571fa0c6348085e7d6a827cdc2346f57728a5.JPG" width="689" height="500">
```

---
## \#13 Posted by: NIK Posted at: 2015-12-13T15:16:27.738Z Reads: 93

```
After several test, yup, it shows fault code DRV8302. Therefore, I ordered DRV8302 from Texas Instrument and will try to change the IC based on Benjamin Vedder tutorial video.
```

---
## \#14 Posted by: NIK Posted at: 2015-12-13T21:05:20.782Z Reads: 95

```
Is it suppose to be shorted together?

<img src="/uploads/db1493/original/2X/e/e4ec03410833db0ad79d9de5a04a44d8aea5cb28.JPG" width="548" height="399">
```

---
## \#15 Posted by: elkick Posted at: 2015-12-13T21:23:12.938Z Reads: 94

```
That's normal, but could it be that your VESC is one out of the first batch (May/June) which had some problems?
```

---
## \#16 Posted by: chaka Posted at: 2015-12-13T21:25:35.943Z Reads: 95

```
Yes, those are fine. Is this a photo of your VESC?
```

---
## \#17 Posted by: NIK Posted at: 2015-12-13T21:54:10.285Z Reads: 98

```
I got the picture from one of the thread regarding vesc. Still, mine is the same as the picture. pin 54 & 53 and 51& 50 should be shorted together. 

@elkick chances are the problem comes from my careless arse which forgot to heat shrink the motor lead connection. 

@chaka so if I change the pic drv8302, I need to short both pin like in the picture? 

<img src="/uploads/db1493/original/2X/5/5f78bd156f56833d6d7945cb92e3d506b17c674f.JPG" width="303" height="500">
```

---
## \#18 Posted by: chaka Posted at: 2015-12-13T22:15:31.045Z Reads: 96

```
The pads under those pins are already connected so it isn't a big deal either way.
```

---
## \#19 Posted by: NIK Posted at: 2015-12-13T22:56:05.156Z Reads: 97

```
ah thats clear things up. Cheers
```

---
## \#20 Posted by: chaka Posted at: 2015-12-14T16:34:32.983Z Reads: 94

```
[quote="Jeff, post:5, topic:703"]
I may attempt to replace the power leads when I get some free time. I find it silly that the wire leads were such high gauge though that they could potentially burn up (came from the first Enertion 4.10 batch).
[/quote]

Looks like those cables are low strand count wire similar to what you would get at an automotive supply. You definitely want to switch those out for some high strand silicone wire. It is common for the insulation to melt on the low strand count wire due to a much larger amount of resistance too. 

Anyone installing one of these units would serve themselves well by replacing all cables.
```

---
## \#21 Posted by: Jeff Posted at: 2015-12-14T16:40:55.558Z Reads: 92

```
Agreed, I am waiting for a response from Enertion to see if the VESCs are covered under any sort of warranty. It is a hard pill to swallow when you spent $240 on speed controllers that lasted you two weeks....

If I could do it over again I would use high strand silicone coated wire, heat sinks, and lower the temperature cutoff range so I could be confident that the VESCs will run nicely for a very long time.
```

---
## \#22 Posted by: chaka Posted at: 2015-12-14T17:05:08.686Z Reads: 91

```
The VESC default temp settings are fine. I have been trying to burn one up with heavy use and have not had any success. I have even gone as far as intentionally overheating it repeatedly and haven't been able to produce a hardware failure.
```

---
## \#23 Posted by: Jeff Posted at: 2015-12-14T18:19:20.934Z Reads: 90

```
Good to know...I have no clue why they failed then
```

---
## \#24 Posted by: NIK Posted at: 2015-12-14T18:54:38.280Z Reads: 95

```
Just removed the DRV8302. Good surgery. Currently waiting for new PIC from TI. I will upload more infos and pics. <img src="/uploads/db1493/original/2X/e/e9a4208cf572124a70c2265ec63a833efd4b1e41.jpeg" width="500" height="500">
```

---
## \#25 Posted by: onloop Posted at: 2015-12-14T23:06:14.782Z Reads: 94

```
@nik please stop hijacking this thread if you have a problem create your own unique thread.

@longhairedboy @cmatson @psychotiller @torqueboards 
If you guys see this stuff happening please move the comments to a unique thread for each person. 

Jumbling all this into one thread creates a mess.
```

---
## \#26 Posted by: onloop Posted at: 2015-12-14T23:06:56.797Z Reads: 94

```
http://www.electric-skateboard.builders/t/vesc-faq-my-vesc-doesnt-work-help-qiqo/672
```

---
## \#27 Posted by: NIK Posted at: 2015-12-14T23:14:28.837Z Reads: 95

```
ouh sorry guys. cheers
```

---
