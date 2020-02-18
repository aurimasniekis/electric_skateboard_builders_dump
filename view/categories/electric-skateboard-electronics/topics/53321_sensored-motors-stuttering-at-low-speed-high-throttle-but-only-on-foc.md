# Sensored motors stuttering at low speed &amp; high throttle, but only on FOC

### Replies: 13 Views: 640

## \#1 Posted by: TSG_AU Posted at: 2018-04-24T08:20:20.093Z Reads: 126

```
I've got a 12S dual VESC setup with hummie's original steel hubs, with retrofitted hall sensors.
With FOC, startup is very smooth with moderate acceleration (much more than my single belt drive could do) but if I slam the throttle wide open, the motor starts up, then stalls and stutters. I've tried adjusting the speed that the hall sensors disengage at, and found that this stuttering has happened regardless of whether or not the sensors are being used.
The problem doesn't occur with BLDC mode, so I'm hoping that my detected FOC motor parameters are just off. Or maybe it's something else, please comment if you have any suggestions because I'm at a loss. Also, the motors are running very hot- I hit the temp limit of 70 degrees C after just a mile or so of hard riding.
What are the settings other people on similar setups are using? Mine are:
![image|690x222](upload://lFWuSpf4ngvzL0rAHRVYmhF4n7G.png)
![image|690x153](upload://peA6bQVx2Kg0yfNatgHkhIXBXeK.png)
![image|690x260](upload://rNkX7gYRx8uvuSNEkkLps3fuBpP.png)
```

---
## \#2 Posted by: CarlCollins Posted at: 2018-04-24T10:56:10.173Z Reads: 99

```
What is the KV and Amperage of the motor and battery?
```

---
## \#3 Posted by: TSG_AU Posted at: 2018-04-24T11:34:34.414Z Reads: 92

```
70kv motor, no specs given for motor max current.
5Ah 20C continuous 12S lipo
```

---
## \#4 Posted by: CarlCollins Posted at: 2018-04-24T11:36:05.854Z Reads: 92

```
70 KV is way too low for 12s system
It would be better if you use 10s with it.
```

---
## \#5 Posted by: TSG_AU Posted at: 2018-04-24T11:48:47.980Z Reads: 89

```
I've heard of too high a kv and battery voltage causing the VESC to go over the safe ERPM level, but why would too low a kv be an issue?
```

---
## \#6 Posted by: JohnnyMeduse Posted at: 2018-04-24T12:53:34.251Z Reads: 82

```
I think you need to activate the sensor in 2 different places to get the foc to work with the new firmware, In the tabs FOC there a place to put it in sensor mode. 

[quote="CarlCollins, post:4, topic:53321, full:true"]
70 KV is way too low for 12s system

It would be better if you use 10s with it.
[/quote]


Sorry Carl But 70KV is fine for 12s and even better than 10S
```

---
## \#7 Posted by: CarlCollins Posted at: 2018-04-24T13:02:03.613Z Reads: 79

```
@JohnnyMeduse

Thanks man but is it okay with default values?
Also as per the history one of our customer fried his FOCBOX due to low KV motor use.
```

---
## \#8 Posted by: JohnnyMeduse Posted at: 2018-04-24T13:03:37.604Z Reads: 78

```
[quote="CarlCollins, post:7, topic:53321"]
Also as per the history one of our customer fried his FOCBOX due to low KV motor use.
[/quote]

hummm Not really, I'm pretty sure it was something else.
```

---
## \#9 Posted by: CarlCollins Posted at: 2018-04-24T13:04:26.203Z Reads: 76

```
What do you think? issue is with the FOC parameters?
```

---
## \#10 Posted by: TSG_AU Posted at: 2018-04-24T13:21:49.437Z Reads: 72

```
Yeah, just in FOC>General>Sensor Mode and in General>General>Sensor Port Mode, right?
Also as an aside, I put the motor max current down to 30A and the issue is still there when I floor it. Maybe I am expecting too much of the sensors? I just expected them to be more robust than this.

Perhaps there is a control loop somewhere that becomes unstable with too sudden of an input? I'm in current control mode with the Nunchuk app, so I'll look at maybe reducing Current KP in FOC
```

---
## \#11 Posted by: JohnnyMeduse Posted at: 2018-04-25T01:25:01.662Z Reads: 62

```
Yeah this one :+1: and the one in General/General/Sensor Port Mode.
```

---
## \#12 Posted by: TSG_AU Posted at: 2018-04-25T01:42:48.490Z Reads: 60

```
Alright, looks like I made an incorrect observation earlier. I put "Sensorless ERPM" up to 7000 (corresponding to ~15km/h) and I can floor it with no problems. 
My only concern is the potential inefficiency when I'm just cruising along on a low throttle setting with those sensors. Under no load, I'm reading double the current when running using sensors vs sensorless.
```

---
## \#13 Posted by: b264 Posted at: 2018-04-25T01:53:09.614Z Reads: 54

```
[quote="CarlCollins, post:4, topic:53321"]
70 KV is way too low for 12s system
[/quote]

This is just an opinion, *especially* with no mention of wheel size.  I, for one, feel almost everything on the market has too high a top speed and not enough torque so don't ever make too many assumptions...
```

---
