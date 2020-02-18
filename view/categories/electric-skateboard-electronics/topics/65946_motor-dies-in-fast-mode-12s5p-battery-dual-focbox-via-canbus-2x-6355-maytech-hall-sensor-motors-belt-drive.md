# Motor &ldquo;dies&rdquo; in fast mode? 12s5p battery, Dual FocBox via Canbus, 2x 6355 maytech hall sensor motors, belt drive

### Replies: 6 Views: 221

## \#1 Posted by: Simonwantstobuildabo Posted at: 2018-08-24T14:18:00.768Z Reads: 112

```
Hi! My dual beast 6355 maytech motor setup, with dual focbox and 12s5p has some issues!
( I use maytech standard remote and reciver )

Also i use VESC TOOL!

One of the motors in “fast mode” shuts down? So i can press full throttle in eco mode, no problem, but when i switch to fast mode it shuts off after a while? Like you can hear 100% Throttle, and after 5,10,20 seconds it goes down to like 60% or even less?

Short version: When pressing full throttle in fast mode, motor start slowing down.

Please help vesc tool gods!
```

---
## \#2 Posted by: linsus Posted at: 2018-08-24T14:29:03.015Z Reads: 107

```
Not familiar with the modes on the remote.
But there are temp limits on the VESC that kick in if  tresholds are met that reduce performance to save the hardware. It would be helpful if you could give us some logs on the actual event and we could investigate further.
```

---
## \#3 Posted by: Sender Posted at: 2018-08-24T14:32:01.484Z Reads: 102

```
Is the fast mode a switch on the remote?  If so, did you set up the PPM values while it was set to the fast mode or regular?
```

---
## \#4 Posted by: dareno Posted at: 2018-08-24T21:48:01.125Z Reads: 68

```
Post your settings so they can be looked at.
```

---
## \#5 Posted by: rey8801 Posted at: 2018-08-24T22:11:35.623Z Reads: 63

```
Do you have a BMS for discharging connected? And yes post the vesc setting. I guess you hit some current limit, either the BMS (but should remove power to both of the motors) or the vesc
```

---
## \#6 Posted by: rey8801 Posted at: 2018-08-24T22:13:20.829Z Reads: 63

```
That's true I did the same stupid thing the first time I used a nano-x :laughing:
```

---
