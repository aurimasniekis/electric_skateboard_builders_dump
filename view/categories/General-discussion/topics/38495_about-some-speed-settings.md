# About some speed settings

### Replies: 20 Views: 1549

## \#1 Posted by: Bloop Posted at: 2017-11-16T09:06:34.277Z Reads: 125

```
Hey guys o/ is there any setup that could be made on vesc to reduce the overall speed ?

Or speed only depends on motors kv, transmision and wheel size ?

Thank you.
```

---
## \#2 Posted by: krloz Posted at: 2017-11-16T10:01:33.049Z Reads: 120

```
You can directly limit the speed through the erpm which cam be translated to motors rpm Which translates to wheel speed.
Also ackmaniac firmware, that I know at least, let's you set a limit directly for speed
```

---
## \#3 Posted by: Bloop Posted at: 2017-11-16T10:07:12.644Z Reads: 114

```
<img src="/uploads/db1493/original/3X/4/f/4fbc5ae4c2bb475bd48094e2e87f133d16e20425.png" width="281" height="500">

So here if i reduce that max speed to 25 it wont go over ? 

Not sure why but i did not changed that so far i will have to test it out
```

---
## \#4 Posted by: Ackmaniac Posted at: 2017-11-16T11:35:43.186Z Reads: 89

```
Yes, but tale care that you set up the correct pulley sizes, wheelsize and magnet count.
```

---
## \#5 Posted by: Bloop Posted at: 2017-11-16T11:43:12.732Z Reads: 86

```
I have them set (not 100% sure about the magnets count i guess 14. I will ask to see for sure). But what will happened if this settings are off ?

This might be exactly what i need to limit the board for some beginner friends .. few days ago one of them tried the board and he didnt really liked to go slow and he went to 30 35 km/h then felt ... so from now on i will limit to ~25 for beginners just in case ... 

Thank you <3
```

---
## \#6 Posted by: Bloop Posted at: 2017-11-21T11:18:03.332Z Reads: 63

```
hey i just tested today and is not working for me :-( i still got to 44km/h .. any idea what am i doing wrong?
 <img src="/uploads/db1493/original/3X/b/0/b0069a01aebda06fe9e0dd4270aca35a0fa5b6f0.png" width="281" height="500">
<img src="/uploads/db1493/original/3X/4/4/4428ae73bf0d1d8b6ece14ffc22cb38821d9c532.png" width="281" height="500">
```

---
## \#7 Posted by: Ackmaniac Posted at: 2017-11-21T11:28:10.665Z Reads: 56

```
Which firmware do you use?
```

---
## \#8 Posted by: Bloop Posted at: 2017-11-21T11:50:15.495Z Reads: 55

```
Your firmware i installee it like 2 months ago and ran watt mode 

https://www.electric-skateboard.builders/t/extended-bldc-tool-with-watt-control-mode-ppm-cruise-control-individual-throttle-curve-and-android-app/12286?u=bloop
```

---
## \#9 Posted by: krloz Posted at: 2017-11-21T12:18:34.560Z Reads: 51

```
Was that max speed you hit maybe going down hill?
```

---
## \#10 Posted by: Bloop Posted at: 2017-11-21T12:30:40.245Z Reads: 50

```
straight line :( when i left home i have a good straight  road so i tested there and now agian .. no sign of it stoping at 20km/h as i set it...
```

---
## \#11 Posted by: Ackmaniac Posted at: 2017-11-21T12:34:11.533Z Reads: 51

```
I can see that in the activated mode the speed wasn't updated.
Did you first activate the mode and the adjust the max speed? Because each time you make changes to a mode you have to activate it another time so that the changes take place.
<img src="/uploads/db1493/original/3X/9/9/99ca76850e6b3a88ac45e352428b5665ef3ed073.png" width="310" height="499">
```

---
## \#12 Posted by: Bloop Posted at: 2017-11-21T12:39:10.548Z Reads: 46

```
i made the new mode then activated it .. but even now when im activating it is set to 280 the Max km/h stay always at 280 no matter of what mode i select
```

---
## \#13 Posted by: Bloop Posted at: 2017-11-21T12:40:35.416Z Reads: 52

```
I guess is taking only the default value :-??

<img src="/uploads/db1493/original/3X/e/9/e9bf01aa9008d5c640597e4de8882ab27235c6a3.png" width="281" height="500">
<img src="/uploads/db1493/original/3X/2/c/2c5391edf8907508e93f38a057260455f7464d85.png" width="281" height="500">
```

---
## \#14 Posted by: Ackmaniac Posted at: 2017-11-21T12:43:35.309Z Reads: 51

```
Which remote do you use?

Seems that i have a error in the old firmware with the adjusted speeds. Need to have a look at it, in the meanwhile you can also use the new Firmware which is based on VESC-Tool firmware.

http://www.electric-skateboard.builders/t/extended-ackmaniac-esc-tool-based-on-vesc-tool/35116
```

---
## \#15 Posted by: Bloop Posted at: 2017-11-21T12:47:24.140Z Reads: 51

```
Enertions Nano X remote.

Alright i will try to upload the new firmware first to read a bit about it
But really fast any problems with watt mode on foc -> im using 2 focbox'es

If i can help you just let me know :-?? i can test this more or idk how to get logs or what you need.
Thank you.
```

---
## \#16 Posted by: krloz Posted at: 2017-11-21T12:54:45.141Z Reads: 52

```
@Ackmaniac
 I think my speed limit worked fine.  And I am using your first firmware
```

---
## \#17 Posted by: Bloop Posted at: 2017-11-25T13:17:48.844Z Reads: 45

```
What version should i install ? What is the  Hardware version 

Im using focbox.

<img src="/uploads/db1493/original/3X/8/3/833bc092ad68699378de41fcc1d0c14928622069.png" width="690" height="446">
```

---
## \#18 Posted by: Ackmaniac Posted at: 2017-11-25T13:33:18.968Z Reads: 43

```
The FOCBOX is based on the 4.12 Hardware
<img src="/uploads/db1493/original/3X/5/2/52e16301d9292132a7cbaaf1854ee3eaa7c75b1e.png" width="690" height="446">
```

---
## \#19 Posted by: Bloop Posted at: 2017-11-25T15:57:37.810Z Reads: 36

```
@Ackmaniac  Sorry for lots of questions really appreciate your help 

I cant find the watt mode tho ? am i doing something wrong ? shouldn't it be here or is named different ?

<img src="/uploads/db1493/original/3X/1/7/174f19b2816a2f737d87effcad1355666ee4f1ae.png" width="690" height="408">
```

---
## \#20 Posted by: Ackmaniac Posted at: 2017-11-25T16:23:43.381Z Reads: 33

```
In my firmware mod current control is Watt control because in the first public version of VESC-tool current control was the same as Watt control at acceleration. Now VESC-tool is back to the old current control.
```

---
