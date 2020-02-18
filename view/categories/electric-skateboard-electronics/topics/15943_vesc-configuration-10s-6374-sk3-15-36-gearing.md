# Vesc configuration (10s, 6374 sk3, 15/36 gearing)

### Replies: 50 Views: 3670

## \#1 Posted by: laikiux Posted at: 2017-01-12T13:27:10.249Z Reads: 387

```
Hello,
Maybe you have some suggestions on some of the limits?
My setup:
10s, sk3 6374, 16/36 gearing, 80mm wheels
<img src="/uploads/db1493/original/3X/d/d/dd1d5fb8928e9b3e54ca802d6b1e407f4370f170.png" width="690" height="494">
<img src="/uploads/db1493/original/3X/8/d/8dcbec6c7769a163df4b435f63c8033de4d052d8.png" width="690" height="493"> I'm totally confused with ERPM limits.
```

---
## \#2 Posted by: Ackmaniac Posted at: 2017-01-12T13:47:36.295Z Reads: 359

```
Set the maximum input voltage to 57V (don't ask).
If you have a Li-Ion Battery set the battery cutoff start to 30 and the cutoff end to 28 and if you have a Lipo Battery set the  cutoff start to 36 and the cutoff end to 34. Or more aggressive to 35 and 33. If you want more power at lower speeds set the motor max to 70 or 80.
The ERPM limit should be set to 60000 and -60000. But with a 12S you won't reach those speeds. But with 60000 you are on the safe side.
Everything else looks good if you have a single drive.
```

---
## \#3 Posted by: Ackmaniac Posted at: 2017-01-12T13:49:04.233Z Reads: 356

```
Also post screenshots of the advanced tap and your remote (application) settings
```

---
## \#4 Posted by: laikiux Posted at: 2017-01-12T14:31:15.533Z Reads: 343

```
<img src="/uploads/db1493/original/3X/4/c/4c0c96789b9b8ead83b4f833b7ceec0b0962fe28.png" width="690" height="483"><img src="/uploads/db1493/original/3X/6/3/6360450ac46a5241a1fccba8e198408bd2d2c329.png" width="690" height="467">
```

---
## \#5 Posted by: Ackmaniac Posted at: 2017-01-12T14:33:48.595Z Reads: 291

```
If you have a single drive disable the "Send status over CAN" in the General Tab. If you have dual only activate it for the slave when the two VESCs are connected via CAN.

Please also post the PPM Tab
```

---
## \#6 Posted by: laikiux Posted at: 2017-01-12T14:36:29.294Z Reads: 291

```
Thank you. So everything else is ok.
But I have not understood you. 
[quote="Ackmaniac, post:5, topic:15943, full:true"]
The ERPM limit should be set to 60000 and -60000. But with a 12S you won't reach those speeds. But with 60000 you are on the safe side.
[/quote]
I'm running 10s, not 12s
```

---
## \#7 Posted by: Ackmaniac Posted at: 2017-01-12T14:39:51.330Z Reads: 280

```
Sorry i meant with 10S you won't reach those speeds as long as your motors kv is not higher than 190kv. With 12S you could only reach it on the bench but not when you ride it. Set it to max 60000 and min -60000 and you will be safe.
```

---
## \#8 Posted by: laikiux Posted at: 2017-01-12T14:47:13.742Z Reads: 271

```
I have one more question.
Batt min (regen) and Moter min (regen) is not too high?
```

---
## \#9 Posted by: Ackmaniac Posted at: 2017-01-12T14:57:17.810Z Reads: 269

```
What battery do you have and do you have 2 motors or only 1?
```

---
## \#10 Posted by: laikiux Posted at: 2017-01-12T15:06:10.432Z Reads: 271

```
1 motor.
10s3p Li-ion batt
```

---
## \#11 Posted by: Ackmaniac Posted at: 2017-01-12T15:07:42.629Z Reads: 262

```
-12 battery min is fine.
-40 motor min also. If you want more brake power you can raise the motor min to even -80. You need to find out by yourself what suites you. I have -60 on my single.

And if you like to have more power then you can go up to 80 motor max and 60 battery max. But that is already a lot for your belts.
```

---
## \#12 Posted by: Ackmaniac Posted at: 2017-01-12T15:09:59.763Z Reads: 252

```
You can sumarize it to 
Motor Max = Power at low speed
Battery Max = Total Power or Power at high speed
Motor Min = Brake power at mid to low speed
Battery Min = Brake power at high speed
```

---
## \#13 Posted by: treenutter Posted at: 2017-01-12T15:11:30.026Z Reads: 250

```
[quote="Ackmaniac, post:12, topic:15943, full:true"]
You can sumarize it to Motor Max = Power at low speedBattery Max = Total Power or Power at high speedMotor Min = Brake power at mid to low speedBattery Min = Brake power at high speed
[/quote]


@Ackmaniac That's a great summary it took me a lot of trial and error to sort these values out when I got my first VESC!
```

---
## \#14 Posted by: florensvb Posted at: 2017-10-09T09:07:23.407Z Reads: 198

```
Sorry for jumping in on this thread :D 

Lets say i have a 10s2p with Samsung 30Q cells ... They have a discharge of 15A (some may say 20A). Does that mean for me that I should not set my Motor Max, Min and Battery Max to more than 30A (or 40A)?

Cheers!
```

---
## \#15 Posted by: michichopf Posted at: 2017-10-16T12:24:09.087Z Reads: 186

```
Have the same pack and run it with a 6734 singel on my commuter board.

got those values atm:

Motor Max: 50a
Batt max: 40a
Motor min: -50a (this is purely how you want the brakes to feel)
```

---
## \#16 Posted by: florensvb Posted at: 2017-10-16T13:39:44.342Z Reads: 183

```
Hey @michichopf,

what i don't quite understand is that if you limit your Battery Max to 40A, the Motor Max will never exceed the 40A right? Even though its set to 50A? Those two values should act like a bottle neck to each other right?
```

---
## \#17 Posted by: michichopf Posted at: 2017-10-16T14:03:45.011Z Reads: 181

```
well as far as I would say it and take that with a gran of salt:
you wont ever max out your motor a at higher speeds, thats mostly for acceleration at lower speeds. So motor max is more how much he can pull for start up and acceleration.

your Battery A is more of a bottleneck how much the set up can draw during higher speeds ( top speed).

So I usually played around with settings on the safer side, then I asked poeple who ran the same setup with expertise in the vesc area and copied theirs. I am more of a rider (downhill/esk8) than I am a builder, grabted I did few DIY but allways sought after confirmation from better informed individuals. sorry .(
```

---
## \#18 Posted by: florensvb Posted at: 2017-10-16T14:15:14.748Z Reads: 176

```
But so just hypothetically assuming youd go full acceleration at very low speed, it would try to pull 50A for your 10S2P but I am hoping that the Battery Max will prevent it from actually drawing that much, as it would damage the batteries .... ?
```

---
## \#19 Posted by: michichopf Posted at: 2017-10-16T14:46:59.635Z Reads: 173

```
pretty much, also got a fuse between the battery and the vesc, in all of my builds actually.
```

---
## \#20 Posted by: florensvb Posted at: 2017-10-16T15:03:38.524Z Reads: 184

```
So youre thinking it might actually draw 50A even though the Battery Max is set to 40A? Thats quite frightening :D
```

---
## \#21 Posted by: SORRENTINO Posted at: 2017-10-16T15:04:57.990Z Reads: 182

```
Motor amps can be higher then battery amps during certain situations. If you set your battery max to 40amps the max amps that can be pulled from battery is 40amps.There are many times on my single drive ( 10s_6374_16/36_83mm wheels ) when my battery is pulling lower amps then what my motor is pulling. Here is an example. You can see the motor is pulling more amps then the battery. This is 40amps max battery and I think 50 or 60 amps max motor ( 1500w max settings in ack software)

https://youtu.be/hSZ04eYgT04

<img src="/uploads/db1493/original/3X/e/3/e33f9f7c121dd9007d96c05a455501f8cb7c02e6.png" width="243" height="500">
```

---
## \#22 Posted by: SORRENTINO Posted at: 2017-10-16T15:05:59.650Z Reads: 162

```
You set you battery max to 40amps the vesc should never hypothetically go over 40 amps with battery.
```

---
## \#23 Posted by: florensvb Posted at: 2017-10-16T15:06:52.457Z Reads: 159

```
OK. So please can someone explain to me how the Motor can draw more current than the Battery is delivering? I guess that is where I am confused. I must be fundamentally misunderstanding some of the concepts here :D
```

---
## \#24 Posted by: SORRENTINO Posted at: 2017-10-16T15:10:50.225Z Reads: 158

```
http://www.electric-skateboard.builders/t/motor-draws-more-current-than-the-battery-supplies-free-energy/30006
```

---
## \#25 Posted by: SORRENTINO Posted at: 2017-10-16T15:11:41.298Z Reads: 157

```
Jinra sums it up on first comment.
```

---
## \#26 Posted by: florensvb Posted at: 2017-10-16T15:19:19.353Z Reads: 157

```
Alright thank you!! Also good to know that the vesc will never actually pull more from the battery than specified
```

---
## \#27 Posted by: Colson003 Posted at: 2017-10-19T06:06:56.130Z Reads: 151

```
If my motor is max rated at 50a can I do more than (I guess technically less than) -50a? Say -60a?
```

---
## \#28 Posted by: y.k Posted at: 2018-11-11T20:54:10.942Z Reads: 100

```
hi.in ppm part app configuration in i dont know what to choose . i want my eborad go front and goback. what is disabled and curentt with no reverse with braking and … . i dont know what to choose.
```

---
## \#29 Posted by: y.k Posted at: 2018-11-11T20:59:03.905Z Reads: 102

```
my battery is 8s2p 2600ma every each battery. i need the min battery
(regen) and max battry.
thanks
```

---
## \#30 Posted by: Ackmaniac Posted at: 2018-11-12T10:34:54.616Z Reads: 99

```
8S2P seems to be very small. Is it a Lipo or a Li-Ion battery and do you have a dual or single setup?
```

---
## \#31 Posted by: y.k Posted at: 2018-11-12T15:22:19.452Z Reads: 100

```
my single motor is 220kv sensorless alien power 2200w with 8s2p li ion(LG) pack.
i want to help me
1.what i put in battery max and battery min?
2.i want my eboard would have Reverse and i do not know to choose DISABLED or CURRENT?
```

---
## \#32 Posted by: Ackmaniac Posted at: 2018-11-12T21:03:02.029Z Reads: 96

```
Which battery pack do you have exactly. There are too many different cells available.
```

---
## \#33 Posted by: y.k Posted at: 2018-11-13T09:13:18.422Z Reads: 91

```
i sen them to you in private
```

---
## \#34 Posted by: y.k Posted at: 2018-11-13T09:15:54.475Z Reads: 94

```
[
4m](https://www.electric-skateboard.builders/t/vesc/74540?u=y.k)

hi. my battery is
IT IS LGABB41865
Q058B277AD
2600MA
```

---
## \#35 Posted by: y.k Posted at: 2018-11-15T09:56:55.749Z Reads: 87

```
hi bro.could you answer to my 2 question?
```

---
## \#36 Posted by: Ackmaniac Posted at: 2018-11-15T21:31:59.115Z Reads: 84

```
Your battery is rated for 5A max discharge and 2.5A max continuous charge. I mostly go 50 higher in charge current. So you can use 10A max battery and 7.5A min battery.
Not really great. So finally you have the wrong battery in i too small configuration.
```

---
## \#37 Posted by: y.k Posted at: 2018-11-21T21:41:54.778Z Reads: 81

```
8×2600=20080ma
20080×25c= is this true?
```

---
## \#38 Posted by: Ackmaniac Posted at: 2018-11-22T22:32:47.131Z Reads: 81

```
It's 2x2600ma=5200ma. The battery's in series only increase the voltage but not the A.
```

---
## \#39 Posted by: y.k Posted at: 2018-11-24T05:57:51.819Z Reads: 78

```
i found out the batteries C is 5. i wanna put the max amper at 20 how do you think,? would there be any problem? and the min at-10?
```

---
## \#40 Posted by: y.k Posted at: 2018-12-11T18:12:28.744Z Reads: 70

```
hii plugged in every thing and clicked on the connect part on BLDCtools program  but it says Not connected. what sould i do bro?
```

---
## \#41 Posted by: Ackmaniac Posted at: 2018-12-12T00:09:45.126Z Reads: 65

```
Did you power the VESC by a battery and did you select the right COM port?
```

---
## \#42 Posted by: briman05 Posted at: 2018-12-12T00:21:17.811Z Reads: 61

```
Where did you get the micro usb as some are only for charging you need one that has the ability to transfer data. A ps4 cable for a controller is perfect for it.
```

---
## \#43 Posted by: y.k Posted at: 2018-12-12T08:58:01.741Z Reads: 55

```
maytech cable. cable is fabric.
```

---
## \#44 Posted by: y.k Posted at: 2018-12-12T09:23:11.759Z Reads: 53

```
there is only one way of usb in the vesc. the erorr is code29 of usb
```

---
## \#45 Posted by: briman05 Posted at: 2018-12-12T14:43:31.315Z Reads: 53

```
I would try a different usb cable
```

---
## \#46 Posted by: y.k Posted at: 2018-12-13T06:54:02.426Z Reads: 49

```
i tryed 3 diffrent cables
```

---
## \#47 Posted by: briman05 Posted at: 2018-12-13T12:38:07.950Z Reads: 48

```
It has to be a certain cable it has to be able to transmit data. Where the cables you happen to use phone charging cables
```

---
## \#48 Posted by: y.k Posted at: 2018-12-16T06:56:08.319Z Reads: 42

```


hi sorry again dude. i configured it but there is a problem.when i pushed back the jowstick the motor doesnot rotate back.

Reply

 Invite  Archive  Reply

Watching

You will receive notifications because you created this topic.

 Quo
```

---
## \#49 Posted by: Acidfie Posted at: 2019-03-18T21:02:13.332Z Reads: 27

```
sorry for digging out,

my brakes are really weak at high speeds, when im like going 45 - 60 km/h. I have a **12S4P w/ 30Q**. Afaik the max. charge for these types is: 3A, so splitted up to 2 VESC (dual) it would be around 6A battery min per VESC. I have it around -7.5a for each one, totaling 15A. How "bad" can it be raising these numbers to, lets say about 10 or even 15A per VESC to get more braking power (really ned it, im relatively heavy with 90kg mass)? 
Since the charging is not continuously, the battery's should not get damaged, or am i wrong?
```

---
## \#50 Posted by: Ackmaniac Posted at: 2019-03-18T21:32:56.275Z Reads: 24

```
I have 12S4P 30q as well and I use - 12A on each vesc. Cells are rated for 4A max continuous charge but I also think that short burst will not harm them. But I am not a battery engineer. But better the battery's die than me.
```

---
