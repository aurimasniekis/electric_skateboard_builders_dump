# HM10 module not seen

### Replies: 12 Views: 244

## \#1 Posted by: ProgressionOfFun Posted at: 2018-09-13T03:13:17.356Z Reads: 96

```
Sooo got my hm10 module hooked up to my master focbox, everything is plugged in right and baud rate is set to 9600. I've also tried 115200. The red light is blinking (as in to indicate discovery?) My phone just wont see it in ackmaniacs app and the metr app. My phone is a samsung s8. Any insights are appreciated.
```

---
## \#2 Posted by: SeanHacker Posted at: 2018-09-13T03:22:48.494Z Reads: 94

```
Make sure you have UART + PPM selected. 

What version of Android are you running? Oreo won't work with generic (clone) modules.
```

---
## \#3 Posted by: ProgressionOfFun Posted at: 2018-09-13T03:29:29.153Z Reads: 91

```
Gotcha, probably the module then, could you point me in the direction of one that would work on Oreo?
```

---
## \#4 Posted by: threebysix Posted at: 2018-09-13T03:33:18.095Z Reads: 85

```
Are the TX/RX (HM10) and RX/TX (FOCBOX) connected correctly to one another?
```

---
## \#5 Posted by: ProgressionOfFun Posted at: 2018-09-13T03:34:42.848Z Reads: 80

```
Yeah its all set up right, it was just a cheap module i had laying around.
```

---
## \#6 Posted by: AlexBE Posted at: 2018-09-13T03:35:15.345Z Reads: 76

```
If the red light is flashing and your phone can't see it, something is wrong with the module->phone connection. Try to find the module in the bluetooth part of your phone settings, ie don't use the apps.
```

---
## \#7 Posted by: ProgressionOfFun Posted at: 2018-09-13T03:36:41.076Z Reads: 81

```
Did that, no dice. Its gotta be what @SeanHacker said.
```

---
## \#8 Posted by: mmaner Posted at: 2018-09-13T03:38:48.050Z Reads: 82

```
If your using Android 8 it most likely will not see the hm-10 module, Bluetooth standards have changed in 8. 

An hm-10 will never work with Metr. You have to have the Metr module to use the Metr app. It's worth it though, I've got 2.
```

---
## \#9 Posted by: boramiNYC Posted at: 2018-09-13T04:01:55.273Z Reads: 78

```
Would the firmware on Focbox affect UART transmission? Having similar problem.
```

---
## \#10 Posted by: AlexBE Posted at: 2018-09-13T04:05:08.628Z Reads: 79

```
I would disconnect the tx/RX pins, they aren't relevant to your phone being able to see the bluetooth device. TRy and see if you can pair with it using a laptop. If you can't even see the bluetooth device, the focbox connection side of things is irrelevant.
```

---
## \#11 Posted by: Acido Posted at: 2018-09-13T05:54:16.952Z Reads: 63

```
Try turning on the locaton services
```

---
## \#12 Posted by: ProgressionOfFun Posted at: 2018-09-13T15:30:36.872Z Reads: 43

```
UPDATE: Tried on an older android phone without Oreo. Picked it up just fine. I appreciate the insights, thanks everyone.
```

---
