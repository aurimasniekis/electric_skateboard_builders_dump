# VESC FAQ &#124; Setting up receiver and brakes PPM

### Replies: 11 Views: 13972

## \#1 Posted by: onloop Posted at: 2015-09-27T08:27:57.127Z Reads: 1666

```
Big thanks to Marcin, 

Here is a really good video tutorial showing you how to change settings in the BLDC tool to configure the VESC for optimal input control using PPM, which is used by the common RC controller GT-2B. 

Basically it's fine tuning the input data recieved from the TX. Another example of why the VESC is superior.

The video also shows how to adjust brake & regen. This is important because too much brake force from the motor can exceed the torque load rating of the 9mm wide, 5mm pitch HTD drive belts that most of us use on our eboards.

Too much brake force basically means the belt will skip teeth and eventually shred itself (because the force of forward momentum is greater than the force the belt can apply onto each pulley tooth to counter the momentum). So basically these settings can improve belt life and also give you a customized braking experience... please note that your body weight should be factored into the adjustment you make. The more you weigh the bigger the load that needs to be stopped. Lighter riders can have harder (higher) brake force because their load is easier to stop.

Also note dual motors (with dual belts) have 2x the potential brake force. Because you have double, it means you have better brakes. Both belts combined can handle twice the torque load of a single belt..

So dual drive eboards can have higher regen numbers then what is showed in the video.

Note: if using the space cell that has a 30A fuse installed - your regen set to high could blow the fuse! So try setting it around -40 this offers good strong brake force and safe regen currents.


WATCH THE VIDEO
https://youtu.be/OtuofrQr3F8
```

---
## \#2 Posted by: Lukaszlisc Posted at: 2016-09-27T14:19:42.017Z Reads: 1025

```
hi i just got the VESC and i follow all the setups and try different one is well but got problem to start board from 0km/h when standing or small up hill, motors just shaking and making noise (not going forward), i have to push my self to start and after board is so fast and can claim even big hills on slow speed (not had this problem with standard ESC) any ideas what could be wrong?
```

---
## \#3 Posted by: Carvin_Ginger Posted at: 2016-09-27T16:38:21.783Z Reads: 891

```
Where's the VESC from?
```

---
## \#4 Posted by: Jinra Posted at: 2016-09-27T16:48:18.503Z Reads: 822

```
This is a small problem with unsensored setups, but it's no big deal to do a small kick start each time. You can minimize the effect if you raise the startup boost on BLDC tool to about .03-.05
```

---
## \#5 Posted by: Lukaszlisc Posted at: 2016-10-01T07:39:09.220Z Reads: 766

```
VESC is from scramboards. Is problem for me as im using mountain board with straps. And wiggling around something she's not enough power to start. Got 12s setup and 16s lifepo with 6355 190kv china motors wonder if i will put 6374 3kw motors will help?
```

---
## \#6 Posted by: elkick Posted at: 2016-10-01T07:47:34.227Z Reads: 700

```
It might be a problem with those VESCs, I have seen some of them not working properly (falling off Caps for example and non genuine parts).
```

---
## \#7 Posted by: Lukaszlisc Posted at: 2016-10-01T08:06:53.028Z Reads: 656

```
Had problem to conect them via canbus is well. I did use Y wire from receiver but after 20min using 1 vesc got Drv foult. Spoked with manufacturer and they said will send replacement, will see in new one be okay
```

---
## \#9 Posted by: kuphjr Posted at: 2017-08-27T20:39:15.478Z Reads: 358

```
I am having an issue configuring the throttle on my ESC.  What happens is when I plug in the ESC to the battery pack, I hear rapid beeping indicating that the throttle must be pushed to the lowest position.  After I do that, as soon as I let the throttle return to the middle position the motor starts to spin.

Does anyone know how to calibrate it so that when the throttle is in the middle the motors do no spin?  Also, does anyone know how I can set up the ESC so that when I pull the throttle down it applies the breaks?

Thanks!

Here is a link to the ESC I am using: https://hobbyking.com/en_us/turnigy-sentilon-v4-100a-5-12s-hv-bulletproof-speed-controller-w-rpm-sensor.html
```

---
## \#10 Posted by: DevinG Posted at: 2018-04-18T22:47:19.005Z Reads: 205

```
do the settings in the video translate differently when ridden? i have concerns that this accelerates to hard and brakes to sudden with my 2.4ghz mini controller.
```

---
## \#11 Posted by: JohnnyMeduse Posted at: 2018-04-18T22:57:36.117Z Reads: 193

```
Yes, it is different, since there is no load on the motor when you are on the bench
```

---
## \#12 Posted by: DevinG Posted at: 2018-04-18T23:00:21.181Z Reads: 181

```
thank you once again @JohnnyMeduse huge headache avoided, now its just aesthetic/function work...
```

---
