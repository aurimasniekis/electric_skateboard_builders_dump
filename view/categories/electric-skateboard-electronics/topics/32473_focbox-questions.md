# FOCBOX Questions

### Replies: 18 Views: 1525

## \#1 Posted by: rolexbene Posted at: 2017-09-06T21:33:11.500Z Reads: 214

```
So I bit the bullet and purchased a FOCBOX. Now I need some help and advice with understanding the possible configs. My questions are:

* Is there anything special about the Enertion BLDC tool / 2.18 Firmware (downloaded from the Enertion website)?
* Can I safely use Ackmaniac BLDC tool with Ackmaniac firmware in FOC?
* Can I safely use the new VESC-tool and 3.27 firmware?

* Can I safely run a 270kv motor in FOC with any of the above?
```

---
## \#2 Posted by: JohnnyMeduse Posted at: 2017-09-06T21:37:09.792Z Reads: 208

```
You can use any firmware you want, but It's might be a void of warranty, specially if you use a firmware or option that as not been properly tested, and are still in experimental phase.
```

---
## \#3 Posted by: rolexbene Posted at: 2017-09-06T21:42:14.080Z Reads: 204

```
But do you happen to know if Enertion firmware has anything added to interface with there hardware, for instance to stop the DVR from burning out?
```

---
## \#4 Posted by: JohnnyMeduse Posted at: 2017-09-06T21:44:09.867Z Reads: 199

```
No there is nothing added it is the original firmware for the 4.12 from Vedder
```

---
## \#5 Posted by: Namasaki Posted at: 2017-09-06T21:45:19.927Z Reads: 198

```
[quote="rolexbene, post:1, topic:32473"]
Can I safely run a 270kv motor in FOC with any of the above?
[/quote]


Safe Motor KV depends on what voltage your running.
```

---
## \#6 Posted by: rolexbene Posted at: 2017-09-06T21:47:31.874Z Reads: 196

```
Ok so using new firmware 3.27 should be better for VOC as stated by Benjamin?

@Namasaki I am going to be running an 8s setup.
```

---
## \#7 Posted by: Mikenopolis Posted at: 2017-09-06T22:00:56.943Z Reads: 195

```
Gonna jump on this thread and hope to get some insight.

I have a Raptor 1 deck with a 10s3p battery, two VESC-X and waiting for the CarvOn V3 drives. I hope to use FOC for smooth standing startups. Clicking on the FOC tab I'm a bit hesitant on FOC there are so many settings! Besides using a Y cable instead of canbus and swapping the sensor T & H3 wires...

WHAT SUGGESTIONS DO EXPERIENCED FOC USERS HAVE IN TERMS OF NOT BLOWING ANYTHING UP ON THIS DUAL SETUP?
```

---
## \#8 Posted by: Namasaki Posted at: 2017-09-07T01:44:09.515Z Reads: 178

```
[quote="rolexbene, post:6, topic:32473"]
@Namasaki I am going to be running an 8s setup.
[/quote]

8s + 270kv exceeds the Vesc 60k ERPM limit and though you may be able to protect the drv chip by limiting ERPM in bldc tool, the 270 KV motor may be a little weak in torque requiring more current and generating more heat. 
I would recommend using a lower KV motor unless your trying to break some flat ground speed record. 

For an everyday dependable build I think maximum torque with adequate top speed is the best combo with a motor that will draw minimum current and run as cool as possible.
```

---
## \#9 Posted by: BenTheBarre Posted at: 2017-09-07T04:30:56.392Z Reads: 160

```
@Namasaki 

Just inputted 8s and 270kv into the esk8 calc and got 55k erpm... am I missing something?
```

---
## \#10 Posted by: onepunchboard Posted at: 2017-09-07T04:36:57.013Z Reads: 157

```
cal with full charge 4.2 times 8
```

---
## \#11 Posted by: Namasaki Posted at: 2017-09-07T04:37:23.258Z Reads: 156

```
Yes, you should calculate with full charge 4.2v per cell
```

---
## \#12 Posted by: High-roller Posted at: 2017-09-07T04:42:03.416Z Reads: 153

```
Gonna jump on your jump on this thread.
I have a similar setup- dual FOCboxes, dual 190kv motors, 10s5p 36v battery, planning to use a Y cable.
I'm about to start programming my vescs for the first time and there's suddenly alot of options out there for doing it. I'll probably start with bldc then switch to FOC later on.
What program/ settings does the community recommend for not blowing up?
```

---
## \#13 Posted by: BenTheBarre Posted at: 2017-09-07T05:09:24.516Z Reads: 149

```
@Namasaki

Oh right, totally makes sense👍
```

---
## \#14 Posted by: rolexbene Posted at: 2017-09-07T08:30:39.660Z Reads: 146

```
[quote="onepunchboard, post:10, topic:32473"]
4.2 times 8
[/quote]

Well my thinking was that I have measured the motor on the bench, no wheel or pulley, at 270kv. I believe that this means KV will drop 10-15 on the board. Meaning 260KV. This gives me 53872 ERPM on Esk8 calculator and a weighted speed of 21mph (not that excessive for the setup?). I understand at full charge this may be a little to high on the ERPM, but can I not just limit this in Vesc-tool.
I have a feeling that when testing on the bench it was topping out at 55000 at full throttle, will check again later this eve.

I am planning on running mostly on flat ground, but I guess I can always swap my motor at a later date if torque is an issue. @Namasaki what KV would you recommend for this setup to be able to hit some hills on a single, 200kv?

Based on this information I am spot on with my calculations.
https://www.electric-skateboard.builders/t/choosing-the-right-motor-kv-for-the-vesc/3125
```

---
## \#15 Posted by: onepunchboard Posted at: 2017-09-07T12:38:51.190Z Reads: 130

```
you can just limitt on vesc. it's  just the system gets inefficient over 60k which BV pointed out on his development. so many recommend low kv motors with low gear ratio and high voltage.

I don't use 60k limit and motor goes beyond it. but I never got to use it anyways cuz I have to go 65kmh at least which might kill me. also if u go beyond 40kmh there is drag that belt creates everytime I stop throttle.
```

---
## \#16 Posted by: Namasaki Posted at: 2017-09-07T13:53:20.230Z Reads: 121

```
You will not likely exceed the ERPM limit riding unless you like to go flying downhill. 
However if your testing your board while it's sitting upside down on the bench you could easily exceed it
```

---
## \#17 Posted by: rolexbene Posted at: 2017-09-07T13:55:12.700Z Reads: 126

```
[quote="Namasaki, post:16, topic:32473"]
exceed
[/quote]

Ok thanks for the info, I will be sure to put some limits in place.
```

---
## \#18 Posted by: Tomash Posted at: 2017-09-07T14:22:08.073Z Reads: 116

```
270 kV motor, would be "safe" for 6S setup, if you have 60k eRPM limit in mind.
245 kV motor is best for 8S setup.
190 kV motor for 10S setup.

For example, 190 kV 6364 outrunner is better if you want torque at expense of speed.
245 kV is better if you want more speed.
You can always go with 190 kV on 8 or 6S, but as other mention before me,  you will be slower.
You can always go higher kV motor. (ofc. on right voltage), and make double motor drive, then you will get more torque :smile:

I run with 8S, 245 kV, twin motor setup. I am fat (120 kg), and still i ride with no problem with top speed of at least 50 km/h. I have 7 inch pneumatic wheels.
```

---
