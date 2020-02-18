# Current limiting issues

### Replies: 6 Views: 186

## \#1 Posted by: chrismccabe Posted at: 2018-12-02T16:53:19.682Z Reads: 78

```
Hey guys, I have a question hopefully one of you can help me with. I accidentally changed a few settings in VESC tool and all of a sudden my board seems to limit at 30A motor current. It stays hanging around 29.something. If I go full stick I see in the bluetooth app the motor current stays at 30A max.

When I go into VESC tool and look at the settings for max motor current en max battery current they are all set to a higher value. What is causing the motor current to max out at 30A (also the battery voltage sag is very minimal, so that also should be the problem.

My BMS should be capable of 60A (http://www.batterysupports.com/36v-37v-42v-10s-60a-10x-36v-lithium-ion-lipolymer-battery-bms-p-267.html)
```

---
## \#2 Posted by: taz Posted at: 2018-12-02T17:02:16.060Z Reads: 72

```
Single or double drive?
```

---
## \#3 Posted by: chrismccabe Posted at: 2018-12-02T17:09:09.319Z Reads: 67

```
Single drive, Maytech VESC, SK3 motor.
I used to defo pump way more amp through it. It would launch pretty insane. Now something is limiting the current at 30A.

I was looking to the remote controller settings and was wondering about it being set to 'current no reverse with brake'. How does the controller influence the actual output speed of the board in that (standard) mode. Is the PWM signal value translated to percentage of the max set current?
```

---
## \#4 Posted by: taz Posted at: 2018-12-02T17:10:09.275Z Reads: 60

```
Yes it is.
You have to set the endpoints on the vesc app.
```

---
## \#5 Posted by: chrismccabe Posted at: 2018-12-02T17:43:25.075Z Reads: 45

```
These were set but seem to be off now indeed. I did replace the receiver because my earlier Benchwheel receiver died. Damn! Such a simple fix... :confused: 
Wasn't the place I was looking.
I did a quick ride and all is good again. Thanks bro!!!

This does make me think about failsafe behaviour. What if the current sensor fails, could the board go into full throttle? (A bit of a side question)
```

---
## \#6 Posted by: mmaner Posted at: 2018-12-03T02:04:16.783Z Reads: 26

```
Check if you set max watts or changed duty cycle.
```

---
