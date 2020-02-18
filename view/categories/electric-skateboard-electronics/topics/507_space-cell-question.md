# Space Cell question

### Replies: 9 Views: 1308

## \#1 Posted by: BigAl Posted at: 2015-11-18T14:43:22.701Z Reads: 90

```
so my next question is regarding the space cell. when I unpacked the cell this weekend I turned it on and it indicated 76%. obviously when I charge it, it will indicate 100%, so my question is, how long can I use it for? to what percentage can I discharge it to without causing any damage to the cell?

Thanks guys
Al...
```

---
## \#2 Posted by: chaka Posted at: 2015-11-18T15:16:19.644Z Reads: 90

```
The BMS in that pack will shut off in two different scenarios. 

If you ask for more than 60amps it will cut power.

If you discharge below 3v or 2.8v it will cut power.

The second scenario can happen at many different levels of discharge depending on the how many amps you are asking the pack to deliver.  Lets say the BMS cuts power while you are blasting around at full throttle due to low voltage, if you then switch to a less aggressive riding style you will get a few more miles before it cuts power again.
```

---
## \#3 Posted by: BigAl Posted at: 2015-11-18T15:58:23.179Z Reads: 87

```
@chaka that makes sense, thank you

So I can run the battery until it shuts off without damage?  What about the 80% rule???  does that still apply?

Thanks again for your response

Al...
```

---
## \#4 Posted by: chaka Posted at: 2015-11-18T16:18:14.985Z Reads: 83

```
That rule is based on resting voltage, the voltage will bounce back up to about 3.5v per cell when not under load in most cases.
```

---
## \#5 Posted by: kai Posted at: 2015-11-18T16:40:01.046Z Reads: 79

```
So you can run the space cell till it shuts down on its own then? I am confused.
```

---
## \#6 Posted by: Iceni Posted at: 2015-11-18T17:03:29.773Z Reads: 78

```
Yes, you can run it until it shuts down on its own.
```

---
## \#7 Posted by: onloop Posted at: 2015-11-19T00:36:27.621Z Reads: 75

```
You can ride until the battery turns off, It's got safety features built-in so it's designed to be as fool proof as possible....

If you combine it with the vesc and adjust all the settings accordingly you will never exceed the amp draw limit and you will never have to worry about damaging the battery ever. SET&FORGET

The Low Voltage Cut off (LVC) of S.P.A.C.E Cell is 27.5v
This is how the LCD is programmed.
42v = 100%
40v = 80%
37v = 50%
35v = 30%
33v = 10%
32v = 0%

Once the battery reaches 0% under load you will probably be hitting the LVC

So in theory you can ride it until the readout reaches 0%
```

---
## \#8 Posted by: El_Cid Posted at: 2016-07-28T16:30:51.755Z Reads: 44

```
Hey, when I first got my raptor dual it was perfect. I could ride hard accelerate fast and stop hard! after a few days of riding I've been having the issue that even with a fully charged battery and with the VESCs set to only pull 25A Max from the battery each so total of 50A But if I accelerate any more than a gentle rolling start the battery shuts off (display turns off) even if the rocker switch is still on. I turn the switch off and then back on and the battery comes back to 97 or whatever percent it was at and continues to work as long as I accelerate very gently... what could it be? please help... its very annoying to have a full battery and then take off to cross a street and have it shut down on me half way through the intersection...
```

---
## \#9 Posted by: CamBo Posted at: 2017-10-28T23:56:07.500Z Reads: 18

```
Did you ever figure this out?  I have a space cell doing the same thing.
```

---
