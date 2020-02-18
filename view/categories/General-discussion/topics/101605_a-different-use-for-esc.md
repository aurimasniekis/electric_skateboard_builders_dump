# A different use for esc

### Replies: 13 Views: 629

## \#1 Posted by: omar1976 Posted at: 2019-09-10T22:45:24.879Z Reads: 151

```
hi guys i'm new in this forum because i'm approaching now the world of brushless motors ..... i bought two hub motors and their esc on amazon and i created a cablecam ..... but i'd like to change the system control with a better one, and being able to manage the ESC via arduino so that you can use cablecam braking sensors .... can anyone help me ???? place some photos on what I did ...![image|666x500](upload://tRqJA2z159XKuWBxB3sDmwAokUc.jpeg) ![image|666x500](upload://q1wOjXkKnJevxKrNp5HCw9bJue7.jpeg) ![image|666x500](upload://qfJuwOTD2knXjHeX8gvHKfqWDlf.jpeg) ![image|666x500](upload://dkOK3oDE7oGDn02giRgZGUclRZ3.jpeg) ![image|666x500](upload://hfIhU7a3Z5DJdJypq8jDlh7LY0L.jpeg)
```

---
## \#2 Posted by: Halbj613 Posted at: 2019-09-11T09:39:09.642Z Reads: 120

```
those esc can not be programmed you have to buy a vesc which is programable through the app
```

---
## \#3 Posted by: omar1976 Posted at: 2019-09-11T10:43:03.224Z Reads: 113

```
thanks for the answer but here two connectors near the red signs what are they for ??? are the inputs or outputs ???
```

---
## \#4 Posted by: Ben.Nexus Posted at: 2019-09-11T11:58:30.783Z Reads: 99

```
Well, depending on the ESC version, one is the 4WD Canbus connector (Often also used to flash the firmware, or only used to flash firmware on older versions) and the other one is the LED lights control/auxiliary power The unmarked one is likely the auxiliary wired for a voltage meter... There are so many variations its hard to tell though.
```

---
## \#5 Posted by: omar1976 Posted at: 2019-09-11T13:00:57.444Z Reads: 91

```
if it is a can bus port can I control it with arduino ???
and not wanting to use his wirless control I can control it with a cable made in doc ... opening the esc and opening the remote control I have born that on the pcb there is a brush for a 7 pin connector ....
```

---
## \#6 Posted by: Ben.Nexus Posted at: 2019-09-11T15:26:28.667Z Reads: 75

```
You can't do anything more than 1 channel control through the supplied remote or another remote that connects to that connector, and maybe 2 channel with a remote that has the LED light switch on it. You could take apart the remote and have your own potentiometer data get fed into the remote transmitter, possibly.
```

---
## \#7 Posted by: cybervzhn Posted at: 2019-09-12T14:47:53.185Z Reads: 46

```
You may want to consider a PID controller used in robotics and the radio control hobbies.  You can do this with audrino or raspberry PI, however, there is already mature controller software and hardware developed for this intended for autonomous and radio controlled air and ground craft that have accelerometers and gyroscope built in.  It might be worthwhile to look at APM/Ardupilot and iNAV.  Oh, and you can get like 8 channels of tunable motor control along with multiple high speed serial ports on the controllers, and they are usually based on an ARM F3, F4, or F7 chipset.
```

---
## \#8 Posted by: omar1976 Posted at: 2019-09-17T07:57:56.631Z Reads: 34

```
hello I had some time and I opened both the controller and the esc and I noticed these pins that I highlighted ...... it is possible that red can be used to control the esc with cables ??? and what are the yellow and blue ones for ????![image|374x500](upload://uPrsojVDAsQcVoPlDLyAN3lSDbT.jpeg) ![image|667x500](upload://rii6NGcDRCuD2HIkWWpN6Py9Z1d.jpeg)
```

---
## \#9 Posted by: omar1976 Posted at: 2019-09-17T08:01:02.742Z Reads: 29

```
I saw a video on youtube that used two escs and controlled 4 wheels with only one command ... and the two escs were connected to each other by that red connector ...
```

---
## \#10 Posted by: omar1976 Posted at: 2019-09-17T08:05:31.286Z Reads: 28

```
place the link so you can see...
https://youtu.be/_FY0mZrbf5g
```

---
## \#11 Posted by: Ben.Nexus Posted at: 2019-09-17T12:15:52.266Z Reads: 25

```
So it looks like you have the version with seperated BUS and DEV ports. so yes, that port is for 4WD. You could possibly connect the two and it might work? But the connection protocol might be something you can't easily decode. Wouldn't it be easier just to have the small wireless connection, and control the potentiometer on the remote instead of using the ESC?

Also, by the way, unless you need all the speed, it is possible to control something like this with a 30$ ESC + $50 nice controller - just at lower voltage and higher amps. Even just a setup with a servo ESC might work
```

---
## \#12 Posted by: omar1976 Posted at: 2019-09-17T15:40:59.510Z Reads: 18

```
I would like to try to control the ESC by cable so as to be able to have more distance than the declared 8 meters ... to be able to have a safe control without unhooking
```

---
## \#13 Posted by: Ben.Nexus Posted at: 2019-09-17T16:24:29.133Z Reads: 15

```
Well you could always extend the potentiometer wires to as long a distance as you want, and keep the receiver and transmitter right next to each other. I would also wire in the input to the remote to the battery (With a step down) so it would never run out of power. Kind of a "silly" solution but it would work. Might also be nice to have the option to just buy a second controller and have that in hand if a different use for your rig comes about, and swap easily between the two.
```

---
