# Update firmware on the vesc w/ windows

### Replies: 20 Views: 5059

## \#1 Posted by: locktight Posted at: 2015-12-11T23:17:31.463Z Reads: 281

```
hello all i am trying to update my vesc to v2.3 i am at v1.14 now. when i open the new version of the bldc tool for windows and connect i get this message<img src="/uploads/db1493/original/2X/7/7529f1bc2ba3c1276dbfd3830e474e9d1484ebe0.PNG" width="564" height="206">

so i go to the firmware tab and in the update new firm ware section i hit the choose button and this pops up <img src="/uploads/db1493/original/2X/1/109c4397293bd0e2f12eaae7ead396fcc8860557.PNG" width="580" height="268">

i tried opening all of these but could not get any firmware updates. how can i update the firmware on the vesc using the windows version of the bldc tool?
```

---
## \#2 Posted by: sl33py Posted at: 2015-12-11T23:39:04.107Z Reads: 244

```
careful.  I ended up only partially updating the firmware w/ BLDC tool (windows port) and when it hung/failed it was D.E.D.

Until i hooked up a programmer board in linux and reflashed to latest.  I was trying to go from 1.10 to 1.13 at the time.

As an insurance policy do you have a programming board? (ST-LINK v2?)  Linux system to use if ported version doesn't work?
```

---
## \#3 Posted by: Jeff Posted at: 2015-12-11T23:40:24.684Z Reads: 239

```
I remember reading somewhere that you should update the firmware on the VESC before running the new version of the BLDC.
```

---
## \#4 Posted by: cmatson Posted at: 2015-12-11T23:42:14.652Z Reads: 236

```
I'm interested in this thread topic, and was actually going to make one right now had I not seen yours! 

Haha I really want FOC, but I don't trust myself to successfully update everything..
```

---
## \#5 Posted by: tomtnt Posted at: 2015-12-12T04:34:10.784Z Reads: 226

```
the update was very and quick - I used the OS X version that jaccobloy compiled.  The new versions are actually v2.4 firmware and app.
```

---
## \#6 Posted by: kai Posted at: 2015-12-24T17:03:44.544Z Reads: 220

```
did you ever figure this out @locktight ? i have the same problem with the windows version
```

---
## \#7 Posted by: locktight Posted at: 2015-12-24T19:19:01.262Z Reads: 216

```
i haven't figured it out. i still need to try a few things but what you have done is probably what i am going to try. it hasn't been high on my priority due to the snow. i might be able to try tomorrow. Merry Christmas everyone! :smile:
```

---
## \#8 Posted by: kai Posted at: 2015-12-24T19:32:49.891Z Reads: 210

```
merry christmas bro. i just got an rc remote for a temp controller so i can get riding. just need to button it up now
```

---
## \#9 Posted by: EnertionSupport Posted at: 2015-12-31T04:22:44.601Z Reads: 205

```
A Warning about updating VESC firmware!!


> *Quote By: Benjamin Vedder. Using the wrong firmware will most likely kill the FETs and/or the drv, so when you change firmware you should use some kind of power supply that cannot deliver too much current at first and preferably a low voltage (<20 V).*


Only attempt to change the firmware if you are aware of the risks. A failed firmware upgrade can permanently damage the VESC. The enertion warranty doesn't cover faults relating to failed firmware upgrades.
```

---
## \#10 Posted by: EnertionSupport Posted at: 2015-12-31T04:26:50.381Z Reads: 200

```
Try this version of BLDC tool as it is compatible with the firmware of December Batch of Enertion VESC https://drive.google.com/file/d/0B4M52aF7FaMWM2lsalBNbjlWNWM/view?usp=sharing
```

---
## \#11 Posted by: trbt555 Posted at: 2015-12-31T07:26:30.892Z Reads: 198

```
The folders in that link don't seem to contain the actual .bin firmware files, which is what @locktight was asking in his original post.
```

---
## \#12 Posted by: trbt555 Posted at: 2015-12-31T07:45:28.326Z Reads: 198

```
Here's a link from @jacobbloy which will lead you to all versions of the BLDC tool. I found this very useful.

[LINK TO ALL VERSIONS OF BLDC TOOL][1]

Here's what worked for me:

 - dowload the 2.7 version
 - connect vesc to reliable power supply
 - connect the VESC to USB and let BLDC tell you the firmware is old
 - go to firmware tab, select "choose" 
 - navigate to folder "firmwares 2.7    FOC" and then the folder for
   your hardware version (written on your    Vesc, right next to the PPM
   pins)
 - select "default.bin"
 - update firmware
 - done


  [1]: https://drive.google.com/folderview?id=0Bym9XrdeViekfkRETmRndENkcVpySW5sWjIzOWdrLThCY01HY3BPOXpqYVRHUlQxS0R5ZlU&usp=drive_web#list
```

---
## \#13 Posted by: OGP Posted at: 2016-02-14T22:05:26.959Z Reads: 169

```
Is there a version compatible with FOC 2.8 that was recently sent out?  I'm totally scared to update the firmware or mess with the VESC.
```

---
## \#14 Posted by: EnertionSupport Posted at: 2016-02-15T01:56:43.309Z Reads: 166

```
With the VESC, we usually don't recommend trying to update and change the firmware unless you know exactly what you are doing. It isn't too terribly difficult, but if you were to incorrectly update it, your VESC very well could be dead. 

Are you asking what windows version is compatible with FOC 2.8, or which VESC PCB is compatible? 

For the windows versions, check out this thread:

http://www.electric-skateboard.builders/t/vesc-faq-windows-version-of-bldc-tool/141
```

---
## \#15 Posted by: locktight Posted at: 2016-03-12T17:53:26.658Z Reads: 147

```
well i tried upgrading firmware again today and ran into some issues.i first tried updating on the newest version of the bldc tool but it could not update  due to the older firmware on my vescs. next i tried downloading the firmware from that bldc tool using an older version. it starts by saying buffer erase under the loading bar but it then switches to buffer erase timeout, and doesn't do anything. any suggestions on how i go about fixing this?
```

---
## \#16 Posted by: alexjones Posted at: 2016-07-24T08:43:34.380Z Reads: 115

```
Hello locktight...just wanted to know if you managed to fix the upgrading firmware issue? I have exactly the same problem with my version 4.12 VESC trying to upgrade from 2.15 to 2.17 - 2.18 issue and I have no idea what to do. Cheers, Alex
```

---
## \#17 Posted by: ninja Posted at: 2016-11-19T02:15:25.666Z Reads: 89

```
Hi! 
How did you manage your problem with 4.12 VESC trying to upgrade from 2.15 to 2.17 - 2.18 issue? I have same situation now.
```

---
## \#18 Posted by: tibal32 Posted at: 2017-02-16T02:56:06.278Z Reads: 72

```
<img src="/uploads/db1493/original/3X/9/8/989209a7dc8bce48657a343e11e121a960fb122c.png" width="690" height="251">

so im doing my first build for learning purposes but im in this situation i got my 4.12 VESC with firmware 2.18 and i got the windows BLDC-Tool ACKMANIAC mod 2,53 and it says the connected vesc has too old of a firmware... should i get an older bldc tool or update the firmware of my VESC. and where do i get the firmware or the tool cuz the older tool i got is the 2.52 from ackamniac :disappointed_relieved: would really appreciate the help PS: i got my vesc motor receiver and controller all hooked up and the vesc is powering the motor and i can control it with the remote so at least i got the remote pairing thing right i guess :smile: any help would be deeply appreciated
```

---
## \#19 Posted by: lox897 Posted at: 2017-02-16T05:50:24.275Z Reads: 63

```
@ackmaniac could probably help you
```

---
## \#20 Posted by: Ackmaniac Posted at: 2017-02-16T07:25:33.792Z Reads: 57

```
To use my modded bldc-tool you have to flash the vesc with my firmware mod which can Fiat the same Dropbox link.
```

---
