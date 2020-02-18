# 3 red lights vesc, new board

### Replies: 28 Views: 1990

## \#1 Posted by: trancejunkiexxl Posted at: 2017-05-21T22:25:16.761Z Reads: 180

```
getting a triple red light on initial startup of vesc, had rc control then it vanished so I walked home... i flashed the fw on vesc to 2.54, but still getting a triple red light on initial start, rc control is completely missing, i checked ppm settings but dont know which one will fix whats going on, motor detection test also fails, but before that it was smooth sailing.. now I have to unstrip a motor mount screw, either way I have no power, and when it was working, the motor was spazzing untill wide open throttle..

~Tony
```

---
## \#2 Posted by: Namasaki Posted at: 2017-05-22T02:36:20.277Z Reads: 164

```
3 red blinks is normal at startup on the vesc.
what controller are you using?
any fault codes beside failed motor detection?
```

---
## \#3 Posted by: trancejunkiexxl Posted at: 2017-05-22T03:13:56.405Z Reads: 154

```
no fault codes, no matter how I run the test. generic controller/w reciever say diy_v2c. originally i think it was supposed to be configured for ppm, I lost rc input randomly, so i looked but couldnt find burnt electronics.. motor is really weird though, slow speed doesnt work and clicks and behaves intermittently, while high speed works if i push start.. Board will stay on and vesc has been flashed ok, however no imput.. and motor calibration fail in bldc..<img src="/uploads/db1493/original/3X/9/4/94013f4d474d6da0b5286f1ac67b503d0036fad7.jpg" width="281" height="500">
```

---
## \#4 Posted by: Namasaki Posted at: 2017-05-22T03:24:44.337Z Reads: 131

```
I would have guessed that something wrong with that controller. But I can't figure why motor detection is failing.
did you try motor detection with the remotes receiver disconnected from the vesc?
Maybe a signal from the receiver is messing with the motor detection.
```

---
## \#5 Posted by: trancejunkiexxl Posted at: 2017-05-22T03:35:26.124Z Reads: 133

```
pretty sure the reciever was off, the arrow keys work in the application, so I know the boards got drive power, as I move em the motor spins up, strange, so the diy reciever has 2 options for input leads, one is cn4 and the other is blank.. either way Ive tried both and couldnt get control back, maybe I should flash again, and leave the tx/rx stuff unplugged... the little reciever has a tiny reset button, I will try that in the am, as far as radio transmitting goes do you know how to do the rf initial setup?
```

---
## \#6 Posted by: Namasaki Posted at: 2017-05-22T03:46:36.582Z Reads: 125

```
You should unplug the receiver from the vesc and try the motor detection again.
I don't think you need to flash the vesc firmware.
I don't know what the pairing procedure is for that remote, it should have come with instructions for pairing.
It's beginning to look like the remote is causing all the problems though.
```

---
## \#7 Posted by: trancejunkiexxl Posted at: 2017-05-22T16:21:59.435Z Reads: 109

```
hall sensor detection failed finally showed up, adjusting the current, it kinda spins, but it sounds very sick... =/
having the receiver removed was good advice the detection now works, and the motor spins, it just struggles to get going a bit and there are a string of numbers -1, -1, -1. so on and so forth for the description
```

---
## \#8 Posted by: Namasaki Posted at: 2017-05-22T16:46:43.015Z Reads: 96

```
Try disconnecting the sensors and change Bldc settings to sensorless. 
And do the motor detection again and see how that works.
There could be a problem with the sensor or sensor wires
```

---
## \#9 Posted by: trancejunkiexxl Posted at: 2017-05-22T16:58:56.749Z Reads: 96

```
<img src="/uploads/db1493/original/3X/f/7/f7f6935c9419c360aaee8ee7ef1cb5eb053af3ab.jpg" width="690" height="388">
not exactly sure which sensors i need to dc, would this pic help? I think the board is good now, i just need to get tx up, I would just connect my stuff from another setup but i dont feel like riding with a dx7s around my neck =| Im pretty sure the motor i got now doesnt have a sensor... maybe im wrong..
```

---
## \#10 Posted by: Namasaki Posted at: 2017-05-22T17:34:03.239Z Reads: 91

```
I meant disc the motor Hal sensor. 
If your motor has a Hal sensor, there will be a harness of small wires coming out of the motor with a plug on the end that plugs into a socket on the Vesc. 
If your motor don't have it then just check bldc settings and make sure it's set for non sensored motor.
```

---
## \#11 Posted by: trancejunkiexxl Posted at: 2017-05-22T17:39:42.869Z Reads: 89

```
ya just realized its b/c i dont have that sensor lol, ya i double checked the options it is set to sensorless, It runs good now that the reciever is unplugged, when I plug it in though none of the ppm settings are working unfortunately, and i have no clue how to pair it,
```

---
## \#12 Posted by: trancejunkiexxl Posted at: 2017-05-22T19:16:19.869Z Reads: 91

```
<img src="/uploads/db1493/original/3X/6/2/626d55fa6598c3abb8e1f18021497f51d4ce15fb.jpg" width="281" height="500">

Here is a nice big picture of the diy reciever. I tried finding some information on pairing it, but nothings come up yet.
```

---
## \#13 Posted by: Namasaki Posted at: 2017-05-22T19:56:13.635Z Reads: 77

```
https://www.electric-skateboard.builders/t/benchwheel-pairing-issues/18360/12
```

---
## \#14 Posted by: Namasaki Posted at: 2017-05-22T20:05:00.456Z Reads: 78

```
<img src="/uploads/db1493/original/3X/c/a/ca0a6a5ce15a9d588a310f455fdbd20a7fe357ac.JPG" width="690" height="460">
```

---
## \#15 Posted by: trancejunkiexxl Posted at: 2017-05-22T20:53:58.726Z Reads: 70

```
ya no dice, on any combination of powering esc, holding handtrasmitter power down and with or w/o small white button on rx module down before powering vesc or after powering vesc..
```

---
## \#16 Posted by: Namasaki Posted at: 2017-05-22T20:56:28.485Z Reads: 65

```
Maybe time to try a different remote
```

---
## \#17 Posted by: trancejunkiexxl Posted at: 2017-05-22T21:07:59.731Z Reads: 62

```
if you have any suggestions that can have me rolling in less than 24hours let me know lol!!
```

---
## \#18 Posted by: trancejunkiexxl Posted at: 2017-05-22T21:48:57.622Z Reads: 64

```
<img src="/uploads/db1493/original/3X/b/f/bf5527bbb5515bc81980e336a9fd2ba0cae33cdf.png" width="625" height="235">
would this be ok you think?
```

---
## \#19 Posted by: Namasaki Posted at: 2017-05-22T21:57:00.838Z Reads: 60

```
Thats a nano remote and they are known to have issues just like the one you already have.

Where are you located?
```

---
## \#20 Posted by: trancejunkiexxl Posted at: 2017-05-22T22:05:20.418Z Reads: 59

```
california, not many hobby places close by, i went ahead and ordered one it looks identical to the torque boards, one from the diystore... not very happy to hear about this remote issues though,
```

---
## \#21 Posted by: Namasaki Posted at: 2017-05-22T22:06:59.992Z Reads: 55

```
They have signal drop out  issues and not very good control.
You might want to cancel that order if you can.
I sent you a pm.
I'm in San Diego, CA
```

---
## \#22 Posted by: trancejunkiexxl Posted at: 2017-05-23T15:30:50.477Z Reads: 50

```
thanks for all your help, it seems I have learned a bunch watching a lot of youtube trying to learn Under App config, and PPM tab there is a nifty display check box on bottom that shows when there is registered input from controller. This is IF, the controller is being by BLDC, mine isnt registering so, as you are probably right its time for a new tx/rx
```

---
## \#23 Posted by: trancejunkiexxl Posted at: 2017-05-26T01:14:58.794Z Reads: 49

```
got the new remote in, getting solid green on remote, and solid red on reciever.. still not registering in ppm/appconfig
```

---
## \#24 Posted by: Namasaki Posted at: 2017-05-26T01:27:38.867Z Reads: 45

```
which channel are you plugging the vesc into on the receiver?
```

---
## \#25 Posted by: trancejunkiexxl Posted at: 2017-05-26T02:03:58.987Z Reads: 46

```
<img src="/uploads/db1493/original/3X/3/1/31e03958f1652315be87e84376a11e1abf960ecc.jpg" width="281" height="500">

there are 3 options 

... blank
... ch2
... ch1

i think b/c the way they have it labeled i cant tell which one i need
```

---
## \#26 Posted by: trancejunkiexxl Posted at: 2017-05-26T02:10:57.579Z Reads: 44

```
basically i hooked the vesc servo cable to the rx, and should be g2g as the seller just informed me its autobind?

https://www.youtube.com/watch?v=nUrmKLpR70E

i went through this it looks bind and is solid red, in bldc though display doesnt show input registering
```

---
## \#27 Posted by: trancejunkiexxl Posted at: 2017-05-26T02:12:04.543Z Reads: 44

```
ok so i have board tx power and it moves but its only the low speed setting how do i get my throttle adjusted
```

---
## \#28 Posted by: trancejunkiexxl Posted at: 2017-05-26T02:50:08.420Z Reads: 42

```
thanks man Its a sucess!!!! I really appreciate the help.. for some reason the slow switch setting just spazes the motor out and doesnt really do anything, and the ubec switch that does power wont shut off board =( besides that though, i am very happy with this remote.. i really really wanted a small one for my sweater pocket, boy am I happy, these calibrations can be tough though!
```

---
