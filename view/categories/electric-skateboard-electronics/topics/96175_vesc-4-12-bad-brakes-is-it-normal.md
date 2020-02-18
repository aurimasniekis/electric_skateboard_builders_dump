# Vesc 4.12 Bad brakes, is it normal?

### Replies: 8 Views: 244

## \#1 Posted by: Gilldur Posted at: 2019-06-08T17:25:59.806Z Reads: 86

```
Hello everyone.

Just finished my first build and it came together really well, except for the braking.

Running dual 6355, with vesc 4.12, firmware 3,57~, Vesc is from Torqueboards 
16/36 pulleys.
10s4p 30q
85mm wheels (caguamas)
BLDC mode.
Flipsky VX1 remote.

So the brake settings are -60a for the motors and -12a on regen (3a per P) which should be nice and safe on the 30q cells. I know i can go to 4a per cell safely but i have yet to try that. I doubt 1 more amp will make much difference considering how bad it is now.

The reason i am making this post is that i have a wowgo 2s that i was using to commute until my DIY board was finished. And the wowgo 2s has much MUCH better brakes. And the wowgo 2s only has a 10s2p 30q pack in it. So unless the hobywing esc has resistors to help brake i cant imagine that it would be better.

I have been reading a lott on settings and other topics on weak brakes and so on so i know i should not expect very good braking with my setup. But is it really normal that is so much weaker then a normal wowgo 2s? Any other settings in the vesc that i should know about?

I have also soldered TVS diodes to my PCB's so i might be brave enough to run FOC mode, would that help with brakes?
```

---
## \#2 Posted by: kntzn Posted at: 2019-06-08T19:08:15.119Z Reads: 69

```
Hi. As you mentioned, you have dual motors and -12A regen current. Is it set to -12A on each vesc or -12A collectively?
According to your setup, each vesc should give -6A to the battery, not -12A.

Do your motors get hot while you are using maximum braking?

And also, what control type you are using? Current/Duty cycle?
```

---
## \#3 Posted by: bazis Posted at: 2019-06-08T20:10:22.176Z Reads: 62

```
4A is safe current for 30q for full charging from empty. For short braking period you can set much more charging current. It's all about heat. If battery in normal temp, charging current is acceptable.
```

---
## \#4 Posted by: Gilldur Posted at: 2019-06-08T20:31:18.091Z Reads: 57

```
Hello kntzn, Thanks for the reply. 
-12 is total, each vesc is set to -6. I will re-config tomorrow to -8 per vesc but i doubt it will be a huge difference. 

I went down some long hills today at speed and braking all the way down. The motors were lukewarm at most. so no real heat.

As embarrassing as it is to admit i have no idea what control type i am using :blush:. Where can i see those settings?
```

---
## \#5 Posted by: kntzn Posted at: 2019-06-08T20:46:45.681Z Reads: 52

```
Control type in VESC tool located at:

_App Settings > PPM > General > Control Type._
```

---
## \#6 Posted by: Gilldur Posted at: 2019-06-08T20:50:18.980Z Reads: 50

```
So the remote i use communicates using uart. And from what i can read that is not configurable? So my PPM is currently disabled.
```

---
## \#7 Posted by: kntzn Posted at: 2019-06-08T21:44:17.561Z Reads: 45

```
In this case badly calibrated remote is not the reason of your problem. Because i thought that badly calibrated remote at 100% brakes reads as 25% brake, so your current at 100% brake is not 60A, but 15A or something like that.

And what is the name of the remote?

Anyway, if your motors do not heat up while breaking there is no conversion of mecanical energy to heat. In this case you can try to cranck up the braking current of the motor. I think that braking current of the motor does not even get close to 60A when you are braking so it is quite interesting if something will change with increased breaking current. 

If it increases but slightly it is still going to be seem to be a bad remote calibration. If nothing changes the problem is elsewhere.
```

---
## \#8 Posted by: Gilldur Posted at: 2019-06-08T22:21:40.389Z Reads: 40

```
Thanks for the advice. I will increase regen as well as motor braking current. I think i increase the settings until either motor or battery temps start to rise. Like i said, right now nothing ever gets hot.
```

---
