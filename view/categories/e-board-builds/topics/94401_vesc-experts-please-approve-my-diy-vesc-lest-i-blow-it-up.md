# VESC experts: Please approve my DIY VESC lest I blow it up

### Replies: 19 Views: 814

## \#1 Posted by: Fungineers Posted at: 2019-05-20T08:14:05.988Z Reads: 240

```
Hey guys!

I recently got into SMD soldering and thought I would build a VESC. The first one I built blew up right away- as soon as I gave it 12V (0.3A current), I saw some interesting sparks on the DRV. I reckon the failure was due to using solder paste and not cleaning it, creating short circuits on the DRV. 
Anyway, lesson learned, here is my brand new VESC. Before I power it on, I want to run it through the experts here: @chaka @trampa @onloop @longhairedboy (anyone else?).
Does this look good?
Oh, and one question: All LEDs seem to work when tested with multimeter, except the blue LED. I tried to replace it, took a new one that worked on the table, but as soon as I soldered the new one, it stopped working too! Weird. Anyway Im thinking I dont need the LED (I ran out of them, and order takes time), so the question is, is there an LED bypass on the VESC? Or will it cause an open circuit where the LED is? 
Pictures attached below:
![IMG_20190520_110943|375x500](upload://wflSF8iRnLTYeYdtmjFm8tz0mYZ.jpeg) ![IMG_20190520_110926|375x500](upload://2GfwFDa2MeI1Js84IgsTpv1U4Ex.jpeg) ![IMG_20190520_110916|375x500](upload://tgUabokcFaX7CwV5oRmurICpmos.jpeg) 






Thanks guys!
```

---
## \#2 Posted by: louwii Posted at: 2019-05-20T08:31:34.899Z Reads: 212

```
Not an expert about the VESC, but there are 3 bent pins on the DRV (well I think it's the DRV, long SMD chip on the first picture). Looks like those pins might not be in contact with the right pads.

There are 2 bridges on 2 pins too on the same chip (but that might be on purpose I guess).
```

---
## \#3 Posted by: bluegreen Posted at: 2019-05-20T08:45:08.858Z Reads: 207

```
There are a few problems, addition to the 2 noticed by @louwii I think you've put one of the mosfets completely off it's footprint by one pad:

![image|375x500](upload://r4xq5o7oALJdeNUyQVIVVXyj2qk.jpeg)
```

---
## \#4 Posted by: linsus Posted at: 2019-05-20T08:56:35.488Z Reads: 189

```
Two pairs on the DRV is s'posed to be bridge, so thats probably them on the lower part of the picture.
I recommend that you inspect both the DRV and MCU with a sterescope before you try to run any power thru. Use plenty of flux.
Are you sure the LED is soldered with correct polarity?

I can't remember the idle current of the VESC but try to use a current limiting DC-box when powering up the first time. 100mA should be more then enough for a VESC without any FW on it.
```

---
## \#5 Posted by: Fungineers Posted at: 2019-05-20T09:40:04.329Z Reads: 182

```
Thanks @linsus and @bluegreen
Yes, those 2 pairs of pads that are soldered together are the ones that are supposed to be shorted.
As for the other pins that @bluegreen highlighted on the DRV, those are bent, and I cant seem to straighten them (Im afraid it will lift the pads from the board if i push it too hard). I checked with a mulitmeter and they arent shorted. Still, do you think I should take off the DRV, straighten the pins, and resolder? 
As for the MOSFET, yeah it seems to have drifted off while reflowing, but does it matter? I mean all the pins are connected to the same pad end of the day, isnt it? 
Thanks again guys!
```

---
## \#6 Posted by: linsus Posted at: 2019-05-20T09:46:17.897Z Reads: 171

```
I would resoled both the DRV and the mostfet. 
The leg you soldered incorrectly is the gate pin. It is not electrically connected to the other ones.
```

---
## \#7 Posted by: Fungineers Posted at: 2019-05-20T10:02:23.065Z Reads: 163

```
Yeah good advise. Will re-do those two. Thanks!
```

---
## \#8 Posted by: longhairedboy Posted at: 2019-05-21T20:03:31.920Z Reads: 127

```
it is the correct color to go fast.
```

---
## \#9 Posted by: Fungineers Posted at: 2019-05-23T04:41:33.403Z Reads: 89

```
So I redid the DRV, and the MOSFETs, I connected the power cables to 12V powersupply. All was good for about 2 mins and then some burning smell, and little sparks between some pins of the DRV....again.
At this point, I dont know what I am doing wrong. I have one last DRV to try, and I wanna make this count. I am going to clean the board, redo the DRV, triple-check for shorts/ solder bridges. Any other advice? PLEASE let me know.
Thanks!
```

---
## \#10 Posted by: Gamer43 Posted at: 2019-05-23T05:29:23.867Z Reads: 80

```
Which pins? Are there shorts to ground on any of the power supply rails or phase connections?
```

---
## \#11 Posted by: Fungineers Posted at: 2019-05-23T06:34:56.413Z Reads: 76

```
No shorts that I could see! 
I will get a photo when I get home.
```

---
## \#12 Posted by: linsus Posted at: 2019-05-23T13:53:00.879Z Reads: 68

```
Please us a current limiting supply and u wont have to burn thru your chips.
```

---
## \#13 Posted by: Fungineers Posted at: 2019-05-23T14:20:13.855Z Reads: 63

```
@linsus thats the surprising part. I did! 12V and almost nothing in current. 0.3A maybe. Im lost.
```

---
## \#14 Posted by: Gamer43 Posted at: 2019-05-23T16:23:03.582Z Reads: 54

```
Set the limit to 0.1A, and did you probe around with a multimeter?
```

---
## \#15 Posted by: bluegreen Posted at: 2019-05-23T18:31:32.306Z Reads: 50

```
If it didn't blow up immediately then it's probably not a dead short. What it sounds like is maybe one of the resistors is installed with the incorrect value or maybe a diode is the wrong way. You'll have to check each component with a multi meter if there aren't any visual problems.
```

---
## \#16 Posted by: Fungineers Posted at: 2019-05-25T13:25:43.251Z Reads: 45

```
Update: They say 3rd time is the charm. 
This time I desoldered the DRV, cleaned the damned board. Got a new DRV on, checked for bridges. Checked with a multimeter for bridges. Rechecked then triple checked. Then i cleaned with a lot of alcohol, and connected to the power supply and hid behind my desk to hear an explosion....no explosion. Hurrah! 
Successfully booted and programmed. 
Thanks to everyone on this thread!
```

---
## \#17 Posted by: Singh Posted at: 2019-09-17T20:43:22.949Z Reads: 30

```
I need some help with the setup to use the vesc, does it run on hub motors?
```

---
## \#18 Posted by: Singh Posted at: 2019-09-17T21:10:26.081Z Reads: 23

```
Wich vesc tool have the latest firmware?
```

---
## \#19 Posted by: Fungineers Posted at: 2019-09-18T01:24:35.756Z Reads: 17

```
You should open a new discussion since this is not related to the topic.
Anyway, yes vesc can run the hubwheel.
Just download the latest tool from vedders website and it will have the firmware needed on the connections page.
```

---
