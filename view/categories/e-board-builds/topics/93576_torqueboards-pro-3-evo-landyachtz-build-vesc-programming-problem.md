# Torqueboards PRO 3 &#124;EVO Landyachtz build &#124; VESC programming problem

### Replies: 12 Views: 275

## \#1 Posted by: G8dsent Posted at: 2019-05-12T15:47:51.674Z Reads: 102

```
Hi guys, first time builder here 👋. I started with an evolve gtx but wanted more speed and range without the sag. So after much research I decided to go with the Pro 3 kit from torque boards with a Evo from landyachtz. I had an unexpected problem where the gear attached to the wheel would touch the trucks and stop the rotation, so an easy fix was to dremel down the trucks abit. Afterwards I ran into into another issue when I downloaded the latest version of the VESC tool and updated the firmware on my master vesc. Since then I've tried 3.5 and Ackmaniacs bldc tool versions to no avail. The motors spin slightly and roughly for a second and I get a bad detection error message. Sitting here stumped lol would appreciate any help 🙏. ![20190510_235852|690x335](upload://tGZ05yKFaWzY03BTbUlu7eXeEk1.jpeg) ![20190510_235835|690x335](upload://ocXfQqiv69rVc1e7GDFu3BTLWEP.jpeg)
```

---
## \#2 Posted by: rusins Posted at: 2019-05-12T15:57:57.336Z Reads: 94

```
Hi, welcome to the forum! That's a cool build you have there!

First of all, you should update the firmware to be the same version on both vescs.

Secondly, I can see you haven't connected your motors' sensor wires to the vescs. (Which is fine, if you want to run sensor-less, but why would you? :stuck_out_tongue: )

It seems like you're getting an error during setup because it's looking for hall sensors, but you haven't connected the wires, so it's failing. Try running the motor wizzard in either BLDC sensorless or FOC sensorless, so that it doesn't complain about no sensors. Let us know how it goes!
```

---
## \#3 Posted by: AlanZhou Posted at: 2019-05-12T17:00:04.453Z Reads: 74

```
[quote="rusins, post:2, topic:93576"]
(Which is fine, if you want to run sensor-less, but why would you? :stuck_out_tongue: )
[/quote]

to have a higher top speed and one less failure point. :stuck_out_tongue_winking_eye:
```

---
## \#4 Posted by: rusins Posted at: 2019-05-12T17:09:10.360Z Reads: 63

```
Some people prefer knowing the temperatures of their motors and adjusting current accordingly :stuck_out_tongue:

How does it increase top speed though? I've heard BLDC mode can be slightly faster than FOC (also don't know why), but don't know if sensors have anything to do with it.
```

---
## \#5 Posted by: AlanZhou Posted at: 2019-05-12T17:10:57.617Z Reads: 63

```
[quote="rusins, post:4, topic:93576"]
but don’t know if sensors have anything to do with it.
[/quote]

usually people run hybrid, sensored at startup then vesc automatically switches to unsensored  at a certain speed to increase speed.
```

---
## \#6 Posted by: rusins Posted at: 2019-05-12T17:11:28.349Z Reads: 57

```
Wow, that sounds cool! Is it Ackmaniac's firmware I need for that?
```

---
## \#7 Posted by: AlanZhou Posted at: 2019-05-12T17:12:14.200Z Reads: 57

```
no.... its a normal vesc feature that is in the original firmware
```

---
## \#8 Posted by: rusins Posted at: 2019-05-12T17:13:20.685Z Reads: 60

```
Ah, found it; it's under BLDC settings. Thanks!
![vesvc|664x98](upload://5gQdC9B3cCDDEjs0eSr5ftBA0yW.png)
```

---
## \#9 Posted by: wafflejock Posted at: 2019-05-12T17:19:45.629Z Reads: 54

```
FOC is quite a bit quieter but BLDC is just a bit of a whine anyway not terribly loud, like you said BLDC mode is punchier.  Using trapezoidal looking power to the motor so more of a full on full off from the coils whereas FOC mode it's sinusodial power delivery to the motor so more of a smooth transition into power delivery but not as much power delivered per coil energizing/per cycle (as far as I grok it)
```

---
## \#10 Posted by: skatardude10 Posted at: 2019-05-12T17:46:31.976Z Reads: 45

```
your trucks are backwards
```

---
## \#11 Posted by: G8dsent Posted at: 2019-05-12T17:47:33.892Z Reads: 49

```
Hi thanks for the response. I don't have the master and Slave vescs connected yet, I haven't even programmed the master first. I've tried to flash the firmware on the vesc to 3.5 which is what torqueboards recommended and it still didn't work. Then I tried Ackmaniacs bldc tool and still it didn't work. I'm running sensorless because that's what torqueboard's recommended setup is.
```

---
## \#12 Posted by: G8dsent Posted at: 2019-05-12T17:49:53.333Z Reads: 48

```
😂 I just noticed. I put the motor mount on quickly just to setup the vesc and test the motors
```

---
