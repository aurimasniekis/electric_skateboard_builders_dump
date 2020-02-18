# Motor detection failed (Stutters) focbox

### Replies: 38 Views: 1324

## \#1 Posted by: Bjork3n Posted at: 2018-04-20T09:14:02.521Z Reads: 143

```
Hey guys!
So today i was about to install my new Focboxes. 
I have an issue during the motor detection.

Motor spins up well in start of the detection but in the end of the detection it studders as crazy and detection fails.
No faults in terminal.
I can use the keyboard to control motor and that works perfectly.

Just wondering could this be due to a bad solder connection? Or is it something else im missing?
My other standard vesc 4.12 has no issue detecting with the same settings.

Appreciate the help.

https://youtu.be/Mgo335BVjHY
```

---
## \#2 Posted by: CarlCollins Posted at: 2018-04-20T09:44:11.181Z Reads: 142

```
@Bjork3n

Can you please share your  Motor detection tab settings and also it would be great if you record a video during detections?
Also tell us about your setup and are you using FOC or BLDC?
```

---
## \#3 Posted by: Bjork3n Posted at: 2018-04-20T10:29:18.598Z Reads: 136

```
Hey Carl.
Sure here is a video that shows what happening during detection.
https://youtu.be/iCYdQNtBwRM


My setup
Dual 6355 190kv motors
Battery 10s4p samsung 30Q cells

This is when setting up in bldc.
No fault codes in terminal after failed detection.
```

---
## \#4 Posted by: CarlCollins Posted at: 2018-04-20T10:40:56.715Z Reads: 126

```
Sorry man but screen is not clear and fully visible
Try recording another video
```

---
## \#5 Posted by: Bjork3n Posted at: 2018-04-20T10:48:12.092Z Reads: 121

```
Video is only to show the problem, im uploading photos of settings now! :)
```

---
## \#6 Posted by: Bjork3n Posted at: 2018-04-20T10:50:45.985Z Reads: 123

```
![Vesc general|690x388](upload://s6su0EWIDGeKjHVssdXnJqbvdeU.png)![vesc RPM|690x388](upload://yVT0zcNenVJpapZdQOSYUkh1ETH.png)![Vesc voltage|690x388](upload://34oW42IJVCNAz2OzOzvU1BXWG98.png)![Vesc current|690x388](upload://quTWdPUGePBdS2AHXMAyLml2kxW.png)![vesc advanced|690x388](upload://daBXkF2y1OB0CWbIl5hZSBBxR28.png)

@CarlCollins
```

---
## \#7 Posted by: CarlCollins Posted at: 2018-04-20T10:50:59.820Z Reads: 112

```
Please share because that sound came when we do detection in FOC mode
```

---
## \#8 Posted by: Bjork3n Posted at: 2018-04-20T10:52:07.984Z Reads: 115

```
Well im only using BLDC to be on the safe side.
```

---
## \#9 Posted by: CarlCollins Posted at: 2018-04-20T10:53:49.196Z Reads: 116

```
@Bjork3n

Your maximum input voltage is high, it must be below 50.4V I think,
Try lowering it and adjust the minimum and maximum accordingly and try performing a detection again
```

---
## \#10 Posted by: Bjork3n Posted at: 2018-04-20T10:56:06.292Z Reads: 117

```
Same issue with voltage 50.4.

It seems like its only the last part of the detection that fails. 
Spins up fine first then slows down and stutters.
```

---
## \#11 Posted by: CarlCollins Posted at: 2018-04-20T10:56:57.748Z Reads: 115

```
What firmware you are on the FOCBOX?
```

---
## \#12 Posted by: Bjork3n Posted at: 2018-04-20T10:58:00.088Z Reads: 115

```
Im using Ackmaniac FW 3.100 
Saw you recommended that in another thread.
```

---
## \#13 Posted by: CarlCollins Posted at: 2018-04-20T11:01:05.116Z Reads: 117

```
lower the batt max must be 30A 
And Batt Min 15A

Batt Max is high for 10s system
```

---
## \#14 Posted by: Bjork3n Posted at: 2018-04-20T11:03:45.003Z Reads: 116

```
I use 30A max on battery A.
And Battery min at -8A so i dont overcharge the cells on braking

But honestly those values shouldn't affect the motor detection? 
No problem with detection motors with my maytech vesc,
```

---
## \#15 Posted by: CarlCollins Posted at: 2018-04-20T11:05:19.074Z Reads: 116

```
What lights you got when you do the detection on FOCBOX?
```

---
## \#16 Posted by: Bjork3n Posted at: 2018-04-20T11:06:26.051Z Reads: 118

```
No lights and no fault in terminal tab after detection.
Just says Bad detection in the corner of the vesc tool.
```

---
## \#17 Posted by: CarlCollins Posted at: 2018-04-20T11:09:04.420Z Reads: 121

```
There isn't any light lit on the FOCBOX?
```

---
## \#18 Posted by: Bjork3n Posted at: 2018-04-20T11:11:07.225Z Reads: 126

```
There are lights but they dont change while doing motor detection.
Power light is on.
```

---
## \#19 Posted by: CarlCollins Posted at: 2018-04-20T11:14:19.787Z Reads: 128

```
@barajabali please have a look to this one.
@Bjork3n If you purchased it from us then try downgrading the firmware and perform detections using Enertion's BLDC tool.
```

---
## \#20 Posted by: Bjork3n Posted at: 2018-04-20T11:34:54.833Z Reads: 127

```
Im uploading a video now to show the issue.
```

---
## \#21 Posted by: Bjork3n Posted at: 2018-04-20T11:42:51.311Z Reads: 120

```
https://youtu.be/Mgo335BVjHY

I also tried with the stock vesctool firmware. Same issue.

Oh and using the arrow keys on the keyboard to control motor works perfectly!

I have 2 focboxes and both has same issue and fails on motor detection.
```

---
## \#22 Posted by: CarlCollins Posted at: 2018-04-20T11:49:00.595Z Reads: 120

```
@Bjork3n

Are you using Ackmaniac FW and VESC tool?

Can you please try using Enertion's FW and BLDC tool?
```

---
## \#23 Posted by: Bjork3n Posted at: 2018-04-20T11:53:43.880Z Reads: 118

```
I tried the vesctool 3.37 FW and it was the same issue.
I doubt its a FW issue?
```

---
## \#24 Posted by: CarlCollins Posted at: 2018-04-20T11:54:43.744Z Reads: 119

```
@Bjork3n

I guess so, That's why advised you to downgrade the FW to 2.18 and use Enertion's BLDC tool.
```

---
## \#25 Posted by: Bjork3n Posted at: 2018-04-20T11:59:09.625Z Reads: 117

```
There are plenty people here running vesctool/ack fw on focbox with no issue. 
But sure i can try downgrade and let you know if its any diffrence.

Ok one box is now ok when i raised the duty on detection to 0.1
Other box shows the same issue even when i raise the duty to 0.1
```

---
## \#26 Posted by: rpasichnyk Posted at: 2018-04-20T12:06:13.046Z Reads: 113

```
I had this issue as well. Try to increase duty cycle (D:) from 0,05 to 0,20.
```

---
## \#27 Posted by: Bjork3n Posted at: 2018-04-20T12:10:58.671Z Reads: 114

```
its so violent when rasing the duty... feels unsafe? no?
```

---
## \#28 Posted by: rpasichnyk Posted at: 2018-04-20T12:24:22.251Z Reads: 113

```
You want to complete motor detection or no? Sometimes you need to be violent and punish dat focbox. It's raising duty time! Wear helmet for safety :+1:
```

---
## \#29 Posted by: Bjork3n Posted at: 2018-04-20T12:25:13.230Z Reads: 110

```
Ofcourse i do but i dont want any POOFING this time ;)
```

---
## \#30 Posted by: CarlCollins Posted at: 2018-04-20T12:26:23.586Z Reads: 108

```
Found this on the forum: http://www.electric-skateboard.builders/t/tutorial-how-to-solve-focbox-bad-detection/52806
```

---
## \#31 Posted by: Bjork3n Posted at: 2018-04-20T12:38:42.321Z Reads: 106

```
I tried up to 0.12 but im afraid going higher since it becomes more violent as i increase the duty.
Looking for some more input before i decide to go higher, i would be sad to blow a focbox before even testing it out :confused:
```

---
## \#32 Posted by: Bjork3n Posted at: 2018-04-20T12:54:19.775Z Reads: 106

```
you wont belive me when i tell you the issue... 
I used a too long usb cable.
Now it works
```

---
## \#33 Posted by: CarlCollins Posted at: 2018-04-20T13:00:57.296Z Reads: 103

```
@Bjork3n

Oh I forgot about the USB voltage drop. 
Glad you solved it. 
Always use standard size USB cable or long USB cable with USB adapter or hub.

It's due to voltage drop
```

---
## \#34 Posted by: Bjork3n Posted at: 2018-04-20T13:56:56.462Z Reads: 96

```
What's the perfect length? :slight_smile:
```

---
## \#35 Posted by: CarlCollins Posted at: 2018-04-20T14:00:14.196Z Reads: 94

```
Standard size is 1.5 m approx
Maximum length of the cable : 5 meters (with HI speed USB port 2.0)
```

---
## \#36 Posted by: Bjork3n Posted at: 2018-04-20T14:22:44.277Z Reads: 90

```
Ok I used 3M cable first. 
I still had to raise the duty to 0.1 to get a complete detection. 
Rode to work 6km and everything worked great!
```

---
## \#37 Posted by: Silverline Posted at: 2018-04-20T15:30:43.548Z Reads: 86

```
I all so have this problems with focbox.... i just increase the test Amp and Rpm`s.... and then it detects fine...
```

---
## \#38 Posted by: Gjf1 Posted at: 2018-12-16T04:11:03.643Z Reads: 45

```
This worked for me thanks!
```

---
