# Vesc not spinning up motor on test

### Replies: 18 Views: 1476

## \#1 Posted by: richi Posted at: 2017-11-25T10:19:26.778Z Reads: 93

```
Hello, i have a problem with my first skateboard build, I have a Vesc from ESK8.de (bought on the forum so it's known good) and every time i try to do the motor detection test it twitches the motor and then gives me a failed detection test, 

i'm running 2x 5000mh zippy 3 cells in series and am trying to drive an SK3 285kw turnigy motor, the only thing i've done is replaced the bullet connectors on the vesc  otherwise all is standard.

my min charge cutoff i have had set at 0 and still the same, i've tried the amps up to 12 in the test to no avail also, I have tried another usb cable- same result,

is there anyway to test the motor to see if the problem lies there?
<img src="/uploads/db1493/original/3X/a/a/aab68f869d33694b7eb7d1f1879afad55a71b673.JPG" width="375" height="500"><img src="/uploads/db1493/original/3X/2/1/21d031ae7d6e006bca8c40b378d4119a723c3d6f.JPG" width="375" height="500">
 anyone have any ideas this is killing me! thanks for your time.
```

---
## \#2 Posted by: ARetardedPillow Posted at: 2017-11-25T10:30:52.645Z Reads: 82

```
Okay do you want to die???? The wire on the antispark is exposed and you cannot touch the metal or bad things will happen to you
```

---
## \#3 Posted by: aigenic Posted at: 2017-11-25T10:32:14.882Z Reads: 81

```
First of all, isolate everything...
```

---
## \#4 Posted by: aigenic Posted at: 2017-11-25T10:32:44.321Z Reads: 80

```
Then send us more pictures of your BLDC and circuits, how is everything connected together...
```

---
## \#5 Posted by: ARetardedPillow Posted at: 2017-11-25T10:33:11.625Z Reads: 81

```
Go to terminal and type in "faults" and see if you get anything. 
And how are you placing the motor?
```

---
## \#6 Posted by: FredrikHems Posted at: 2017-11-25T10:38:32.559Z Reads: 80

```
Its just a loop key, you wont get shocked or short anything If you touch it
```

---
## \#7 Posted by: ARetardedPillow Posted at: 2017-11-25T10:39:52.313Z Reads: 78

```
Its still dangerous, theres current going through that thing.
```

---
## \#8 Posted by: FredrikHems Posted at: 2017-11-25T10:41:10.242Z Reads: 77

```
I wont say its dangerous before you expose both the negative and the positive..
```

---
## \#9 Posted by: richi Posted at: 2017-11-25T11:02:41.185Z Reads: 71

```
O.K you're right unisolated anti spark not really good!- fixed!

no faults on the terminal (thanks for that never knew about it)

the motor is only on a mount at the moment as i would like to know it works before putting i on the board

here is my connections,
<img src="/uploads/db1493/original/3X/1/1/11ecab0e544a8b5bc29a09c860caca1ca795f644.JPG" width="375" height="500">

so it's positive from the vesc through the anti spark going to an xt60 going to the battery pack with another leg going to a charging point 
the negative is going direct to the xt60 for thr battery pack and then doubling back to the charge point.

should  i make screen shots from the vesc tool? if so which ones,
many thanks for your speedy replies and help
```

---
## \#10 Posted by: ARetardedPillow Posted at: 2017-11-25T11:24:49.146Z Reads: 68

```
Make sure the motor can spin freely and there is no resistance, and make sure the circlip isnt being held down by the mount.
Take screenshots of the first page when you open vesc tool, and the motor settings (motor detection page)

Edit: Im assuming youre using an sk3?
```

---
## \#11 Posted by: richi Posted at: 2017-11-25T11:38:15.830Z Reads: 70

```
yes it's an SK3, the motor is able to spin freely and the circlip is not obstructed, i'm using the wizard for setup should i do it manually?

<img src="/uploads/db1493/original/3X/7/8/7899d5b50187ef6ffd6a40010155ccee5e970bcc.png" width="690" height="431">

<img src="/uploads/db1493/original/3X/3/7/37e8a443b6acc33594946eb79ef255ebaec2e461.png" width="690" height="431">
```

---
## \#12 Posted by: ARetardedPillow Posted at: 2017-11-25T11:47:50.002Z Reads: 65

```
Hmmm im not experienced with this vesc tool, most people use the other bldc tool
```

---
## \#13 Posted by: ARetardedPillow Posted at: 2017-11-25T11:48:37.011Z Reads: 66

```
Can you post your Bldc settings on the left?
```

---
## \#14 Posted by: richi Posted at: 2017-11-25T11:59:33.989Z Reads: 65

```
should i download the other tool and use that?

<img src="/uploads/db1493/original/3X/1/5/159b6abe5f5be1a6d4d36500dea285dfdb6b6702.png" width="690" height="431">

<img src="/uploads/db1493/original/3X/8/2/8239d47369614058ef08ce6cbf5dbb668c0d81e7.png" width="690" height="431">

<img src="/uploads/db1493/original/3X/e/a/ea276cc7d86ea5dd92e1fef240e8f258b4841faa.png" width="690" height="431">

<img src="/uploads/db1493/original/3X/8/6/86e8ecf18fce61f5807752e719a93f07ecbd25df.png" width="690" height="431">
```

---
## \#15 Posted by: richi Posted at: 2017-11-25T12:01:38.361Z Reads: 61

```
some more settings

<img src="/uploads/db1493/original/3X/1/2/1212acea751e15402856cc85d5ac7c5b4b7a5bbd.png" width="690" height="431">

<img src="/uploads/db1493/original/3X/d/b/dbba5379ebd6108b55dbf3b163ced31b22559f67.png" width="690" height="431">

<img src="/uploads/db1493/original/3X/e/f/ef1cd1c7225e453e0ff4b33a176baabdfcbe8d2d.png" width="690" height="431">
```

---
## \#16 Posted by: richi Posted at: 2017-11-25T12:38:09.913Z Reads: 61

```
Thank you all ever so much for the help, after 10 hours of pulling my hair out i found the problem, when i soldered the new bullets to the vesc i managed to splash a bit of solder onto one of the mosfets causing a bridge, totally my bad, but thanks to another members post i new what  i was looking at as soon as i eventually saw it, so thanks again and happy riding!, i will post some pics as soon as i get this board finished.
```

---
## \#17 Posted by: Namasaki Posted at: 2017-11-30T02:56:16.146Z Reads: 52

```
So did your motor detection pass after fixing the solder bridge?
```

---
## \#18 Posted by: richi Posted at: 2017-12-08T08:24:21.245Z Reads: 45

```
sorry for the late reply, yes it did, today i am finishing my case and themn it will be the final build up (hopefully)!
```

---
