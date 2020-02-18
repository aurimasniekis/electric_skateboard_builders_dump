# Trouble calibrating Ezrun MAX6 with mini remote

### Replies: 7 Views: 950

## \#1 Posted by: ciocan Posted at: 2016-10-01T10:28:22.459Z Reads: 94

```
Hui guys,

I just finished putting all the parts together but I the calibration seems not to work. The miniremote is paired with the receiver, I did all the steps read in the docs but the esc start normally.

So basically, I turn on the remote, press and hold the set button on Max6 then press turn on button and release set. It suppose to go in calibrate mode but it does not.

What seems to be wrong? The esc or the receiver?
```

---
## \#2 Posted by: EssEnn Posted at: 2016-10-01T23:09:43.159Z Reads: 78

```
I found I needed to hold the set button, press the power button for 0.5 seconds, dont just tap it. Then after the first bleep, release the set button.
```

---
## \#3 Posted by: ciocan Posted at: 2016-10-02T21:38:06.697Z Reads: 65

```
Thanks @EssEnn. It seems that their manual is wrong.
```

---
## \#4 Posted by: EssEnn Posted at: 2016-10-02T21:55:38.214Z Reads: 65

```
Yeah it took me a few trys to figure it out. Just poorly explained. I hope you got one of the 3in1 programming boxes.
```

---
## \#5 Posted by: ciocan Posted at: 2016-10-02T22:17:28.236Z Reads: 66

```
Yes, I have the programming box. Without it's a nightmare to configure all the params.
```

---
## \#6 Posted by: EssEnn Posted at: 2016-10-02T22:22:33.168Z Reads: 67

```
Yeah when I read the manual I realised I would need the box. Also mega handy to check my LIPO's voltage as well.
```

---
## \#7 Posted by: Nowind Posted at: 2016-10-03T07:53:37.820Z Reads: 55

```
Manual is wrong.

      Power on remote control

      hold SET and power on ESC on powerswitch, release powerswitch
      immeditaly... BUT hold SET until it starts to beep beep beep beep
      beep beep

      release SET button it should still makes beep beep beep beep beep
      beep

      trigger in neutral : press set shortly, one beeps 

      hit full trotthle : press set shortly, two beeps 

      hit full brake : press set shortly, three beeps

      little melodie appears..... GREAT

      Power OFF ..... then power on again and try

## You can check this way if you done it correct:

hold full throttle : the led on esc should get green
hold full brake :  the led on esc should get green

if its only red then something is not right and do calibration again.... 
check if the potientiometer of throttle is in neutral


Make sure that you have deactivate the BEC by one ESC before connecting them via Y-Wire.
You know just remove by one ESC the middle, red, positive wire out of connector and isolate.
I would calibrate both ESC at the same time !

Check if Remote correctly bindet to reciever.
Led on the reciever on?
Connectet to port 2 ?

<img src="/uploads/db1493/original/3X/5/9/59bd61e27c8ffd4da02d03a67b658d2f1d610021.PNG" width="325" height="283">

<img src="/uploads/db1493/original/3X/9/7/972a38acc5c8d293e065df1dfeaf970c4abdb4aa.PNG" width="316" height="340">
```

---
