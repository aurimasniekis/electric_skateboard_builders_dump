# Whole build from scratch!

### Replies: 12 Views: 295

## \#1 Posted by: kmb Posted at: 2019-10-02T05:46:41.890Z Reads: 116

```
Hey guys, I am working on a build for an E-board and I could use a lot of tips. 

For the deck I currently own an atom drop-deck board that I love (picture attached). I love this deck however I want to keep that board. I am taking a class about working with composites so I am hoping to make a copy out of a carbon fiber/fiberglass mixture. I don't know for sure what that will look like yet but I am working on that with my teacher. 
![PT2|500x500](upload://qynwc6MrlDTAxK1Sj7s951n1wvL.jpeg) 

I currently have a nice big motor, it's a Turnigy Aerodrive SK3 - 6364-245KV Brushless Outrunner Motor. Here are the specs for the motor. I am debating getting a second one for symmetry's sake.
Turns: 14T
Voltage:  10S Lipoly
RPM/V:  245KV
Internal resistance: 0.018 Ohm
Max Loading: 70A
Max Power: 2700W
Shaft Dia: 8.0mm
Bolt holes: 32mm
Bolt thread: M4
Weight: 718g
Motor Plug: 4mm Bullet Connector
![18128|566x415](upload://8MXTOStiZSzAFaE4OdlcheNcstg.jpeg) 

I have a FSESC 4.12 50A Based on VESC® 4.12 esc, will it be easier to add another one or should I just buy a dual in order to run two? Here are the specs for mine:
Hardware:V4.12
EPRM:60000
Firmware: V3.40(Keep upgrated with the latest firmware version)
PCB:4 layers, size: 40*60mm
Current: 50A continuous / 240A peak
Voltage: 8V-60V (Cells: 3-13S LiPo)
Recommended 10S battery
BEC: 5V@1.5A
BEC type: Internal driver support 
Timing: Software calibration 
Motor control interface: PPM signal (RC servo), analog, UART, I2C, USB or CAN‐bus. 
Cutoff Voltage: Programmable
Frequency: PWM input 
Governor: No
Weight: 80g
FSESC4.12 Size: 110x40x20mm
Programming card: No
Reverse: Yes
![DSC04948_3178096d-5ec1-46ff-b145-57eb75ff4eca_1800x1800|500x500](upload://sAfhlfosaOmrsdSvjWMOdQ1YBDY.jpeg) 

I have a 10s Lipo battery however I am looking into making my own preferably Lion battery because I heard they are less volatile and easier to charge.

I have seen some offroad wheels on some of these threads but it wasn't clear what in the final verdict was on what you guys liked. 

I don't have trucks or motor mounts but part of me was wondering about casting my own with the mounts built in.

I basically have lots of creative ability and hoping to make something that will last me forever. I am also particularly curious in a power switch, charging, and a battery level indicator.
```

---
## \#2 Posted by: BillGordon Posted at: 2019-10-02T08:27:56.480Z Reads: 90

```
You don"t want that motor kv. Stick with something 200kv or under.
```

---
## \#3 Posted by: kmb Posted at: 2019-10-08T22:00:15.530Z Reads: 51

```
Will that motor not have enough power?
```

---
## \#4 Posted by: rusins Posted at: 2019-10-08T22:05:09.656Z Reads: 50

```
Power? Yes. Torque? No. Lower kv will have the same power, but more torque (less top speed, but you don't wanna go 60mph on this thing lol)
```

---
## \#5 Posted by: kmb Posted at: 2019-10-08T22:17:19.213Z Reads: 47

```
Can I not fix that with the gearing on my belt drive?
```

---
## \#6 Posted by: rusins Posted at: 2019-10-08T22:21:32.140Z Reads: 43

```
Yes and no. Theoretically: of course! Practically: if your motor pulley is too small, the belt will slip. If your wheel pulley is too big – it won't fit the wheels you choose!

Another important factor is that ESCs based on the VESC 4 aren't rated to handle high kv motors at the usual voltages we use, so your ESC could die, and possibly throw you off the board. Many esk8 calculators will multiply your battery voltage by the kv and 7 (number of motor pole pairs) to show you the eRPM, which is the value you should keep under 60k if you plan to use it with your Flipsky ESC. Some controllers, like the Focbox Unity, can do much more, but trust me – just using a lower kv motor is easier :)
```

---
## \#7 Posted by: kmb Posted at: 2019-10-08T22:25:37.327Z Reads: 38

```
So what is a motor you suggest? I am a fan of the dual drive idea and I found this ESC on Amazon will this work?

[New Dual ESC](https://www.amazon.com/dp/B07MMTS4YN/ref=sspa_dk_detail_2?psc=1&pd_rd_i=B07MMTS4YN&pd_rd_w=TKtzz&pf_rd_p=45a72588-80f7-4414-9851-786f6c16d42b&pd_rd_wg=iefdk&pf_rd_r=F2B7DXXMRF8QR7S62NW6&pd_rd_r=e9cac89b-c68e-49d1-ba88-3ec4692f0c26&spLa=ZW5jcnlwdGVkUXVhbGlmaWVyPUExNFEzT1NGQ0ZJS0pNJmVuY3J5cHRlZElkPUEwODYxMDMyMUFWM1IzSE43STc1RiZlbmNyeXB0ZWRBZElkPUEwOTkyOTIwVDJYUjVVREdaNDhRJndpZGdldE5hbWU9c3BfZGV0YWlsJmFjdGlvbj1jbGlja1JlZGlyZWN0JmRvTm90TG9nQ2xpY2s9dHJ1ZQ==)
```

---
## \#8 Posted by: rusins Posted at: 2019-10-08T22:28:09.639Z Reads: 32

```
If you already have a Flipsky ESC then the best option is to just buy another one and a CAN-bus cable to connect them. That ESC you linked is Chinese garbage – it's what weak prebuilt boards use.

I'm beginning to think you haven't read through the getting started threads on this forum, I'll link them to you, 1 sec
```

---
## \#9 Posted by: rusins Posted at: 2019-10-08T22:28:57.159Z Reads: 34

```
https://www.electric-skateboard.builders/t/start-here-faq-for-diy-electric-skateboard-builders/215

As the thread says, you really should read all of that before you start ordering parts. Will save you time and money in the long run :+1:
```

---
## \#10 Posted by: kmb Posted at: 2019-10-08T22:30:15.740Z Reads: 30

```
I've looked through that a few times but I wasn't seeing much about combining ESC's and building batteries which I had more questions about than my motor.
```

---
## \#11 Posted by: kmb Posted at: 2019-10-08T22:32:45.813Z Reads: 29

```
I ordered these about 3 years ago and I am finally gritting through to where I am actually doing this.
```

---
## \#12 Posted by: BillGordon Posted at: 2019-10-09T06:20:21.510Z Reads: 28

```
Don't start your parts list with workarounds. By beginning in a popular and proven range, you can use the same motor if you decide to go AT later on and you have more pulley options. By far the most popular kv for urethane wheels is 190kv, with those doing pneumatic builds going as low as 130 but many in the 150-170 range.

I admire that you're planning to do your build from scratch, but that approach requires a lot of reading and prep before you pull it off. This is especially true when you get to the battery. I promise you that if you dig deep, it is all there. A bunch of really smart people put it there expressly for you and this purpose.
```

---
