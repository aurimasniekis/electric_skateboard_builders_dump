# VESC 75/300 Backwards Startup with High Inertia

### Replies: 13 Views: 542

## \#1 Posted by: goffzh Posted at: 2019-04-04T06:44:39.240Z Reads: 103

```
Trying to use the VESC 75/300 to spin up a large inertial flywheel and having lots of issues getting it to startup in the right direction. In this video you can see it starts running backwards twice and the 3rd try it gets going in the right direction. This is a sensorless Neumotor 8038/145kv on 12S. VESC is in BLDC Duty Cycle No Reverse. Motor detection wizard ran flawlessly without the flywheel attached. It'll take about 5 seconds to get to full speed on 250A current limit with the flywheel. Any suggestions on parameters to adjust to improve the backwards startup? https://www.youtube.com/watch?v=WmGrzgxXZ1U&amp;feature=youtu.be
```

---
## \#2 Posted by: lrdesigns Posted at: 2019-04-04T06:57:03.720Z Reads: 98

```
I find increasing "minimum current" and "start up boost" will help unsensored motors get moving more easily with less coging. 

![image|589x251](upload://z5dCe7CU97beDXUE7cwT5byBnTZ.png) 

![image|385x149](upload://zETbpElDK8zsUKl1L3WYSDq8xpF.png)
```

---
## \#3 Posted by: goffzh Posted at: 2019-04-04T07:15:47.892Z Reads: 87

```
I'll give those a try tomorrow but pretty sure those only affect Current Control Type whereas I'm really wanting to stay with Duty Cycle Control Type to have the flywheel speed proportional to throttle position.
```

---
## \#4 Posted by: Gamer43 Posted at: 2019-04-04T07:20:47.604Z Reads: 81

```
Maybe try setting a minimum duty cycle in that case?

The only issue with that is you'll have to let it coast to zero speed from said minimum duty cycle when slowing down or stopping the flywheel.

Just curious, have you tried PID Speed Control mode?
```

---
## \#5 Posted by: goffzh Posted at: 2019-04-04T07:24:24.340Z Reads: 76

```
Is there a way to slow down the open loop startup commutation? Seems like the VESC is trying to accelerate the motor way faster during open loop commutation than the inertia of the flywheel will allow.
```

---
## \#6 Posted by: goffzh Posted at: 2019-04-04T07:48:40.012Z Reads: 72

```
I'm totally fine with coasting the flywheel, would rather not dump all that energy back into the VESC. Infact, we're having problems disabling braking in duty cycle mode. When the motor current max brake and battery current max regen are set to 0, the motor just keeps on going, never slows down despite air and rolling resistance.

Haven't played with PID speed control mode yet, was hoping to not introduce more variables but may start messing with it if I can't get duty cycle startup working reliably.
```

---
## \#7 Posted by: AlexBE Posted at: 2019-04-04T07:51:10.174Z Reads: 64

```
I would be interested to hear if you can change the speed of the Sensorless startup for slow start applications like this.

A potential hack for the moment is to run the FOC_openloop command and just set the RPM very low and slowly ramp it up manually.
```

---
## \#8 Posted by: Pedrodemio Posted at: 2019-04-05T00:06:58.993Z Reads: 42

```
Unfortunately there isn't a duty cycle no brakes like most RC esc when using the duty cycle mode

What you could try is is set the min currents to zero or really low
```

---
## \#9 Posted by: Gamer43 Posted at: 2019-04-05T00:22:21.523Z Reads: 41

```
Disabling braking on duty cycle control is basically impossible. If you disable synchronous recitifcation, it becomes a sort of pseudo current control with extreme heat dissipation.
Might have to do PID speed control with zero braking current, as I'm pretty sure the VESC would then just let the flywheel coast to the desired speed.
```

---
## \#10 Posted by: goffzh Posted at: 2019-04-05T04:03:18.721Z Reads: 41

```
Allright, gave up on BLDC and switched to FOC. Autodetect worked flawless and then cranking up the stator saturation compensation to 35% got it moving pretty reliably when hooked up to the flywheel. There's very little friction just lots of momentum. It'll still turn in the wrong direction for a couple seconds but the VESC eventually figures it out and will reverse to start spinning the right direction. Any other obvious settings to experiment with to get it kickstarted in the right direction from a dead stop?
```

---
## \#11 Posted by: AlexBE Posted at: 2019-04-05T04:07:40.846Z Reads: 38

```
I don't believe it's possible to make an unsensored motor move in the correct direction from standstill, there is always a 50-50 chance on initial direction based on how the magnets are aligned.
```

---
## \#12 Posted by: goffzh Posted at: 2019-04-05T04:26:34.604Z Reads: 36

```
I've been able to get dumber controllers like Simonk and MGM Compro tuned to start these high inertia loads very reliably sensorless so with all the parameters the VESC offers I expect it should be possible.
```

---
## \#13 Posted by: MysticalDork Posted at: 2019-04-05T05:49:10.052Z Reads: 30

```
You could always add some hall sensors to the motor. Either inside the case like OEMs do it (It's not that hard, I've done it to Ebike motors before), or with a bracket/PCB like [this](http://e0designs.com/products/hall-effect-sensor-board/) on the outside.
```

---
