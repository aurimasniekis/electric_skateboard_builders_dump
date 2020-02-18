# \[Solved\] Vesc can&rsquo;t connect to pc!

### Replies: 14 Views: 3623

## \#1 Posted by: Evan Posted at: 2016-08-09T09:20:41.343Z Reads: 287

```
It was still working yesterday but then today it doesn't connect to pc at all. Didn't do anything on vesc or the usb 1.0 cable. My pc can't even find it on any usb port..... I need help please! Any indicator should turn on when it's successfully connected? (don't remember what it was like when it was still working)
```

---
## \#2 Posted by: kampfhahn Posted at: 2016-08-09T09:45:44.633Z Reads: 287

```
Sorry, i don´t want to assume that you are stupid, but is your battery connected to the VESC? To my knowledge, the power from the USB-Port isn´t enough for the configuration of the VESC.

Another fact is that the VESC is very picky with the USB-Cables. Use a short one with good shielding.
```

---
## \#3 Posted by: lowGuido Posted at: 2016-08-09T10:03:23.762Z Reads: 280

```
check you device settings for the com port number. make sure you select the com port thats listed in devices.
```

---
## \#4 Posted by: Evan Posted at: 2016-08-09T10:03:54.909Z Reads: 278

```
Cool mate.Yes it's connected to space pro 4 first. Well actually  I fucked up the cable I used yesterday which came from Enertion(steez) controller.

<img src="/uploads/db1493/original/2X/3/317a053fc59d51b429066129ff306aec34cc9360.jpg" width="500" height="500">

Cos even though the connecting head was longer then the ordinary one, somehow it was still bit short to charge the controller so I cut the edge thought it could be long enough but accidently tear it in half.....

<img src="/uploads/db1493/original/2X/c/c19887051c98fa3b4111bde0ab1c7225a0053186.JPG" width="690" height="388">

<img src="/uploads/db1493/original/2X/7/7cd44914b10b478e2d979afcdc5e5cab41fbffe5.JPG" width="690" height="388">

Is it possible because of this particular usb cable I broke so the vesc doesn't connect to pc anymore? I should buy a[ new one](http://www.ebay.co.uk/itm/USB-Type-A-Male-to-Mini-B-5-Pin-Cable-Extra-Long-Plug-V3-Lead-For-MP3-MP4-MP5-/291596726947)?
```

---
## \#5 Posted by: Evan Posted at: 2016-08-09T10:09:15.642Z Reads: 241

```
device manager doesn't show anything up when I connect the vesc to pc. BLDC tool only got com3 can pick and keep saying the firmware is too old I should update it (just because can't read vesc)
```

---
## \#6 Posted by: kampfhahn Posted at: 2016-08-09T10:11:36.853Z Reads: 241

```
So just to get this right:

You used to use the Enertion cable which always worked but now it´s broken and you tried another one which isn´t working? Then i would definitely say that the VESC doesn´t like your spare cable.

Usually there are a lot of these cables in a household. Do you have a Gopro or an old cardreader / external 2,5" harddrive with the same mini usb connector?
```

---
## \#7 Posted by: lowGuido Posted at: 2016-08-09T10:11:49.745Z Reads: 232

```
well if it connects enough to say you need to update the firmware then its connected..
```

---
## \#8 Posted by: Evan Posted at: 2016-08-09T10:20:00.086Z Reads: 225

```
Nice logic mate!

What I've got now are two cheap cables that I already forget where did they come from. But I tried my mate's nikon camera usb cable and it doesn't work.

So what I'm trying to say is WHAT IF I did something wrong to vesc cause the usb port doesn't function anymore, any sign show on vesc? Just guessing.
```

---
## \#9 Posted by: Evan Posted at: 2016-08-09T10:20:28.970Z Reads: 218

```
BLDC tool shows nothing has been found so..... :slight_frown:
```

---
## \#10 Posted by: Evan Posted at: 2016-08-09T10:36:27.716Z Reads: 210

```
OKAY GUYS IT'S WORKING AGAIN!!!

Got no idea why but hey.....all we want is the good result like this lol

<img src="/uploads/db1493/original/2X/9/9a4240f96e3d7a3070ce7bdadf7e54173b522ee9.JPG" width="690" height="388">
```

---
## \#11 Posted by: kampfhahn Posted at: 2016-08-09T11:06:28.120Z Reads: 200

```
Good to hear that!

I like the braces box :D
```

---
## \#12 Posted by: racidon Posted at: 2016-08-09T11:17:54.423Z Reads: 192

```
Does enertion's control use the same type of usb port? I thought it would have been the same as other controllers

I thought the controller would use Micro-B where as the VESC uses Mini-B
```

---
## \#13 Posted by: Evan Posted at: 2016-08-10T10:28:51.485Z Reads: 175

```
It uses MINI-B!! And needs a extra long plug in order to reach the charging port....

<img src="/uploads/db1493/original/2X/7/732291d07d82f87e8232040e6485bdd0bbf4a4c8.JPG" width="690" height="388">
```

---
## \#14 Posted by: kampfhahn Posted at: 2016-08-10T11:12:08.378Z Reads: 164

```
That obviously is not really the best solution for a charging port :confused:
```

---
