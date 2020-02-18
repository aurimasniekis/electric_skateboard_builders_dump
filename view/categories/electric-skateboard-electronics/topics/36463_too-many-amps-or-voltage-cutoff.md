# Too Many Amps or voltage cutoff?

### Replies: 25 Views: 2308

## \#1 Posted by: TeslaAlex Posted at: 2017-10-25T10:49:25.899Z Reads: 236

```
Hi!

I spent this summer to build an electric longboard and it works good, most of the time. The only problem is that my motor draws too many amps when going uphill and exceeds the max amp rating on my ESC. Since my ESC "safety feature" for this is stopping immediatly, I get thrown of the board. 

I have searched for a solution for a long time, and I got a suggestion to go dual drive. Two motors would split the amps and I would therefor not exceed the max amp rating on the ESC. Is this a good solution?

Specs:
Ntm Propdrive 5060 V2
X-Car Beast ESC 120A
```

---
## \#2 Posted by: FredrikHems Posted at: 2017-10-25T11:13:20.433Z Reads: 232

```
Have you measured how many amps you really pull? That motor can max draw 90 amps, while your esc is good for 120. I have never heard about amp limits on that esc too?
```

---
## \#4 Posted by: TeslaAlex Posted at: 2017-10-25T11:27:10.723Z Reads: 216

```
Well at this point it´s my theory of whats happening, and im not sure how to test how many amps the motor draws.

Someone also mentioned it could be that im voltage sagging the batteries. I bought a voltmeter but it displays the voltage in percent. Going uphill at 100% charge, the display will show about 80 to 70%. Is that ok?
```

---
## \#5 Posted by: FredrikHems Posted at: 2017-10-25T11:33:54.408Z Reads: 194

```
Im not sure about the voltmeter, but if you want to check how many amps youre pulling, you can buy a turning wattmeter or similar. What exact batteries do you use?
```

---
## \#6 Posted by: TeslaAlex Posted at: 2017-10-25T11:37:06.784Z Reads: 182

```
Im using 2x Zippy flightmax 5000 mah 3s 20c.
```

---
## \#7 Posted by: ducktaperules Posted at: 2017-10-25T11:39:45.153Z Reads: 177

```
if this only happens going up hill could it be a heat related issue? maybe it cuts out cause it goes into thermal protection.
```

---
## \#8 Posted by: FredrikHems Posted at: 2017-10-25T11:40:55.245Z Reads: 173

```
Your batteries are rated for 100 amps max, and when you most likely pull 90, you will have some serious voltage sag. again, if you get a wattmeter, you can check the voltage when going uphill. 
I guess you hit the voltage protection.
```

---
## \#9 Posted by: TeslaAlex Posted at: 2017-10-25T11:41:27.831Z Reads: 164

```
It happens during regular acceleration too. If i pull the trigger too hard it stops immediatly. It´s quite annoying really...
```

---
## \#10 Posted by: FredrikHems Posted at: 2017-10-25T11:49:13.135Z Reads: 164

```
Pretty sure you hit the voltage protection.
```

---
## \#11 Posted by: TeslaAlex Posted at: 2017-10-25T12:03:36.492Z Reads: 162

```
Could batteries with better c-rating solve the problem, since they would not voltage sag as much? 

Maybe something similar to this, but for 6s (upgrade to 10s later):

[https://www.electric-skateboard.builders/t/high-power-10s-lipo-battery-pack-with-bms/10014?u=teslaalex](https://www.electric-skateboard.builders/t/high-power-10s-lipo-battery-pack-with-bms/10014?u=teslaalex)
```

---
## \#12 Posted by: FredrikHems Posted at: 2017-10-25T12:09:16.615Z Reads: 146

```
Yes, high C batteries like those will help a lot on voltage sag. But before investing 100$+ in new batteries, i would have bought a wattmeter to check if it really is the voltage sag that is the problem.
```

---
## \#13 Posted by: TeslaAlex Posted at: 2017-10-25T12:10:46.362Z Reads: 142

```
Well, ok. Im having a hard time finding a wattmeter that supports up to at least 120a. Could you link me one that is commonly used?
```

---
## \#14 Posted by: FredrikHems Posted at: 2017-10-25T12:12:53.812Z Reads: 137

```
https://hobbyking.com/en_us/turnigy-180a-watt-meter-and-power-analyzer.html This one support 180 amp, up to 12s
```

---
## \#15 Posted by: TeslaAlex Posted at: 2017-10-25T12:14:14.217Z Reads: 130

```
Thanks mate! I really appretiate it! Finally some progress, been trying to solve this for months!
```

---
## \#16 Posted by: Wilsonliang777 Posted at: 2017-10-25T15:45:19.090Z Reads: 128

```
How about getting a cheap battery checker.  The alarm will go off when battery cells drop below 3.7 to 3.2v.  I had a lot of battery voltage sag with my 25c rated lipo.
```

---
## \#17 Posted by: MontPierre Posted at: 2017-10-25T16:05:03.548Z Reads: 132

```
I would also recommend Bluetooth module and phone app like Metr ( there is thread about it here on the forum ). I will show you like your amps and also you can record your trips. Below is my today’s trip where up a Hill I tripped low voltage limit in vesc and shut off my board. It is 37V at the momemnt but with a sag up a hill it went below 35-33 and shut off my board.

https://metr.at/r/trTBo

Highly recommended for diagnostics and fun!
```

---
## \#18 Posted by: E1Allen Posted at: 2017-10-27T07:25:17.705Z Reads: 107

```
That is cool. Any reason motor temp isn't showing?
```

---
## \#19 Posted by: MontPierre Posted at: 2017-10-27T08:47:24.953Z Reads: 101

```
I think temperature displayed is the Vesc temp. Not sure if motors can be shown. You’ll have to ask @rpasichnyk who developed the app. 

Also  @emmaanuel has iPhone app (paid ) which works with cheap hm10 Bluetooth modules. I have both apps but haven’t checked out properly @emmaanuel one yet as it just got updated to ackmaniac 3.1 and vedder 3.0 firmware.
```

---
## \#20 Posted by: E1Allen Posted at: 2017-10-27T09:02:19.063Z Reads: 99

```
I'll have to check into those for my build. Has some great information.
```

---
## \#21 Posted by: emmaanuel Posted at: 2017-10-27T09:53:56.820Z Reads: 101

```
Yes the motor temp is one of the data available across the app:
http://www.electric-skateboard.builders/t/new-version-2-1-ios-eskate-vesc-app-for-standard-and-ackmaniac-fw/32340?u=emmaanuel

Your motor need to have a temp sensor for that.
This data is not in the default view, but you can add it.
```

---
## \#22 Posted by: TeslaAlex Posted at: 2017-10-29T07:53:03.457Z Reads: 86

```
**Update**

I ordered the wattmater from Hobbyking that works up to 60V and 180A, it should arrive soon. 
In the meantime I recorded a video of the problem so you really can see whats happening. 

YT Link: https://youtu.be/iRhGuUsmYLc
```

---
## \#23 Posted by: bartroosen12 Posted at: 2017-10-29T12:08:22.259Z Reads: 88

```
I should just buy 2 extra batteries and put them in parallel, like 50€ and you will get double the range and it's better for your batteries.
I got also a 120A esc and 2 x 20C batteries in parallel and no problems, enough power.
```

---
## \#24 Posted by: TeslaAlex Posted at: 2017-11-06T14:21:13.937Z Reads: 74

```
**Update!**
I finally got the wattmeter and hooked it up to my board. These are the results after the board shut off when riding:

<img src="/uploads/db1493/original/3X/2/4/2420b2663a5aed92bf9afe9a2ed9651b75bc4fb5.PNG" width="640" height="359"><img src="/uploads/db1493/original/3X/1/9/1963f1ff6608e6cb4f9d2cfe61861f73bca0faf4.PNG" width="640" height="359"><img src="/uploads/db1493/original/3X/d/a/da545f6b6319851f59844aef4571e2188f834b4b.PNG" width="640" height="359"><img src="/uploads/db1493/original/3X/6/c/6c0e2023e8069031a5500791a458cd668a1807be.PNG" width="640" height="359"><img src="/uploads/db1493/original/3X/3/8/389bcd3ddbe9daff87c8fa24c8b10d851159d7b5.PNG" width="640" height="359">

It seems as if i only hit about 35 amps, so the ESC is not the problem. The voltage goes to about 21,7V, is that low enough to trigger the voltage cutoff?
```

---
## \#25 Posted by: TeslaAlex Posted at: 2017-11-06T15:22:05.490Z Reads: 60

```
The ESC should be able to handle 120A and I am no where near that on my board. 

I used the programming card and set the voltage cutoff to 3.0V. Since I am running at 6s, that would mean that the voltage would have to go under 18V (6 x 3V = 18V) for the voltage cutoff to kick in, right?

If this is correct, neither the ESC or the batteries are the problem... If I am wrong, please help me understand! :slight_smile:

I did another test run:
<img src="/uploads/db1493/original/3X/9/0/90095c62af3783107aab676a0a0e44cf12c3c5d6.png" width="353" height="500">
```

---
## \#26 Posted by: TeslaAlex Posted at: 2017-11-06T17:29:51.866Z Reads: 47

```
Does anyone have a clue? Im getting tired of not knowing what the problem is.
```

---
