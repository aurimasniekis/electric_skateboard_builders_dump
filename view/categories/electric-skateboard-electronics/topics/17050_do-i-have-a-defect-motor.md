# Do i have a defect motor?

### Replies: 26 Views: 1293

## \#1 Posted by: Philippe1 Posted at: 2017-02-01T20:59:37.260Z Reads: 130

```
is it possible that I have a defect motor? Whenever i try riding it it goed really slow. When it's on the ground and nothing on it it stutters and doesn't move. I have tried to redo my motor detection but it failed. I hope my motor is not defect because i live in europe and i bought it from DIYelectricskateboards.

here are some pictures of my setting on BLDC
<img src="/uploads/db1493/original/3X/1/1/11ff439391b3d06e078ad745141d5501405d31f6.png" width="690" height="431"><img src="/uploads/db1493/original/3X/c/8/c8164e8bcab0baada2f0713f5ba5aa78405bb646.png" width="690" height="431"><img src="/uploads/db1493/original/3X/5/c/5cbb5fac2d0e21317c4a5ad1312785be2e51be1e.png" width="690" height="431"><img src="/uploads/db1493/original/3X/a/5/a5e7f051fe42a350d352d9a72ba32cd52dd5c7cc.png" width="690" height="431">

I also have a video of my riding it on full thortlle: [here](https://www.youtube.com/watch?v=-hVb-UtkaZY)

I also have a video of my setup and my motor running on full throttle on the ground: [Here](https://youtu.be/9P4KCoh5h6s)

Thank you so much for looking at my request! i hope that you can help me😁😁😁
```

---
## \#2 Posted by: Hummie Posted at: 2017-02-01T21:06:06.384Z Reads: 104

```
defective motor?  if it fails the bldc test most likely.  have you tried opening it and seeing if the phase wires are insulated from the housing or each other.  
you could also use an inductance meter for 15$ to check each phase or maybe if you get a really accurate resistance meter it will show up.  the inductance meter and resistance meter on the vesc foc program test are really good and you might still be able to get some results from that.
```

---
## \#3 Posted by: torqueboards Posted at: 2017-02-02T00:57:42.149Z Reads: 93

```
It was working and then it stopped working? What voltage are you running? A failed detection could be the wrong battery cut off settings. Bad soldered motor wires. Did you check the faults?
```

---
## \#4 Posted by: Philippe1 Posted at: 2017-02-02T18:29:14.946Z Reads: 82

```
Well it was always like this so it never was working. I am running 33.3 volts so that is 9s. I don't know what you mean with the faults
```

---
## \#5 Posted by: torqueboards Posted at: 2017-02-02T18:50:48.739Z Reads: 77

```
You'll want to explain more of your setup. Motor, battery setup, etc. Photos..

Can't really troubleshoot your issue if you give no info :/
```

---
## \#6 Posted by: Philippe1 Posted at: 2017-02-02T18:51:45.178Z Reads: 73

```
of what do you need pictures?
```

---
## \#7 Posted by: torqueboards Posted at: 2017-02-02T18:54:07.186Z Reads: 71

```
You'll want to explain more of your setup. Motor, battery setup, etc. Photos..
```

---
## \#8 Posted by: Philippe1 Posted at: 2017-02-02T19:04:14.212Z Reads: 69

```
i have 3 9s battery's from zippy flightmax. Each 5000 mah and 11.1 volts. I have thos 3 batterys connected in series to my vesc. The vesc is a VESC BLDC Speed Controller that i got from DIYelectricskateboards.com. My motor is a Electric Skateboard Motor 6355 190KV also from DIYelectricskateboards.com. I also have a TorqueBoards 2.4ghz Nano Remote Controller. 
That's all i guess. I have a [link](https://www.youtube.com/watch?v=9P4KCoh5h6s&feature=youtu.be) here that leads to a video of my setup
```

---
## \#9 Posted by: torqueboards Posted at: 2017-02-03T02:22:12.642Z Reads: 61

```
so your running 9S? You might have to adjust your battery cut off start & stop settings.

Usually, I would do

9S (9) * 3.6v = 32.4v
9S (9) * 3.3v = 29.7v

See if that fixes your issue.
```

---
## \#10 Posted by: Philippe1 Posted at: 2017-02-03T18:29:37.199Z Reads: 51

```
changed it but it did not work
```

---
## \#11 Posted by: psychotiller Posted at: 2017-02-03T18:49:49.561Z Reads: 50

```
Sounds to me like you are actually running three 3s batteries in parallel (not series) for a total of 11v. That would be really slow. Also you should make sure your motor connections are solid
```

---
## \#12 Posted by: Ackmaniac Posted at: 2017-02-03T19:05:24.054Z Reads: 45

```
Have a look in the realtime tab. Activate the sampling and tell us the Battery Voltage that you see there.

<img src="/uploads/db1493/original/3X/d/b/db7e100d5044682519fef87b1f67843183966aba.png" width="690" height="464">
```

---
## \#13 Posted by: sl33py Posted at: 2017-02-03T19:13:56.020Z Reads: 44

```
Please show us a pic or video (if video - more light so we can see clearly).

Specifically of your battery connections - how they are connected so we can validate if it's in parallel or series.

It would be good to also see pictures of your connectors - as close as possible and use flash if needed so it's clear.  Looking for good soldering if you made your own connectors or replaced battery connectors.

Plus the above suggestions on VESC BLDC settings.

What's your gearing?  Motor gear # teeth, and Wheel gear # teeth?

HTH - GL!
```

---
## \#14 Posted by: Philippe1 Posted at: 2017-02-04T10:13:12.326Z Reads: 38

```
<img src="/uploads/db1493/original/3X/1/7/17301bbafeee623c1a57693997098046079640b8.png" width="690" height="431"> This is what it shows
```

---
## \#15 Posted by: Philippe1 Posted at: 2017-02-04T10:33:17.267Z Reads: 39

```
Here are some pictures of my connections
<img src="/uploads/db1493/original/3X/5/f/5f03942b52b8b029f2a3f974bd9875f2ec0b7bee.JPG" width="666" height="500"><img src="/uploads/db1493/original/3X/1/0/101df7482f2370fcef1c6cc85ad0bfe4aaf44cd4.JPG" width="666" height="500"><img src="/uploads/db1493/original/3X/9/a/9ab4318c4d30789eb327ee9f1d9be1e1381817e0.JPG" width="375" height="500"><img src="/uploads/db1493/original/3X/4/3/43114f7b6abaa15c223ca1602769bd00bdd1541d.JPG" width="666" height="500">
<img src="/uploads/db1493/original/3X/d/a/da4964b6fcec8e9215bb8bd19fb0e810255775d7.JPG" width="375" height="500">
<img src="/uploads/db1493/original/3X/a/a/aa1efc51ba8649482e8939eddaec5a2f8e51a9d0.JPG" width="666" height="500">
<img src="/uploads/db1493/original/3X/7/f/7f90c09d6c94f4841b6c41caff7d493d05f3ea8a.JPG" width="666" height="500">
<img src="/uploads/db1493/original/3X/1/6/1681941186778227242b93a6b6e423cb72b55124.JPG" width="666" height="500">
<img src="/uploads/db1493/original/3X/8/e/8e103814f38436f50e5aa143427b524574919108.JPG" width="666" height="500">
<img src="/uploads/db1493/original/3X/3/8/383450f6a27a1d5dddcc49ea792900c7473f9634.JPG" width="666" height="500">

Here is the connection of the motor wires:
<img src="/uploads/db1493/original/3X/f/3/f3c210bef5954b0194c7772834639fcd2463614b.JPG" width="375" height="500">

here are some pictures of the motor:
The wheel pulley has 36t
the motor pulley has 16t
265mm 12mm width belt
<img src="/uploads/db1493/original/3X/b/7/b71dda2451132a5b4883218cb50a0ed3b85a9b68.JPG" width="666" height="500"><img src="/uploads/db1493/original/3X/b/4/b48347136ed9382f77bd7686376e2dcac1f5d006.JPG" width="666" height="500"><img src="/uploads/db1493/original/3X/7/a/7a6c9ff65f17a6a98027f1ef39e135be4fbf2e20.JPG" width="666" height="500"><img src="/uploads/db1493/original/3X/a/6/a61c1e994ce26c01f57722d45cf3f6e3287c4eb9.JPG" width="375" height="500">
```

---
## \#16 Posted by: Ackmaniac Posted at: 2017-02-04T10:39:13.095Z Reads: 38

```
Charge your battery. The voltage of 28.7V is below the cutoff voltage.
```

---
## \#17 Posted by: Philippe1 Posted at: 2017-02-04T11:00:08.248Z Reads: 38

```
what happens then if it is below the cutoff voltage?
```

---
## \#18 Posted by: Ackmaniac Posted at: 2017-02-04T11:43:52.167Z Reads: 38

```
The VESC shuts off the power to protect the battery. So your battery is empty. Just charge it and then try it again.
```

---
## \#19 Posted by: Philippe1 Posted at: 2017-02-04T14:18:17.335Z Reads: 38

```
<img src="/uploads/db1493/original/3X/3/e/3e27bd62669cd34508e6fed8d9c5e08ca0bd325c.png" width="690" height="431">This is what it should look like right.
But now it goes extreemly fast. How do i make it go slower?
```

---
## \#20 Posted by: Hummie Posted at: 2017-02-04T16:18:06.427Z Reads: 37

```
Try riding now
```

---
## \#21 Posted by: sl33py Posted at: 2017-02-04T23:01:35.286Z Reads: 35

```
[quote="Philippe1, post:19, topic:17050"]
But now it goes extreemly fast. How do i make it go slower?
[/quote]


Great!  You just need to be gentle on the throttle.  It will go "extremely" fast under no load - get out and ride and you'll see how you can adjust speed with the throttle.  Be careful - wear protective gear!

GL!
```

---
## \#22 Posted by: Philippe1 Posted at: 2017-02-05T11:03:39.157Z Reads: 28

```
So does this mean that when the battery is lower then my cutoff voltage i cannot ride my board anymore. I need to recharge the battery's again?
```

---
## \#23 Posted by: Ackmaniac Posted at: 2017-02-05T11:06:50.777Z Reads: 28

```
Correct. I guess you think that when a battery is charged to 37.8 V that you can discharge it till 0V. But a LiPo battey is already empty at 3.3 V a cell ( 29.7 V for 9S).
You chould read some background information about Lipo and Li-ion Batterys.
```

---
## \#24 Posted by: Philippe1 Posted at: 2017-02-05T11:10:01.443Z Reads: 25

```
About how much riding time would i get then?
```

---
## \#25 Posted by: Ackmaniac Posted at: 2017-02-05T11:49:06.087Z Reads: 24

```
You can calculate 3.7V a cell * 9S * 5Ah battery = 166.5 Wh. And for each kilometer you need between 10 - 12 Wh on average. So you will get around 15 km.
```

---
## \#26 Posted by: Philippe1 Posted at: 2017-02-05T14:19:23.933Z Reads: 21

```
Thank you all so much for helping me!
```

---
