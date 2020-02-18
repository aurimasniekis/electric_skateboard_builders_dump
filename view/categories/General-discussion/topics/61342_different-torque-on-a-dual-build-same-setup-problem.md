# Different torque on a dual build same setup (problem)

### Replies: 16 Views: 339

## \#1 Posted by: Komamtb Posted at: 2018-07-09T12:27:30.214Z Reads: 142

```
Hey guys, as the title says, I have a build running identical dual setup, I can feel by hand, that one motor has a lot less torque while  starting up, I can barely hold one, while I can stop another by a slight force to a dead stop, I do run same vescs settings on both, I don't feel any drifting of one side or the other, I had a pulley slipped on the stronger motor and had to ride a bit with a weaker one and was not impresive at all, what this problem could be?
```

---
## \#2 Posted by: i2oadsweepei2 Posted at: 2018-07-09T13:30:30.283Z Reads: 134

```
Have you double and triple checked both vesc settings? The only other thing I can thing of is weak solder joint somewhere on the weak side.

Hope you find the reason.
```

---
## \#3 Posted by: kuphjr Posted at: 2018-07-09T13:56:14.851Z Reads: 119

```
Did you try plugging the each motor into the opposite VESC?  This will make it easier to determine if the problem is with the motor, VESC or maybe one of your solder or wiring connections.
```

---
## \#4 Posted by: kuphjr Posted at: 2018-07-09T13:57:01.520Z Reads: 112

```
Also pictures might be helpful.  You would be amazed and what issues I have seen solved on this forum just by someone noticing something in a picture.
```

---
## \#5 Posted by: Komamtb Posted at: 2018-07-09T14:59:08.460Z Reads: 100

```
Here it is, I have shortened the vesc wires today from the plug side and tested the board on a single motor each side, the stronger motor doesn't move now! What could've  I do wrong? Vesc seems fine, but can't detect the motor no more.![IMG_20180705_163914|374x500](upload://evzv7amgd4htlI7xpvTmNuOt62J.jpg)
```

---
## \#6 Posted by: Hummie Posted at: 2018-07-09T15:32:55.502Z Reads: 89

```
bet a phase wire either shorted or broke in the motor.  seems to happen a lot with the vibrations on a skateboard
```

---
## \#7 Posted by: Komamtb Posted at: 2018-07-09T16:05:54.252Z Reads: 80

```
So I should open the motor up?
```

---
## \#8 Posted by: kuphjr Posted at: 2018-07-09T16:29:42.221Z Reads: 78

```
I agree with Hummie. What motors are you using?
```

---
## \#9 Posted by: kuphjr Posted at: 2018-07-09T16:31:53.000Z Reads: 76

```
I usually recommend just doing a return. If you bought certain hobbyking motors, I can tell you I always had problems with them shorting because of where the wires entered the motor was sharp.  If you have those motors you are better off just trying to make a return and picking up ones from @torqueboards 

You can't usually return a motor that you have opened up.
```

---
## \#10 Posted by: Hummie Posted at: 2018-07-09T16:35:33.641Z Reads: 74

```
if you open it and close it they wont know.   maybe you can find where the problem is and maybe insulate it.   a multimeter helps
```

---
## \#11 Posted by: Komamtb Posted at: 2018-07-10T13:40:31.894Z Reads: 46

```
Apearantly the motors are fine, both of them work from the same vesc, but the slave one is acting up, the green light is on then I push the throtle, but the motor is still not spining and vesc can't detected it?

Edit I'm using torgue board parts with 6374 motors.
```

---
## \#12 Posted by: sayekim Posted at: 2018-07-10T14:03:05.939Z Reads: 45

```
I’d try restoring the default settings on the slave or reading the settings from the master and then writing those settings to the slave but not before changing the slave id first. 
Afterwards if you can run motor detection on the slave, setup the slave accordingly again ie in your desired settings. 

Don’t forget to always read and then write settings afterwards.
```

---
## \#13 Posted by: Komamtb Posted at: 2018-07-10T14:34:38.569Z Reads: 38

```
New problem started to hapen, on one of the last configuration settings, the motor on the slave starts spining at it's max for now reason, and doesn't stop besides turning the power off, so now i don't know hot to set it?
```

---
## \#14 Posted by: sayekim Posted at: 2018-07-10T14:46:59.738Z Reads: 38

```
I have had this too but unfortunately I don’t remember why it happened. I do know that I played with the settings on the slave to resolve it.
Try going to app settings and return the settings to default.
```

---
## \#15 Posted by: Komamtb Posted at: 2018-07-10T15:56:34.220Z Reads: 36

```
So going back and forth this happened, the motor also was spinning while I was programing the slave vesc, motor started spinning and I saw a little spark and the board shut off, now I also can't turn the other vesc on, my receiver light is blinking, but the LCD is off witch means the bms went to a safe cut off, it usually would go back on reconnecting the LCD but this time it is still off, so now I don't know if it's the bms, the LCD or both of my vescs went dead, @torqueboards could you chip in?![IMG_20180710_185005|374x500](upload://osAdzxnSXQwM7Z3XY6sqdMaTkUP.jpg)

Edit, I have found, that both of mine vescs dvr chips blew out, how could've this happen? Is this my fault?
```

---
## \#16 Posted by: Ishayc Posted at: 2018-07-11T10:52:24.803Z Reads: 17

```
Check for shorts in the phase wire.
Also, If the motors were spinning at full speed on bench, that might have caused the DRV to blow.
```

---
