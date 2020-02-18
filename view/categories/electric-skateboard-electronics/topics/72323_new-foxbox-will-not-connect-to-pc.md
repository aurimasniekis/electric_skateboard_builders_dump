# New Foxbox will not connect to pc

### Replies: 58 Views: 749

## \#1 Posted by: StefanMe Posted at: 2018-10-25T17:11:45.188Z Reads: 135

```
Hello guys! I got a new FocBox... my first one. I tried to connect to pc, but id doesn't show up on MAC oder WINDOWS. Do I have to do something special? My VESCs or Arduinos showing up normally.... 

Is there any trick? I connected it to my charger and the USB to pc (as I do it for my VESCs). the FB starts blinking red and then stay solid on blue (power). 

Any idea?
```

---
## \#2 Posted by: Trdolan03 Posted at: 2018-10-25T17:42:44.924Z Reads: 121

```
Try a different usb cable. The connectors are really finicky
```

---
## \#3 Posted by: StefanMe Posted at: 2018-10-25T18:06:03.085Z Reads: 120

```
I ll try... bot the VESC and the Arduinos work great. Without any issues.
```

---
## \#4 Posted by: Holyman92 Posted at: 2018-10-25T18:08:04.697Z Reads: 118

```
![image|690x388](upload://4DD3rnzOQsKbWBkB69GatcCjuZb.jpeg)
```

---
## \#5 Posted by: Saturn_Corp Posted at: 2018-10-25T18:08:10.978Z Reads: 116

```
Was about to suggest your USB cable might not be data capable but if you had no issues before on other devices this might not be the case.
```

---
## \#6 Posted by: barajabali Posted at: 2018-10-25T18:33:30.941Z Reads: 112

```
@StefanMe If this problem persists, contact support. 

Common reasons:
Broken usb port on focbox
Bad cable
Try a different computer
Ensure Focbox is powered on when plugging in
```

---
## \#7 Posted by: Andy87 Posted at: 2018-10-25T18:37:23.813Z Reads: 107

```
I read in one of the threads that @CarlCollins suggested to clean up the micro USB ports on the focbox. Sometimes they covered and the connection is not good because of that.
```

---
## \#8 Posted by: dareno Posted at: 2018-10-25T19:06:54.734Z Reads: 107

```
I had one like that and it turned out to be the usb.  Had a small piece of film stuck in there but I had to take it out of the casing to clean it.  Make sure that support are good with that warranty wise.  Sure they will be.
```

---
## \#9 Posted by: Acido Posted at: 2018-10-25T19:26:43.083Z Reads: 104

```
check your device menager
```

---
## \#10 Posted by: StefanMe Posted at: 2018-10-25T19:34:42.311Z Reads: 100

```
Running it on Mac. u don't need any device manager. A lot fo VESCs worked fine so far. 

I tried some different cables, different power supply, different pc. It just do nothing. it should also light up when just plug in the usb cable without power supply. Also doesn't light up. 

No combinations work. Whats next? Connect @EnertionSupport ?

I am really disappointed ... I needed this part. Now I have to wait for another month...
```

---
## \#11 Posted by: taz Posted at: 2018-10-25T19:35:32.593Z Reads: 96

```
Also the plug on some usb cables is too short and with the focbox case on cannot be inserted fully.
Try taking off the plastic case and make sure the plug is fully inserted.
```

---
## \#12 Posted by: Acido Posted at: 2018-10-25T19:38:47.841Z Reads: 91

```
go to your pc and open up the device manager 
vesc may show up there with a yellow triangle indicating some kind of an error

i had some trouble with mine until i installed some drivers and got it to work
```

---
## \#13 Posted by: StefanMe Posted at: 2018-10-25T19:40:19.719Z Reads: 87

```
Thanks,  it just doesn’t show up like not connected.

I already did this with cutting apart some of the plastic. Same result.
```

---
## \#14 Posted by: Acido Posted at: 2018-10-25T19:43:12.509Z Reads: 83

```
i think you just lost your warranty there....
```

---
## \#15 Posted by: StefanMe Posted at: 2018-10-25T20:03:47.520Z Reads: 74

```
I CUT THE CABLE! Not the FocBox of course!
```

---
## \#16 Posted by: CarlCollins Posted at: 2018-10-25T23:27:01.077Z Reads: 69

```
@StefanMe
I think I am able to help you, Can you please do the following?
remove your FOCBOX plastic casing and connect the MicroUSB cable.
And check if your MAC recognize it.

Also, I would love to help you via team viewer.
```

---
## \#17 Posted by: StefanMe Posted at: 2018-10-26T05:01:45.571Z Reads: 65

```
After removing the plastic housing, the pc is recognizing the FOCBOX. But the PC detects it as UNKNOWN DEVICE (WIN). I installed the latest BLDC Tool from your website... is there any driver i need?
```

---
## \#18 Posted by: CarlCollins Posted at: 2018-10-26T05:13:15.753Z Reads: 63

```
Here: for Windows Only: https://drive.google.com/file/d/1MS1AHeaHXwG0DQmIWHlHhhbm4MExJdw9/view?usp=sharing
```

---
## \#19 Posted by: StefanMe Posted at: 2018-10-26T05:41:06.822Z Reads: 64

```
I installed the driver,  But device is still UNKNOWN DEVICE...
```

---
## \#20 Posted by: CarlCollins Posted at: 2018-10-26T05:41:46.255Z Reads: 64

```
@StefanMe
Install team viewer on your Windows PC, Let me help you virtually
```

---
## \#21 Posted by: Andy87 Posted at: 2018-10-26T06:32:56.019Z Reads: 61

```
if you guys fix the problem, please let us know what it was.
Just for future cases, good to know what to suggest.
```

---
## \#22 Posted by: CarlCollins Posted at: 2018-10-26T06:33:30.020Z Reads: 61

```
@Andy87
I think it's damaged USB port
```

---
## \#23 Posted by: StefanMe Posted at: 2018-10-26T06:34:22.353Z Reads: 60

```
 Not damaged... the USB port is not placed correctly by the assambly...
```

---
## \#24 Posted by: Andy87 Posted at: 2018-10-26T06:35:09.429Z Reads: 60

```
USB port means on the PC?
just to get it right...
```

---
## \#25 Posted by: CarlCollins Posted at: 2018-10-26T06:35:42.471Z Reads: 60

```
@Andy87
On the FOCBOX (MicroUSB Port)
```

---
## \#26 Posted by: Andy87 Posted at: 2018-10-26T06:37:14.480Z Reads: 60

```
@CarlCollins thx for the info

@StefanMe would you mind to upload a picture how the port on the focbox look? it´s easy to see?
```

---
## \#27 Posted by: StefanMe Posted at: 2018-10-26T06:37:59.726Z Reads: 61

```
![image|666x500](upload://yRv2xd50babW56ohm1bE8trp2Zo.jpeg)

the left pin of the USB Port is loose and the right pin of the USB Port is is shiftet to the second right pad... all are shiftet one to the left
```

---
## \#28 Posted by: Andy87 Posted at: 2018-10-26T06:42:24.662Z Reads: 59

```
ok thx! hope you will get a replacement for it and soon get one working focbox ;)
```

---
## \#29 Posted by: StefanMe Posted at: 2018-10-26T06:43:12.433Z Reads: 59

```
and wait for another month... i need this part right know. That sucks, but can happen...

Funny that they placed an QC Passed Sticker on top while there is no (and never been) connection to the USB port. @EnertionSupport
```

---
## \#30 Posted by: Andy87 Posted at: 2018-10-26T06:48:51.042Z Reads: 59

```
:joy::joy::joy: so much about the QC....

can feel with you, wait already 4 month for APS motors which was promissed to be delivered during 6weeks...waiting sucks...especially if the winter is in front of the door...

but why you think it will take 4 weeks?
shipping should take not longer than 2
```

---
## \#31 Posted by: CarlCollins Posted at: 2018-10-26T06:49:08.389Z Reads: 58

```
@StefanMe
USB ports are soldered as they came on the FOCBOX, there are chances that they slightly get miss placed a little. This is a rare case and rest of the batch is clear and have no defects.
So it happens

Arranging a Replacement for him :slight_smile:
```

---
## \#32 Posted by: Schulerbible Posted at: 2018-10-26T06:57:28.995Z Reads: 55

```
What happens to those returned focboxes where the USB connector is faulty? I’ve successfully connected a detached USB to my old Vesc-x. I mean before you throw them away .....
```

---
## \#33 Posted by: StefanMe Posted at: 2018-10-26T06:58:57.512Z Reads: 55

```
haha no they will solder them new. But i dont want to do that. Its an expensive part and it should work out of the box.

Thanks, i ll get a replacement. Great fast support from @EnertionSupport
```

---
## \#34 Posted by: taz Posted at: 2018-10-26T08:46:38.023Z Reads: 53

```
Do you have another Focbox in your build?
If yes you could set this to slave and have access to it via canbus until they ship you the replacement.
Scratch that, I just read this is your first one.
```

---
## \#35 Posted by: StefanMe Posted at: 2018-10-26T08:58:35.947Z Reads: 54

```
I have to send the focbox before they send me the replacement.
```

---
## \#36 Posted by: StefanMe Posted at: 2018-12-10T08:04:55.972Z Reads: 44

```
Got a replacment from enertion... drove a few km... broken. I am done with enertion. I ordert a VESC6.6. Already wrote @EnertionSupport . See what they say... FocBox do not light up or anything. Wait another month for a replacment ^^

 https://metr.at/r/TRymT

Super strange temperature behaviour... FocBox got much to warm. (Outside temperature was around 10 C).
```

---
## \#37 Posted by: Andy87 Posted at: 2018-12-10T08:08:13.766Z Reads: 42

```
That sounds strange.
Can you post your settings here?
If the focbox become too hot it could be that your bat max values are too high.
Before you install any other esc make sure it’s not the motor or any of the connections which cause the controller to break.
```

---
## \#38 Posted by: taz Posted at: 2018-12-10T08:28:32.247Z Reads: 41

```
Some of the Focboxes were sent with the protective film still attached to the thermal conduction pad.
Could you check if yours is one of them?
```

---
## \#39 Posted by: StefanMe Posted at: 2018-12-10T08:30:42.596Z Reads: 41

```
40A battery 
60A motor
Nothing special... motor is nearly new 6374 from eskate.eu... motor windings look good. Is this too much for a single setup? Motor temp is fine... so u guess everything is ok from motor side.
```

---
## \#40 Posted by: Andy87 Posted at: 2018-12-10T08:38:35.834Z Reads: 40

```
I had same issue with the exactly same set up in single drive. Just it wasn’t a focbox it was a vesc 4.12 from Esk8.de 
In my case also motor got warm about 70-80degree. Unfortunately I couldn’t find out what was the issue.
If I see that right, it doesn’t take long till your focbox get hot and start to shut down.
In my case it took max 5min.

The focbox should handle the settings you set.
But just for testing did you try a lower current to look if it becomes less?
Maybe to set the motor max to 50
and the bat Max to 35 and try if it will be better
```

---
## \#41 Posted by: taz Posted at: 2018-12-10T08:56:09.654Z Reads: 41

```
This is definitely not normal. The currents you draw should not heat up the esc in such a short time.
I would check the thermal pad first and go from there.
Is there a chance you have increased the FOC frequency too much?
```

---
## \#42 Posted by: StefanMe Posted at: 2018-12-10T09:00:55.298Z Reads: 41

```
I used just basic settings on FOC. Did not change there anything at all. Just did the motor detection and took a ride. 

I opend the FocBox now... looks super strange inside.

![image|280x500](upload://n56Dg16lpwh8L9LmjUXmVBZ9YTL.jpeg) ![image|375x500](upload://5N56nhKUcuXC2T7vQdsfhvloZ67.jpeg) ![image|375x500](upload://ciCuuBBYLaotnpXCV71PB7BW4LH.jpeg) 

@Andy87 i cannot try anything... the vesc doenst boot up anymore.
```

---
## \#43 Posted by: taz Posted at: 2018-12-10T09:01:48.259Z Reads: 38

```
[quote="StefanMe, post:42, topic:72323"]
I opend the FocBox now… looks super strange inside.
[/quote]
What do you mean? Can you take a photo?
```

---
## \#44 Posted by: StefanMe Posted at: 2018-12-10T09:03:51.587Z Reads: 40

```
Sorry, just give me a second.... upload pics from my phone...

It looks "wet" on the thermal pad... only on the pad. Everything around is super dry, also in my board its super dry! This is no fluid from outside!
```

---
## \#45 Posted by: Andy87 Posted at: 2018-12-10T09:08:16.026Z Reads: 40

```
i need to check other pictures, but i know that there need or can be some solder bridges on the drv legs.
```

---
## \#46 Posted by: taz Posted at: 2018-12-10T09:09:19.933Z Reads: 40

```
Could it be the clear plastic film that melted?
```

---
## \#47 Posted by: Andy87 Posted at: 2018-12-10T09:10:16.409Z Reads: 42

```
Seems right with the bridges 
https://www.electric-skateboard.builders/t/vesc-drv8032-problems-new-soldered/49082/4?u=andy87
```

---
## \#48 Posted by: taz Posted at: 2018-12-10T09:17:37.018Z Reads: 42

```
Here is a thread showing the film.
https://www.electric-skateboard.builders/t/focbox-factory-mishap/50891/62
```

---
## \#49 Posted by: StefanMe Posted at: 2018-12-10T09:25:53.467Z Reads: 43

```
Thanks... i ll check later. Anyway... the focbox is already broken.
```

---
## \#50 Posted by: Andy87 Posted at: 2018-12-10T09:31:33.415Z Reads: 44

```
@Martinsp does a repair job, just in case that would be an option for you.

http://electricskateboard.repair/index.php?id_category=19&controller=category
before you through the focbox to the trash... i´m ready to take the one :stuck_out_tongue_winking_eye:
```

---
## \#51 Posted by: StefanMe Posted at: 2018-12-10T09:35:24.269Z Reads: 42

```
Haha no, I have an instant replacement warranty by enertion. I ll get a new one ^^ then I maybe use it as a coffee cup warmer 😛
```

---
## \#52 Posted by: Andy87 Posted at: 2018-12-10T09:36:22.607Z Reads: 41

```
good to hear!
still... in case... you know i´m here.... just let me know :joy:
```

---
## \#53 Posted by: dareno Posted at: 2018-12-10T09:38:03.553Z Reads: 41

```
&lrm;Slut.
```

---
## \#54 Posted by: Andy87 Posted at: 2018-12-10T09:38:38.321Z Reads: 42

```
:kissing_heart::kissing_heart::kissing_heart:
:joy:
```

---
## \#55 Posted by: dareno Posted at: 2018-12-10T09:39:11.805Z Reads: 42

```
I feel dirty.
```

---
## \#56 Posted by: StefanMe Posted at: 2018-12-10T09:44:48.952Z Reads: 41

```
Eskate is getting dirty 😂
```

---
## \#57 Posted by: StefanMe Posted at: 2018-12-11T19:34:34.908Z Reads: 33

```
From exertion support:

    If you already got one replacement, then there is something seriously wrong with your setup
    I would like to know your BLDC tool Values and setup specs before getting your faulty FOCBOXes back and sending new ones

They mean the FoxBox they replaced the first time, where they screwed up the to solder the USB port correctly. Looks like that was also my fault :rofl:

https://www.electric-skateboard.builders/t/new-foxbox-will-not-connect-to-pc/72323/27?u=stefanme
```

---
## \#58 Posted by: CarlCollins Posted at: 2018-12-11T20:57:39.951Z Reads: 30

```
@StefanMe
Thank you so much for sharing this :stuck_out_tongue:

Let me elaborate something, 
We don't want you to suffer again to get a replacement
Just trying to be sure that it's not the issue with the FOCBOX

I already offered you to ship a new FOCBOX within this week.
Just want those faulty ones to nearest RA for inspection to assist you better
 
I hope now it's clear :slight_smile:
```

---
