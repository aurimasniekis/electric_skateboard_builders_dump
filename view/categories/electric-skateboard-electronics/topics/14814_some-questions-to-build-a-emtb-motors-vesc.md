# Some questions to build a EMTB (motors, vesc)

### Replies: 23 Views: 2387

## \#1 Posted by: tueboard Posted at: 2016-12-17T03:05:45.919Z Reads: 138

```
hi,

1- i've two 300kv maytech motors from scramboards, something that worries me is the length of cables, the large ones are from the motor, and the short one is the sensor lead, this is safe?

<img src="/uploads/db1493/original/3X/0/e/0ea73f7c7a3a7c095ce868afb060af6dbe3280e9.jpg" width="666" height="500">

2- if i want to build a all terrain board, should i use the sensor lead? there is any advantage than running the motor as sensorless?

3- it's possible to connect the sensor lead to the Enertion's VESC?

4- i've another ESC FVT 120A, 2-6S LIPO SBEC 3A/6V with a sensor port, it's better to use two of these than two VESC ?

<img src="/uploads/db1493/original/3X/6/0/60d673d4d2018e9c1a6d758d8a307ef22105d816.jpg" width="666" height="500">

5- all the EMTB boards I've seen, are using two boxes one for the 2 ESCs and another for the batteries,  if my motor cables are so large i can use only one box in the middle of the board? if this is a bad idea why?

<img src="/uploads/db1493/original/3X/8/7/874ae1f8cfc6bd340102a5b476912e24f86b620b.png" width="690" height="345">

6- if the motors have 300kv i need special settings on the VESC? (motor max, etc..)
<img src="/uploads/db1493/original/3X/c/4/c423666faff3896c4cec9c939afce2d2e465ac14.png" width="690" height="298">

thank you!
```

---
## \#2 Posted by: BoardSportsRN Posted at: 2016-12-17T03:18:11.388Z Reads: 124

```
<p>This post was flagged by the community and is temporarily hidden.</p>
```

---
## \#4 Posted by: tueboard Posted at: 2016-12-17T03:25:00.555Z Reads: 121

```
the  full boards from scramboards looks like they use two 300kv motors and two VESC
https://www.scramboards.com/es-scram-board-2wd.html
```

---
## \#5 Posted by: BoardSportsRN Posted at: 2016-12-17T05:11:45.101Z Reads: 115

```
<p>This post was flagged by the community and is temporarily hidden.</p>
```

---
## \#6 Posted by: Okami Posted at: 2017-01-09T21:48:02.290Z Reads: 102

```
Hi! Any progress?

I've seen some high kv motors on the ES forum, I think the guy ran 280kv or so motor.. with high ratio (1:6 or so).. and he was doing fine :slight_smile:

Though, you should check how much vesc is compatible with that kv rating and your voltage.. might hit that erpm limit everyone is talking about :)
```

---
## \#7 Posted by: tueboard Posted at: 2017-01-09T23:25:00.681Z Reads: 95

```
hi,

- i limited the VESC's erpm to 60.000 and the motor max to 60A.

- i'm running the motors in BLDC mode, i would like the FOC mode but I don't want to fry the 2 VESCs.

- i'm using 2 lipos Floureon 6S 22.2V 8000mAh 35C each one, I don't have any problems running at 12S.

- I've tried the FVT ESC at 12S 44.4v and fried it, i learnt by the hard way the max is 6s...

- i realize that i have much less range than my street eboard (30km) vs eMTB (3-4km), i would like to try 190kv motors if this can improve the range and torque, any idea?
```

---
## \#8 Posted by: Okami Posted at: 2017-01-09T23:31:10.200Z Reads: 91

```
Wait.. so how many kilometers can u do with emtb? 4km versus 30km sounds terrible.. maybe you made a typo.. 14km might seem ok (even good) with 8000mah battery

3.7 x 12 x 8 = 355wh
So even at nominal capacity and 20wh consumtion, u should be able to go around 17km i think or so.

Unless u ride really fast and consume 40wh :)
```

---
## \#9 Posted by: zmoney Posted at: 2017-01-09T23:49:50.500Z Reads: 87

```
I had an email from someone that had their VESC die because of that configuration
```

---
## \#10 Posted by: JohnnyMeduse Posted at: 2017-01-10T00:11:04.712Z Reads: 87

```
You need to limit the max erpm at around 60000 to 70000 to avoid any problem. 😉
```

---
## \#11 Posted by: Ackmaniac Posted at: 2017-01-10T00:52:04.973Z Reads: 88

```
@tueboard what are your battery cutoff start and end? Because 10 times less range doesn't make sense.
```

---
## \#12 Posted by: tueboard Posted at: 2017-01-10T09:04:21.819Z Reads: 88

```
@Okami @Ackmaniac lamentably, is not a typo :(

i'm running the lipos at 12s, 44.4v to get more power.

here is the config of each VESC, do you see anything bad?
 <img src="/uploads/db1493/original/3X/f/b/fb0171db8c6daecce3084018ad8f2222bf495ef7.png" width="690" height="348">

maybe the reason is that i'm using two 300kv motors on eMTB and just a single 190kv motor on streetboard ?

thanks all for your comments!
```

---
## \#13 Posted by: Ackmaniac Posted at: 2017-01-10T10:00:49.625Z Reads: 85

```
300kv with which gearing and wheel size.
```

---
## \#14 Posted by: tueboard Posted at: 2017-01-10T14:18:43.029Z Reads: 85

```
@Ackmaniac 

wheel size: 8 inch - 20,32 cm
belt: 5M-415
belt teeth: 73
belt width: 15 mm
motor cog teeth: 12
wheel drive gear teeth: 72
```

---
## \#15 Posted by: DilatedPupils Posted at: 2017-01-10T14:42:41.618Z Reads: 86

```
4km range is ridiculously low.
Your low voltage cuttoff seems high.
How much do you charge your lipos?
```

---
## \#16 Posted by: Ackmaniac Posted at: 2017-01-10T14:56:19.132Z Reads: 82

```
You are lossing already 43% of your performance because of the too high kv. Because 300kv at 12S is good for 105840 ERPM. But the limit is 60000 ERPM. Your topspeed at 60000 is 54,7 km/h. 
In theory your gering at 12S would be capable of 96 km/h if there wouldn't be the 60000 limit. So i would recommend to get other motors. 190kv should be fine.
```

---
## \#17 Posted by: tueboard Posted at: 2017-01-10T16:00:48.728Z Reads: 82

```
what cutoff do you recommend me?

i charge the lipos upto 4.19 each cell
```

---
## \#18 Posted by: tueboard Posted at: 2017-01-10T16:02:07.760Z Reads: 80

```
thank you, maybe i will get some sk3
```

---
## \#19 Posted by: Ackmaniac Posted at: 2017-01-10T16:31:40.881Z Reads: 78

```
Normally for Lipos i would recommend 3,6v cutoff start and 3,4V cutof end. But i think 3,5 and 3,3 is also fine. Depends a bit on the Lipos and once you realize the VESC reduces the power because of those limits you should try to stop your ride. With Li-Ion you can continue longer because lipos kind of collapse if you discharge them too low.
```

---
## \#20 Posted by: DilatedPupils Posted at: 2017-01-10T20:48:52.440Z Reads: 74

```
I have my cutoff at 3.6 - 3.4
I charge my 12s 8000 mah to 4.15 and I get over 8 miles on my Trampa, sk3 149kv with 1:6 chain drive
```

---
## \#21 Posted by: Aggdaddy Posted at: 2017-01-11T04:08:44.362Z Reads: 76

```
I have those motors from scramboards.  They were included in a complete MTB from scramboards.  I used 2 vescs from Flier ESC in china.  They come with heatsink.  Worked good once I got them configured.  A little slow on take off, but scary fast (to me anyway) once you get beyond 20mph.  When it was up to 26mph, the motors still had quite a bit of punch.  That was faster than I wanted to go.

Cables being that long doesn't seem to be an issue.  I am using one box in the middle with battery and ESC in the same box.  I think if I was going to build a new E-MTB, I would go for two separate boxes.  I would feel more comfortable having the battery separate from the ESC's.  Just from seeing that video of "jens?" torturing his board and the esc caught fire, but it was separate from the battery.

I got about 35 miles in that configuration.  Then one day I was going to do an errand and one of my wheels wouldn't spin.  I had a failure on one of the vescs.   Motors are still strong, but, using a 10s battery and 300KV motor, it eventually killed the vesc.   The vesc no longer responds. Can't read the logs or anything.

I have removed the last vesc and replaced with a dual ESC.  Flier ESC sent me a replacement VESC with little question.  Doesn't seem like there are any issues with high KV motors with the dual ESC.  It runs the motors pretty strong.  Much stronger acceleration than the vesc.  Brakes are literally killer.  Like, they will lock up if you barely touch the trigger in the default config.  I have toned them down, but haven't had much time to get a feel for the new esc.  Just rode it for 15 minutes today to test the configuration.
```

---
## \#22 Posted by: Okami Posted at: 2017-01-11T11:52:58.164Z Reads: 74

```
@Aggdaddy Im not sure is it the same flier esc but it could be the same one, for which there is "firmware floating around the web" and this firmware has better brakes for these esc's. 

Are they red or gold in color with a heatsink capable of 12s?

Take a look at this:

http://www.electric-skateboard.builders/t/efx3-trampa-holypro-35-esc-fvt-120a-tunigy-sk3-6374-149kv-lipo-16ah-8s/14305/36
```

---
## \#23 Posted by: Aggdaddy Posted at: 2017-01-11T15:10:44.931Z Reads: 69

```
Heatsink is silver.  Heatshrink is yellow.  Not quite the same..  I think this is the model.  
http://www.fliermodel.com/en/prc-show.asp?id=681
Style：
F-8S-120A-S

I've had the dual ESC for a few weeks, but I just received the USB cable to make modifications to it yesterday.  I changed the brakes to ABS 50%   it made the e-MTB much more managable, but I'm still a little hesitant to do any speed on it.  I got thrown off literally the first time I rode the e-MTB with the dual ESC.  I'm gonna bump it up to ABS 75% to see if that'll give me a comfort zone I can live with.  50% ABS, is still a little touchy.

I looked at the thread for the ESC FVT 120A, looks similar, but mine is two esc's under one heatsink.  

<img src="/uploads/db1493/original/3X/3/f/3f8d6d4fbdd0744201654f05369ac59ac4d06589.jpg" width="377" height="499">
```

---
## \#24 Posted by: tueboard Posted at: 2017-01-25T20:23:26.852Z Reads: 60

```
hi,

i need some help, i want to change the two 300kv motors to a lower ones because my range is so bad right now and they are very noisy.

i'm considering two options:
sk3 6374-149kv
sk3 6374-192kv

i want:
- stick with two VESCS.
- reach 25-30km/h it's enought for me.
- get the lower motor noise as posible.
- but the most important is to get the most range as posible.

which motor is the best for me 149kv or 192kv?

my gearing
wheel size: 8 inch - 20,32 cm
belt: 5M-415
belt teeth: 73
belt width: 15 mm
motor cog teeth: 12
wheel drive gear teeth: 72

thank you
```

---
