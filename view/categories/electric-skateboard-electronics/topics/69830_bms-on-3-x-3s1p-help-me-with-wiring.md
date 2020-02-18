# BMS on 3 x 3S1P - Help me with wiring

### Replies: 34 Views: 705

## \#1 Posted by: 00taffe Posted at: 2018-10-02T10:30:22.720Z Reads: 84

```
Hi everyone, 
I am building my first skateboard, before of start a new topic about my configuration, I would like to ask your help to connect correctly my BMS. 

I bought this model from Amazon to test on my skateboard > https://amzn.to/2IBT08F

This is the image from Amazon about the top of the BMS 
![_SL1001_|500x500](upload://zRri8fX4Gj0iFtNixfah3dFN4xL.jpeg) 

This is an image about the bottom. 
![IMG_7381|375x500](upload://hSC140Ju1Zb9WXqgSxKYrPax47d.jpeg) 

I have connected: 

- B- with the negative of the battery (black wire).
- C- with the negative of the charger port 
- P- will go to the negative port of the VESC 

I would like to connect the BMS and try to charge the batteries but I have some problems with the balance port. 

My setup has: 3 batteries (5000mAh 3S1P) in series, so I have 9 cells. 

Every battery has the balance port with this configuration:
- red wire last cell
- yellow wire middle cell
- white wire first cell 
- black wire the ground. 

Please, someone could help me to connect correctly my BMS? 
I am a bit confused about the balance port. 

Thank you very much for you help :slight_smile: 
This forum is amazing and I hope to share my skateboard soon :)
```

---
## \#2 Posted by: Andy87 Posted at: 2018-10-02T12:17:51.535Z Reads: 68

```
prinzipiell it´s always the same
like this just that you only have 3s
https://www.electric-skateboard.builders/t/connecting-a-bms-quick-guide-how-to/6122/59?u=andy87

hope you know that your bms can only handle 35a.
```

---
## \#3 Posted by: 00taffe Posted at: 2018-10-02T15:40:29.574Z Reads: 66

```
Thank you Andy. 
I have 9 cells in total and the BMS support max 10 cells. 

If I will connect in order the balance port for every battery to the BMS, I will have one port of the BMS empty. 

How should I do? 
Could this involve problems? 

Thank you very much :)
```

---
## \#4 Posted by: Andy87 Posted at: 2018-10-02T16:01:13.635Z Reads: 57

```
I never made it by my own but I read as long as you start from first port and only last balance port is free it should work.
Maybe @b264 can confirm if this is right or not.
I think he knows how to wire it up right.
```

---
## \#5 Posted by: b264 Posted at: 2018-10-02T18:52:54.376Z Reads: 53

```
The image from amazon above is totally 100% wrong and if you use it, you will burn something down.  Delete the image and never look at it again.

@00taffe Search the "Beautiful Diagrams" thread and you can post something here for verification.  The most positive balance lead is the one that needs to be left unhooked.
```

---
## \#6 Posted by: 00taffe Posted at: 2018-10-04T08:26:56.125Z Reads: 49

```
Thank you very much 🙏🏻
I saw the thread and every schemas. 

Based on the image of the bottom and on schema in the thread, i have to connect:

- B1 to the white wire of the first battery
- B2 to the yellow wire of the first battery
- B3 to the red wire of the first battery and so on
....
- B9 to the red wire of the third battery

I have to left unhooked the B10 or B1?
Where i have to connect B-? to the black wire of the first battery?
```

---
## \#7 Posted by: 00taffe Posted at: 2018-10-10T07:11:30.659Z Reads: 39

```
Hi guys, someone can help me?
Thank you :)
```

---
## \#8 Posted by: b264 Posted at: 2018-10-10T07:20:57.301Z Reads: 38

```
You should take photos of your batteries and your BMS because I'm not sure which wires are which.  Also you will need a multimeter to check the voltages
```

---
## \#9 Posted by: 00taffe Posted at: 2018-10-10T07:34:32.385Z Reads: 37

```
Sure, i am out from home now and i will upload all photos here asap. 
Thanks!
```

---
## \#10 Posted by: 00taffe Posted at: 2018-10-10T19:52:15.620Z Reads: 35

```
Hi, see the images below :slight_smile:

Tester 

- I put the black cable of tester to the - of the battery
![IMG_7695|375x500](upload://A6tWkqFFIkSudcYGPzLlFYyYfMY.jpeg)  

- Black to red wire 
![IMG_7692|375x500](upload://jUdFEdKMWubFsi7mJM4P7Jtg7x2.jpeg)

- Black to yellow wire
 ![IMG_7693|375x500](upload://2uZbOtYYAsX4zp2eeqTdLTan7ON.jpeg) 

- Black to white wire
![IMG_7694|375x500](upload://lIYSzTrpJgE2vTkEq3FMZfBHEHb.jpeg) 

and this is the image of the BMS 

![](https://www.electric-skateboard.builders/uploads/db1493/optimized/3X/7/d/7d515e9811170360afc07d481a3650c65ef1c2c7_1_375x500.jpeg)

Thank you for your help :blush:
```

---
## \#11 Posted by: b264 Posted at: 2018-10-10T20:27:05.388Z Reads: 33

```
[quote="00taffe, post:6, topic:69830"]
Based on the image of the bottom and on schema in the thread, i have to connect:

* B1 to the white wire of the first battery
* B2 to the yellow wire of the first battery
* B3 to the red wire of the first battery and so on
…
* B9 to the red wire of the third battery

I have to left unhooked the B10 or B1?
Where i have to connect B-? to the black wire of the first battery?
[/quote]

B- (B0) to the black wire of the first battery
B1 to the white wire of the first battery
B2 to the yellow wire of the first battery
B3 to the red wire of the first battery and the black wire of the second battery
B4 to the white wire of the second battery
B5 to the yellow wire of the second battery
B6 to the red wire of the second battery and the black wire of the third battery
B7 to the white wire of the third battery
B8 to the yellow wire of the third battery
B9 to the red wire of the third battery

NEVER solder the wires directly on the BMS.  Solder them to a connector that plugs into the BMS.  Only work on ONE wire at a time and finish and insulate it BEFORE you start working on another wire.
```

---
## \#12 Posted by: b264 Posted at: 2018-10-10T20:29:52.420Z Reads: 34

```
Also, a photo of the top of the BMS would help some too.  Some BMS need a bridge to use it in 9S mode when it's designed for 10S.  You may have to connect B9 to B10.  Not sure.  Try without first.
```

---
## \#13 Posted by: 00taffe Posted at: 2018-10-10T22:01:04.314Z Reads: 33

```
This is the image of the top ![](https://www.electric-skateboard.builders/uploads/db1493/original/3X/f/b/fb568e93992777abfbd938a3ea7befe74dcfdae5.jpeg) (but the connection aren’t correct) 

I tried the connections and apparently everything is working fine but in output through P- and the positive of the battery, the tension is 10v (more or less). Is this normal? 

The total tension of the battery is 33.3v

I tried to charge the batteries and the tension was increased of 0.4v and every battery are at the same tension after change (11.3v)

Thank you very much for your help ❤️
```

---
## \#14 Posted by: b264 Posted at: 2018-10-10T22:11:49.799Z Reads: 30

```
I meant a photograph of your actual BMS, not a stock photo.  It's important to see if there is a bridge of some sort.  That BMS PCB is desgined to be used for up to 16S but it's configured currently for 10S.  I don't know if they put a jumper somewhere between B10 and B16 (B+) to do that, or if they did not do that.  Some need it, some don't.

&ZeroWidthSpace;

&ZeroWidthSpace;

&ZeroWidthSpace;


Also, that is the image I was referring to
[quote="b264, post:5, topic:69830"]
The image from amazon above is totally 100% wrong and if you use it, you will burn something down. Delete the image and never look at it again.
[/quote]
Please heed.  You have to want to help yourself in order for someone else to be able to help ;-)

[quote="b264, post:5, topic:69830"]
Delete the image and never look at it again.
[/quote]
[quote="b264, post:5, topic:69830"]
Delete the image and never look at it again.
[/quote]
```

---
## \#15 Posted by: 00taffe Posted at: 2018-10-11T06:43:43.955Z Reads: 26

```
yes yes,  don't worry, the image isn't correct and I don't use it as a reference.
See the image below of the top :) 

![IMG_7707|375x500](upload://gDdqurZhFSorbM2Qz1SIXGSpwCq.jpeg) 
![IMG_7706|375x500](upload://qkYiIxJAWx5NCyOYuVSz3Ng8hwn.jpeg)
```

---
## \#16 Posted by: b264 Posted at: 2018-10-11T06:57:09.109Z Reads: 24

```
You don't need the jumper on this BMS, just leave B10 unhooked :smiley:
```

---
## \#17 Posted by: 00taffe Posted at: 2018-10-11T06:59:50.451Z Reads: 24

```
Fantastic!! 

So, in output from the BMS i have 10v (more or less), is this normal?
I measured with P- and the positive of the battery :)
```

---
## \#18 Posted by: b264 Posted at: 2018-10-11T07:06:19.714Z Reads: 23

```
It doesn't sound normal, no.  What is B- to B+
```

---
## \#19 Posted by: 00taffe Posted at: 2018-10-11T07:24:36.645Z Reads: 22

```
I have connected 
- B- to the negative of the batteries
- P- to the out (this will go to the VESC)
- C- to the charge connector 

This is the standard configuration that I found here
I have 10v between P- and the positive of the batteries.

Do you think that my BMS has any components burned?
```

---
## \#20 Posted by: b264 Posted at: 2018-10-11T07:42:58.127Z Reads: 20

```
It doesn’t sound normal, no. What is B- to B+
```

---
## \#21 Posted by: 00taffe Posted at: 2018-10-11T07:54:34.952Z Reads: 19

```
Sorry, can you explain? 
I don’t understand your message 😞
Sorry!
```

---
## \#22 Posted by: b264 Posted at: 2018-10-11T08:57:32.179Z Reads: 18

```
What is the voltage measured with a multimeter from the battery negative to the battery positive?  Not on the BMS, but on the battery itself.
```

---
## \#23 Posted by: 00taffe Posted at: 2018-10-11T09:15:22.188Z Reads: 19

```
Every battery has 11.3v and the total in serie is 33.8v between B- and B+
```

---
## \#24 Posted by: Andy87 Posted at: 2018-10-11T09:32:01.172Z Reads: 19

```
Can you make a picture how it’s wired up now?
```

---
## \#25 Posted by: 00taffe Posted at: 2018-10-11T10:48:22.384Z Reads: 19

```
Yes, sorry for the caos 😂

![image|666x500](upload://13yybFArbYbUO8RfOS9Cp90Q7Ae.jpeg) ![image|666x500](upload://yNoX5hv4PqIxd3CUvZV07RDw4Vs.jpeg) ![image|666x500](upload://jjLXHPSBf2Y89Su3W1KPdAF3bgC.jpeg) ![image|375x500](upload://dTp4x01KjYdqcujBMCL1y0koo7h.jpeg)
```

---
## \#26 Posted by: Andy87 Posted at: 2018-10-11T11:41:08.962Z Reads: 18

```
maybe i see it wrong, but did you bridge the black balance wire form pack one to pack two? if yes, why?
```

---
## \#27 Posted by: 00taffe Posted at: 2018-10-11T13:46:42.118Z Reads: 19

```
Based on the suggestion of @b264

https://www.electric-skateboard.builders/t/bms-on-3-x-3s1p-help-me-with-wiring/69830/11?u=00taffe 

With or without the bridge, the tension between P- and B+ is very very low :(
```

---
## \#28 Posted by: Andy87 Posted at: 2018-10-11T13:55:01.057Z Reads: 19

```
Ok i have overseen that.
Just didn’t understood, as in this diagram the - is only from the first pack connected 
![image|532x500](upload://xyJ9a1XK3N2je1VsddstcnjsXvD.jpeg) 

Seems i‘ll learn something today too 😅
```

---
## \#29 Posted by: 00taffe Posted at: 2018-10-11T14:50:13.103Z Reads: 17

```
Yes, in fact the tension with or without the bridge is the same in out from the BMS (between P- and B+).
The black wires on the balance port there are the same as on the negative pole (B-), are soldered on the same point.

But i don't know why the tension is too low :D
```

---
## \#30 Posted by: b264 Posted at: 2018-10-11T19:11:51.318Z Reads: 17

```
[quote="Andy87, post:26, topic:69830"]
bridge the black balance wire form pack one to pack two? if yes, why?
[/quote]

If the XT60 series connection are unhooked, then charging would still work.  This is the reason.  To separate the charging function from the discharging function.  If the XT60s are connected, it is the same.  This should charge correctly without any XT60 connected.
```

---
## \#31 Posted by: Andy87 Posted at: 2018-10-11T20:42:41.173Z Reads: 15

```
Just to get it right, if to unhook the xt60 I would only charge through the balance leads?
If yes, it would mean that if I have a 4a charger I would charge 4a through the leads instead of the 50-100mA which usually used for balancing.
```

---
## \#32 Posted by: b264 Posted at: 2018-10-11T21:07:49.547Z Reads: 14

```
I set them up to charge if the large wires are unhooked; yes.  Some folks might not.  I know a lot of folks don't.

A 22AWG wire should handle 4A just fine.  A 24AWG wire should handle 4A also but it's basically at maximum capacity.

I just like the charging and discharging to be separate functions and each one works independent of the other.  So, I don't rely on the discharge to be connected in order to charge.

The risk here is if one of your large series connections came loose on the road, the entire battery current would be going through a balance wire.  So there is a risk.  It depends if you've made your series connections robust and used cable-ties on the XT60.  To be safer, connect the black and red balance wires together through a 5A automotive fuse or leave them unhooked (meaning discharge must be connected to charge)
```

---
## \#33 Posted by: Andy87 Posted at: 2018-10-12T04:41:20.220Z Reads: 13

```
Thx for the explanation.
Now I understood why some people here don’t recommend 8 or higher amp charger.
Never thought about it. Always thought the balance wires just need to handle the balance current which is kind a tiny.
```

---
## \#34 Posted by: 00taffe Posted at: 2018-10-12T13:04:30.602Z Reads: 13

```
Hi guys,  my BMS was burned and this was the cause of low voltage in output. I tried with new BMS, like this, and everything is ok. The tension between P- and B + is: 33.7v the same of all batteries in series.

Thank you @b264 and @Andy87 for the support!
I am learning more and more things here and I can't wait to try the skate :D
```

---
