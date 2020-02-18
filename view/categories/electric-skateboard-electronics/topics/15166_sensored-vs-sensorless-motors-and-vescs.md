# Sensored vs sensorless motors and vescs

### Replies: 11 Views: 4233

## \#1 Posted by: NewbieBoardBuilder Posted at: 2016-12-25T00:36:28.810Z Reads: 565

```
So I have been doing a TON of reading recently about sensored motors and sensored VESCs, VS. sensorless motors and sensorless VESCs. What are the advantages and what do they even do?!?!? I'm new and please don't tell me "go read more"! Trust me I have
```

---
## \#2 Posted by: lox897 Posted at: 2016-12-25T00:45:55.377Z Reads: 564

```
Sensored gives a smoother startup, but a lower top speed. The VESC can use sensors at startup and disable them at a certain RPM.
```

---
## \#3 Posted by: NewbieBoardBuilder Posted at: 2016-12-25T00:53:46.828Z Reads: 555

```
[quote="lox897, post:2, topic:15166"]
and disable them at a certain RPM.
[/quote]

The sensors are disabled? Also, what kind of sensors are they (what do they measure or prevent), and where can they be found besides a VESC?
```

---
## \#4 Posted by: lox897 Posted at: 2016-12-25T00:56:47.194Z Reads: 550

```
There aren't any in the vesc. They are in the motor. The sensors get turned off after startup so they don't limit speed.
```

---
## \#5 Posted by: NickTheDude Posted at: 2016-12-25T01:02:52.154Z Reads: 539

```
Their called Hall Sensors. From what I understand they measure the mangetic field around them and output a voltage based the fields strength. I think in this case they are used so the VESC can determine where the motors magnets are, and electrify the right parts of the stator to reduce cogging. However I dont know why they would reduce top speed.

I'm pretty sure the boosted boards remote uses them as well. The throttle wheel has two magnets on it, one on either end and a hall sensor attached to center throttle position. When the wheel gets turned the hall sensor measures an increase or decrease in magnetic field strength since the magnet attached to the wheel is now further from the center, and sends that value to the reciever.
```

---
## \#6 Posted by: ArmandR Posted at: 2016-12-25T02:07:06.395Z Reads: 518

```
So it's best to get sensored and have the vesc un sensor them?
```

---
## \#7 Posted by: PXSS Posted at: 2016-12-25T02:15:26.618Z Reads: 511

```
Yes you are right, the hall sensors output a voltage based on the position of the stator with respect to the magnets (they measure the electromagnetic induced current). The VESC can then more accurately command the motor to the correct RPM.

The reason this limits the top speed is that this process takes time and it's probably not as fast as when the motor is going at top speed so to keep accurate tabs the VESC slows it down to whatever speed it can manage.
```

---
## \#8 Posted by: PXSS Posted at: 2016-12-25T02:17:23.598Z Reads: 504

```
There is a hybrid mode you can run that is sensored at low RPMs to reduce cogging and have a smoother startup and non sensored after a certain RPM where it is no longer needed. 

You can find plenty of info by googling rc sensored vs sensorless motors and on the VESC how to threads
```

---
## \#9 Posted by: SageTX Posted at: 2016-12-25T03:20:07.155Z Reads: 496

```
IF you can figure out the order of the wires.  I'm still stumped.
```

---
## \#10 Posted by: Hummie Posted at: 2017-09-02T16:23:22.470Z Reads: 330

```
anyone know how much more efficient sensors are in foc or have done real comparisons?
#####
According to rew on vedders site they do little for efficiency
```

---
## \#11 Posted by: itsmikeholland Posted at: 2017-09-04T05:46:07.304Z Reads: 289

```
basically an unsensored motor will chirp for a bit if you try to accelerate from a stand still on flat ground, but after literally one second it will go. during your actual cruising you will notice no difference between sensors and no sensors.
```

---
